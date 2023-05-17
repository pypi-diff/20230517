# Comparing `tmp/photutils-1.7.0.tar.gz` & `tmp/photutils-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photutils-1.7.0.tar", last modified: Thu Apr  6 03:10:21 2023, max compression
+gzip compressed data, was "photutils-1.8.0.tar", last modified: Wed May 17 18:27:07 2023, max compression
```

## Comparing `photutils-1.7.0.tar` & `photutils-1.8.0.tar`

### file list

```diff
@@ -1,314 +1,316 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.775234 photutils-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-06 03:10:01.000000 photutils-1.7.0/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.739234 photutils-1.7.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-06 03:10:01.000000 photutils-1.7.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.731234 photutils-1.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.739234 photutils-1.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-06 03:10:01.000000 photutils-1.7.0/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-06 03:10:01.000000 photutils-1.7.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-06 03:10:01.000000 photutils-1.7.0/.github/workflows/cron_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-06 03:10:01.000000 photutils-1.7.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-06 03:10:01.000000 photutils-1.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 03:10:01.000000 photutils-1.7.0/.lgtm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-06 03:10:01.000000 photutils-1.7.0/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-04-06 03:10:01.000000 photutils-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-06 03:10:01.000000 photutils-1.7.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    72373 2023-04-06 03:10:01.000000 photutils-1.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-06 03:10:01.000000 photutils-1.7.0/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-06 03:10:01.000000 photutils-1.7.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-06 03:10:01.000000 photutils-1.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-06 03:10:01.000000 photutils-1.7.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-06 03:10:01.000000 photutils-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-06 03:10:21.775234 photutils-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-06 03:10:01.000000 photutils-1.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-06 03:10:01.000000 photutils-1.7.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.743234 photutils-1.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.743234 photutils-1.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/_static/photutils.css
--rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/_static/photutils_banner-475x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/_static/photutils_banner.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    44248 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/_static/photutils_banner.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/_static/photutils_banner_original.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/_static/photutils_logo-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/_static/photutils_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/aperture.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/background.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/centroids.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/datasets.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/detection.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.743234 photutils-1.7.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/dev/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/epsf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/geometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/grouping.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/isophote.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/isophote_faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/morphology.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/pixel_conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/profiles.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28319 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_matching.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.747234 photutils-1.7.0/docs/psf_spec/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/background_estimator.rst
--rw-r--r--   0 runner    (1001) docker     (123)   472207 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/block_diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/block_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/culler_and_ender.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/finder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/fitter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/group_maker.rst
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/noise_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/psf_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/scene_maker.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/psf_spec/single_object_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/rtd_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26053 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/test_function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.747234 photutils-1.7.0/docs/whats_new/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/whats_new/1.1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/whats_new/1.2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/whats_new/1.3.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/whats_new/1.4.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/whats_new/1.5.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/whats_new/1.6.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/whats_new/1.7.rst
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-06 03:10:01.000000 photutils-1.7.0/docs/whats_new/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.747234 photutils-1.7.0/photutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-06 03:10:21.000000 photutils-1.7.0/photutils/_compiler.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.751234 photutils-1.7.0/photutils/aperture/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)    31482 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    21642 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23768 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    57922 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.751234 photutils-1.7.0/photutils/aperture/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/test_aperture_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/test_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/test_circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/test_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    32220 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/test_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/aperture/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.751234 photutils-1.7.0/photutils/background/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28361 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/background/background_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    23895 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/background/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/background/interpolators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.755234 photutils-1.7.0/photutils/background/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/background/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/background/tests/test_background_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/background/tests/test_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.755234 photutils-1.7.0/photutils/centroids/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/centroids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/centroids/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/centroids/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.755234 photutils-1.7.0/photutils/centroids/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/centroids/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/centroids/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/centroids/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.755234 photutils-1.7.0/photutils/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/datasets/load.py
--rw-r--r--   0 runner    (1001) docker     (123)    32633 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/datasets/make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.755234 photutils-1.7.0/photutils/datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/datasets/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/datasets/tests/test_make.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.755234 photutils-1.7.0/photutils/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    25269 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/daofinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/irafstarfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/peakfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/starfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.755234 photutils-1.7.0/photutils/detection/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.759234 photutils-1.7.0/photutils/detection/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm02.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm02.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm02.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.5.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm02.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/test_daofinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/test_irafstarfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/test_peakfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/detection/tests/test_starfinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.759234 photutils-1.7.0/photutils/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.759234 photutils-1.7.0/photutils/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/circular_overlap.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/core.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/core.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/elliptical_overlap.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/rectangular_overlap.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.759234 photutils-1.7.0/photutils/geometry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/tests/test_circular_overlap_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/tests/test_elliptical_overlap_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/geometry/tests/test_rectangular_overlap_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.763234 photutils-1.7.0/photutils/isophote/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/isophote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.763234 photutils-1.7.0/photutils/isophote/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.763234 photutils-1.7.0/photutils/isophote/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/data/M51_table.fits
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/data/minimum_radius_test.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/data/synth_highsnr_table.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/data/synth_lowsnr_table.fits
--rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/data/synth_table.fits
--rw-r--r--   0 runner    (1001) docker     (123)    80640 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/data/synth_table_mean.fits
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/data/synth_table_mean.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/make_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_isophote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/isophote/tests/test_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.763234 photutils-1.7.0/photutils/morphology/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/morphology/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/morphology/non_parametric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.767234 photutils-1.7.0/photutils/morphology/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/morphology/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/morphology/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/morphology/tests/test_non_parametric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.767234 photutils-1.7.0/photutils/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/profiles/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/profiles/curve_of_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/profiles/radial_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.767234 photutils-1.7.0/photutils/profiles/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/profiles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/profiles/tests/test_curve_of_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/profiles/tests/test_radial_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.767234 photutils-1.7.0/photutils/psf/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/epsf.py
--rw-r--r--   0 runner    (1001) docker     (123)    27025 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/epsf_stars.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/groupstars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.767234 photutils-1.7.0/photutils/psf/matching/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/matching/fourier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.767234 photutils-1.7.0/photutils/psf/matching/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/matching/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/matching/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/matching/tests/test_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/matching/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)    42935 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    51286 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/photometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.771234 photutils-1.7.0/photutils/psf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/tests/test_epsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/tests/test_epsf_stars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/tests/test_groupstars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14981 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    37009 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/tests/test_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/psf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.771234 photutils-1.7.0/photutils/segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   134870 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    54487 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    23336 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/deblend.py
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.771234 photutils-1.7.0/photutils/segmentation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36580 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13443 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/tests/test_deblend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/tests/test_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/segmentation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.771234 photutils-1.7.0/photutils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.775234 photutils-1.7.0/photutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_optional_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_quantity_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_round.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/_wcs_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/cutouts.py
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/footprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/interpolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.775234 photutils-1.7.0/photutils/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_cutouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_depths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_footprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-06 03:10:01.000000 photutils-1.7.0/photutils/utils/tests/test_quantity_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-06 03:10:21.000000 photutils-1.7.0/photutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 03:10:21.751234 photutils-1.7.0/photutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-06 03:10:21.000000 photutils-1.7.0/photutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-04-06 03:10:21.000000 photutils-1.7.0/photutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 03:10:21.000000 photutils-1.7.0/photutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 03:10:21.000000 photutils-1.7.0/photutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-06 03:10:21.000000 photutils-1.7.0/photutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 03:10:21.000000 photutils-1.7.0/photutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-06 03:10:01.000000 photutils-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-06 03:10:21.779234 photutils-1.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2193 2023-04-06 03:10:01.000000 photutils-1.7.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-04-06 03:10:01.000000 photutils-1.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.970378 photutils-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 18:26:37.000000 photutils-1.8.0/.bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.858373 photutils-1.8.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-17 18:26:37.000000 photutils-1.8.0/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.834372 photutils-1.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.858373 photutils-1.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/32bit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/cron_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-17 18:26:37.000000 photutils-1.8.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-17 18:26:37.000000 photutils-1.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 18:26:37.000000 photutils-1.8.0/.lgtm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 18:26:37.000000 photutils-1.8.0/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-17 18:26:37.000000 photutils-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-17 18:26:37.000000 photutils-1.8.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    73988 2023-05-17 18:26:37.000000 photutils-1.8.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 18:26:37.000000 photutils-1.8.0/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 18:26:37.000000 photutils-1.8.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-05-17 18:26:37.000000 photutils-1.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-17 18:26:37.000000 photutils-1.8.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-17 18:26:37.000000 photutils-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-17 18:27:07.970378 photutils-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-17 18:26:37.000000 photutils-1.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-17 18:26:37.000000 photutils-1.8.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.870373 photutils-1.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.874374 photutils-1.8.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20779 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_banner-475x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_banner.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    44248 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_banner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_banner_original.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_logo-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/_static/photutils_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/aperture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/background.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/centroids.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/detection.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.874374 photutils-1.8.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/dev/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/epsf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/grouping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/isophote.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/isophote_faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/morphology.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/pixel_conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/profiles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28319 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_matching.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.882374 photutils-1.8.0/docs/psf_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/background_estimator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   472207 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/block_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/block_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/culler_and_ender.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/finder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/fitter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/group_maker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/noise_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/psf_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/scene_maker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/psf_spec/single_object_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/rtd_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/test_function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.886374 photutils-1.8.0/docs/whats_new/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.4.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.5.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.6.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.7.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/1.8.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-17 18:26:37.000000 photutils-1.8.0/docs/whats_new/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.886374 photutils-1.8.0/photutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils/_compiler.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.894374 photutils-1.8.0/photutils/aperture/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30661 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21642 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23768 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57981 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.898375 photutils-1.8.0/photutils/aperture/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_aperture_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32220 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/aperture/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.898375 photutils-1.8.0/photutils/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28240 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/background_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23895 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/interpolators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.902375 photutils-1.8.0/photutils/background/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/tests/test_background_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/background/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.902375 photutils-1.8.0/photutils/centroids/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18869 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.906375 photutils-1.8.0/photutils/centroids/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/centroids/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.906375 photutils-1.8.0/photutils/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32633 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.906375 photutils-1.8.0/photutils/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/datasets/tests/test_make.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.910375 photutils-1.8.0/photutils/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25269 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/daofinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/irafstarfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/peakfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/starfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.910375 photutils-1.8.0/photutils/detection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.918375 photutils-1.8.0/photutils/detection/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm02.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm02.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm02.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm02.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/test_daofinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/test_irafstarfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/test_peakfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/detection/tests/test_starfinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.918375 photutils-1.8.0/photutils/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.918375 photutils-1.8.0/photutils/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/circular_overlap.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/core.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/elliptical_overlap.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/rectangular_overlap.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.922376 photutils-1.8.0/photutils/geometry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/tests/test_circular_overlap_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/tests/test_elliptical_overlap_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/geometry/tests/test_rectangular_overlap_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.926376 photutils-1.8.0/photutils/isophote/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16995 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29450 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/isophote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.930376 photutils-1.8.0/photutils/isophote/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.934376 photutils-1.8.0/photutils/isophote/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/M51_table.fits
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/minimum_radius_test.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_highsnr_table.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_lowsnr_table.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    28800 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_table.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    80640 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_table_mean.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/data/synth_table_mean.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/make_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_harmonics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_isophote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/isophote/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.934376 photutils-1.8.0/photutils/morphology/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/non_parametric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.938376 photutils-1.8.0/photutils/morphology/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/morphology/tests/test_non_parametric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.938376 photutils-1.8.0/photutils/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10764 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/curve_of_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/radial_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.942376 photutils-1.8.0/photutils/profiles/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/tests/test_curve_of_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/profiles/tests/test_radial_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.942376 photutils-1.8.0/photutils/psf/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/epsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27025 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/epsf_stars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/groupstars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.946376 photutils-1.8.0/photutils/psf/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/fourier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.946376 photutils-1.8.0/photutils/psf/matching/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/tests/test_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/matching/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42730 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51286 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/photometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.950377 photutils-1.8.0/photutils/psf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_epsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_epsf_stars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_groupstars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37009 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/psf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.954377 photutils-1.8.0/photutils/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135232 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52595 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/deblend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.954377 photutils-1.8.0/photutils/segmentation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36763 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_deblend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/segmentation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.958377 photutils-1.8.0/photutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.962377 photutils-1.8.0/photutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_optional_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_quantity_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_round.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/_wcs_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/cutouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/footprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/interpolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.970378 photutils-1.8.0/photutils/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_cutouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_depths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_footprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-17 18:26:37.000000 photutils-1.8.0/photutils/utils/tests/test_quantity_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:27:07.890374 photutils-1.8.0/photutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 18:27:07.000000 photutils-1.8.0/photutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-17 18:26:37.000000 photutils-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-17 18:27:07.970378 photutils-1.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2193 2023-05-17 18:26:37.000000 photutils-1.8.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-17 18:26:37.000000 photutils-1.8.0/tox.ini
```

### Comparing `photutils-1.7.0/.github/workflows/ci_tests.yml` & `photutils-1.8.0/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/.github/workflows/codeql.yml` & `photutils-1.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/.github/workflows/cron_tests.yml` & `photutils-1.8.0/.github/workflows/cron_tests.yml`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/.github/workflows/publish.yml` & `photutils-1.8.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/.gitignore` & `photutils-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/.pre-commit-config.yaml` & `photutils-1.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/CHANGES.rst` & `photutils-1.8.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,71 @@
+1.8.0 (2023-05-17)
+------------------
+
+General
+^^^^^^^
+
+- The minimum required Numpy is now 1.21. [#1528]
+
+- The minimum required Scipy is now 1.7.0. [#1528]
+
+- The minimum required Matplotlib is now 3.5.0. [#1528]
+
+- The minimum required scikit-image is now 0.19.0. [#1528]
+
+- The minimum required gwcs is now 0.18. [#1528]
+
+New Features
+^^^^^^^^^^^^
+
+- ``photutils.profiles``
+
+  - The ``RadialProfile`` and ``CurveOfGrowth`` radial bins can now be
+    directly input, which also allows for non-uniform radial spacing.
+    [#1540]
+
+Bug Fixes
+^^^^^^^^^
+
+- ``photutils.psf``
+
+  - Fixed an issue with the local model cache in ``GriddedPSFModel``,
+    significantly improving performance. [#1536]
+
+API Changes
+^^^^^^^^^^^
+
+- Removed the deprecated ``axes`` keyword in favor of ``ax`` for
+  consistency with other packages. [#1523]
+
+- ``photutils.aperture``
+
+  - Removed the ``ApertureStats`` ``unpack_nddata`` method. [#1537]
+
+- ``photutils.profiles``
+
+  - The API for defining the radial bins for the ``RadialProfile`` and
+    ``CurveOfGrowth`` classes was changed. While the new API allows for
+    more flexibility, unfortunately, it is not backwards-compatible.
+    [#1540]
+
+- ``photutils.segmentation``
+
+  - Removed the deprecated ``kernel`` keyword from ``detect_sources``
+    and ``deblend_sources``. [#1524]
+
+  - Deprecated the ``kernel`` keyword in ``SourceCatalog``. [#1525]
+
+  - Removed the deprecated ``outline_segments`` method from
+    ``SegmentationImage``. [#1526]
+
+  - The ``SourceCatalog`` ``kron_params`` attribute is no longer
+    returned as a ``ndarray``. It is returned as a ``tuple``. [#1531]
+
+
 1.7.0 (2023-04-05)
 ------------------
 
 General
 ^^^^^^^
 
 - The ``rasterio`` and ``shapely`` packages are now optional
```

### Comparing `photutils-1.7.0/CONTRIBUTING.rst` & `photutils-1.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/LICENSE.rst` & `photutils-1.8.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/PKG-INFO` & `photutils-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photutils
-Version: 1.7.0
+Version: 1.8.0
 Summary: An Astropy package for source detection and photometry
 Home-page: https://github.com/astropy/photutils
 Author: Photutils Developers
 Author-email: photutils.team@gmail.com
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,photometry,aperture,psf,source detection,background,segmentation,centroids,isophote,morphology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `photutils-1.7.0/README.rst` & `photutils-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/Makefile` & `photutils-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/_static/favicon.ico` & `photutils-1.8.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/_static/photutils_banner-475x120.png` & `photutils-1.8.0/docs/_static/photutils_banner-475x120.png`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/_static/photutils_banner.pdf` & `photutils-1.8.0/docs/_static/photutils_banner.pdf`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/_static/photutils_banner.svg` & `photutils-1.8.0/docs/_static/photutils_banner.svg`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/_static/photutils_banner_original.svg` & `photutils-1.8.0/docs/_static/photutils_banner_original.svg`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/_static/photutils_logo-32x32.png` & `photutils-1.8.0/docs/_static/photutils_logo-32x32.png`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/_static/photutils_logo.svg` & `photutils-1.8.0/docs/_static/photutils_logo.svg`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/aperture.rst` & `photutils-1.8.0/docs/aperture.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/background.rst` & `photutils-1.8.0/docs/background.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Background Estimation (`photutils.background`)
 ==============================================
 
 Introduction
 ------------
 
-To accurately measure the photometry and morphological properties of
-astronomical sources, one requires an accurate estimate of the
-background, which can be from both the sky and the detector.
-Similarly, having an accurate estimate of the background noise is
-important for determining the significance of source detections and
-for estimating photometric errors.
-
-Unfortunately, accurate background and background noise estimation is
-a difficult task.  Further, because astronomical images can cover a
-wide variety of scenes, there is not a single background estimation
-method that will always be applicable. Photutils provides tools for
-estimating the background and background noise in your data, but they
-will likely require some tweaking to optimize the background estimate
-for your data.
+To accurately measure the photometry and morphological properties
+of astronomical sources, one requires an accurate estimate of the
+background, which can be from both the sky and the detector. Similarly,
+having an accurate estimate of the background noise is important for
+determining the significance of source detections and for estimating
+photometric errors.
+
+Unfortunately, accurate background and background noise estimation is a
+difficult task. Further, because astronomical images can cover a wide
+variety of scenes, there is not a single background estimation method
+that will always be applicable. Photutils provides tools for estimating
+the background and background noise in your data, but they will likely
+require some tweaking to optimize the background estimate for your data.
 
 
 Scalar Background and Noise Estimation
 --------------------------------------
 
 Simple Statistics
 ^^^^^^^^^^^^^^^^^
 
 If the background level and noise are relatively constant across an
 image, the simplest way to estimate these values is to derive scalar
-quantities using simple approximations.  Of course, when computing the
-image statistics one must take into account the astronomical sources
-present in the images, which add a positive tail to the distribution
-of pixel intensities. For example, one may consider using the image
-median as the background level and the image standard deviation as the
-1-sigma background noise, but the resulting values are obviously
-biased by the presence of real sources.
-
-A slightly better method involves using statistics that are robust
-against the presence of outliers, such as the biweight location for
-the background level and biweight scale or `median absolute deviation
-(MAD) <https://en.wikipedia.org/wiki/Median_absolute_deviation>`__ for
-the background noise estimation. However, for most astronomical scenes
-these methods will also be biased by the presence of astronomical
-sources in the image.
+quantities using simple approximations. When computing the image
+statistics one must take into account the astronomical sources present
+in the images, which add a positive tail to the distribution of pixel
+intensities. For example, one may consider using the image median as
+the background level and the image standard deviation as the 1-sigma
+background noise, but the resulting values are biased by the presence of
+real sources.
+
+A slightly better method involves using statistics that
+are robust against the presence of outliers, such as the
+biweight location for the background level and biweight
+scale or normalized `median absolute deviation (MAD)
+<https://en.wikipedia.org/wiki/Median_absolute_deviation>`__ for the
+background noise estimation. However, for most astronomical scenes these
+methods will also be biased by the presence of astronomical sources in
+the image.
 
 As an example, we load a synthetic image comprised of 100 sources with
 a Gaussian-distributed background whose mean is 5 and standard
 deviation is 2::
 
     >>> from photutils.datasets import make_100gaussians_image
     >>> data = make_100gaussians_image()
@@ -94,36 +94,35 @@
     2.1443760096598914
 
 
 Sigma Clipping Sources
 ^^^^^^^^^^^^^^^^^^^^^^
 
 The most widely used technique to remove the sources from the image
-statistics is called sigma clipping.  Briefly, pixels that are above
-or below a specified sigma level from the median are discarded and the
-statistics are recalculated.  The procedure is typically repeated over
-a number of iterations or until convergence is reached.  This method
+statistics is called sigma clipping. Briefly, pixels that are above or
+below a specified sigma level from the median are discarded and the
+statistics are recalculated. The procedure is typically repeated over
+a number of iterations or until convergence is reached. This method
 provides a better estimate of the background and background noise
 levels::
 
     >>> from astropy.stats import sigma_clipped_stats
     >>> mean, median, std = sigma_clipped_stats(data, sigma=3.0)
     >>> print((mean, median, std))  # doctest: +FLOAT_CMP
     (5.199138651621793, 5.155587433358291, 2.094275212132969)
 
 
 Masking Sources
 ^^^^^^^^^^^^^^^
 
 An even better procedure is to exclude the sources in the image by
