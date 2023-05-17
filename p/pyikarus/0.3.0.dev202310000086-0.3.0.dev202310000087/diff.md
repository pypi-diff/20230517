# Comparing `tmp/pyikarus-0.3.0.dev202310000086.tar.gz` & `tmp/pyikarus-0.3.0.dev202310000087.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.0.dev202310000086.tar", last modified: Wed May 17 21:04:27 2023, max compression
+gzip compressed data, was "pyikarus-0.3.0.dev202310000087.tar", last modified: Wed May 17 21:05:49 2023, max compression
```

## Comparing `pyikarus-0.3.0.dev202310000086.tar` & `pyikarus-0.3.0.dev202310000087.tar`

### file list

```diff
@@ -1,329 +1,330 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:27.209421 pyikarus-0.3.0.dev202310000086/
--rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.bettercodehub.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1300 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.clang-format
--rwxrwxrwx   0 user      (1001) user      (1001)     1017 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.cmake-format
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:22.544330 pyikarus-0.3.0.dev202310000086/.github/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:22.937150 pyikarus-0.3.0.dev202310000086/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 user      (1001) user      (1001)      615 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.077559 pyikarus-0.3.0.dev202310000086/.github/workflows/
--rwxrwxrwx   0 user      (1001) user      (1001)      476 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/codespell.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1034 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/createDockerContainer.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     4900 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/createRelease.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1635 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/debian-coverage.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2414 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/debian.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/ghpages.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/reuseLint.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2854 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/runExamples.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1212 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.github/workflows/style.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      455 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/.gitignore
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.090628 pyikarus-0.3.0.dev202310000086/.reuse/
--rwxrwxrwx   0 user      (1001) user      (1001)      661 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/.reuse/dep5
--rwxrwxrwx   0 user      (1001) user      (1001)     3324 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/CHANGELOG.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1342 2023-05-17 21:01:23.000000 pyikarus-0.3.0.dev202310000086/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5335 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/LICENSE.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.165334 pyikarus-0.3.0.dev202310000086/LICENSES/
--rwxrwxrwx   0 user      (1001) user      (1001)    18375 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/LICENSES/CC-BY-SA-4.0.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     7048 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/LICENSES/CC0-1.0.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    42098 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/LICENSES/LGPL-3.0-or-later.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1078 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/LICENSES/MIT.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    16727 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/LICENSES/MPL-2.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-17 21:04:27.207370 pyikarus-0.3.0.dev202310000086/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/README.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:22.554227 pyikarus-0.3.0.dev202310000086/Testing/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.198986 pyikarus-0.3.0.dev202310000086/Testing/Temporary/
--rwxrwxrwx   0 user      (1001) user      (1001)        4 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/Testing/Temporary/CTestCostData.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/Testing/Temporary/LastTest.log
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.231397 pyikarus-0.3.0.dev202310000086/cmake/
--rwxrwxrwx   0 user      (1001) user      (1001)      973 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/cmake/CPM.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.250990 pyikarus-0.3.0.dev202310000086/cmake/FormatTarget/
--rwxrwxrwx   0 user      (1001) user      (1001)     1270 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.354567 pyikarus-0.3.0.dev202310000086/cmake/modules/
--rwxrwxrwx   0 user      (1001) user      (1001)      715 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/cmake/modules/AddAutoDiffFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      683 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/cmake/modules/AddEigenFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      740 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/cmake/modules/AddMatplotppFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      691 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/cmake/modules/AddSpdlogFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-17 20:06:12.000000 pyikarus-0.3.0.dev202310000086/cmake/modules/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      379 2023-05-17 20:12:55.000000 pyikarus-0.3.0.dev202310000086/cmake/modules/IkarusMacros.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)     2040 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/cmake/tools.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      148 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/codecov.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/codespellignore
--rwxrwxrwx   0 user      (1001) user      (1001)     1588 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/config.h.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.434515 pyikarus-0.3.0.dev202310000086/docs/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.448446 pyikarus-0.3.0.dev202310000086/docs/BuildLocally/
--rwxrwxrwx   0 user      (1001) user      (1001)      439 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/BuildLocally/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      333 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.478065 pyikarus-0.3.0.dev202310000086/docs/__pycache__/
--rwxrwxrwx   0 user      (1001) user      (1001)     1136 2023-04-21 10:05:27.000000 pyikarus-0.3.0.dev202310000086/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rwxrwxrwx   0 user      (1001) user      (1001)     6961 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/literature.bib
--rwxrwxrwx   0 user      (1001) user      (1001)      117 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/literature.bib.license
--rwxrwxrwx   0 user      (1001) user      (1001)     1245 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/mkdocs-macros.py
--rwxrwxrwx   0 user      (1001) user      (1001)      394 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/mkdocs.insiders.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     5042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/mkdocs.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:22.578361 pyikarus-0.3.0.dev202310000086/docs/overrides/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.498276 pyikarus-0.3.0.dev202310000086/docs/overrides/partials/
--rwxrwxrwx   0 user      (1001) user      (1001)     1732 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/overrides/partials/comments.html
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.576021 pyikarus-0.3.0.dev202310000086/docs/website/
--rwxrwxrwx   0 user      (1001) user      (1001)       24 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/.meta.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:23.829332 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/
--rwxrwxrwx   0 user      (1001) user      (1001)     4710 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/assembler.md
--rwxrwxrwx   0 user      (1001) user      (1001)     6387 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/controlRoutines.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2024 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/dirichletBCs.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3237 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/feRequirements.md
--rwxrwxrwx   0 user      (1001) user      (1001)     8524 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/finiteElements.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2745 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/grids.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/index.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4932 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/localBasis.md
--rwxrwxrwx   0 user      (1001) user      (1001)    44213 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/localFunctions.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3978 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/manifolds.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2590 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/nonlinearOperator.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3086 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/observer.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5211 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.001261 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/
--rwxrwxrwx   0 user      (1001) user      (1001)     6655 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/cantileverBeam.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7251 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/computePi.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5439 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/cooksMembrane.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7055 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/incompressibleRubberBlock.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2164 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/index.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7702 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/kirchhoffPlate.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5114 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/newtonRaphsonMethod.md
--rwxrwxrwx   0 user      (1001) user      (1001)     6200 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/nonLinearElasticity.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4071 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.084448 pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/
--rwxrwxrwx   0 user      (1001) user      (1001)     2439 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/buildDocumentationLocally.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1002 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/codeStyle.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2415 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/howToEdit.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1762 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.121994 pyikarus-0.3.0.dev202310000086/docs/website/04_blog/
--rwxrwxrwx   0 user      (1001) user      (1001)      274 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/04_blog/.authors.yml
--rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/04_blog/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.144503 pyikarus-0.3.0.dev202310000086/docs/website/04_blog/posts/
--rwxrwxrwx   0 user      (1001) user      (1001)     7731 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.166981 pyikarus-0.3.0.dev202310000086/docs/website/05_cppReferences/
--rwxrwxrwx   0 user      (1001) user      (1001)     2324 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.189184 pyikarus-0.3.0.dev202310000086/docs/website/99_Literature/
--rwxrwxrwx   0 user      (1001) user      (1001)      169 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.266822 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.492378 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/
--rwxrwxrwx   0 user      (1001) user      (1001)    52795 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    46250 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     2852 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    17924 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     9455 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.714007 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/
--rwxrwxrwx   0 user      (1001) user      (1001)    35234 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    62184 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     2281 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    40033 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    25505 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     8101 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/logo_blue.svg
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/logo_blue.svg.license
--rwxrwxrwx   0 user      (1001) user      (1001)     8255 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/logo_white.svg
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/logo_white.svg.license
--rwxrwxrwx   0 user      (1001) user      (1001)     4364 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/download.md
--rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/gallery.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1358 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.735322 pyikarus-0.3.0.dev202310000086/docs/website/javascripts/
--rwxrwxrwx   0 user      (1001) user      (1001)      486 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.753814 pyikarus-0.3.0.dev202310000086/docs/website/stylesheets/
--rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/docs/website/stylesheets/extra.css
--rwxrwxrwx   0 user      (1001) user      (1001)      502 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/dune.module
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.768247 pyikarus-0.3.0.dev202310000086/ikarus/
--rwxrwxrwx   0 user      (1001) user      (1001)      748 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.812967 pyikarus-0.3.0.dev202310000086/ikarus/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      268 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    11069 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/assembler/simpleAssemblers.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    10714 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.858269 pyikarus-0.3.0.dev202310000086/ikarus/controlRoutines/
--rwxrwxrwx   0 user      (1001) user      (1001)      239 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/controlRoutines/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2575 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/controlRoutines/loadControl.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2970 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:24.944177 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/
--rwxrwxrwx   0 user      (1001) user      (1001)      349 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      185 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.014259 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feBases/
--rwxrwxrwx   0 user      (1001) user      (1001)      282 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feBases/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2925 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feBases/autodiffFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2305 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feBases/powerBasisFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1827 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feBases/scalarFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1041 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feRequirements.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     8419 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feRequirements.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1338 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.106402 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/
--rwxrwxrwx   0 user      (1001) user      (1001)      345 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    19628 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12549 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.289811 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/
--rwxrwxrwx   0 user      (1001) user      (1001)      397 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5699 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/interface.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2718 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     4635 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     3809 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5734 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/svk.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      473 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/tags.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     8010 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1196 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     7827 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12655 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.352537 pyikarus-0.3.0.dev202310000086/ikarus/linearAlgebra/
--rwxrwxrwx   0 user      (1001) user      (1001)      301 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/linearAlgebra/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     6734 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/linearAlgebra/dirichletValues.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     7791 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/linearAlgebra/nonLinearOperator.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12303 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.367097 pyikarus-0.3.0.dev202310000086/ikarus/python/
--rwxrwxrwx   0 user      (1001) user      (1001)      294 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.400153 pyikarus-0.3.0.dev202310000086/ikarus/python/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      249 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3149 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.436045 pyikarus-0.3.0.dev202310000086/ikarus/python/basis/
--rwxrwxrwx   0 user      (1001) user      (1001)      237 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/basis/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     4559 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.472350 pyikarus-0.3.0.dev202310000086/ikarus/python/dirichletValues/
--rwxrwxrwx   0 user      (1001) user      (1001)      257 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/dirichletValues/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     4116 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.524477 pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/
--rwxrwxrwx   0 user      (1001) user      (1001)      303 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5036 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.566985 pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/materials/
--rwxrwxrwx   0 user      (1001) user      (1001)      259 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/materials/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5107 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/materials/material.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5503 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.685347 pyikarus-0.3.0.dev202310000086/ikarus/python/test/
--rwxrwxrwx   0 user      (1001) user      (1001)      564 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/test/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     4062 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/test/linearElasticTest.py
--rwxrwxrwx   0 user      (1001) user      (1001)  2704357 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/test/nameTest.vtu
--rwxrwxrwx   0 user      (1001) user      (1001)     4447 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/test/nonLinearElasticTest.py
--rwxrwxrwx   0 user      (1001) user      (1001)      862 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.720301 pyikarus-0.3.0.dev202310000086/ikarus/python/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      245 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1181 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.735896 pyikarus-0.3.0.dev202310000086/ikarus/solver/
--rwxrwxrwx   0 user      (1001) user      (1001)      211 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.774152 pyikarus-0.3.0.dev202310000086/ikarus/solver/linearSolver/
--rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/solver/linearSolver/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     8891 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:25.844765 pyikarus-0.3.0.dev202310000086/ikarus/solver/nonLinearSolver/
--rwxrwxrwx   0 user      (1001) user      (1001)      272 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5407 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     8297 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    18574 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.165313 pyikarus-0.3.0.dev202310000086/ikarus/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      712 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1741 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/algorithms.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      878 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/autodiffHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1445 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/basis.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     6930 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/concepts.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      503 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.237791 pyikarus-0.3.0.dev202310000086/ikarus/utils/drawing/
--rwxrwxrwx   0 user      (1001) user      (1001)      262 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/drawing/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1654 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/drawing/griddrawer.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      544 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/drawing/matplotHelper.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      703 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/drawing/matplotHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2484 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/duneUtilities.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2347 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/eigenDuneTransformations.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      682 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/eigenSparseAddon.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1367 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/findLineSegment.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/findLineSegment.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     3611 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/flatPreBasis.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2171 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/functionSanityChecks.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6359 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/functionSanityChecks.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     3152 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/init.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    15244 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/linearAlgebraHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1711 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.400941 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/
--rwxrwxrwx   0 user      (1001) user      (1001)      450 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1554 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/controlLogger.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2307 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/controlVTKWriter.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      905 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/genericControlObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1053 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/gridDrawerObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1132 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/loadControlObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1985 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/nonLinearSolverLogger.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5497 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/observer.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      489 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/observerMessages.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     4159 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/pathFollowingFunctions.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1131 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/polyfit.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      570 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/polyfit.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    10054 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/tensorUtils.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    15044 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus/utils/traits.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      432 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/ikarus.pc.in
--rwxrwxrwx   0 user      (1001) user      (1001)      196 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/iwyu.imp
--rwxrwxrwx   0 user      (1001) user      (1001)    47361 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/logfile
--rwxrwxrwx   0 user      (1001) user      (1001)      422 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.425250 pyikarus-0.3.0.dev202310000086/python/
--rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-17 19:26:46.000000 pyikarus-0.3.0.dev202310000086/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.513500 pyikarus-0.3.0.dev202310000086/python/ikarus/
--rwxrwxrwx   0 user      (1001) user      (1001)      517 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      603 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     5636 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.545696 pyikarus-0.3.0.dev202310000086/python/ikarus/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      167 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2300 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/assembler/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1491 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/basis.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1408 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.582100 pyikarus-0.3.0.dev202310000086/python/ikarus/finite_elements/
--rwxrwxrwx   0 user      (1001) user      (1001)      173 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/finite_elements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3465 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/finite_elements/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1792 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/materials.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.617509 pyikarus-0.3.0.dev202310000086/python/ikarus/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      163 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1496 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.691330 pyikarus-0.3.0.dev202310000086/python/pyikarus.egg-info/
--rwxrwxrwx   0 user      (1001) user      (1001)     3638 2023-05-17 21:04:20.000000 pyikarus-0.3.0.dev202310000086/python/pyikarus.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     9959 2023-05-17 21:04:22.000000 pyikarus-0.3.0.dev202310000086/python/pyikarus.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1001) user      (1001)        1 2023-05-17 21:04:20.000000 pyikarus-0.3.0.dev202310000086/python/pyikarus.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 21:04:20.000000 pyikarus-0.3.0.dev202310000086/python/pyikarus.egg-info/requires.txt
--rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-17 21:04:20.000000 pyikarus-0.3.0.dev202310000086/python/pyikarus.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      632 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/python/setup.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.703616 pyikarus-0.3.0.dev202310000086/sandbox/
--rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/sandbox/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.731588 pyikarus-0.3.0.dev202310000086/sandbox/src/
--rwxrwxrwx   0 user      (1001) user      (1001)     1220 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.748219 pyikarus-0.3.0.dev202310000086/sandbox/src/auxiliaryFiles/
--rwxrwxrwx   0 user      (1001) user      (1001)   674469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/sandbox/src/auxiliaryFiles/circle.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      320 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/sandbox/src/sandbox.cpp
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-17 21:04:27.209927 pyikarus-0.3.0.dev202310000086/setup.cfg
--rwxrwxrwx   0 user      (1001) user      (1001)     1308 2023-05-17 21:03:53.000000 pyikarus-0.3.0.dev202310000086/setup.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:26.770881 pyikarus-0.3.0.dev202310000086/tests/
--rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/tests/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:27.102999 pyikarus-0.3.0.dev202310000086/tests/src/
--rwxrwxrwx   0 user      (1001) user      (1001)     1418 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/tests/src/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3906 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/tests/src/assemblerTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     9913 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/tests/src/common.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2639 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/dependenciesTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6520 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/tests/src/dirichletValueTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     3820 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/easTest.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1473 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/enhancedAssumedStrainsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      608 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/tests/src/factories.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1870 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/tests/src/functionTraitsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     2661 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000086/tests/src/linearElasticityTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     2378 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/manifoldsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     7961 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/tests/src/materialTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6770 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/tests/src/nonLinearElasticityTest.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      729 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/tests/src/nonLinearElasticityTestSVK.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     9936 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/nonLinearOperatorTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6327 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/pathFollowingTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     1651 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/polyFitTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      695 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/pythonConversionTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     1292 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/testAutodiffHelper.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     5805 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000086/tests/src/testFEElement.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:04:27.190062 pyikarus-0.3.0.dev202310000086/tests/src/testFiles/
--rwxrwxrwx   0 user      (1001) user      (1001)     9028 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000086/tests/src/testFiles/unstructuredQuadscoarse.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      395 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000086/tests/src/testFiles/unstructuredTest.geo
--rwxrwxrwx   0 user      (1001) user      (1001)      497 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000086/tests/src/testFiles/unstructuredTest.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      546 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000086/tests/src/testFiles/unstructuredTest2.geo
--rwxrwxrwx   0 user      (1001) user      (1001)    11431 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000086/tests/src/testFiles/unstructuredTrianglesfine.msh
--rwxrwxrwx   0 user      (1001) user      (1001)     1114 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000086/tests/src/testHelpers.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    17595 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000086/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.496288 pyikarus-0.3.0.dev202310000087/
+-rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.bettercodehub.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1300 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.clang-format
+-rwxrwxrwx   0 user      (1001) user      (1001)     1017 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.cmake-format
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.045416 pyikarus-0.3.0.dev202310000087/.github/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.432115 pyikarus-0.3.0.dev202310000087/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      615 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.569080 pyikarus-0.3.0.dev202310000087/.github/workflows/
+-rwxrwxrwx   0 user      (1001) user      (1001)      476 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/codespell.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1034 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/createDockerContainer.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     4900 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/createRelease.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1635 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/debian-coverage.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2414 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/debian.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/ghpages.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/reuseLint.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2854 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/runExamples.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1212 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.github/workflows/style.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      455 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/.gitignore
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.580646 pyikarus-0.3.0.dev202310000087/.reuse/
+-rwxrwxrwx   0 user      (1001) user      (1001)      661 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/.reuse/dep5
+-rwxrwxrwx   0 user      (1001) user      (1001)     3324 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/CHANGELOG.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1342 2023-05-17 21:01:23.000000 pyikarus-0.3.0.dev202310000087/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5335 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSE.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.635819 pyikarus-0.3.0.dev202310000087/LICENSES/
+-rwxrwxrwx   0 user      (1001) user      (1001)    18375 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSES/CC-BY-SA-4.0.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     7048 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSES/CC0-1.0.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    42098 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSES/LGPL-3.0-or-later.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1078 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/LICENSES/MIT.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    16727 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-17 21:05:49.494606 pyikarus-0.3.0.dev202310000087/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/README.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.053761 pyikarus-0.3.0.dev202310000087/Testing/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.664654 pyikarus-0.3.0.dev202310000087/Testing/Temporary/
+-rwxrwxrwx   0 user      (1001) user      (1001)        4 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/Testing/Temporary/CTestCostData.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/Testing/Temporary/LastTest.log
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.698677 pyikarus-0.3.0.dev202310000087/cmake/
+-rwxrwxrwx   0 user      (1001) user      (1001)       57 2023-05-17 21:01:23.000000 pyikarus-0.3.0.dev202310000087/cmake/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      973 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/CPM.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.711591 pyikarus-0.3.0.dev202310000087/cmake/FormatTarget/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1270 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.799965 pyikarus-0.3.0.dev202310000087/cmake/modules/
+-rwxrwxrwx   0 user      (1001) user      (1001)      715 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/AddAutoDiffFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      683 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/AddEigenFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      740 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/AddMatplotppFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      691 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/AddSpdlogFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-17 20:06:12.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      379 2023-05-17 20:12:55.000000 pyikarus-0.3.0.dev202310000087/cmake/modules/IkarusMacros.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)     2040 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/cmake/tools.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      148 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/codecov.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/codespellignore
+-rwxrwxrwx   0 user      (1001) user      (1001)     1588 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/config.h.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.866838 pyikarus-0.3.0.dev202310000087/docs/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.879918 pyikarus-0.3.0.dev202310000087/docs/BuildLocally/
+-rwxrwxrwx   0 user      (1001) user      (1001)      439 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/BuildLocally/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      333 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.907987 pyikarus-0.3.0.dev202310000087/docs/__pycache__/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1136 2023-04-21 10:05:27.000000 pyikarus-0.3.0.dev202310000087/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     6961 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/literature.bib
+-rwxrwxrwx   0 user      (1001) user      (1001)      117 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/literature.bib.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     1245 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/mkdocs-macros.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      394 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/mkdocs.insiders.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     5042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/mkdocs.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.078989 pyikarus-0.3.0.dev202310000087/docs/overrides/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.924528 pyikarus-0.3.0.dev202310000087/docs/overrides/partials/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1732 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/overrides/partials/comments.html
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:45.982767 pyikarus-0.3.0.dev202310000087/docs/website/
+-rwxrwxrwx   0 user      (1001) user      (1001)       24 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/.meta.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.217162 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/
+-rwxrwxrwx   0 user      (1001) user      (1001)     4710 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/assembler.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     6387 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/controlRoutines.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2024 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/dirichletBCs.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3237 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/feRequirements.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     8524 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/finiteElements.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2745 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/grids.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/index.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4932 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/localBasis.md
+-rwxrwxrwx   0 user      (1001) user      (1001)    44213 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/localFunctions.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3978 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/manifolds.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2590 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/nonlinearOperator.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3086 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/observer.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5211 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.393545 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/
+-rwxrwxrwx   0 user      (1001) user      (1001)     6655 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/cantileverBeam.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7251 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/computePi.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5439 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/cooksMembrane.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7055 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/incompressibleRubberBlock.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2164 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/index.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7702 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/kirchhoffPlate.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5114 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/newtonRaphsonMethod.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     6200 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/nonLinearElasticity.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4071 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.464276 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2439 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/buildDocumentationLocally.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1002 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/codeStyle.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2415 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/howToEdit.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1762 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.499853 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/
+-rwxrwxrwx   0 user      (1001) user      (1001)      274 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/.authors.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.519013 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/posts/
+-rwxrwxrwx   0 user      (1001) user      (1001)     7731 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.537392 pyikarus-0.3.0.dev202310000087/docs/website/05_cppReferences/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2324 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.554643 pyikarus-0.3.0.dev202310000087/docs/website/99_Literature/
+-rwxrwxrwx   0 user      (1001) user      (1001)      169 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.626425 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:46.834012 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/
+-rwxrwxrwx   0 user      (1001) user      (1001)    52795 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    46250 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     2852 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    17924 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     9455 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.053197 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/
+-rwxrwxrwx   0 user      (1001) user      (1001)    35234 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    62184 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     2281 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    40033 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    25505 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     8101 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_blue.svg
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_blue.svg.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     8255 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_white.svg
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_white.svg.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     4364 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/download.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/gallery.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1358 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.072337 pyikarus-0.3.0.dev202310000087/docs/website/javascripts/
+-rwxrwxrwx   0 user      (1001) user      (1001)      486 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.089591 pyikarus-0.3.0.dev202310000087/docs/website/stylesheets/
+-rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/docs/website/stylesheets/extra.css
+-rwxrwxrwx   0 user      (1001) user      (1001)      502 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/dune.module
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.101231 pyikarus-0.3.0.dev202310000087/ikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      748 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.146088 pyikarus-0.3.0.dev202310000087/ikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      268 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    11069 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/assembler/simpleAssemblers.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    10714 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.189581 pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/
+-rwxrwxrwx   0 user      (1001) user      (1001)      239 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2575 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/loadControl.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2970 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.277381 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      349 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      185 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.348300 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/
+-rwxrwxrwx   0 user      (1001) user      (1001)      282 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2925 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/autodiffFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2305 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1827 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/scalarFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1041 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feRequirements.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     8419 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feRequirements.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1338 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.438110 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/
+-rwxrwxrwx   0 user      (1001) user      (1001)      345 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    19628 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12549 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.608826 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/
+-rwxrwxrwx   0 user      (1001) user      (1001)      397 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5699 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/interface.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2718 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     4635 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3809 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5734 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/svk.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      473 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/tags.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     8010 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1196 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     7827 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12655 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.667948 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/
+-rwxrwxrwx   0 user      (1001) user      (1001)      301 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     6734 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/dirichletValues.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     7791 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/nonLinearOperator.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12303 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.682564 pyikarus-0.3.0.dev202310000087/ikarus/python/
+-rwxrwxrwx   0 user      (1001) user      (1001)      294 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.716833 pyikarus-0.3.0.dev202310000087/ikarus/python/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      249 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3149 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.751965 pyikarus-0.3.0.dev202310000087/ikarus/python/basis/
+-rwxrwxrwx   0 user      (1001) user      (1001)      237 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/basis/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     4559 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.788310 pyikarus-0.3.0.dev202310000087/ikarus/python/dirichletValues/
+-rwxrwxrwx   0 user      (1001) user      (1001)      257 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/dirichletValues/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     4116 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.843687 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      303 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5036 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.884012 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/materials/
+-rwxrwxrwx   0 user      (1001) user      (1001)      259 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5107 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/materials/material.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5503 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:47.997674 pyikarus-0.3.0.dev202310000087/ikarus/python/test/
+-rwxrwxrwx   0 user      (1001) user      (1001)      564 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     4062 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/linearElasticTest.py
+-rwxrwxrwx   0 user      (1001) user      (1001)  2704357 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/nameTest.vtu
+-rwxrwxrwx   0 user      (1001) user      (1001)     4447 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/nonLinearElasticTest.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      862 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.034166 pyikarus-0.3.0.dev202310000087/ikarus/python/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      245 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1181 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.050627 pyikarus-0.3.0.dev202310000087/ikarus/solver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      211 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.084303 pyikarus-0.3.0.dev202310000087/ikarus/solver/linearSolver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/linearSolver/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     8891 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.155485 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      272 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5407 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     8297 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    18574 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.462496 pyikarus-0.3.0.dev202310000087/ikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      712 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1741 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/algorithms.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      878 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/autodiffHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1445 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/basis.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     6930 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/concepts.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      503 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.534118 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/
+-rwxrwxrwx   0 user      (1001) user      (1001)      262 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1654 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/griddrawer.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      544 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/matplotHelper.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      703 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/matplotHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2484 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/duneUtilities.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2347 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/eigenDuneTransformations.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      682 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/eigenSparseAddon.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1367 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/findLineSegment.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/findLineSegment.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3611 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/flatPreBasis.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2171 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/functionSanityChecks.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6359 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/functionSanityChecks.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3152 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/init.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    15244 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/linearAlgebraHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1711 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.693182 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/
+-rwxrwxrwx   0 user      (1001) user      (1001)      450 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1554 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/controlLogger.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2307 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/controlVTKWriter.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      905 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/genericControlObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1053 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/gridDrawerObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1132 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/loadControlObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1985 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5497 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/observer.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      489 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/observerMessages.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     4159 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/pathFollowingFunctions.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1131 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/polyfit.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      570 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/polyfit.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    10054 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/tensorUtils.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    15044 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus/utils/traits.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      432 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/ikarus.pc.in
+-rwxrwxrwx   0 user      (1001) user      (1001)      196 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/iwyu.imp
+-rwxrwxrwx   0 user      (1001) user      (1001)    47361 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/logfile
+-rwxrwxrwx   0 user      (1001) user      (1001)      422 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/pyproject.toml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.717821 pyikarus-0.3.0.dev202310000087/python/
+-rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-17 19:26:46.000000 pyikarus-0.3.0.dev202310000087/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.801017 pyikarus-0.3.0.dev202310000087/python/ikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      517 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      603 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     5636 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.834710 pyikarus-0.3.0.dev202310000087/python/ikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      167 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2300 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/assembler/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1491 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/basis.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1408 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.869674 pyikarus-0.3.0.dev202310000087/python/ikarus/finite_elements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      173 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/finite_elements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3465 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/finite_elements/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1792 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/materials.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.904624 pyikarus-0.3.0.dev202310000087/python/ikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      163 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1496 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.978720 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/
+-rwxrwxrwx   0 user      (1001) user      (1001)     3638 2023-05-17 21:05:43.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     9980 2023-05-17 21:05:45.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)        1 2023-05-17 21:05:43.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-17 21:05:43.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/requires.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-17 21:05:43.000000 pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      632 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/python/setup.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:48.990660 pyikarus-0.3.0.dev202310000087/sandbox/
+-rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/sandbox/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.018338 pyikarus-0.3.0.dev202310000087/sandbox/src/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1220 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.034326 pyikarus-0.3.0.dev202310000087/sandbox/src/auxiliaryFiles/
+-rwxrwxrwx   0 user      (1001) user      (1001)   674469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/sandbox/src/auxiliaryFiles/circle.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      320 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/sandbox/src/sandbox.cpp
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-17 21:05:49.496795 pyikarus-0.3.0.dev202310000087/setup.cfg
+-rwxrwxrwx   0 user      (1001) user      (1001)     1308 2023-05-17 21:05:40.000000 pyikarus-0.3.0.dev202310000087/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.054202 pyikarus-0.3.0.dev202310000087/tests/
+-rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/tests/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.388406 pyikarus-0.3.0.dev202310000087/tests/src/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1418 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3906 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/assemblerTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     9913 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/common.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2639 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/dependenciesTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6520 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/tests/src/dirichletValueTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     3820 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/easTest.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1473 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/enhancedAssumedStrainsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      608 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/tests/src/factories.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1870 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/functionTraitsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     2661 2023-05-10 14:46:30.000000 pyikarus-0.3.0.dev202310000087/tests/src/linearElasticityTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     2378 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/manifoldsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     7961 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/materialTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6770 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTest.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTestNeoHooke.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      729 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTestSVK.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     9936 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/nonLinearOperatorTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6327 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/pathFollowingTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     1651 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/polyFitTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      695 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/pythonConversionTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     1292 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/testAutodiffHelper.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     5805 2023-05-17 18:43:33.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFEElement.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-17 21:05:49.478309 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/
+-rwxrwxrwx   0 user      (1001) user      (1001)     9028 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      395 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTest.geo
+-rwxrwxrwx   0 user      (1001) user      (1001)      497 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTest.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      546 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTest2.geo
+-rwxrwxrwx   0 user      (1001) user      (1001)    11431 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1114 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000087/tests/src/testHelpers.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    17595 2023-05-10 14:46:05.000000 pyikarus-0.3.0.dev202310000087/tests/src/trustRegionTest.cpp
```

### Comparing `pyikarus-0.3.0.dev202310000086/.clang-format` & `pyikarus-0.3.0.dev202310000087/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.cmake-format` & `pyikarus-0.3.0.dev202310000087/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.0.dev202310000087/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.0.dev202310000087/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.github/workflows/createRelease.yml` & `pyikarus-0.3.0.dev202310000087/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.0.dev202310000087/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.github/workflows/debian.yml` & `pyikarus-0.3.0.dev202310000087/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.github/workflows/ghpages.yml` & `pyikarus-0.3.0.dev202310000087/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.github/workflows/runExamples.yml` & `pyikarus-0.3.0.dev202310000087/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.github/workflows/style.yml` & `pyikarus-0.3.0.dev202310000087/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/.reuse/dep5` & `pyikarus-0.3.0.dev202310000087/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/CHANGELOG.md` & `pyikarus-0.3.0.dev202310000087/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000087/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/CODE_OF_CONDUCT.md` & `pyikarus-0.3.0.dev202310000087/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/LICENSE.md` & `pyikarus-0.3.0.dev202310000087/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.0.dev202310000087/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.0.dev202310000087/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.0.dev202310000087/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/LICENSES/MIT.txt` & `pyikarus-0.3.0.dev202310000087/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.0.dev202310000087/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/PKG-INFO` & `pyikarus-0.3.0.dev202310000087/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000086
+Version: 0.3.0.dev202310000087
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
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000086 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000087 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000086/README.md` & `pyikarus-0.3.0.dev202310000087/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/cmake/CPM.cmake` & `pyikarus-0.3.0.dev202310000087/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000087/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.0.dev202310000087/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.0.dev202310000087/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.0.dev202310000087/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.0.dev202310000087/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/cmake/tools.cmake` & `pyikarus-0.3.0.dev202310000087/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/config.h.cmake` & `pyikarus-0.3.0.dev202310000087/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.0.dev202310000087/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/literature.bib` & `pyikarus-0.3.0.dev202310000087/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/mkdocs-macros.py` & `pyikarus-0.3.0.dev202310000087/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/mkdocs.yml` & `pyikarus-0.3.0.dev202310000087/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/overrides/partials/comments.html` & `pyikarus-0.3.0.dev202310000087/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/assembler.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/grids.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/index.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/observer.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/01_framework/solvers.md` & `pyikarus-0.3.0.dev202310000087/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/computePi.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/index.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.0.dev202310000087/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.0.dev202310000087/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.0.dev202310000087/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.0.dev202310000087/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.0.dev202310000087/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/download.md` & `pyikarus-0.3.0.dev202310000087/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/docs/website/index.md` & `pyikarus-0.3.0.dev202310000087/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000087/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.0.dev202310000087/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feRequirements.cpp` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feRequirements.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/basis/basis.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/test/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000087/ikarus/python/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.0.dev202310000087/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/test/nameTest.vtu` & `pyikarus-0.3.0.dev202310000087/ikarus/python/test/nameTest.vtu`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.0.dev202310000087/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.0.dev202310000087/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/algorithms.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/basis.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/concepts.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/init.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/polyfit.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/ikarus/utils/traits.hh` & `pyikarus-0.3.0.dev202310000087/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/logfile` & `pyikarus-0.3.0.dev202310000087/logfile`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000087/python/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/__init__.py` & `pyikarus-0.3.0.dev202310000087/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/_ikarus.cc` & `pyikarus-0.3.0.dev202310000087/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.0.dev202310000087/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/basis.py` & `pyikarus-0.3.0.dev202310000087/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/dirichletValues.py` & `pyikarus-0.3.0.dev202310000087/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.0.dev202310000087/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/materials.py` & `pyikarus-0.3.0.dev202310000087/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/ikarus/utils/__init__.py` & `pyikarus-0.3.0.dev202310000087/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000086
+Version: 0.3.0.dev202310000087
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
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000086 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000087 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000086/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.0.dev202310000087/python/pyikarus.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 LICENSES/CC-BY-SA-4.0.txt
 LICENSES/CC0-1.0.txt
 LICENSES/LGPL-3.0-or-later.txt
 LICENSES/MIT.txt
 LICENSES/MPL-2.0.txt
 Testing/Temporary/CTestCostData.txt
 Testing/Temporary/LastTest.log
+cmake/CMakeLists.txt
 cmake/CPM.cmake
 cmake/tools.cmake
 cmake/FormatTarget/CMakeLists.txt
 cmake/modules/AddAutoDiffFlags.cmake
 cmake/modules/AddEigenFlags.cmake
 cmake/modules/AddMatplotppFlags.cmake
 cmake/modules/AddSpdlogFlags.cmake
```

