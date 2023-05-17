# Comparing `tmp/lumicks.pylake-1.0.0.tar.gz` & `tmp/lumicks.pylake-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumicks.pylake-1.0.0.tar", last modified: Tue Mar 14 14:14:43 2023, max compression
+gzip compressed data, was "lumicks.pylake-1.1.0.tar", last modified: Wed May 17 16:01:45 2023, max compression
```

## Comparing `lumicks.pylake-1.0.0.tar` & `lumicks.pylake-1.1.0.tar`

### file list

```diff
@@ -1,258 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.417761 lumicks.pylake-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-14 14:14:43.417761 lumicks.pylake-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.381761 lumicks.pylake-1.0.0/lumicks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.389761 lumicks.pylake-1.0.0/lumicks/pylake/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/adjustments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    31524 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.389761 lumicks.pylake-1.0.0/lumicks/pylake/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/confocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/h5_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/imaging_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.389761 lumicks.pylake-1.0.0/lumicks/pylake/detail/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/tests/test_widefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/timeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    22625 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/detail/widefield.py
--rw-r--r--   0 runner    (1001) docker     (123)    11255 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fdensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/file_download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.393761 lumicks.pylake-1.0.0/lumicks/pylake/fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.393761 lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/derivative_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/link_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42413 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/model_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    29491 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/fitdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    29332 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35161 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/parameter_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/profile_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.393761 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_condition_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_fd_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    26077 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_model_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_model_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_stepping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.393761 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33294 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/calibration_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/convenience.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.397761 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/drag_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/driving_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/power_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/power_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.397761 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.397761 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
--rw-r--r--   0 runner    (1001) docker     (123)    95740 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/reference_spectrum.npz
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_axial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_diode_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_driving_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_hydro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_power_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_touchdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/touchdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    24485 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/image_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    35234 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.397761 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.401761 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/linalg_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/localization_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    43119 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/msd_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/scoring_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/stitch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    49684 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/kymotrack.py
--rw-r--r--   0 runner    (1001) docker     (123)    23262 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/kymotracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/stitching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.401761 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.405761 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/csv_bad_format.csv
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/csv_unparseable.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/test_sequence_corrupted.gb
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.405761 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28854 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    44023 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8384 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_loc_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_stitching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/marker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.405761 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/correlated_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.405761 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/detail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/detail/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/detail/undostack.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/image_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/range_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.409761 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_undostack.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/note.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.409761 lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/piezo_tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.409761 lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/point_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.409761 lumicks.pylake-1.0.0/lumicks/pylake/population/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/dwelltime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/mixture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.409761 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.409761 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/exponential_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/generate_exponential_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/generate_trace_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/trace_data.npz
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/test_dwelltimes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/population/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/scalebar.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.409761 lumicks.pylake-1.0.0/lumicks/pylake/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/simulation/diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.409761 lumicks.pylake-1.0.0/lumicks/pylake/simulation/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/simulation/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/simulation/tests/test_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.413761 lumicks.pylake-1.0.0/lumicks/pylake/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.413761 lumicks.pylake-1.0.0/lumicks/pylake/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_confocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_widefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/data/test_mock_confocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.413761 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_channels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_channels/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_channels/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32471 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_channels/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_fdcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_fdensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.417761 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file/test_file_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.417761 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    45272 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.417761 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.417761 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    44182 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_imagestack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_point_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    30585 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_import_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_scalebar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_timeindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/lumicks/pylake/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:14:43.385761 lumicks.pylake-1.0.0/lumicks.pylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-14 14:14:43.000000 lumicks.pylake-1.0.0/lumicks.pylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-03-14 14:14:43.000000 lumicks.pylake-1.0.0/lumicks.pylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:14:43.000000 lumicks.pylake-1.0.0/lumicks.pylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:14:43.000000 lumicks.pylake-1.0.0/lumicks.pylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-14 14:14:43.000000 lumicks.pylake-1.0.0/lumicks.pylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-14 14:14:43.000000 lumicks.pylake-1.0.0/lumicks.pylake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-14 14:14:43.417761 lumicks.pylake-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/setup.manifest
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-03-14 14:14:25.000000 lumicks.pylake-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.260728 lumicks.pylake-1.1.0/lumicks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.264728 lumicks.pylake-1.1.0/lumicks/pylake/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/adjustments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31524 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.268729 lumicks.pylake-1.1.0/lumicks/pylake/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/confocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/h5_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/imaging_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.268729 lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/test_widefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/timeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22625 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/detail/widefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fdensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/file_download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.268729 lumicks.pylake-1.1.0/lumicks/pylake/fitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.272729 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/derivative_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/link_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42413 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/model_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29491 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/fitdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29332 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35226 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/parameter_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25402 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/profile_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.276728 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_condition_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_fd_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26077 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_model_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_model_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_stepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.276728 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33294 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/calibration_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/convenience.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.276728 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/drag_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/driving_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/power_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/power_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.280729 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.280729 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95740 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/reference_spectrum.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_axial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_diode_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_driving_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19094 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_hydro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20748 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_touchdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/touchdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24485 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/image_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35234 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.284729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.284729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/linalg_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/localization_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43966 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/msd_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15878 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/scoring_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/stitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61675 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/kymotrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/kymotracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/stitching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.288729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.292729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/csv_bad_format.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/csv_unparseable.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence_corrupted.gb
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.292729 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_image_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53232 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7813 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_loc_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_stitching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/marker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.296729 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/correlated_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.296729 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/undostack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/image_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35707 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/range_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.296729 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_undostack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/note.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.296729 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/piezo_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/point_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/population/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47601 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/dwelltime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/mixture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17320 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/exponential_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/generate_exponential_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/generate_trace_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/trace_data.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/test_dwelltimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/population/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/simulation/diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/simulation/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/simulation/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/simulation/tests/test_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18096 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_confocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_widefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/data/test_mock_confocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.300729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32471 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_fdcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_fdensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/test_file_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45272 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44182 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_imagestack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_point_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30585 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_scalebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_timeindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/lumicks/pylake/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 16:01:45.264728 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 16:01:45.000000 lumicks.pylake-1.1.0/lumicks.pylake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-17 16:01:45.304729 lumicks.pylake-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/setup.manifest
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-17 16:01:31.000000 lumicks.pylake-1.1.0/setup.py
```

### Comparing `lumicks.pylake-1.0.0/PKG-INFO` & `lumicks.pylake-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumicks.pylake
-Version: 1.0.0
+Version: 1.1.0
 Summary: Bluelake data analysis tools
 Home-page: https://github.com/lumicks/pylake
 Author: Lumicks B.V.
 Author-email: devteam@lumicks.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lumicks.pylake-1.0.0/license.md` & `lumicks.pylake-1.1.0/license.md`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/__init__.py` & `lumicks.pylake-1.1.0/lumicks/pylake/__init__.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/adjustments.py` & `lumicks.pylake-1.1.0/lumicks/pylake/adjustments.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/benchmark.py` & `lumicks.pylake-1.1.0/lumicks/pylake/benchmark.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/calibration.py` & `lumicks.pylake-1.1.0/lumicks/pylake/calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/channel.py` & `lumicks.pylake-1.1.0/lumicks/pylake/channel.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/alignment.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/alignment.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/confocal.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/confocal.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,22 +269,48 @@
 
 class ConfocalImage(BaseScan, TiffExport):
     def _to_spatial(self, data):
         """Implements any necessary post-processing actions after image reconstruction from infowave"""
         raise NotImplementedError
 
     @cachetools.cachedmethod(lambda self: self._cache)
-    def _image(self, channel):
-        assert channel in ("red", "green", "blue")
-        return self._image_factory(self, channel)
+    def _image(self, channel) -> np.ndarray:
+        """Returns a (read-only) reconstructed image.
+
+        Parameters
+        ----------
+        channel : str
+            Channel to return. Must be "red", "green" or "blue".
+        """
+        if channel not in ("red", "green", "blue"):
+            raise ValueError(f'Channel must be "red", "green" or "blue", got "{channel}".')
+
+        image = self._image_factory(self, channel)
+        image.flags.writeable = False
+
+        return image
 
     @cachetools.cachedmethod(lambda self: self._cache)
-    def _timestamps(self, channel, reduce=timestamp_mean):
-        assert channel == "timestamps"
-        return self._timestamp_factory(self, reduce)
+    def _timestamps(self, channel, reduce=timestamp_mean) -> np.ndarray:
+        """Returns (read-only) reconstructed timestamps.
+
+        Parameters
+        ----------
+        channel : str
+            Must be "timestamps".
+        reduce : callable
+            Function to reduce sample timestamps into aggregate timestamps.
+        """
+        if channel != "timestamps":
+            raise ValueError(f'channel must be "timestamps", got "{channel}"')
+
+        timestamps = self._timestamp_factory(self, reduce)
+        timestamps.flags.writeable = False
+
+        return timestamps
 
     def _get_plot_data(self, channel, adjustment=no_adjustment, frame=None):
         """Get image data for plotting requested channel.
 
         Parameters
         ----------
         channel : str
@@ -388,15 +414,15 @@
 
     @property
     def _num_pixels(self):
         return self._pixelcount_factory(self)
 
     @property
     def fast_axis(self):
-        """The axis that was scanned (x or y)"""
+        """The axis that was scanned ("X" or "Y")"""
         return self._metadata.fast_axis
 
     @property
     def timestamps(self) -> np.ndarray:
         """Timestamps for each image pixel.
 
         The returned array has the same shape as the `{color}_image` arrays. Timestamps are defined
@@ -429,8 +455,9 @@
         ----------
         channel : {'red', 'green', 'blue', 'rgb'}
             The color channel of the requested data.
         """
         if channel == "rgb":
             return np.stack([self.get_image(color) for color in ("red", "green", "blue")], axis=-1)
         else:
+            # Make sure we don't return a reference to our cache
             return self._image(channel)
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/h5_helper.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/h5_helper.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/image.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/image.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/imaging_mixins.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/imaging_mixins.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/mixin.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/plotting.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/tests/test_plotting.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/tests/test_widefield.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/tests/test_widefield.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/timeindex.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/timeindex.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/utilities.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/detail/widefield.py` & `lumicks.pylake-1.1.0/lumicks/pylake/detail/widefield.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fdcurve.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fdcurve.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,40 @@
 from collections import namedtuple
 
 
 FdSlice = namedtuple("FdSlice", "f d")
 
 
 class FdCurve(DownsampledFD):
-    """An FD curve exported from Bluelake
+    r"""An FD curve exported from Bluelake
 
     By default, the primary force and distance channels are `downsampled_force2`
     and `distance1`. Alternatives can be selected using :func:`FdCurve.with_channels()`.
     Note that it does not modify the FD curve in place but returns a copy.
 
+    Note
+    ----
+    The default channel `downsampled_force2` is the total force on trap 2, e.g.
+    :math:`\sqrt{F_{2, x}^2 + F_{2, y}^2}`
+
+    Examples
+    --------
+    ::
+
+        import lumicks.pylake as lk
+        f = lk.File("fdcurves.h5")
+
+        # Show FdCurve "1"
+        fd_curve = f.fdcurves["1"]
+        fd_curve.plot()
+
+        # Make a new F,d curve based on the `start` and `stop` time of FdCurve "1", but only include
+        # the x-component of the force on trap 2
+        fd_curve = fd_curve.with_channels("2x", distance="1")
+
     Attributes
     ----------
     file : lumicks.pylake.File
         The parent file. Used to look up channel data.
     start, stop : int
         The time range (ns) of this FD curve within the file.
     name : str
@@ -202,15 +222,41 @@
         f, d = self.f.data, self.d.data
         valid_idx = np.logical_and.reduce(
             (d > 0, d >= distance_min, d < distance_max, f >= force_min, f < force_max)
         )
         return FdSlice(f[valid_idx], d[valid_idx])
 
     def with_channels(self, force, distance):
-        """Return a copy of this FD curve with difference primary force and distance channels"""
+        r"""Return a copy of this FD curve with different primary force and distance channels
+
+        Parameters
+        ----------
+        force : str
+            Force channel to use (i.e. "1", "2", "1x", "1y").
+        distance : str
+            Distance channel to use (i.e. "1", "2").
+
+        Returns
+        -------
+        FdCurve
+
+        Examples
+        --------
+        ::
+
+            import lumicks.pylake as lk
+            f = lk.File("fdcurves.h5")
+
+            # Grab the FdCurve with the name "1"
+            fd_curve = f.fdcurves["1"]
+
+            # Make a new F,d curve based on the start and stop time of FdCurve "1" but only include
+            # the x-component of the force on trap 2
+            fd_curve = fd_curve.with_channels("2x", distance="1")
+        """
         new_fd = copy(self)
         new_fd._primary_force_channel = force
         new_fd._primary_distance_channel = distance
         return new_fd
 
     def plot_scatter(self, **kwargs):
         """Plot the FD curve points
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fdensemble.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fdensemble.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/file.py` & `lumicks.pylake-1.1.0/lumicks/pylake/file.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/file_download.py` & `lumicks.pylake-1.1.0/lumicks/pylake/file_download.py`

 * *Files 18% similar despite different names*