-masking them. Of course, this technique requires one to :ref:`identify
-the sources in the data <source_detection>`, which in turn depends
-on the background and background noise. Therefore, this method for
-estimating the background and background RMS requires an iterative
-procedure.
+masking them. This technique requires one to :ref:`identify the sources
+in the data <source_detection>`, which in turn depends on the background
+and background noise. Therefore, this method for estimating the
+background and background RMS requires an iterative procedure.
 
 One method to create a source mask is to use a
 :ref:`segmentation image <image_segmentation>`. Here we use the
 `~photutils.segmentation.detect_threshold` convenience function to get a
 rough estimate of the threshold at the 2-sigma background noise level.
 Then we use the `~photutils.segmentation.detect_sources` function to
 generate a `~photutils.segmentation.SegmentationImage`. Finally, we use
@@ -140,32 +139,32 @@
     >>> segment_img = detect_sources(data, threshold, npixels=10)
     >>> footprint = circular_footprint(radius=10)
     >>> mask = segment_img.make_source_mask(footprint=footprint)
     >>> mean, median, std = sigma_clipped_stats(data, sigma=3.0, mask=mask)
     >>> print((mean, median, std))  # doctest: +FLOAT_CMP
     (4.994042038715669, 4.991333562774164, 1.9699473426119296)
 
-Of course, the source detection and masking procedure can be iterated
-further. Even with one iteration we are within 0.2% of the true
-background value and 1.5% of the true background RMS.
+The source detection and masking procedure can be iterated further. Even
+with one iteration we are within 0.2% of the true background value and
+1.5% of the true background RMS.
 
 .. _scipy: https://www.scipy.org/
 
 
 2D Background and Noise Estimation
 ----------------------------------
 
 If the background or the background noise varies across the image,
 then you will generally want to generate a 2D image of the background
-and background RMS (or compute these values locally).  This can be
+and background RMS (or compute these values locally). This can be
 accomplished by applying the above techniques to subregions of the
-image.  A common procedure is to use sigma-clipped statistics in each
+image. A common procedure is to use sigma-clipped statistics in each
 mesh of a grid that covers the input data to create a low-resolution
-background image.  The final background or background RMS image can
-then be generated by interpolating the low-resolution image.
+background image. The final background or background RMS image can then
+be generated by interpolating the low-resolution image.
 
 Photutils provides the :class:`~photutils.background.Background2D`
 class to estimate the 2D background and background noise in an
 astronomical image. :class:`~photutils.background.Background2D`
 requires the size of the box (``box_size``) in which to estimate the
 background.  Selecting the box size requires some care by the user.
 The box size should generally be larger than the typical size of
@@ -189,40 +188,39 @@
 * `~photutils.background.BiweightLocationBackground`
 
 The default is a `~photutils.background.SExtractorBackground` instance.
 For this method, the background in each mesh is calculated as ``(2.5 *
 median) - (1.5 * mean)``. However, if ``(mean - median) / std > 0.3``
 then the ``median`` is used instead.
 
-Likewise, the background RMS level in each mesh is calculated using
-the function or callable object input via the ``bkgrms_estimator``
-keyword.  Photutils provides the following classes for this purpose:
+Likewise, the background RMS level in each mesh is calculated using the
+function or callable object input via the ``bkgrms_estimator`` keyword.
+Photutils provides the following classes for this purpose:
 
 * `~photutils.background.StdBackgroundRMS`
 * `~photutils.background.MADStdBackgroundRMS`
 * `~photutils.background.BiweightScaleBackgroundRMS`
 
 For even more flexibility, users may input a custom function or
 callable object to the ``bkg_estimator`` and/or ``bkgrms_estimator``
 keywords.
 
-By default, the ``bkg_estimator`` and ``bkgrms_estimator`` are applied
-to sigma clipped data.  Sigma clipping is defined by inputting a
-:class:`astropy.stats.SigmaClip` object to the ``sigma_clip`` keyword.
-The default is to perform sigma clipping with ``sigma=3`` and
-``maxiters=10``.  Sigma clipping can be turned off by setting
+By default, the ``bkg_estimator`` and ``bkgrms_estimator`` are
+applied to sigma clipped data. Sigma clipping is defined by inputting
+a :class:`astropy.stats.SigmaClip` object to the ``sigma_clip``
+keyword. The default is to perform sigma clipping with ``sigma=3``
+and ``maxiters=10``. Sigma clipping can be turned off by setting
 ``sigma_clip=None``.
 
-After the background level has been determined in each of the boxes,
-the low-resolution background image can be median filtered, with a
-window of size of ``filter_size``, to suppress local under- or
-overestimations (e.g., due to bright galaxies in a particular box).
-Likewise, the median filter can be applied only to those boxes where
-the background level is above a specified threshold
-(``filter_threshold``).
+After the background level has been determined in each of the boxes, the
+low-resolution background image can be median filtered, with a window
+of size of ``filter_size``, to suppress local under- or overestimations
+(e.g., due to bright galaxies in a particular box). Likewise, the median
+filter can be applied only to those boxes where the background level is
+above a specified threshold (``filter_threshold``).
 
 The low-resolution background and background RMS images are resized to
 the original data size using the function or callable object
 input via the ``interpolator`` keyword.  Photutils provides two
 interpolator classes:
 :class:`~photutils.background.BkgZoomInterpolator` (default), which
 performs spline interpolation, and
@@ -270,20 +268,19 @@
     >>> bkg_estimator = MedianBackground()
     >>> bkg = Background2D(data2, (50, 50), filter_size=(3, 3),
     ...                    sigma_clip=sigma_clip, bkg_estimator=bkg_estimator)
 
 
 The 2D background and background RMS images are retrieved using the
 ``background`` and ``background_rms`` attributes, respectively, on the
-returned object.  The low-resolution versions of these images are
-stored in the ``background_mesh`` and ``background_rms_mesh``
-attributes, respectively.   The global median value of the
-low-resolution background and background RMS image can be accessed
-with the ``background_median`` and ``background_rms_median``
-attributes, respectively:
+returned object. The low-resolution versions of these images are stored
+in the ``background_mesh`` and ``background_rms_mesh`` attributes,
+respectively. The global median value of the low-resolution background
+and background RMS image can be accessed with the ``background_median``
+and ``background_rms_median`` attributes, respectively:
 
 .. doctest-requires:: scipy
 
     >>> print(bkg.background_median)  # doctest: +FLOAT_CMP
     10.821997862561792
     >>> print(bkg.background_rms_median)  # doctest: +FLOAT_CMP
     2.298820539683762
@@ -486,15 +483,16 @@
 
 Plotting Meshes
 ^^^^^^^^^^^^^^^
 
 Finally, the meshes that were used in generating the 2D
 background can be plotted on the original image using the
 :meth:`~photutils.background.Background2D.plot_meshes` method. Here we
-zoom in on a small portion of the image to show the background meshes:
+zoom in on a small portion of the image to show the background meshes.
+Meshes without a center marker were excluded.
 
 .. doctest-skip::
 
     >>> plt.imshow(data3, origin='lower', cmap='Greys_r', norm=norm,
     ...            interpolation='nearest')
     >>> bkg3.plot_meshes(outlines=True, marker='.', color='cyan', alpha=0.3)
     >>> plt.xlim(0, 250)
```

### Comparing `photutils-1.7.0/docs/centroids.rst` & `photutils-1.8.0/docs/centroids.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/conf.py` & `photutils-1.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/contributing.rst` & `photutils-1.8.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/datasets.rst` & `photutils-1.8.0/docs/datasets.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/detection.rst` & `photutils-1.8.0/docs/detection.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,52 +4,57 @@
 ========================================
 
 Introduction
 ------------
 
 One generally needs to identify astronomical sources in their data
 before they can perform photometry or morphological measurements.
-Photutils provides two functions designed specifically to detect
-point-like (stellar) sources in an astronomical image.  Photutils also
-provides a function to identify local peaks in an image that are above
-a specified threshold value.
+Photutils provides several tools designed specifically to detect
+point-like (stellar) sources in an astronomical image. Photutils also
+provides a function to identify local peaks in an image that are above a
+specified threshold value.
 
 For general-use source detection and extraction of both point-like
 and extended sources, please see :ref:`Image Segmentation
 <image_segmentation>`.
 
 
 Detecting Stars
 ---------------
 
 Photutils includes two widely-used tools that are used to detect stars
-in an image, `DAOFIND`_ and IRAF's `starfind`_.
+in an image, `DAOFIND`_ and IRAF's `starfind`_, plus a third tool that
+allows input of a custom user-defined kernel.
 
-:class:`~photutils.detection.DAOStarFinder` is a class that provides
-an implementation of the `DAOFIND`_ algorithm (`Stetson 1987, PASP 99,
-191
+:class:`~photutils.detection.DAOStarFinder` is a class that provides an
+implementation of the `DAOFIND`_ algorithm (`Stetson 1987, PASP 99, 191
 <https://ui.adsabs.harvard.edu/abs/1987PASP...99..191S/abstract>`_).
 It searches images for local density maxima that have a peak amplitude
 greater than a specified threshold (the threshold is applied to a
 convolved image) and have a size and shape similar to a defined 2D
-Gaussian kernel.  :class:`~photutils.detection.DAOStarFinder` also
+Gaussian kernel. :class:`~photutils.detection.DAOStarFinder` also
 provides an estimate of the objects' roundness and sharpness, whose
 lower and upper bounds can be specified.
 
 :class:`~photutils.detection.IRAFStarFinder` is a class that
-implements IRAF's `starfind`_ algorithm.  It is fundamentally similar
-to :class:`~photutils.detection.DAOStarFinder`, but
-:class:`~photutils.detection.DAOStarFinder` can use an elliptical
-Gaussian kernel. One other difference in
+implements IRAF's `starfind`_ algorithm. It is fundamentally
+similar to :class:`~photutils.detection.DAOStarFinder`,
+but :class:`~photutils.detection.DAOStarFinder` can use
+an elliptical Gaussian kernel. One other difference in
 :class:`~photutils.detection.IRAFStarFinder` is that it calculates the
 objects' centroid, roundness, and sharpness using image moments.
 
-As an example, let's load an image from the bundled datasets and
-select a subset of the image.  We will estimate the background and
-background noise using sigma-clipped statistics::
+:class:`~photutils.detection.StarFinder` is a class similar to
+:class:`~photutils.detection.IRAFStarFinder`, but which allows input
+of a custom user-defined kernel as a 2D array. This allows for more
+generalization beyond simple Gaussian kernels.
+
+As an example, let's load an image from the bundled datasets and select
+a subset of the image. We will estimate the background and background
+noise using sigma-clipped statistics::
 
     >>> from astropy.stats import sigma_clipped_stats
     >>> from photutils.datasets import load_star_image
     >>> hdu = load_star_image()  # doctest: +REMOTE_DATA
     >>> data = hdu.data[0:401, 0:401]  # doctest: +REMOTE_DATA
     >>> mean, median, std = sigma_clipped_stats(data, sigma=3.0)  # doctest: +REMOTE_DATA
     >>> print((mean, median, std))  # doctest: +REMOTE_DATA, +FLOAT_CMP
@@ -140,17 +145,14 @@
 
    >>> from photutils.detection import DAOStarFinder
    >>> daofind = DAOStarFinder(fwhm=3.0, threshold=5.0 * std)
    >>> mask = np.zeros(data.shape, dtype=bool)
    >>> mask[50:151, 50:351] = True
    >>> mask[250:351, 150:351] = True
    >>> sources = daofind(data - median, mask=mask)
-   >>> for col in sources.colnames:
-   >>>     sources[col].info.format = '%.8g'  # for consistent table output
-   >>> print(sources)
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
     from astropy.stats import sigma_clipped_stats
     from astropy.visualization import SqrtStretch
@@ -181,28 +183,23 @@
 
 
 Local Peak Detection
 --------------------
 
 Photutils also includes a :func:`~photutils.detection.find_peaks`
 function to find local peaks in an image that are above a specified
-threshold value. Peaks are the local maxima above a specified
-threshold that are separated by a specified minimum number of pixels.
-
-By default, the returned pixel coordinates are always integer-valued
-(i.e., no centroiding is performed, only the peak pixel is
-identified).  However, a centroiding function can be input via the
-``centroid_func`` keyword to :func:`~photutils.detection.find_peaks`
-to compute centroid coordinates with subpixel precision.
-
-:func:`~photutils.detection.find_peaks` supports a number of
-additional options, including searching for peaks only within a
-specified footprint.  Please see the
-:func:`~photutils.detection.find_peaks` documentation for more
-options.
+threshold value. Peaks are the local maxima above a specified threshold
+that are separated by a specified minimum number of pixels, defined by a
+box size or a local footprint.
+
+The returned pixel coordinates for the peaks are always integer-valued
+(i.e., no centroiding is performed, only the peak pixel is identified).
+However, a centroiding function can be input via the ``centroid_func``
+keyword to :func:`~photutils.detection.find_peaks` to also compute
+centroid coordinates with subpixel precision.
 
 As a simple example, let's find the local peaks in an image that are 5
 sigma above the background and a separated by at least 5 pixels:
 
 .. doctest-requires:: scipy
 
     >>> from astropy.stats import sigma_clipped_stats
```

### Comparing `photutils-1.7.0/docs/dev/releasing.rst` & `photutils-1.8.0/docs/dev/releasing.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/epsf.rst` & `photutils-1.8.0/docs/epsf.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/getting_started.rst` & `photutils-1.8.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/grouping.rst` & `photutils-1.8.0/docs/grouping.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Grouping Algorithms
-===================
+Star Grouping Algorithms
+========================
 
 Introduction
 ------------
 
-In Point Spread Function (PSF) photometry, a grouping algorithm is
-used to separate stars into optimum groups.  The stars in each group
-are defined as those close enough together such that they need to be
-fit simultaneously, i.e., their profiles overlap.
+In Point Spread Function (PSF) photometry, a grouping algorithm is used
+to separate stars into optimum groups. The stars in each group are
+defined as those close enough together such that they need to be fit
+simultaneously, i.e., their profiles overlap.
 
 Photutils currently provides two classes to group stars:
 
   * :class:`~photutils.psf.DAOGroup`:  An implementation of the
     `DAOPHOT
     <https://ui.adsabs.harvard.edu/abs/1987PASP...99..191S/abstract>`_
     GROUP algorithm.
@@ -24,20 +24,19 @@
 DAOPHOT GROUP
 -------------
 
 Stetson, in his seminal paper (`Stetson 1987, PASP 99, 191
 <https://ui.adsabs.harvard.edu/abs/1987PASP...99..191S/abstract>`_),
 provided a simple and powerful grouping algorithm to decide whether
 the profile of a given star extends into the fitting region of any
-other star.  Stetson defines this in terms of a "critical separation"
+other star. Stetson defines this in terms of a "critical separation"
 parameter, which is defined as the minimal distance that any two stars
-must be separated by in order to be in different groups.  Stetson
-gives intuitive reasoning to suggest that the critical separation may
-be defined as a multiple of the stellar full width at half maximum
-(FWHM).
+must be separated by in order to be in different groups. Stetson gives
+intuitive reasoning to suggest that the critical separation may be
+defined as a multiple of the stellar full width at half maximum (FWHM).
 
 Photutils provides an implementation of the DAOPHOT GROUP algorithm in
 the :class:`~photutils.psf.DAOGroup` class. Let's take a look at a
 simple example.
 
 First, let's make some Gaussian sources using
 `~photutils.datasets.make_random_gaussians_table` and
@@ -79,19 +78,19 @@
 Here we rename ``x_mean`` to ``x_0`` and ``y_mean`` to ``y_0``:
 
 .. doctest-skip::
 
     >>> starlist['x_mean'].name = 'x_0'
     >>> starlist['y_mean'].name = 'y_0'
 
-Now, let's find the stellar groups.  We start by creating a
-`~photutils.psf.DAOGroup` object.  Here we set its ``crit_separation``
+Now, let's find the stellar groups. We start by creating a
+`~photutils.psf.DAOGroup` object. Here we set its ``crit_separation``
 parameter ``2.5 * fwhm``, where the stellar ``fwhm`` was defined above
-when we created the stars as 2D Gaussians.  In general one will need
-to measure the FWHM of the stellar profiles.
+when we created the stars as 2D Gaussians. In general one will need to
+measure the FWHM of the stellar profiles.
 
 .. doctest-skip::
 
     >>> from astropy.stats import gaussian_sigma_to_fwhm
     >>> from photutils.psf.groupstars import DAOGroup
     >>> fwhm = sigma_psf * gaussian_sigma_to_fwhm
     >>> daogroup = DAOGroup(crit_separation=2.5 * fwhm)
@@ -100,18 +99,18 @@
 as a calling function that receives as input a table of stars (e.g.,
 ``starlist``):
 
 .. doctest-skip::
 
     >>> star_groups = daogroup(starlist)
 
-The ``star_groups`` output is copy of the input ``starlist`` table,
-but with an extra column called ``group_id``.  This column contains
-integers that represent the group assigned to each source.  Here the
-grouping algorithm separated the 350 stars into 92 distinct groups:
+The ``star_groups`` output is copy of the input ``starlist`` table, but
+with an extra column called ``group_id``. This column contains integers
+that represent the group assigned to each source. Here the grouping
+algorithm separated the 350 stars into 92 distinct groups:
 
 .. doctest-skip::
 
     >>> print(max(star_groups['group_id']))
     92
 
 One can use the ``group_by`` functionality from `~astropy.table.Table`
@@ -198,26 +197,26 @@
         ap = CircularAperture(xypos, r=fwhm)
         ap.plot(color=cmap.colors[i])
 
 
 DBSCANGroup
 -----------
 
-Photutils also provides a :class:`~photutils.psf.DBSCANGroup` class to
-group stars based on the `Density-Based Spatial Clustering of
-Applications with Noise (DBSCAN)
+Photutils also provides a :class:`~photutils.psf.DBSCANGroup`
+class to group stars based on the `Density-Based
+Spatial Clustering of Applications with Noise (DBSCAN)
 <https://en.wikipedia.org/wiki/DBSCAN>`_ algorithm.
 :class:`~photutils.psf.DBSCANGroup` provides a more general algorithm
 than :class:`~photutils.psf.DAOGroup`.
 
 Here's a simple example using :class:`~photutils.psf.DBSCANGroup` with
-``min_samples=1`` and ``metric=euclidean``.  With these parameters,
-the result is identical to the `~photutils.psf.DAOGroup` algorithm.
-Note that `scikit-learn <https://scikit-learn.org/>`_ must be installed
-to use :class:`~photutils.psf.DBSCANGroup`.
+``min_samples=1`` and ``metric=euclidean``. With these parameters, the
+result is identical to the `~photutils.psf.DAOGroup` algorithm. Note
+that `scikit-learn <https://scikit-learn.org/>`_ must be installed to
+use :class:`~photutils.psf.DBSCANGroup`.
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
     from astropy.stats import gaussian_sigma_to_fwhm
     from matplotlib import rcParams
```

### Comparing `photutils-1.7.0/docs/install.rst` & `photutils-1.8.0/docs/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 Requirements
 ============
 
 Photutils has the following strict requirements:
 
 * `Python <https://www.python.org/>`_ 3.8 or later
 
-* `Numpy <https://numpy.org/>`_ 1.20 or later
+* `Numpy <https://numpy.org/>`_ 1.21 or later
 
 * `Astropy`_ 5.0 or later
 
 Photutils also optionally depends on other packages for some features:
 
-* `Scipy <https://www.scipy.org/>`_ 1.6.0 or later:  To power a variety of
+* `Scipy <https://www.scipy.org/>`_ 1.7.0 or later:  To power a variety of
   features in several modules (strongly recommended).
 
-* `matplotlib <https://matplotlib.org/>`_ 3.3.0 or later:  To power a
+* `matplotlib <https://matplotlib.org/>`_ 3.5.0 or later:  To power a
   variety of plotting features (e.g., plotting apertures).
 
-* `scikit-image <https://scikit-image.org/>`_ 0.18.0 or later: Used for
+* `scikit-image <https://scikit-image.org/>`_ 0.19.0 or later: Used for
   deblending segmented sources.
 
 * `scikit-learn <https://scikit-learn.org/>`_ 1.0 or later:  Used in
   `~photutils.psf.DBSCANGroup` to create star groups.
 
-* `gwcs <https://github.com/spacetelescope/gwcs>`_ 0.16 or later:
+* `gwcs <https://github.com/spacetelescope/gwcs>`_ 0.18 or later:
   Used in `~photutils.datasets.make_gwcs` to create a simple celestial
   gwcs object.
 
 * `bottleneck <https://github.com/pydata/bottleneck>`_: Improves the
   performance of sigma clipping and other functionality that may require
   computing statistics on arrays with NaN values.
 
@@ -41,15 +41,15 @@
 * `rasterio <https://rasterio.readthedocs.io/>`_: Used for converting
   source segments into polygon objects.
 
 * `Shapely <https://shapely.readthedocs.io/>`_: Used for converting
   source segments into polygon objects.
 
 Photutils depends on `pytest-astropy
-<https://github.com/astropy/pytest-astropy>`_ (0.4 or later) to run
+<https://github.com/astropy/pytest-astropy>`_ (0.10 or later) to run
 the test suite.
 
 
 Installing the latest released version
 ======================================
 
 The latest released (stable) version of Photutils can be installed
@@ -141,15 +141,15 @@
 the "-e" option::
 
     pip install -e ".[all]"
 
 Alternatively, `pip`_ can be used to retrieve, build, and install the
 latest development version from `GitHub`_::
 
-    pip install "git+https://github.com/astropy/photutils.git#egg=photutils[all]"
+    pip install "photutils[all] @ git+https://github.com/astropy/photutils.git"
 
 
 Testing an installed Photutils
 ==============================
 
 The easiest way to test your installed version of Photutils is running
 correctly is to use the :func:`photutils.test` function:
```

### Comparing `photutils-1.7.0/docs/isophote.rst` & `photutils-1.8.0/docs/isophote.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/isophote_faq.rst` & `photutils-1.8.0/docs/isophote_faq.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/make.bat` & `photutils-1.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/morphology.rst` & `photutils-1.8.0/docs/morphology.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/overview.rst` & `photutils-1.8.0/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/pixel_conventions.rst` & `photutils-1.8.0/docs/pixel_conventions.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/profiles.rst` & `photutils-1.8.0/docs/profiles.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Profiles (`photutils.profiles`)
 ===============================
 
 Introduction
 ------------
 
 `photutils.profiles` provides tools to calculate radial profiles and
-curves of growth using concentric apertures.
+curves of growth using concentric circular apertures.
 
 
 Preliminaries
 -------------
 
 Let’s start by making a synthetic image of a single source. Note that
 there is no background in this image. One should background-subtract the
@@ -46,75 +46,66 @@
     plt.figure(figsize=(5, 5))
     plt.imshow(data, norm=norm)
 
 
 Creating a Radial Profile
 -------------------------
 
+Photutils provides the :class:`~photutils.profiles.RadialProfile` class
+for computing radial profiles. The radial bins are defined by inputting
+a 1D array of radial edges. The radial spacing does not need to be
+constant.
+
 First, we'll use the `~photutils.centroids.centroid_quadratic` function
 to find the source centroid::
 
     >>> from photutils.centroids import centroid_quadratic
     >>> xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
     >>> print(xycen)  # doctest: +FLOAT_CMP
     [47.61226319 52.04668132]
 
-Now let's create a radial profile using the
-`~photutils.profiles.RadialProfile` class. The radial profile will
-be centered at our centroid position. It will be computed over the
-radial range from ``min_radius`` to ``max_radius`` with steps of
-``radius_step``::
+Now, let's create a radial profile. The radial profile will be centered
+at our centroid position computed above.
 
     >>> from photutils.profiles import RadialProfile
-    >>> min_radius = 0.0
-    >>> max_radius = 25.0
-    >>> radius_step = 1.0
-    >>> rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-    ...                    error=error, mask=None)
-
+    >>> edge_radii = np.arange(25)
+    >>> rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
-The `~photutils.profiles.RadialProfile` instance
-has `~photutils.profiles.RadialProfile.radius`,
+The `~photutils.profiles.RadialProfile.radius` (radial bin centers),
 `~photutils.profiles.RadialProfile.profile`, and