### Comparing `pyikarus-0.3.0.dev202310000086/python/setup.py.in` & `pyikarus-0.3.0.dev202310000087/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000087/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.0.dev202310000087/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/setup.py` & `pyikarus-0.3.0.dev202310000087/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # cd /tmp/Ikarus
 #  /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # > /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
 
-ikarusVersion = "0.3.0.dev202310000086" #+ datetime.today().time().strftime("%H%M%S")
+ikarusVersion = "0.3.0.dev202310000087" #+ datetime.today().time().strftime("%H%M%S")
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor sicne ikarus pypi package already exists
 print(metadata)
```

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000087/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/assemblerTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/assemblerTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/common.hh` & `pyikarus-0.3.0.dev202310000087/tests/src/common.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/dependenciesTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/dependenciesTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/dirichletValueTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/dirichletValueTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/easTest.hh` & `pyikarus-0.3.0.dev202310000087/tests/src/easTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/enhancedAssumedStrainsTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/enhancedAssumedStrainsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/factories.hh` & `pyikarus-0.3.0.dev202310000087/tests/src/factories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/functionTraitsTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/functionTraitsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/linearElasticityTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/linearElasticityTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/manifoldsTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/manifoldsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/materialTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/materialTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/nonLinearElasticityTest.hh` & `pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/nonLinearElasticityTestNeoHooke.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTestNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/nonLinearElasticityTestSVK.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/nonLinearElasticityTestSVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/nonLinearOperatorTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/nonLinearOperatorTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/pathFollowingTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/pathFollowingTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/polyFitTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/polyFitTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/pythonConversionTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/pythonConversionTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/testFEElement.hh` & `pyikarus-0.3.0.dev202310000087/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.0.dev202310000087/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/testHelpers.hh` & `pyikarus-0.3.0.dev202310000087/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000086/tests/src/trustRegionTest.cpp` & `pyikarus-0.3.0.dev202310000087/tests/src/trustRegionTest.cpp`

 * *Files identical despite different names*