```diff
@@ -76,29 +76,39 @@
             m.update(b)
             b = f.read(chunk_size)
 
     return m.hexdigest() == reference_hash
 
 
 def download_from_doi(doi, target_path="", force_download=False, show_progress=True):
-    """Download files from a Zenodo DOI (i.e. 10.5281/zenodo.#######) and returns a file list in the
-    form of a List[str].
+    """Download files from a Zenodo DOI (i.e. 10.5281/zenodo.#######)
+
+    Note
+    ----
+    This function will not re-download files that have already been downloaded. You can therefore
+    safely use it at the start of a notebook or script without worrying that it will download
+    files unnecessarily.
 
     Parameters
     ----------
     doi : str
         DOI of the files to download.
     target_path : str
         Target path to download to. Default downloads to current folder.
     force_download : bool
         Force re-downloading the file even if it already exists and the hash checks out.
         When the hash of an existing file does not match, this will overwrite the existing file with
         a freshly downloaded copy.
     show_progress : bool
         Show a progress bar while downloading.
+
+    Returns
+    -------
+    list of str
+        List of downloaded file names.
     """
     url = get_url_from_doi(doi)
 
     if "zenodo" not in url:
         raise RuntimeError("Only Zenodo DOIs are supported.")
 
     record_number = url.split("/")[-1].strip()
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/datasets.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/datasets.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/derivative_manipulation.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/derivative_manipulation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/link_functions.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/link_functions.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/model_implementation.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/model_implementation.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/detail/utilities.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/detail/utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/fit.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/fit.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/fitdata.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/fitdata.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/model.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/model.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/models.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
            identities of RNA and DNA double helices unveiled at the single-molecule level. Journal
            of the American Chemical Society, 135(1), 122-131.
     .. [6] Saenger, W. (1984). Principles of Nucleic Acid Structure. Springer. New York, Berlin,
            Heidelberg.
     """
     from scipy import constants
 
-    model = ewlc_odijk_force(name)
+    model = ewlc_odijk_distance(name)
     model.defaults[f"{name}/Lc"].value = dna_length_kbp * um_per_kbp
     model.defaults[f"{name}/Lp"].value = 50.0  # [3]
     model.defaults[f"{name}/St"].value = 1200.0  # [4, 5]
     model.defaults["kT"].value = (
         1e21 * constants.k * constants.convert_temperature(temperature, "C", "K")
     )
     return model
@@ -683,15 +683,18 @@
     .. [2] Wang, M. D., Yin, H., Landick, R., Gelles, J., & Block, S. M. (1997). Stretching DNA
            with optical tweezers. Biophysical journal, 72(3), 1335-1346.
     """
     return ewlc_marko_siggia_distance(name)
 
 
 @deprecated(
-    reason=("This function will be removed in a future release. Use `wlc_force('name')` instead."),
+    reason=(
+        "This function will be removed in a future release. Use `wlc_marko_siggia_force('name')` "
+        "instead."
+    ),
     action="always",
     version="0.13.2",
 )
 def marko_siggia_simplified(name):
     """Marko Siggia's Worm-like Chain model.
 
     This model [1]_ is based on only entropic contributions (valid for F << 10 pN). This model has
@@ -707,15 +710,16 @@
     .. [1] J. Marko, E. D. Siggia. Stretching dna., Macromolecules 28.26, 8759-8770 (1995).
     """
     return wlc_marko_siggia_force(name)
 
 
 @deprecated(
     reason=(
-        "This function will be removed in a future release. Use `wlc_distance('name')` instead."
+        "This function will be removed in a future release. Use "
+        "`wlc_marko_siggia_distance('name')` instead."
     ),
     action="always",
     version="0.13.2",
 )
 def inverted_marko_siggia_simplified(name):
     """Marko Siggia's Worm-like Chain model.
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/parameter_trace.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/parameter_trace.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/parameters.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/parameters.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/profile_likelihood.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/profile_likelihood.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,59 @@
+from dataclasses import dataclass
 from scipy.stats import chi2
 import numpy as np
-from typing import NamedTuple
+from typing import Tuple, Optional
 import matplotlib.pyplot as plt
 from warnings import warn
 import enum
 
 
+def _validate_in_bound(error_description, params, lower_bounds, upper_bounds, bound_tolerance):
+    """Check whether parameters are in bound and raise if they're not.
+
+    Parameters
+    ----------
+    error_description : str
+        Description to be included as part of the error message raised when bounds are violated.
+    params : np.ndarray
+        Parameter vector
+    lower_bounds, upper_bounds : np.ndarray
+        Bounds
+    bound_tolerance : float
+        Tolerance used when checking the bound. This tolerance uses whichever is the most
+        permissive of an absolute and relative tolerance threshold.
+
+    Raises
+    ------
+    RuntimeError
+        If params is not within the bounds.
+    """
+    # Only use tolerance if it is nonzero, otherwise one gets issues with 0 * np.inf being undefined
+    if bound_tolerance:
+        lower = lower_bounds - bound_tolerance * np.maximum(abs(lower_bounds), 1.0)
+        upper = upper_bounds + bound_tolerance * np.maximum(abs(upper_bounds), 1.0)
+    else:
+        lower, upper = lower_bounds, upper_bounds
+
+    if np.any(params > upper) or np.any(params < lower):
+        over_str = " ".join(
+            f"Param {idx} was over limit by {params[idx] - upper_bounds[idx]}."
+            for idx in np.atleast_1d(np.argwhere(params > upper_bounds).squeeze())
+        )
+        under_str = " ".join(
+            f"Param {idx} was under limit by {lower_bounds[idx] - params[idx]}."
+            for idx in np.atleast_1d(np.argwhere(params < lower_bounds).squeeze())
+        )
+
+        raise RuntimeError(
+            f"{error_description}\nCurrent parameter values: {params}. "
+            f"Lower bound: {lower_bounds}, upper bound: {upper_bounds}. {over_str}{under_str}"
+        )
+
+
 def clamp_step(x_origin, x_step, lower_bound, upper_bound):
     """Shortens a step to stay within some box constraints.
 
     Parameters
     ----------
     x_origin : np.ndarray
         Parameter position we are stepping from.
@@ -20,24 +64,15 @@
 
     Returns
     -------
     new_position : np.ndarray
         New position
     scaling : bool
         Have we shrunk the step?
-
-    Raises
-    ------
-    RuntimeError
-        If the initial position `x_origin` is not within the box constraints given by `lower_bound`
-        and `upper_bound`.
     """
-    if np.any(np.logical_or(x_origin < lower_bound, x_origin > upper_bound)):
-        raise RuntimeError("Initial position was not in box constraints.")
-
     alpha_ub = np.inf * np.ones(x_step.shape)
     alpha_lb = np.inf * np.ones(x_step.shape)
 
     # Fetch distance to the boundary in multiples of the step size. Steps towards the boundary are
     # positive.
     mask = x_step != 0
     alpha_ub[mask] = (upper_bound[mask] - x_origin[mask]) / x_step[mask]
@@ -50,16 +85,18 @@
     scaling = np.min(np.maximum(alpha_ub, alpha_lb))
     if scaling > 1.0:
         scaling = 1.0
 
     return x_origin + scaling * x_step, scaling != 1.0
 
 
-class StepConfig(NamedTuple):
-    """
+@dataclass
+class StepConfig:
+    """Profile likelihood stepsize control configuration
+
     min_abs_step: float
         minimal step size in parameter space
     max_abs_step: float
         maximal step size in parameter space
     step_factor : float
         factor by which to change the step size
     min_chi2_step_size: float
@@ -77,36 +114,42 @@
     step_factor: float
     min_chi2_step_size: float
     max_chi2_step_size: float
     lower_bounds: np.array
     upper_bounds: np.array
 
 
-class ScanConfig(NamedTuple):
-    """
+@dataclass
+class ScanConfig:
+    """Profile likelihood optimization configuration
+
     lower_bounds: np.array
         optimization lower bounds
     upper_bounds: np.array
         optimization upper bounds
     fitted: np.array
         which parameters are fitted?
     step_function: callable
         function which performs 1D line scans
     termination_level: float
         chi squared value at which the optimization terminates
+    bound_tolerance : float
+        tolerance to use when verifying whether solution is inside the bounds
     """
 
     lower_bounds: np.array
     upper_bounds: np.array
     fitted: np.array
     step_function: callable
     termination_level: float
+    bound_tolerance: float
 
 
-class ProfileInfo(NamedTuple):
+@dataclass
+class ProfileInfo:
     minimum_chi2: float
     profiled_parameter_index: int
     delta_chi2: float
     confidence_level: float
     parameter_names: list
 
 
@@ -238,18 +281,28 @@
         current_step_size, p_next = scan_config.step_function(
             chi2_last, p_next, current_step_size, step_sign
         )
         try:
             p_next = fit_function(
                 p_next, scan_config.lower_bounds, scan_config.upper_bounds, scan_config.fitted
             )
-        except (ValueError, RuntimeError):
+
+            _validate_in_bound(
+                "Optimization failed to stay in bound.",
+                p_next,
+                scan_config.lower_bounds,
+                scan_config.upper_bounds,
+                scan_config.bound_tolerance,
+            )
+
+        except (ValueError, RuntimeError) as exception:
             warn(
                 f"Optimization error encountered at iteration {step}, while attempting "
-                f"parameter values: {p_next}. Terminating profile. Parameter bound not found.",
+                f"parameter values: {p_next}:\n {repr(exception)}.\n\nTerminating profile. "
+                f"Parameter bound not found.",
                 RuntimeWarning,
             )
             break
 
         chi2_last = chi2_function(p_next)
         chi2_list.append(chi2_last)
         parameter_vectors.append(p_next)
@@ -257,15 +310,17 @@
         if verbose:
             print(f"Iteration {step}: Step size: {current_step_size}, p_next: {p_next}")
 
         step += 1
         if chi2_last > scan_config.termination_level:
             break
 
-    return np.array(chi2_list), np.vstack(parameter_vectors)
+    return np.array(chi2_list), (
+        np.vstack(parameter_vectors) if parameter_vectors else np.empty((0, parameter_vector.size))
+    )
 
 
 def find_crossing(x, y, crossing):
     (indices,) = np.where(y >= crossing)
 
     if np.any(indices):
         index = indices[0]
@@ -284,28 +339,75 @@
         max_step=1.0,
         step_factor=2.0,
         min_chi2_step=0.05,
         max_chi2_step=0.5,
         termination_significance=0.99,
         confidence_level=0.95,
         num_dof=1,
+        bound_tolerance=0.0,
     ):
+        """Profile likelihood
+
+        This method traces an optimal path through parameter space in order to estimate parameter
+        confidence intervals. It iteratively performs a step for the profiled parameter, then
+        fixes that parameter and re-optimizes all the other parameters [1]_ [2]_.
+
+        Parameters
+        ----------
+        parameter_name : str
+            Name of the parameter to profile
+        min_step : float
+            Minimum step size, default: 1e-4
+        max_step : float
+            Maximum step size, default: 1.0
+        step_factor : float
+            Step factor. This is by what ratio the stepsize is increased when stepping too slow (low
+            increase in likelihood) or decreased when stepping too fast. Default: 2.0.
+        min_chi2_step : float
+            Minimum increase in chi-squared that we aim for in each step. Going below this limit
+            results in the step size being increased. Default: 0.05.
+        max_chi2_step : float
+            Maximum increase in chi-squared that we aim for in each step. Going above this limit
+            results in the step being rejected and the step size being decreased. Default: 0.5
+        termination_significance : float
+            At what significance level should the profiling terminate. Default: 0.99.
+        confidence_level : float
+            At which confidence level should the confidence interval be determined. Default: 0.95
+        num_dof : int
+            Number of degrees of freedom. Default: 1.
+        bound_tolerance : float
+            Bound tolerance. By default, the profiling procedure checks whether the solver stayed
+            within the user specified parameter bounds. The valid range specified here is given as
+            [lower_bnd - tol * max(1.0, abs(lower_bnd)), upper_bnd + tol * max(1.0, abs(upper_bnd))]
+            Default: 0.
+
+        References
+        ----------
+        .. [1] Raue, A., Kreutz, C., Maiwald, T., Bachmann, J., Schilling, M., Klingmüller, U.,
+               & Timmer, J. (2009). Structural and practical identifiability analysis of partially
+               observed dynamical models by exploiting the profile likelihood. Bioinformatics,
+               25(15), 1923-1929.
+        .. [2] Maiwald, T., Hass, H., Steiert, B., Vanlier, J., Engesser, R., Raue, A., Kipkeew,
+               F., Bock, H.H., Kaschek, D., Kreutz, C. and Timmer, J., 2016. Driving the model to
+               its limit: profile likelihood based model reduction. PloS one, 11(9).
+        """
         self.parameter_name = parameter_name
 
         # These are the user exposed options. They can be modified by the user in the struct if
         # desired. They are parsed into actual algorithm parameters once the algorithm starts.
         self.options = {
             "min_step": min_step,
             "max_step": max_step,
             "step_factor": step_factor,
             "min_chi2_step": min_chi2_step,
             "max_chi2_step": max_chi2_step,
             "termination_significance": termination_significance,
             "confidence_level": confidence_level,
             "num_dof": num_dof,
+            "bound_tolerance": bound_tolerance,
         }
 
         self.profile_info = None
         self._chi2 = {}
         self._parameters = {}
 
     def __str__(self):
@@ -354,14 +456,22 @@
 
         if options["max_chi2_step"] <= options["min_chi2_step"]:
             raise RuntimeError(
                 "max_chi2_step must be larger than min_chi2_step, got max_chi2_step="
                 f"{options['max_chi2_step']} and min_chi2_step={options['min_chi2_step']}."
             )
 
+        _validate_in_bound(
+            "Initial position was not in box constraints.",
+            parameters.values,
+            parameters.lower_bounds,
+            parameters.upper_bounds,
+            options["bound_tolerance"],
+        )
+
         self.profile_info = ProfileInfo(
             minimum_chi2=chi2_function(parameters.values),
             profiled_parameter_index=list(parameters.keys()).index(parameter_name),
             delta_chi2=chi2.ppf(options["confidence_level"], options["num_dof"]),
             confidence_level=options["confidence_level"],
             parameter_names=list(parameters.keys()),
         )
@@ -400,14 +510,15 @@
         scan_config = ScanConfig(
             lower_bounds=parameters.lower_bounds,
             upper_bounds=parameters.upper_bounds,
             fitted=fitted,
             step_function=step_function,
             termination_level=self.profile_info.minimum_chi2
             + chi2.ppf(options["termination_significance"], options["num_dof"]),
+            bound_tolerance=options["bound_tolerance"],
         )
 
         def scan_direction(chi2_last, parameter_vector, step_sign, num_steps, verbose):
             return scan_dir_optimisation(
                 chi2_function,
                 fit_function,
                 chi2_last,
@@ -451,45 +562,106 @@
 
     @property
     def upper_bound(self):
         cutoff = self.profile_info.minimum_chi2 + self.profile_info.delta_chi2
         p_index = self.profile_info.profiled_parameter_index
         return find_crossing(self._parameters["fwd"][:, p_index], self._chi2["fwd"], cutoff)
 
+    def get_interval(self, significance_level=None) -> Tuple[Optional[float], Optional[float]]:
+        """Calculate confidence interval at a particular significance level
+
+        Parameter
+        ---------
+        significance level : float
+            Desired significance level (resulting in a 100 * (1 - alpha)% confidence interval).
+            If omitted, the value specified when creating the profile is used.
+
+        Returns
+        -------
+        lower_bound : float, optional
+            Lower bound of the confidence interval.
+        upper_bound : float, optional
+            Upper bound of the confidence interval. If a bound cannot be determined (either due to
+            an insufficient number of steps or lack of information in the data, the bound is given
+            as `None`).
+
+        Raises
+        ------
+        RuntimeError
+            If significance level is chosen higher than the termination level of the profile.
+        """
+        profiled_level = 1.0 - self.options["termination_significance"]
+        significance_level = (
+            significance_level
+            if significance_level is not None
+            else 1.0 - self.options["confidence_level"]
+        )
+
+        if significance_level <= profiled_level:
+            raise RuntimeError(
+                f"Significance level ({significance_level}) cannot be chosen lower or equal than "
+                f"the minimum profiled level ({profiled_level:.2f})."
+            )
+
+        cutoff = self.profile_info.minimum_chi2 + chi2.ppf(
+            1.0 - significance_level, self.options["num_dof"]
+        )
+
+        p_index = self.profile_info.profiled_parameter_index
+        return (
+            find_crossing(self._parameters["bwd"][:, p_index], self._chi2["bwd"], cutoff),
+            find_crossing(self._parameters["fwd"][:, p_index], self._chi2["fwd"], cutoff),
+        )
+
     @property
     def parameters(self):
         return np.vstack((np.flipud(self._parameters["bwd"]), self._parameters["fwd"]))
 
     @property
     def chi2(self):
         return np.hstack((np.flipud(self._chi2["bwd"]), self._chi2["fwd"]))
 
     @property
     def p(self):
         return self.parameters[:, self.profile_info.profiled_parameter_index]
 
-    def plot(self, **kwargs):
+    def plot(self, *, significance_level=None, **kwargs):
+        """Plot profile likelihood
+
+        Parameters
+        ----------
+        significance_level : float, optional
+            Desired significance level  (resulting in a 100 * (1 - alpha)% confidence interval) to
+            plot. Default is the significance level specified when the profile was generated.
+        """
         dash_length = 5
         plt.plot(self.p, self.chi2, **kwargs)
-        confidence_chi2 = self.profile_info.minimum_chi2 + self.profile_info.delta_chi2
+
+        confidence_coefficient = (
+            1.0 - significance_level
+            if significance_level is not None
+            else self.profile_info.confidence_level
+        )
+        delta_chi2 = chi2.ppf(confidence_coefficient, self.options["num_dof"])
+        confidence_chi2 = self.profile_info.minimum_chi2 + delta_chi2
         plt.axhline(y=confidence_chi2, linewidth=1, color="k", dashes=[dash_length, dash_length])
 
-        ci_min, ci_max = self.lower_bound, self.upper_bound
+        ci_min, ci_max = self.get_interval(significance_level)
         if ci_min:
             plt.axvline(x=ci_min, linewidth=1, color="k", dashes=[dash_length, dash_length])
         if ci_max:
             plt.axvline(x=ci_max, linewidth=1, color="k", dashes=[dash_length, dash_length])
 
-        plt.text(min(self.p), confidence_chi2, f"{self.profile_info.confidence_level * 100}%")
+        plt.text(min(self.p), confidence_chi2, f"{confidence_coefficient * 100}%")
         plt.ylabel("$\\chi^2$")
         plt.xlabel(self.parameter_name)
         plt.ylim(
             [
-                self.profile_info.minimum_chi2 - 0.1 * self.profile_info.delta_chi2,
-                self.profile_info.minimum_chi2 + 1.1 * self.profile_info.delta_chi2,
+                self.profile_info.minimum_chi2 - 0.1 * delta_chi2,
+                self.profile_info.minimum_chi2 + 1.1 * delta_chi2,
             ]
         )
 
     def plot_relations(self, params=None, **kwargs):
         """Plot the relations between the different parameters.
 
         Parameters
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_condition_handling.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_condition_handling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_fd_models.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_fd_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -177,7 +177,35 @@
 def test_invalid_params_models(model, test_params):
     for test_param in test_params:
         params = {p: 1 for p in getfullargspec(model).args}
         for value in (0, -1):
             with pytest.raises(ValueError, match="must be bigger than 0"):
                 params[test_param] = value
                 model(**params)
+
+
+@pytest.mark.parametrize(
+    "convenience_model, ref_model, ref_params",
+    [
+        [
+            dsdna_ewlc_odijk_distance,
+            ewlc_odijk_distance,
+            {"m/Lc": 100 * 0.34, "m/Lp": 50.0, "m/St": 1200.0, "kT": 4.11},
+        ],
+        [
+            ssdna_efjc_distance,
+            efjc_distance,
+            {"m/Lc": 100 * 0.56, "m/Lp": 0.7, "m/St": 750.0, "kT": 4.11},
+        ],
+    ],
+)
+def test_convenience_models(convenience_model, ref_model, ref_params):
+    x = np.arange(1.0, 5.0)
+    model = convenience_model("m", 100)
+    params = dict(model.defaults)
+
+    for param in ref_params.keys():
+        np.testing.assert_allclose(params[param].value, ref_params[param])
+
+    # The convenience part is in the parameters, with the old parameters they should produce the
+    # exact same as what they are supposed to be based on
+    np.testing.assert_allclose(model(x, params), ref_model("m")(x, params))
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_fit.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_fit.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_model_composition.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_model_composition.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_model_sim.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_model_sim.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_parameter_inversion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_parameters.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_pickling.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_stderr.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_stderr.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_stepping.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_stepping.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,19 +111,7 @@
             step_sign=1,
             step_config=cfg,
         )
         assert step_size == cfg.min_abs_step
         np.testing.assert_allclose(
             p_trial, np.array([2.0 + cfg.min_abs_step, 2.0 + cfg.min_abs_step])
         )
-
-
-@pytest.mark.parametrize("pos, dir", [(5, 6), (3, 2)])
-def test_out_of_bounds_step_origin(pos, dir):
-    with pytest.raises(RuntimeError, match="Initial position was not in box constraints"):
-        # If we step even the tiniest increment over one of the bounds, it should fire!
-        clamp_step(
-            np.array([np.nextafter(pos, dir)]), np.asarray([1]), np.asarray([3]), np.asarray([5])
-        )
-
-    # Position itself should be fine
-    clamp_step(np.array([pos]), np.asarray([1]), np.asarray([3]), np.asarray([5]))
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/fitting/tests/test_utilities.py` & `lumicks.pylake-1.1.0/lumicks/pylake/fitting/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/calibration_models.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/calibration_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/convenience.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/convenience.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/drag_models.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/drag_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/driving_input.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/driving_input.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/hydrodynamics.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/detail/power_models.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/detail/power_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/power_spectrum.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/power_spectrum.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/power_spectrum_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/simulate_calibration_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/data/simulate_ideal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/reference_spectrum.npz` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/reference_spectrum.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_active_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_axial.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_axial.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_convenience.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_convenience.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_diode_models.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_diode_models.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_driving_input.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_driving_input.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_hydro.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_hydro.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_power_model.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_model.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_spectrum.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_power_spectrum_calibration.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_simulations.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/tests/test_touchdown.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/tests/test_touchdown.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/force_calibration/touchdown.py` & `lumicks.pylake-1.1.0/lumicks/pylake/force_calibration/touchdown.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/group.py` & `lumicks.pylake-1.1.0/lumicks/pylake/group.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/image_stack.py` & `lumicks.pylake-1.1.0/lumicks/pylake/image_stack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymo.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymo.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/gaussian_mle.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/geometry_2d.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/geometry_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/linalg_2d.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/linalg_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/msd_estimation.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/msd_estimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,25 +580,29 @@
     if max_lag < 2:
         raise ValueError("You need at least two lags to estimate a diffusion constant")
 
     if any(np.diff(frame_idx) > 1):
         if method == "gls":
             raise RuntimeError(
                 "Your tracks cannot have missing frames when using the GLS estimator. Refine your "
-                "tracks using `lk.refine_tracks_centroid()`. Please refer to "
-                "`help(lk.refine_tracks_centroid)` for more information."
+                "tracks using `lk.refine_tracks_centroid()` or `lk.refine_tracks_gaussian()`. "
+                "Please refer to `help(lk.refine_tracks_centroid)` or "
+                "`help(lk.refine_tracks_gaussian())` for more information."
             )
         elif method == "ols":
             warnings.warn(
                 RuntimeWarning(
                     "Your tracks have missing frames. Note that this results in a poor estimate of "
                     "the standard error of the estimate. To avoid this warning, you can refine "
-                    "your tracks using `lk.refine_tracks_centroid()`. Please refer to "
-                    "`help(lk.refine_tracks_centroid)` for more information."
-                )
+                    "your tracks using `lk.refine_tracks_centroid()` or "
+                    "`lk.refine_tracks_gaussian()`. Please refer to "
+                    "`help(lk.refine_tracks_centroid)` or `help(lk.refine_tracks_gaussian)` for "
+                    "more information."
+                ),
+                stacklevel=2,
             )
 
     frame_lags, msd = calculate_msd(frame_idx, coordinate, max_lag)
 
     method_fun = _diffusion_gls if method == "gls" else _diffusion_ols
     intercept, slope, var_slope = method_fun(frame_lags, msd, len(coordinate))
 
