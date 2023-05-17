# Comparing `tmp/pyikarus-0.3.0.dev202310000082.tar.gz` & `tmp/pyikarus-0.3.0.dev202310000083.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.0.dev202310000082.tar", last modified: Wed May 17 11:56:25 2023, max compression
+gzip compressed data, was "pyikarus-0.3.0.dev202310000083.tar", last modified: Wed May 17 12:28:25 2023, max compression
```

## Comparing `pyikarus-0.3.0.dev202310000082.tar` & `pyikarus-0.3.0.dev202310000083.tar`

### file list

```diff
@@ -1,328 +1,328 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.754805 pyikarus-0.3.0.dev202310000082/
--rw-r--r--   0 user      (1001) user      (1001)      312 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/.bettercodehub.yml
--rw-r--r--   0 user      (1001) user      (1001)     1300 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/.clang-format
--rw-r--r--   0 user      (1001) user      (1001)     1017 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/.cmake-format
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.666806 pyikarus-0.3.0.dev202310000082/.github/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.678806 pyikarus-0.3.0.dev202310000082/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 user      (1001) user      (1001)      460 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 user      (1001) user      (1001)      615 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.682806 pyikarus-0.3.0.dev202310000082/.github/workflows/
--rw-r--r--   0 user      (1001) user      (1001)      476 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/codespell.yml
--rw-r--r--   0 user      (1001) user      (1001)     1034 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 user      (1001) user      (1001)     4900 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/createRelease.yml
--rw-r--r--   0 user      (1001) user      (1001)     1635 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/debian-coverage.yml
--rw-r--r--   0 user      (1001) user      (1001)     2414 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/debian.yml
--rw-r--r--   0 user      (1001) user      (1001)     2042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/ghpages.yml
--rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/reuseLint.yml
--rw-r--r--   0 user      (1001) user      (1001)     2854 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/runExamples.yml
--rw-r--r--   0 user      (1001) user      (1001)     1212 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/.github/workflows/style.yml
--rw-r--r--   0 user      (1001) user      (1001)      455 2023-05-17 07:45:53.000000 pyikarus-0.3.0.dev202310000082/.gitignore
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.682806 pyikarus-0.3.0.dev202310000082/.reuse/
--rw-r--r--   0 user      (1001) user      (1001)      661 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/.reuse/dep5
--rw-r--r--   0 user      (1001) user      (1001)     3324 2023-05-15 08:38:51.000000 pyikarus-0.3.0.dev202310000082/CHANGELOG.md
--rw-r--r--   0 user      (1001) user      (1001)     1318 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5335 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/CODE_OF_CONDUCT.md
--rw-r--r--   0 user      (1001) user      (1001)      759 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/LICENSE.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.682806 pyikarus-0.3.0.dev202310000082/LICENSES/
--rw-r--r--   0 user      (1001) user      (1001)    18375 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     7048 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/LICENSES/CC0-1.0.txt
--rw-r--r--   0 user      (1001) user      (1001)    42098 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 user      (1001) user      (1001)     1078 2023-03-24 20:46:08.000000 pyikarus-0.3.0.dev202310000082/LICENSES/MIT.txt
--rw-r--r--   0 user      (1001) user      (1001)    16727 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/LICENSES/MPL-2.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-17 11:56:25.754805 pyikarus-0.3.0.dev202310000082/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)     3229 2023-03-06 10:17:28.000000 pyikarus-0.3.0.dev202310000082/README.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.666806 pyikarus-0.3.0.dev202310000082/Testing/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.682806 pyikarus-0.3.0.dev202310000082/Testing/Temporary/
--rw-r--r--   0 user      (1001) user      (1001)        4 2023-05-15 11:55:16.000000 pyikarus-0.3.0.dev202310000082/Testing/Temporary/CTestCostData.txt
--rw-r--r--   0 user      (1001) user      (1001)      121 2023-05-15 11:55:16.000000 pyikarus-0.3.0.dev202310000082/Testing/Temporary/LastTest.log
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.686806 pyikarus-0.3.0.dev202310000082/cmake/
--rw-r--r--   0 user      (1001) user      (1001)      973 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/cmake/CPM.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.686806 pyikarus-0.3.0.dev202310000082/cmake/FormatTarget/
--rw-r--r--   0 user      (1001) user      (1001)     1270 2023-03-10 08:15:25.000000 pyikarus-0.3.0.dev202310000082/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.686806 pyikarus-0.3.0.dev202310000082/cmake/modules/
--rw-r--r--   0 user      (1001) user      (1001)      715 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      683 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      740 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      691 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      226 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/cmake/modules/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      446 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 user      (1001) user      (1001)     2040 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/cmake/tools.cmake
--rw-r--r--   0 user      (1001) user      (1001)      148 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/codecov.yml
--rw-r--r--   0 user      (1001) user      (1001)      121 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/codespellignore
--rw-r--r--   0 user      (1001) user      (1001)     1588 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/config.h.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.686806 pyikarus-0.3.0.dev202310000082/docs/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.686806 pyikarus-0.3.0.dev202310000082/docs/BuildLocally/
--rw-r--r--   0 user      (1001) user      (1001)      439 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      333 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.686806 pyikarus-0.3.0.dev202310000082/docs/__pycache__/
--rw-r--r--   0 user      (1001) user      (1001)     1136 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 user      (1001) user      (1001)     6961 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/literature.bib
--rw-r--r--   0 user      (1001) user      (1001)      117 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/literature.bib.license
--rw-r--r--   0 user      (1001) user      (1001)     1245 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/mkdocs-macros.py
--rw-r--r--   0 user      (1001) user      (1001)      394 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/mkdocs.insiders.yml
--rw-r--r--   0 user      (1001) user      (1001)     5042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/docs/mkdocs.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.666806 pyikarus-0.3.0.dev202310000082/docs/overrides/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.686806 pyikarus-0.3.0.dev202310000082/docs/overrides/partials/
--rw-r--r--   0 user      (1001) user      (1001)     1732 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/overrides/partials/comments.html
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.690806 pyikarus-0.3.0.dev202310000082/docs/website/
--rw-r--r--   0 user      (1001) user      (1001)       24 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/.meta.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.690806 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/
--rw-r--r--   0 user      (1001) user      (1001)     4710 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/assembler.md
--rw-r--r--   0 user      (1001) user      (1001)     6387 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 user      (1001) user      (1001)     2024 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 user      (1001) user      (1001)     3237 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 user      (1001) user      (1001)     8524 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 user      (1001) user      (1001)     2745 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/grids.md
--rw-r--r--   0 user      (1001) user      (1001)     4121 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/index.md
--rw-r--r--   0 user      (1001) user      (1001)     4932 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/localBasis.md
--rw-r--r--   0 user      (1001) user      (1001)    44213 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 user      (1001) user      (1001)     3978 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/manifolds.md
--rw-r--r--   0 user      (1001) user      (1001)     2590 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 user      (1001) user      (1001)     3086 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/observer.md
--rw-r--r--   0 user      (1001) user      (1001)     5211 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.690806 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/
--rw-r--r--   0 user      (1001) user      (1001)     6655 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 user      (1001) user      (1001)     7251 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/computePi.md
--rw-r--r--   0 user      (1001) user      (1001)     5439 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 user      (1001) user      (1001)     7055 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 user      (1001) user      (1001)     2164 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/index.md
--rw-r--r--   0 user      (1001) user      (1001)     7702 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 user      (1001) user      (1001)     5114 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 user      (1001) user      (1001)     6200 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 user      (1001) user      (1001)     4071 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.694806 pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/
--rw-r--r--   0 user      (1001) user      (1001)     2439 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 user      (1001) user      (1001)     1002 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 user      (1001) user      (1001)     2415 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 user      (1001) user      (1001)     1762 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.694806 pyikarus-0.3.0.dev202310000082/docs/website/04_blog/
--rw-r--r--   0 user      (1001) user      (1001)      274 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/04_blog/.authors.yml
--rw-r--r--   0 user      (1001) user      (1001)        7 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/04_blog/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.694806 pyikarus-0.3.0.dev202310000082/docs/website/04_blog/posts/
--rw-r--r--   0 user      (1001) user      (1001)     7731 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.694806 pyikarus-0.3.0.dev202310000082/docs/website/05_cppReferences/
--rw-r--r--   0 user      (1001) user      (1001)     2324 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.694806 pyikarus-0.3.0.dev202310000082/docs/website/99_Literature/
--rw-r--r--   0 user      (1001) user      (1001)      169 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.694806 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.698806 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 user      (1001) user      (1001)    52795 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 user      (1001) user      (1001)    46250 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 user      (1001) user      (1001)     2852 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 user      (1001) user      (1001)    17924 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 user      (1001) user      (1001)     9455 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.702806 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 user      (1001) user      (1001)    35234 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 user      (1001) user      (1001)    62184 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 user      (1001) user      (1001)     2281 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 user      (1001) user      (1001)    40033 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 user      (1001) user      (1001)    25505 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 user      (1001) user      (1001)     8101 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/logo_blue.svg
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/logo_blue.svg.license
--rw-r--r--   0 user      (1001) user      (1001)     8255 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/logo_white.svg
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/logo_white.svg.license
--rw-r--r--   0 user      (1001) user      (1001)     4364 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000082/docs/website/download.md
--rw-r--r--   0 user      (1001) user      (1001)      244 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/gallery.md
--rw-r--r--   0 user      (1001) user      (1001)     1358 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.702806 pyikarus-0.3.0.dev202310000082/docs/website/javascripts/
--rw-r--r--   0 user      (1001) user      (1001)      486 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.702806 pyikarus-0.3.0.dev202310000082/docs/website/stylesheets/
--rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/docs/website/stylesheets/extra.css
--rw-r--r--   0 user      (1001) user      (1001)      502 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/dune.module
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.702806 pyikarus-0.3.0.dev202310000082/ikarus/
--rw-r--r--   0 user      (1001) user      (1001)      748 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/ikarus/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.702806 pyikarus-0.3.0.dev202310000082/ikarus/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      268 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)    11069 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 user      (1001) user      (1001)    10714 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.706806 pyikarus-0.3.0.dev202310000082/ikarus/controlRoutines/
--rw-r--r--   0 user      (1001) user      (1001)      239 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2575 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 user      (1001) user      (1001)     2970 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.706806 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/
--rw-r--r--   0 user      (1001) user      (1001)      349 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      185 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.706806 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feBases/
--rw-r--r--   0 user      (1001) user      (1001)      282 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2925 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     2305 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     1827 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     1041 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feRequirements.cpp
--rw-r--r--   0 user      (1001) user      (1001)     8419 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 user      (1001) user      (1001)     1338 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.710806 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/
--rw-r--r--   0 user      (1001) user      (1001)      345 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)    19628 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 user      (1001) user      (1001)    12549 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.710806 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 user      (1001) user      (1001)      397 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5699 2023-05-08 12:58:29.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 user      (1001) user      (1001)     2718 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 user      (1001) user      (1001)     4635 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 user      (1001) user      (1001)     3809 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 user      (1001) user      (1001)     5734 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 user      (1001) user      (1001)      473 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 user      (1001) user      (1001)     8010 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 user      (1001) user      (1001)     1196 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 user      (1001) user      (1001)     7827 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 user      (1001) user      (1001)    12655 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.714806 pyikarus-0.3.0.dev202310000082/ikarus/linearAlgebra/
--rw-r--r--   0 user      (1001) user      (1001)      301 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     6734 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 user      (1001) user      (1001)     7791 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 user      (1001) user      (1001)    12303 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.714806 pyikarus-0.3.0.dev202310000082/ikarus/python/
--rw-r--r--   0 user      (1001) user      (1001)      294 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.714806 pyikarus-0.3.0.dev202310000082/ikarus/python/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      249 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3149 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.714806 pyikarus-0.3.0.dev202310000082/ikarus/python/basis/
--rw-r--r--   0 user      (1001) user      (1001)      237 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     4559 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.714806 pyikarus-0.3.0.dev202310000082/ikarus/python/dirichletValues/
--rw-r--r--   0 user      (1001) user      (1001)      257 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     4116 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.718806 pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/
--rw-r--r--   0 user      (1001) user      (1001)      303 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5036 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.718806 pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/materials/
--rw-r--r--   0 user      (1001) user      (1001)      259 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5107 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 user      (1001) user      (1001)     5503 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.726806 pyikarus-0.3.0.dev202310000082/ikarus/python/test/
--rw-r--r--   0 user      (1001) user      (1001)      564 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     4062 2023-05-17 08:21:12.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 user      (1001) user      (1001)  2704357 2023-05-15 11:50:45.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/test/nameTest.vtu
--rw-r--r--   0 user      (1001) user      (1001)     4447 2023-05-15 09:03:11.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 user      (1001) user      (1001)      862 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.726806 pyikarus-0.3.0.dev202310000082/ikarus/python/utils/
--rw-r--r--   0 user      (1001) user      (1001)      245 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1181 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000082/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.726806 pyikarus-0.3.0.dev202310000082/ikarus/solver/
--rw-r--r--   0 user      (1001) user      (1001)      211 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.726806 pyikarus-0.3.0.dev202310000082/ikarus/solver/linearSolver/
--rw-r--r--   0 user      (1001) user      (1001)      244 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     8891 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.726806 pyikarus-0.3.0.dev202310000082/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 user      (1001) user      (1001)      272 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5407 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 user      (1001) user      (1001)     8297 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 user      (1001) user      (1001)    18574 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.734806 pyikarus-0.3.0.dev202310000082/ikarus/utils/
--rw-r--r--   0 user      (1001) user      (1001)      712 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1741 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/algorithms.hh
--rw-r--r--   0 user      (1001) user      (1001)      878 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     1445 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/basis.hh
--rw-r--r--   0 user      (1001) user      (1001)     6930 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/concepts.hh
--rw-r--r--   0 user      (1001) user      (1001)      503 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.734806 pyikarus-0.3.0.dev202310000082/ikarus/utils/drawing/
--rw-r--r--   0 user      (1001) user      (1001)      262 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1654 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 user      (1001) user      (1001)      544 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 user      (1001) user      (1001)      703 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     2484 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 user      (1001) user      (1001)     2347 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 user      (1001) user      (1001)      682 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 user      (1001) user      (1001)     1367 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 user      (1001) user      (1001)      724 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 user      (1001) user      (1001)     3611 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 user      (1001) user      (1001)     2171 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6359 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 user      (1001) user      (1001)     3152 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/init.hh
--rw-r--r--   0 user      (1001) user      (1001)    15244 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     1711 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.734806 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/
--rw-r--r--   0 user      (1001) user      (1001)      450 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1554 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 user      (1001) user      (1001)     2307 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 user      (1001) user      (1001)      905 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1053 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1132 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1985 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 user      (1001) user      (1001)     5497 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/observer.hh
--rw-r--r--   0 user      (1001) user      (1001)      489 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 user      (1001) user      (1001)     4159 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 user      (1001) user      (1001)     1131 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/polyfit.cpp
--rw-r--r--   0 user      (1001) user      (1001)      570 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/polyfit.hh
--rw-r--r--   0 user      (1001) user      (1001)    10054 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 user      (1001) user      (1001)    15044 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/ikarus/utils/traits.hh
--rw-r--r--   0 user      (1001) user      (1001)      432 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/ikarus.pc.in
--rw-r--r--   0 user      (1001) user      (1001)      196 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/iwyu.imp
--rw-r--r--   0 user      (1001) user      (1001)      422 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000082/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.734806 pyikarus-0.3.0.dev202310000082/python/
--rw-r--r--   0 user      (1001) user      (1001)      586 2023-05-17 07:43:44.000000 pyikarus-0.3.0.dev202310000082/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.738806 pyikarus-0.3.0.dev202310000082/python/ikarus/
--rw-r--r--   0 user      (1001) user      (1001)      517 2023-05-15 08:59:18.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      605 2023-05-17 11:55:51.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     5636 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.738806 pyikarus-0.3.0.dev202310000082/python/ikarus/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      167 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2300 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/assembler/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     1491 2023-05-15 08:55:23.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/basis.py
--rw-r--r--   0 user      (1001) user      (1001)     1408 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.738806 pyikarus-0.3.0.dev202310000082/python/ikarus/finite_elements/
--rw-r--r--   0 user      (1001) user      (1001)      173 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/finite_elements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3465 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/finite_elements/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     1792 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/materials.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.738806 pyikarus-0.3.0.dev202310000082/python/ikarus/utils/
--rw-r--r--   0 user      (1001) user      (1001)      163 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1496 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000082/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.742806 pyikarus-0.3.0.dev202310000082/python/pyikarus.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-17 11:56:25.000000 pyikarus-0.3.0.dev202310000082/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)     9951 2023-05-17 11:56:25.000000 pyikarus-0.3.0.dev202310000082/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-17 11:56:25.000000 pyikarus-0.3.0.dev202310000082/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-17 11:56:25.000000 pyikarus-0.3.0.dev202310000082/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 user      (1001) user      (1001)        7 2023-05-17 11:56:25.000000 pyikarus-0.3.0.dev202310000082/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) user      (1001)      628 2023-05-17 11:28:20.000000 pyikarus-0.3.0.dev202310000082/python/setup.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.742806 pyikarus-0.3.0.dev202310000082/sandbox/
--rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/sandbox/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.742806 pyikarus-0.3.0.dev202310000082/sandbox/src/
--rw-r--r--   0 user      (1001) user      (1001)     1220 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000082/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.742806 pyikarus-0.3.0.dev202310000082/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 user      (1001) user      (1001)   674469 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 user      (1001) user      (1001)      320 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/sandbox/src/sandbox.cpp
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-17 11:56:25.754805 pyikarus-0.3.0.dev202310000082/setup.cfg
--rw-r--r--   0 user      (1001) user      (1001)     1894 2023-05-17 11:56:21.000000 pyikarus-0.3.0.dev202310000082/setup.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.742806 pyikarus-0.3.0.dev202310000082/tests/
--rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/tests/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.750805 pyikarus-0.3.0.dev202310000082/tests/src/
--rw-r--r--   0 user      (1001) user      (1001)     1418 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3906 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000082/tests/src/assemblerTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     9913 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/common.hh
--rw-r--r--   0 user      (1001) user      (1001)     2639 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/dependenciesTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6520 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/dirichletValueTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     3820 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/easTest.hh
--rw-r--r--   0 user      (1001) user      (1001)     1473 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/enhancedAssumedStrainsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)      608 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/factories.hh
--rw-r--r--   0 user      (1001) user      (1001)     1870 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/functionTraitsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     2661 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/linearElasticityTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     2378 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/manifoldsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     7961 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/materialTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6770 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000082/tests/src/nonLinearElasticityTest.hh
--rw-r--r--   0 user      (1001) user      (1001)      724 2023-05-08 13:07:10.000000 pyikarus-0.3.0.dev202310000082/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rw-r--r--   0 user      (1001) user      (1001)      729 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/nonLinearElasticityTestSVK.cpp
--rw-r--r--   0 user      (1001) user      (1001)     9936 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/nonLinearOperatorTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6327 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/pathFollowingTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     1651 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/polyFitTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)      695 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/pythonConversionTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     1292 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 user      (1001) user      (1001)     5805 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/testFEElement.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 11:56:25.754805 pyikarus-0.3.0.dev202310000082/tests/src/testFiles/
--rw-r--r--   0 user      (1001) user      (1001)     9028 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 user      (1001) user      (1001)      395 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 user      (1001) user      (1001)      497 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 user      (1001) user      (1001)      546 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 user      (1001) user      (1001)    11431 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000082/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 user      (1001) user      (1001)     1114 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000082/tests/src/testHelpers.hh
--rw-r--r--   0 user      (1001) user      (1001)    17595 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000082/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.063904 pyikarus-0.3.0.dev202310000083/
+-rw-r--r--   0 user      (1001) user      (1001)      312 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/.bettercodehub.yml
+-rw-r--r--   0 user      (1001) user      (1001)     1300 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/.clang-format
+-rw-r--r--   0 user      (1001) user      (1001)     1017 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/.cmake-format
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.979904 pyikarus-0.3.0.dev202310000083/.github/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.991904 pyikarus-0.3.0.dev202310000083/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 user      (1001) user      (1001)      460 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 user      (1001) user      (1001)      615 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.991904 pyikarus-0.3.0.dev202310000083/.github/workflows/
+-rw-r--r--   0 user      (1001) user      (1001)      476 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/codespell.yml
+-rw-r--r--   0 user      (1001) user      (1001)     1034 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 user      (1001) user      (1001)     4900 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/createRelease.yml
+-rw-r--r--   0 user      (1001) user      (1001)     1635 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 user      (1001) user      (1001)     2414 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/debian.yml
+-rw-r--r--   0 user      (1001) user      (1001)     2042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/ghpages.yml
+-rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/reuseLint.yml
+-rw-r--r--   0 user      (1001) user      (1001)     2854 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/runExamples.yml
+-rw-r--r--   0 user      (1001) user      (1001)     1212 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/.github/workflows/style.yml
+-rw-r--r--   0 user      (1001) user      (1001)      455 2023-05-17 07:45:53.000000 pyikarus-0.3.0.dev202310000083/.gitignore
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.991904 pyikarus-0.3.0.dev202310000083/.reuse/
+-rw-r--r--   0 user      (1001) user      (1001)      661 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/.reuse/dep5
+-rw-r--r--   0 user      (1001) user      (1001)     3324 2023-05-15 08:38:51.000000 pyikarus-0.3.0.dev202310000083/CHANGELOG.md
+-rw-r--r--   0 user      (1001) user      (1001)     1318 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5335 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/CODE_OF_CONDUCT.md
+-rw-r--r--   0 user      (1001) user      (1001)      759 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/LICENSE.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.995904 pyikarus-0.3.0.dev202310000083/LICENSES/
+-rw-r--r--   0 user      (1001) user      (1001)    18375 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)     7048 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)    42098 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1078 2023-03-24 20:46:08.000000 pyikarus-0.3.0.dev202310000083/LICENSES/MIT.txt
+-rw-r--r--   0 user      (1001) user      (1001)    16727 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-17 12:28:25.063904 pyikarus-0.3.0.dev202310000083/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)     3229 2023-03-06 10:17:28.000000 pyikarus-0.3.0.dev202310000083/README.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.979904 pyikarus-0.3.0.dev202310000083/Testing/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.995904 pyikarus-0.3.0.dev202310000083/Testing/Temporary/
+-rw-r--r--   0 user      (1001) user      (1001)        4 2023-05-15 11:55:16.000000 pyikarus-0.3.0.dev202310000083/Testing/Temporary/CTestCostData.txt
+-rw-r--r--   0 user      (1001) user      (1001)      121 2023-05-15 11:55:16.000000 pyikarus-0.3.0.dev202310000083/Testing/Temporary/LastTest.log
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.995904 pyikarus-0.3.0.dev202310000083/cmake/
+-rw-r--r--   0 user      (1001) user      (1001)      973 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/cmake/CPM.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.995904 pyikarus-0.3.0.dev202310000083/cmake/FormatTarget/
+-rw-r--r--   0 user      (1001) user      (1001)     1270 2023-03-10 08:15:25.000000 pyikarus-0.3.0.dev202310000083/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.995904 pyikarus-0.3.0.dev202310000083/cmake/modules/
+-rw-r--r--   0 user      (1001) user      (1001)      715 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      683 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      740 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      691 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      226 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)      446 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 user      (1001) user      (1001)     2040 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/cmake/tools.cmake
+-rw-r--r--   0 user      (1001) user      (1001)      148 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/codecov.yml
+-rw-r--r--   0 user      (1001) user      (1001)      121 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/codespellignore
+-rw-r--r--   0 user      (1001) user      (1001)     1588 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/config.h.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.999904 pyikarus-0.3.0.dev202310000083/docs/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.999904 pyikarus-0.3.0.dev202310000083/docs/BuildLocally/
+-rw-r--r--   0 user      (1001) user      (1001)      439 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)      333 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.999904 pyikarus-0.3.0.dev202310000083/docs/__pycache__/
+-rw-r--r--   0 user      (1001) user      (1001)     1136 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 user      (1001) user      (1001)     6961 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/literature.bib
+-rw-r--r--   0 user      (1001) user      (1001)      117 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/literature.bib.license
+-rw-r--r--   0 user      (1001) user      (1001)     1245 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/mkdocs-macros.py
+-rw-r--r--   0 user      (1001) user      (1001)      394 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/mkdocs.insiders.yml
+-rw-r--r--   0 user      (1001) user      (1001)     5042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/docs/mkdocs.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.983904 pyikarus-0.3.0.dev202310000083/docs/overrides/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.999904 pyikarus-0.3.0.dev202310000083/docs/overrides/partials/
+-rw-r--r--   0 user      (1001) user      (1001)     1732 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/overrides/partials/comments.html
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:24.999904 pyikarus-0.3.0.dev202310000083/docs/website/
+-rw-r--r--   0 user      (1001) user      (1001)       24 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/.meta.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.003904 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/
+-rw-r--r--   0 user      (1001) user      (1001)     4710 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/assembler.md
+-rw-r--r--   0 user      (1001) user      (1001)     6387 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 user      (1001) user      (1001)     2024 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 user      (1001) user      (1001)     3237 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 user      (1001) user      (1001)     8524 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 user      (1001) user      (1001)     2745 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/grids.md
+-rw-r--r--   0 user      (1001) user      (1001)     4121 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/index.md
+-rw-r--r--   0 user      (1001) user      (1001)     4932 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 user      (1001) user      (1001)    44213 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 user      (1001) user      (1001)     3978 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 user      (1001) user      (1001)     2590 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 user      (1001) user      (1001)     3086 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/observer.md
+-rw-r--r--   0 user      (1001) user      (1001)     5211 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.007904 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/
+-rw-r--r--   0 user      (1001) user      (1001)     6655 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 user      (1001) user      (1001)     7251 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/computePi.md
+-rw-r--r--   0 user      (1001) user      (1001)     5439 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 user      (1001) user      (1001)     7055 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 user      (1001) user      (1001)     2164 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/index.md
+-rw-r--r--   0 user      (1001) user      (1001)     7702 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 user      (1001) user      (1001)     5114 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 user      (1001) user      (1001)     6200 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 user      (1001) user      (1001)     4071 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.007904 pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/
+-rw-r--r--   0 user      (1001) user      (1001)     2439 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 user      (1001) user      (1001)     1002 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 user      (1001) user      (1001)     2415 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 user      (1001) user      (1001)     1762 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.011904 pyikarus-0.3.0.dev202310000083/docs/website/04_blog/
+-rw-r--r--   0 user      (1001) user      (1001)      274 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 user      (1001) user      (1001)        7 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/04_blog/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.011904 pyikarus-0.3.0.dev202310000083/docs/website/04_blog/posts/
+-rw-r--r--   0 user      (1001) user      (1001)     7731 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.011904 pyikarus-0.3.0.dev202310000083/docs/website/05_cppReferences/
+-rw-r--r--   0 user      (1001) user      (1001)     2324 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.011904 pyikarus-0.3.0.dev202310000083/docs/website/99_Literature/
+-rw-r--r--   0 user      (1001) user      (1001)      169 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.011904 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.015904 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 user      (1001) user      (1001)    52795 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    46250 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 user      (1001) user      (1001)     2852 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    17924 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 user      (1001) user      (1001)     9455 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.015904 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 user      (1001) user      (1001)    35234 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    62184 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 user      (1001) user      (1001)     2281 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    40033 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 user      (1001) user      (1001)    25505 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 user      (1001) user      (1001)     8101 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/logo_blue.svg
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/logo_blue.svg.license
+-rw-r--r--   0 user      (1001) user      (1001)     8255 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/logo_white.svg
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/logo_white.svg.license
+-rw-r--r--   0 user      (1001) user      (1001)     4364 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000083/docs/website/download.md
+-rw-r--r--   0 user      (1001) user      (1001)      244 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/gallery.md
+-rw-r--r--   0 user      (1001) user      (1001)     1358 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.019904 pyikarus-0.3.0.dev202310000083/docs/website/javascripts/
+-rw-r--r--   0 user      (1001) user      (1001)      486 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.019904 pyikarus-0.3.0.dev202310000083/docs/website/stylesheets/
+-rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/docs/website/stylesheets/extra.css
+-rw-r--r--   0 user      (1001) user      (1001)      502 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/dune.module
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.019904 pyikarus-0.3.0.dev202310000083/ikarus/
+-rw-r--r--   0 user      (1001) user      (1001)      748 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/ikarus/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.019904 pyikarus-0.3.0.dev202310000083/ikarus/assembler/
+-rw-r--r--   0 user      (1001) user      (1001)      268 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)    11069 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 user      (1001) user      (1001)    10714 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.019904 pyikarus-0.3.0.dev202310000083/ikarus/controlRoutines/
+-rw-r--r--   0 user      (1001) user      (1001)      239 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     2575 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2970 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.019904 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/
+-rw-r--r--   0 user      (1001) user      (1001)      349 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)      185 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.023904 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feBases/
+-rw-r--r--   0 user      (1001) user      (1001)      282 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     2925 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2305 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1827 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1041 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feRequirements.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     8419 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1338 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.023904 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 user      (1001) user      (1001)      345 2023-05-12 10:40:33.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)    19628 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 user      (1001) user      (1001)    12549 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.027904 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 user      (1001) user      (1001)      397 2023-03-23 09:50:04.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5699 2023-05-08 12:58:29.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2718 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 user      (1001) user      (1001)     4635 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 user      (1001) user      (1001)     3809 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 user      (1001) user      (1001)     5734 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 user      (1001) user      (1001)      473 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 user      (1001) user      (1001)     8010 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1196 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 user      (1001) user      (1001)     7827 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 user      (1001) user      (1001)    12655 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.027904 pyikarus-0.3.0.dev202310000083/ikarus/linearAlgebra/
+-rw-r--r--   0 user      (1001) user      (1001)      301 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     6734 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 user      (1001) user      (1001)     7791 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 user      (1001) user      (1001)    12303 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.027904 pyikarus-0.3.0.dev202310000083/ikarus/python/
+-rw-r--r--   0 user      (1001) user      (1001)      294 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.031904 pyikarus-0.3.0.dev202310000083/ikarus/python/assembler/
+-rw-r--r--   0 user      (1001) user      (1001)      249 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3149 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.031904 pyikarus-0.3.0.dev202310000083/ikarus/python/basis/
+-rw-r--r--   0 user      (1001) user      (1001)      237 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     4559 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.031904 pyikarus-0.3.0.dev202310000083/ikarus/python/dirichletValues/
+-rw-r--r--   0 user      (1001) user      (1001)      257 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     4116 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.031904 pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/
+-rw-r--r--   0 user      (1001) user      (1001)      303 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5036 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.031904 pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 user      (1001) user      (1001)      259 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5107 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 user      (1001) user      (1001)     5503 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.035904 pyikarus-0.3.0.dev202310000083/ikarus/python/test/
+-rw-r--r--   0 user      (1001) user      (1001)      564 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     4062 2023-05-17 08:21:12.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 user      (1001) user      (1001)  2704357 2023-05-15 11:50:45.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/test/nameTest.vtu
+-rw-r--r--   0 user      (1001) user      (1001)     4447 2023-05-15 09:03:11.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 user      (1001) user      (1001)      862 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.035904 pyikarus-0.3.0.dev202310000083/ikarus/python/utils/
+-rw-r--r--   0 user      (1001) user      (1001)      245 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1181 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000083/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.035904 pyikarus-0.3.0.dev202310000083/ikarus/solver/
+-rw-r--r--   0 user      (1001) user      (1001)      211 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.035904 pyikarus-0.3.0.dev202310000083/ikarus/solver/linearSolver/
+-rw-r--r--   0 user      (1001) user      (1001)      244 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     8891 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.039904 pyikarus-0.3.0.dev202310000083/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 user      (1001) user      (1001)      272 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     5407 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 user      (1001) user      (1001)     8297 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 user      (1001) user      (1001)    18574 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.043904 pyikarus-0.3.0.dev202310000083/ikarus/utils/
+-rw-r--r--   0 user      (1001) user      (1001)      712 2023-04-04 06:38:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1741 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/algorithms.hh
+-rw-r--r--   0 user      (1001) user      (1001)      878 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1445 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/basis.hh
+-rw-r--r--   0 user      (1001) user      (1001)     6930 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/concepts.hh
+-rw-r--r--   0 user      (1001) user      (1001)      503 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.047904 pyikarus-0.3.0.dev202310000083/ikarus/utils/drawing/
+-rw-r--r--   0 user      (1001) user      (1001)      262 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1654 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 user      (1001) user      (1001)      544 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      703 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2484 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2347 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 user      (1001) user      (1001)      682 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1367 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      724 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 user      (1001) user      (1001)     3611 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2171 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     6359 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 user      (1001) user      (1001)     3152 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/init.hh
+-rw-r--r--   0 user      (1001) user      (1001)    15244 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1711 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.047904 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/
+-rw-r--r--   0 user      (1001) user      (1001)      450 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1554 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2307 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 user      (1001) user      (1001)      905 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1053 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1132 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1985 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 user      (1001) user      (1001)     5497 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 user      (1001) user      (1001)      489 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 user      (1001) user      (1001)     4159 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1131 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      570 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/polyfit.hh
+-rw-r--r--   0 user      (1001) user      (1001)    10054 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 user      (1001) user      (1001)    15044 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/ikarus/utils/traits.hh
+-rw-r--r--   0 user      (1001) user      (1001)      432 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/ikarus.pc.in
+-rw-r--r--   0 user      (1001) user      (1001)      196 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/iwyu.imp
+-rw-r--r--   0 user      (1001) user      (1001)      422 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000083/pyproject.toml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.047904 pyikarus-0.3.0.dev202310000083/python/
+-rw-r--r--   0 user      (1001) user      (1001)      586 2023-05-17 07:43:44.000000 pyikarus-0.3.0.dev202310000083/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.051904 pyikarus-0.3.0.dev202310000083/python/ikarus/
+-rw-r--r--   0 user      (1001) user      (1001)      517 2023-05-15 08:59:18.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)      603 2023-05-17 12:14:01.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     5636 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.051904 pyikarus-0.3.0.dev202310000083/python/ikarus/assembler/
+-rw-r--r--   0 user      (1001) user      (1001)      167 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     2300 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     1491 2023-05-15 08:55:23.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/basis.py
+-rw-r--r--   0 user      (1001) user      (1001)     1408 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.051904 pyikarus-0.3.0.dev202310000083/python/ikarus/finite_elements/
+-rw-r--r--   0 user      (1001) user      (1001)      173 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/finite_elements/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3465 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/finite_elements/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)     1792 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/materials.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.051904 pyikarus-0.3.0.dev202310000083/python/ikarus/utils/
+-rw-r--r--   0 user      (1001) user      (1001)      163 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     1496 2023-05-15 08:30:08.000000 pyikarus-0.3.0.dev202310000083/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.051904 pyikarus-0.3.0.dev202310000083/python/pyikarus.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-17 12:28:24.000000 pyikarus-0.3.0.dev202310000083/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)     9951 2023-05-17 12:28:24.000000 pyikarus-0.3.0.dev202310000083/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-17 12:28:24.000000 pyikarus-0.3.0.dev202310000083/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-17 12:28:24.000000 pyikarus-0.3.0.dev202310000083/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) user      (1001)        7 2023-05-17 12:28:24.000000 pyikarus-0.3.0.dev202310000083/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 user      (1001) user      (1001)      632 2023-05-17 12:19:53.000000 pyikarus-0.3.0.dev202310000083/python/setup.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.051904 pyikarus-0.3.0.dev202310000083/sandbox/
+-rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/sandbox/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.051904 pyikarus-0.3.0.dev202310000083/sandbox/src/
+-rw-r--r--   0 user      (1001) user      (1001)     1220 2023-03-23 09:49:49.000000 pyikarus-0.3.0.dev202310000083/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.051904 pyikarus-0.3.0.dev202310000083/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 user      (1001) user      (1001)   674469 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 user      (1001) user      (1001)      320 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/sandbox/src/sandbox.cpp
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-17 12:28:25.063904 pyikarus-0.3.0.dev202310000083/setup.cfg
+-rw-r--r--   0 user      (1001) user      (1001)     1894 2023-05-17 12:28:04.000000 pyikarus-0.3.0.dev202310000083/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.055904 pyikarus-0.3.0.dev202310000083/tests/
+-rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/tests/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.059904 pyikarus-0.3.0.dev202310000083/tests/src/
+-rw-r--r--   0 user      (1001) user      (1001)     1418 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/CMakeLists.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3906 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000083/tests/src/assemblerTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     9913 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/common.hh
+-rw-r--r--   0 user      (1001) user      (1001)     2639 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/dependenciesTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     6520 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/dirichletValueTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     3820 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/easTest.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1473 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/enhancedAssumedStrainsTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      608 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/factories.hh
+-rw-r--r--   0 user      (1001) user      (1001)     1870 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/functionTraitsTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     2661 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/linearElasticityTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     2378 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/manifoldsTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     7961 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/materialTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     6770 2023-05-12 13:45:55.000000 pyikarus-0.3.0.dev202310000083/tests/src/nonLinearElasticityTest.hh
+-rw-r--r--   0 user      (1001) user      (1001)      724 2023-05-08 13:07:10.000000 pyikarus-0.3.0.dev202310000083/tests/src/nonLinearElasticityTestNeoHooke.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      729 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/nonLinearElasticityTestSVK.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     9936 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/nonLinearOperatorTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     6327 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/pathFollowingTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     1651 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/polyFitTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)      695 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/pythonConversionTest.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     1292 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 user      (1001) user      (1001)     5805 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/testFEElement.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 12:28:25.063904 pyikarus-0.3.0.dev202310000083/tests/src/testFiles/
+-rw-r--r--   0 user      (1001) user      (1001)     9028 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 user      (1001) user      (1001)      395 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 user      (1001) user      (1001)      497 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 user      (1001) user      (1001)      546 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 user      (1001) user      (1001)    11431 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000083/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 user      (1001) user      (1001)     1114 2023-03-24 20:46:25.000000 pyikarus-0.3.0.dev202310000083/tests/src/testHelpers.hh
+-rw-r--r--   0 user      (1001) user      (1001)    17595 2023-05-12 10:40:34.000000 pyikarus-0.3.0.dev202310000083/tests/src/trustRegionTest.cpp
```

### Comparing `pyikarus-0.3.0.dev202310000082/.clang-format` & `pyikarus-0.3.0.dev202310000083/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.cmake-format` & `pyikarus-0.3.0.dev202310000083/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.0.dev202310000083/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.0.dev202310000083/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.github/workflows/createRelease.yml` & `pyikarus-0.3.0.dev202310000083/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.0.dev202310000083/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.github/workflows/debian.yml` & `pyikarus-0.3.0.dev202310000083/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.github/workflows/ghpages.yml` & `pyikarus-0.3.0.dev202310000083/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.github/workflows/runExamples.yml` & `pyikarus-0.3.0.dev202310000083/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.github/workflows/style.yml` & `pyikarus-0.3.0.dev202310000083/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/.reuse/dep5` & `pyikarus-0.3.0.dev202310000083/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/CHANGELOG.md` & `pyikarus-0.3.0.dev202310000083/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/CODE_OF_CONDUCT.md` & `pyikarus-0.3.0.dev202310000083/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/LICENSE.md` & `pyikarus-0.3.0.dev202310000083/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.0.dev202310000083/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.0.dev202310000083/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.0.dev202310000083/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/LICENSES/MIT.txt` & `pyikarus-0.3.0.dev202310000083/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.0.dev202310000083/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/PKG-INFO` & `pyikarus-0.3.0.dev202310000083/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000082
+Version: 0.3.0.dev202310000083
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000082 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000083 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000082/README.md` & `pyikarus-0.3.0.dev202310000083/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/cmake/CPM.cmake` & `pyikarus-0.3.0.dev202310000083/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.0.dev202310000083/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.0.dev202310000083/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.0.dev202310000083/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.0.dev202310000083/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/cmake/tools.cmake` & `pyikarus-0.3.0.dev202310000083/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/config.h.cmake` & `pyikarus-0.3.0.dev202310000083/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.0.dev202310000083/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/literature.bib` & `pyikarus-0.3.0.dev202310000083/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/mkdocs-macros.py` & `pyikarus-0.3.0.dev202310000083/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/mkdocs.yml` & `pyikarus-0.3.0.dev202310000083/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/overrides/partials/comments.html` & `pyikarus-0.3.0.dev202310000083/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/assembler.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/grids.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/index.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/observer.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/01_framework/solvers.md` & `pyikarus-0.3.0.dev202310000083/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/computePi.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/index.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.0.dev202310000083/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.0.dev202310000083/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.0.dev202310000083/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.0.dev202310000083/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.0.dev202310000083/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/download.md` & `pyikarus-0.3.0.dev202310000083/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/docs/website/index.md` & `pyikarus-0.3.0.dev202310000083/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.0.dev202310000083/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feRequirements.cpp` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feRequirements.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/basis/basis.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/test/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/ikarus/python/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.0.dev202310000083/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/test/nameTest.vtu` & `pyikarus-0.3.0.dev202310000083/ikarus/python/test/nameTest.vtu`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.0.dev202310000083/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.0.dev202310000083/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/algorithms.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/basis.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/concepts.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/init.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/polyfit.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/ikarus/utils/traits.hh` & `pyikarus-0.3.0.dev202310000083/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/python/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/__init__.py` & `pyikarus-0.3.0.dev202310000083/python/ikarus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     from dune.packagemetadata import registerExternalModule
     import pathlib
 
     # register ikarus to be recognized by dune-py (code generation module)
     # as a module of the dune universe
     registerExternalModule(
-        moduleName="pyikarus",
+        moduleName="ikarus",
         modulePath=str(pathlib.Path(__file__).parent.resolve()),
     )
 
 except ImportError:
     pass
 
 from ._ikarus import *
