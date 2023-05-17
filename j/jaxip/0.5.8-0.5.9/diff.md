# Comparing `tmp/jaxip-0.5.8.tar.gz` & `tmp/jaxip-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.5.8.tar", last modified: Tue May  9 21:10:40 2023, max compression
+gzip compressed data, was "jaxip-0.5.9.tar", last modified: Wed May 17 19:33:14 2023, max compression
```

## Comparing `jaxip-0.5.8.tar` & `jaxip-0.5.9.tar`

### file list

```diff
@@ -1,140 +1,141 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.267821 jaxip-0.5.8/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.8/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.8/CONTRIBUTING.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.8/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.8/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.8/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5342 2023-05-09 21:10:40.267821 jaxip-0.5.8/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4755 2023-05-08 16:51:03.000000 jaxip-0.5.8/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.247821 jaxip-0.5.8/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.8/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.239821 jaxip-0.5.8/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.239821 jaxip-0.5.8/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.247821 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-09 20:59:51.000000 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_potential_training_30_21.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-09 20:59:52.000000 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-09 20:59:52.000000 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-09 20:59:52.000000 jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.239821 jaxip-0.5.8/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.247821 jaxip-0.5.8/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    15512 2023-05-09 20:58:04.000000 jaxip-0.5.8/docs/_build/html/_images/notebooks_potential_training_30_21.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-09 20:58:05.000000 jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-09 20:58:05.000000 jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-09 20:58:05.000000 jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.251821 jaxip-0.5.8/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.8/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.8/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.8/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.8/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6406 2023-05-01 12:49:56.000000 jaxip-0.5.8/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.8/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       81 2023-05-01 12:51:50.000000 jaxip-0.5.8/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.8/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.251821 jaxip-0.5.8/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.8/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.8/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.5.8/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.8/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      507 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      595 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.models.nn.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      234 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1129 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      941 2023-05-09 21:10:18.000000 jaxip-0.5.8/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.8/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-09 20:57:57.000000 jaxip-0.5.8/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.8/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.5.8/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.8/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.251821 jaxip-0.5.8/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.5.8/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.255821 jaxip-0.5.8/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/atoms/_box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/atoms/_neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3724 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.8/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3015 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    16818 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.255821 jaxip-0.5.8/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6668 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/datasets/runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1021 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/datasets/transformer.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.8/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.5.8/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7583 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2228 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2644 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1354 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1011 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      765 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/descriptors/base.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/models/nn/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/nn/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/nn/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/nn/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2849 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/models/nn/network.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.259822 jaxip-0.5.8/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1949 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1807 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/potentials/atomic_potential.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.263821 jaxip-0.5.8/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      196 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9589 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9747 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    19255 2023-05-08 16:51:03.000000 jaxip-0.5.8/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11326 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3555 2023-05-09 21:10:18.000000 jaxip-0.5.8/jaxip/pytree.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.5.8/jaxip/types.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.8/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.263821 jaxip-0.5.8/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.8/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.8/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.8/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.8/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.255821 jaxip-0.5.8/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5342 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3142 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-09 21:10:40.000000 jaxip-0.5.8/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-09 21:10:40.267821 jaxip-0.5.8/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.8/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.267821 jaxip-0.5.8/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-09 21:10:40.267821 jaxip-0.5.8/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.8/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.8/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.8/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.8/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.8/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.8/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.8/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-09 21:01:28.000000 jaxip-0.5.8/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-09 21:01:28.000000 jaxip-0.5.8/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-05-07 11:23:30.000000 jaxip-0.5.8/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4116 2023-05-08 16:51:03.000000 jaxip-0.5.8/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3420 2023-05-01 12:41:07.000000 jaxip-0.5.8/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.8/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.8/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.8/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-09 21:01:28.000000 jaxip-0.5.8/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-09 21:01:28.000000 jaxip-0.5.8/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.069933 jaxip-0.5.9/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.5.9/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.5.9/CONTRIBUTING.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      569 2023-03-02 17:04:49.000000 jaxip-0.5.9/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.5.9/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.5.9/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-05-17 19:33:14.069933 jaxip-0.5.9/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4745 2023-05-17 19:30:18.000000 jaxip-0.5.9/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.049933 jaxip-0.5.9/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.5.9/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.045933 jaxip-0.5.9/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.045933 jaxip-0.5.9/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.045933 jaxip-0.5.9/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    12610 2023-05-17 19:29:17.000000 jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.5.9/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.9/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.5.9/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.5.9/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6394 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.5.9/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       71 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.5.9/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.5.9/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.5.9/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.5.9/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.5.9/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      662 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-05-17 19:30:18.000000 jaxip-0.5.9/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      941 2023-05-17 19:29:09.000000 jaxip-0.5.9/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-10 20:36:05.000000 jaxip-0.5.9/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.5.9/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-05-17 19:29:09.000000 jaxip-0.5.9/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.5.9/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.5.9/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.5.9/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.053933 jaxip-0.5.9/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.5.9/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.057933 jaxip-0.5.9/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      174 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      355 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/atoms/_box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      779 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/atoms/_neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1342 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3724 2023-05-09 21:10:18.000000 jaxip-0.5.9/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5034 2023-05-01 06:50:37.000000 jaxip-0.5.9/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3015 2023-05-09 21:10:18.000000 jaxip-0.5.9/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    16813 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1131 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.057933 jaxip-0.5.9/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/datasets/dataset.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6445 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/datasets/runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1039 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/datasets/transformer.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.057933 jaxip-0.5.9/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.061933 jaxip-0.5.9/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.5.9/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5275 2023-05-06 13:11:44.000000 jaxip-0.5.9/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7689 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/descriptors/descriptor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7476 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.061933 jaxip-0.5.9/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.5.9/jaxip/models/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/models/model.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.065933 jaxip-0.5.9/jaxip/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.5.9/jaxip/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.5.9/jaxip/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.5.9/jaxip/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2911 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.065933 jaxip-0.5.9/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1973 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1831 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.065933 jaxip-0.5.9/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9155 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9364 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      545 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    18966 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11352 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3585 2023-05-17 19:30:18.000000 jaxip-0.5.9/jaxip/pytree.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      643 2023-05-07 09:13:07.000000 jaxip-0.5.9/jaxip/types.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      200 2023-01-05 20:40:22.000000 jaxip-0.5.9/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.065933 jaxip-0.5.9/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1427 2023-02-18 20:52:11.000000 jaxip-0.5.9/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2008 2023-03-23 20:22:06.000000 jaxip-0.5.9/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.5.9/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.5.9/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.057933 jaxip-0.5.9/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5332 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3091 2023-05-17 19:33:14.000000 jaxip-0.5.9/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-05-17 19:33:13.000000 jaxip-0.5.9/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-05-17 19:33:14.069933 jaxip-0.5.9/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.5.9/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.069933 jaxip-0.5.9/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-05-17 19:33:14.069933 jaxip-0.5.9/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.9/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.5.9/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.5.9/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.5.9/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.5.9/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.5.9/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.5.9/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-05-17 19:26:08.000000 jaxip-0.5.9/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-05-17 19:26:08.000000 jaxip-0.5.9/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5117 2023-05-07 11:23:30.000000 jaxip-0.5.9/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4116 2023-05-08 16:51:03.000000 jaxip-0.5.9/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3472 2023-05-17 19:30:18.000000 jaxip-0.5.9/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4816 2023-05-01 12:41:07.000000 jaxip-0.5.9/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2859 2023-05-01 12:41:07.000000 jaxip-0.5.9/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4937 2023-04-24 20:54:27.000000 jaxip-0.5.9/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-05-17 19:26:08.000000 jaxip-0.5.9/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-05-17 19:26:08.000000 jaxip-0.5.9/tests/weights.008.pkl
```

### Comparing `jaxip-0.5.8/CONTRIBUTING.rst` & `jaxip-0.5.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/HISTORY.rst` & `jaxip-0.5.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/LICENSE` & `jaxip-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/PKG-INFO` & `jaxip-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.5.8
+Version: 0.5.9
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,16 +49,16 @@
 
 
 See `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
-Main features
--------------
+Features
+--------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
 * It uses `autograd` to make defining new descriptors straightforward.
 * Jaxip is written purely in Python and optimized with `just-in-time` (JIT) compilation.
 * It also supports `GPU-accelerated` computing, which can significantly speed up preprocessing and model training.
 
 .. warning::
         This package is under heavy development and the current focus is on the implementation of high-dimensional
```