-`~photutils.profiles.RadialProfile.profile_error` attributes which
-contain 1D `~numpy.ndarray` objects::
+`~photutils.profiles.RadialProfile.profile_error` attributes contain the
+output 1D `~numpy.ndarray` objects::
 
     >>> print(rp.radius)  # doctest: +FLOAT_CMP
-    [ 0.  1.  2.  3.  4.  5.  6.  7.  8.  9. 10. 11. 12. 13. 14. 15. 16. 17.
-     18. 19. 20. 21. 22. 23. 24. 25.]
+    [ 0.5  1.5  2.5  3.5  4.5  5.5  6.5  7.5  8.5  9.5 10.5 11.5 12.5 13.5
+     14.5 15.5 16.5 17.5 18.5 19.5 20.5 21.5 22.5 23.5]
 
     >>> print(rp.profile)  # doctest: +FLOAT_CMP
-    [ 4.27430150e+01  4.02150658e+01  3.81601146e+01  3.38116846e+01
-      2.89343205e+01  2.34250297e+01  1.84368533e+01  1.44310461e+01
-      9.55543388e+00  6.55415896e+00  4.49693014e+00  2.56010523e+00
-      1.50362911e+00  7.35389056e-01  6.04663625e-01  8.08820954e-01
-      2.31751912e-01 -1.39063329e-01  1.25181410e-01  4.84601845e-01
-      1.94567871e-01  4.49109676e-01 -2.00995374e-01 -7.74387397e-02
-      5.70302749e-02 -3.27578439e-02]
+    [ 4.15632243e+01  3.93402079e+01  3.59845746e+01  3.15540506e+01
+      2.62300757e+01  2.07297033e+01  1.65106801e+01  1.19376723e+01
+      7.75743772e+00  5.56759777e+00  3.44112671e+00  1.91350281e+00
+      1.17092981e+00  4.22261078e-01  9.70256904e-01  4.16355795e-01
+      1.52328707e-02 -6.69985111e-02  4.15522650e-01  2.48494731e-01
+      4.03348112e-01  1.43482678e-01 -2.62777461e-01  7.30653622e-02]
 
     >>> print(rp.profile_error)  # doctest: +FLOAT_CMP
-    [2.95008692 1.17855895 0.6610777  0.51902503 0.47524302 0.43072819
-     0.39770113 0.37667594 0.33909996 0.35356048 0.30377721 0.29455808
-     0.25670656 0.26599511 0.27354232 0.2430305  0.22910334 0.22204777
-     0.22327174 0.23816561 0.2343794  0.2232632  0.19893783 0.17888776
-     0.18228289 0.19680823]
+    [1.69588246 0.81797694 0.61132694 0.44670831 0.49499835 0.38025361
+     0.40844702 0.32906672 0.36466713 0.33059274 0.29661894 0.27314739
+     0.25551933 0.27675376 0.25553986 0.23421017 0.22966813 0.21747036
+     0.23654884 0.22760386 0.23941711 0.20661313 0.18999134 0.17469024]
 
-The radial profile can be normalized using the
-:meth:`~photutils.profiles.RadialProfile.normalize` method:
-
-.. doctest-skip::
-
-    >>> rp.normalize(method='max')
+If desired, the radial profiles can be normalized using the
+:meth:`~photutils.profiles.RadialProfile.normalize` method.
 
 There are also convenience methods to plot the radial profile and its
 error:
 
 .. doctest-skip::
 
-    >>> rp.plot()
+    >>> rp.plot(label='Radial Profile')
     >>> rp.plot_error()
 
 .. plot::
 
     import numpy as np
     from astropy.modeling.models import Gaussian2D
 
@@ -129,28 +120,25 @@
     error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
     data += error
 
     # find the source centroid
     xycen = centroid_quadratic(data, xpeak=47, ypeak=52)
 
     # create the radial profile
-    min_radius = 0.0
-    max_radius = 25.0
-    radius_step = 1.0
-    rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                       error=error, mask=None)
+    edge_radii = np.arange(26)
+    rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
     # plot the radial profile
-    rp.normalize()
-    rp.plot()
+    rp.plot(label='Radial Profile')
     rp.plot_error()
+    plt.legend()
 
 The `~photutils.profiles.RadialProfile.apertures` attribute contains a
-list of the apertures. Let's plot two of the annulus apertures on the
-data:
+list of the apertures. Let's plot two of the annulus apertures for the
+`~photutils.profiles.RadialProfile` instance on the data:
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
     from astropy.modeling.models import Gaussian2D
     from astropy.visualization import simple_norm
@@ -166,19 +154,16 @@
     error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
     data += error
 
     # find the source centroid
     xycen = centroid_quadratic(data, xpeak=47, ypeak=52)
 
     # create the radial profile
-    min_radius = 0.0
-    max_radius = 25.0
-    radius_step = 1.0
-    rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                       error=error, mask=None)
+    edge_radii = np.arange(26)
+    rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
     norm = simple_norm(data, 'sqrt')
     plt.figure(figsize=(5, 5))
     plt.imshow(data, norm=norm)
     rp.apertures[5].plot(color='C0', lw=2)
     rp.apertures[10].plot(color='C1', lw=2)
 
@@ -186,25 +171,26 @@
 Now let's fit a 1D Gaussian to the radial
 profile and return the Gaussian model using the
 `~photutils.profiles.RadialProfile.gaussian_fit` attribute:
 
 .. doctest-requires:: scipy
 
     >>> rp.gaussian_fit  # doctest: +FLOAT_CMP
-    <Gaussian1D(amplitude=41.80620963, mean=0., stddev=4.69126969)>
+    <Gaussian1D(amplitude=41.54880743, mean=0., stddev=4.71059406)>
 
 The FWHM of the fitted 1D Gaussian model is stored in the
 `~photutils.profiles.RadialProfile.gaussian_fwhm` attribute:
 
 .. doctest-requires:: scipy
 
     >>> print(rp.gaussian_fwhm)  # doctest: +FLOAT_CMP
-    11.04709589620093
+    11.09260130738712
 
-Finally, let's plot the fitted 1D Gaussian on the radial profile:
+Finally, let's plot the fitted 1D Gaussian model for the
+class:`~photutils.profiles.RadialProfile` radial profile:
 
 .. plot::
 
     import matplotlib.pyplot as plt
     import numpy as np
     from astropy.modeling.models import Gaussian2D
 
@@ -219,79 +205,65 @@
     error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
     data += error
 
     # find the source centroid
     xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
 
     # create the radial profile
-    min_radius = 0.0
-    max_radius = 25.0
-    radius_step = 1.0
-    rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                       error=error, mask=None)
+    edge_radii = np.arange(26)
+    rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
     # plot the radial profile
-    rp.normalize()
     rp.plot(label='Radial Profile')
     rp.plot_error()
     plt.plot(rp.radius, rp.gaussian_profile, label='Gaussian Fit')
+
     plt.legend()
 
 
 Creating a Curve of Growth
 --------------------------
 
 Now let's create a curve of growth using the
 `~photutils.profiles.CurveOfGrowth` class. We use the simulated image
 defined above and the same source centroid.
 
 The curve of growth will be centered at our centroid position. It will
-be computed over the radial range from ``min_radius`` to ``max_radius``
-with steps of ``radius_step``::
+be computed over the radial range given by the input ``radii`` array::
 
     >>> from photutils.profiles import CurveOfGrowth
-    >>> min_radius = 0.0
-    >>> max_radius = 25.0
-    >>> radius_step = 1.0
-    >>> cog = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-    ...                     error=error, mask=None)
-
+    >>> radii = np.arange(1, 26)
+    >>> cog = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
 
 The `~photutils.profiles.CurveOfGrowth` instance
 has `~photutils.profiles.CurveOfGrowth.radius`,
 `~photutils.profiles.CurveOfGrowth.profile`, and
 `~photutils.profiles.CurveOfGrowth.profile_error` attributes which
 contain 1D `~numpy.ndarray` objects::
 
     >>> print(cog.radius)  # doctest: +FLOAT_CMP
-    [ 0.  1.  2.  3.  4.  5.  6.  7.  8.  9. 10. 11. 12. 13. 14. 15. 16. 17.
-     18. 19. 20. 21. 22. 23. 24. 25.]
+    [ 1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24
+     25]
 
     >>> print(cog.profile)  # doctest: +FLOAT_CMP
-    [   0.          130.57472018  501.34744442 1066.59182074 1760.50163608
-     2502.13955554 3218.50667597 3892.81448231 4455.36403436 4869.66609313
-     5201.99745378 5429.02043984 5567.28370644 5659.24831854 5695.06577065
-     5783.46217755 5824.01080702 5825.59003768 5818.22316662 5866.52307412
-     5896.96917375 5948.92254787 5968.30540534 5931.15611704 5941.94457249
-     5942.06535486]
+    [ 130.57472018  501.34744442 1066.59182074 1760.50163608 2502.13955554
+     3218.50667597 3892.81448231 4455.36403436 4869.66609313 5201.99745378
+     5429.02043984 5567.28370644 5659.24831854 5695.06577065 5783.46217755
+     5824.01080702 5825.59003768 5818.22316662 5866.52307412 5896.96917375
+     5948.92254787 5968.30540534 5931.15611704 5941.94457249 5942.06535486]
 
     >>> print(cog.profile_error)  # doctest: +FLOAT_CMP
-    [  0.           5.32777186   9.37111012  13.41750992  16.62928904
-      21.7350922   25.39862532  30.3867526   34.11478867  39.28263973
-      43.96047829  48.11931395  52.00967328  55.7471834   60.48824739
-      64.81392778  68.71042311  72.71899201  76.54959872  81.33806741
-      85.98568713  91.34841248  95.5173253   99.22190499 102.51980185
-     106.83601366]
-
-The curve of growth profile can be normalized using the
-:meth:`~photutils.profiles.RadialProfile.normalize` method:
-
-.. doctest-skip::
+    [  5.32777186   9.37111012  13.41750992  16.62928904  21.7350922
+      25.39862532  30.3867526   34.11478867  39.28263973  43.96047829
+      48.11931395  52.00967328  55.7471834   60.48824739  64.81392778
+      68.71042311  72.71899201  76.54959872  81.33806741  85.98568713
+      91.34841248  95.5173253   99.22190499 102.51980185 106.83601366]
 
-    >>> rp.normalize(method='max')
+If desired, the curve of growth profile can be normalized using the
+:meth:`~photutils.profiles.RadialProfile.normalize` method.
 
 There are also convenience methods to plot the curve of growth and its
 error:
 
 .. doctest-skip::
 
     >>> rp.plot()
@@ -313,22 +285,18 @@
     error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
     data += error
 
     # find the source centroid
     xycen = centroid_quadratic(data, xpeak=47, ypeak=52)
 
     # create the radial profile
-    min_radius = 0.0
-    max_radius = 25.0
-    radius_step = 1.0
-    cog = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=error, mask=None)
+    radii = np.arange(1, 26)
+    cog = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
 
     # plot the radial profile
-    cog.normalize()
     cog.plot()
     cog.plot_error()
 
 The `~photutils.profiles.CurveOfGrowth.apertures` attribute contains a
 list of the apertures. Let's plot a couple of the apertures on the data:
 
 .. plot::
@@ -349,19 +317,16 @@
     error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
     data += error
 
     # find the source centroid
     xycen = centroid_quadratic(data, xpeak=47, ypeak=52)
 
     # create the radial profile
-    min_radius = 0.0
-    max_radius = 25.0
-    radius_step = 1.0
-    cog = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=error, mask=None)
+    radii = np.arange(1, 26)
+    cog = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
 
     norm = simple_norm(data, 'sqrt')
     plt.figure(figsize=(5, 5))
     plt.imshow(data, norm=norm)
     cog.apertures[5].plot(color='C0', lw=2)
     cog.apertures[10].plot(color='C1', lw=2)
```

### Comparing `photutils-1.7.0/docs/psf.rst` & `photutils-1.8.0/docs/psf.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_matching.rst` & `photutils-1.8.0/docs/psf_matching.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/background_estimator.rst` & `photutils-1.8.0/docs/psf_spec/background_estimator.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/block_diagram.png` & `photutils-1.8.0/docs/psf_spec/block_diagram.png`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/block_template.rst` & `photutils-1.8.0/docs/psf_spec/block_template.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/culler_and_ender.rst` & `photutils-1.8.0/docs/psf_spec/culler_and_ender.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/finder.rst` & `photutils-1.8.0/docs/psf_spec/finder.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/group_maker.rst` & `photutils-1.8.0/docs/psf_spec/group_maker.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/noise_data.rst` & `photutils-1.8.0/docs/psf_spec/noise_data.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/psf_model.rst` & `photutils-1.8.0/docs/psf_spec/psf_model.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/scene_maker.rst` & `photutils-1.8.0/docs/psf_spec/scene_maker.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/psf_spec/single_object_model.rst` & `photutils-1.8.0/docs/psf_spec/single_object_model.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/segmentation.rst` & `photutils-1.8.0/docs/segmentation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,15 @@
     nlabels: 94
     labels: [ 1  2  3  4  5 ... 90 91 92 93 94]
 
 
 Modifying a Segmentation Image
 ------------------------------
 The :class:`~photutils.segmentation.SegmentationImage` object provides
-several methods that can be used to visualize or modify itself (e.g.,
+several methods that can be used to modify itself (e.g.,
 combining labels, removing labels, removing border segments) prior to
 measuring source photometry and other source properties, including:
 
   * :meth:`~photutils.segmentation.SegmentationImage.reassign_label`:
     Reassign one or more label numbers.
 
   * :meth:`~photutils.segmentation.SegmentationImage.relabel_consecutive`:
@@ -297,17 +297,14 @@
 
   * :meth:`~photutils.segmentation.SegmentationImage.remove_border_labels`:
     Remove labeled segments near the image border.
 
   * :meth:`~photutils.segmentation.SegmentationImage.remove_masked_labels`:
     Remove labeled segments located within a masked region.
 
-  * :meth:`~photutils.segmentation.SegmentationImage.outline_segments`:
-    Outline the labeled segments for plotting.
-
 
 Photometry, Centroids, and Shape Properties
 -------------------------------------------
 The :class:`~photutils.segmentation.SourceCatalog` class is the primary
 tool for measuring the photometry, centroids, and shape/morphological
 properties of sources defined in a segmentation image. In its most
 basic form, it takes as input the (background-subtracted) image and
```

### Comparing `photutils-1.7.0/docs/whats_new/1.1.rst` & `photutils-1.8.0/docs/whats_new/1.1.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/whats_new/1.4.rst` & `photutils-1.8.0/docs/whats_new/1.4.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/whats_new/1.5.rst` & `photutils-1.8.0/docs/whats_new/1.5.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/whats_new/1.6.rst` & `photutils-1.8.0/docs/whats_new/1.6.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/docs/whats_new/1.7.rst` & `photutils-1.8.0/docs/whats_new/1.7.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/CITATION.rst` & `photutils-1.8.0/photutils/CITATION.rst`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/__init__.py` & `photutils-1.8.0/photutils/__init__.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/_compiler.c` & `photutils-1.8.0/photutils/_compiler.c`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/attributes.py` & `photutils-1.8.0/photutils/aperture/attributes.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/bounding_box.py` & `photutils-1.8.0/photutils/aperture/bounding_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """
 This module defines a class for a rectangular bounding box.
 """
 
 import math
 
 import numpy as np
-from astropy.utils.decorators import deprecated_renamed_argument
 
 __all__ = ['BoundingBox']
 
 
 class BoundingBox:
     """
     A rectangular bounding box in integer (not float) pixel indices.
@@ -266,15 +265,14 @@
         # prevent circular import
         from photutils.aperture.rectangle import RectangularAperture
 
         xypos = self.center[::-1]  # xy order
         height, width = self.shape
         return RectangularAperture(xypos, w=width, h=height, theta=0.0)
 