```

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/_ikarus.cc` & `pyikarus-0.3.0.dev202310000083/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.0.dev202310000083/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/basis.py` & `pyikarus-0.3.0.dev202310000083/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/dirichletValues.py` & `pyikarus-0.3.0.dev202310000083/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.0.dev202310000083/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/materials.py` & `pyikarus-0.3.0.dev202310000083/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/ikarus/utils/__init__.py` & `pyikarus-0.3.0.dev202310000083/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.0.dev202310000083/python/pyikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000082
+Version: 0.3.0.dev202310000083
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000082 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000083 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000082/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.0.dev202310000083/python/pyikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/python/setup.py.in` & `pyikarus-0.3.0.dev202310000083/python/setup.py.in`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from setuptools import setup, find_packages
 REQUIRED_PACKAGES = '${RequiredPythonModules}'.replace(';',' ').split(' ')
 
 setup(
-    name="ikarus",
+    name="pyikarus",
     description="${ProjectDescription}",
     version="${ProjectVersionString}",
     author="${ProjectAuthor}",
     author_email="${ProjectMaintainerEmail}",
     packages=find_packages(exclude=["docs/*"]),
     zip_safe=0,
-    package_data={"": ["*.so"], "ikarus": ["data/*.cmake"]},
+    package_data={"": ["*.so"], "pyikarus": ["data/*.cmake"]},
     install_requires=REQUIRED_PACKAGES,
     include_package_data=True,
 )