### Comparing `jaxip-0.5.8/README.rst` & `jaxip-0.5.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 
 
 See `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
-Main features
--------------
+Features
+--------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
 * It uses `autograd` to make defining new descriptors straightforward.
 * Jaxip is written purely in Python and optimized with `just-in-time` (JIT) compilation.
 * It also supports `GPU-accelerated` computing, which can significantly speed up preprocessing and model training.
 
 .. warning::
         This package is under heavy development and the current focus is on the implementation of high-dimensional
```

### Comparing `jaxip-0.5.8/docs/Makefile` & `jaxip-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png` & `jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png` & `jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png` & `jaxip-0.5.9/docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_38_0.png` & `jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_45_0.png` & `jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/_build/html/_images/notebooks_tutorials_51_0.png` & `jaxip-0.5.9/docs/_build/html/_images/notebooks_tutorials_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/conf.py` & `jaxip-0.5.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 html_theme_options = {
     # "search_bar_position": "sidebar",
-    # "github_url": "https://github.com/hghcomphys/jaxip",
+    "github_url": "https://github.com/hghcomphys/jaxip",
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
@@ -216,12 +216,12 @@
 
 curdir = os.path.dirname(os.path.abspath(__file__))
 notebooks_dir = os.path.join(curdir, "notebooks")
 if os.path.exists(notebooks_dir):
     shutil.rmtree(notebooks_dir)
 os.makedirs(notebooks_dir, exist_ok=True)
 
-for filename in ("tutorials.ipynb", "potential_training.ipynb"):
+for filename in ("tutorials.ipynb", "training.ipynb"):
     shutil.copyfile(  # copytree(
         os.path.join(curdir, "..", "examples", filename),
         os.path.join(curdir, "notebooks", filename),
     )
```

### Comparing `jaxip-0.5.8/docs/images/flowchart.drawio.png` & `jaxip-0.5.9/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/images/water.png` & `jaxip-0.5.9/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/installation.rst` & `jaxip-0.5.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/jaxip.atoms.rst` & `jaxip-0.5.9/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.5.9/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/jaxip.descriptors.rst` & `jaxip-0.5.9/docs/jaxip.descriptors.rst`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,18 @@
    :maxdepth: 4
 
    jaxip.descriptors.acsf
 
 Submodules
 ----------
 
-jaxip.descriptors.base module
------------------------------
+jaxip.descriptors.descriptor module
+-----------------------------------
 
-.. automodule:: jaxip.descriptors.base
+.. automodule:: jaxip.descriptors.descriptor
    :members:
    :undoc-members:
    :show-inheritance:
 
 jaxip.descriptors.scaler module
 -------------------------------
```

### Comparing `jaxip-0.5.8/docs/jaxip.models.nn.rst` & `jaxip-0.5.9/docs/jaxip.models.nn.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/jaxip.potentials.nnp.rst` & `jaxip-0.5.9/docs/jaxip.potentials.nnp.rst`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 -----------------------------------
 
 .. automodule:: jaxip.potentials.nnp.metrics
    :members:
    :undoc-members:
    :show-inheritance:
 
+jaxip.potentials.nnp.nnp module
+-------------------------------
+
+.. automodule:: jaxip.potentials.nnp.nnp
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 jaxip.potentials.nnp.potential module
 -------------------------------------
 
 .. automodule:: jaxip.potentials.nnp.potential
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `jaxip-0.5.8/docs/jaxip.rst` & `jaxip-0.5.9/docs/jaxip.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/jaxip.utils.rst` & `jaxip-0.5.9/docs/jaxip.utils.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/make.bat` & `jaxip-0.5.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/theory.rst` & `jaxip-0.5.9/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/docs/usage.rst` & `jaxip-0.5.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/__init__.py` & `jaxip-0.5.9/jaxip/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/atoms/_neighbor.py` & `jaxip-0.5.9/jaxip/atoms/_neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/atoms/_structure.py` & `jaxip-0.5.9/jaxip/atoms/_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/atoms/box.py` & `jaxip-0.5.9/jaxip/atoms/box.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/atoms/element.py` & `jaxip-0.5.9/jaxip/atoms/element.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/atoms/neighbor.py` & `jaxip-0.5.9/jaxip/atoms/neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/atoms/structure.py` & `jaxip-0.5.9/jaxip/atoms/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -222,29 +222,29 @@
 
     def __post_init__(self) -> None:
         """Post initializations."""
         self.position = self.box.shift_inside_box(self.position)
         logger.debug(f"Initializing {self.__class__.__name__}()")
         self._assert_jit_dynamic_attributes(
             expected=(
-                "position", 
-                "force", 
-                "energy", 
-                "total_energy", 
-                "charge", 
+                "position",
+                "force",
+                "energy",
+                "total_energy",
+                "charge",
                 "total_charge",
-                "atom_type"
+                "atom_type",
             )
         )
         self._assert_jit_static_attributes(
             expected=(
-                'box', 
-                'element_map',
-                'neighbor',
-                'requires_neighbor_update',
+                "box",
+                "element_map",
+                "neighbor",
+                "requires_neighbor_update",
             )
         )
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
```