-    @deprecated_renamed_argument('axes', 'ax', '1.6.0')
     def plot(self, ax=None, origin=(0, 0), **kwargs):
         """
         Plot the `BoundingBox` on a matplotlib `~matplotlib.axes.Axes`
         instance.
 
         Parameters
         ----------
```

### Comparing `photutils-1.7.0/photutils/aperture/circle.py` & `photutils-1.8.0/photutils/aperture/circle.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/core.py` & `photutils-1.8.0/photutils/aperture/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import warnings
 from copy import deepcopy
 
 import astropy.units as u
 import numpy as np
 from astropy.coordinates import SkyCoord
 from astropy.utils import lazyproperty
-from astropy.utils.decorators import deprecated_renamed_argument
 
 from photutils.aperture.bounding_box import BoundingBox
 from photutils.utils._wcs_helpers import _pixel_scale_angle_at_skycoord
 
 __all__ = ['Aperture', 'SkyAperture', 'PixelAperture']
 
 
@@ -542,51 +541,36 @@
         apermasks = self.to_mask(method=method, subpixels=subpixels)
         if self.isscalar:
             apermasks = (apermasks,)
 
         aperture_sums = []
         aperture_sum_errs = []
         for apermask in apermasks:
-            slc_large, slc_small = apermask.get_overlap_slices(data.shape)
+            (slc_large,
+             aper_weights,
+             pixel_mask) = apermask._get_overlap_cutouts(data.shape, mask=mask)
 
             # no overlap of the aperture with the data
             if slc_large is None:
                 aperture_sums.append(np.nan)
                 aperture_sum_errs.append(np.nan)
                 continue
 
-            data_cutout = data[slc_large]
-            apermask_cutout = apermask.data[slc_small]
-            pixel_mask = apermask_cutout > 0  # good pixels
-
-            if mask is not None:
-                if mask.shape != data.shape:
-                    raise ValueError('mask and data must have the same shape')
-                pixel_mask &= ~mask[slc_large]
-
-            # ignore multiplication with non-finite data values
             with warnings.catch_warnings():
+                # ignore multiplication with non-finite data values
                 warnings.simplefilter('ignore', RuntimeWarning)
-                values = (data_cutout * apermask_cutout)[pixel_mask]
-            aperture_sums.append(values.sum())
 
-            if error is not None:
-                if error.shape != data.shape:
-                    raise ValueError('error and data must have the same shape')
-                var_cutout = error[slc_large]**2
+                values = (data[slc_large] * aper_weights)[pixel_mask]
+                aperture_sums.append(values.sum())
 
-                # ignore multiplication with non-finite data values
-                with warnings.catch_warnings():
-                    warnings.simplefilter('ignore', RuntimeWarning)
-                    values = (var_cutout * apermask_cutout)[pixel_mask]
-                aperture_sum_errs.append(np.sqrt(values.sum()))
+                if error is not None:
+                    variance = (error[slc_large]**2 * aper_weights)[pixel_mask]
+                    aperture_sum_errs.append(np.sqrt(variance.sum()))
 
         aperture_sums = np.array(aperture_sums)
-        if error is None:
-            aperture_sum_errs = []
         aperture_sum_errs = np.array(aperture_sum_errs)
 
         # apply units
         if unit is not None:
             aperture_sums <<= unit
             aperture_sum_errs <<= unit
 
@@ -671,15 +655,14 @@
         patch : `~matplotlib.patches.patch` or list of `~matplotlib.patches.patch`
             A patch for the aperture.  If the aperture is scalar then a
             single `~matplotlib.patches.patch` is returned, otherwise a
             list of `~matplotlib.patches.patch` is returned.
         """
         raise NotImplementedError('Needs to be implemented in a subclass.')
 
-    @deprecated_renamed_argument('axes', 'ax', '1.6.0')
     def plot(self, ax=None, origin=(0, 0), **kwargs):
         """
         Plot the aperture on a matplotlib `~matplotlib.axes.Axes`
         instance.
 
         Parameters
         ----------
```

### Comparing `photutils-1.7.0/photutils/aperture/ellipse.py` & `photutils-1.8.0/photutils/aperture/ellipse.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/mask.py` & `photutils-1.8.0/photutils/aperture/mask.py`

 * *Files 18% similar despite different names*

```diff
@@ -218,14 +218,69 @@
                 weighted_cutout = cutout * self.data
 
             # fill values outside of the mask but within the bounding box
             weighted_cutout[self._mask] = fill_value
 
             return weighted_cutout
 
+    def _get_overlap_cutouts(self, shape, mask=None):
+        """
+        Get the aperture mask weights, pixel mask, and slice for the
+        overlap with the input shape.
+
+        If input, the ``mask`` is included in the output pixel mask
+        cutout.
+
+        Parameters
+        ----------
+        shape : tuple of int
+            The shape of data.
+
+        mask : array_like (bool), optional
+            A boolean mask with the same shape as ``shape`` where a
+            `True` value indicates a masked pixel.
+
+        Returns
+        -------
+        slices_large : tuple of slices or `None`
+            A tuple of slice objects for each axis of the large array
+            of given ``shape``, such that ``large_array[slices_large]``
+            extracts the region of the large array that overlaps with
+            the small array. `None` is returned if there is no overlap
+            of the bounding box with the given image shape.
+
+        aper_weights: 2D float `~numpy.ndarray`
+            The cutout aperture mask weights for the overlap.
+
+        pixel_mask: 2D bool `~numpy.ndarray`
+            The cutout pixel mask for the overlap.
+
+        Notes
+        -----
+        This method is separate from ``get_values`` to facilitate
+        applying the same slices, aper_weights, and pixel_mask to
+        multiple associated arrays (e.g., data and error arrays). It is
+        used in this way by the `PixelAperture.do_photometry` method.
+        """
+        if mask is not None:
+            if mask.shape != shape:
+                raise ValueError('mask and data must have the same shape')
+
+        slc_large, slc_small = self.get_overlap_slices(shape)
+        if slc_large is None:  # no overlap
+            return None, None, None
+
+        aper_weights = self.data[slc_small]
+        pixel_mask = (aper_weights > 0)  # good pixels
+
+        if mask is not None:
+            pixel_mask &= ~mask[slc_large]
+
+        return slc_large, aper_weights, pixel_mask
+
     def get_values(self, data, mask=None):
         """
         Get the mask-weighted pixel values from the data as a 1D array.
 
         If the ``ApertureMask`` was created with ``method='center'``,
         (where the mask weights are only 1 or 0), then the returned
         values will simply be pixel values extracted from the data.
@@ -244,23 +299,19 @@
         -------
         result : `~numpy.ndarray`
             A 1D array of mask-weighted pixel values from the input
             ``data``. If there is no overlap of the aperture with the
             input ``data``, the result will be an empty array with shape
             (0,).
         """
-        slc_large, slc_small = self.get_overlap_slices(data.shape)
+        slc_large, aper_weights, pixel_mask = self._get_overlap_cutouts(
+            data.shape, mask=mask)
+
         if slc_large is None:
             return np.array([])
-        cutout = data[slc_large]
-        apermask = self.data[slc_small]
-        pixel_mask = (apermask > 0)  # good pixels
-
-        if mask is not None:
-            if mask.shape != data.shape:
-                raise ValueError('mask and data must have the same shape')
-            pixel_mask &= ~mask[slc_large]
 
         # ignore multiplication with non-finite data values
         with warnings.catch_warnings():
             warnings.simplefilter('ignore', RuntimeWarning)
-            return (cutout * apermask)[pixel_mask]
+            # pixel_mask is used so that pixels value where data = 0 and
+            # aper_weights != 0 are still returned
+            return (data[slc_large] * aper_weights)[pixel_mask]
```

### Comparing `photutils-1.7.0/photutils/aperture/photometry.py` & `photutils-1.8.0/photutils/aperture/photometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/rectangle.py` & `photutils-1.8.0/photutils/aperture/rectangle.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/stats.py` & `photutils-1.8.0/photutils/aperture/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,16 @@
     """
 
     def __init__(self, data, aperture, *, error=None, mask=None, wcs=None,
                  sigma_clip=None, sum_method='exact', subpixels=5,
                  local_bkg=None):
 
         if isinstance(data, NDData):
-            data, error, mask, wcs = self.unpack_nddata(data, error, mask, wcs)
+            data, error, mask, wcs = self._unpack_nddata(data, error, mask,
+                                                         wcs)
 
         (data, error, local_bkg), unit = process_quantities(
             (data, error, local_bkg), ('data', 'error', 'local_bkg'))
         self._data = self._validate_array(data, 'data', shape=False)
         self._data_unit = unit
         self.aperture = self._validate_aperture(aperture)
 
@@ -254,15 +255,15 @@
             self._local_bkg = local_bkg  # always an iterable
 
         self._ids = np.arange(self.n_apertures) + 1
         self.default_columns = DEFAULT_COLUMNS
         self.meta = _get_meta()
 
     @staticmethod
-    def unpack_nddata(data, error, mask, wcs):
+    def _unpack_nddata(data, error, mask, wcs):
         nddata_attr = {'error': error, 'mask': mask, 'wcs': wcs}
         for key, value in nddata_attr.items():
             if value is not None:
                 warnings.warn(f'The {key!r} keyword is be ignored. Its '
                               'value is obtained from the input NDData '
                               'object.', AstropyUserWarning)
```

### Comparing `photutils-1.7.0/photutils/aperture/tests/test_aperture_common.py` & `photutils-1.8.0/photutils/aperture/tests/test_aperture_common.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/tests/test_bounding_box.py` & `photutils-1.8.0/photutils/aperture/tests/test_bounding_box.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/tests/test_circle.py` & `photutils-1.8.0/photutils/aperture/tests/test_circle.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/tests/test_ellipse.py` & `photutils-1.8.0/photutils/aperture/tests/test_ellipse.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/tests/test_mask.py` & `photutils-1.8.0/photutils/aperture/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/tests/test_photometry.py` & `photutils-1.8.0/photutils/aperture/tests/test_photometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/tests/test_rectangle.py` & `photutils-1.8.0/photutils/aperture/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/aperture/tests/test_stats.py` & `photutils-1.8.0/photutils/aperture/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/background/background_2d.py` & `photutils-1.8.0/photutils/background/background_2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import warnings
 
 import astropy.units as u
 import numpy as np
 from astropy.nddata import NDData
 from astropy.stats import SigmaClip
 from astropy.utils import lazyproperty
-from astropy.utils.decorators import deprecated_renamed_argument
 from astropy.utils.exceptions import AstropyUserWarning
 from numpy.lib.index_tricks import index_exp
 
 from photutils.aperture import RectangularAperture
 from photutils.background.core import SExtractorBackground, StdBackgroundRMS
 from photutils.background.interpolators import BkgZoomInterpolator
 from photutils.utils import ShepardIDWInterpolator
@@ -651,15 +650,14 @@
         bkg_rms = self.interpolator(self.background_rms_mesh, self)
         if self.coverage_mask is not None:
             bkg_rms[self.coverage_mask] = self.fill_value
         if self.unit is not None:
             bkg_rms <<= self.unit
         return bkg_rms
 
-    @deprecated_renamed_argument('axes', 'ax', '1.6.0')
     def plot_meshes(self, *, ax=None, marker='+', markersize=None,
                     color='blue', alpha=None, outlines=False, **kwargs):
         """
         Plot the low-resolution mesh boxes on a matplotlib Axes
         instance.
 
         Parameters
```

### Comparing `photutils-1.7.0/photutils/background/core.py` & `photutils-1.8.0/photutils/background/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/background/interpolators.py` & `photutils-1.8.0/photutils/background/interpolators.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/background/tests/test_background_2d.py` & `photutils-1.8.0/photutils/background/tests/test_background_2d.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/background/tests/test_core.py` & `photutils-1.8.0/photutils/background/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/centroids/core.py` & `photutils-1.8.0/photutils/centroids/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/centroids/gaussian.py` & `photutils-1.8.0/photutils/centroids/gaussian.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/centroids/tests/test_core.py` & `photutils-1.8.0/photutils/centroids/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/centroids/tests/test_gaussian.py` & `photutils-1.8.0/photutils/centroids/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/conftest.py` & `photutils-1.8.0/photutils/conftest.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/datasets/load.py` & `photutils-1.8.0/photutils/datasets/load.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/datasets/make.py` & `photutils-1.8.0/photutils/datasets/make.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/datasets/tests/test_make.py` & `photutils-1.8.0/photutils/datasets/tests/test_make.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/core.py` & `photutils-1.8.0/photutils/detection/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/daofinder.py` & `photutils-1.8.0/photutils/detection/daofinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/irafstarfinder.py` & `photutils-1.8.0/photutils/detection/irafstarfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/peakfinder.py` & `photutils-1.8.0/photutils/detection/peakfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/starfinder.py` & `photutils-1.8.0/photutils/detection/starfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.0.txt` & `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.5.txt` & `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm01.5.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm02.0.txt` & `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh08.0_fwhm02.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.0.txt` & `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.5.txt` & `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm01.5.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm02.0.txt` & `photutils-1.8.0/photutils/detection/tests/data/daofind_test_thresh10.0_fwhm02.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.0.txt` & `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.5.txt` & `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm01.5.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm02.0.txt` & `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh08.0_fwhm02.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.0.txt` & `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.5.txt` & `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm01.5.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm02.0.txt` & `photutils-1.8.0/photutils/detection/tests/data/irafstarfind_test_thresh10.0_fwhm02.0.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/test_daofinder.py` & `photutils-1.8.0/photutils/detection/tests/test_daofinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/test_irafstarfinder.py` & `photutils-1.8.0/photutils/detection/tests/test_irafstarfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/test_peakfinder.py` & `photutils-1.8.0/photutils/detection/tests/test_peakfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/detection/tests/test_starfinder.py` & `photutils-1.8.0/photutils/detection/tests/test_starfinder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/geometry/circular_overlap.pyx` & `photutils-1.8.0/photutils/geometry/circular_overlap.pyx`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/geometry/core.pxd` & `photutils-1.8.0/photutils/geometry/core.pxd`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/geometry/core.pyx` & `photutils-1.8.0/photutils/geometry/core.pyx`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/geometry/elliptical_overlap.pyx` & `photutils-1.8.0/photutils/geometry/elliptical_overlap.pyx`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/geometry/rectangular_overlap.pyx` & `photutils-1.8.0/photutils/geometry/rectangular_overlap.pyx`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/geometry/tests/test_circular_overlap_grid.py` & `photutils-1.8.0/photutils/geometry/tests/test_circular_overlap_grid.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/geometry/tests/test_elliptical_overlap_grid.py` & `photutils-1.8.0/photutils/geometry/tests/test_elliptical_overlap_grid.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/geometry/tests/test_rectangular_overlap_grid.py` & `photutils-1.8.0/photutils/geometry/tests/test_rectangular_overlap_grid.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/ellipse.py` & `photutils-1.8.0/photutils/isophote/ellipse.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/fitter.py` & `photutils-1.8.0/photutils/isophote/fitter.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/geometry.py` & `photutils-1.8.0/photutils/isophote/geometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/harmonics.py` & `photutils-1.8.0/photutils/isophote/harmonics.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/integrator.py` & `photutils-1.8.0/photutils/isophote/integrator.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/isophote.py` & `photutils-1.8.0/photutils/isophote/isophote.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/model.py` & `photutils-1.8.0/photutils/isophote/model.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/sample.py` & `photutils-1.8.0/photutils/isophote/sample.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/data/M51_table.fits` & `photutils-1.8.0/photutils/isophote/tests/data/M51_table.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/data/minimum_radius_test.fits` & `photutils-1.8.0/photutils/isophote/tests/data/minimum_radius_test.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/data/synth_highsnr_table.fits` & `photutils-1.8.0/photutils/isophote/tests/data/synth_highsnr_table.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/data/synth_lowsnr_table.fits` & `photutils-1.8.0/photutils/isophote/tests/data/synth_lowsnr_table.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/data/synth_table.fits` & `photutils-1.8.0/photutils/isophote/tests/data/synth_table.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/data/synth_table_mean.fits` & `photutils-1.8.0/photutils/isophote/tests/data/synth_table_mean.fits`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/data/synth_table_mean.txt` & `photutils-1.8.0/photutils/isophote/tests/data/synth_table_mean.txt`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/make_test_data.py` & `photutils-1.8.0/photutils/isophote/tests/make_test_data.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_angles.py` & `photutils-1.8.0/photutils/isophote/tests/test_angles.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_ellipse.py` & `photutils-1.8.0/photutils/isophote/tests/test_ellipse.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_fitter.py` & `photutils-1.8.0/photutils/isophote/tests/test_fitter.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_geometry.py` & `photutils-1.8.0/photutils/isophote/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_harmonics.py` & `photutils-1.8.0/photutils/isophote/tests/test_harmonics.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
     def test_fit_upper_harmonics(self):
         data = make_test_image(noise=1.0e-10, seed=0)
         sample = EllipseSample(data, 40)
         fitter = EllipseFitter(sample)
         iso = fitter.fit(maxit=400)
 
-        assert_allclose(iso.a3, 6.825e-7, atol=1.0e-9)
+        assert_allclose(iso.a3, 6.825e-7, atol=1.0e-8)
         assert_allclose(iso.b3, -1.68e-6, atol=1.0e-8)
         assert_allclose(iso.a4, 4.36e-6, atol=1.0e-8)
         assert_allclose(iso.b4, -4.73e-5, atol=1.0e-7)
 
         assert_allclose(iso.a3_err, 8.152e-6, atol=1.0e-7)
         assert_allclose(iso.b3_err, 8.115e-6, atol=1.0e-7)
         assert_allclose(iso.a4_err, 7.501e-6, atol=1.0e-7)
```

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_integrator.py` & `photutils-1.8.0/photutils/isophote/tests/test_integrator.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_isophote.py` & `photutils-1.8.0/photutils/isophote/tests/test_isophote.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_model.py` & `photutils-1.8.0/photutils/isophote/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_regression.py` & `photutils-1.8.0/photutils/isophote/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/isophote/tests/test_sample.py` & `photutils-1.8.0/photutils/isophote/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/morphology/core.py` & `photutils-1.8.0/photutils/morphology/core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/morphology/non_parametric.py` & `photutils-1.8.0/photutils/morphology/non_parametric.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/morphology/tests/test_core.py` & `photutils-1.8.0/photutils/morphology/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/profiles/core.py` & `photutils-1.8.0/photutils/profiles/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 This module provides a base class for profiles.
 """
 
-import math
+import abc
 import warnings
 
 import numpy as np
 from astropy.utils import lazyproperty
 from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.utils._quantity_helpers import process_quantities
 
 __all__ = ['ProfileBase']
 
 
-class ProfileBase:
+class ProfileBase(metaclass=abc.ABCMeta):
     """
-    Base class for profile classes.
+    Abtract base class for profile classes.
 
     Parameters
     ----------
     data : 2D `numpy.ndarray`
         The 2D data array. The data should be background-subtracted.
 
     xycen : tuple of 2 floats
         The ``(x, y)`` pixel coordinate of the source center.
 
-    min_radius : float
-        The minimum radius for the profile.
-
-    max_radius : float
-        The maximum radius for the profile.
-
-    radius_step : float
-        The radial step size in pixels.
+    radii : 1D float `numpy.ndarray`
+        An array of radii defining the edges of the radial bins.
+        ``radii`` must be strictly increasing with a minimum value
+        greater than or equal to zero, and contain at least 2 values.
+        The radial spacing does not need to be constant. The output
+        `radius` attribute will be defined at the bin centers.
 
     error : 2D `numpy.ndarray`, optional
         The 1-sigma errors of the input ``data``. ``error`` is assumed
         to include all sources of error, including the Poisson error
         of the sources (see `~photutils.utils.calc_total_error`) .
         ``error`` must have the same shape as the input ``data``.
 
@@ -73,87 +71,106 @@
     subpixels : int, optional
         For the ``'subpixel'`` method, resample pixels by this factor
         in each dimension. That is, each pixel is divided into
         ``subpixels**2`` subpixels. This keyword is ignored unless
         ``method='subpixel'``.
     """
 
-    _circular_radii = None
-    profile = None
-    profile_error = None
-
-    def __init__(self, data, xycen, min_radius, max_radius, radius_step, *,
-                 error=None, mask=None, method='exact', subpixels=5):
+    def __init__(self, data, xycen, radii, *, error=None, mask=None,
+                 method='exact', subpixels=5):
 
         (data, error), unit = process_quantities((data, error),
                                                  ('data', 'error'))
 
         if error is not None and error.shape != data.shape:
-            raise ValueError('error must have the same same as data')
+            raise ValueError('error must have the same shape as data')
+
+        self.data = data
+        self.unit = unit
+        self.xycen = xycen
+        self.radii = self._validate_radii(radii)
+        self.error = error
+        self.mask = self._compute_mask(data, error, mask)
+        self.method = method
+        self.subpixels = subpixels
+
+    def _validate_radii(self, edge_radii):
+        edge_radii = np.array(edge_radii)
+        if edge_radii.ndim != 1 or edge_radii.size < 2:
+            raise ValueError('edge_radii must be a 1D array and have at '
+                             'least two values')
+        if edge_radii.min() < 0:
+            raise ValueError('minimum edge_radii must be >= 0')
 
+        if not np.all(edge_radii[1:] > edge_radii[:-1]):
+            raise ValueError('edge_radii must be strictly increasing')
+
+        return edge_radii
+
+    def _compute_mask(self, data, error, mask):
+        """
+        Compute the mask array, automatically masking non-finite data or
+        error values.
+        """
         badmask = ~np.isfinite(data)
         if error is not None:
             badmask |= ~np.isfinite(error)
         if mask is not None:
             if mask.shape != data.shape:
-                raise ValueError('mask must have the same same as data')
+                raise ValueError('mask must have the same shape as data')
             badmask &= ~mask  # non-finite values not in input mask
             mask |= badmask  # all masked pixels
         else:
             mask = badmask
 
         if np.any(badmask):
             warnings.warn('Input data contains non-finite values (e.g., NaN '
                           'or inf) that were automatically masked.',
                           AstropyUserWarning)
 
-        self.data = data
-        self.error = error
-        self.mask = mask
-        self.unit = unit
-        self.xycen = xycen
-
-        if min_radius < 0 or max_radius < 0:
-            raise ValueError('min_radius and max_radius must be >= 0')
-        if min_radius >= max_radius:
-            raise ValueError('max_radius must be greater than min_radius')
-        if radius_step <= 0:
-            raise ValueError('radius_step must be > 0')
-        self.min_radius = min_radius
-        self.max_radius = max_radius
-        self.radius_step = radius_step
-        self.method = method
-        self.subpixels = subpixels
+        return mask
 
     @lazyproperty
     def radius(self):
         """
         The profile radius in pixels as a 1D `~numpy.ndarray`.
         """