@@ -1024,26 +1028,36 @@
         method="cve",
         unit=unit,
         _unit_label=unit_label,
         variance_of_localization_variance=var_of_localization_var,
     )
 
 
-def ensemble_cve(kymotracks):
+def ensemble_cve(kymotracks, calculate_localization_var=True):
     """Calculate ensemble-based CVE.
 
     Determines the weighted average of the mean and standard error of the CVE estimates.
 
     See docstring for _cve for more information on the estimator itself. The averaging is handled
     through equation 57 and 58 from [14]_.
 
     Parameters
     ----------
     kymotracks : lumicks.pylake.kymotracker.kymotrack.KymoTrackGroup
         Group of kymotracks
+    calculate_localization_var : bool
+        If localization variance can be calculated. Must be False if source kymographs
+        do not have the same line times or pixel sizes.
+
+    Warns
+    -----
+    RuntimeWarning
+        if `method == "cve"` and the source kymographs do not have the same line times
+        or pixel sizes. As a result, the localization variance and variance of the localization
+        variance not be available. Estimates that are unavailable are returned as `np.nan`.
 
     References
     ----------
     .. [14] Vestergaard, C. L., Blainey, P. C., & Flyvbjerg, H. (2014). Optimal estimation of
             diffusion coefficients from single-particle trajectories. Physical Review E, 89(2),
             022726.
     """
@@ -1062,16 +1076,19 @@
 
     counts = np.array([c.num_points for c in cve_based])
     counts_sum = sum(counts)
 
     ensemble_mean, ensemble_mean_var = mean_var(
         np.array([c.value for c in cve_based]), counts, counts_sum
     )