### Comparing `jaxip-0.5.8/jaxip/config.py` & `jaxip-0.5.9/jaxip/config.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/datasets/runner.py` & `jaxip-0.5.9/jaxip/datasets/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,21 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from pathlib import Path
-from typing import DefaultDict, Dict, List, Optional, Protocol, TextIO
+from typing import DefaultDict, Dict, List, Optional, TextIO
 
 from jaxip.atoms.structure import Structure
-from jaxip.datasets.transformer import ToStructure, Transformer
+from jaxip.datasets.dataset import DatasetInterface
+from jaxip.datasets.transformer import ToStructure, TransformerInterface
 from jaxip.logger import logger
 from jaxip.utils.tokenize import tokenize
 
 
-class Dataset(Protocol):
-    """
-    A data container for atom data structure.
-
-    Features:
-
-    * it must access data item in a lazy mode.
-    * it should be able to cache data via a `persist` input flag.
-    """
-
-    def __len__(self) -> int:
-        ...
-
-    def __getitem__(self, index: int) -> Structure:
-        ...
-
-class RunnerDataset(Dataset):
+class RunnerDataset(DatasetInterface):
     """
     Dataset for `RuNNer`_ data file format.
 
     The input structure file contains atom info and simulation box.
     Each snapshot contains two per-atom and collective properties as follows:
 
     * `per-atom` properties include the element name, positions, energy, charge, force components, etc.
@@ -39,30 +24,32 @@
     .. _RuNNer: https://www.uni-goettingen.de/de/560580.html
     """
 
     def __init__(
         self,
         filename: Path,
         persist: bool = False,
-        transform: Optional[Transformer] = None,
+        transform: Optional[TransformerInterface] = None,
     ) -> None:
         """
         Initialize the `RuNNer`_ structure dataset.
 
         :param filename: Path
         :type filename: path to the RuNNer structure file
         :param persist: Persist structure data in the memory, defaults to False
         :type persist: bool, optional
         :param transform: applied transformation on raw data, default is ToStructure.
 
         .. _RuNNer: https://www.uni-goettingen.de/de/560580.html
         """
         self.filename: Path = Path(filename)
         self.persist: bool = persist
-        self.transform: Transformer = ToStructure() if transform is None else transform
+        self.transform: TransformerInterface = (
+            ToStructure() if transform is None else transform
+        )
         self._cached_structures: Dict[int, Structure] = dict()
         self._current_index: int = 0
 
     def __len__(self) -> int:
         """Return number of structures."""
         num_structures: int = 0
         with open(str(self.filename), "r") as file:
```

### Comparing `jaxip-0.5.8/jaxip/datasets/transformer.py` & `jaxip-0.5.9/jaxip/datasets/transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Dict, Optional, Protocol
 
 from jaxip.atoms.structure import Structure
 from jaxip.types import Dtype
 from jaxip.types import dtype as _dtype
 
 
-class Transformer(Protocol):
+class TransformerInterface(Protocol):
     """
     A base transformer class which applies on the structure dataset.
     """
 
     def __call__(self, data: Dict, **kwargs: Any) -> Structure:
         ...
 
     def __repr__(self) -> str:
         ...
 
 
-class ToStructure(Transformer):
+class ToStructure(TransformerInterface):
     """Transform a dictionary of data into to a Structure."""
 
     def __init__(
         self,
         r_cutoff: Optional[float] = None,
         dtype: Optional[Dtype] = None,
     ) -> None:
```

### Comparing `jaxip-0.5.8/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.5.9/jaxip/descriptors/acsf/_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.5.9/jaxip/descriptors/acsf/acsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from jaxip.atoms.structure import Structure
 from jaxip.descriptors.acsf._acsf import (
     _calculate_descriptor,
     _calculate_grad_descriptor_per_atom,
 )
 from jaxip.descriptors.acsf.angular import AngularSymmetryFunction
 from jaxip.descriptors.acsf.radial import RadialSymmetryFunction
-from jaxip.descriptors.acsf.symmetry import EnvironmentElements, SymmetryFunction
-from jaxip.descriptors.base import Descriptor
+from jaxip.descriptors.acsf.symmetry import BaseSymmetryFunction, EnvironmentElements
+from jaxip.descriptors.descriptor import DescriptorInterface
 from jaxip.logger import logger
-from jaxip.pytree import register_jax_pytree_node
+from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array, Element
 
 
 @dataclass
-class ACSF(Descriptor):
+class ACSF(BaseJaxPytreeDataClass, DescriptorInterface):
     """
     Atom-centered Symmetry Function (`ACSF`_) descriptor.
 
     ACSF describes the local environment of an atom (neighbor distributions).
     It usually contains multiple combinations of `radial` (two-body)
     and `angular` (three-body) symmetry functions.
 
@@ -71,15 +71,15 @@
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     def add(
         self,
-        symmetry_function: SymmetryFunction,
+        symmetry_function: BaseSymmetryFunction,
         neighbor_element_j: Element,
         neighbor_element_k: Optional[Element] = None,
     ) -> None:
         """Add the input symmetry function to the list of ACSFs."""
         if isinstance(symmetry_function, RadialSymmetryFunction):
             self.radial_symmetry_functions = self.radial_symmetry_functions + (
                 (
@@ -108,15 +108,16 @@
         atom_index: Optional[Array] = None,
     ) -> Array:
         """
         Calculate descriptor values for the input given structure and atom index.
 
         :param structure: input structure instance
         :type structure: Structure