```

### Comparing `pyikarus-0.3.0.dev202310000082/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.0.dev202310000083/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/setup.py` & `pyikarus-0.3.0.dev202310000083/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # You are logged in as $(whoami)
 # EOF
 # nano ~/.pypirc
 # python -m venv /dune/dune-common/build-cmake/dune-env/
 # source /dune/dune-common/build-cmake/dune-env/bin/activate
 # pip install ikarus  --no-build-isolation
 
-ikarusVersion = "0.3.0.dev202310000082" #+ datetime.today().time().strftime("%H%M%S")
+ikarusVersion = "0.3.0.dev202310000083" #+ datetime.today().time().strftime("%H%M%S")
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor sicne ikarus pypi package already exists
 print(metadata)
```

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000083/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/assemblerTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/assemblerTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/common.hh` & `pyikarus-0.3.0.dev202310000083/tests/src/common.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/dependenciesTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/dependenciesTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/dirichletValueTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/dirichletValueTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/easTest.hh` & `pyikarus-0.3.0.dev202310000083/tests/src/easTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/enhancedAssumedStrainsTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/enhancedAssumedStrainsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/factories.hh` & `pyikarus-0.3.0.dev202310000083/tests/src/factories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/functionTraitsTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/functionTraitsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/linearElasticityTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/linearElasticityTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/manifoldsTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/manifoldsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/materialTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/materialTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/nonLinearElasticityTest.hh` & `pyikarus-0.3.0.dev202310000083/tests/src/nonLinearElasticityTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/nonLinearElasticityTestNeoHooke.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/nonLinearElasticityTestNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/nonLinearElasticityTestSVK.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/nonLinearElasticityTestSVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/nonLinearOperatorTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/nonLinearOperatorTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/pathFollowingTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/pathFollowingTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/polyFitTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/polyFitTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/pythonConversionTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/pythonConversionTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/testFEElement.hh` & `pyikarus-0.3.0.dev202310000083/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.0.dev202310000083/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.0.dev202310000083/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.0.dev202310000083/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/testHelpers.hh` & `pyikarus-0.3.0.dev202310000083/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000082/tests/src/trustRegionTest.cpp` & `pyikarus-0.3.0.dev202310000083/tests/src/trustRegionTest.cpp`

 * *Files identical despite different names*