-        nsteps = int(math.floor((self.max_radius - self.min_radius)
-                                / self.radius_step))
-        max_radius = self.min_radius + (nsteps * self.radius_step)
-        return np.linspace(self.min_radius, max_radius, nsteps + 1)
+        return self.radii
+
+    @property
+    @abc.abstractmethod
+    def profile(self):
+        """
+        The radial profile as a 1D `~numpy.ndarray`.
+        """
+        raise NotImplementedError('Needs to be implemented in a subclass.')
+
+    @property
+    @abc.abstractmethod
+    def profile_error(self):
+        """
+        The radial profile errors as a 1D `~numpy.ndarray`.
+        """
+        raise NotImplementedError('Needs to be implemented in a subclass.')
 
     @lazyproperty
     def _circular_apertures(self):
         """
         A list of `~photutils.aperture.CircularAperture` objects.
 
         The first element may be `None`.
         """
         from photutils.aperture import CircularAperture
 
         apertures = []
-        for radius in self._circular_radii:
+        for radius in self.radii:
             if radius <= 0.0:
-                aper = None
+                apertures.append(None)
             else:
-                aper = CircularAperture(self.xycen, radius)
-            apertures.append(aper)
+                apertures.append(CircularAperture(self.xycen, radius))
         return apertures
 
     @lazyproperty
     def _photometry(self):
         """
         The aperture fluxes, flux errors, and areas as a function of
         radius.
```

### Comparing `photutils-1.7.0/photutils/profiles/curve_of_growth.py` & `photutils-1.8.0/photutils/profiles/curve_of_growth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 This module provides tools for generating curves of growth.
 """
-
+import numpy as np
 from astropy.utils import lazyproperty
 
 from photutils.profiles.core import ProfileBase
 
 __all__ = ['CurveOfGrowth']
 
 
@@ -14,39 +14,37 @@
     """
     Class to create a curve of growth using concentric circular
     apertures.
 
     The curve of growth profile represents the circular aperture flux as
     a function of circular radius.
 
-    Non-finite values (e.g., NaN or inf) in the ``data`` or ``error``
-    array are automatically masked.
-
     Parameters
     ----------
     data : 2D `numpy.ndarray`
         The 2D data array. The data should be background-subtracted.
+        Non-finite values (e.g., NaN or inf) in the ``data`` or
+        ``error`` array are automatically masked.
 
     xycen : tuple of 2 floats
         The ``(x, y)`` pixel coordinate of the source center.
 
-    min_radius : float
-        The minimum radius for the profile.
-
-    max_radius : float
-        The maximum radius for the profile.
-
-    radius_step : float
-        The radial step size in pixels.
+    radii : 1D float `numpy.ndarray`
+        An array of the circular radii. ``radii`` must be strictly
+        increasing with a minimum value greater than zero, and contain
+        at least 2 values. The radial spacing does not need to be
+        constant.
 
     error : 2D `numpy.ndarray`, optional
         The 1-sigma errors of the input ``data``. ``error`` is assumed
         to include all sources of error, including the Poisson error
         of the sources (see `~photutils.utils.calc_total_error`) .
         ``error`` must have the same shape as the input ``data``.
+        Non-finite values (e.g., NaN or inf) in the ``data`` or
+        ``error`` array are automatically masked.
 
     mask : 2D bool `numpy.ndarray`, optional
         A boolean mask with the same shape as ``data`` where a `True`
         value indicates the corresponding element of ``data`` is masked.
         Masked data are excluded from all calculations.
 
     method : {'exact', 'center', 'subpixel'}, optional
@@ -95,39 +93,34 @@
     >>> data = gmodel(xx, yy)
     >>> error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
     >>> data += error
 
     Create the curve of growth.
 
     >>> xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
-    >>> min_radius = 0.0
-    >>> max_radius = 25.0
-    >>> radius_step = 1.0
-    >>> cog = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-    ...                     error=error, mask=None)
+    >>> radii = np.arange(1, 26)
+    >>> cog = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
 
     >>> print(cog.radius)  # doctest: +FLOAT_CMP
-    [ 0.  1.  2.  3.  4.  5.  6.  7.  8.  9. 10. 11. 12. 13. 14. 15. 16. 17.
-     18. 19. 20. 21. 22. 23. 24. 25.]
+    [ 1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24
+     25]
 
     >>> print(cog.profile)  # doctest: +FLOAT_CMP
-    [   0.          130.57472018  501.34744442 1066.59182074 1760.50163608
-     2502.13955554 3218.50667597 3892.81448231 4455.36403436 4869.66609313
-     5201.99745378 5429.02043984 5567.28370644 5659.24831854 5695.06577065
-     5783.46217755 5824.01080702 5825.59003768 5818.22316662 5866.52307412
-     5896.96917375 5948.92254787 5968.30540534 5931.15611704 5941.94457249
-     5942.06535486]
+    [ 130.57472018  501.34744442 1066.59182074 1760.50163608 2502.13955554
+     3218.50667597 3892.81448231 4455.36403436 4869.66609313 5201.99745378
+     5429.02043984 5567.28370644 5659.24831854 5695.06577065 5783.46217755
+     5824.01080702 5825.59003768 5818.22316662 5866.52307412 5896.96917375
+     5948.92254787 5968.30540534 5931.15611704 5941.94457249 5942.06535486]
 
     >>> print(cog.profile_error)  # doctest: +FLOAT_CMP
-    [  0.           5.32777186   9.37111012  13.41750992  16.62928904
-      21.7350922   25.39862532  30.3867526   34.11478867  39.28263973
-      43.96047829  48.11931395  52.00967328  55.7471834   60.48824739
-      64.81392778  68.71042311  72.71899201  76.54959872  81.33806741
-      85.98568713  91.34841248  95.5173253   99.22190499 102.51980185
-     106.83601366]
+    [  5.32777186   9.37111012  13.41750992  16.62928904  21.7350922
+      25.39862532  30.3867526   34.11478867  39.28263973  43.96047829
+      48.11931395  52.00967328  55.7471834   60.48824739  64.81392778
+      68.71042311  72.71899201  76.54959872  81.33806741  85.98568713
+      91.34841248  95.5173253   99.22190499 102.51980185 106.83601366]
 
     Plot the curve of growth.
 
     .. plot::
 
         import matplotlib.pyplot as plt
         import numpy as np
@@ -145,19 +138,16 @@
         error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
         data += error
 
         # find the source centroid
         xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
 
         # create the curve of growth
-        min_radius = 0.0
-        max_radius = 25.0
-        radius_step = 1.0
-        cog = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                            error=error, mask=None)
+        radii = np.arange(1, 26)
+        cog = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
 
         # plot the curve of growth
         cog.plot()
         cog.plot_error()
 
     Normalize the profile and plot the normalized curve of growth.
 
@@ -179,19 +169,16 @@
         error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
         data += error
 
         # find the source centroid
         xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
 
         # create the curve of growth
-        min_radius = 0.0
-        max_radius = 25.0
-        radius_step = 1.0
-        cog = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                            error=error, mask=None)
+        radii = np.arange(1, 26)
+        cog = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
 
         # plot the curve of growth
         cog.normalize()
         cog.plot()
         cog.plot_error()
 
     Plot a couple of the apertures on the data.
@@ -214,30 +201,33 @@
         error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
         data += error
 
         # find the source centroid
         xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
 
         # create the curve of growth
-        min_radius = 0.0
-        max_radius = 25.0
-        radius_step = 1.0
-        cog = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                            error=error, mask=None)
+        radii = np.arange(1, 26)
+        cog = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
 
         norm = simple_norm(data, 'sqrt')
         plt.figure(figsize=(5, 5))
         plt.imshow(data, norm=norm)
         cog.apertures[5].plot(color='C0', lw=2)
         cog.apertures[10].plot(color='C1', lw=2)
     """
 
-    @lazyproperty
-    def _circular_radii(self):
-        return self.radius
+    def __init__(self, data, xycen, radii, *, error=None, mask=None,
+                 method='exact', subpixels=5):
+
+        radii = np.array(radii)
+        if radii.min() <= 0:
+            raise ValueError('radii must be > 0')
+
+        super().__init__(data, xycen, radii, error=error, mask=mask,
+                         method=method, subpixels=subpixels)
 
     @lazyproperty
     def apertures(self):
         """
         A list of `~photutils.aperture.CircularAperture` objects used to
         measure the profile.
```

### Comparing `photutils-1.7.0/photutils/profiles/radial_profile.py` & `photutils-1.8.0/photutils/profiles/radial_profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 This module provides tools for generating radial profiles.
 """
 
-import math
 import warnings
 
 import numpy as np
 from astropy.modeling.fitting import LevMarLSQFitter
 from astropy.modeling.models import Gaussian1D
 from astropy.stats import gaussian_sigma_to_fwhm
 from astropy.utils import lazyproperty
@@ -17,44 +16,48 @@
 __all__ = ['RadialProfile']
 
 __doctest_requires__ = {('RadialProfile'): ['scipy']}
 
 
 class RadialProfile(ProfileBase):
     """
-    Class to create a radial profile using concentric apertures.
+    Class to create a radial profile using concentric circular
+    apertures.
 
     The radial profile represents the azimuthally-averaged flux in
     circular annuli apertures as a function of radius.
 
-    Non-finite values (e.g., NaN or inf) in the ``data`` or ``error``
-    array are automatically masked.
+    For this class, the input radii represent the edges of the radial
+    bins. This differs from the `RadialProfile` class, where the inputs
+    represent the centers of the radial bins.
 
     Parameters
     ----------
     data : 2D `numpy.ndarray`
         The 2D data array. The data should be background-subtracted.
+        Non-finite values (e.g., NaN or inf) in the ``data`` or
+        ``error`` array are automatically masked.
 
     xycen : tuple of 2 floats
         The ``(x, y)`` pixel coordinate of the source center.
 
-    min_radius : float
-        The minimum radius for the profile.
-
-    max_radius : float
-        The maximum radius for the profile.
-
-    radius_step : float
-        The radial step size in pixels.
+    edge_radii : 1D float `numpy.ndarray`
+        An array of radii defining the edges of the radial bins.
+        ``edge_radii`` must be strictly increasing with a minimum value
+        greater than or equal to zero, and contain at least 2 values.
+        The radial spacing does not need to be constant. The output
+        `radius` attribute will be defined at the bin centers.
 
     error : 2D `numpy.ndarray`, optional
         The 1-sigma errors of the input ``data``. ``error`` is assumed
         to include all sources of error, including the Poisson error
         of the sources (see `~photutils.utils.calc_total_error`) .
         ``error`` must have the same shape as the input ``data``.
+        Non-finite values (e.g., NaN or inf) in the ``data`` or
+        ``error`` array are automatically masked.
 
     mask : 2D bool `numpy.ndarray`, optional
         A boolean mask with the same shape as ``data`` where a `True`
         value indicates the corresponding element of ``data`` is masked.
         Masked data are excluded from all calculations.
 
     method : {'exact', 'center', 'subpixel'}, optional
@@ -82,20 +85,23 @@
 
     subpixels : int, optional
         For the ``'subpixel'`` method, resample pixels by this factor
         in each dimension. That is, each pixel is divided into
         ``subpixels**2`` subpixels. This keyword is ignored unless
         ``method='subpixel'``.
 
+    See Also
+    --------
+    RadialProfile
+
     Notes
     -----
-    If the ``min_radius`` is less than or equal to half the
-    ``radius_step``, then a circular aperture with radius equal to
-    ``min_radius + 0.5 * radius_step`` will be used for the innermost
-    aperture.
+    If the minimum of ``edge_radii`` is zero, then a circular aperture
+    with radius equal to ``edge_radii[1]`` will be used for the
+    innermost aperture.
 
     Examples
     --------
     >>> import numpy as np
     >>> from astropy.modeling.models import Gaussian2D
     >>> from astropy.visualization import simple_norm
     >>> from photutils.centroids import centroid_quadratic
@@ -110,39 +116,36 @@
     >>> data = gmodel(xx, yy)
     >>> error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
     >>> data += error
 
     Create the radial profile.
 
     >>> xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
-    >>> min_radius = 0.0
-    >>> max_radius = 25.0
-    >>> radius_step = 1.0
-    >>> rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-    ...                    error=error, mask=None)
+    >>> edge_radii = np.arange(26)
+    >>> rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
     >>> print(rp.radius)  # doctest: +FLOAT_CMP
-    [ 0.  1.  2.  3.  4.  5.  6.  7.  8.  9. 10. 11. 12. 13. 14. 15. 16. 17.
-     18. 19. 20. 21. 22. 23. 24. 25.]
+    [ 0.5  1.5  2.5  3.5  4.5  5.5  6.5  7.5  8.5  9.5 10.5 11.5 12.5 13.5
+     14.5 15.5 16.5 17.5 18.5 19.5 20.5 21.5 22.5 23.5 24.5]
 
     >>> print(rp.profile)  # doctest: +FLOAT_CMP
-    [ 4.27430150e+01  4.02150658e+01  3.81601146e+01  3.38116846e+01
-      2.89343205e+01  2.34250297e+01  1.84368533e+01  1.44310461e+01
-      9.55543388e+00  6.55415896e+00  4.49693014e+00  2.56010523e+00
-      1.50362911e+00  7.35389056e-01  6.04663625e-01  8.08820954e-01
-      2.31751912e-01 -1.39063329e-01  1.25181410e-01  4.84601845e-01
-      1.94567871e-01  4.49109676e-01 -2.00995374e-01 -7.74387397e-02
-      5.70302749e-02 -3.27578439e-02]
+    [ 4.15632243e+01  3.93402079e+01  3.59845746e+01  3.15540506e+01
+      2.62300757e+01  2.07297033e+01  1.65106801e+01  1.19376723e+01
+      7.75743772e+00  5.56759777e+00  3.44112671e+00  1.91350281e+00
+      1.17092981e+00  4.22261078e-01  9.70256904e-01  4.16355795e-01
+      1.52328707e-02 -6.69985111e-02  4.15522650e-01  2.48494731e-01
+      4.03348112e-01  1.43482678e-01 -2.62777461e-01  7.30653622e-02
+      7.84616804e-04]
 
     >>> print(rp.profile_error)  # doctest: +FLOAT_CMP
-    [2.95008692 1.17855895 0.6610777  0.51902503 0.47524302 0.43072819
-     0.39770113 0.37667594 0.33909996 0.35356048 0.30377721 0.29455808
-     0.25670656 0.26599511 0.27354232 0.2430305  0.22910334 0.22204777
-     0.22327174 0.23816561 0.2343794  0.2232632  0.19893783 0.17888776
-     0.18228289 0.19680823]
+    [1.69588246 0.81797694 0.61132694 0.44670831 0.49499835 0.38025361
+     0.40844702 0.32906672 0.36466713 0.33059274 0.29661894 0.27314739
+     0.25551933 0.27675376 0.25553986 0.23421017 0.22966813 0.21747036
+     0.23654884 0.22760386 0.23941711 0.20661313 0.18999134 0.17469024
+     0.19527558]
 
     Plot the radial profile.
 
     .. plot::
 
         import matplotlib.pyplot as plt
         import numpy as np
@@ -160,19 +163,16 @@
         error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
         data += error
 
         # find the source centroid
         xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
 
         # create the radial profile
-        min_radius = 0.0
-        max_radius = 25.0
-        radius_step = 1.0
-        rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                           error=error, mask=None)
+        edge_radii = np.arange(26)
+        rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
         # plot the radial profile
         rp.plot()
         rp.plot_error()
 
     Normalize the profile and plot the normalized radial profile.
 
@@ -194,19 +194,16 @@
         error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
         data += error
 
         # find the source centroid
         xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
 
         # create the radial profile
-        min_radius = 0.0
-        max_radius = 25.0
-        radius_step = 1.0
-        rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                           error=error, mask=None)
+        edge_radii = np.arange(26)
+        rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
         # plot the radial profile
         rp.normalize()
         rp.plot()
         rp.plot_error()
 
     Plot two of the annulus apertures on the data.
@@ -229,34 +226,31 @@
         error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
         data += error
 
         # find the source centroid
         xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
 
         # create the radial profile
-        min_radius = 0.0
-        max_radius = 25.0
-        radius_step = 1.0
-        rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                           error=error, mask=None)
+        edge_radii = np.arange(26)
+        rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
         norm = simple_norm(data, 'sqrt')
         plt.figure(figsize=(5, 5))
         plt.imshow(data, norm=norm)
         rp.apertures[5].plot(color='C0', lw=2)
         rp.apertures[10].plot(color='C1', lw=2)
 
     Fit a 1D Gaussian to the radial profile and return the Gaussian
     model.
 
     >>> rp.gaussian_fit  # doctest: +FLOAT_CMP
-    <Gaussian1D(amplitude=41.80620963, mean=0., stddev=4.69126969)>
+    <Gaussian1D(amplitude=41.54880743, mean=0., stddev=4.71059406)>
 
     >>> print(rp.gaussian_fwhm)  # doctest: +FLOAT_CMP
-    11.04709589620093
+    11.09260130738712
 
     Plot the fitted 1D Gaussian on the radial profile.
 
     .. plot::
 
         import matplotlib.pyplot as plt
         import numpy as np
@@ -274,41 +268,33 @@
         error = make_noise_image(data.shape, mean=0., stddev=2.4, seed=123)
         data += error
 
         # find the source centroid
         xycen = centroid_quadratic(data, xpeak=48, ypeak=52)
 
         # create the radial profile
-        min_radius = 0.0
-        max_radius = 25.0
-        radius_step = 1.0
-        rp = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                           error=error, mask=None)
+        edge_radii = np.arange(26)
+        rp = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
 
         # plot the radial profile
         rp.normalize()
         rp.plot(label='Radial Profile')
         rp.plot_error()
         plt.plot(rp.radius, rp.gaussian_profile, label='Gaussian Fit')
         plt.legend()
     """
 
     @lazyproperty
-    def _circular_radii(self):
+    def radius(self):
         """
-        The circular aperture radii for the radial bin edges (inner and
-        outer annulus radii).
+        The profile radius (bin centers) in pixels as a 1D
+        `~numpy.ndarray`.
         """
-        shift = self.radius_step / 2
-        min_radius = self.min_radius - shift
-        max_radius = self.max_radius + shift
-        nsteps = int(math.floor((max_radius - min_radius)
-                                / self.radius_step))
-        max_radius = min_radius + (nsteps * self.radius_step)
-        return np.linspace(min_radius, max_radius, nsteps + 1)
+        # define the radial bin centers from the radial bin edges
+        return (self.radii[:-1] + self.radii[1:]) / 2
 
     @lazyproperty
     def apertures(self):
         """
         A list of the circular annulus apertures used to measure the
         radial profile.
 
@@ -316,21 +302,21 @@
         ``radius_step``, then a circular aperture with radius equal
         to ``min_radius + 0.5 * radius_step`` will be used for the
         innermost aperture.
         """
         from photutils.aperture import CircularAnnulus, CircularAperture
 
         apertures = []
-        for i in range(len(self._circular_radii) - 1):
+        for i in range(len(self.radii) - 1):
             try:
-                aperture = CircularAnnulus(self.xycen, self._circular_radii[i],
-                                           self._circular_radii[i + 1])
+                aperture = CircularAnnulus(self.xycen, self.radii[i],
+                                           self.radii[i + 1])
             except ValueError:  # zero radius
                 aperture = CircularAperture(self.xycen,
-                                            self._circular_radii[i + 1])
+                                            self.radii[i + 1])
             apertures.append(aperture)
 
         return apertures
 
     @lazyproperty
     def _flux(self):
         """
```

### Comparing `photutils-1.7.0/photutils/profiles/tests/test_curve_of_growth.py` & `photutils-1.8.0/photutils/profiles/tests/test_curve_of_growth.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,93 +34,73 @@
 
     return xycen, data, error, mask
 
 
 def test_curve_of_growth(profile_data):
     xycen, data, _, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-    cg1 = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=None)
+    radii = np.arange(1, 37)
+    cg1 = CurveOfGrowth(data, xycen, radii, error=None, mask=None)
 
-    assert_equal(cg1.radius, np.arange(36))
+    assert_equal(cg1.radius, radii)
     assert cg1.area.shape == (36,)
     assert cg1.profile.shape == (36,)
     assert cg1.profile_error.shape == (0,)
-    assert cg1.area[0] == 0.0
+    assert_allclose(cg1.area[0], np.pi)
 
     assert len(cg1.apertures) == 36
-    assert cg1.apertures[0] is None
-    assert isinstance(cg1.apertures[1], CircularAperture)
+    assert isinstance(cg1.apertures[0], CircularAperture)
 
-    min_radius = 1.0
-    max_radius = 35.0
-    radius_step = 1.0
-    cg2 = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=None)
+    radii = np.arange(1, 36)
+    cg2 = CurveOfGrowth(data, xycen, radii, error=None, mask=None)
     assert cg2.area[0] > 0.0
     assert isinstance(cg2.apertures[0], CircularAperture)
 
 
 def test_curve_of_growth_units(profile_data):
     xycen, data, error, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
+    radii = np.arange(1, 36)
     unit = u.Jy
-    cg1 = CurveOfGrowth(data << unit, xycen, min_radius, max_radius,
-                        radius_step, error=error << unit, mask=None)
+    cg1 = CurveOfGrowth(data << unit, xycen, radii, error=error << unit,
+                        mask=None)
 
     assert cg1.profile.unit == unit
     assert cg1.profile_error.unit == unit
 
     with pytest.raises(ValueError):
-        CurveOfGrowth(data << unit, xycen, min_radius, max_radius, radius_step,
-                      error=error, mask=None)
+        CurveOfGrowth(data << unit, xycen, radii, error=error, mask=None)
 
 
 def test_curve_of_growth_error(profile_data):
     xycen, data, error, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-    cg1 = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=error, mask=None)
+    radii = np.arange(1, 36)
+    cg1 = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
 
-    assert cg1.profile.shape == (36,)
-    assert cg1.profile_error.shape == (36,)
+    assert cg1.profile.shape == (35,)
+    assert cg1.profile_error.shape == (35,)
 
 
 def test_curve_of_growth_mask(profile_data):
     xycen, data, error, mask = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-    cg1 = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=error, mask=None)
-    cg2 = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=error, mask=mask)
+    radii = np.arange(1, 36)
+    cg1 = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
+    cg2 = CurveOfGrowth(data, xycen, radii, error=error, mask=mask)
 
     assert cg1.profile.sum() > cg2.profile.sum()
     assert np.sum(cg1.profile_error**2) > np.sum(cg2.profile_error**2)
 
 
 def test_curve_of_growth_normalize(profile_data):
     xycen, data, _, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-    cg1 = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=None)
+    radii = np.arange(1, 36)
+    cg1 = CurveOfGrowth(data, xycen, radii, error=None, mask=None)
 
     profile1 = cg1.profile
     cg1.normalize()
     profile2 = cg1.profile
     assert np.mean(profile2) < np.mean(profile1)
 
     cg1.normalize(method='sum')
@@ -135,61 +115,53 @@
     with pytest.warns(AstropyUserWarning, match=msg):
         cg1.normalize(method='max')
 
 
 def test_curve_of_growth_inputs(profile_data):
     xycen, data, error, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-
-    with pytest.raises(ValueError):
-        CurveOfGrowth(data, xycen, -1, max_radius, radius_step, error=None,
+    msg = 'radii must be > 0'
+    with pytest.raises(ValueError, match=msg):
+        radii = np.arange(10)
+        CurveOfGrowth(data, xycen, radii, error=None, mask=None)
+
+    msg = 'radii must be a 1D array and have at least two values'
+    with pytest.raises(ValueError, match=msg):
+        CurveOfGrowth(data, xycen, [1], error=None, mask=None)
+    with pytest.raises(ValueError, match=msg):
+        CurveOfGrowth(data, xycen, np.arange(1, 7).reshape(2, 3), error=None,
                       mask=None)
-    with pytest.raises(ValueError):
-        CurveOfGrowth(data, xycen, 10.0, 1.0, radius_step, error=None,
-                      mask=None)
-    with pytest.raises(ValueError):
-        CurveOfGrowth(data, xycen, min_radius, max_radius, -1.0, error=None,
-                      mask=None)
-    with pytest.raises(ValueError):
-        CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                      error=np.ones((3, 3)), mask=None)
-    with pytest.raises(ValueError):
-        CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                      error=None, mask=np.ones((3, 3)))
+
+    msg = 'radii must be strictly increasing'
+    with pytest.raises(ValueError, match=msg):
+        radii = np.arange(1, 10)[::-1]
+        CurveOfGrowth(data, xycen, radii, error=None, mask=None)
 
     with pytest.raises(ValueError):
         unit1 = u.Jy
         unit2 = u.km
-        CurveOfGrowth(data << unit1, xycen, min_radius, max_radius,
-                      radius_step, error=error << unit2)
+        radii = np.arange(1, 36)
+        CurveOfGrowth(data << unit1, xycen, radii, error=error << unit2)
 
 
 @pytest.mark.skipif(not HAS_MATPLOTLIB, reason='matplotlib is required')
 def test_curve_of_growth_plot(profile_data):
     xycen, data, error, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-
-    cg1 = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=None)
+    radii = np.arange(1, 36)
+    cg1 = CurveOfGrowth(data, xycen, radii, error=None, mask=None)
     cg1.plot()
     with pytest.warns(AstropyUserWarning, match='Errors were not input'):
         cg1.plot_error()
 
-    cg2 = CurveOfGrowth(data, xycen, min_radius, max_radius, radius_step,
-                        error=error, mask=None)
+    cg2 = CurveOfGrowth(data, xycen, radii, error=error, mask=None)
     cg2.plot()
     pc1 = cg2.plot_error()
     assert_allclose(pc1.get_facecolor(), [[0.5, 0.5, 0.5, 0.3]])
     pc2 = cg2.plot_error(facecolor='blue')
     assert_allclose(pc2.get_facecolor(), [[0, 0, 1, 1]])
 
     unit = u.Jy
-    cg3 = CurveOfGrowth(data << unit, xycen, min_radius, max_radius,
-                        radius_step, error=error << unit, mask=None)
+    cg3 = CurveOfGrowth(data << unit, xycen, radii, error=error << unit,
+                        mask=None)
     cg3.plot()
     cg3.plot_error()
```

### Comparing `photutils-1.7.0/photutils/profiles/tests/test_radial_profile.py` & `photutils-1.8.0/photutils/profiles/tests/test_radial_profile.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,134 +34,141 @@
 
     return xycen, data, error, mask
 
 
 def test_radial_profile(profile_data):
     xycen, data, _, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-    rp1 = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=None)
-
-    assert_equal(rp1.radius, np.arange(36))
-    assert rp1.area.shape == (36,)
-    assert rp1.profile.shape == (36,)
+    edge_radii = np.arange(36)
+    rp1 = RadialProfile(data, xycen, edge_radii, error=None, mask=None)
+
+    assert_equal(rp1.radius, np.arange(35) + 0.5)
+    assert rp1.area.shape == (35,)
+    assert rp1.profile.shape == (35,)
     assert rp1.profile_error.shape == (0,)
     assert rp1.area[0] > 0.0
 
-    assert len(rp1.apertures) == 36
+    assert len(rp1.apertures) == 35
     assert isinstance(rp1.apertures[0], CircularAperture)
     assert isinstance(rp1.apertures[1], CircularAnnulus)
 
-    min_radius = 0.7
-    max_radius = 35.0
-    radius_step = 1.0
-    rp2 = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=None)
+    edge_radii = np.arange(36) + 0.1
+    rp2 = RadialProfile(data, xycen, edge_radii, error=None, mask=None)
     assert isinstance(rp2.apertures[0], CircularAnnulus)
 
 
+def test_radial_profile_inputs(profile_data):
+    xycen, data, _, _ = profile_data
+
+    msg = 'minimum edge_radii must be >= 0'
+    with pytest.raises(ValueError, match=msg):
+        edge_radii = np.arange(-1, 10)
+        RadialProfile(data, xycen, edge_radii, error=None, mask=None)
+
+    msg = 'edge_radii must be a 1D array and have at least two values'
+    with pytest.raises(ValueError, match=msg):
+        edge_radii = [1]
+        RadialProfile(data, xycen, edge_radii, error=None, mask=None)
+    with pytest.raises(ValueError, match=msg):
+        edge_radii = np.arange(6).reshape(2, 3)
+        RadialProfile(data, xycen, edge_radii, error=None, mask=None)
+
+    msg = 'edge_radii must be strictly increasing'
+    with pytest.raises(ValueError, match=msg):
+        edge_radii = np.arange(10)[::-1]
+        RadialProfile(data, xycen, edge_radii, error=None, mask=None)
+
+    msg = 'error must have the same shape as data'
+    with pytest.raises(ValueError, match=msg):
+        edge_radii = np.arange(10)
+        RadialProfile(data, xycen, edge_radii, error=np.ones(3), mask=None)
+
+    msg = 'mask must have the same shape as data'
+    with pytest.raises(ValueError, match=msg):
+        edge_radii = np.arange(10)
+        mask = np.ones(3, dtype=bool)
+        RadialProfile(data, xycen, edge_radii, error=None, mask=mask)
+
+
 @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
 def test_radial_profile_gaussian(profile_data):
     xycen, data, _, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-    rp1 = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=None)
+    edge_radii = np.arange(36)
+    rp1 = RadialProfile(data, xycen, edge_radii, error=None, mask=None)
 
     assert isinstance(rp1.gaussian_fit, Gaussian1D)
-    assert rp1.gaussian_profile.shape == (36,)
+    assert rp1.gaussian_profile.shape == (35,)
     assert rp1.gaussian_fwhm < 23.6
 
-    max_radius = 200
-    rp2 = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=None)
+    edge_radii = np.arange(201)
+    rp2 = RadialProfile(data, xycen, edge_radii, error=None, mask=None)
     assert isinstance(rp2.gaussian_fit, Gaussian1D)
-    assert rp2.gaussian_profile.shape == (201,)
+    assert rp2.gaussian_profile.shape == (200,)
     assert rp2.gaussian_fwhm < 23.6
 
 
 def test_radial_profile_unit(profile_data):
     xycen, data, error, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
+    edge_radii = np.arange(36)
     unit = u.Jy
-    rp1 = RadialProfile(data << unit, xycen, min_radius, max_radius,
-                        radius_step, error=error << unit, mask=None)
+    rp1 = RadialProfile(data << unit, xycen, edge_radii, error=error << unit,
+                        mask=None)
     assert rp1.profile.unit == unit
     assert rp1.profile_error.unit == unit
 
     with pytest.raises(ValueError):
-        RadialProfile(data << unit, xycen, min_radius, max_radius, radius_step,
-                      error=error, mask=None)
+        RadialProfile(data << unit, xycen, edge_radii, error=error, mask=None)
 
 
 def test_radial_profile_error(profile_data):
     xycen, data, error, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-    rp1 = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                        error=error, mask=None)
-
-    assert_equal(rp1.radius, np.arange(36))
-    assert rp1.area.shape == (36,)
-    assert rp1.profile.shape == (36,)
-    assert rp1.profile_error.shape == (36,)
+    edge_radii = np.arange(36)
+    rp1 = RadialProfile(data, xycen, edge_radii, error=error, mask=None)
+
+    assert_equal(rp1.radius, np.arange(35) + 0.5)
+    assert rp1.area.shape == (35,)
+    assert rp1.profile.shape == (35,)
+    assert rp1.profile_error.shape == (35,)
 
-    assert len(rp1.apertures) == 36
+    assert len(rp1.apertures) == 35
     assert isinstance(rp1.apertures[0], CircularAperture)
     assert isinstance(rp1.apertures[1], CircularAnnulus)
 
 
 def test_radial_profile_normalize_nan(profile_data):
     """
     If the profile has NaNs (e.g., aperture outside of the image),
     make sure the normalization ignores them.
     """
     xycen, data, _, _ = profile_data
 
-    min_radius = 0.0
-    max_radius = 100.0
-    radius_step = 1.0
-
-    rp1 = RadialProfile(data, xycen, min_radius, max_radius, radius_step)
+    edge_radii = np.arange(101)
+    rp1 = RadialProfile(data, xycen, edge_radii)
     rp1.normalize()
     assert not np.isnan(rp1.profile[0])
 
 
 def test_radial_profile_nonfinite(profile_data):
     xycen, data, error, _ = profile_data
     data2 = data.copy()
     data2[40, 40] = np.nan
     mask = ~np.isfinite(data2)
 
-    min_radius = 0.0
-    max_radius = 35.0
-    radius_step = 1.0
-
-    rp1 = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                        error=None, mask=mask)
+    edge_radii = np.arange(36)
+    rp1 = RadialProfile(data, xycen, edge_radii, error=None, mask=mask)
 
-    rp2 = RadialProfile(data2, xycen, min_radius, max_radius, radius_step,
-                        error=error, mask=mask)
+    rp2 = RadialProfile(data2, xycen, edge_radii, error=error, mask=mask)
     assert_allclose(rp1.profile, rp2.profile)
 
     msg = 'Input data contains non-finite values'
     with pytest.warns(AstropyUserWarning, match=msg):
-        rp3 = RadialProfile(data2, xycen, min_radius, max_radius, radius_step,
-                            error=error, mask=None)
+        rp3 = RadialProfile(data2, xycen, edge_radii, error=error, mask=None)
         assert_allclose(rp1.profile, rp3.profile)
 
     error2 = error.copy()
     error2[40, 40] = np.inf
     with pytest.warns(AstropyUserWarning, match=msg):
-        rp4 = RadialProfile(data, xycen, min_radius, max_radius, radius_step,
-                            error=error2, mask=None)
+        rp4 = RadialProfile(data, xycen, edge_radii, error=error2, mask=None)
         assert_allclose(rp1.profile, rp4.profile)
```

### Comparing `photutils-1.7.0/photutils/psf/__init__.py` & `photutils-1.8.0/photutils/psf/__init__.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/epsf.py` & `photutils-1.8.0/photutils/psf/epsf.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/epsf_stars.py` & `photutils-1.8.0/photutils/psf/epsf_stars.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/groupstars.py` & `photutils-1.8.0/photutils/psf/groupstars.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/matching/fourier.py` & `photutils-1.8.0/photutils/psf/matching/fourier.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/matching/tests/test_fourier.py` & `photutils-1.8.0/photutils/psf/matching/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/matching/tests/test_windows.py` & `photutils-1.8.0/photutils/psf/matching/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/matching/windows.py` & `photutils-1.8.0/photutils/psf/matching/windows.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/models.py` & `photutils-1.8.0/photutils/psf/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -765,15 +765,15 @@
         # @lru_cache/cache to prevent memory leaks
         self._compute_local_model = lru_cache(maxsize=128)(
             self._compute_local_model_uncached)
 
         super().__init__(flux, x_0, y_0)
 
     @staticmethod
-    def _find_bounds_1d(data, x):
+    def _find_start_idx(data, x):
         """
         Find the index of the lower bound where ``x`` should be inserted
         into ``a`` to maintain order.
 
         The index of the upper bound is the index of the lower bound
         plus 2.  Both bound indices must be within the array.
 
@@ -793,49 +793,41 @@
         idx = np.searchsorted(data, x)
         if idx == 0:
             idx0 = 0
         elif idx == len(data):  # pragma: no cover
             idx0 = idx - 2
         else:
             idx0 = idx - 1
-
         return idx0
 
     def _find_bounding_points(self, x, y):
         """
         Find the indices of the grid points that bound the input
         ``(x, y)`` position.
 
         Parameters
         ----------
         x, y : float
             The ``(x, y)`` position where the PSF is to be evaluated.
+            The position must be inside the region defined by the grid
+            of PSF positions.
 
         Returns
         -------
         indices : list of int
             A list of indices of the bounding grid points.
         """
-        if not np.isscalar(x) or not np.isscalar(y):  # pragma: no cover
-            raise TypeError('x and y must be scalars')
-
-        if (x < self._xgrid_min
-                or x > self._xgrid_max
-                or y < self._ygrid_min
-                or y > self._ygrid_max):  # pragma: no cover
-            raise ValueError('(x, y) position is outside of the region '
-                             'defined by grid of PSF positions')
-
-        x0 = self._find_bounds_1d(self._xgrid, x)
-        y0 = self._find_bounds_1d(self._ygrid, y)
-        points = list(itertools.product(self._xgrid[x0:x0 + 2],
-                                        self._ygrid[y0:y0 + 2]))
+        x0 = self._find_start_idx(self._xgrid, x)
+        y0 = self._find_start_idx(self._ygrid, y)
+        xypoints = list(itertools.product(self._xgrid[x0:x0 + 2],
+                                          self._ygrid[y0:y0 + 2]))
 
+        # find the grid_xypos indices of the reference xypoints
         indices = []
-        for xx, yy in points:
+        for xx, yy in xypoints:
             indices.append(np.argsort(np.hypot(self._grid_xpos - xx,
                                                self._grid_ypos - yy))[0])
 
         return indices
 
     @staticmethod
     def _bilinear_interp(xyref, zref, xi, yi):