-        :param atom_index: index for atom(s), defaults select all atom indices of type the central element of the descriptor.
+        :param atom_index: index for atom(s), defaults select all atom indices
+        of type the central element of the descriptor.
         :type atom_index: Optional[Array], optional
         :return: descriptor values
         :rtype: Array
         """
 
         if self.num_symmetry_functions == 0:
             logger.warning(
@@ -124,15 +125,15 @@
                 f" radial={self.num_radial_symmetry_functions}"
                 f", angular={self.num_angular_symmetry_functions}"
             )
 
         if atom_index is None:
             atom_index = structure.select(self.element)
         else:
-            atom_index = jnp.atleast_1d(atom_index)
+            atom_index = jnp.atleast_1d(atom_index)  # type: ignore
             # Check aid atom type match the central element
             if not jnp.all(
                 structure.element_map.element_to_atype[self.element]
                 == structure.atom_type[atom_index]
             ):
                 logger.error(
                     f"Inconsistent central element '{self.element}': input aid={atom_index}"
@@ -210,13 +211,13 @@
             ]
         )
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}(element='{self.element}'"
             f", symmetry_functions={self.num_symmetry_functions}"
-            f", r_cutoff={self.r_cutoff}"
+            # f", r_cutoff={self.r_cutoff}"
             ")"
         )
 
 
 register_jax_pytree_node(ACSF)
```

### Comparing `jaxip-0.5.8/jaxip/descriptors/acsf/angular.py` & `jaxip-0.5.9/jaxip/descriptors/acsf/angular.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 
 import jax
 import jax.numpy as jnp
 
 from jaxip.descriptors.acsf.cutoff import CutoffFunction
-from jaxip.descriptors.acsf.symmetry import SymmetryFunction
+from jaxip.descriptors.acsf.symmetry import BaseSymmetryFunction
 from jaxip.pytree import register_jax_pytree_node
 from jaxip.types import Array
 
 
-class AngularSymmetryFunction(SymmetryFunction, metaclass=ABCMeta):
+class AngularSymmetryFunction(BaseSymmetryFunction, metaclass=ABCMeta):
     """A base class for `three body` (angular) symmetry functions."""
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     @abstractmethod
```

### Comparing `jaxip-0.5.8/jaxip/descriptors/acsf/cutoff.py` & `jaxip-0.5.9/jaxip/descriptors/acsf/cutoff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import functools
 import math
 from dataclasses import dataclass
 from typing import Callable, Optional
 
 import jax
 import jax.numpy as jnp
 
@@ -35,15 +34,15 @@
             except AttributeError:
                 logger.error(
                     f"'{self.__class__.__name__}' has no cutoff function '{self.cutoff_type}'",
                     exception=NotImplementedError,
                 )
         self._assert_jit_dynamic_attributes()
         self._assert_jit_static_attributes(
-            expected=('r_cutoff', 'cutoff_type', 'cutoff_function')
+            expected=("r_cutoff", "cutoff_type", "cutoff_function")
         )
 
     def __hash__(self) -> int:
         """Enforce to use the parent class's hash method (JIT)."""
         return super().__hash__()
 
     @jax.jit
```

### Comparing `jaxip-0.5.8/jaxip/descriptors/acsf/radial.py` & `jaxip-0.5.9/jaxip/descriptors/acsf/radial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 
 import jax
 import jax.numpy as jnp
 
 from jaxip.descriptors.acsf.cutoff import CutoffFunction
-from jaxip.descriptors.acsf.symmetry import SymmetryFunction
+from jaxip.descriptors.acsf.symmetry import BaseSymmetryFunction
 from jaxip.pytree import register_jax_pytree_node
 from jaxip.types import Array
 
 
-class RadialSymmetryFunction(SymmetryFunction, metaclass=ABCMeta):
+class RadialSymmetryFunction(BaseSymmetryFunction, metaclass=ABCMeta):
     """A base class for `two body` (radial) symmetry functions."""
 
+    def __hash__(self) -> int:
+        """Enforce to use the parent class's hash method (JIT)."""
+        return super().__hash__()
+
     @abstractmethod
     def __call__(self, rij: Array) -> Array:
         ...
 
 
 @dataclass
 class G1(RadialSymmetryFunction):
```

### Comparing `jaxip-0.5.8/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.5.9/jaxip/descriptors/acsf/symmetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from jaxip.descriptors.acsf.cutoff import CutoffFunction
 from jaxip.logger import logger
 from jaxip.pytree import BaseJaxPytreeDataClass
 from jaxip.types import Array, Element
 
 
-class SymmetryFunction(BaseJaxPytreeDataClass, metaclass=ABCMeta):
+class BaseSymmetryFunction(BaseJaxPytreeDataClass, metaclass=ABCMeta):
     """
     A base class for symmetry functions.
     All symmetry functions (i.e. radial and angular) must derive from this base class.
     """
 
     def __init__(self, cfn: CutoffFunction) -> None:
         self.cfn: CutoffFunction = cfn
```

### Comparing `jaxip-0.5.8/jaxip/descriptors/base.py` & `jaxip-0.5.9/jaxip/descriptors/descriptor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-from abc import ABCMeta, abstractmethod
+from typing import Any, Protocol
 
-from jaxip.pytree import BaseJaxPytreeDataClass
 from jaxip.types import Array
 
 
-class Descriptor(BaseJaxPytreeDataClass, metaclass=ABCMeta):
+class DescriptorInterface(Protocol):
     """A base class for atomic environment descriptors."""
 
-    @abstractmethod
-    def add(self, *args, **kwargs) -> None:
+    def add(self, *args: Any, **kwargs: Any) -> None:
         ...
 
-    @abstractmethod
-    def __call__(self, *args, **kwargs) -> Array:
+    def __call__(self, *args: Any, **kwargs: Any) -> Array:
         ...
 
-    @abstractmethod
-    def grad(self, *args, **kwargs) -> Array:
+    def grad(self, *args: Any, **kwargs: Any) -> Array:
         ...
 
     @property
-    @abstractmethod
     def num_descriptors(self) -> int:
         """Return number of items in the descriptor array."""
         ...
 
     @property
-    @abstractmethod
     def r_cutoff(self) -> float:
         """Return the cutoff radius of the descriptor."""
         ...
```

### Comparing `jaxip-0.5.8/jaxip/descriptors/scaler.py` & `jaxip-0.5.9/jaxip/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/logger.py` & `jaxip-0.5.9/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/models/nn/activation.py` & `jaxip-0.5.9/jaxip/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/models/nn/initializer.py` & `jaxip-0.5.9/jaxip/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/models/nn/network.py` & `jaxip-0.5.9/jaxip/models/nn/network.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from pathlib import Path
 from typing import Callable, List, Tuple
 
 from flax import linen as nn
 from frozendict import frozendict
 
 from jaxip.logger import logger
+from jaxip.models.model import ModelInterface
 from jaxip.models.nn.activation import _activation_function_map
 from jaxip.types import Array, Dtype
 from jaxip.types import dtype as _dtype
 
 