-    ensemble_localization_var, var_of_localization_var = mean_var(
-        np.array([c.localization_variance for c in cve_based]), counts, counts_sum
+
+    ensemble_localization_var, var_of_localization_var = (
+        mean_var(np.array([c.localization_variance for c in cve_based]), counts, counts_sum)
+        if calculate_localization_var
+        else (np.nan, np.nan)
     )
 
     return DiffusionEstimate(
         value=ensemble_mean,
         std_err=np.sqrt(ensemble_mean_var),
         num_lags=np.nan,
         num_points=counts_sum,
@@ -1127,17 +1144,18 @@
         else max_lag
     )
 
     intercept, slope, var_slope = _diffusion_ols(
         ensemble_msd.lags[:optimal_lags], ensemble_msd.msd[:optimal_lags], track_length
     )
 
-    time_step = kymotracks._kymo.line_time_seconds
+    time_step = kymotracks._kymos[0].line_time_seconds
     to_time = 1.0 / (2.0 * time_step)
-    src_calibration = kymotracks._kymo._calibration
+
+    src_calibration = kymotracks._kymos[0]._calibration
     return DiffusionEstimate(
         value=slope * to_time,
         std_err=np.sqrt(var_slope / np.mean(ensemble_msd.effective_sample_size)) * to_time,
         num_lags=optimal_lags,
         num_points=sum(len(t) for t in kymotracks),
         localization_variance=intercept / 2.0,
         method="ensemble ols",
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/peakfinding.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/peakfinding.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/scoring_functions.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/scoring_functions.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/sequence.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/sequence.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/stitch.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/stitch.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/detail/trace_line_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/kymotrack.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/kymotrack.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,55 @@
+import itertools
 from copy import copy
 from sklearn.neighbors import KernelDensity
 from .detail.msd_estimation import *
 from .detail.localization_models import LocalizationModel
 from .. import __version__
 from ..population.dwelltime import DwelltimeModel
 
 
-def export_kymotrackgroup_to_csv(filename, kymotrack_group, delimiter, sampling_width):
+def export_kymotrackgroup_to_csv(
+    filename, kymotrack_group, delimiter, sampling_width, *, correct_origin=None
+):
     """Export KymoTrackGroup to a csv file.
 
     Parameters
     ----------
     filename : str
         Filename to output KymoTrackGroup to.
     kymotrack_group : KymoTrackGroup
         Kymograph tracks to export.
     delimiter : str
         Which delimiter to use in the csv file.
     sampling_width : int or None
-        If, this will sample the source image around the kymograph track and export the summed intensity with
-        the image. The value indicates the number of pixels in either direction to sum over.
+        If specified, this will sample the source image around the kymograph track and export the
+        summed intensity with the image. The value indicates the number of pixels in either
+        direction to sum over.
+    correct_origin : bool, optional
+        Use the correct pixel origin when sampling from image. Kymotracks are defined with the
+        origin of each image pixel defined at the center. Earlier versions of the method that
+        samples photon counts around the track had a bug which assumed the origin at the edge
+        of the pixel. Setting this flag to `True` produces the correct behavior. The default is
+        set to `None` which reproduces the old behavior and results in a warning, while `False`
+        reproduces the old behavior without a warning.
+
+    Raises
+    ------
+    NotImplementedError
+        If group contains tracks from more than one source kymograph.
     """
     if not kymotrack_group:
         raise RuntimeError("No kymograph tracks to export")
 
+    kymotrack_group._validate_single_source(
+        "Exporting a group with tracks from more than a single source kymograph"
+    )
+
     time_units = "seconds"
-    position_units = kymotrack_group._kymo._calibration.unit
+    position_units = kymotrack_group._calibration_info["unit"]
 
     idx = np.hstack([np.full(len(track), idx) for idx, track in enumerate(kymotrack_group)])
     coords_idx = np.hstack([track.coordinate_idx for track in kymotrack_group])
     times_idx = np.hstack([track.time_idx for track in kymotrack_group])
 
     position = np.hstack([track.position for track in kymotrack_group])
     seconds = np.hstack([track.seconds for track in kymotrack_group])
@@ -48,15 +68,20 @@
     store_column(f"time ({time_units})", "%.18e", seconds)
     store_column(f"position ({position_units})", "%.18e", position)
 
     if sampling_width is not None:
         store_column(
             f"counts (summed over {2 * sampling_width + 1} pixels)",
             "%d",
-            np.hstack([track.sample_from_image(sampling_width) for track in kymotrack_group]),
+            np.hstack(
+                [
+                    track.sample_from_image(sampling_width, correct_origin=correct_origin)
+                    for track in kymotrack_group
+                ]
+            ),
         )
 
     version_header = f"Exported with pylake v{__version__} | track coordinates v2\n"
     header = version_header + delimiter.join(column_titles)
     data = np.vstack(data).T
     np.savetxt(filename, data, fmt=fmt, header=header, delimiter=delimiter)
 
@@ -169,44 +194,67 @@
         return KymoTrack(
             time_idx,
             localization,
             self._kymo,
             self._channel,
         )
 
+    def _flip(self, kymo):
+        """Return a copy flipped vertically.
+
+        Parameters
+        ----------
+        kymo : lumicks.pylake.Kymo
+            Flipped kymograph
+        """
+
+        return KymoTrack(
+            self.time_idx,
+            self._localization._flip(self._kymo.pixelsize[0] * (self._kymo.pixels_per_line - 1)),
+            kymo,
+            self._channel,
+        )
+
     def with_offset(self, time_offset, coordinate_offset):
         """Returns an offset version of the KymoTrack"""
         # Convert from image units to (integer rounded toward zero) pixels
         time_pixel_offset = int(time_offset / self._line_time_seconds)
         coordinate_pixel_offset = int(coordinate_offset / self._pixelsize)
 
         return self._with_coordinates(
             self.time_idx + time_pixel_offset,
             self.coordinate_idx + coordinate_pixel_offset,
         )
 
     def __add__(self, other):
         """Concatenate two KymoTracks"""
-        return self._with_coordinates(
-            np.hstack((self.time_idx, other.time_idx)),
-            np.hstack((self.coordinate_idx, other.coordinate_idx)),
-        )
+        try:
+            localization = self._localization + other._localization
+        except TypeError:
+            # If one of them is a refined localization and the other is not, fall back to
+            # a non-refined localization.
+            localization = np.hstack((self.coordinate_idx, other.coordinate_idx))
+
+        return self._with_coordinates(np.hstack((self.time_idx, other.time_idx)), localization)
 
     def __getitem__(self, item):
         return np.squeeze(
             np.array(np.vstack((self.time_idx[item], self.coordinate_idx[item]))).transpose()
         )
 
     @property
     def time_idx(self):
         return self._time_idx
 
     @property
     def coordinate_idx(self):
-        """Return spatial coordinates in units of pixels."""
+        """Return spatial coordinates in units of pixels.
+
+        Coordinates are defined w.r.t. pixel centers (i.e. 0, 0 is the center of the first pixel).
+        """
         return self._localization.position / self._kymo.pixelsize[0]
 
     @property
     def seconds(self):
         """The tracked temporal coordinates in seconds."""
         return self._line_time_seconds * self.time_idx
 
@@ -250,31 +298,82 @@
 
     def interpolate(self):
         """Interpolate KymoTrack to whole pixel values"""
         interpolated_time = np.arange(int(np.min(self.time_idx)), int(np.max(self.time_idx)) + 1, 1)
         interpolated_coord = np.interp(interpolated_time, self.time_idx, self.coordinate_idx)
         return self._with_coordinates(interpolated_time, interpolated_coord)
 
-    def sample_from_image(self, num_pixels, reduce=np.sum):
+    def _split(self, node):
+        """Split track.
+
+        Splits a track at `node`. Returns two tracks if successful.
+
+        Parameters
+        ----------
+        node : int
+            Node index to split at
+
+        Raises
+        ------
+        ValueError
+            If asked to split at a point that would result in an empty track.
+        """
+        node = np.clip(node, 0, len(self))
+        before = self._with_coordinates(self.time_idx[:node], self._localization[:node])
+        after = self._with_coordinates(self.time_idx[node:], self._localization[node:])
+
+        if not before or not after:
+            raise ValueError("Invalid split point. This split would result in an empty track")
+
+        return before, after
+
+    def sample_from_image(self, num_pixels, reduce=np.sum, *, correct_origin=None):
         """Sample from image using coordinates from this KymoTrack.
 
         This function samples data from the image given in data based on the points in this
         KymoTrack. It samples from `[time, position - num_pixels : position + num_pixels + 1]` and
         then applies the function sum.
 
         Parameters
         ----------
         num_pixels : int
             Number of pixels in either direction to include in the sample
         reduce : callable
             Function evaluated on the sample. (Default: np.sum which produces sum of photon counts).
+        correct_origin : bool, optional
+            Use the correct pixel origin when sampling from image. Kymotracks are defined with the
+            origin of each image pixel defined at the center. Earlier versions of the method that
+            samples photon counts around the track had a bug which assumed the origin at the edge
+            of the pixel. Setting this flag to `True` produces the correct behavior. The default is
+            set to `None` which reproduces the old behavior and results in a warning, while `False`
+            reproduces the old behavior without a warning.
         """
-        # Time and coordinates are being cast to an integer since we use them to index into a data array.
+        if correct_origin is None:
+            warnings.warn(
+                RuntimeWarning(
+                    "Prior to version 1.1.0 the method `sample_from_image` had a bug that assumed "
+                    "the origin of a pixel to be at the edge rather than the center of the pixel. "
+                    "Consequently, the sampled window could frequently be off by one pixel. To get "
+                    "the correct behavior and silence this warning, specify `correct_origin=True`. "
+                    "The old (incorrect) behavior is maintained until the next major release to "
+                    "ensure backward compatibility. To silence this warning use "
+                    "`correct_origin=False`."
+                ),
+                stacklevel=2,
+            )
+
+        # Time and coordinates are being cast to an integer since we use them to index into a data
+        # array. Note that coordinate pixel centers are defined at integer coordinates.
+        offset = 0.0 if not correct_origin else 0.5
         return [
-            reduce(self._image[max(int(c) - num_pixels, 0) : int(c) + num_pixels + 1, int(t)])
+            reduce(
+                self._image[
+                    max(int(c + offset) - num_pixels, 0) : int(c + offset) + num_pixels + 1, int(t)
+                ]
+            )
             for t, c in zip(self.time_idx, self.coordinate_idx)
         ]
 
     def extrapolate(self, forward, n_estimate, extrapolation_length):
         """This function linearly extrapolates a track segment towards positive time.
 
         Parameters
@@ -647,33 +746,96 @@
         # Or index by a list or numpy array
         tracks[[1, 3]]  # Extract the second and fourth track.
         tracks[np.asarray([1, 3])]  # Same as above.
     """
 
     def __init__(self, kymo_tracks):
         self._src = kymo_tracks
-        if self:
-            if len(set(kymo_tracks)) != len(kymo_tracks):
-                raise ValueError(
-                    "Some tracks appear multiple times. The provided tracks must be unique."
-                )
+        self._kymos = self._validate_compatible_sources()
 
-            self._validate_single_source(kymo_tracks)
+    def _validate_compatible_sources(self, additional_tracks=()):
+        """Check that source kymos for all tracks (including in self) are compatible.
 
-    def _validate_single_source(self, kymo_tracks):
-        kymos = set([track._kymo._id for track in kymo_tracks])
-        channels = set([track._channel for track in kymo_tracks])
+        Parameters
+        ----------
+        additional_tracks : KymoTrackGroup, optional
+            Additional tracks to be added to the current instance.
 
-        if len(kymos) > 1:
-            raise ValueError("All tracks must have the same source kymograph.")
+        Returns
+        -------
+        tuple
+            Tuple of source kymograph instances
+        """
+        tracks = list(itertools.chain(self, additional_tracks))
+        if not len(tracks):
+            return ()
 
+        if len(set(tracks)) != len(tracks):
+            raise ValueError(
+                "Cannot extend this KymoTrackGroup with a KymoTrack that is already part of the group"
+                if additional_tracks
+                else "Some tracks appear multiple times. The provided tracks must be unique."
+            )
+
+        channels = {track._channel for track in tracks}
         if len(channels) > 1:
             raise ValueError("All tracks must be from the same color channel.")
 
-        return next(iter(kymos)), next(iter(channels))
+        kymos = tuple({track._kymo: None for track in tracks}.keys())
+        if len(calibrations := set([kymo._calibration.unit for kymo in kymos])) > 1:
+            raise ValueError(
+                f"All tracks must be calibrated in the same units, got {calibrations}."
+            )
+
+        return kymos
+
+    def _validate_single_source(self, method_description):
+        if not self:
+            raise RuntimeError("No kymo associated with this empty group (no tracks available)")
+
+        if (n_kymos := len(self._kymos)) > 1:
+            raise NotImplementedError(
+                f"{method_description} is not supported. "
+                f"This group contains tracks from {n_kymos} source kymographs."
+            )
+
+    def _validate_single_linetime_pixelsize(self):
+        """Check that image acquisition attributes (scan line times and pixel sizes)
+        are the same for all source kymos.
+
+        Returns
+        -------
+        bool
+            If validity criteria are met (all source kymographs have the same line times and pixel sizes)
+        str
+            Error message to be raised if validity criteria are not met
+        """
+
+        line_times = {kymo.line_time_seconds for kymo in self._kymos}
+        pixel_sizes = {kymo.pixelsize_um[0] for kymo in self._kymos}
+
+        line_times_err_msg = (
+            ""
+            if len(line_times) == 1
+            else (
+                f"All source kymographs must have the same line times, got {sorted(line_times)} seconds."
+            )
+        )
+
+        px_size_err_msg = (
+            ""
+            if len(pixel_sizes) == 1
+            else (
+                "All source kymographs must have the same pixel sizes, "
+                f"got {sorted(pixel_sizes)} {self._calibration_info['unit']}."
+            )
+        )
+
+        if line_times_err_msg or px_size_err_msg:
+            raise ValueError(" ".join([line_times_err_msg, px_size_err_msg]))
 
     def __iter__(self):
         return self._src.__iter__()
 
     def __getitem__(self, item):
         if isinstance(item, slice):
             return KymoTrackGroup(self._src[item])
@@ -718,33 +880,69 @@
         ----------
         track : KymoTrack
             track to remove from the group
         """
         self._src.remove(track)
 
     @property
-    def _kymo(self):
+    def _channel(self):
         try:
-            return self[0]._kymo
+            return self[0]._channel
         except IndexError:
-            raise RuntimeError("No kymo associated with this empty group (no tracks available)")
+            raise RuntimeError("No channel associated with this empty group (no tracks available)")
 
     @property
-    def _channel(self):
+    def _calibration_info(self):
         try:
-            return self[0]._channel
+            kymo = self._kymos[0]
+            return {"unit": kymo._calibration.unit, "unit_label": kymo._calibration.unit_label}
         except IndexError:
-            raise RuntimeError("No channel associated with this empty group (no tracks available)")
+            raise RuntimeError("No kymo associated with this empty group (no tracks available)")
+
+    def _flip(self):
+        """Return a flipped copy of this KymoTrackGroup.
+
+        Raises
+        ------
+        NotImplementedError
+            If group contains tracks from more than one source kymograph.
+        """
+        self._validate_single_source("Flipping")
+        flipped_kymo = self._kymos[0].flip()
+        return KymoTrackGroup([track._flip(flipped_kymo) for track in self])
+
+    def _split_track(self, track, split_node, min_length):
+        """Split a track at a particular node
+
+        Splits a track at index `split_node`. Modifies the `KymoTrackGroup` in-place. The track to
+        be split is removed and the split tracks are appended to the list of `KymoTracks` if they
+        are long enough for inclusion (length equal or larger than `min_length`).
+
+        Parameters
+        ----------
+        track : KymoTrack
+            Track to split
+        split_node : int
+            Index of the node in the track to split at
+        min_length : int
+            Minimum length of a track. Tracks shorter than this will be discarded.
+
+        Raises
+        ------
+        ValueError
+            If asked to split at a point that would result in an empty track.
+        """
+        new_tracks = [t for t in track._split(split_node) if len(t) >= min_length]
+
+        self._src.remove(track)
+        self._src.extend(new_tracks)
 
     def _merge_tracks(self, starting_track, starting_node, ending_track, ending_node):
         """Connect two tracks from any given nodes, removing the points in between.
 
-        Note: Any specialized refinement (eg. gaussian refinement) will be lost when
-        tracks are merged.
-
         Parameters
         ----------
         starting_track: KymoTrack
             First track to connect
         starting_node : int
             Index of the node in the track to connect from
         ending_track: KymoTrack
@@ -775,20 +973,20 @@
         if start_time_idx > end_time_idx:
             starting_track, ending_track = ending_track, starting_track
             starting_node, ending_node = ending_node, starting_node
 
         # up to and *including* starting_node
         first_half = starting_track._with_coordinates(
             starting_track.time_idx[: starting_node + 1],
-            starting_track.coordinate_idx[: starting_node + 1],
+            starting_track._localization[: starting_node + 1],
         )
 
         last_half = ending_track._with_coordinates(
             ending_track.time_idx[ending_node:],
-            ending_track.coordinate_idx[ending_node:],
+            ending_track._localization[ending_node:],
         )
 
         self._src[self._src.index(starting_track)] = first_half + last_half
         if starting_track != ending_track:
             self.remove(ending_track)
 
     def __len__(self):
@@ -820,28 +1018,15 @@
         if not (isinstance(other, KymoTrack) or isinstance(other, self.__class__)):
             raise TypeError(
                 f"You can only extend a {self.__class__.__name__} with a {self.__class__.__name__} "
                 f"or {KymoTrack.__name__}"
             )
 
         other = self.__class__([other]) if isinstance(other, KymoTrack) else other
-        other_kymo, other_channel = self._validate_single_source(other)
-        if self:
-            if self._kymo._id != other_kymo:
-                raise ValueError("All tracks must have the same source kymograph.")
-
-            if self._channel != other_channel:
-                raise ValueError("All tracks must be from the same color channel.")
-
-        if len(set(other._src) | set(self._src)) != len(self._src) + len(other._src):
-            raise ValueError(
-                "Cannot extend this KymoTrackGroup with a KymoTrack that is already part of the "
-                "group"
-            )
-
+        self._kymos = self._validate_compatible_sources(other)
         self._src.extend(other._src)
 
     def remove_tracks_in_rect(self, rect, all_points=False):
         """Removes tracks that fall in a particular region.
 
         Parameters
         ----------
@@ -878,31 +1063,128 @@
         from ..detail.plotting import get_axes
 
         ax = get_axes(axes)
         for track in self:
             track.plot(show_outline=show_outline, show_labels=False, axes=ax, **kwargs)
 
         if show_labels:
-            ax.set_ylabel(f"position ({self._kymo._calibration.unit_label})")
+            ax.set_ylabel(f"position ({self._calibration_info['unit_label']})")
             ax.set_xlabel("time (s)")
 
-    def save(self, filename, delimiter=";", sampling_width=None):
+    def save(self, filename, delimiter=";", sampling_width=None, *, correct_origin=None):
         """Export kymograph tracks to a csv file.
 
         Parameters
         ----------
         filename : str
             Filename to output kymograph tracks to.
         delimiter : str
             Which delimiter to use in the csv file.
         sampling_width : int or None
             When supplied, this will sample the source image around the kymograph track and export the summed intensity
             with the image. The value indicates the number of pixels in either direction to sum over.
+        correct_origin : bool, optional
+            Use the correct pixel origin when sampling from image. Kymotracks are defined with the
+            origin of each image pixel defined at the center. Earlier versions of the method that
+            samples photon counts around the track had a bug which assumed the origin at the edge
+            of the pixel. Setting this flag to `True` produces the correct behavior. The default is
+            set to `None` which reproduces the old behavior and results in a warning, while `False`
+            reproduces the old behavior without a warning.
         """
-        export_kymotrackgroup_to_csv(filename, self, delimiter, sampling_width)
+        export_kymotrackgroup_to_csv(
+            filename, self, delimiter, sampling_width, correct_origin=correct_origin
+        )
+
+    def _tracks_by_kymo(self):
+        """Find tracks for each `Kymo` in the group.
+
+        Returns
+        -------
+        dict of KymoTrackGroup
+            returns a dictionary where the keys are Kymos which the associated tracks
+        """
+        groups = [
+            KymoTrackGroup([track for track in self if track._kymo == kymo]) for kymo in self._kymos
+        ]
+
+        indices = [
+            [j for j, track in enumerate(self) if track._kymo == kymo] for kymo in self._kymos
+        ]
+
+        return groups, indices
+
+    @staticmethod
+    def _extract_dwelltime_data_from_groups(groups, exclude_ambiguous_dwells):
+        """Compute data needed for dwelltime analysis from a dictionary of KymoTrackGroups.
+
+        This data consists of dwelltimes and observation limits per track. Note that dwelltimes of zero
+        are automatically dropped.
+
+        Parameters
+        ----------
+        groups : iterable of KymoTrackGroup
+            An iterable which provides a sequence of KymoTrackGroup. Note that each group can only
+            have one `Kymo` associated with it.
+        exclude_ambiguous_dwells : bool
+            Determines whether to exclude dwelltimes which are not exactly determined. If `True`,
+            tracks which start in the first frame or end in the last frame of the kymograph are not
+            used in the analysis, since the exact start/stop times of the binding event are not
+            definitively known.
+
+        Returns
+        -------
+        dwelltimes : numpy.ndarray
+            Dwelltimes
+        min_obs : numpy.ndarray
+            List of minimum observation times extracted from the kymos
+        max_obs : numpy.ndarray
+            List of maximum observation time
+        removed_zeros : bool
+            Whether zeroes were dropped
+
+        Raises
+        ------
+        ValueError
+            if one of the KymoTrackGroups has more than one `Kymo` associated with it
+        """
+        removed_zeros = False
+
+        def extract_dwelltime_data(group):
+            nonlocal removed_zeros
+
+            if len(group._kymos) > 1:
+                raise ValueError("This group has more than one Kymo associated with it.")
+
+            tracks = (
+                filter(KymoTrack._check_ends_are_defined, group)
+                if exclude_ambiguous_dwells
+                else group
+            )
+            dwelltimes_sec = np.array([track.seconds[-1] - track.seconds[0] for track in tracks])
+            nonzero_dwelltimes_sec = dwelltimes_sec[dwelltimes_sec > 0]
+            removed_zeros = removed_zeros or len(nonzero_dwelltimes_sec) != len(dwelltimes_sec)
+
+            # Gracefully handle empty groups
+            if nonzero_dwelltimes_sec.size == 0:
+                return np.empty((3, 0))
+
+            min_observation_time = np.min(nonzero_dwelltimes_sec)
+            max_observation_time = group[0]._image.shape[1] * group[0]._line_time_seconds
+
+            return np.vstack(
+                list(
+                    np.broadcast(nonzero_dwelltimes_sec, min_observation_time, max_observation_time)
+                )
+            ).T
+
+        dwelltimes, min_obs, max_obs = np.hstack(
+            [extract_dwelltime_data(tracks) for tracks in groups]
+        )
+
+        return dwelltimes, min_obs, max_obs, removed_zeros
 
     def fit_binding_times(
         self, n_components, *, exclude_ambiguous_dwells=True, tol=None, max_iter=None
     ):
         """Fit the distribution of bound dwelltimes to an exponential (mixture) model.
 
         Parameters
@@ -916,49 +1198,47 @@
         tol : float
             The tolerance for optimization convergence. This parameter is forwarded as the `ftol` argument
             to `scipy.minimize(method="L-BFGS-B")`.
         max_iter : int
             The maximum number of iterations to perform. This parameter is forwarded as the `maxiter` argument
             to `scipy.minimize(method="L-BFGS-B")`.
         """
+        if not len(self):
+            raise RuntimeError("No tracks available for analysis")
 
         if n_components not in (1, 2):
             raise ValueError(
                 "Only 1- and 2-component exponential distributions are currently supported."
             )
 
-        tracks = (
-            filter(KymoTrack._check_ends_are_defined, self) if exclude_ambiguous_dwells else self
+        groups, _ = self._tracks_by_kymo()
+        dwelltimes, min_obs, max_obs, removed_zeros = self._extract_dwelltime_data_from_groups(
+            groups, exclude_ambiguous_dwells
         )
-        dwelltimes_sec = np.array([track.seconds[-1] - track.seconds[0] for track in tracks])
 
-        nonzero_dwelltimes_sec = dwelltimes_sec[dwelltimes_sec > 0]
-        if len(nonzero_dwelltimes_sec) != len(dwelltimes_sec):
+        if removed_zeros:
             warnings.warn(
                 RuntimeWarning(
                     "Some dwell times are zero. A dwell time of zero indicates that some of the "
                     "tracks were only observed in a single frame. For these samples it is not "
                     "possible to actually determine a dwell time. Therefore these samples are "
                     "dropped from the analysis. If you wish to not see this warning, filter the "
                     "tracks with `lk.filter_tracks` with a minimum length of 2 samples."
                 ),
                 stacklevel=2,
             )
 
-        if nonzero_dwelltimes_sec.size == 0:
+        if dwelltimes.size == 0:
             raise RuntimeError("No tracks available for analysis")
 
-        min_observation_time = np.min(nonzero_dwelltimes_sec)
-        max_observation_time = self[0]._image.shape[1] * self[0]._line_time_seconds
-
         return DwelltimeModel(
-            nonzero_dwelltimes_sec,
+            dwelltimes,
             n_components,
-            min_observation_time=min_observation_time,
-            max_observation_time=max_observation_time,
+            min_observation_time=min_obs,
+            max_observation_time=max_obs,
             tol=tol,
             max_iter=max_iter,
         )
 
     def _histogram_binding_events(self, kind, bins=10):
         """Make histogram of bound events.
 
@@ -1005,15 +1285,15 @@
         """
         import matplotlib.pyplot as plt
 
         counts, edges = self._histogram_binding_events(kind, bins)
         widths = np.diff(edges)
         plt.bar(edges[:-1], counts, width=widths, align="edge", **kwargs)
         plt.ylabel("Counts")
-        plt.xlabel(f"Position ({self._kymo._calibration.unit_label})")
+        plt.xlabel(f"Position ({self._calibration_info['unit_label']})")
 
     def _histogram_binding_profile(self, n_time_bins, bandwidth, n_position_points, roi=None):
         """Calculate a Kernel Density Estimate (KDE) of binding density along the tether for time bins.
 
         First the kymograph is binned along the temporal axis. In the case of non-integer `frames / bins`,
         remaining frames are discarded. Next, for each time bin, a KDE is calculated along the spatial axis.
 
@@ -1024,29 +1304,32 @@
         bandwidth : float
             KDE bandwidth; units are in the physical spatial units of the kymograph.
         n_position_points : int
             Length of the returned density array(s).
         roi: list or None
             ROI coordinates as `[[min_time, min_position], [max_time, max_position]]`.
         """
+        self._validate_single_source("Binding profile")
+        _kymo = self._kymos[0]
+
         if n_time_bins == 0:
             raise ValueError("Number of time bins must be > 0.")
         if n_position_points < 2:
             raise ValueError("Number of spatial bins must be >= 2.")
 
         if roi is None:
-            n_rows, n_frames = self._kymo.get_image(self._channel).shape
+            n_rows, n_frames = _kymo.get_image(self._channel).shape
             start_frame = 0
             min_position = 0
-            max_position = n_rows * self._kymo.pixelsize[0]
+            max_position = n_rows * _kymo.pixelsize[0]
         else:
             (min_time, min_position), (max_time, max_position) = roi
-            n_rows = np.ceil((max_position - min_position) / self._kymo.pixelsize[0])
-            n_frames = np.ceil((max_time - min_time) / self._kymo.line_time_seconds)
-            start_frame = min_time // self._kymo.line_time_seconds
+            n_rows = np.ceil((max_position - min_position) / _kymo.pixelsize[0])
+            n_frames = np.ceil((max_time - min_time) / _kymo.line_time_seconds)
+            start_frame = min_time // _kymo.line_time_seconds
 
         try:
             bin_size = n_frames // n_time_bins
             bin_edges = np.arange(start_frame, start_frame + n_frames, step=bin_size)
         except ZeroDivisionError:
             raise ValueError("Number of time bins must be <= number of frames.")
 
@@ -1147,32 +1430,54 @@
               :meth:`KymoTrack.estimate_diffusion` for more detailed information and references.
             - "ols" : Ordinary least squares. Determines the ensemble mean squared displacements for
               the entire KymoTrackGroup and estimates a diffusion constant for it. See
               :meth:`KymoTrack.estimate_diffusion` for more detailed information and references.
         max_lag : int
             Maximum number of lags to include when using the ordinary least squares method (OLS).
 
+        Raises
+        ------
+        ValueError
+            if `method == "ols"` and the source kymographs do not have the same line times
+            or pixel sizes.
+
         Warns
         -----
         RuntimeWarning
             if `method == "cve"` and the source kymograph does not have a clearly defined motion
             blur constant. As a result, the localization variance and standard error for the
             diffusion constant will not be available. If only one track is available, the standard
             error on the diffusion constant will also not be available. Estimates that are
             unavailable are returned as `np.nan`.
+        RuntimeWarning
+            if `method == "cve"` and the source kymographs do not have the same line times
+            or pixel sizes. As a result, the localization variance and variance of the localization
+            variance are not available. Estimates that are unavailable are returned as `np.nan`.
 
         References
         ----------
         .. [7] Vestergaard, C. L., Blainey, P. C., & Flyvbjerg, H. (2014). Optimal estimation of
                diffusion coefficients from single-particle trajectories. Physical Review E, 89(2),
                022726.
         """
         if method == "cve":
-            return ensemble_cve(self)
+            try:
+                self._validate_single_linetime_pixelsize()
+                is_valid = True
+            except ValueError:
+                warnings.warn(
+                    RuntimeWarning(
+                        "Localization variances cannot be reliably calculated for an ensemble of "
+                        "tracks from kymographs with different line times or pixel sizes."
+                    ),
+                )
+                is_valid = False
+            return ensemble_cve(self, calculate_localization_var=is_valid)
         elif method == "ols":
+            self._validate_single_linetime_pixelsize()
             return ensemble_ols(self, max_lag)
         else:
             raise ValueError(f'Invalid method ({method}) selected. Method must be "cve" or "ols".')
 
     def ensemble_msd(self, max_lag=None, min_count=2) -> EnsembleMSD:
         r"""This method returns the weighted average of the Mean Squared Displacement (MSD) for all
         tracks in this group.
@@ -1220,15 +1525,15 @@
                single-particle tracking. Physical Review E, 85(6), 061916.
         """
         track_msds = [
             calculate_msd_counts(np.array(track.time_idx, dtype=int), track.position, max_lag)
             for track in self._src
         ]
 
-        src_calibration = self._kymo._calibration
+        self._validate_single_linetime_pixelsize()
+
         return calculate_ensemble_msd(
             line_msds=track_msds,
-            time_step=self._kymo.line_time_seconds,
-            unit=src_calibration.unit,
-            unit_label=src_calibration.unit_label,
+            time_step=self._kymos[0].line_time_seconds,
             min_count=min_count,
+            **self._calibration_info,
         )
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/kymotracker.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/kymotracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     refine_peak_based_on_moment,
     merge_close_peaks,
     KymoPeaks,
 )
 from .detail.localization_models import GaussianLocalizationModel
 import numpy as np
 import warnings
+from itertools import chain
 
 __all__ = [
     "track_greedy",
     "track_lines",
     "filter_tracks",
     "refine_tracks_centroid",
     "refine_tracks_gaussian",
@@ -363,14 +364,32 @@
         Detected tracks on a kymograph.
     minimum_length : int
         Minimum length for the track to be accepted.
     """
     return KymoTrackGroup([track for track in tracks if len(track) >= minimum_length])
 
 
+def _apply_to_group(tracks, func, *args, **kwargs):
+    """Break a group of tracks into sets with a single source kymograph, apply `func`,
+    and rebuild group in original order.
+
+    Parameters
+    ----------
+    tracks : KymoTrackGroup
+        Tracks to apply function to
+    func : callable
+        Function to be applied to tracks
+    *args, **kwargs
+        Additional arguments supplied to `func`
+    """
+    groups, indices = tracks._tracks_by_kymo()
+    groups = [func(group, *args, **kwargs) for group in groups]
+    return KymoTrackGroup([track for _, track in sorted(zip(chain(*indices), chain(*groups)))])
+
+
 def refine_tracks_centroid(tracks, track_width=None, bias_correction=True):
     """Refine the tracks based on the brightness-weighted centroid.
 
     This function interpolates the determined tracks (in time) and then uses the pixels in the
     vicinity of the tracks to make small adjustments to the estimated location. The refinement
     correction is computed by considering the brightness weighted centroid.
 
@@ -408,24 +427,33 @@
     ----------
     .. [1] Berglund, A. J., McMahon, M. D., McClelland, J. J., & Liddle, J. A. (2008).
            Fast, bias-free algorithm for tracking single particles with variable size and
            shape. Optics express, 16(18), 14064-14075.
     """
     tracks = KymoTrackGroup(tracks) if isinstance(tracks, (list, tuple)) else tracks
 
+    if len(tracks._kymos) > 1:
+        return _apply_to_group(
+            tracks, refine_tracks_centroid, track_width=track_width, bias_correction=bias_correction
+        )
+
     if not tracks:
         return KymoTrackGroup([])
 
-    minimum_width = 3 * tracks._kymo.pixelsize[0]
+    # the existence of tracks implies there is at least one source kymo
+    # _apply_to_group ensures there is only a single source kymo at this point
+    kymo = tracks._kymos[0]
+
+    minimum_width = 3 * kymo.pixelsize[0]
     if track_width is None:
-        track_width = max(_default_track_widths[tracks._kymo._calibration.unit], minimum_width)
+        track_width = max(_default_track_widths[kymo._calibration.unit], minimum_width)
 
-    _validate_track_width(track_width, minimum_width, tracks._kymo._calibration.unit)
+    _validate_track_width(track_width, minimum_width, kymo._calibration.unit)
 
-    half_width_pixels = _to_half_kernel_size(track_width, tracks._kymo.pixelsize[0])
+    half_width_pixels = _to_half_kernel_size(track_width, kymo.pixelsize[0])
 
     interpolated_tracks = [track.interpolate() for track in tracks]
     time_idx = np.round(
         np.array(np.hstack([track.time_idx for track in interpolated_tracks]))
     ).astype(int)
     coordinate_idx = np.round(
         np.array(np.hstack([track.coordinate_idx for track in interpolated_tracks]))
@@ -481,21 +509,34 @@
     fixed_background : float
         Fixed background parameter in photons per second.
         When supplied, the background is not estimated but fixed at this value.
     """
     if overlap_strategy not in ("ignore", "skip", "multiple"):
         raise ValueError("Invalid overlap strategy selected.")
 
+    if len(tracks._kymos) > 1:
+        return _apply_to_group(
+            tracks,
+            refine_tracks_gaussian,
+            window,
+            refine_missing_frames,
+            overlap_strategy,
+            initial_sigma=initial_sigma,
+            fixed_background=fixed_background,
+        )
+
     if not tracks:
         return KymoTrackGroup([])
 
     if refine_missing_frames:
         tracks = KymoTrackGroup([track.interpolate() for track in tracks])
 
-    kymo = tracks._kymo
+    # the existence of tracks implies there is at least one source kymo
+    # _apply_to_group ensures there is only a single source kymo at this point
+    kymo = tracks._kymos[0]
     channel = tracks._channel
     image_data = kymo.get_image(channel)
 
     initial_sigma = kymo.pixelsize[0] * 1.1 if initial_sigma is None else initial_sigma
 
     full_position = np.arange(image_data.shape[0]) * kymo.pixelsize[0]
     overlap_count = 0
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/stitching.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/stitching.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/gaussian_data_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/generate_gaussian_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/kymo_data_2lines.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence.gb`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/test_sequence_no_features.gb`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v0.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v1.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/tracks_v2.csv`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/data/two_gaussians_1d.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_derived_quantities/test_msd.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,16 +291,17 @@
         determine_optimal_points(lag_idx, lag_idx**2, max_iterations=100)
 
     with pytest.warns(
         RuntimeWarning,
         match=re.escape(
             "Your tracks have missing frames. Note that this results in a poor estimate of "
             "the standard error of the estimate. To avoid this warning, you can refine "
-            "your tracks using `lk.refine_tracks_centroid()`. Please refer to "
-            "`help(lk.refine_tracks_centroid)` for more information."
+            "your tracks using `lk.refine_tracks_centroid()` or `lk.refine_tracks_gaussian()`. "
+            "Please refer to `help(lk.refine_tracks_centroid)` or `help(lk.refine_tracks_gaussian)` "
+            "for more information."
         ),
     ):
         estimate_diffusion_constant_simple(lag_idx, lag_idx**2, 1, 5, method="ols")
 
 
 @pytest.mark.parametrize(
     "diffusion,num_points,max_lag,time_step,obs_noise,diff_est,std_err_est,loc_variance",
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_gaussian_mle.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_geometry_2d.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     the original image, or that the reference to the image held by KymoTrack is a reference to a
     subset of the image, while the coordinates are still in the global coordinate system."""
     line_time = kymo_integration_test_data.line_time_seconds
     pixel_size = kymo_integration_test_data.pixelsize_um[0]
     rect = [[0.0 * line_time, 15.0 * pixel_size], [30 * line_time, 30.0 * pixel_size]]
 
     tracks = track_greedy(kymo_integration_test_data, "red", track_width=3 * pixel_size, pixel_threshold=4, rect=rect)
-    np.testing.assert_allclose(tracks[0].sample_from_image(1), [40] * np.ones(10))
+    np.testing.assert_allclose(
+        tracks[0].sample_from_image(1, correct_origin=True), [40] * np.ones(10)
+    )
 
 
 def test_kymotracker_regression_test_subset_comes_up_empty(kymo_integration_test_data):
     """Test whether we gracefully handle the case where the ROI results in no lines."""
     tracks = track_greedy(
         kymo_integration_test_data,
         "red",
@@ -62,16 +64,20 @@
     np.testing.assert_allclose(tracks[1].coordinate_idx, [21] * np.ones(10))
     np.testing.assert_allclose(tracks[0].position, [11 * pixel_size] * np.ones(10))
     np.testing.assert_allclose(tracks[1].position, [21 * pixel_size] * np.ones(10))
     np.testing.assert_allclose(tracks[0].time_idx, np.arange(10, 20))
     np.testing.assert_allclose(tracks[1].time_idx, np.arange(15, 25))
     np.testing.assert_allclose(tracks[0].seconds, np.arange(10, 20) * line_time)
     np.testing.assert_allclose(tracks[1].seconds, np.arange(15, 25) * line_time)
-    np.testing.assert_allclose(tracks[0].sample_from_image(1), [50] * np.ones(10))
-    np.testing.assert_allclose(tracks[1].sample_from_image(1), [40] * np.ones(10))
+    np.testing.assert_allclose(
+        tracks[0].sample_from_image(1, correct_origin=True), [50] * np.ones(10)
+    )
+    np.testing.assert_allclose(
+        tracks[1].sample_from_image(1, correct_origin=True), [40] * np.ones(10)
+    )
 
     rect = [[0.0 * line_time, 15.0 * pixel_size], [30 * line_time, 30.0 * pixel_size]]
     tracks = track_greedy(test_data, "red", track_width=3 * pixel_size, pixel_threshold=4, rect=rect)
     np.testing.assert_allclose(tracks[0].coordinate_idx, [21] * np.ones(10))
     np.testing.assert_allclose(tracks[0].time_idx, np.arange(15, 25))
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_io.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import pytest
 import numpy as np
 import inspect
 import re
 import io
 from pathlib import Path
+from copy import copy
+from lumicks.pylake.kymo import _kymo_from_array
 from lumicks.pylake.kymotracker.kymotrack import (
     KymoTrack,
     KymoTrackGroup,
     import_kymotrackgroup_from_csv,
 )
 from lumicks.pylake.tests.data.mock_confocal import generate_kymo
 
@@ -84,15 +86,15 @@
             KymoTrack(np.array(time_idx), np.array(position_idx), kymo, "red")
             for time_idx, position_idx in track_coordinates
         ]
     )
 
     # Test round trip through the API
     testfile = f"{tmpdir_factory.mktemp('pylake')}/test.csv"
-    tracks.save(testfile, delimiter, sampling_width)
+    tracks.save(testfile, delimiter, sampling_width, correct_origin=True)
     imported_tracks = import_kymotrackgroup_from_csv(testfile, kymo, "red", delimiter=delimiter)
     data, pylake_version, csv_version = read_txt(testfile, delimiter)
 
     compare_kymotrack_group(tracks, imported_tracks)
 
     for track1, time in zip(tracks, data["time (seconds)"]):
         np.testing.assert_allclose(track1.seconds, time)
@@ -104,19 +106,44 @@
         assert len([key for key in data.keys() if "counts" in key]) == 0
     else:
         count_field = [key for key in data.keys() if "counts" in key][0]
         for track1, cnt in zip(tracks, data[count_field]):
             np.testing.assert_allclose([sampling_outcome] * len(track1.coordinate_idx), cnt)
 
 
+def test_export_sources(tmpdir_factory):
+    kymo1 = _kymo_from_array(np.random.poisson(5, (5, 5, 3)), "rgb", 1e-4, start=20e9)
+    kymo2 = copy(kymo1)
+    tracks1 = KymoTrackGroup([KymoTrack(np.arange(3), np.arange(3), kymo1, "red")])
+    tracks2 = KymoTrackGroup([KymoTrack(np.arange(5), np.arange(5), kymo2, "red")])
+    tracks3 = tracks1 + tracks2
+
+    testfile = f"{tmpdir_factory.mktemp('pylake')}/failed_test.csv"
+
+    # can export group with single source
+    tracks1.save(testfile, ";")
+
+    # cannot export group with more than one source
+    with pytest.raises(
+        NotImplementedError,
+        match=re.escape(
+            "Exporting a group with tracks from more than a single source kymograph is not supported. "
+            "This group contains tracks from 2 source kymographs."
+        ),
+    ):
+        tracks3.save(testfile, ";")
+
+
 @pytest.mark.parametrize(
-    "delimiter, sampling_width",
-    [[";", 0], [",", 0], [";", 1], [";", None]],
+    "delimiter, sampling_width, correct_origin",
+    [[";", 0, True], [",", 0, True], [";", 1, True], [";", None, True]],
 )
-def test_roundtrip_without_file(delimiter, sampling_width, kymo_integration_test_data):
+def test_roundtrip_without_file(
+    delimiter, sampling_width, correct_origin, kymo_integration_test_data
+):
     # Validate that this also works when providing a string handle (this is the API LV uses).
 
     def get_args(func):
         return list(inspect.signature(func).parameters.keys())
 
     # This helps us ensure that if we get additional arguments to this function, we don't forget to
     # add them to the parametrization here.
@@ -133,15 +160,17 @@
         [
             KymoTrack(np.array(time_idx), np.array(position_idx), kymo_integration_test_data, "red")
             for time_idx, position_idx in track_coordinates
         ]
     )
 
     with io.StringIO() as s:
-        tracks.save(s, delimiter=delimiter, sampling_width=sampling_width)
+        tracks.save(
+            s, delimiter=delimiter, sampling_width=sampling_width, correct_origin=correct_origin
+        )
         string_representation = s.getvalue()
 
     with io.StringIO(string_representation) as s:
         read_tracks = import_kymotrackgroup_from_csv(
             s, kymo_integration_test_data, "green", delimiter=delimiter
         )
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_kymotrack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import pytest
 import matplotlib.pyplot as plt
+from copy import copy
 from lumicks.pylake.kymotracker.kymotrack import *
 from lumicks.pylake.kymotracker.kymotracker import _to_half_kernel_size
 from lumicks.pylake.kymotracker.detail.localization_models import *
-from lumicks.pylake import filter_tracks
 from lumicks.pylake.kymo import _kymo_from_array
 from ...tests.data.mock_confocal import generate_kymo
 
 
 def test_kymo_track(blank_kymo):
     k1 = KymoTrack(np.array([1, 2, 3]), np.array([2, 3, 4]), blank_kymo, "red")
     np.testing.assert_allclose(k1[1], [2, 3])
@@ -221,16 +221,17 @@
 
     tracks = KymoTrackGroup([k1, k2, k3])
     tracks.extend(k4)
     assert [k for k in tracks] == [k1, k2, k3, k4]
 
     tracks = KymoTrackGroup([k1, k2, k3])
 
-    duplicate_error = "Cannot extend this KymoTrackGroup with a KymoTrack that is already " \
-                      "part of the group"
+    duplicate_error = (
+        "Cannot extend this KymoTrackGroup with a KymoTrack that is already part of the group"
+    )
 
     for extension, exception, error in (
         (5, TypeError, "You can only extend a KymoTrackGroup with a KymoTrackGroup or KymoTrack"),
         (KymoTrackGroup([k3, k4]), ValueError, duplicate_error),
         (k3, ValueError, duplicate_error),
     ):
         with pytest.raises(exception, match=error):
@@ -241,15 +242,15 @@
 
 
 def test_kymotrack_group(blank_kymo):
     def validate_same(kymoline_group, ref_list, source_items, ref_kymo):
         assert [k for k in kymoline_group] == ref_list
         assert id(kymoline_group) not in (id(s) for s in source_items)
         if ref_kymo:
-            assert id(kymoline_group._kymo) == id(ref_kymo)
+            assert id(kymoline_group._kymos[0]) == id(ref_kymo)
 
     k1 = KymoTrack(np.array([1, 2, 3]), np.array([2, 3, 4]), blank_kymo, "red")
     k2 = KymoTrack(np.array([2, 3, 4]), np.array([3, 4, 5]), blank_kymo, "red")
     k3 = KymoTrack(np.array([3, 4, 5]), np.array([4, 5, 6]), blank_kymo, "red")
     k4 = KymoTrack(np.array([4, 5, 6]), np.array([5, 6, 7]), blank_kymo, "red")
 
     tracks1 = KymoTrackGroup([k1, k2])
@@ -533,120 +534,151 @@
 
 
 def test_empty_binding_histogram():
     with pytest.raises(RuntimeError, match="No tracks available for analysis"):
         KymoTrackGroup([]).plot_binding_histogram("binding")
 
 
-def test_kymotrackgroup_source_kymo():
-    # test that all tracks are from the same source Kymo and tracked
-    # on the same color channel
-
-    image = np.random.randint(0, 20, size=(10, 10, 3))
-    kwargs = dict(line_time_seconds=10e-3, start=np.int64(20e9), pixel_size_um=0.05, name="test")
-    kymos = [_kymo_from_array(image, "rgb", **kwargs) for _ in range(2)]
-
-    time_idx = ([1, 2, 3], [4, 6, 7], [1, 2, 3], [4, 6, 7])
-
-    pos_idx = ([4, 5, 6], [1, 7, 7], [1, 2, 3], [1, 2, 3])
-
-    green_tracks_a = [KymoTrack(t, p, kymos[0], "green") for t, p in zip(time_idx, pos_idx)]
-    green_tracks_b = [KymoTrack(t, p, kymos[1], "green") for t, p in zip(time_idx, pos_idx)]
-
-    red_tracks_a = [KymoTrack(t, p, kymos[0], "red") for t, p in zip(time_idx, pos_idx)]
-    red_tracks_b = [KymoTrack(t, p, kymos[1], "red") for t, p in zip(time_idx, pos_idx)]
-
-    # test proper group construction
-    tracks_a = KymoTrackGroup(green_tracks_a[:2])
-    assert len(tracks_a) == 2
-
-    tracks_b = KymoTrackGroup(green_tracks_b[:2])
-    assert len(tracks_b) == 2
+def test_kymotrackgroup_copy(blank_kymo):
+    k1 = KymoTrack(np.array([1, 2, 3]), np.array([1, 1, 1]), blank_kymo, "red")
+    k2 = KymoTrack(np.array([6, 7, 8]), np.array([2, 2, 2]), blank_kymo, "red")
+    group = KymoTrackGroup([k1, k2])
+    assert id(group._src) != id(copy(group)._src)
 
-    assert id(tracks_a._kymo) == id(kymos[0])
-    assert tracks_a._channel == "green"
 
-    # test empty result
-    tracks_empty = KymoTrackGroup([])
-    assert len(tracks_empty) == 0
+def test_kymotrack_split(blank_kymo):
+    k1 = KymoTrack(np.array([1, 2, 3]), np.array([1, 3, 4]), blank_kymo, "red")
+    k2, k3 = k1._split(1)
+    np.testing.assert_allclose(k2.position, [1])
+    np.testing.assert_allclose(k3.position, [3, 4])
+
+    k2, k3 = k1._split(2)
+    np.testing.assert_allclose(k2.position, [1, 3])
+    np.testing.assert_allclose(k3.position, [4])
+
+    # Test corner cases
+    for split_point in [-1, 0, 3]:
+        with pytest.raises(ValueError, match="Invalid split point"):
+            k1._split(split_point)
+
+
+def test_kymotrackgroup_split(blank_kymo):
+    k1 = KymoTrack(np.array([1, 2, 3]), np.array([1, 3, 4]), blank_kymo, "red")
+    k2 = KymoTrack(np.array([1, 2, 3]), np.array([8, 9, 11]), blank_kymo, "red")
 
-    tracks_empty = filter_tracks(tracks_a, 5)
-    assert len(tracks_empty) == 0
+    group = KymoTrackGroup([k1, k2])
+    assert len(group) == 2
+    group._split_track(k1, 1, min_length=1)
+    assert len(group) == 3
+    np.testing.assert_allclose(group[-2].position, [1])
+    np.testing.assert_allclose(group[-1].position, [3, 4])
+    group._split_track(k2, 2, min_length=1)
+    assert len(group) == 4
+    np.testing.assert_allclose(group[-2].position, [8, 9])
+    np.testing.assert_allclose(group[-1].position, [11])
 
-    with pytest.raises(
-        RuntimeError,
-        match=re.escape("No kymo associated with this empty group (no tracks available)"),
-    ):
-        tracks_empty._kymo
 
-    with pytest.raises(
-        RuntimeError,
-        match=re.escape("No channel associated with this empty group (no tracks available)"),
-    ):
-        tracks_empty._channel
+@pytest.mark.parametrize(
+    "split, filter, filtered",
+    [
+        (5, 5, 0),
+        (4, 5, 1),
+        (6, 5, 1),
+        (4, 4, 0),
+    ],
+)
+def test_kymotrackgroup_split_filter(blank_kymo, split, filter, filtered):
+    k1 = KymoTrack(np.arange(10), np.arange(10), blank_kymo, "red")
+    group = KymoTrackGroup([k1])
 
-    # cannot make group from different source kymos
-    with pytest.raises(ValueError, match="All tracks must have the same source kymograph."):
-        KymoTrackGroup([*green_tracks_a, *green_tracks_b])
-
-    # test extend with single track
-    tracks_a.extend(green_tracks_a[2])
-    assert len(tracks_a) == 3
-
-    # test extend with KymoTrackGroup
-    tracks_a.extend(KymoTrackGroup(green_tracks_a[-1:]))
-    assert len(tracks_a) == 4
-
-    # cannot extend with different source kymos
-    with pytest.raises(ValueError, match="All tracks must have the same source kymograph."):
-        tracks_a.extend(tracks_b)
-
-    # test extend from empty group
-    tracks_empty = KymoTrackGroup([])
-    tracks_empty.extend(tracks_a)
-    assert len(tracks_empty) == 4
-
-    # cannot make group from different color channels
-    with pytest.raises(ValueError, match="All tracks must be from the same color channel."):
-        KymoTrackGroup([*green_tracks_a, *red_tracks_a])
-
-    # cannot extend with different color channels
-    with pytest.raises(ValueError, match="All tracks must be from the same color channel."):
-        tracks_a.extend(red_tracks_a[0])
-    with pytest.raises(ValueError, match="All tracks must be from the same color channel."):
-        tracks_a.extend(KymoTrackGroup(red_tracks_a))
-
-
-def test_kymotrackgroup_copy(blank_kymo):
-    k1 = KymoTrack(np.array([1, 2, 3]), np.array([1, 1, 1]), blank_kymo, "red")
-    k2 = KymoTrack(np.array([6, 7, 8]), np.array([2, 2, 2]), blank_kymo, "red")
-    group = KymoTrackGroup([k1, k2])
-    assert id(group._src) != id(copy(group)._src)
+    group._split_track(k1, split, min_length=filter)
+    assert len(group) == 2 - filtered
 
 
 def test_kymotrack_concat_gaussians(blank_kymo):
     k1 = KymoTrack(np.array([1, 2, 3]), np.array([1, 1, 1]), blank_kymo, "red")
+    k1g = KymoTrack(
+        np.array([1, 2, 3]),
+        GaussianLocalizationModel(
+            np.full(3, 2), np.full(3, 7), np.full(3, 0.5), np.ones(3), np.full(3, False)
+        ),
+        blank_kymo,
+        "red",
+    )
     k2 = KymoTrack(
         np.array([6, 7, 8]),
         GaussianLocalizationModel(
             np.full(3, 2), np.full(3, 7), np.full(3, 0.5), np.ones(3), np.full(3, False)
         ),
         blank_kymo,
         "red",
     )
     group = KymoTrackGroup([k1, k2])
 
     assert isinstance(k1._localization, LocalizationModel)
     assert isinstance(k2._localization, GaussianLocalizationModel)
 
-    # test merging clears gaussian parameters
+    # test merging gaussian and non-gaussian localized lines clears gaussian parameters
     group._merge_tracks(k1, 2, k2, 2)
     assert len(group) == 1
     assert isinstance(group[0]._localization, LocalizationModel)
 
+    # test whether merging two gaussian localized lines preserves the localization
+    group = KymoTrackGroup([k1g, k2])
+    group._merge_tracks(k1g, 2, k2, 2)
+    assert len(group) == 1
+    assert isinstance(group[0]._localization, GaussianLocalizationModel)
+
+
+@pytest.mark.parametrize("num_pixels, pixelsize_um", [(10, 0.1), (15, 0.2)])
+def test_kymotrack_flip(num_pixels, pixelsize_um):
+    kymo = _kymo_from_array(
+        np.ones((num_pixels, 10)), "r", line_time_seconds=1e-2, pixel_size_um=pixelsize_um
+    )
+    coords = np.arange(1.0, 4.0)
+
+    track = KymoTrack([1, 2, 3], coords / pixelsize_um, kymo, "red")
+    flipped_kymo = kymo.flip()
+    flipped_track = track._flip(flipped_kymo)
+    assert id(track) != id(flipped_track)
+
+    center_to_center_um = pixelsize_um * (num_pixels - 1)
+    np.testing.assert_allclose(flipped_track.position, center_to_center_um - coords)
+    np.testing.assert_equal(flipped_track.time_idx, track.time_idx)
+    assert id(flipped_track._kymo) == id(flipped_kymo)
+    assert flipped_track._channel == track._channel
+
+    np.testing.assert_allclose(flipped_track._flip(kymo).position, track.position)
+
+
+def test_kymotrackgroup_flip():
+    kymo = _kymo_from_array(np.ones((5, 10)), "r", line_time_seconds=1e-2, pixel_size_um=1.0)
+    coords = np.arange(1.0, 4.0)
+
+    tracks = KymoTrackGroup([KymoTrack([1, 2, 3], coords, kymo, "red") for _ in range(3)])
+    flipped_tracks = tracks._flip()
+    assert all([id(t._kymo) == id(flipped_tracks[0]._kymo) for t in flipped_tracks])
+    for track, flipped_track in zip(tracks, flipped_tracks):
+        np.testing.assert_allclose(track._flip(kymo.flip()).position, flipped_track.position)
+
+    tracks2 = tracks + KymoTrackGroup([KymoTrack([], [], copy(kymo), "red")])
+    with pytest.raises(
+        NotImplementedError,
+        match=re.escape(
+            "Flipping is not supported. This group contains tracks from 2 source kymographs."
+        ),
+    ):
+        tracks2._flip()
+
+    with pytest.raises(
+        RuntimeError,
+        match=re.escape("No kymo associated with this empty group (no tracks available)"),
+    ):
+        KymoTrackGroup([])._flip()
+
 
 def test_binding_profile_histogram():
     kymo = generate_kymo(
         "",
         np.ones((10, 10)),
         pixel_size_nm=1000,
         start=np.int64(20e9),
@@ -700,14 +732,32 @@
     with pytest.raises(ValueError, match="Number of time bins must be <= number of frames."):
         tracks._histogram_binding_profile(11, 0.2, 4)
 
     # no bins requested
     with pytest.raises(ValueError, match="Number of time bins must be > 0."):
         tracks._histogram_binding_profile(0, 0.2, 4)
 
+    # disallowed for multiple source kymos
+    combined_tracks = tracks + KymoTrackGroup(
+        [KymoTrack(np.array([7, 8, 9]), np.array([1, 1, 1]), copy(kymo), "red")]
+    )
+    with pytest.raises(
+        NotImplementedError,
+        match=(
+            r"Binding profile is not supported. This group contains tracks from 2 source kymographs."
+        ),
+    ):
+        combined_tracks._histogram_binding_profile(n_time_bins=1, bandwidth=1, n_position_points=10)
+
+    with pytest.raises(
+        RuntimeError,
+        match=re.escape("No kymo associated with this empty group (no tracks available)"),
+    ):
+        KymoTrackGroup([])._histogram_binding_profile(3, 0.2, 4)
+
 
 def test_fit_binding_times(blank_kymo):
     k1 = KymoTrack(np.array([0, 1, 2]), np.zeros(3), blank_kymo, "red")
     k2 = KymoTrack(np.array([2, 3, 4, 5, 6]), np.zeros(5), blank_kymo, "red")
     k3 = KymoTrack(np.array([3, 4, 5]), np.zeros(3), blank_kymo, "red")
     k4 = KymoTrack(np.array([8, 9]), np.zeros(2), blank_kymo, "red")
 
@@ -719,16 +769,15 @@
     dwells = tracks.fit_binding_times(1, exclude_ambiguous_dwells=False)
     np.testing.assert_allclose(dwells.lifetimes, [1.25710457])
 
 
 def test_fit_binding_times_nonzero(blank_kymo):
     k1 = KymoTrack(np.array([2]), np.zeros(3), blank_kymo, "red")
     k2, k3, k4, k5 = (
-        KymoTrack(np.array([2, 3, 4, 5, 6]), np.zeros(5), blank_kymo, "red")
-        for _ in range(4)
+        KymoTrack(np.array([2, 3, 4, 5, 6]), np.zeros(5), blank_kymo, "red") for _ in range(4)
     )
     tracks = KymoTrackGroup([k1, k2, k3, k4, k5])
 
     with pytest.warns(
         RuntimeWarning,
         match=r"Some dwell times are zero. A dwell time of zero indicates that some of the tracks "
         r"were only observed in a single frame. For these samples it is not possible to "
@@ -743,14 +792,104 @@
 
 
 def test_fit_binding_times_empty():
     with pytest.raises(RuntimeError, match="No tracks available for analysis"):
         KymoTrackGroup([]).fit_binding_times(1)
 
 
+def test_multi_kymo_dwell():
+    kymos = [
+        _kymo_from_array(np.zeros((10, 10, 3)), "rgb", line_time_seconds=time, pixel_size_um=size)
+        for time, size in ((10e-4, 0.05), (10e-3, 0.1))
+    ]
+
+    k1 = KymoTrack(np.array([1, 2, 3]), np.array([1, 2, 3]), kymos[0], "red")
+    k2 = KymoTrack(np.array([2, 3, 4, 5]), np.array([2, 3, 4, 5]), kymos[0], "red")
+    k3 = KymoTrack(np.array([3, 4, 5]), np.array([3, 4, 5]), kymos[1], "red")
+    k4 = KymoTrack(np.array([4, 5, 6]), np.array([4, 5, 6]), kymos[1], "red")
+    k5 = KymoTrack(np.array([7]), np.array([7]), kymos[1], "red")
+
+    # Normal use case
+    dwell, obs_min, obs_max, removed_zeroes = KymoTrackGroup._extract_dwelltime_data_from_groups(
+        [KymoTrackGroup([k1, k2]), KymoTrackGroup([k3, k4])], False
+    )
+    np.testing.assert_allclose(dwell, [0.002, 0.003, 0.02, 0.02])
+    np.testing.assert_allclose(obs_min, [0.002, 0.002, 0.02, 0.02])
+    np.testing.assert_allclose(obs_max, [0.01, 0.01, 0.1, 0.1])
+    assert removed_zeroes is False
+
+    # Drop one "empty" dwell
+    dwell, obs_min, obs_max, removed_zeroes = KymoTrackGroup._extract_dwelltime_data_from_groups(
+        [KymoTrackGroup([k1, k2]), KymoTrackGroup([k3, k4, k5])], False
+    )
+    np.testing.assert_allclose(dwell, [0.002, 0.003, 0.02, 0.02])
+    np.testing.assert_allclose(obs_min, [0.002, 0.002, 0.02, 0.02])
+    np.testing.assert_allclose(obs_max, [0.01, 0.01, 0.1, 0.1])
+    assert removed_zeroes is True
+
+    # Test with empty group
+    dwell, obs_min, obs_max, removed_zeroes = KymoTrackGroup._extract_dwelltime_data_from_groups(
+        [KymoTrackGroup([k1, k2]), KymoTrackGroup([])], False
+    )
+    np.testing.assert_allclose(dwell, [0.002, 0.003])
+    np.testing.assert_allclose(obs_min, [0.002, 0.002])
+    np.testing.assert_allclose(obs_max, [0.01, 0.01])
+    assert removed_zeroes is False
+
+    # Test with group that is empty after filtering
+    dwell, obs_min, obs_max, removed_zeroes = KymoTrackGroup._extract_dwelltime_data_from_groups(
+        [KymoTrackGroup([k1, k2]), KymoTrackGroup([k5])], False
+    )
+    np.testing.assert_allclose(dwell, [0.002, 0.003])
+    np.testing.assert_allclose(obs_min, [0.002, 0.002])
+    np.testing.assert_allclose(obs_max, [0.01, 0.01])
+    assert removed_zeroes is True
+
+    dwell, obs_min, obs_max, removed_zeroes = KymoTrackGroup._extract_dwelltime_data_from_groups(
+        [KymoTrackGroup([k5]), KymoTrackGroup([k5])], False
+    )
+    np.testing.assert_allclose(dwell, [])
+    np.testing.assert_allclose(obs_min, [])
+    np.testing.assert_allclose(obs_max, [])
+    assert removed_zeroes is True
+
+
+def test_multi_kymo_dwelltime_analysis():
+    """This test tests only the happy path since others test more specific edge cases"""
+    np.random.seed(123)
+
+    shared_args = {
+        "image": np.empty((1, 5000, 3)),
+        "color_format": "rgb",
+        "start": np.int64(20e9),
+        "pixel_size_um": 2,
+    }
+
+    kymo1 = _kymo_from_array(**shared_args, line_time_seconds=0.01)
+    kymo2 = _kymo_from_array(**shared_args, line_time_seconds=0.02)
+    args = [np.array([1.0, 1.0]), kymo1, "red"]
+    group1 = KymoTrackGroup(
+        [
+            KymoTrack(np.array([1, int(round(t / kymo1.line_time_seconds)) + 1]), *args)
+            for t in np.random.exponential(2, size=(200,))
+        ],
+    )
+    args = [np.array([1.0, 1.0]), kymo2, "red"]
+    group2 = KymoTrackGroup(
+        [
+            KymoTrack(np.array([1, int(round(t / kymo2.line_time_seconds)) + 1]), *args)
+            for t in np.random.exponential(6, size=(200,))
+        ],
+    )
+
+    model = (group1 + group2).fit_binding_times(2, tol=1e-16)
+    np.testing.assert_allclose(model.lifetimes, (2.05754716, 6.89790037))
+    np.testing.assert_allclose(model.amplitudes, (0.61360417, 0.38639583))
+
+
 @pytest.mark.parametrize("method,max_lags", [("ols", 2), ("ols", None), ("gls", 2), ("gls", None)])
 def test_kymotrack_group_diffusion(blank_kymo, method, max_lags):
     """Tests whether we can call this function at the diffusion level"""
     kymotracks = KymoTrackGroup(
         [
             KymoTrack(time_idx, coordinate, blank_kymo, "red")
             for (time_idx, coordinate) in (
@@ -964,28 +1103,24 @@
 
 
 def test_ensemble_api(blank_kymo):
     """Test whether API arguments are forwarded"""
     short_tracks = [
         KymoTrack(np.arange(1, 6), np.arange(1, 6), blank_kymo, "red") for _ in range(3)
     ]
-    long_tracks = [
-        KymoTrack(np.arange(1, 7), np.arange(1, 7), blank_kymo, "red")
-        for _ in range(2)
-    ]
+    long_tracks = [KymoTrack(np.arange(1, 7), np.arange(1, 7), blank_kymo, "red") for _ in range(2)]
     tracks = KymoTrackGroup(short_tracks + long_tracks)
 
     assert len(tracks.ensemble_msd(3).lags) == 3
     assert len(tracks.ensemble_msd(100, 3).lags) == 4
     assert len(tracks.ensemble_msd(100, 2).lags) == 5
 
     # Because of the gaps in this track, we will be missing lags 1 and 3
     gap_tracks = [
-        KymoTrack(np.array([1, 3, 5]), np.array([1, 3, 5]), blank_kymo, "red")
-        for _ in range(3)
+        KymoTrack(np.array([1, 3, 5]), np.array([1, 3, 5]), blank_kymo, "red") for _ in range(3)
     ]
     tracks = KymoTrackGroup(short_tracks[0:2] + gap_tracks)
     np.testing.assert_allclose(tracks.ensemble_msd(100, 3).lags, [2, 4])
     np.testing.assert_allclose(tracks.ensemble_msd(100, 3).msd, [4.0, 16.0])
     np.testing.assert_allclose(tracks.ensemble_msd(100, 2).lags, [1, 2, 3, 4])
     np.testing.assert_allclose(tracks.ensemble_msd(100, 2).msd, [1.0, 4.0, 9.0, 16.0])
 
@@ -1018,18 +1153,21 @@
     # Consistency check
     single_group_msd = KymoTrackGroup([kymotracks[0]]).ensemble_diffusion("cve")
     single_track_msd = kymotracks[0].estimate_diffusion("cve")
     np.testing.assert_allclose(single_group_msd.value, single_track_msd.value)
     np.testing.assert_allclose(single_group_msd.std_err, single_track_msd.std_err)
 
 
-@pytest.mark.parametrize("max_lag, diffusion_ref, std_err_ref, localization_var_ref", [
-    (None, 0.44567901234567886, 0.27564925652921307, -0.17827160493827154),
-    (4, 0.3030617283950619, 0.2895503367634419, 0.08913580246913569),
-])
+@pytest.mark.parametrize(
+    "max_lag, diffusion_ref, std_err_ref, localization_var_ref",
+    [
+        (None, 0.44567901234567886, 0.27564925652921307, -0.17827160493827154),
+        (4, 0.3030617283950619, 0.2895503367634419, 0.08913580246913569),
+    ],
+)
 def test_ensemble_ols(blank_kymo, max_lag, diffusion_ref, std_err_ref, localization_var_ref):
     """Tests the ensemble diffusion estimate"""
     kymotracks = KymoTrackGroup(
         [
             KymoTrack(time_idx, coordinate, blank_kymo, "red")
             for (time_idx, coordinate) in (
                 (np.arange(1, 6), np.array([-1.0, 1.0, -1.0, -3.0, -5.0]) / 2),
@@ -1046,29 +1184,118 @@
     assert ensemble_diffusion.variance_of_localization_variance is None
     np.testing.assert_allclose(ensemble_diffusion.num_points, 15)
     assert ensemble_diffusion.method == "ensemble ols"
     assert ensemble_diffusion.unit == "um^2 / s"
     assert ensemble_diffusion._unit_label == "$\\mu$m$^2$/s"
 
 
+@pytest.mark.parametrize("max_lag", [None, 4])
+def test_ensemble_ols_multiple_sources(blank_kymo, max_lag):
+    """Tests the happy path for OLS ensemble diffusion estimate with multiple source kymos."""
+    groups = [
+        KymoTrackGroup(
+            [
+                KymoTrack(time_idx, coordinate, kymo, "red")
+                for (time_idx, coordinate) in (
+                    (np.arange(1, 6), np.array([-1.0, 1.0, -1.0, -3.0, -5.0]) / 2),
+                    (np.arange(1, 6), np.array([-1.0, 1.0, -1.0, -3.0, -5.0]) / 3),
+                    (np.arange(1, 6), np.array([-1.0, 1.0, -1.0, -3.0, -5.0]) / 5),
+                )
+            ]
+        )
+        for kymo in (blank_kymo, copy(blank_kymo))
+    ]
+    assert id(groups[0]._kymos[0]) != id(groups[1]._kymos[0])
+
+    tracks = groups[0][:2] + groups[1][2]
+    assert len(tracks._kymos) == 2
+
+    ref_ensemble_diffusion = groups[0].ensemble_diffusion("ols", max_lag=max_lag)
+    ensemble_diffusion = tracks.ensemble_diffusion("ols", max_lag=max_lag)
+
+    np.testing.assert_allclose(ensemble_diffusion.value, ref_ensemble_diffusion.value)
+    np.testing.assert_allclose(ensemble_diffusion.std_err, ref_ensemble_diffusion.std_err)
+    np.testing.assert_allclose(
+        ensemble_diffusion.localization_variance, ref_ensemble_diffusion.localization_variance
+    )
+    assert ensemble_diffusion.variance_of_localization_variance is None
+    np.testing.assert_allclose(ensemble_diffusion.num_points, 15)
+    assert ensemble_diffusion.method == "ensemble ols"
+    assert ensemble_diffusion.unit == "um^2 / s"
+    assert ensemble_diffusion._unit_label == "$\\mu$m$^2$/s"
+
+
 def test_invalid_ensemble_diffusion(blank_kymo):
     """Tests whether we can call this function at the diffusion level"""
     kymotracks = KymoTrackGroup([KymoTrack([], [], blank_kymo, "red")])
     with pytest.raises(ValueError, match=re.escape("Invalid method (egg) selected")):
         kymotracks.ensemble_diffusion("egg")
 
 
+def test_ensemble_diffusion_different_attributes():
+    line_times = (1, 0.5)
+    pixel_sizes = (0.1, 0.05)
+    kwargs = [{"line_time_seconds": t, "pixel_size_um": s} for t in line_times for s in pixel_sizes]
+    kymos = [_kymo_from_array(np.random.poisson(5, (25, 25, 3)), "rgb", **k) for k in kwargs]
+    tracks = [
+        KymoTrackGroup(
+            [KymoTrack(np.arange(5), np.random.uniform(3, 5, 5), k, "green") for _ in range(5)]
+        )
+        for k in kymos
+    ]
+
+    error_messages = {
+        "line times": re.escape(
+            "All source kymographs must have the same line times, got [0.5, 1] seconds."
+        ),
+        "pixel sizes": re.escape(
+            "All source kymographs must have the same pixel sizes, got [0.05, 0.1] um."
+        ),
+        "both": re.escape(
+            "All source kymographs must have the same line times, got [0.5, 1] seconds. "
+            "All source kymographs must have the same pixel sizes, got [0.05, 0.1] um."
+        ),
+    }
+
+    combo_tracks = tracks[0] + tracks[1]
+    with pytest.raises(ValueError, match=error_messages["pixel sizes"]):
+        combo_tracks.ensemble_msd(max_lag=3)
+    with pytest.raises(ValueError, match=error_messages["pixel sizes"]):
+        combo_tracks.ensemble_diffusion(method="ols")
+
+    combo_tracks = tracks[0] + tracks[2]
+    with pytest.raises(ValueError, match=error_messages["line times"]):
+        combo_tracks.ensemble_msd(max_lag=3)
+    with pytest.raises(ValueError, match=error_messages["line times"]):
+        combo_tracks.ensemble_diffusion(method="ols")
+
+    combo_tracks = tracks[0] + tracks[3]
+    with pytest.raises(ValueError, match=error_messages["both"]):
+        combo_tracks.ensemble_msd(max_lag=3)
+    with pytest.raises(ValueError, match=error_messages["both"]):
+        combo_tracks.ensemble_diffusion(method="ols")
+
+    with pytest.warns(
+        RuntimeWarning,
+        match=(
+            "Localization variances cannot be reliably calculated for an ensemble of tracks from "
+            "kymographs with different line times or pixel sizes."
+        ),
+    ):
+        combo_tracks.ensemble_diffusion(method="cve")
+
+
 @pytest.mark.parametrize(
     "window, pixelsize, result",
     [
         # fmt:off
         (1.0, 1.0, 0), (2.0, 1.0, 1), (3.0, 1.0, 1), (3.01, 1.0, 2), (4.0, 1.0, 2), (4.99, 1.0, 2),
         (1.0, 2.0, 0), (2.0, 2.0, 0), (6.0, 2.0, 1), (6.01, 2.0, 2), (7.0, 2.0, 2), (7.99, 2.0, 2),
         # fmt:on
-    ]
+    ],
 )
 def test_half_kernel(window, pixelsize, result):
     assert _to_half_kernel_size(window, pixelsize) == result
 
 
 def test_integral_times_kymotrack(blank_kymo):
     with pytest.raises(TypeError, match="Time indices should be of integer type, got float64"):
@@ -1089,12 +1316,12 @@
         estimate = track.estimate_diffusion("cve")
         assert np.isnan(estimate.std_err)
         assert np.isnan(estimate.localization_variance)
 
     with pytest.raises(
         ValueError,
         match="Cannot compute diffusion constant reliably for a kymograph that does not"
-              "have a clearly defined motion blur constant and the localization variance "
-              "is provided. Omit the localization variance to calculate a diffusion "
-              "constant.",
+        "have a clearly defined motion blur constant and the localization variance "
+        "is provided. Omit the localization variance to calculate a diffusion "
+        "constant.",
     ):
         track.estimate_diffusion("cve", localization_variance=1)
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_lines_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,28 +111,34 @@
     the original image, or that the reference to the image held by KymoLine is a reference to a
     subset of the image, while the coordinates are still in the global coordinate system."""
     line_time = kymo_integration_test_data.line_time_seconds
     pixel_size = kymo_integration_test_data.pixelsize_um[0]
     rect = [[0.0 * line_time, 15.0 * pixel_size], [30 * line_time, 30.0 * pixel_size]]
 
     lines = track_lines(kymo_integration_test_data, "red", 3 * pixel_size, 4, rect=rect)
-    np.testing.assert_allclose(np.sum(lines[0].sample_from_image(1)), 40 * 10 + 6)
+    np.testing.assert_allclose(
+        np.sum(lines[0].sample_from_image(1, correct_origin=True)), 40 * 10 + 6
+    )
 
 
 def test_kymotracker_lines_algorithm_integration_tests(kymo_integration_test_data):
     line_time = kymo_integration_test_data.line_time_seconds
     pixel_size = kymo_integration_test_data.pixelsize_um[0]
 
     lines = track_lines(kymo_integration_test_data, "red", 3 * pixel_size, 4)
     np.testing.assert_allclose(lines[0].coordinate_idx, [11] * len(lines[0].coordinate_idx))
     np.testing.assert_allclose(lines[1].coordinate_idx, [21] * len(lines[1].coordinate_idx))
     np.testing.assert_allclose(lines[0].time_idx, np.arange(9, 21))
     np.testing.assert_allclose(lines[1].time_idx, np.arange(14, 26))
-    np.testing.assert_allclose(np.sum(lines[0].sample_from_image(1)), 50 * 10 + 6)
-    np.testing.assert_allclose(np.sum(lines[1].sample_from_image(1)), 40 * 10 + 6)
+    np.testing.assert_allclose(
+        np.sum(lines[0].sample_from_image(1, correct_origin=True)), 50 * 10 + 6
+    )
+    np.testing.assert_allclose(
+        np.sum(lines[1].sample_from_image(1, correct_origin=True)), 40 * 10 + 6
+    )
 
     rect = [[0.0 * line_time, 15.0 * pixel_size], [30 * line_time, 30.0 * pixel_size]]
     lines = track_lines(kymo_integration_test_data, "red", 3 * pixel_size, 4, rect=rect)
     np.testing.assert_allclose(lines[0].coordinate_idx, [21] * len(lines[0].coordinate_idx))
     np.testing.assert_allclose(lines[0].time_idx, np.arange(14, 26))
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_peakfinding.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_refinement.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_refinement.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     coordinate_idx = np.array([1.0, 3.0, 3.0])
     kymotrack = KymoTrack(time_idx, coordinate_idx, blank_kymo, "red")
     interpolated = kymotrack.interpolate()
     np.testing.assert_equal(interpolated.time_idx, [1, 2, 3, 4, 5])
     np.testing.assert_allclose(interpolated.coordinate_idx, [1.0, 2.0, 3.0, 3.0, 3.0])
 
     # Test whether concatenation still works after interpolation
-    np.testing.assert_equal(
-        (interpolated + kymotrack).time_idx, [1, 2, 3, 4, 5, 1, 3, 5]
-    )
+    np.testing.assert_equal((interpolated + kymotrack).time_idx, [1, 2, 3, 4, 5, 1, 3, 5])
     np.testing.assert_allclose(
         (interpolated + kymotrack).coordinate_idx, [1.0, 2.0, 3.0, 3.0, 3.0, 1.0, 3.0, 3.0]
     )
 
 
 def test_refinement_2d():
     time_idx = np.array([1, 2, 3, 4, 5])
@@ -103,14 +101,31 @@
     ):
         refine_tracks_centroid([KymoTrack([0], [25], kymo_integration_test_data, "red")], 0.149)[0]
 
     # This should be fine though
     refine_tracks_centroid([KymoTrack([0], [25], kymo_integration_test_data, "red")], 0.15)[0]
 
 
+def test_centroid_refinement_multiple_sources(kymogroups_2tracks, kymogroups_close_tracks):
+    tracks1, *_ = kymogroups_2tracks
+    tracks2 = kymogroups_close_tracks
+    assert [id(k) for k in tracks1._kymos] != [id(k) for k in tracks2._kymos]
+
+    tracks3 = tracks1[:1] + tracks2 + tracks1[1:]
+
+    refined_tracks1 = refine_tracks_centroid(tracks1)
+    refined_tracks2 = refine_tracks_centroid(tracks2)
+    refined_tracks3 = refine_tracks_centroid(tracks3)
+
+    reference_refined_tracks = refined_tracks1[:1] + refined_tracks2 + refined_tracks1[1:]
+
+    for track, ref_track in zip(refined_tracks3, reference_refined_tracks):
+        np.testing.assert_allclose(track.position, ref_track.position)
+
+
 @pytest.mark.parametrize("fit_mode", ["ignore", "multiple"])
 def test_gaussian_refinement(kymogroups_2tracks, fit_mode):
     tracks, gapped_tracks, mixed_tracks = kymogroups_2tracks
 
     # full data, no overlap
     refined = refine_tracks_gaussian(
         tracks, window=3, refine_missing_frames=True, overlap_strategy=fit_mode
@@ -218,14 +233,37 @@
     )
     assert np.allclose(
         refined[1].position,
         [3.32775782, 3.42564736, 3.33315701, 3.60090496, 3.26356061],
     )
 
 
+def test_gaussian_refinement_multiple_sources(kymogroups_2tracks, kymogroups_close_tracks):
+    tracks1, *_ = kymogroups_2tracks
+    tracks2 = kymogroups_close_tracks
+    assert [id(k) for k in tracks1._kymos] != [id(k) for k in tracks2._kymos]
+
+    tracks3 = tracks1[:1] + tracks2 + tracks1[1:]
+
+    refinement_kwargs = {
+        "window": 3,
+        "refine_missing_frames": False,
+        "overlap_strategy": "multiple",
+    }
+
+    refined_tracks1 = refine_tracks_gaussian(tracks1, **refinement_kwargs)
+    refined_tracks2 = refine_tracks_gaussian(tracks2, **refinement_kwargs)
+    refined_tracks3 = refine_tracks_gaussian(tracks3, **refinement_kwargs)
+
+    reference_refined_tracks = refined_tracks1[:1] + refined_tracks2 + refined_tracks1[1:]
+
+    for track, ref_track in zip(refined_tracks3, reference_refined_tracks):
+        np.testing.assert_allclose(track.position, ref_track.position)
+
+
 def test_filter_tracks(blank_kymo):
     k1 = KymoTrack([1, 2, 3], [1, 2, 3], blank_kymo, "red")
     k2 = KymoTrack([2, 3], [1, 2], blank_kymo, "red")
     k3 = KymoTrack([2, 3, 4, 5], [1, 2, 4, 5], blank_kymo, "red")
     tracks = KymoTrackGroup([k1, k2, k3])
     assert len(filter_tracks(tracks, 5)) == 0
     assert all([track1 == track2 for track1, track2 in zip(filter_tracks(tracks, 5), [k1, k3])])
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_sequence.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_stitching.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_stitching.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/kymotracker/tests/test_tracing.py` & `lumicks.pylake-1.1.0/lumicks/pylake/kymotracker/tests/test_tracing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/marker.py` & `lumicks.pylake-1.1.0/lumicks/pylake/marker.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/correlated_plot.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/correlated_plot.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/detail/mouse.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/mouse.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,31 +6,33 @@
     x: float
     y: float
     dx: float
     dy: float
 
 
 class MouseDragCallback:
-    def __init__(self, axes, button, drag_callback, press_callback=None, release_callback=None):
+    def __init__(
+        self, axes, button, drag_callback=None, press_callback=None, release_callback=None
+    ):
         """Callback handler to handle mouse dragging for a particular button. Callback is called
         with x, y, dx, dy as arguments.
 
         Parameters
         ----------
         axes : :class:`~matplotlib.axes.Axes`
             Axes to attach the callback to.
         button : int
             Which button to respond to (0: Left, 3: Right).
-        drag_callback : callable
+        drag_callback : callable, optional
             Which function to call when dragging takes place. Note that this function should have
             the following input signature: fun(MouseDragEvent). MouseDragEvent contains x, y,
             dx and dy which are all defined in data coordinates.
-        press_callback : callable
+        press_callback : callable, optional
             Function to call when drag is initiated. Must return True if it is a valid drag.
-        release_callback : callable
+        release_callback : callable, optional
             Function to call when drag is released.
         """
         self._axes = axes
         self._button = button
         self._drag_callback = drag_callback
         self._release_callback = release_callback
         self._press_callback = press_callback
@@ -48,20 +50,25 @@
                 self._axes.get_figure().canvas.mpl_disconnect(self._callback_ids[callback_name])
                 self._callback_ids[callback_name] = None
 
         if state:
             self._callback_ids["press"] = self._axes.get_figure().canvas.mpl_connect(
                 "button_press_event", lambda event: self.button_down(event)
             )
+
             self._callback_ids["release"] = self._axes.get_figure().canvas.mpl_connect(
                 "button_release_event", lambda event: self.button_release(event)
             )
-            self._callback_ids["motion"] = self._axes.get_figure().canvas.mpl_connect(
-                "motion_notify_event", lambda event: self.handle_motion(event)
-            )
+
+            if self._drag_callback:
+                self._callback_ids["motion"] = self._axes.get_figure().canvas.mpl_connect(
+                    "motion_notify_event", lambda event: self.handle_motion(event)
+                )
+
+            self._axes.get_figure().canvas.flush_events()
         else:
             self.dragging = False
 
     def button_down(self, event):
         if event.inaxes == self._axes and not event.canvas.widgetlock.locked():
             if event.button == self._button:
                 # If there's a starting callback, then it decides whether this will initiate a drag.
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/detail/undostack.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/detail/undostack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/image_editing.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/image_editing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/kymotracker_widgets.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional
 import inspect
+import warnings
 import numpy as np
 import matplotlib.pyplot as plt
 from copy import copy
 from matplotlib.widgets import RectangleSelector
 from lumicks.pylake.kymotracker.kymotracker import track_greedy
 from lumicks.pylake import filter_tracks, refine_tracks_centroid
 from lumicks.pylake.nb_widgets.detail.mouse import MouseDragCallback
@@ -20,14 +21,15 @@
         channel,
         *,
         axis_aspect_ratio,
         use_widgets,
         output_filename,
         algorithm,
         algorithm_parameters,
+        correct_origin=None,
         **kwargs,
     ):
         """Create a widget for performing kymotracking.
 
         Parameters
         ----------
         kymo : lumicks.pylake.Kymo
@@ -43,14 +45,23 @@
         output_filename : str
             Filename to save to and load from.
         algorithm : callable
             Kymotracking algorithm used
         algorithm_parameters : dict
             Dictionary of `KymotrackerParameter` instances holding the slider attributes
             and values for the tracking algorithm parameters
+        correct_origin : bool, optional
+            Use the correct pixel origin when summing track intensities when saving the file. When
+            saving the tracks, the widget stores the sum of the intensities around the tracks.
+            Tracks are defined with the origin of each image pixel defined at the center. However,
+            prior to Pylake version 1.1.0, the method that samples photon counts around the track
+            had a bug which assumed the origin at the edge of the pixel. Setting this flag to
+            `True` produces the correct behavior. The default is set to `None` which reproduces
+            the old behavior and results in a warning when saving tracks, while `False` reproduces
+            the old behavior without a warning.
         **kwargs
             Extra arguments forwarded to imshow.
         """
         data = kymo.get_image(channel)
 
         # Forcing the aspect ratio only makes sense when the time axis is longer.
         self._axis_aspect_ratio = (
@@ -67,17 +78,19 @@
         self._channel = channel
         self._labels = {}
         self._fig = None
         self._axes = None
         self._adding = True
         self._show_tracks = True
         self._output_filename = output_filename
+        self._correct_origin = correct_origin
 
         self._area_selector = None
         self._track_connector = None
+        self._track_splitter = None
 
         self._algorithm = algorithm
         self._algorithm_parameters = algorithm_parameters
 
         self._show(use_widgets=use_widgets, **kwargs)
 
     @property
@@ -165,14 +178,58 @@
         def get_nearest(x, y):
             nonlocal nodes
             ref_position = np.array([x, y])
             squared_dist = np.sum(((ref_position - nodes[:, -2:]) / self._get_scale()) ** 2, 1)
             idx = np.argmin(squared_dist)
             return np.sqrt(squared_dist[idx]), idx
 
+        def split_track(event):
+            nonlocal nodes
+
+            if len(self.tracks) == 0:
+                return
+
+            nodes = get_node_info()
+            distance, idx = get_nearest(event.x, event.y)
+            if distance < cutoff_radius:
+                track_index, node_index, seconds, _ = nodes[idx]
+
+                # Explicit copy to ensure current state pushed to undo stack on assignment.
+                tracks = copy(self.tracks)
+
+                # If we click _beyond_ the node, cut there! Without adding the check on seconds
+                # we get the annoying case where the nearest is on the start of a long gap, but the
+                # line gets cut _left_ of the gap.
+                cut_point = int(node_index) + int(seconds < event.x)
+
+                try:
+                    tracks._split_track(
+                        tracks[int(track_index)],
+                        cut_point,
+                        self._algorithm_parameters["min_length"].value,
+                    )
+
+                    delta_count = len(tracks) - len(self.tracks)
+                    if delta_count < 1:
+                        count, verb = (
+                            ("One track", "was") if delta_count == 0 else ("Two tracks", "were")
+                        )
+                        self._set_label(
+                            "warning",
+                            f"{count} {verb} below the minimum length threshold and {verb} "
+                            f"filtered. Decrease the minimum length if this was not intended.",
+                        )
+
+                    self.tracks = tracks
+                    self._update_tracks()
+
+                except ValueError:
+                    # Gracefully handle the case where we clicked an endpoint
+                    pass
+
         def initiate_track(event):
             nonlocal nodes, clicked_track_info
             if len(self.tracks) == 0:
                 return
 
             nodes = get_node_info()
             distance, idx = get_nearest(event.x, event.y)
@@ -216,20 +273,23 @@
 
                 self.tracks = tracks
                 self._update_tracks()
 
         self._track_connector = MouseDragCallback(
             self._axes,
             3,
-            drag_track,
+            drag_callback=drag_track,
             press_callback=initiate_track,
             release_callback=finalize_track,
         )
         self._track_connector.set_active(False)
 
+        self._track_splitter = MouseDragCallback(self._axes, 3, press_callback=split_track)
+        self._track_splitter.set_active(False)
+
     def _update_tracks(self):
         for track in self._plotted_tracks:
             track.remove()
         self._plotted_tracks = []
 
         if self._show_tracks:
             self._plotted_tracks = [
@@ -267,15 +327,37 @@
         delimiter : str
             Which delimiter to use in the csv file.
         sampling_width : int or None
             When supplied, this will sample the source image around the kymograph track and export
             the summed intensity with the image. The value indicates the number of pixels in either direction
             to sum over.
         """
-        self.tracks.save(filename, delimiter, sampling_width)
+        correct_origin = self._correct_origin
+        if correct_origin is None:
+            # Emit more specific warning for the widget
+            correct_origin = False
+            warnings.warn(
+                RuntimeWarning(
+                    "Prior to version 1.1.0 the method `sample_from_image` had a bug that assumed "
+                    "the origin of a pixel to be at the edge rather than the center of the pixel. "
+                    "Consequently, the sampled window could frequently be off by one pixel. To get "
+                    "the correct behavior and silence this warning, specify `correct_origin=True` "
+                    "when opening the kymotracking widget. The old (incorrect) behavior is "
+                    "maintained until the next major release to ensure backward compatibility. "
+                    "To silence this warning use `correct_origin=False`."
+                )
+            )
+            self._set_label(
+                "warning",
+                "Sampled intensities are using the wrong pixel origin. To correct this, add extra "
+                "argument correct_origin=True when opening the widget. Run "
+                "help(lk.KymoWidgetGreedy) for more info.",
+            )
+
+        self.tracks.save(filename, delimiter, sampling_width, correct_origin=correct_origin)
 
     def _load_from_ui(self):
         try:
             self.tracks = import_kymotrackgroup_from_csv(
                 self._output_filename, self._kymo, self._channel
             )
             self._update_tracks()
@@ -393,15 +475,15 @@
         def set_fn(value):
             self._output_filename = value.new
 
         fn_widget = ipywidgets.Text(value=self._output_filename, description="File")
         fn_widget.observe(set_fn, "value")
 
         self._mode = ipywidgets.RadioButtons(
-            options=["Track", "Remove Tracks", "Connect Tracks"],
+            options=["Track", "Remove Tracks", "Connect Tracks", "Split Tracks"],
             disabled=False,
             tooltip="Choose between adding, removing, or connecting tracks",
             layout=ipywidgets.Layout(flex_flow="row"),
         )
         self._mode.observe(self._select_state, "value")
 
         output = ipywidgets.Output()
@@ -441,26 +523,30 @@
                 display(self._fig)
 
     def _select_state(self, value):
         """Select a different state to operate the widget in. Note that the input argument is value
         because it is hooked up to a ToggleButton directly"""
         self._area_selector.set_active(False)
         self._track_connector.set_active(False)
+        self._track_splitter.set_active(False)
 
         if value["new"] == "Track":
             self._set_label("status", "Drag right mouse button to track an ROI")
             self._area_selector.set_active(True)
             self._adding = True
         elif value["new"] == "Remove Tracks":
             self._set_label("status", "Drag right mouse button to remove tracks from an ROI")
             self._area_selector.set_active(True)
             self._adding = False
         elif value["new"] == "Connect Tracks":
             self._set_label("status", "Drag right mouse button to connect two tracks")
             self._track_connector.set_active(True)
+        elif value["new"] == "Split Tracks":
+            self._set_label("status", "Click track with right mouse button to split a track")
+            self._track_splitter.set_active(True)
 
     def _show(self, use_widgets, **kwargs):
         if self._fig:
             plt.close(self._fig)
             self._plotted_tracks = []
 
         if use_widgets:
@@ -549,14 +635,23 @@
     output_filename : str, optional
         Filename to save to and load from.
     slider_ranges : dict of list, optional
         Dictionary with custom ranges for selected parameter sliders. Ranges should be in the
         following format: (lower bound, upper bound).
         Valid options are: "window", "pixel_threshold", "track_width", "sigma", "min_length" and
         "velocity".
+    correct_origin : bool, optional
+        Use the correct pixel origin when summing track intensities when saving the file. When
+        saving the tracks, the widget stores the sum of the intensities around the tracks. Tracks
+        are defined with the origin of each image pixel defined at the center. However, prior to
+        Pylake version 1.1.0, the method that samples photon counts around the track had a bug
+        which assumed the origin at the edge of the pixel. Setting this flag to `True` produces
+        the correct behavior. The default is set to `None` which reproduces the old behavior and
+        results in a warning when saving tracks, while `False` reproduces the old behavior without
+        a warning.
     """
 
     def __init__(
         self,
         kymo,
         channel,
         *,
@@ -568,14 +663,15 @@
         velocity=None,
         diffusion=None,
         sigma_cutoff=None,
         min_length=None,
         use_widgets=True,
         output_filename="kymotracks.txt",
         slider_ranges=None,
+        correct_origin=None,
         **kwargs,
     ):
         def wrapped_track_greedy(kymo, channel, min_length, **kwargs):
             return filter_tracks(
                 track_greedy(kymo, channel, **kwargs),
                 min_length,
             )
@@ -620,14 +716,15 @@
             kymo,
             channel,
             axis_aspect_ratio=axis_aspect_ratio,
             use_widgets=use_widgets,
             output_filename=output_filename,
             algorithm=algorithm,
             algorithm_parameters=algorithm_parameters,
+            correct_origin=correct_origin,
             **kwargs,
         )
 
     def _create_algorithm_sliders(self):
         import ipywidgets
 
         slider_box = ipywidgets.VBox(
@@ -739,15 +836,15 @@
             abridged_name="Max gap",
         ),
         "min_length": KymotrackerParameter(
             "Minimum length",
             "Minimum number of frames a spot has to be detected in to be considered.",
             "int",
             3,
-            *(1, 10),
+            *(2, 10),
             True,
             r"Minimum length defines the minimum number of points a tracked line must contain for "
             r"it to be considered valid. Reducing this parameter can be effective in reducing "
             r"tracking noise. Note that this length refers to the number of detected points, not "
             r"length in time!",
             abridged_name="Min length",
         ),
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/range_selector.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/range_selector.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_correlated_plot.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_fd_selector.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_image_editing.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_kymotracker_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from lumicks.pylake.kymotracker.kymotrack import KymoTrack, KymoTrackGroup
 from lumicks.pylake.kymo import _kymo_from_array
 import numpy as np
 import re
 import pytest
 
 
+class MockLabel:
+    def __init__(self):
+        self.value = ""
+
 def calibrate_to_kymo(kymo):
     return (
         lambda coord_idx: kymo.pixelsize_um[0] * coord_idx,
         lambda time_idx: kymo.line_time_seconds * time_idx,
     )
 
 
@@ -106,19 +110,47 @@
     assert len(kymo_widget.tracks) == 2
 
 
 def test_save_load_from_ui(kymograph, tmpdir_factory):
     """Check if a round trip through the UI saving function works."""
     testfile = f"{tmpdir_factory.mktemp('pylake')}/kymo.csv"
 
+    kymo_widget = KymoWidgetGreedy(
+        kymograph, "red", axis_aspect_ratio=1, use_widgets=False, correct_origin=False
+    )
+    kymo_widget._labels = {"status": MockLabel(), "warning": MockLabel()}
+    kymo_widget._output_filename = testfile
+    kymo_widget._save_from_ui()
+    assert len(kymo_widget._labels["warning"].value) == 0
+
     kymo_widget = KymoWidgetGreedy(kymograph, "red", axis_aspect_ratio=1, use_widgets=False)
+    kymo_widget._labels = {"status": MockLabel(), "warning": MockLabel()}
     kymo_widget._algorithm_parameters["pixel_threshold"].value = 4
     kymo_widget._track_all()
     kymo_widget._output_filename = testfile
-    kymo_widget._save_from_ui()
+
+    with pytest.warns(
+        RuntimeWarning,
+        match=re.escape(
+            "Prior to version 1.1.0 the method `sample_from_image` had a bug that assumed "
+            "the origin of a pixel to be at the edge rather than the center of the pixel. "
+            "Consequently, the sampled window could frequently be off by one pixel. To get "
+            "the correct behavior and silence this warning, specify `correct_origin=True` "
+            "when opening the kymotracking widget. The old (incorrect) behavior is "
+            "maintained until the next major release to ensure backward compatibility. "
+            "To silence this warning use `correct_origin=False`."
+        ),
+    ):
+        kymo_widget._save_from_ui()
+
+    assert kymo_widget._labels["warning"].value == (
+        "<font color='red'>Sampled intensities are using the wrong pixel origin. To correct "
+        "this, add extra argument correct_origin=True when opening the widget. Run "
+        "help(lk.KymoWidgetGreedy) for more info."
+    )
 
     tracks = kymo_widget.tracks
 
     kymo_widget = KymoWidgetGreedy(kymograph, "red", axis_aspect_ratio=1, use_widgets=False)
     assert len(kymo_widget.tracks) == 0
 
     kymo_widget._output_filename = testfile
@@ -130,18 +162,14 @@
 
 
 def test_refine_from_widget(kymograph, region_select):
     kymo_widget = KymoWidgetGreedy(kymograph, "red", axis_aspect_ratio=1, use_widgets=False)
     in_um, in_s = calibrate_to_kymo(kymograph)
 
     # Test whether error is handled when refining before tracking / loading
-    class MockLabel:
-        def __init__(self):
-            self.value = ""
-
     kymo_widget._labels = {"status": MockLabel()}
     kymo_widget._refine()
     assert (
         kymo_widget._labels["status"].value
         == "You need to track this kymograph or load tracks before you can refine them"
     )
 
@@ -375,7 +403,51 @@
 
     default_params = _get_default_parameters(kymo, "red")
     for key, param in ref_values.items():
         value, mini, maxi = param
         np.testing.assert_allclose(default_params[key].value, value, err_msg=f"{key}")
         np.testing.assert_allclose(default_params[key].lower_bound, mini, err_msg=f"{key}")
         np.testing.assert_allclose(default_params[key].upper_bound, maxi, err_msg=f"{key}")
+
+
+def test_split(kymograph, mockevent):
+    kymo_widget = KymoWidgetGreedy(kymograph, "red", axis_aspect_ratio=1, use_widgets=False)
+    kymo_widget._labels = {"warning": MockLabel(), "status": MockLabel()}
+
+    k1 = KymoTrack(
+        np.array([0, 1, 2, 3, 6, 7, 8, 9, 10]),
+        np.array([1, 1, 1, 1, 1, 1, 1, 1, 1]),
+        kymograph,
+        "red",
+    )
+    kymo_widget.tracks = KymoTrackGroup([k1])
+
+    # Go into track connection mode
+    kymo_widget._select_state({"new": "Split Tracks"})
+
+    assert len(kymo_widget.tracks) == 1
+
+    in_um, in_s = calibrate_to_kymo(kymograph)
+
+    # Click too far from the line to split
+    kymo_widget._track_splitter.button_down(mockevent(kymo_widget._axes, in_s(3), in_um(5), 3, 0))
+    assert len(kymo_widget.tracks) == 1
+
+    # Split line
+    kymo_widget._track_splitter.button_down(mockevent(kymo_widget._axes, in_s(3), in_um(1), 3, 0))
+    assert len(kymo_widget.tracks) == 2
+
+    kymo_widget._track_splitter.button_down(mockevent(kymo_widget._axes, in_s(7), in_um(1), 3, 0))
+    assert len(kymo_widget.tracks) == 2
+    assert kymo_widget._labels["warning"].value == (
+        "<font color='red'>One track was below the minimum length threshold and was filtered. "
+        "Decrease the minimum length if this was not intended."
+    )
+
+    # Split line where both lines are dropped
+    kymo_widget._labels = {"warning": MockLabel()}
+    kymo_widget._track_splitter.button_down(mockevent(kymo_widget._axes, in_s(9), in_um(1), 3, 0))
+    assert len(kymo_widget.tracks) == 1
+    assert kymo_widget._labels["warning"].value == (
+        "<font color='red'>Two tracks were below the minimum length threshold and were filtered. "
+        "Decrease the minimum length if this was not intended."
+    )
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_mouse.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_mouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     np.testing.assert_allclose(current_dx, 3)
     np.testing.assert_allclose(current_dy, 3)
 
 
 def test_set_active():
     ax = open_plot()
     button = 1
-    mouse_drag = MouseDragCallback(ax, button, [])
+    mouse_drag = MouseDragCallback(ax, button, lambda x: x)
 
     # Callbacks should be on initially
     for cib in mouse_drag._callback_ids.values():
         assert cib
 
     # Inactive handler should not be dragging
     mouse_drag.dragging = True
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/nb_widgets/tests/test_undostack.py` & `lumicks.pylake-1.1.0/lumicks/pylake/nb_widgets/tests/test_undostack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/note.py` & `lumicks.pylake-1.1.0/lumicks/pylake/note.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/baseline.py` & `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/baseline.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/piezo_tracking.py` & `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/piezo_tracking.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/tests/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py` & `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/test_baseline.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py` & `lumicks.pylake-1.1.0/lumicks/pylake/piezo_tracking/tests/test_piezo_tracking.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/point_scan.py` & `lumicks.pylake-1.1.0/lumicks/pylake/point_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/population/mixture.py` & `lumicks.pylake-1.1.0/lumicks/pylake/population/mixture.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/population/tests/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/exponential_data.npz` & `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/exponential_data.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/generate_exponential_data.py` & `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/generate_exponential_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/generate_trace_data.py` & `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/generate_trace_data.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/population/tests/data/trace_data.npz` & `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/data/trace_data.npz`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/population/tests/test_mixture.py` & `lumicks.pylake-1.1.0/lumicks/pylake/population/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/scalebar.py` & `lumicks.pylake-1.1.0/lumicks/pylake/scalebar.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/scan.py` & `lumicks.pylake-1.1.0/lumicks/pylake/scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/simulation/diffusion.py` & `lumicks.pylake-1.1.0/lumicks/pylake/simulation/diffusion.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/simulation/tests/test_diffusion.py` & `lumicks.pylake-1.1.0/lumicks/pylake/simulation/tests/test_diffusion.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,10 +31,7 @@
     """Test whether we can add kymograph tracks.
 
     It should be possible to add tracks generated by separate calls with the same kymo properties.
     """
     params = {"diffusion_constant": 4, "steps": 10, "dt": 0.01, "num_tracks": 2}
     tracks = simulate_diffusive_tracks(**params) + simulate_diffusive_tracks(**params)
     assert len(tracks) == 4
-
-    with pytest.raises(ValueError, match="All tracks must have the same source kymograph"):
-        simulate_diffusive_tracks(**params) + simulate_diffusive_tracks(**{**params, "dt": 0.05})
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_confocal.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_fdcurve.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_file.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         return dset
 
     def make_timetags_channel(self, group, name, data):
         raise NotImplementedError
 
 
 class MockDataFile_v2(MockDataFile_v1):
+    # CAVE: Please respect that `MockDataFile_v2` is used by another Lumicks project
 
     def get_file_format_version(self):
         return 2
 
     def make_calibration_data(self, calibration_idx, group, attributes):
         if "Calibration" not in self.file:
             self.file.create_group("Calibration")
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_json.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_json.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/data/mock_widefield.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/mock_widefield.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,22 +181,20 @@
 def write_tiff_file(image, description, n_frames, filename):
     # We use the dimension of image data to evaluate the number of color channels
     channels = 1 if image.ndim == 2 else 3
     movie = np.stack([image for n in range(n_frames)], axis=0)
 
     # Orientation = ORIENTATION.TOPLEFT
     tag_orientation = (274, "H", 1, 1, False)
-    # SampleFormat = SAMPLEFORMAT.UINT
-    tag_sample_format = (339, "H", channels, (1,) * channels, False)
 
     with tifffile.TiffWriter(filename) as tif:
         for n, frame in enumerate(movie):
             str_datetime = f"{n*10+10}:{n*10+18}"
             tag_datetime = (306, "s", len(str_datetime), str_datetime, False)
             tif.write(
                 frame,
                 description=json.dumps(description, indent=4),
                 software="Bluelake Unknown",
                 metadata=None,
                 contiguous=False,
-                extratags=(tag_orientation, tag_sample_format, tag_datetime),
+                extratags=(tag_orientation, tag_datetime),
             )
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/data/test_mock_confocal.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/data/test_mock_confocal.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_channels/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_channels/test_arithmetic.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_channels/test_channels.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_channels/test_channels.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_fdcurve.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_fdcurve.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_fdensemble.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_fdensemble.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file/test_file.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/test_file.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file/test_file_items.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file/test_file_items.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_file_download.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_file_download.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_image.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/test_export.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_export.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_image_reconstruction.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_camera/test_image_stack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal/test_confocal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pytest
 from lumicks.pylake.detail.confocal import ScanAxis, ScanMetaData
+from lumicks.pylake.kymo import _kymo_from_array
 
-from ..data.mock_confocal import generate_scan_json
+from ..data.mock_confocal import generate_scan_json, generate_scan, generate_kymo
 
 
 @pytest.mark.parametrize(
     "axis, num_pixels, pixel_size_um, label",
     [(0, 10, 0.5, "X"), (1, 5, 0.4, "Y"), (2, 15, 0.35, "Z")],
 )
 def test_scanaxis(axis, num_pixels, pixel_size_um, label):
@@ -93,7 +94,32 @@
     assert metadata.num_axes == len(scan_axes)
     assert metadata.fast_axis == scan_axes[0].axis_label
     assert len(metadata.scan_order) == len(scan_order)
     np.testing.assert_equal(metadata.scan_order, scan_order)
     assert np.all(
         [oa == sa for oa, sa in zip(metadata.ordered_axes, [scan_axes[i] for i in scan_order])]
     )
+
+
+@pytest.mark.parametrize(
+    "item, has_timestamps",
+    [
+        (generate_kymo("Mock", np.ones((5, 5))), True),
+        (generate_scan("Mock", np.ones((5, 5)), [1, 1]), True),
+        (_kymo_from_array(np.ones((5, 5)), "r", 1), False),
+    ],
+)
+def test_immutable_returns(item, has_timestamps):
+    """Ensure that users cannot modify data in the cache."""
+    red = item.get_image("red")
+
+    with pytest.raises(ValueError, match="assignment destination is read-only"):
+        red[2, 2] = 100
+    assert item.get_image("red")[2, 2] == 1
+
+    if has_timestamps:
+        ts = item.timestamps
+        ref_ts = ts[2, 2]
+
+        with pytest.raises(ValueError, match="assignment destination is read-only"):
+            ts[2, 2] = 100
+        assert item.timestamps[2, 2] == ref_ts
```

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/conftest.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/conftest.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_array.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_array.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_imagestack.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_kymo_from_imagestack.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_point_scan.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_point_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_confocal_old/test_scan.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_confocal_old/test_scan.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_imaging_mixins.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_imaging_mixins.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_import_time.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_import_time.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_mixin.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_scalebar.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_scalebar.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_timeindex.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_timeindex.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks/pylake/tests/test_utilities.py` & `lumicks.pylake-1.1.0/lumicks/pylake/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/lumicks.pylake.egg-info/PKG-INFO` & `lumicks.pylake-1.1.0/lumicks.pylake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumicks.pylake
-Version: 1.0.0
+Version: 1.1.0
 Summary: Bluelake data analysis tools
 Home-page: https://github.com/lumicks/pylake
 Author: Lumicks B.V.
 Author-email: devteam@lumicks.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lumicks.pylake-1.0.0/lumicks.pylake.egg-info/SOURCES.txt` & `lumicks.pylake-1.1.0/lumicks.pylake.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 lumicks/pylake/kymotracker/tests/test_algorithm_scaling.py
 lumicks/pylake/kymotracker/tests/test_gaussian_mle.py
 lumicks/pylake/kymotracker/tests/test_geometry_2d.py
 lumicks/pylake/kymotracker/tests/test_greedy_algorithm.py
 lumicks/pylake/kymotracker/tests/test_image_sampling.py
 lumicks/pylake/kymotracker/tests/test_io.py
 lumicks/pylake/kymotracker/tests/test_kymotrack.py
+lumicks/pylake/kymotracker/tests/test_kymotrackgroup_sources.py
 lumicks/pylake/kymotracker/tests/test_lines_algorithm.py
 lumicks/pylake/kymotracker/tests/test_loc_models.py
 lumicks/pylake/kymotracker/tests/test_peakfinding.py
 lumicks/pylake/kymotracker/tests/test_refinement.py
 lumicks/pylake/kymotracker/tests/test_sequence.py
 lumicks/pylake/kymotracker/tests/test_stitching.py
 lumicks/pylake/kymotracker/tests/test_tracing.py
```

### Comparing `lumicks.pylake-1.0.0/readme.md` & `lumicks.pylake-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `lumicks.pylake-1.0.0/setup.py` & `lumicks.pylake-1.1.0/setup.py`

 * *Files identical despite different names*