@@ -859,21 +851,14 @@
             rectangle defined by ``xyref``.
 
         Returns
         -------
         result : 2D `~numpy.ndarray`
             The 2D interpolated array.
         """
-        if len(xyref) != 4:
-            raise ValueError('xyref must contain only 4 (x, y) pairs')
-
-        if zref.shape[0] != 4:
-            raise ValueError('zref must have a length of 4 on the first '
-                             'axis.')
-
         xyref = [tuple(i) for i in xyref]
         idx = sorted(range(len(xyref)), key=xyref.__getitem__)
         xyref = sorted(xyref)  # sort by x, then y
         (x0, y0), (_x0, y1), (x1, _y0), (_x1, _y1) = xyref
 
         if x0 != _x0 or x1 != _x1 or y0 != _y0 or y1 != _y1:
             raise ValueError('The refxy points do not form a rectangle.')
@@ -896,20 +881,19 @@
 
     def _compute_local_model_uncached(self, x_0, y_0):
         """
         Return `FittableImageModel` for interpolated PSF at some (x_0, y_0).
         """
         if (x_0 < self._xgrid_min or x_0 > self._xgrid_max
                 or y_0 < self._ygrid_min or y_0 > self._ygrid_max):
-
             # position is outside of the grid, so simply use the
             # closest reference PSF
-            self._ref_indices = np.argsort(np.hypot(self._grid_xpos - x_0,
-                                                    self._grid_ypos - y_0))[0]
-            self._psf_interp = self.data[self._ref_indices, :, :]
+            self._ref_index = np.argsort(np.hypot(self._grid_xpos - x_0,
+                                                  self._grid_ypos - y_0))[0]
+            self._psf_interp = self.data[self._ref_index, :, :]
         else:
             # find the four bounding reference PSFs and interpolate
             self._ref_indices = self._find_bounding_points(x_0, y_0)
             xyref = np.array(self.grid_xypos)[self._ref_indices]
             psfs = self.data[self._ref_indices, :, :]
 
             self._psf_interp = self._bilinear_interp(xyref, psfs, x_0, y_0)
@@ -919,25 +903,27 @@
                                       oversampling=self.oversampling)
         return psfmodel
 
     def evaluate(self, x, y, flux, x_0, y_0):
         """
         Evaluate the `GriddedPSFModel` for the input parameters.
         """
-        # NOTE: this is needed because the PSF photometry routines input
-        # length-1 values instead of scalars.  TODO: fix the photometry
-        # routines.
+        # NOTE: the astropy base Model.__call__() method converts scalar
+        # inputs to size-1 arrays before calling evaluate().
+        if not np.isscalar(flux):
+            flux = flux[0]
         if not np.isscalar(x_0):
             x_0 = x_0[0]
         if not np.isscalar(y_0):
             y_0 = y_0[0]
 
-        # calculate the local (interpolated) PSF at (x_0, y_0) from the
-        # grid of PSF models
-        psfmodel = self._compute_local_model(x_0, y_0)
+        # Calculate the local (interpolated) PSF at (x_0, y_0) from the
+        # grid of PSF models. Only the integer part of the position is
+        # input so that the local model can be cached.
+        psfmodel = self._compute_local_model(int(x_0), int(y_0))
 
         # now evaluate the PSF at the (x_0, y_0) subpixel position on
         # the input (x, y) values
         return psfmodel.evaluate(x, y, flux, x_0, y_0)
 
 
 class IntegratedGaussianPRF(Fittable2DModel):
@@ -1089,14 +1075,21 @@
         # used in the future to expose how the integration happens
         self._dblquadkwargs = {}
 
         super().__init__(n_models=1, x_0=x_0, y_0=y_0, flux=flux, **kwargs)
 
     def evaluate(self, x, y, flux, x_0, y_0):
         """The evaluation function for PRFAdapter."""
+        if not np.isscalar(flux):
+            flux = flux[0]
+        if not np.isscalar(x_0):
+            x_0 = x_0[0]
+        if not np.isscalar(y_0):
+            y_0 = y_0[0]
+
         if self.xname is None:
             dx = x - x_0
         else:
             dx = x
             setattr(self.psfmodel, self.xname, x_0)
 
         if self.xname is None:
```

### Comparing `photutils-1.7.0/photutils/psf/photometry.py` & `photutils-1.8.0/photutils/psf/photometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/tests/test_epsf.py` & `photutils-1.8.0/photutils/psf/tests/test_epsf.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/tests/test_epsf_stars.py` & `photutils-1.8.0/photutils/psf/tests/test_epsf_stars.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/tests/test_groupstars.py` & `photutils-1.8.0/photutils/psf/tests/test_groupstars.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/tests/test_models.py` & `photutils-1.8.0/photutils/psf/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,23 +161,17 @@
         y, x = np.mgrid[170:270, 170:270]
         psf4 = self.psfmodel.evaluate(x=x, y=y, flux=100, x_0=220, y_0=220)
         assert_allclose(psf3, psf4)
 
     @pytest.mark.skipif(not HAS_SCIPY, reason='scipy is required')
     def test_gridded_psf_model_interp(self):
         # test xyref length
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             self.psfmodel._bilinear_interp([1, 1], 1, 1, 1)
 
-        # test zref shape
-        with pytest.raises(ValueError):
-            xyref = [[0, 0], [0, 1], [1, 0], [1, 1]]
-            zref = np.ones((3, 4, 4))
-            self.psfmodel._bilinear_interp(xyref, zref, 1, 1)
-
         # test if refxy points form a rectangle
         with pytest.raises(ValueError):
             xyref = [[0, 0], [0, 1], [1, 0], [2, 2]]
             zref = np.ones((4, 4, 4))
             self.psfmodel._bilinear_interp(xyref, zref, 1, 1)
 
         # test if xi and yi are outside of xyref
```

### Comparing `photutils-1.7.0/photutils/psf/tests/test_photometry.py` & `photutils-1.8.0/photutils/psf/tests/test_photometry.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/tests/test_utils.py` & `photutils-1.8.0/photutils/psf/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/psf/utils.py` & `photutils-1.8.0/photutils/psf/utils.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/segmentation/catalog.py` & `photutils-1.8.0/photutils/segmentation/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,30 +86,30 @@
     Class to create a catalog of photometry and morphological properties
     for sources defined by a segmentation image.
 
     Parameters
     ----------
     data : 2D `~numpy.ndarray` or `~astropy.units.Quantity`, optional
         The 2D array from which to calculate the source photometry and
-        properties. If ``convolved_data`` (or ``kernel``) is input,
-        then a convolved version of ``data`` will be used instead of
-        ``data`` to calculate the source centroid and morphological
-        properties. Source photometry is always measured from ``data``.
-        For accurate source properties and photometry, ``data`` should
-        be background-subtracted. Non-finite ``data`` values (NaN and
-        inf) are automatically masked.
+        properties. If ``convolved_data`` is input, then a convolved
+        version of ``data`` will be used instead of ``data`` to
+        calculate the source centroid and morphological properties.
+        Source photometry is always measured from ``data``. For
+        accurate source properties and photometry, ``data`` should be
+        background-subtracted. Non-finite ``data`` values (NaN and inf)
+        are automatically masked.
 
     segment_img : `~photutils.segmentation.SegmentationImage`
         A `~photutils.segmentation.SegmentationImage` object defining
         the sources.
 
     convolved_data : 2D `~numpy.ndarray` or `~astropy.units.Quantity`, optional
         The 2D array used to calculate the source centroid and
-        morphological properties. It is recommended that the user input
-        the convolved data directly instead of using the ``kernel``
+        morphological properties. The user should input the convolved
+        data directly instead of using the deprecated ``kernel``
         keyword. If ``convolved_data`` is input, then the ``kernel``
         keyword will be ignored. If both ``convolved_data`` and
         ``kernel`` are `None`, then the unconvolved ``data`` will be
         used instead. Non-finite ``convolved_data`` values (NaN and
         inf) are not automatically masked, unless they are at the same
         position of non-finite values in the input ``data`` array. Such
         pixels can be masked using the ``mask`` keyword.
@@ -132,14 +132,17 @@
         A boolean mask with the same shape as ``data`` where a `True`
         value indicates the corresponding element of ``data`` is masked.
         Masked data are excluded from all calculations. Non-finite
         values (NaN and inf) in the input ``data`` are automatically
         masked.
 
     kernel : 2D `~numpy.ndarray` or `~astropy.convolution.Kernel2D`, optional
+        Deprecated. Please input a convolved image directly into the
+        ``convolved_data`` keyword.
+
         The 2D kernel used to filter the data prior to calculating
         the source centroid and morphological parameters. The
         kernel should be the same one used in defining the
         source segments, i.e., the detection image (e.g., see
         :func:`~photutils.segmentation.detect_sources`). If `None`, then
         the unfiltered ``data`` will be used instead. This keyword is
         ignored if ``convolved_data`` is input (recommended).
@@ -189,15 +192,15 @@
           * 'mask': mask pixels assigned to neighboring sources
             (equivalent to MASK_TYPE=BLANK in SourceExtractor).
           * 'none': do not mask any pixels (equivalent to MASK_TYPE=NONE
             in SourceExtractor).
 
         This keyword will be ignored if ``detection_cat`` is input.
 
-    kron_params : list of 2 or 3 floats, optional
+    kron_params : tuple of 2 or 3 floats, optional
         A list of parameters used to determine the Kron aperture.
         The first item is the scaling parameter of the unscaled Kron
         radius and the second item represents the minimum value for
         the unscaled Kron radius in pixels. The optional third item is
         the minimum circular radius in pixels. If ``kron_params[0]``
         * `kron_radius` * sqrt(`semimajor_sigma` * `semiminor_sigma`)
         is less than or equal to this radius, then the Kron aperture
@@ -247,18 +250,17 @@
 
     `SourceExtractor`_'s centroid and morphological parameters are
     always calculated from a convolved, or filtered, "detection"
     image (``convolved_data``), i.e., the image used to define the
     segmentation image. The usual downside of the filtering is the
     sources will be made more circular than they actually are. If
     you wish to reproduce `SourceExtractor`_ centroid and morphology
-    results, then input the ``convolved_data`` (or ``kernel``, but not
-    both). If ``convolved_data`` and ``kernel`` are both `None`, then
-    the unfiltered ``data`` will be used for the source centroid and
-    morphological parameters.
+    results, then input the ``convolved_data`` If ``convolved_data`` and
+    ``kernel`` are both `None`, then the unfiltered ``data`` will be
+    used for the source centroid and morphological parameters.
 
     Negative data values within the source segment are set to zero
     when calculating morphological properties based on image moments.
     Negative values could occur, for example, if the segmentation
     image was defined from a different image (e.g., different
     bandpass) or if the background was oversubtracted. However,
     `~photutils.segmentation.SourceCatalog.segment_flux` always includes
@@ -285,14 +287,19 @@
     ``error`` and ``background`` arrays. The mask is `True` for pixels
     outside of the source segment, masked pixels from the ``mask``
     input, or any non-finite ``data`` values (NaN and inf).
 
     .. _SourceExtractor: https://sextractor.readthedocs.io/en/latest/
     """
 