-class NeuralNetworkModel(nn.Module):
+class NeuralNetworkModel(nn.Module, ModelInterface):
     """Neural network model that outputs energy."""
 
     hidden_layers: Tuple[Tuple[int, str], ...]
     output_layer: Tuple[int, str] = (1, "identity")
     param_dtype: Dtype = field(default_factory=lambda: _dtype.FLOATX)
     kernel_initializer: Callable = nn.initializers.lecun_normal()
     # bias_initializer: Callable = nn.initializers.zeros
```

### Comparing `jaxip-0.5.8/jaxip/potentials/_energy.py` & `jaxip-0.5.9/jaxip/potentials/_energy.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import jax.numpy as jnp
 from frozendict import frozendict
 from jax import jit
 
 from jaxip.atoms.structure import Inputs
 from jaxip.descriptors import Scaler
 from jaxip.descriptors.acsf._acsf import _calculate_descriptor
-from jaxip.descriptors.base import Descriptor
+from jaxip.descriptors.descriptor import DescriptorInterface
 from jaxip.models import NeuralNetworkModel
 from jaxip.types import Array, Element
 
 
 class AtomicPotentialInterface(Protocol):
     """An interface for AtomicPotential."""
 
-    descriptor: Descriptor
+    descriptor: DescriptorInterface
     scaler: Scaler
     model: NeuralNetworkModel
 
 
 @partial(jit, static_argnums=(0,))
 def _compute_atomic_energy(
     atomic_potential: AtomicPotentialInterface,
```

### Comparing `jaxip-0.5.8/jaxip/potentials/_force.py` & `jaxip-0.5.9/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/potentials/atomic_potential.py` & `jaxip-0.5.9/jaxip/potentials/atomic_potential.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 
 from frozendict import frozendict
 
 from jaxip.atoms.structure import Structure
-from jaxip.descriptors.base import Descriptor
+from jaxip.descriptors.descriptor import DescriptorInterface
 from jaxip.descriptors.scaler import Scaler
 from jaxip.models.nn.network import NeuralNetworkModel
 from jaxip.potentials._energy import _compute_atomic_energy
 from jaxip.types import Array, Element
 
 
 @dataclass(frozen=True)
@@ -15,15 +15,15 @@
     """
     Atomic potential.
 
     It chains all the required transformers (descriptor, scaler, model, etc.)
     to calculate per-atom energy.
     """
 
-    descriptor: Descriptor
+    descriptor: DescriptorInterface
     scaler: Scaler
     model: NeuralNetworkModel
 
     def apply(
         self,
         params: frozendict,
         structure: Structure,
```

### Comparing `jaxip-0.5.8/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.5.9/jaxip/potentials/nnp/gradient_descent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,60 @@
 from __future__ import annotations
 
 import math
 import random
 from collections import defaultdict
-from typing import Any, Callable, Dict, List, Protocol, Tuple
+from typing import Any, Callable, Dict, List, Tuple
 
 import jax.numpy as jnp
 import numpy as np
 import optax
 from flax.training.train_state import TrainState
 from frozendict import frozendict
 from jax import value_and_grad
 from optax import GradientTransformation
 from tqdm import tqdm
 
 from jaxip.atoms.structure import Structure
+from jaxip.datasets.dataset import DatasetInterface
 from jaxip.logger import logger
 from jaxip.potentials._energy import _energy_fn
 from jaxip.potentials._force import _compute_force
-from jaxip.potentials.atomic_potential import AtomicPotential
 from jaxip.potentials.nnp.metrics import ErrorMetric
-from jaxip.potentials.nnp.settings import PotentialSettings
+from jaxip.potentials.nnp.nnp import (
+    NeuralNetworkPotentialInterface as PotentialInterface,
+)
+from jaxip.potentials.nnp.settings import (
+    NeuralNetworkPotentialSettings as PotentialSettings,
+)
 from jaxip.types import Array, Element
 
 
 def _mse_loss(*, logits: Array, targets: Array) -> Array:
     return ((targets - logits) ** 2).mean()
 
-class StructureDataset(Protocol):
-    """A data container for atom data structure."""
-
-    def __len__(self) -> int:
-        ...
-
-    def __getitem__(self, index: int) -> Structure:
-        ...
-
-class Updater(Protocol):
-    """Interface for potential weight updaters."""
-
-    def fit(self, dataset: StructureDataset) -> Dict:
-        ...
-
-
-class Potential(Protocol):
-    """Interface for Potential."""
-
-    settings: PotentialSettings
-    elements: Tuple[Element, ...]
-    atomic_potential: Dict[Element, AtomicPotential]
-    model_params: Dict[Element, frozendict]
 
 # @dataclass
-class GradientDescentUpdater(Updater):
+class GradientDescentUpdater:
     """
     A trainer class to fit a generic NNP potential weights using target values of the total
     energy and force components.
 
     See https://pytorch.org/tutorials/beginner/introyt/trainingyt.html
     """
 
     # potential: PotentialInterface
     # settings: PotentialSettings
     # criterion: Callable = field(default_factory=lambda: mse_loss)
     # error_metric: ErrorMetric
     # optimizer: Dict[Element, Any]
 
-    def __init__(self, potential: Potential) -> None:
+    def __init__(self, potential: PotentialInterface) -> None:
         """Initialize potential."""
-        self.potential: Potential = potential
+        self.potential: PotentialInterface = potential
         self.criterion: Callable[..., Array] = _mse_loss
         self.error_metric: ErrorMetric = ErrorMetric.create(
             self.potential.settings.main_error_metric
         )
         self._init_parameters()
         self._init_optimizer()
 
@@ -113,15 +95,15 @@
                     tx=self.optimizer,  # [element]?
                 )
 
         return {element: state for element, state in generate_train_state()}
 
     # ------------------------------------------------------------------------
 
-    def fit(self, dataset: StructureDataset, **kwargs):
+    def fit(self, dataset: DatasetInterface, **kwargs):
         """Train potential."""
         batch_size: int = kwargs.get("batch_size", 1)
         steps: int = kwargs.get("steps", math.ceil(len(dataset) / batch_size))
         epochs: int = kwargs.get("epochs", 10)
 
         states: Dict[Element, TrainState] = self._init_train_state()
         history = defaultdict(list)
```

### Comparing `jaxip-0.5.8/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.5.9/jaxip/potentials/nnp/kalman_filter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,49 @@
 import random
 from collections import defaultdict
-from typing import Callable, Dict, Protocol, Tuple
+from typing import Callable, Dict
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from frozendict import frozendict
 from jax import flatten_util
 from tqdm import tqdm
 
 from jaxip.atoms.structure import Structure
+from jaxip.datasets.dataset import DatasetInterface
 from jaxip.logger import logger
 from jaxip.potentials._energy import _compute_energy
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.atomic_potential import AtomicPotential
-from jaxip.potentials.nnp.settings import PotentialSettings
+from jaxip.potentials.nnp.nnp import (
+    NeuralNetworkPotentialInterface as PotentialInterface,
+)
+from jaxip.potentials.nnp.settings import (
+    NeuralNetworkPotentialSettings as PotentialSettings,
+)
 from jaxip.types import Array, Element
 from jaxip.types import dtype as default_dtype
 
 
 def _tree_flatten(pytree: Dict) -> Array:
     return flatten_util.ravel_pytree(pytree)[0].reshape(-1, 1)  # type: ignore
 
 
-class StructureDataset(Protocol):
-    """A data container for atom data structure."""
-
-    def __len__(self) -> int:
-        ...
-
-    def __getitem__(self, index: int) -> Structure:
-        ...
-
-class Updater(Protocol):
-    """Interface for potential weight updaters."""
-
-    def fit(self, dataset: StructureDataset) -> Dict:
-        ...
-
-
-class Potential(Protocol):
-    """Interface for Potential."""
-
-    settings: PotentialSettings
-    elements: Tuple[Element, ...]
-    atomic_potential: Dict[Element, AtomicPotential]
-    model_params: Dict[Element, frozendict]
-
-
-class KalmanFilterUpdater(Updater):
+class KalmanFilterUpdater:
     """
     A potential trainer which uses Kalman filter to update model weights (see this_).
 
     .. _this: https://pubs.acs.org/doi/10.1021/acs.jctc.8b01092
     """
 
     # https://github.com/CompPhysVienna/n2p2/blob/master/src/libnnptrain/KalmanFilter.cpp
 
-    def __init__(self, potential: Potential) -> None:
-        self.potential: Potential = potential
+    def __init__(self, potential: PotentialInterface) -> None:
+        self.potential: PotentialInterface = potential
         self._init_parameters()
         self._init_matrices()
 
     def _init_parameters(self) -> None:
         """Set required parameters from the potential settings."""
         settings: PotentialSettings = self.potential.settings
         self.kalman_type: int = settings.kalman_type
@@ -94,15 +75,15 @@
         # Error covariance matrix
         self.P: Array = (1.0 / self.epsilon) * jnp.identity(
             self.num_states, dtype=default_dtype.FLOATX
         )
 
     def fit(
         self,
-        dataset: StructureDataset,
+        dataset: DatasetInterface,
     ) -> defaultdict:
         """
         Fit potential weights.
 
         :param dataset: training dataset
         :type dataset: StructureDataset
         """
@@ -158,25 +139,23 @@
 
         # ----------------------
 
         indices: list[int] = [i for i in range(len(dataset))]
 
         history = defaultdict(list)
         for epoch in range(settings.epochs):
-
             print(f"Epoch: {epoch + 1} of {settings.epochs}")
             random.shuffle(indices)
 
             loss_energy_per_epoch: Array = jnp.asarray(0.0)
             loss_force_per_epoch: Array = jnp.asarray(0.0)
             num_energy_updates_per_epoch: int = 0
             num_force_updates_per_epoch: int = 0
 
             for index in tqdm(indices):
-
                 structure: Structure = dataset[index]
 
                 # Error and jacobian matrices
                 if np.random.rand() < self.force_fraction:
                     Xi = self.beta * compute_force_error(
                         self.W,
                         structure,
```

### Comparing `jaxip-0.5.8/jaxip/potentials/nnp/metrics.py` & `jaxip-0.5.9/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/potentials/nnp/potential.py` & `jaxip-0.5.9/jaxip/potentials/nnp/potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,113 +2,102 @@
 
 from collections import defaultdict
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, Optional, Protocol, Tuple
 
 import jax.numpy as jnp
-from ase import data
 from frozendict import frozendict
 from jax import random
 from tqdm import tqdm
 
 from jaxip.atoms.element import ElementMap
 from jaxip.atoms.structure import Structure
+from jaxip.datasets.dataset import DatasetInterface
 from jaxip.datasets.runner import RunnerDataset
 from jaxip.descriptors.acsf.acsf import ACSF
 from jaxip.descriptors.acsf.angular import G3, G9
 from jaxip.descriptors.acsf.cutoff import CutoffFunction
 from jaxip.descriptors.acsf.radial import G1, G2
 from jaxip.descriptors.scaler import Scaler
 from jaxip.logger import logger
 from jaxip.models.nn.initializer import UniformInitializer
 from jaxip.models.nn.network import NeuralNetworkModel
 from jaxip.potentials._energy import _compute_energy
 from jaxip.potentials._force import _compute_force
 from jaxip.potentials.atomic_potential import AtomicPotential
 from jaxip.potentials.nnp.gradient_descent import GradientDescentUpdater
 from jaxip.potentials.nnp.kalman_filter import KalmanFilterUpdater
-from jaxip.potentials.nnp.settings import PotentialSettings
+from jaxip.potentials.nnp.settings import (
+    NeuralNetworkPotentialSettings as PotentialSettings,
+)
 from jaxip.types import Array, Element
 
 
-class StructureDataset(Protocol):
-    """A data container for atom data structure."""
-
-    def __len__(self) -> int:
-        ...
-
-    def __getitem__(self, index: int) -> Structure:
-        ...
-
-class Updater(Protocol):
+class UpdaterInterface(Protocol):
     """Interface for potential weight updaters."""
 
-    def fit(self, dataset: StructureDataset) -> Dict:
+    def fit(self, dataset: DatasetInterface) -> Dict:
         ...
 
 
 @dataclass
 class NeuralNetworkPotential:
     """
     High-dimensional neural network potential (HDNNP) - second generation.
 
     It contains all the required descriptors, scalers, and neural networks for each element,
     and an updater to fit the potential model using the reference structure data.
 
     Example
     -------
-    Ways to initialize neural network potential.
+    Different methods to initialize neural network potential (NNP):
 
     .. code-block:: python
         :linenos:
 
         from jaxip.potentials import NeuralNetworkPotential
-        from jaxip.potentials import PotentialSettings
+        from jaxip.potentials.nnp import NeuralNetworkPotentialSettings as Settings
 
         # Method #1 (potential file)
         nnp1 = NeuralNetworkPotential.create_from_file("input.nn")
 
         # Method #2 (json file)
         nnp3 = NeuralNetworkPotential.create_from_file('h2o.json')
 
         # Method #3 (dictionary of parameters)
-        settings = PotentialSettings(**params_dict)
+        settings = Settings(**params_dict)
         nnp3 = NeuralNetworkPotential(settings)
     """
 
     settings: PotentialSettings = field(repr=False)
     output_dir: Path = field(default=Path("."), repr=False)
     atomic_potential: Dict[Element, AtomicPotential] = field(
         default_factory=dict, repr=True, init=False
     )
     model_params: Dict[Element, frozendict] = field(
         default_factory=dict, repr=False, init=False
     )
-    updater: Optional[Updater] = field(default=None, repr=False, init=False)
+    updater: Optional[UpdaterInterface] = field(default=None, repr=False, init=False)
 
     @classmethod
     def create_from_file(cls, filename: Path) -> NeuralNetworkPotential:
         """Create an instance of the potential from input file (RuNNer format)."""
         logger.info("Creating potential from input file (RuNNer format)")
         potfile = Path(filename)
         suffix: str = potfile.suffix.lower()
         if ".json" == suffix:
             logger.info(f"Initializing from json file: {potfile.name}")
             settings = PotentialSettings.create_from_json(potfile)
-        elif ".nn" == suffix:
+        else:
             logger.info(
                 f"Initializing from original RuNNer file format: {potfile.name}"
             )
             settings = PotentialSettings.create_from_file(potfile)
-        else:
-            logger.error(
-                f"Unknown potential setting file format: {potfile.name}",
-                exception=TypeError,
-            )
+
         return NeuralNetworkPotential(
             settings=settings,  # type: ignore
             output_dir=potfile.parent,
         )
 
     def __post_init__(self) -> None:
         """
@@ -339,15 +328,14 @@
     # ------------------------------------------------------------------------
 
     def fit_scaler(self, dataset: RunnerDataset) -> None:
         """
         Fit scaler parameters for each element using the input structure data.
         No gradient history is required here.
         """
-        # loader = TorchDataLoader(dataset, collate_fn=lambda batch: batch)
         print("Fitting descriptor scaler...")
         try:
             dataset_size: int = len(dataset)
             for index in tqdm(range(dataset_size)):
                 structure: Structure = dataset[index]
                 elements: Tuple[Element, ...] = structure.elements
                 for element in elements:
@@ -499,7 +487,10 @@
         """Return scaler for each element."""
         return {elem: pot.scaler for elem, pot in self.atomic_potential.items()}
 
     @property
     def model(self) -> Dict:
         """Return model for each element."""
         return {elem: pot.model for elem, pot in self.atomic_potential.items()}
+
+
+NNP = NeuralNetworkPotential
```

### Comparing `jaxip-0.5.8/jaxip/potentials/nnp/settings.py` & `jaxip-0.5.9/jaxip/potentials/nnp/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 gradient_type_map: Mapping[str, str] = {
     "0": "fixed_step",
     "1": "adam",
 }
 
 
-class PotentialSettings(_CFG):
+class NeuralNetworkPotentialSettings(_CFG):
     """
     A configuration class for neural network potential parameters.
 
     It contains a collections of all potential setting keywords and their default values.
     """
 
     # sphinx-pydantic can be useful to better document pydantic classes
@@ -136,15 +136,15 @@
     cutoff_type: str = "tanh"
     scale_type: str = "center"
     scale_min_short: float = 0.0
     scale_max_short: float = 1.0
     symfunction_short: List[SymFuncArgs] = Field(default_factory=list)
 
     @classmethod
-    def create_from_file(cls, filename: Path) -> PotentialSettings:
+    def create_from_file(cls, filename: Path) -> NeuralNetworkPotentialSettings:
         """
         Read all potential settings from the input file.
 
         Parameters such as `elements`, `cutoff type`, `symmetry functions`, `neural network`, `training parameters`, etc
         (see `here <https://compphysvienna.github.io/n2p2/topics/keywords.html>`_).
         """
```

### Comparing `jaxip-0.5.8/jaxip/pytree.py` & `jaxip-0.5.9/jaxip/pytree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Optional, Tuple
+from typing import Any, Dict, Tuple
 
 from jax import tree_util
 
 from jaxip.logger import logger
 
 
 class BaseJaxPytreeDataClass:
@@ -37,15 +37,15 @@
         return (children, aux_data)
 
     @classmethod
     def _tree_unflatten(
         cls, aux_data: Dict[str, Any], children: Tuple[Any, ...]
     ) -> BaseJaxPytreeDataClass:
         return cls(*children, **aux_data)  # type: ignore
-    
+
     def __hash__(self) -> int:
         """
         Define hash method based on the `JAX JIT compilation` static attributes.
         This is useful when wants to identify changes on the static arguments of a jit-compiled method.
         """
         aux_data: Dict[str, Any] = self._tree_flatten()[1]
         return hash(tuple(frozenset(sorted(aux_data.items()))))
@@ -62,35 +62,42 @@
         """Get JAX JIT compilation static attribute names."""
         dynamic_attributes = cls._get_jit_dynamic_attributes()
         return tuple(
             attr
             for attr in cls.__annotations__.keys()
             if attr not in dynamic_attributes
         )
-    
+
     @classmethod
     def _assert_jit_attributes(
-        cls, 
-        available: Tuple[str, ...], 
-        expected: Tuple[str, ...], 
+        cls,
+        available: Tuple[str, ...],
+        expected: Tuple[str, ...],
         tag: str = "",
     ) -> None:
         """Assert to ensure jit (static or dynamics) attributes are correctly identified."""
-        if sorted(available) != sorted(expected): # type: ignore
+        if sorted(available) != sorted(expected):  # type: ignore
             logger.error(
                 f"Expecting JIT {tag} attributes: {expected} but got {available}",
-                exception=AssertionError
-        )
-            
+                exception=AssertionError,
+            )
+
     @classmethod
-    def _assert_jit_static_attributes(cls, expected: Tuple[str, ...] = tuple()) -> None: 
-        cls._assert_jit_attributes(cls._get_jit_static_attributes(), expected, tag="static")
+    def _assert_jit_static_attributes(cls, expected: Tuple[str, ...] = tuple()) -> None:
+        cls._assert_jit_attributes(
+            cls._get_jit_static_attributes(), expected, tag="static"
+        )
 
     @classmethod
-    def _assert_jit_dynamic_attributes(cls, expected: Tuple[str, ...] = tuple()) -> None: 
-        cls._assert_jit_attributes(cls._get_jit_dynamic_attributes(), expected, tag="dynamic")
+    def _assert_jit_dynamic_attributes(
+        cls, expected: Tuple[str, ...] = tuple()
+    ) -> None:
+        cls._assert_jit_attributes(
+            cls._get_jit_dynamic_attributes(), expected, tag="dynamic"
+        )
+
 
 def register_jax_pytree_node(cls) -> None:
     """Register the input class as internal JAX pytree node."""
     tree_util.register_pytree_node(
         cls, cls._tree_flatten, cls._tree_unflatten  # type: ignore
     )
```

### Comparing `jaxip-0.5.8/jaxip/types.py` & `jaxip-0.5.9/jaxip/types.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/utils/attribute.py` & `jaxip-0.5.9/jaxip/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/utils/batch.py` & `jaxip-0.5.9/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/utils/compare.py` & `jaxip-0.5.9/jaxip/utils/compare.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/utils/profiler.py` & `jaxip-0.5.9/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip/utils/tokenize.py` & `jaxip-0.5.9/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/jaxip.egg-info/PKG-INFO` & `jaxip-0.5.9/jaxip.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.5.8
+Version: 0.5.9
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,16 +49,16 @@
 
 
 See `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
-Main features
--------------
+Features
+--------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
 * It uses `autograd` to make defining new descriptors straightforward.
 * Jaxip is written purely in Python and optimized with `just-in-time` (JIT) compilation.
 * It also supports `GPU-accelerated` computing, which can significantly speed up preprocessing and model training.
 
 .. warning::
         This package is under heavy development and the current focus is on the implementation of high-dimensional
```

### Comparing `jaxip-0.5.8/jaxip.egg-info/SOURCES.txt` & `jaxip-0.5.9/jaxip.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,17 @@
 docs/jaxip.rst
 docs/jaxip.utils.rst
 docs/make.bat
 docs/modules.rst
 docs/readme.rst
 docs/theory.rst
 docs/usage.rst
-docs/_build/doctrees/nbsphinx/notebooks_potential_training_30_21.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_38_0.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_45_0.png
 docs/_build/doctrees/nbsphinx/notebooks_tutorials_51_0.png
-docs/_build/html/_images/notebooks_potential_training_30_21.png
 docs/_build/html/_images/notebooks_tutorials_38_0.png
 docs/_build/html/_images/notebooks_tutorials_45_0.png
 docs/_build/html/_images/notebooks_tutorials_51_0.png
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 docs/images/flowchart.drawio.png
@@ -61,39 +59,42 @@
 jaxip/atoms/_neighbor.py
 jaxip/atoms/_structure.py
 jaxip/atoms/box.py
 jaxip/atoms/element.py
 jaxip/atoms/neighbor.py
 jaxip/atoms/structure.py
 jaxip/datasets/__init__.py
+jaxip/datasets/dataset.py
 jaxip/datasets/runner.py
 jaxip/datasets/transformer.py
 jaxip/descriptors/__init__.py
-jaxip/descriptors/base.py
+jaxip/descriptors/descriptor.py
 jaxip/descriptors/scaler.py
 jaxip/descriptors/acsf/__init__.py
 jaxip/descriptors/acsf/_acsf.py
 jaxip/descriptors/acsf/acsf.py
 jaxip/descriptors/acsf/angular.py
 jaxip/descriptors/acsf/cutoff.py
 jaxip/descriptors/acsf/radial.py
 jaxip/descriptors/acsf/symmetry.py
 jaxip/models/__init__.py
+jaxip/models/model.py
 jaxip/models/nn/__init__.py
 jaxip/models/nn/activation.py
 jaxip/models/nn/initializer.py
 jaxip/models/nn/network.py
 jaxip/potentials/__init__.py
 jaxip/potentials/_energy.py
 jaxip/potentials/_force.py
 jaxip/potentials/atomic_potential.py
 jaxip/potentials/nnp/__init__.py
 jaxip/potentials/nnp/gradient_descent.py
 jaxip/potentials/nnp/kalman_filter.py
 jaxip/potentials/nnp/metrics.py
+jaxip/potentials/nnp/nnp.py
 jaxip/potentials/nnp/potential.py
 jaxip/potentials/nnp/settings.py
 jaxip/utils/__init__.py
 jaxip/utils/attribute.py
 jaxip/utils/batch.py
 jaxip/utils/compare.py
 jaxip/utils/profiler.py
```

### Comparing `jaxip-0.5.8/setup.py` & `jaxip-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.5.9/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.5.9/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.5.9/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.5.9/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/h2o.data` & `jaxip-0.5.9/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/h2o.json` & `jaxip-0.5.9/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/test_acsf.py` & `jaxip-0.5.9/tests/test_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/test_nn.py` & `jaxip-0.5.9/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/test_nnp.py` & `jaxip-0.5.9/tests/test_nnp.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 import jax.numpy as jnp
 import pytest
 
 from jaxip.datasets import RunnerDataset
 from jaxip.potentials import NeuralNetworkPotential
-from jaxip.potentials.nnp.settings import PotentialSettings
+from jaxip.potentials.nnp.settings import (
+    NeuralNetworkPotentialSettings as PotentialSettings,
+)
 
 dataset_file = Path("tests", "h2o.data")
 potential_file = Path("tests", "h2o.json")
 
 
 class TestNeuralNetworkPotential:
     dataset = RunnerDataset(dataset_file)
@@ -99,15 +101,15 @@
     ) -> None:
         structure = dataset[0]
         nnp.output_dir = potential_file.parent
         nnp.save()
 
         settings_new = nnp.settings.copy()
         settings_new.random_seed = 4321
-        nnp_new = NeuralNetworkPotential(settings_new)
+        nnp_new = NeuralNetworkPotential(settings=settings_new)
         nnp_new.fit_scaler(dataset)
         nnp_new.output_dir = potential_file.parent
 
         assert not nnp.settings == nnp_new.settings
         assert not jnp.allclose(nnp(structure), nnp_new(structure))
         nnp_new.load()
         assert jnp.allclose(nnp(structure), nnp_new(structure))
```

### Comparing `jaxip-0.5.8/tests/test_runner.py` & `jaxip-0.5.9/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/test_scaler.py` & `jaxip-0.5.9/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/test_structure.py` & `jaxip-0.5.9/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/weights.001.pkl` & `jaxip-0.5.9/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.5.8/tests/weights.008.pkl` & `jaxip-0.5.9/tests/weights.008.pkl`

 * *Files identical despite different names*