+    @deprecated_renamed_argument('kernel', None, '1.8', message='"kernel" was '
+                                 'deprecated in version 1.8 and will be '
+                                 'removed in version 1.9. Instead, please '
+                                 'input a convolved image directly into the '
+                                 '"convolved_data" parameter.')
     def __init__(self, data, segment_img, *, convolved_data=None, error=None,
                  mask=None, kernel=None, background=None, wcs=None,
                  localbkg_width=0, apermask_method='correct',
                  kron_params=(2.5, 1.4, 0.0), detection_cat=None,
                  progress_bar=False):
 
         arrays, unit = process_quantities(
@@ -382,25 +389,26 @@
     def _validate_apermask_method(apermask_method):
         if apermask_method not in ('none', 'mask', 'correct'):
             raise ValueError('Invalid apermask_method value')
         return apermask_method
 
     @staticmethod
     def _validate_kron_params(kron_params):
-        kron_params = np.atleast_1d(kron_params)
+        if np.ndim(kron_params) != 1:
+            raise ValueError('kron_params must by 1D')
         nparams = len(kron_params)
         if nparams not in (2, 3):
             raise ValueError('kron_params must have 2 or 3 elements')
         if kron_params[0] <= 0:
             raise ValueError('kron_params[0] must be > 0')
         if kron_params[1] <= 0:
             raise ValueError('kron_params[1] must be > 0')
         if nparams == 3 and kron_params[2] < 0:
             raise ValueError('kron_params[2] must be >= 0')
-        return kron_params
+        return tuple(kron_params)
 
     def _validate_detection_cat(self, detection_cat):
         if detection_cat is None:
             return None
 
         if not isinstance(detection_cat, SourceCatalog):
             raise TypeError('detection_cat must be a SourceCatalog '
@@ -2797,15 +2805,14 @@
             The circular aperture for each source. The aperture will be
             `None` where the source `centroid` position is not finite or
             where the source is completely masked.
         """
         return self._make_circular_apertures(radius)
 
     @as_scalar
-    @deprecated_renamed_argument('axes', 'ax', '1.6.0')
     def plot_circular_apertures(self, radius, ax=None, origin=(0, 0),
                                 **kwargs):
         """
         Plot circular apertures for each source on a matplotlib
         `~matplotlib.axes.Axes` instance.
 
         The aperture for each source will be centered at its `centroid`
@@ -3188,15 +3195,14 @@
             source is completely masked.
         """
         if kron_params is None:
             return self.kron_aperture
         return self._make_kron_apertures(kron_params)
 
     @as_scalar
-    @deprecated_renamed_argument('axes', 'ax', '1.6.0')
     def plot_kron_apertures(self, kron_params=None, ax=None, origin=(0, 0),
                             **kwargs):
         """
         Plot Kron apertures for each source on a matplotlib
         `~matplotlib.axes.Axes` instance.
 
         The aperture for each source will be centered at its `centroid`
```

### Comparing `photutils-1.7.0/photutils/segmentation/core.py` & `photutils-1.8.0/photutils/segmentation/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import inspect
 import warnings
 from copy import copy, deepcopy
 
 import numpy as np
 from astropy.utils import lazyproperty
-from astropy.utils.decorators import deprecated, deprecated_renamed_argument
 from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.aperture import BoundingBox
 from photutils.utils._optional_deps import HAS_RASTERIO, HAS_SHAPELY
 from photutils.utils._parameters import as_pair
 from photutils.utils.colormaps import make_random_cmap
 
@@ -1289,59 +1288,14 @@
             ax.add_patch(patch)
 
         if labels is not None:
             patches = list(patches)
 
         return patches
 
-    @deprecated('1.7.0', alternative='`plot_patches`')
-    def outline_segments(self, mask_background=False):
-        """
-        Outline the labeled segments.
-
-        The "outlines" represent the pixels *just inside* the segments,
-        leaving the background pixels unmodified.
-
-        Parameters
-        ----------
-        mask_background : bool, optional
-            Set to `True` to mask the background pixels (labels = 0) in
-            the returned array.  This is useful for overplotting the
-            segment outlines.  The default is `False`.
-
-        Returns
-        -------
-        boundaries : `~numpy.ndarray` or `~numpy.ma.MaskedArray`
-            An array with the same shape of the segmentation array
-            containing only the outlines of the labeled segments.  The
-            pixel values in the outlines correspond to the labels in the
-            segmentation array.  If ``mask_background`` is `True`, then
-            a `~numpy.ma.MaskedArray` is returned.
-        """
-        from scipy.ndimage import (generate_binary_structure, grey_dilation,
-                                   grey_erosion)
-
-        # edge connectivity
-        footprint = generate_binary_structure(self._ndim, 1)
-
-        # mode='constant' ensures outline is included on the array borders
-        eroded = grey_erosion(self.data, footprint=footprint, mode='constant',
-                              cval=0.0)
-        dilated = grey_dilation(self.data, footprint=footprint,
-                                mode='constant', cval=0.0)
-
-        outlines = ((dilated != eroded) & (self.data != 0)).astype(int)
-        outlines *= self.data
-
-        if mask_background:
-            outlines = np.ma.masked_where(outlines == 0, outlines)
-
-        return outlines
-
-    @deprecated_renamed_argument('axes', 'ax', '1.6.0')
     def imshow(self, ax=None, figsize=None, dpi=None, cmap=None, alpha=None):
         """
         Display the segmentation image in a matplotlib
         `~matplotlib.axes.Axes` instance.
 
         The segmentation image will be displayed with no interpolation
         and with the origin set to "lower".
@@ -1431,15 +1385,15 @@
         The area of the segment in pixels**2.
 
     polygon : Shapely polygon, optional
         The outline of the segment as a `Shapely
         <https://shapely.readthedocs.io/>`_ polygon.
     """
 
-    def __init__(self, segment_data, label, slices, bbox, area,
+    def __init__(self, segment_data, label, slices, bbox, area, *,
                  polygon=None):
         self._segment_data = segment_data
         self.label = label
         self.slices = slices
         self.bbox = bbox
         self.area = area
         self.polygon = polygon
```

### Comparing `photutils-1.7.0/photutils/segmentation/deblend.py` & `photutils-1.8.0/photutils/segmentation/deblend.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,72 +5,50 @@
 """
 
 import warnings
 from multiprocessing import cpu_count, get_context
 
 import numpy as np
 from astropy.units import Quantity
-from astropy.utils.decorators import deprecated_renamed_argument
 from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.segmentation.core import SegmentationImage
 from photutils.segmentation.detect import _detect_sources
 from photutils.segmentation.utils import _make_binary_structure
-from photutils.utils._convolution import _filter_data
 from photutils.utils._optional_deps import HAS_TQDM
 
 __all__ = ['deblend_sources']
 
 
-@deprecated_renamed_argument('kernel', None, '1.5', message='"kernel" was '
-                             'deprecated in version 1.5 and will be removed '
-                             'in a future version. Instead, if filtering is '
-                             'desired, please input a convolved image '
-                             'directly into the "data" parameter.')
-def deblend_sources(data, segment_img, npixels, kernel=None, labels=None,
-                    nlevels=32, contrast=0.001, mode='exponential',
-                    connectivity=8, relabel=True, nproc=1, progress_bar=True):
+def deblend_sources(data, segment_img, npixels, *, labels=None, nlevels=32,
+                    contrast=0.001, mode='exponential', connectivity=8,
+                    relabel=True, nproc=1, progress_bar=True):
     """
     Deblend overlapping sources labeled in a segmentation image.
 
     Sources are deblended using a combination of multi-thresholding and
     `watershed segmentation
     <https://en.wikipedia.org/wiki/Watershed_(image_processing)>`_.  In
     order to deblend sources, there must be a saddle between them.
 
     Parameters
     ----------
     data : 2D `~numpy.ndarray`
-        The 2D data array. This array should be the same array used in
-        `~photutils.segmentation.detect_sources`.
-
-        .. note::
-           It is strongly recommended that the user convolve the data
-           with ``kernel`` and input the convolved data directly
-           into the ``data`` parameter. In this case do not input a
-           ``kernel``, otherwise the data will be convolved twice.
+        The 2D array of the image. If filtering is desired, please input
+        a convolved image here. This array should be the same array used
+        in `~photutils.segmentation.detect_sources`.
 
     segment_img : `~photutils.segmentation.SegmentationImage`
         The segmentation image to deblend.
 
     npixels : int
         The minimum number of connected pixels, each greater than
         ``threshold``, that an object must have to be deblended.
         ``npixels`` must be a positive integer.
 
-    kernel : 2D `~numpy.ndarray` or `~astropy.convolution.Kernel2D`, optional
-        Deprecated. If filtering is desired, please input a convolved
-        image directly into the ``data`` parameter.
-
-        The 2D kernel used to filter the image before thresholding.
-        Filtering the image will smooth the noise and maximize
-        detectability of objects with a shape similar to the kernel.
-        ``kernel`` must be `None` if the input ``data`` are already
-        convolved.
-
     labels : int or array_like of int, optional
         The label numbers to deblend.  If `None` (default), then all
         labels in the segmentation image will be deblended.
 
     nlevels : int, optional
         The number of multi-thresholding levels to use for deblending.
         Each source will be re-thresholded at ``nlevels`` levels spaced
@@ -174,18 +152,14 @@
     # each with a minimum of npixels
     mask = (segment_img.areas[segment_img.get_indices(labels)]
             >= (npixels * 2))
     labels = labels[mask]
 
     footprint = _make_binary_structure(data.ndim, connectivity)
 
-    if kernel is not None:
-        data = _filter_data(data, kernel, mode='constant',
-                            fill_value=0.0)  # pragma: no cover
-
     if nproc is None:
         nproc = cpu_count()  # pragma: no cover
 
     if progress_bar and HAS_TQDM:
         from tqdm.auto import tqdm  # pragma: no cover
 
     segm_deblended = object.__new__(SegmentationImage)
```

### Comparing `photutils-1.7.0/photutils/segmentation/detect.py` & `photutils-1.8.0/photutils/segmentation/detect.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,29 +2,26 @@
 """
 This module provides tools for detecting sources in an image.
 """
 
 import warnings
 
 import numpy as np
-from astropy.convolution import convolve
 from astropy.stats import SigmaClip
-from astropy.utils.decorators import deprecated_renamed_argument
-from astropy.utils.exceptions import AstropyUserWarning
 
 from photutils.segmentation.core import SegmentationImage
 from photutils.segmentation.utils import _make_binary_structure
 from photutils.utils._quantity_helpers import process_quantities
 from photutils.utils._stats import nanmean, nanstd
 from photutils.utils.exceptions import NoDetectionsWarning
 
 __all__ = ['detect_threshold', 'detect_sources']
 
 
-def detect_threshold(data, nsigma, background=None, error=None, mask=None,
+def detect_threshold(data, nsigma, *, background=None, error=None, mask=None,
                      sigma_clip=SigmaClip(sigma=3.0, maxiters=10)):
     """
     Calculate a pixel-wise threshold image that can be used to detect
     sources.
 
     This is a simple convenience function that uses sigma-clipped
     statistics to compute a scalar background and noise estimate. In
@@ -119,15 +116,15 @@
 
     if unit:
         threshold <<= unit
 
     return threshold
 
 
-def _detect_sources(data, thresholds, npixels, footprint, inverse_mask,
+def _detect_sources(data, thresholds, npixels, footprint, inverse_mask, *,
                     deblend_mode=False):
     """
     Detect sources above a specified threshold value in an image.
 
     Detected sources must have ``npixels`` connected pixels that are
     each greater than the ``threshold`` value.  If the filtering option
     is used, then the ``threshold`` is applied to the filtered image.
@@ -137,21 +134,16 @@
     This function does not deblend overlapping sources.  First use this
     function to detect sources followed by
     :func:`~photutils.segmentation.deblend_sources` to deblend sources.
 
     Parameters
     ----------
     data : 2D `~numpy.ndarray`
-        The 2D array of the image.
-
-        .. note::
-           It is strongly recommended that the user convolve the data
-           with ``kernel`` and input the convolved data directly
-           into the ``data`` parameter. In this case do not input a
-           ``kernel``, otherwise the data will be convolved twice.
+        The 2D array of the image. If filtering is desired, please input
+        a convolved image here.
 
     thresholds : list of 2D `~numpy.ndarray` or 1D array of floats
         The data values (as a 1D array of floats) or pixel-wise data
         values (as a sequence of 2D arrays) to be used for the detection
         thresholds. 2D threshold arrays must have the same shape as
         ``data``.
 
@@ -253,21 +245,15 @@
             continue
 
         segms.append(segm)
 
     return segms
 
 
-@deprecated_renamed_argument('kernel', None, '1.5', message='"kernel" was '
-                             'deprecated in version 1.5 and will be removed '
-                             'in a future version. Instead, if filtering is '
-                             'desired, please input a convolved image '
-                             'directly into the "data" parameter.')
-def detect_sources(data, threshold, npixels, kernel=None, connectivity=8,
-                   mask=None):
+def detect_sources(data, threshold, npixels, *, connectivity=8, mask=None):
     """
     Detect sources above a specified threshold value in an image.
 
     Detected sources must have ``npixels`` connected pixels that are
     each greater than the ``threshold`` value.  If the filtering option
     is used, then the ``threshold`` is applied to the filtered image.
     The input ``mask`` can be used to mask pixels in the input data.
@@ -276,42 +262,27 @@
     This function does not deblend overlapping sources.  First use this
     function to detect sources followed by
     :func:`~photutils.segmentation.deblend_sources` to deblend sources.
 
     Parameters
     ----------
     data : 2D `~numpy.ndarray`
-        The 2D array of the image.
-
-        .. note::
-           It is strongly recommended that the user convolve the data
-           with ``kernel`` and input the convolved data directly
-           into the ``data`` parameter. In this case do not input a
-           ``kernel``, otherwise the data will be convolved twice.
+        The 2D array of the image. If filtering is desired, please input
+        a convolved image here.
 
     threshold : float or 2D `~numpy.ndarray`
         The data value or pixel-wise data values to be used for the
         detection threshold. A 2D ``threshold`` array must have the same
         shape and units as ``data``.
 
     npixels : int
         The minimum number of connected pixels, each greater than
         ``threshold``, that an object must have to be detected.
         ``npixels`` must be a positive integer.
 
-    kernel : 2D `~numpy.ndarray` or `~astropy.convolution.Kernel2D`, optional
-        Deprecated. If filtering is desired, please input a convolved
-        image directly into the ``data`` parameter.
-
-        The 2D array of the kernel used to filter the image before
-        thresholding. Filtering the image will smooth the noise and
-        maximize detectability of objects with a shape similar to the
-        kernel. ``kernel`` must be `None` if the input ``data`` are
-        already convolved.
-
     connectivity : {4, 8}, optional
         The type of pixel connectivity used in determining how pixels
         are grouped into a detected source. The options are 4 or
         8 (default). 4-connected pixels touch along their edges.
         8-connected pixels touch along their edges or corners.
 
     mask : 2D bool `~numpy.ndarray`, optional
@@ -384,18 +355,13 @@
             raise ValueError('mask must not be True for every pixel. There '
                              'are no unmasked pixels in the image to detect '
                              'sources.')
         inverse_mask = np.logical_not(mask)
     else:
         inverse_mask = None
 
-    if kernel is not None:
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore', AstropyUserWarning)
-            data = convolve(data, kernel, mask=mask, normalize_kernel=True)
-
     footprint = _make_binary_structure(data.ndim, connectivity)
 
     with warnings.catch_warnings():
         warnings.simplefilter('ignore', category=RuntimeWarning)
         return _detect_sources(data, (threshold,), npixels, footprint,
                                inverse_mask, deblend_mode=False)[0]
```

### Comparing `photutils-1.7.0/photutils/segmentation/finder.py` & `photutils-1.8.0/photutils/segmentation/finder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/segmentation/tests/test_catalog.py` & `photutils-1.8.0/photutils/segmentation/tests/test_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import astropy.units as u
 import numpy as np
 import pytest
 from astropy.convolution import convolve
 from astropy.coordinates import SkyCoord
 from astropy.modeling.models import Gaussian2D
 from astropy.table import QTable
+from astropy.utils.exceptions import AstropyDeprecationWarning
 from numpy.testing import assert_allclose, assert_equal
 
 from photutils.aperture import (BoundingBox, CircularAperture,
                                 EllipticalAperture)
 from photutils.background import Background2D, MedianBackground
 from photutils.datasets import (make_100gaussians_image, make_gwcs,
                                 make_noise_image, make_wcs)
@@ -435,18 +436,19 @@
         for line in lines:
             assert line in repr(cat)
 
     def test_kernel(self):
         kernel = np.array([[1.0, 2, 1], [2, 4, 2], [1, 2, 100]])
         kernel /= kernel.sum()
 
-        cat1 = SourceCatalog(self.data, self.segm, kernel=None)
-        cat2 = SourceCatalog(self.data, self.segm, kernel=kernel)
-        assert not np.array_equal(cat1.xcentroid, cat2.xcentroid)
-        assert not np.array_equal(cat1.ycentroid, cat2.ycentroid)
+        with pytest.warns(AstropyDeprecationWarning):
+            cat1 = SourceCatalog(self.data, self.segm, kernel=None)
+            cat2 = SourceCatalog(self.data, self.segm, kernel=kernel)
+            assert not np.array_equal(cat1.xcentroid, cat2.xcentroid)
+            assert not np.array_equal(cat1.ycentroid, cat2.ycentroid)
 
         convolved_data = _filter_data(self.data, kernel, mode='constant',
                                       fill_value=0.0,
                                       check_normalization=True)
         cat3 = SourceCatalog(self.data, self.segm,
                              convolved_data=convolved_data)
         assert_allclose(cat2.centroid, cat3.centroid)
@@ -478,14 +480,15 @@
         assert cat.kron_aperture[0] is None
         assert np.isnan(cat.kron_radius[0])
         kronrad = cat.kron_radius.value
         kronrad = kronrad[~np.isnan(kronrad)]
         assert np.min(kronrad) == kron_params[1]
         assert isinstance(cat.kron_aperture[2], EllipticalAperture)
         assert isinstance(cat.kron_aperture[4], EllipticalAperture)
+        assert isinstance(cat.kron_params, tuple)
 
     def test_kron_masking(self):
         apermask_method = 'none'
         cat1 = SourceCatalog(self.data, self.segm,
                              apermask_method=apermask_method)
         apermask_method = 'mask'
         cat2 = SourceCatalog(self.data, self.segm,
```

### Comparing `photutils-1.7.0/photutils/segmentation/tests/test_core.py` & `photutils-1.8.0/photutils/segmentation/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 """
 Tests for the core module.
 """
 
 import numpy as np
 import pytest
 from astropy.utils import lazyproperty
-from astropy.utils.exceptions import (AstropyDeprecationWarning,
-                                      AstropyUserWarning)
+from astropy.utils.exceptions import AstropyUserWarning
 from numpy.testing import assert_allclose, assert_equal
 
 from photutils.segmentation.core import Segment, SegmentationImage
 from photutils.utils import circular_footprint
 from photutils.utils._optional_deps import (HAS_MATPLOTLIB, HAS_RASTERIO,
                                             HAS_SCIPY, HAS_SHAPELY)
 
@@ -424,35 +423,14 @@
         assert isinstance(patches[0], Polygon)
 
         patches = self.segm.plot_patches(labels=(4, 7))
         assert len(patches) == 2
         assert isinstance(patches, list)
         assert isinstance(patches[0], Polygon)
 
-    def test_outline_segments(self):
-        segm_array = np.zeros((5, 5)).astype(int)
-        segm_array[1:4, 1:4] = 2
-        segm = SegmentationImage(segm_array)
-        segm_array_ref = np.copy(segm_array)
-        segm_array_ref[2, 2] = 0
-        with pytest.warns(AstropyDeprecationWarning):
-            assert_allclose(segm.outline_segments(), segm_array_ref)
-
-    def test_outline_segments_masked_background(self):
-        segm_array = np.zeros((5, 5)).astype(int)
-        segm_array[1:4, 1:4] = 2
-        segm = SegmentationImage(segm_array)
-        segm_array_ref = np.copy(segm_array)
-        segm_array_ref[2, 2] = 0
-        with pytest.warns(AstropyDeprecationWarning):
-            segm_outlines = segm.outline_segments(mask_background=True)
-            assert isinstance(segm_outlines, np.ma.MaskedArray)
-            assert np.ma.count(segm_outlines) == 8
-            assert np.ma.count_masked(segm_outlines) == 17
-
 
 class CustomSegm(SegmentationImage):
     @lazyproperty
     def value(self):
         return np.median(self.data)
```

### Comparing `photutils-1.7.0/photutils/segmentation/tests/test_deblend.py` & `photutils-1.8.0/photutils/segmentation/tests/test_deblend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """
 Tests for the deblend module.
 """
 
-import warnings
-
 import numpy as np
 import pytest
 from astropy.modeling.models import Gaussian2D
 from astropy.utils.exceptions import AstropyUserWarning
 from numpy.testing import assert_allclose, assert_equal
 
 from photutils.segmentation.core import SegmentationImage
@@ -32,28 +30,22 @@
         self.threshold = 10
         self.npixels = 5
         self.segm = detect_sources(self.data, self.threshold, self.npixels)
         self.segm3 = detect_sources(self.data3, self.threshold, self.npixels)
 
     @pytest.mark.parametrize('mode', ['exponential', 'linear', 'sinh'])
     def test_deblend_sources(self, mode):
-        # scipy DeprecationWarning is currently raised from skimage
-        # (https://github.com/scikit-image/scikit-image/pull/6231)
-        # This can be removed for skimage >= 0.19.2.
-        with warnings.catch_warnings():
-            warnings.simplefilter('ignore', DeprecationWarning)
-            result = deblend_sources(self.data, self.segm, self.npixels,
-                                     mode=mode, progress_bar=False)
-
-            if mode == 'linear':
-                # test multiprocessing
-                result2 = deblend_sources(self.data, self.segm, self.npixels,
-                                          mode=mode, progress_bar=False,
-                                          nproc=2)
-                assert_equal(result.data, result2.data)
+        result = deblend_sources(self.data, self.segm, self.npixels,
+                                 mode=mode, progress_bar=False)
+
+        if mode == 'linear':
+            # test multiprocessing
+            result2 = deblend_sources(self.data, self.segm, self.npixels,
+                                      mode=mode, progress_bar=False, nproc=2)
+            assert_equal(result.data, result2.data)
 
         assert result.nlabels == 2
         assert result.nlabels == len(result.slices)
         mask1 = (result.data == 1)
         mask2 = (result.data == 2)
         assert_allclose(len(result.data[mask1]), len(result.data[mask2]))
         assert_allclose(np.sum(self.data[mask1]), np.sum(self.data[mask2]))
```

### Comparing `photutils-1.7.0/photutils/segmentation/tests/test_detect.py` & `photutils-1.8.0/photutils/segmentation/tests/test_detect.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 Tests for the detect module.
 """
 
 import astropy.units as u
 import numpy as np
 import pytest
 from astropy.stats import SigmaClip
-from astropy.utils.exceptions import AstropyDeprecationWarning
 from numpy.testing import assert_allclose, assert_array_equal
 
 from photutils.segmentation.detect import detect_sources, detect_threshold
 from photutils.segmentation.utils import make_2dgaussian_kernel
 from photutils.utils._optional_deps import HAS_SCIPY
 from photutils.utils.exceptions import NoDetectionsWarning
 
@@ -206,25 +205,14 @@
     def test_4connectivity(self):
         """Test detection with connectivity=4."""
         data = np.eye(3)
         ref = np.diag([1, 2, 3])
         segm = detect_sources(data, threshold=0.9, npixels=1, connectivity=4)
         assert_array_equal(segm.data, ref)
 
-    def test_basic_kernel(self):
-        """Test detection with kernel."""
-        kernel = np.ones((3, 3)) / 9.0
-        threshold = 0.3
-        expected = np.ones((3, 3))
-        expected[2] = 0
-        with pytest.warns(AstropyDeprecationWarning):
-            segm = detect_sources(self.data, threshold, npixels=1,
-                                  kernel=kernel)
-            assert_array_equal(segm.data, expected)
-
     def test_npixels_nonint(self):
         """Test if error raises if npixel is non-integer."""
         with pytest.raises(ValueError):
             detect_sources(self.data, threshold=1, npixels=0.1)
 
     def test_npixels_negative(self):
         """Test if error raises if npixel is negative."""
@@ -232,26 +220,14 @@
             detect_sources(self.data, threshold=1, npixels=-1)
 
     def test_connectivity_invalid(self):
         """Test if error raises if connectivity is invalid."""
         with pytest.raises(ValueError):
             detect_sources(self.data, threshold=1, npixels=1, connectivity=10)
 
-    def test_kernel_array(self):
-        with pytest.warns(AstropyDeprecationWarning):
-            segm = detect_sources(self.data, 0.1, npixels=1,
-                                  kernel=self.kernel.array)
-            assert_array_equal(segm.data, np.ones((3, 3)))
-
-    def test_kernel(self):
-        with pytest.warns(AstropyDeprecationWarning):
-            segm = detect_sources(self.data, 0.1, npixels=1,
-                                  kernel=self.kernel)
-            assert_array_equal(segm.data, np.ones((3, 3)))
-
     def test_mask(self):
         data = np.zeros((11, 11))
         data[3:8, 3:8] = 5.0
         mask = np.zeros(data.shape, dtype=bool)
         mask[4:6, 4:6] = True
         segm1 = detect_sources(data, 1.0, 1.0)
         segm2 = detect_sources(data, 1.0, 1.0, mask=mask)
```

### Comparing `photutils-1.7.0/photutils/segmentation/tests/test_finder.py` & `photutils-1.8.0/photutils/segmentation/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/segmentation/tests/test_utils.py` & `photutils-1.8.0/photutils/segmentation/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/segmentation/utils.py` & `photutils-1.8.0/photutils/segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/_convolution.py` & `photutils-1.8.0/photutils/utils/_convolution.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/_misc.py` & `photutils-1.8.0/photutils/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/_moments.py` & `photutils-1.8.0/photutils/utils/_moments.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/_optional_deps.py` & `photutils-1.8.0/photutils/utils/_optional_deps.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 __all__ = [f'HAS_{pkg}' for pkg in deps]
 
 
 def __getattr__(name):
     if name in __all__:
         try:
             importlib.import_module(deps[name[4:]])
-        except (ImportError, ModuleNotFoundError):
+        except ImportError:
             return False
         return True
 
     raise AttributeError(f'Module {__name__!r} has no attribute {name!r}.')
```

### Comparing `photutils-1.7.0/photutils/utils/_parameters.py` & `photutils-1.8.0/photutils/utils/_parameters.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/_quantity_helpers.py` & `photutils-1.8.0/photutils/utils/_quantity_helpers.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/_round.py` & `photutils-1.8.0/photutils/utils/_round.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/_stats.py` & `photutils-1.8.0/photutils/utils/_stats.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/_wcs_helpers.py` & `photutils-1.8.0/photutils/utils/_wcs_helpers.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/colormaps.py` & `photutils-1.8.0/photutils/utils/colormaps.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/cutouts.py` & `photutils-1.8.0/photutils/utils/cutouts.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/depths.py` & `photutils-1.8.0/photutils/utils/depths.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/errors.py` & `photutils-1.8.0/photutils/utils/errors.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/footprints.py` & `photutils-1.8.0/photutils/utils/footprints.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/interpolation.py` & `photutils-1.8.0/photutils/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_colormaps.py` & `photutils-1.8.0/photutils/utils/tests/test_colormaps.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_convolution.py` & `photutils-1.8.0/photutils/utils/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_cutouts.py` & `photutils-1.8.0/photutils/utils/tests/test_cutouts.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_depths.py` & `photutils-1.8.0/photutils/utils/tests/test_depths.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_errors.py` & `photutils-1.8.0/photutils/utils/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_footprints.py` & `photutils-1.8.0/photutils/utils/tests/test_footprints.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_interpolation.py` & `photutils-1.8.0/photutils/utils/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_misc.py` & `photutils-1.8.0/photutils/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_moments.py` & `photutils-1.8.0/photutils/utils/tests/test_moments.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_parameters.py` & `photutils-1.8.0/photutils/utils/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils/utils/tests/test_quantity_helpers.py` & `photutils-1.8.0/photutils/utils/tests/test_quantity_helpers.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/photutils.egg-info/PKG-INFO` & `photutils-1.8.0/photutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photutils
-Version: 1.7.0
+Version: 1.8.0
 Summary: An Astropy package for source detection and photometry
 Home-page: https://github.com/astropy/photutils
 Author: Photutils Developers
 Author-email: photutils.team@gmail.com
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,photometry,aperture,psf,source detection,background,segmentation,centroids,isophote,morphology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `photutils-1.7.0/photutils.egg-info/SOURCES.txt` & `photutils-1.8.0/photutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 setup.py
 tox.ini
 ./photutils/geometry/circular_overlap.pyx
 ./photutils/geometry/core.pyx
 ./photutils/geometry/elliptical_overlap.pyx
 ./photutils/geometry/rectangular_overlap.pyx
 .circleci/config.yml
+.github/workflows/32bit_tests.yml
 .github/workflows/ci_tests.yml
 .github/workflows/codeql.yml
 .github/workflows/cron_tests.yml
 .github/workflows/publish.yml
 docs/Makefile
 docs/aperture.rst
 docs/background.rst
@@ -79,14 +80,15 @@
 docs/whats_new/1.1.rst
 docs/whats_new/1.2.rst
 docs/whats_new/1.3.rst
 docs/whats_new/1.4.rst
 docs/whats_new/1.5.rst
 docs/whats_new/1.6.rst
 docs/whats_new/1.7.rst
+docs/whats_new/1.8.rst
 docs/whats_new/index.rst
 photutils/CITATION.rst
 photutils/__init__.py
 photutils/_astropy_init.py
 photutils/_compiler.c
 photutils/conftest.py
 photutils/version.py
```

### Comparing `photutils-1.7.0/setup.cfg` & `photutils-1.8.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,38 +23,38 @@
 
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.8
 setup_requires = setuptools_scm
 install_requires = 
-	numpy>=1.20
+	numpy>=1.21
 	astropy>=5.0
 
 [options.extras_require]
 all = 
-	scipy>=1.6.0
-	matplotlib>=3.3.0
-	scikit-image>=0.18.0
+	scipy>=1.7.0
+	matplotlib>=3.5.0
+	scikit-image>=0.19.0
 	scikit-learn>=1.0
-	gwcs>=0.16
+	gwcs>=0.18
 	bottleneck
 	tqdm
 	rasterio
 	shapely
 test = 
-	pytest-astropy
+	pytest-astropy>=0.10
 docs = 
 	sphinx
 	sphinx-astropy>=1.6
-	scipy>=1.6.0
-	matplotlib>=3.3.0
-	scikit-image>=0.18.0
+	scipy>=1.7.0
+	matplotlib>=3.5.0
+	scikit-image>=0.19.0
 	scikit-learn>=1.0
-	gwcs>=0.16
+	gwcs>=0.18
 	rasterio
 	shapely
 
 [options.package_data]
 photutils = CITATION.rst
 photutils.datasets = data/*
 photutils.detection.tests = data/*
```

### Comparing `photutils-1.7.0/setup.py` & `photutils-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `photutils-1.7.0/tox.ini` & `photutils-1.8.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tox]
 envlist =
     py{38,39,310,311}-test{,-alldeps,-devdeps,-oldestdeps}{,-cov}
-    py{38,39,310,311}-test-numpy{118,119,120,121,122,123}
+    py{38,39,310,311}-test-numpy{121,122,123,124}
     py{38,39,310,311}-test-astropy{50,lts}
-    circleci_32bit
+    32bit
     build_docs
     linkcheck
     codestyle
     pep517
     bandit
 requires =
     setuptools >= 30.3.0
@@ -38,49 +38,45 @@
 #
 description =
     run tests
     alldeps: with all optional dependencies
     devdeps: with the latest developer version of key dependencies
     oldestdeps: with the oldest supported version of key dependencies
     cov: and test coverage
-    numpy118: with numpy 1.18.*
-    numpy119: with numpy 1.19.*
-    numpy120: with numpy 1.20.*
     numpy121: with numpy 1.21.*
     numpy122: with numpy 1.22.*
     numpy123: with numpy 1.23.*
+    numpy124: with numpy 1.24.*
 
     astropy50: with astropy 5.0.*
     astropylts: with the latest astropy LTS
 
 # The following provides some specific pinnings for key packages
 deps =
-    circleci_32bit: numpy==1.21.*
-    circleci_32bit: git+https://github.com/astropy/astropy.git#egg=astropy
+    32bit: numpy==1.21.*
+    32bit: git+https://github.com/astropy/astropy.git#egg=astropy
 
     cov: coverage
 
-    numpy118: numpy==1.18.*
-    numpy119: numpy==1.19.*
-    numpy120: numpy==1.20.*
     numpy121: numpy==1.21.*
     numpy122: numpy==1.22.*
     numpy123: numpy==1.23.*
+    numpy124: numpy==1.24.*
 
     astropy50: astropy==5.0.*
     astropylts: astropy==5.0.*
 
-    oldestdeps: numpy==1.18
+    oldestdeps: numpy==1.21
     oldestdeps: astropy==5.0
-    oldestdeps: scipy==1.6.0
-    oldestdeps: matplotlib==3.1
-    oldestdeps: scikit-image==0.14.2
-    oldestdeps: scikit-learn==0.19
-    oldestdeps: gwcs==0.12
-    oldestdeps: pytest-astropy==0.4
+    oldestdeps: scipy==1.7.0
+    oldestdeps: matplotlib==3.5.0
+    oldestdeps: scikit-image==0.19.0
+    oldestdeps: scikit-learn==1.0
+    oldestdeps: gwcs==0.18
+    oldestdeps: pytest-astropy==0.10
 
     devdeps: numpy>=0.0.dev0
     devdeps: scipy>=0.0.dev0
     devdeps: matplotlib>=0.0.dev0
     devdeps: git+https://github.com/spacetelescope/gwcs.git
 
 # The following indicates which extras_require from setup.cfg will be
@@ -94,17 +90,17 @@
     devdeps: pip install -U -i https://pypi.anaconda.org/astropy/simple astropy --pre
     devdeps: pip install -U -i https://pypi.anaconda.org/scipy-wheels-nightly/simple scikit-learn
     pip freeze
     !cov: pytest --pyargs photutils {toxinidir}/docs {posargs}
     cov: pytest --pyargs photutils {toxinidir}/docs --cov photutils --cov-config={toxinidir}/setup.cfg {posargs}
     cov: coverage xml -o {toxinidir}/coverage.xml
 
-[testenv:circleci_32bit]
+[testenv:32bit]
 changedir = .tmp/{envname}
-description = 32-bit CircleCI tests
+description = 32-bit tests
 extras = test
 commands =
     pip freeze
     !cov: pytest --pyargs photutils {toxinidir}/docs {posargs}
 
 [testenv:build_docs]
 changedir = docs
```

