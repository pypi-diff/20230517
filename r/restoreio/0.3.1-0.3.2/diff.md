# Comparing `tmp/restoreio-0.3.1.tar.gz` & `tmp/restoreio-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "restoreio-0.3.1.tar", last modified: Mon May 15 05:17:09 2023, max compression
+gzip compressed data, was "restoreio-0.3.2.tar", last modified: Tue May 16 22:15:29 2023, max compression
```

## Comparing `restoreio-0.3.1.tar` & `restoreio-0.3.2.tar`

### file list

```diff
@@ -1,177 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-15 05:16:50.000000 restoreio-0.3.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 05:16:50.000000 restoreio-0.3.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-15 05:16:50.000000 restoreio-0.3.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-15 05:16:50.000000 restoreio-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 05:16:50.000000 restoreio-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-15 05:17:09.567025 restoreio-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-15 05:16:50.000000 restoreio-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.551024 restoreio-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.551024 restoreio-0.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.547024 restoreio-0.3.1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.547024 restoreio-0.3.1/docs/source/_static/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.551024 restoreio-0.3.1/docs/source/_static/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/assets/fonts/synconew.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/assets/fonts/syncopate.bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/assets/fonts/syncopate.regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.551024 restoreio-0.3.1/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/css/custom-anaconda-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/css/custom-pydata.css
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.547024 restoreio-0.3.1/docs/source/_static/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.555024 restoreio-0.3.1/docs/source/_static/images/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.png
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.ico
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.png
--rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-light.png
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/_static/images/plots/
--rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/cor_cov.png
--rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/deviation.png
--rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/ensembles.png
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/ensembles_js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/gdop_coverage.png
--rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/js_distance.png
--rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/kl_eigenvalues.png
--rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/kl_eigenvectors.png
--rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/orig_vel_and_error.png
--rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/images/plots/rbf_kernel_2d.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_static/js/custom-pydata.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/ndarray_subclass.rst
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/autosummary/property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/_templates/version.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/cite.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/generated/restoreio.restore.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   151486 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/notebooks/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-15 05:16:50.000000 restoreio-0.3.1/docs/source/recursive_glob.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 05:16:50.000000 restoreio-0.3.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.547024 restoreio-0.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/examples/restore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/main_VaryingNumModes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/plot_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/plot_fixed_size_artificial_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/plot_variable_d_artificial_masks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/restore/plot_variable_size_artificial_masks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.559024 restoreio-0.3.1/examples/uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/_plot_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/plot_gdop_coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-15 05:16:50.000000 restoreio-0.3.1/examples/uncertainty_quant/plot_js_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 05:16:50.000000 restoreio-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 05:16:50.000000 restoreio-0.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21751 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_file_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_file_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_file_utilities/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_geography/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/_find_alpha_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/create_mask_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/detect_land_ocean.py
--rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_geography/locate_missing_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_inpaint/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/_cast_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/_plot_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_inpaint/inpaint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_input_output/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/get_datetime_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/load_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_input_output/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_parser/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_parser/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_parser/parse_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio/_plots/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_display_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_draw_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_quiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_streamlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/_plot_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots/plot_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_plots_uq/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/_refine_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/_shifted_colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_cor_cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_ensembles_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_kl_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_restore/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/_make_array_masked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/refine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/restore_generated_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_restore/restore_main_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34694 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_scripts/scan_netcdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_subset/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_subset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_subset/_array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_subset/subset_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_subset/subset_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/restoreio/_uncertainty_quant/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/_statistical_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/generate_image_ensembles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-15 05:16:50.000000 restoreio-0.3.1/restoreio/_uncertainty_quant/get_ensembles_stat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.563025 restoreio-0.3.1/restoreio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 05:17:09.000000 restoreio-0.3.1/restoreio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-15 05:17:09.567025 restoreio-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-15 05:16:50.000000 restoreio-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 05:17:09.567025 restoreio-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-15 05:16:50.000000 restoreio-0.3.1/tests/test_restore_local_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-15 05:16:50.000000 restoreio-0.3.1/tests/test_restore_remote_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-15 05:16:50.000000 restoreio-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-16 22:15:09.000000 restoreio-0.3.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 22:15:09.000000 restoreio-0.3.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 22:15:09.000000 restoreio-0.3.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-16 22:15:09.000000 restoreio-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-16 22:15:09.000000 restoreio-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-16 22:15:29.934703 restoreio-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-16 22:15:09.000000 restoreio-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.910703 restoreio-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.910703 restoreio-0.3.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_inspect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.898703 restoreio-0.3.2/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.898703 restoreio-0.3.2/docs/source/_static/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.910703 restoreio-0.3.2/docs/source/_static/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   108412 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/assets/fonts/synconew.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65432 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/assets/fonts/syncopate.bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141308 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/assets/fonts/syncopate.regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.914703 restoreio-0.3.2/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/css/custom-anaconda-doc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/css/custom-pydata.css
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.898703 restoreio-0.3.2/docs/source/_static/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.914703 restoreio-0.3.2/docs/source/_static/images/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70855 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26103 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14098 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/_static/images/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)  1078579 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/cor_cov.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386357 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/deviation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419634 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/ensembles.png
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/ensembles_js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   792928 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/gdop_coverage.png
+-rw-r--r--   0 runner    (1001) docker     (123)   130012 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/js_distance.png
+-rw-r--r--   0 runner    (1001) docker     (123)   107758 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/kl_eigenvalues.png
+-rw-r--r--   0 runner    (1001) docker     (123)   541932 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/kl_eigenvectors.png
+-rw-r--r--   0 runner    (1001) docker     (123)   290207 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/orig_vel_and_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)   267216 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/images/plots/rbf_kernel_2d.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_static/js/custom-pydata.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/ndarray_subclass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/autosummary/property.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/_templates/version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/cite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/generated/restoreio.restore.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/generated/restoreio.scan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/notebooks/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-16 22:15:09.000000 restoreio-0.3.2/docs/source/recursive_glob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 22:15:09.000000 restoreio-0.3.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.902703 restoreio-0.3.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.922703 restoreio-0.3.2/examples/restore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30256 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/main_VaryingNumModes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7838 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/plot_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21626 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/plot_fixed_size_artificial_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23405 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/plot_variable_d_artificial_masks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21770 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/restore/plot_variable_size_artificial_masks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/examples/uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/_plot_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16132 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/plot_gdop_coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6715 2023-05-16 22:15:09.000000 restoreio-0.3.2/examples/uncertainty_quant/plot_js_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 22:15:09.000000 restoreio-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 22:15:09.000000 restoreio-0.3.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio/_file_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_file_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_file_utilities/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio/_geography/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/_find_alpha_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/create_mask_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/detect_land_ocean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_geography/locate_missing_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio/_inpaint/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/_cast_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/_plot_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_inpaint/inpaint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.930703 restoreio-0.3.2/restoreio/_input_output/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/get_datetime_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/load_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_input_output/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.930703 restoreio-0.3.2/restoreio/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_parser/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_parser/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_parser/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.930703 restoreio-0.3.2/restoreio/_plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_display_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_draw_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_streamlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/_plot_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots/plot_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.930703 restoreio-0.3.2/restoreio/_plots_uq/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/_refine_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/_shifted_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_cor_cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26594 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_ensembles_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_kl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/restoreio/_restore/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/_make_array_masked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/refine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/restore_generated_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_restore/restore_main_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/restoreio/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_scripts/examples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    40432 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_scripts/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/restoreio/_subset/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_subset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_subset/_array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_subset/subset_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_subset/subset_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/restoreio/_uncertainty_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/_compute_correlation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/_statistical_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/generate_image_ensembles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-05-16 22:15:09.000000 restoreio-0.3.2/restoreio/_uncertainty_quant/get_ensembles_stat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.926703 restoreio-0.3.2/restoreio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 22:15:29.000000 restoreio-0.3.2/restoreio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 22:15:29.938703 restoreio-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-16 22:15:09.000000 restoreio-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 22:15:29.934703 restoreio-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-16 22:15:09.000000 restoreio-0.3.2/tests/test_restore_local_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-16 22:15:09.000000 restoreio-0.3.2/tests/test_restore_remote_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-16 22:15:09.000000 restoreio-0.3.2/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 22:15:09.000000 restoreio-0.3.2/tox.ini
```

### Comparing `restoreio-0.3.1/LICENSE.txt` & `restoreio-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/MANIFEST.in` & `restoreio-0.3.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/PKG-INFO` & `restoreio-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.3.1
+Version: 0.3.2
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.3.1/README.rst` & `restoreio-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/Makefile` & `restoreio-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/make.bat` & `restoreio-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_inspect.py` & `restoreio-0.3.2/docs/source/_inspect.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/assets/fonts/synconew.regular.ttf` & `restoreio-0.3.2/docs/source/_static/assets/fonts/synconew.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/assets/fonts/syncopate.bold.ttf` & `restoreio-0.3.2/docs/source/_static/assets/fonts/syncopate.bold.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/assets/fonts/syncopate.regular.ttf` & `restoreio-0.3.2/docs/source/_static/assets/fonts/syncopate.regular.ttf`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/css/custom-anaconda-doc.css` & `restoreio-0.3.2/docs/source/_static/css/custom-anaconda-doc.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/css/custom-pydata.css` & `restoreio-0.3.2/docs/source/_static/css/custom-pydata.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/css/custom.css` & `restoreio-0.3.2/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/favicon.ico` & `restoreio-0.3.2/docs/source/_static/images/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.ico` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.png` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-anaconda.svg` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-anaconda.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.ico` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.ico`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.png` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-pypi.svg` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-pypi.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-dark.png` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-dark.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-dark.svg` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-dark.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-light.png` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-light.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/icons/logo-restoreio-light.svg` & `restoreio-0.3.2/docs/source/_static/images/icons/logo-restoreio-light.svg`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/cor_cov.png` & `restoreio-0.3.2/docs/source/_static/images/plots/cor_cov.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/deviation.png` & `restoreio-0.3.2/docs/source/_static/images/plots/deviation.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/ensembles.png` & `restoreio-0.3.2/docs/source/_static/images/plots/ensembles.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/ensembles_js_distance.png` & `restoreio-0.3.2/docs/source/_static/images/plots/ensembles_js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/gdop_coverage.png` & `restoreio-0.3.2/docs/source/_static/images/plots/gdop_coverage.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/js_distance.png` & `restoreio-0.3.2/docs/source/_static/images/plots/js_distance.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/kl_eigenvalues.png` & `restoreio-0.3.2/docs/source/_static/images/plots/kl_eigenvalues.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/kl_eigenvectors.png` & `restoreio-0.3.2/docs/source/_static/images/plots/kl_eigenvectors.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/orig_vel_and_error.png` & `restoreio-0.3.2/docs/source/_static/images/plots/orig_vel_and_error.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/images/plots/rbf_kernel_2d.png` & `restoreio-0.3.2/docs/source/_static/images/plots/rbf_kernel_2d.png`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_static/js/custom-pydata.js` & `restoreio-0.3.2/docs/source/_static/js/custom-pydata.js`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_templates/autosummary/class.rst` & `restoreio-0.3.2/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_templates/layout.html` & `restoreio-0.3.2/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/_templates/version.html` & `restoreio-0.3.2/docs/source/_templates/version.html`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/cite.rst` & `restoreio-0.3.2/docs/source/cite.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/conf.py` & `restoreio-0.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/custom_domain.py` & `restoreio-0.3.2/docs/source/custom_domain.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/examples.rst` & `restoreio-0.3.2/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/index.rst` & `restoreio-0.3.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/install.rst` & `restoreio-0.3.2/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/docs/source/recursive_glob.py` & `restoreio-0.3.2/docs/source/recursive_glob.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/restore/main_VaryingNumModes.py` & `restoreio-0.3.2/examples/restore/main_VaryingNumModes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/restore/plot_coverage.py` & `restoreio-0.3.2/examples/restore/plot_coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,22 +149,22 @@
         UsageString = "Usage: " + ExecName + "<InputFilename.{nc,ncml}>"
         print(UsageString)
 
     # Parse arguments, get InputFilename
     InputFilename = ''
     if len(argv) < 1:
         PrintUsage(argv[0])
-        sys.exit()
+        sys.exit(0)
     else:
         InputFilename = argv[1]
 
     # Check input
     if InputFilename == '':
         PrintUsage(argv[0])
-        sys.exit()
+        sys.exit(0)
 
     # Open file
     agg = InputOutput.LoadDataset(InputFilename)
 
     # Load variables
     DatetimeObject,LongitudeObject,LatitudeObject,EastVelocityObject,NorthVelocityObject,EastVelocityErrorObject,NorthVelocityErrorObject = InputOutput.LoadVariables(agg)
```

### Comparing `restoreio-0.3.1/examples/restore/plot_fixed_size_artificial_mask.py` & `restoreio-0.3.2/examples/restore/plot_fixed_size_artificial_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/restore/plot_variable_d_artificial_masks.py` & `restoreio-0.3.2/examples/restore/plot_variable_d_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/restore/plot_variable_size_artificial_masks.py` & `restoreio-0.3.2/examples/restore/plot_variable_size_artificial_masks.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/uncertainty_quant/_display_utilities.py` & `restoreio-0.3.2/examples/uncertainty_quant/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/uncertainty_quant/_draw_map.py` & `restoreio-0.3.2/examples/uncertainty_quant/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/uncertainty_quant/_plot_utilities.py` & `restoreio-0.3.2/examples/uncertainty_quant/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/uncertainty_quant/plot_gdop_coverage.py` & `restoreio-0.3.2/examples/uncertainty_quant/plot_gdop_coverage.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/examples/uncertainty_quant/plot_js_divergence.py` & `restoreio-0.3.2/examples/uncertainty_quant/plot_js_divergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/__main__.py` & `restoreio-0.3.2/restoreio/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,16 +67,16 @@
     # be given, not an interval of time.
     if (uncertainty_quant is True) and (min_time != '' or max_time != ''):
         raise ValueError('When uncertainty quantification is enabled, a time' +
                          'interval cannot be specified, rather a single ' +
                          'time should be specified using "time" argument.')
 
     # When plotting, only a single time point can be plotted
-    if (plot is True) and ((min_time != '') or (max_time != '')) or \
-       ((min_time == '') and (max_time == '') and (time == '')):
+    if (plot is True) and (((min_time != '') or (max_time != '')) or
+       ((min_time == '') and (max_time == '') and (time == ''))):
         raise ValueError('When plotting is enabled, a time interval with ' +
                          '"min_time" or "max_time" arguments should not be ' +
                          'given. Rather, only a single time point can be ' +
                          'plotted that is specified with "time" argument.')
 
     return fill_coast
 
@@ -86,18 +86,18 @@
 # =======
 
 def restore(
         input,
         min_file_index='',
         max_file_index='',
         output='',
-        min_lon=None,
-        max_lon=None,
-        min_lat=None,
-        max_lat=None,
+        min_lon=float('nan'),
+        max_lon=float('nan'),
+        min_lat=float('nan'),
+        max_lat=float('nan'),
         min_time='',
         max_time='',
         time='',
         diffusivity=20,
         sweep=False,
         detect_land=True,
         fill_coast=False,
@@ -106,15 +106,17 @@
         refine_grid=1,
         uncertainty_quant=False,
         num_ensembles=1000,
         ratio_num_modes=1,
         kernel_width=5,
         scale_error=0.08,
         plot=False,
-        verbose=False):
+        save=True,
+        verbose=False,
+        terminate=False):
     """
     Restore incomplete oceanographic dataset.
 
     Parameters
     ----------
 
     input : str
@@ -137,33 +139,33 @@
 
     output : str
         Output filename. This can be either the path to a local file or the url
         to a remote dataset. The file extension should be ``.nc`` or ``.ncml``
         only. If no output file is provided, the output filename is constructed
         by adding the word ``_restored`` at the end of the input filename.
 
-    min_lon : float, default=None
+    min_lon : float, default=float('nan')
         Minimum longitude in the unit of degrees to subset the processing
-        domain. If not provided or set to `None`, the minimum longitude of the
-        input data is considered.
+        domain. If not provided or set to `float('nan')`, the minimum longitude
+        of the input data is considered.
 
-    max_lon : float, default=None
+    max_lon : float, default=float('nan')
         Maximum longitude in the unit of degrees to subset the processing
-        domain. If not provided or set to `None`, the maximum longitude of the
-        input data is considered.
+        domain. If not provided or set to `float('nan')`, the maximum longitude
+        of the input data is considered.
 
-    min_lat : float, default=None
+    min_lat : float, default=float('nan')
         Minimum latitude in the unit of degrees to subset the processing
-        domain. If not provided or set to `None`, the minimum latitude of the
-        input data is considered.
+        domain. If not provided or set to `float('nan')`, the minimum latitude
+        of the input data is considered.
 
-    max_lat : float, default: None
+    max_lat : float, default: float('nan')
         Maximum latitude in the unit of degrees to subset the processing
-        domain. If not provided or set to `None`, the maximum latitude of the
-        input data is considered.
+        domain. If not provided or set to `float('nan')`, the maximum latitude
+        of the input data is considered.
 
     min_time : str, default=''
         The start of the time interval within the dataset times to be
         processed. The time should be provided as a string with the format
         ``'yyyy-mm-ddTHH:MM:SS'`` where ``yyyy`` is year, ``mm`` is month,
         ``dd`` is day, ``HH`` is hour from `00` to `23`, ``MM`` is minutes and
         ``SS`` is seconds. If the given time does not exactly match any time in
@@ -278,19 +280,33 @@
     plot : bool, default=False
         Plots the results. In this case, instead of iterating through all time
         frames, only one time frame (given with option ``timeframe``) is
         restored and plotted. If in addition, the uncertainty quantification is
         enabled (with option ``uncertainty_quant=True``), the statistical
         analysis for the given time frame is also plotted.
 
+    save : bool, default=True
+        If `True`, the plots are not displayed, rather are saved in the current
+        directory as ``.pdf`` and ``.svg`` format. This option is useful when
+        executing this script in an environment without display (such as remote
+        cluster). If `False`, the generated plots will be displayed.
+
     verbose : bool, default=False
         If `True`, prints verbose information during the computation process.
-    """
 
-    save = True  # Test
+    terminate ; bool, default=False
+        If `True`, the program exists with code 1. This is useful when this
+        package is executed on a server to pass exit signals to a Node
+        application. On the downside, this option causes an interactive python
+        environment to both terminate the script and the python environment
+        itself. To avoid this, set this option to `False`. In this case, upon
+        an error, the ``ValueError` is raised, which cases the script to
+        terminate, however, an interactive python environment will not be
+        exited.
+    """
 
     # Check arguments
     fill_coast = process_arguments(
             detect_land, min_file_index, max_file_index, fill_coast,
             time, min_time, max_time, uncertainty_quant, plot)
 
     # Get list of all separate input files to process
@@ -323,22 +339,23 @@
         warnings.filterwarnings('ignore')
 
         # Get datetime info from datetime netcdf object
         datetime_info = get_datetime_info(datetime_obj)
 
         # Subset time
         min_datetime_index, max_datetime_index = subset_datetime(
-            datetime_info, min_time, max_time, time)
+            datetime_info, min_time, max_time, time, terminate)
 
         datetime_info['array'] = \
             datetime_info['array'][min_datetime_index:max_datetime_index+1]
 
         # Subset domain
         min_lon_index, max_lon_index, min_lat_index, max_lat_index = \
-            subset_domain(lon_obj, lat_obj, min_lon, max_lon, min_lat, max_lat)
+            subset_domain(lon_obj, lat_obj, min_lon, max_lon, min_lat, max_lat,
+                          terminate)
         lon = lon_obj[min_lon_index:max_lon_index+1]
         lat = lat_obj[min_lat_index:max_lat_index+1]
 
         # if the velocity arrays have depth dimension, use only the first index
         depth_index = 0
         vel_array_dim = len(east_vel_obj.shape)
```

### Comparing `restoreio-0.3.1/restoreio/_file_utilities/__init__.py` & `restoreio-0.3.2/restoreio/_file_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_file_utilities/file_utilities.py` & `restoreio-0.3.2/restoreio/_file_utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_geography/__init__.py` & `restoreio-0.3.2/restoreio/_geography/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_geography/_find_alpha_shapes.py` & `restoreio-0.3.2/restoreio/_geography/_find_alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_geography/create_mask_info.py` & `restoreio-0.3.2/restoreio/_geography/create_mask_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_geography/detect_land_ocean.py` & `restoreio-0.3.2/restoreio/_geography/detect_land_ocean.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_geography/locate_missing_data.py` & `restoreio-0.3.2/restoreio/_geography/locate_missing_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_inpaint/_cast_types.py` & `restoreio-0.3.2/restoreio/_inpaint/_cast_types.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_inpaint/_image.py` & `restoreio-0.3.2/restoreio/_inpaint/_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_inpaint/_plot_image.py` & `restoreio-0.3.2/restoreio/_inpaint/_plot_image.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_inpaint/inpaint.py` & `restoreio-0.3.2/restoreio/_inpaint/inpaint.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_input_output/__init__.py` & `restoreio-0.3.2/restoreio/_input_output/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_input_output/get_datetime_info.py` & `restoreio-0.3.2/restoreio/_input_output/get_datetime_info.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_input_output/load_dataset.py` & `restoreio-0.3.2/restoreio/_input_output/load_dataset.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_input_output/load_variables.py` & `restoreio-0.3.2/restoreio/_input_output/load_variables.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_input_output/writer.py` & `restoreio-0.3.2/restoreio/_input_output/writer.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_parser/examples.py` & `restoreio-0.3.2/restoreio/_parser/examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # SPDX-FileType: SOURCE
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the license found in the LICENSE.txt file in the root directory
 # of this source tree.
 
+
 examples = """
 Examples:
 
 1. This example reads a local file and restores all time frames in it. A convex
    hull around data points as the working domain.
 
    $ %s -i input.ncml -o output.nc -d 20 -s -c
```

### Comparing `restoreio-0.3.1/restoreio/_parser/formatter.py` & `restoreio-0.3.2/restoreio/_parser/formatter.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_parser/parse_arguments.py` & `restoreio-0.3.2/restoreio/_parser/parse_arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,45 +68,45 @@
     """
     required.add_argument('-o', type=str, default='', metavar='OUTPUT',
                           help=help_output, required=True)
 
     # Min Longitude
     help_min_lon = """
     Minimum longitude in the unit of degrees to subset the processing domain.
-    If not provided or set to `None`, the minimum longitude of the input data
+    If not provided or set to `nan`, the minimum longitude of the input data
     is considered.
     """
-    optional.add_argument('--min-lon', type=float, default=None,
+    optional.add_argument('--min-lon', type=float, default=float('nan'),
                           metavar='MIN_LON', help=help_min_lon)
 
     # Mix Longitude
     help_max_lon = """
     Maximum longitude in the unit of degrees to subset the processing domain.
-    If not provided or set to `None`, the maximum longitude of the input data
+    If not provided or set to `nan`, the maximum longitude of the input data
     is considered.
     """
-    optional.add_argument('--max-lon', type=float, default=None,
+    optional.add_argument('--max-lon', type=float, default=float('nan'),
                           metavar='MAX_LON', help=help_max_lon)
 
     # Min Latitude
     help_min_lat = """
     Minimum latitude in the unit of degrees to subset the processing domain.
-    If not provided or set to `None`, the minimum latitude of the input data
+    If not provided or set to `nan`, the minimum latitude of the input data
     is considered.
     """
-    optional.add_argument('--min-lat', type=float, default=None,
+    optional.add_argument('--min-lat', type=float, default=float('nan'),
                           metavar='MIN_LAT', help=help_min_lat)
 
     # Mix Latitude
     help_max_lat = """
     Maximum latitude in the unit of degrees to subset the processing domain.
-    If not provided or set to `None`, the maximum latitude of the input data
+    If not provided or set to `nan`, the maximum latitude of the input data
     is considered.
     """
-    optional.add_argument('--max-lat', type=float, default=None,
+    optional.add_argument('--max-lat', type=float, default=float('nan'),
                           metavar='MAX_LAT', help=help_max_lat)
 
     # Min time
     help_min_time = """
     The start of the time interval within the dataset times to be processed.
     The time should be provided as a string with the format yyyy-mm-ddTHH:MM:SS
     where yyyy is year, mm is month, dd is day, HH is hour from 00 to 23, MM is
@@ -176,14 +176,23 @@
     Plots the results. In this case, instead of iterating through all time
     frames, only one time frame (given with option -t) is restored and plotted.
     If in addition, the uncertainty quantification is enabled (with option -u),
     the statistical analysis for the given time frame is also plotted.
     """
     optional.add_argument('-p', action='store_true', help=help_plot)
 
+    # Save
+    help_save = """
+    If `True`, the plots are not displayed, rather are saved in the current
+    directory as ``.pdf`` and ``.svg`` format. This option is useful when
+    executing this script in an environment without display (such as remote
+    cluster). If `False`, the generated plots will be displayed.
+    """
+    optional.add_argument('-s', action='store_true', help=help_save)
+
     # Detect land
     help_detect_land = """
     Detect land and exclude it from ocean's missing data points. This option
     should be an boolean or an integer with the following values
     (default: %(default)s):
 
     - False: Same as 0. See below.
@@ -285,15 +294,15 @@
     Scale velocity error of the input data by a factor. Often, the input
     velocity error is the dimensionless GDOP which needs to be scaled by the
     standard deviation of the velocity error to represent the actual velocity
     error. This value scales the error. This option is only relevant to
     uncertainty quantification (when -u is used).
     (default: %(default)s)
     """
-    optional.add_argument('-S', default=0.08, type=float,
+    optional.add_argument('-E', default=0.08, type=float,
                           metavar="SCALE_ERROR", help=help_scale_error)
 
     # Start file index
     help_min_file_index = """
     Start file iterator to be used for processing multiple input files. For
     Instance, ``-i input -I 003 -J 012`` means to read the series of input
     files with iterators ``input003.nc``, ``input004.nc``, to ``input012.nc``.
@@ -314,14 +323,26 @@
 
     # Verbose
     help_verbose = """
     Prints verbose information.
     """
     optional.add_argument('-v', action='store_true', help=help_verbose)
 
+    # Terminate
+    help_terminate = """
+    If `True`, the program exists with code 1. This is useful when this
+    package is executed on a server to pass exit signals to a Node application.
+    On the downside, this option causes an interactive python environment to
+    both terminate the script and the python environment itself. To avoid this,
+    set this option to `False`. In this case, upon an error, the ``ValueError`
+    is raised, which cases the script to terminate, however, an interactive
+    python environment will not be exited.
+    """
+    optional.add_argument('-T', action='store_true', help=help_terminate)
+
     # Version
     help_version = """
     Prints version.
     """
     version = '%(prog)s {version}'.format(version=__version__)
     parser.add_argument('-V', '--version', action='version', version=version,
                         help=help_version)
@@ -338,27 +359,29 @@
         'output': args.o,
         'min_lon': args.min_lon,
         'max_lon': args.max_lon,
         'min_lat': args.min_lat,
         'max_lat': args.max_lat,
         'min_time': args.min_time,
         'max_time': args.max_time,
-        'time': args.t,
+        'time': args.time,
         'diffusivity': args.d,
         'sweep': args.s,
         'plot': args.p,
+        'save': args.S,
         'detect_land': args.L,
         'fill_coast': args.l,
         'convex_hull': args.c,
         'alpha': args.a,
         'refine_grid': args.r,
         'uncertainty_quant': args.u,
         'num_ensembles': args.e,
         'ratio_num_modes': args.m,
         'kernel_width': args.w,
-        'scale_error': args.S,
+        'scale_error': args.E,
         "min_file_index": args.I,
         "max_file_index": args.J,
         "verbose": args.v,
+        "terminate": args.T,
     }
 
     return arguments
```

### Comparing `restoreio-0.3.1/restoreio/_plots/_display_utilities.py` & `restoreio-0.3.2/restoreio/_plots/_display_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots/_draw_map.py` & `restoreio-0.3.2/restoreio/_plots/_draw_map.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots/_plot_grid.py` & `restoreio-0.3.2/restoreio/_plots/_plot_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots/_plot_quiver.py` & `restoreio-0.3.2/restoreio/_plots/_plot_quiver.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots/_plot_streamlines.py` & `restoreio-0.3.2/restoreio/_plots/_plot_streamlines.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots/_plot_utilities.py` & `restoreio-0.3.2/restoreio/_plots/_plot_utilities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots/_plot_velocities.py` & `restoreio-0.3.2/restoreio/_plots/_plot_velocities.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots/plot_results.py` & `restoreio-0.3.2/restoreio/_plots/plot_results.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/__init__.py` & `restoreio-0.3.2/restoreio/_plots_uq/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/_refine_mask.py` & `restoreio-0.3.2/restoreio/_plots_uq/_refine_mask.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/_shifted_colormap.py` & `restoreio-0.3.2/restoreio/_plots_uq/_shifted_colormap.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/plot_auto_correlation.py` & `restoreio-0.3.2/restoreio/_plots_uq/plot_auto_correlation.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/plot_convergence.py` & `restoreio-0.3.2/restoreio/_plots_uq/plot_convergence.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/plot_cor_cov.py` & `restoreio-0.3.2/restoreio/_plots_uq/plot_cor_cov.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/plot_ensembles_stat.py` & `restoreio-0.3.2/restoreio/_plots_uq/plot_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/plot_kl_transform.py` & `restoreio-0.3.2/restoreio/_plots_uq/plot_kl_transform.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/plot_rbf_kernel.py` & `restoreio-0.3.2/restoreio/_plots_uq/plot_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py` & `restoreio-0.3.2/restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_restore/__init__.py` & `restoreio-0.3.2/restoreio/_restore/__init__.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_restore/_make_array_masked.py` & `restoreio-0.3.2/restoreio/_restore/_make_array_masked.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_restore/refine_grid.py` & `restoreio-0.3.2/restoreio/_restore/refine_grid.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_restore/restore_generated_ensembles.py` & `restoreio-0.3.2/restoreio/_restore/restore_generated_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_restore/restore_main_ensemble.py` & `restoreio-0.3.2/restoreio/_restore/restore_main_ensemble.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_scripts/scan_netcdf.py` & `restoreio-0.3.2/restoreio/_scripts/scan.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,161 +15,153 @@
 
 import numpy
 import sys
 import warnings
 import netCDF4
 import pyncml
 import os.path
-import getopt
 import datetime
 import json
 
+import argparse
+from .._parser.formatter import WrappedNewlineFormatter
+from .examples import examples
+from ..__version__ import __version__
+
 try:
     # For python 3
     from urllib.parse import urlparse
 except ImportError:
     # For python 2
     from urlparse import urlparse
 
+__all__ = ['scan']
+
 
 # ====================
 # Terminate With Error
 # ====================
 
-def _terminate_with_error(message):
+def _terminate_with_error(message, terminate=False):
     """
     Returns an incomplete Json object with ScanStatus = False, and an error
     message.
+
+    If terminate is True, the python program is exited with code 1. If False,
+    a valueError is raised without terminating the program.
     """
 
-    # Fill output with defaults
-    dataset_info_dict = {
-        "Scan": {
-            "ScanStatus": False,
-            "Message": message
+    if terminate:
+
+        # Fill output with defaults
+        dataset_info_dict = {
+            "Scan": {
+                "ScanStatus": False,
+                "Message": message
+            }
         }
-    }
 
-    # Print out and exit gracefully
-    dataset_info_json = json.dumps(dataset_info_dict, indent=4)
-    print(dataset_info_json)
-    sys.stdout.flush()
-    sys.exit()
+        # Print out and exit gracefully
+        dataset_info_json = json.dumps(dataset_info_dict, indent=4)
+        print(dataset_info_json)
+        sys.stdout.flush()
+        sys.exit(1)
+
+    else:
+        raise ValueError(message)
 
 
 # ===============
 # Parse Arguments
 # ===============
 
 def _parse_arguments(argv):
     """
     Parses the argument of the executable and obtains the filename.
-
-    Input file is netcdf nc file or ncml file.
-    Output is a stratified Json.
     """
 
-    # -------------
-    # Print Version
-    # -------------
-
-    def _print_version():
-
-        version_string = \
-            """
-Version 0.0.1
-Siavash Ameli
-University of California, Berkeley
-            """
-
-        print(version_string)
-
-    # -----------
-    # Print Usage
-    # -----------
-
-    def _print_usage(exec_name):
-        usage_string = "Usage: " + exec_name + \
-            " -i <input_filename.{nc, ncml}>"
-        options_string = \
-            """
-Required arguments:
-
-    -i --input          Input filename. This should be full path. Input file
-                        extension can be *.nc or *.ncml.
-
-Optional arguments:
-
-    -h --help           Prints this help message.
-    -v --version        Prints the version and author info.
-    -V --Velocity       Scans Velocities in the dataset.
-                """
-        example_string = \
-            """
-Examples:
-
-    1. Using a url on a remote machine. This will not scan the velocities.
-       $ %s -i <url>
-
-    2. Using a filename on the local machine. This will not scan the velocities
-       $ %s -i <filename>
-
-    3. Scan velocities form a url or filename:
-       $ %s -V -i <url or filename>
-                """ % (exec_name, exec_name, exec_name)
-
-        print(usage_string)
-        print(options_string)
-        print(example_string)
-
-    # -----------------
-
-    # Initialize variables (defaults)
-    input_filename = ''
-    scan_velocity_status = False
-
-    try:
-        opts, args = getopt.getopt(argv[1:], "hvVi:",
-                                   ["help", "version", "Velocity", "input="])
-    except getopt.GetoptError:
-        _print_usage(argv[0])
-        sys.exit(2)
-
-    # Assign options
-    for opt, arg in opts:
-
-        if opt in ('-h', '--help'):
-            _print_usage(argv[0])
-            sys.exit()
-        elif opt in ('-v', '--version'):
-            _print_version()
-            sys.exit()
-        elif opt in ("-i", "--input"):
-            input_filename = arg
-        elif opt in ("-V", "--Velocity"):
-            scan_velocity_status = True
-
-    # Check Arguments
-    if len(argv) < 2:
-        _print_usage(argv[0])
-        sys.exit(0)
-
-    # Check input_filename
-    if (input_filename == ''):
-        _print_usage(argv[0])
-        _terminate_with_error("Input filename or url is empty.")
+    # Instantiate the parser
+    description = 'Restore incomplete oceanographic dataset. ' + \
+        '"restore" is provided by "restoreio" python package.'
+    epilog = examples
+    # formatter_class = argparse.RawTextHelpFormatter
+    # formatter_class = argparse.ArgumentDefaultsHelpFormatter
+    # formatter_class = DescriptionWrappedNewlineFormatter
+    formatter_class = WrappedNewlineFormatter
+
+    parser = argparse.ArgumentParser(description=description, epilog=epilog,
+                                     formatter_class=formatter_class,
+                                     add_help=False)
+
+    # Manually create two groups of required and optional arguments
+    parser._action_groups.pop()
+    required = parser.add_argument_group('required arguments')
+    optional = parser.add_argument_group('optional arguments')
+
+    # Add back help
+    optional.add_argument('-h', '--help', action='help',
+                          default=argparse.SUPPRESS,
+                          help='show this help message and exit')
+
+    # Input filename
+    help_input = """
+    Input filename. This can be either the path to a local file or the url to
+    a remote dataset. The file extension should be *.nc or *.ncml only.
+    """
+    required.add_argument('-i', type=str, help=help_input, metavar='INPUT',
+                          required=True)
+
+    # Scan velocities
+    help_scan_velocities = """
+    Scans the velocity arrays of the file. This is useful to find the min and
+    max range of the velocity data to adjust the color bar for plotting.
+    """
+    optional.add_argument('-V', action='store_true', help=help_scan_velocities)
+
+    # Terminate
+    help_terminate = """
+    If `True`, the program exists with code 1. This is useful when this
+    package is executed on a server to pass exit signals to a Node application.
+    On the downside, this option causes an interactive python environment to
+    both terminate the script and the python environment itself. To avoid this,
+    set this option to `False`. In this case, upon an error, the ``ValueError`
+    is raised, which cases the script to terminate, however, an interactive
+    python environment will not be exited.
+    """
+    optional.add_argument('-T', action='store_true', help=help_terminate)
+
+    # Version
+    help_version = """
+    Prints version.
+    """
+    version = '%(prog)s {version}'.format(version=__version__)
+    parser.add_argument('-V', '--version', action='version', version=version,
+                        help=help_version)
+
+    # Parse arguments. Here args is a namespace
+    args = parser.parse_args()
+
+    # Convert namespace to dictionary
+    # args = vars(args)
+
+    # Output dictionary
+    arguments = {
+        'input': args.i,
+        'scan_velocities': args.V,
+        'terminate': args.T,
+    }
 
-    return input_filename, scan_velocity_status
+    return arguments
 
 
 # ==================
 # Load Local Dataset
 # ==================
 
-def _load_local_dataset(filename):
+def _load_local_dataset(filename, terminate):
     """
     Opens either ncml or nc file and returns the aggregation file object.
     """
 
     # Check file extension
     file_extension = os.path.splitext(filename)[1]
     if file_extension in ['.ncml', '.ncml.gz']:
@@ -203,31 +195,34 @@
             "File format %s is not recognized." % file_extension)
 
 
 # ===================
 # Load Remote Dataset
 # ===================
 
-def _load_remote_dataset(url):
+def _load_remote_dataset(url, terminate):
     """
     URL can be point to a *.nc or *.ncml file.
     """
 
     # Check URL is opendap
     if (url.startswith('http://') is False) and \
        (url.startswith('https://') is False):
         _terminate_with_error('Input data URL does not seem to be a URL. ' +
                               'A URL should start with <code>http://</code> ' +
-                              'or <code>https://</code>.')
+                              'or <code>https://</code>.',
+                              terminate)
+
     elif ("/thredds/dodsC/" not in url) and ("opendap" not in url):
         _terminate_with_error('Input data URL is not an <b>OpenDap</b> URL ' +
                               'or is not hosted on a THREDDs server. Check ' +
                               'if your data URL contains ' +
                               '<code>/thredds/dodsC/</code> or ' +
-                              '<code>/opendap/</code>.')
+                              '<code>/opendap/</code>.',
+                              terminate)
 
     # Check file extension
     file_extension = os.path.splitext(url)[1]
 
     # Case of zipped files (get the correct file extension before the '.gz')
     if file_extension == ".gz":
         file_extension = os.path.splitext(url[:-3])[1]
@@ -238,50 +233,52 @@
         # If a file extension exists, check if it is a standard netcdf file
         if file_extension not in \
                 ['.nc', '.ncd', '.nc.gz', '.ncml', '.ncml.gz']:
             _terminate_with_error(
                 'The input data URL is not an <i>netcdf</i> file. The URL ' +
                 'should end with <code>.nc</code>, <code>.ncd</code>, ' +
                 '<code>.nc.gz</code>, <code>.ncml</code>, ' +
-                '<code>.ncml.gz</code>, or without file extension.')
+                '<code>.ncml.gz</code>, or without file extension.',
+                terminate)
 
     try:
         # nc = open_url(url)
         nc = netCDF4.Dataset(url)
 
     except OSError:
-        _terminate_with_error('Unable to read %s.' % url)
+        _terminate_with_error('Unable to read %s.' % url, terminate)
 
     return nc
 
 
 # ============
 # Load Dataset
 # ============
 
-def _load_dataset(input_filename):
+def _load_dataset(input, terminate):
     """
     Dispatches the execution to either of the following two functions:
-    1. LoadMultiFileDataset: For files where the input_filename is a path on
+    1. LoadMultiFileDataset: For files where the input is a path on
        the local machine.
-    2. _load_remote_dataset: For files remotely where input_filename is a URL.
+    2. _load_remote_dataset: For files remotely where input is a URL.
     """
 
     # Check input filename
-    if input_filename == '':
+    if input == '':
         _terminate_with_error('Input data URL is empty. You should provide ' +
-                              'an OpenDap URL.')
+                              'an OpenDap URL.',
+                              terminate)
 
-    # Check if the input_filename has a "host" name
-    if bool(urlparse(input_filename).netloc):
-        # input_filename is a URL
-        return _load_remote_dataset(input_filename)
+    # Check if the input has a "host" name
+    if bool(urlparse(input).netloc):
+        # input is a URL
+        return _load_remote_dataset(input, terminate)
     else:
-        # input_filename is a path
-        return _load_local_dataset(input_filename)
+        # input is a path
+        return _load_local_dataset(input, terminate)
 
 
 # ===============
 # Search Variable
 # ===============
 
 def _search_variable(agg, names_list, standard_names_list):
@@ -332,15 +329,15 @@
     return obj, obj_name, obj_standard_name
 
 
 # =============================
 # Load Time And Space Variables
 # =============================
 
-def _load_time_and_space_variables(agg):
+def _load_time_and_space_variables(agg, terminate):
     """
     Finds the following variables from the aggregation object agg.
 
     - Time
     - Longitude
     - Latitude
     """
@@ -350,58 +347,58 @@
     time_standard_names_list = ['time']
     datetime_obj, datetime_name, datetime_standard_name = _search_variable(
         agg, time_names_list, time_standard_names_list)
 
     # Check time variable
     if datetime_obj is None:
         _terminate_with_error('Can not find the <i>time</i> variable in ' +
-                              'the netcdf file.')
+                              'the netcdf file.', terminate)
     elif hasattr(datetime_obj, 'units') is False:
         _terminate_with_error('The <t>time</i> variable does not have ' +
-                              '<i>units</i> attribute.')
+                              '<i>units</i> attribute.', terminate)
     # elif hasattr(datetime_obj, 'calendar') is False:
     #     _terminate_with_error('The <t>time</i> variable does not have ' +
-    #                           '<i>calendar</i> attribute.')
-    elif datetime_obj.size < 2:
-        _terminate_with_error('The <i>time</i> variable size should be at ' +
-                              'least <tt>2</tt>.')
+    #                           '<i>calendar</i> attribute.', terminate)
+    # elif datetime_obj.size < 2:
+    #     _terminate_with_error('The <i>time</i> variable size should be at ' +
+    #                           'least <tt>2</tt>.', terminate)
 
     # Longitude
     longitude_names_list = ['longitude', 'lon', 'long']
     longitude_standard_names_list = ['longitude']
     longitude_obj, longitude_name, longitude_standard_name = _search_variable(
         agg, longitude_names_list, longitude_standard_names_list)
 
     # Check longitude variable
     if longitude_obj is None:
         _terminate_with_error('Can not find the <i>longitude</i> variable ' +
-                              'in the netcdf file.')
+                              'in the netcdf file.', terminate)
     elif len(longitude_obj.shape) != 1:
         _terminate_with_error('The <t>longitude</i> variable dimension ' +
-                              'should be <tt>1<//t>.')
+                              'should be <tt>1<//t>.', terminate)
     elif longitude_obj.size < 2:
         _terminate_with_error('The <i>longitude</i> variable size should ' +
-                              'be at least <tt>2</tt>.')
+                              'be at least <tt>2</tt>.', terminate)
 
     # Latitude
     latitude_names_list = ['latitude', 'lat']
     latitude_standard_names_list = ['latitude']
     latitude_obj, latitude_name, latitude_standard_name = _search_variable(
         agg, latitude_names_list, latitude_standard_names_list)
 
     # Check latitude variable
     if latitude_obj is None:
         _terminate_with_error('Can not find the <i>latitude</i> variable in ' +
-                              'the netcdf file.')
+                              'the netcdf file.', terminate)
     elif len(latitude_obj.shape) != 1:
         _terminate_with_error('The <t>latitude</i> variable dimension ' +
-                              'should be <tt>1<//t>.')
+                              'should be <tt>1<//t>.', terminate)
     elif latitude_obj.size < 2:
         _terminate_with_error('The <i>latitude</i> variable size should ' +
-                              'be at least <tt>2</tt>.')
+                              'be at least <tt>2</tt>.', terminate)
 
     return datetime_obj, longitude_obj, latitude_obj
 
 
 # =======================
 # Load Velocity Variables
 # =======================
@@ -437,15 +434,15 @@
         north_velocity_standard_name
 
 
 # =================
 # Prepare datetimes
 # =================
 
-def _prepare_datetimes(datetime_obj):
+def _prepare_datetimes(datetime_obj, terminate):
     """
     This is used in writer function.
     Converts date char format to datetime numeric format.
     This parses the times chars and converts them to date times.
     """
 
     # datetimes units
@@ -494,30 +491,30 @@
             days_list.append(datetime.datetime(
                 year, month, day, hour, minute, second))
 
         # Convert dates to numbers
         datetimes = netCDF4.date2num(days_list, units=datetimes_unit,
                                      calendar=datetimes_calendar)
     else:
-        _terminate_with_error("Datetime ndim is more than 2.")
+        _terminate_with_error("Datetime ndim is more than 2.", terminate)
 
     return datetimes, datetimes_unit, datetimes_calendar
 
 
 # =============
 # Get Time Info
 # =============
 
-def _get_time_info(datetime_obj):
+def _get_time_info(datetime_obj, terminate):
     """
     Get the initial time info and time duration.
     """
 
     datetimes, datetimes_unit, datetimes_calendar = \
-        _prepare_datetimes(datetime_obj)
+        _prepare_datetimes(datetime_obj, terminate)
 
     # Initial time
     initial_time = datetimes[0]
     initial_datetime_obj = netCDF4.num2date(
         initial_time, units=datetimes_unit, calendar=datetimes_calendar)
 
     initial_time_dict = {
@@ -806,15 +803,15 @@
     return velocity_name
 
 
 # =====================
 # Get Array Memory Size
 # =====================
 
-def _get_array_memory_size(array):
+def _get_array_memory_size(array, terminate):
     """
     If array ndim is three, such as (time, lat, lon), this function returns
     the size of array(0, :, :).
 
     If array ndim is four, such as (time, depth, lat, lon), this function
     returns the size of array(0, 0, :, :).
     """
@@ -823,15 +820,16 @@
     if array.ndim == 3:
         shape = array.shape[1:]
         itemsize = array[0, 0, :0].itemsize
     elif array.ndim == 4:
         shape = array.shape[2:]
         itemsize = array[0, 0, 0, :0].itemsize
     else:
-        _terminate_with_error('Array ndim should be three or four.')
+        _terminate_with_error('Array ndim should be three or four.',
+                              terminate)
 
     # Size of array (excluding time and depth dimensions)
     size = numpy.prod(shape)
 
     # Size of array in bytes
     num_bytes = size * itemsize
 
@@ -844,24 +842,25 @@
 
 def _get_velocity_info(
         east_velocity_obj,
         north_velocity_obj,
         east_velocity_name,
         north_velocity_name,
         east_velocity_standard_name,
-        north_velocity_standard_name):
+        north_velocity_standard_name,
+        terminate):
     """
     Get dictionary of velocities.
     """
 
     # Get the number of indices to be selected for finding min and max.
     num_times = east_velocity_obj.shape[0]
 
     # Get the size of one of the velocity arrays
-    num_bytes = _get_array_memory_size(east_velocity_obj)
+    num_bytes = _get_array_memory_size(east_velocity_obj, terminate)
     num_Mbytes = num_bytes / (1024**2)
 
     # Number of time instances to sample from velocity data
     if num_Mbytes >= 10.0:
         # If the array is larger than 10 MB, sample only one time of array
         num_time_indices = 1
     elif num_Mbytes >= 1.0:
@@ -870,16 +869,23 @@
         num_time_indices = 5
 
     # Cap the number of time samples by the number of times
     if num_time_indices > num_times:
         num_time_indices = num_times
 
     # The selection of random time indices to be used for finding min and max
-    numpy.random.seed(0)
-    times_indices = numpy.random.randint(0, num_times - 1, num_time_indices)
+    if num_times > 1:
+        numpy.random.seed(0)
+        times_indices = numpy.random.randint(0, num_times - 1,
+                                             num_time_indices)
+    elif num_times == 1:
+        times_indices = [0]
+    else:
+        _terminate_with_error('Velocity array time dimension has zero size.',
+                              terminate)
 
     # Min/Max velocities for each time frame
     east_velocities_mean = numpy.zeros(len(times_indices), dtype=float)
     east_velocities_std = numpy.zeros(len(times_indices), dtype=float)
     north_velocities_mean = numpy.zeros(len(times_indices), dtype=float)
     north_velocities_std = numpy.zeros(len(times_indices), dtype=float)
 
@@ -913,15 +919,16 @@
                     east_velocity_obj[time_index, depth_index, :, :])
                 north_velocities_mean[k] = numpy.nanmean(
                     north_velocity_obj[time_index, depth_index, :, :])
                 north_velocities_std[k] = numpy.nanstd(
                     north_velocity_obj[time_index, depth_index, :, :])
 
             else:
-                _terminate_with_error('Velocity ndim should be three or four.')
+                _terminate_with_error('Velocity ndim should be three or four.',
+                                      terminate)
 
     # Mean and STD of Velocities among all time frames
     east_velocity_mean = numpy.nanmean(east_velocities_mean)
     east_velocity_std = numpy.nanmean(east_velocities_std)
     north_velocity_mean = numpy.nanmean(north_velocities_mean)
     north_velocity_std = numpy.nanmean(north_velocities_std)
 
@@ -963,69 +970,178 @@
     return velocity_info_dict
 
 
 # ====
 # scan
 # ====
 
-def scan(argv):
+def scan(
+        input,
+        scan_velocity=False,
+        terminate=False):
     """
     Reads a netcdf file and returns data info.
 
-    Notes:
+    Parameters
+    ----------
 
-        - If the option -V is used to scan min and max of velocities,
-          we do not find the min and max of velocity for all time frames. This
-          is because if the nc file is large, it takes a long time. Also we do
-          not load the whole velocities like U[:] or V[:] because it the data
-          is large, the netCDF4 package raises an error.
+    input : str
+        The input netcdf file URL (if remote file) or file name (if local
+        data). The URL should either have no extension, if it does have an
+        extension, the file extension should be either of ``.nc``, ``.nc.gz``,
+        ``.ncd``, ``.ncml``, or ``.ncml.gz``.
+
+    scan_velocities : bool, default=False
+        Scans the velocity arrays of the file. This is useful to find the min
+        and max range of the velocity data to adjust the color bar for
+        plotting.
+
+    terminate : bool, default=False
+        If `True`, the program exists with code 1. This is useful when this
+        package is executed on a server to pass exit signals to a Node
+        application. On the downside, this option causes an interactive python
+        environment to both terminate the script and the python environment
+        itself. To avoid this, set this option to `False`. In this case, upon
+        an error, the ``ValueError` is raised, which cases the script to
+        terminate, however, an interactive python environment will not be
+        exited.
+
+    Notes
+    -----
+
+    * If the option -V is used to scan min and max of velocities, we do not
+      find the min and max of velocity for all time frames. This is because if
+      the nc file is large, it takes a long time. Also we do not load the whole
+      velocities like U[:] or V[:] because it the data is large, the netCDF4
+      package raises an error.
+
+    Examples
+    --------
+
+    .. code-block:: python
+
+        >>> from restoreio import scan
+        >>> input = 'http://transport.me.berkeley.edu/thredds/dodsC/root/' + \
+        ...         'WHOI-HFR/WHOI_HFR_2014_original.nc'
+
+        >>> # Run script
+        >>> scan(input, scan_velocities=True, terminate=False)
+        {
+            "Scan": {
+                "ScanStatus": true,
+                "Message": ""
+            },
+            "TimeInfo": {
+                "InitialTime": {
+                    "Year": "2014",
+                    "Month": "07",
+                    "Day": "01",
+                    "Hour": "00",
+                    "Minute": "00",
+                    "Second": "00",
+                    "Microsecond": "000000"
+                },
+                "FinalTime": {
+                    "Year": "2014",
+                    "Month": "09",
+                    "Day": "30",
+                    "Hour": "23",
+                    "Minute": "29",
+                    "Second": "59",
+                    "Microsecond": "000000"
+                },
+                "TimeDuration": {
+                    "Day": "91",
+                    "Hour": "23",
+                    "Minute": "29",
+                    "Second": "59"
+                },
+                "TimeDurationInSeconds": "7946999.0",
+                "DatetimeSize": "4416"
+            },
+            "SpaceInfo": {
+                "DataResolution": {
+                    "LongitudeResolution": "39",
+                    "LatitudeResolution": "36"
+                },
+                "DataBounds": {
+                    "MinLatitude": "41.08644",
+                    "MidLatitude": "41.212500000000006",
+                    "MaxLatitude": "41.33856",
+                    "MinLongitude": "-70.797912",
+                    "MidLongitude": "-70.616667",
+                    "MaxLongitude": "-70.435422"
+                },
+                "DataRange": {
+                    "LongitudeRange": "30355.79907013849",
+                    "LatitudeRange": "28065.8700187999",
+                    "ViewRange": "42498.11869819389",
+                    "PitchAngle": "45.06303"
+                },
+                "CameraBounds": {
+                    "MinLatitude": "41.036086627216",
+                    "MaxLatitude": "41.388913372784",
+                    "MinLongitude": "-70.87033700055551",
+                    "MaxLongitude": "-70.3629969994445"
+                }
+            },
+            "VelocityInfo": {
+                "EastVelocityName": "East_vel",
+                "NorthVelocityName": "North_vel",
+                "EastVelocityStandardName": "eastward_wind",
+                "NorthVelocityStandardName": "northward_wind",
+                "VelocityStandardName": "wind",
+                "MinEastVelocity": "-0.48760945773342956",
+                "MaxEastVelocity": "0.3507359965788057",
+                "MinNorthVelocity": "-0.36285106142279266",
+                "MaxNorthVelocity": "0.312877327708193",
+                "TypicalVelocitySpeed": "0.6121967517719955"
+            }
+        }
     """
 
     # Fill output with defaults
     dataset_info_dict = {
         "Scan": {
             "ScanStatus": True,
             "Message": ""
         },
         "TimeInfo": None,
         "SpaceInfo": None,
         "VelocityInfo": None
     }
 
-    # Parse arguments
-    input_filename, scan_velocity_status = _parse_arguments(argv)
-
     # Open file
-    agg = _load_dataset(input_filename)
+    agg = _load_dataset(input, terminate)
 
     # Load variables
     datetime_obj, longitude_obj, latitude_obj = \
-        _load_time_and_space_variables(agg)
+        _load_time_and_space_variables(agg, terminate)
 
     # Get Time Info
-    time_info_dict = _get_time_info(datetime_obj)
+    time_info_dict = _get_time_info(datetime_obj, terminate)
     dataset_info_dict['TimeInfo'] = time_info_dict
 
     # Get Space Info
     space_info_dict = _get_space_info(longitude_obj, latitude_obj)
     dataset_info_dict['SpaceInfo'] = space_info_dict
 
     # Velocities
-    if scan_velocity_status is True:
+    if scan_velocity is True:
 
         # Get velocity objects
         east_velocity_obj, north_velocity_obj, east_velocity_name, \
             north_velocity_name, east_velocity_standard_name, \
             north_velocity_standard_name = _load_velocity_variables(agg)
 
         # Read velocity data and find info
         velocity_info_dict = _get_velocity_info(
             east_velocity_obj, north_velocity_obj, east_velocity_name,
             north_velocity_name, east_velocity_standard_name,
-            north_velocity_standard_name)
+            north_velocity_standard_name, terminate)
 
         # Store in dictionary
         dataset_info_dict['VelocityInfo'] = velocity_info_dict
 
     agg.close()
 
     dataset_info_json = json.dumps(dataset_info_dict, indent=4)
@@ -1043,16 +1159,19 @@
     """
 
     # Converting all warnings to error
     # warnings.simplefilter('error', UserWarning)
     warnings.filterwarnings("ignore", category=numpy.VisibleDeprecationWarning)
     warnings.filterwarnings("ignore", category=DeprecationWarning)
 
+    # Parse arguments
+    arguments = _parse_arguments(sys.argv)
+
     # Main function
-    scan(sys.argv)
+    scan(**arguments)
 
 
 # ===========
 # Script Main
 # ===========
 
 if __name__ == "__main__":
```

### Comparing `restoreio-0.3.1/restoreio/_subset/_array_utilities.py` & `restoreio-0.3.2/restoreio/_subset/_array_utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,23 +17,30 @@
 __all__ = ['terminate_with_error', 'check_monotonicity', 'find_closest_index']
 
 
 # ====================
 # Terminate With Error
 # ====================
 
-def terminate_with_error(message):
+def terminate_with_error(message, terminate):
     """
     Terminate gracefully with exit code 1. This is used to print error message
     in Restore website.
+
+    If terminate is True, the python program is exited with code 1. If False,
+    only a ValueError is raised, but an interactive python environment is not
+    exited.
     """
 
-    print('ERROR: ' + message)
-    sys.stdout.flush()
-    sys.exit()
+    if terminate:
+        print('ERROR: ' + message)
+        sys.stdout.flush()
+        sys.exit(1)
+    else:
+        raise ValueError(message)
 
 
 # ==================
 # Check Monotonicity
 # ==================
 
 def check_monotonicity(array, array_name):
```

### Comparing `restoreio-0.3.1/restoreio/_uncertainty_quant/_compute_correlation_matrix.py` & `restoreio-0.3.2/restoreio/_uncertainty_quant/_compute_correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py` & `restoreio-0.3.2/restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_uncertainty_quant/_image_utils.py` & `restoreio-0.3.2/restoreio/_uncertainty_quant/_image_utils.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_uncertainty_quant/_statistical_distances.py` & `restoreio-0.3.2/restoreio/_uncertainty_quant/_statistical_distances.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_uncertainty_quant/generate_image_ensembles.py` & `restoreio-0.3.2/restoreio/_uncertainty_quant/generate_image_ensembles.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio/_uncertainty_quant/get_ensembles_stat.py` & `restoreio-0.3.2/restoreio/_uncertainty_quant/get_ensembles_stat.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/restoreio.egg-info/PKG-INFO` & `restoreio-0.3.2/restoreio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: restoreio
-Version: 0.3.1
+Version: 0.3.2
 Summary: Reconstruct incomplete oceanographic dataset
 Home-page: https://github.com/ameli/restoreio
 Download-URL: https://github.com/ameli/restoreio/archive/main.zip
 Author: Siavash Ameli
 Author-email: sameli@berkeley.edu
 Project-URL: Documentation, https://github.com/ameli/restoreio/blob/main/README.rst
 Project-URL: Source, https://github.com/ameli/restoreio
```

### Comparing `restoreio-0.3.1/restoreio.egg-info/SOURCES.txt` & `restoreio-0.3.2/restoreio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 docs/source/_templates/version.html
 docs/source/_templates/autosummary/attribute.rst
 docs/source/_templates/autosummary/class.rst
 docs/source/_templates/autosummary/method.rst
 docs/source/_templates/autosummary/ndarray_subclass.rst
 docs/source/_templates/autosummary/property.rst
 docs/source/generated/restoreio.restore.rst
+docs/source/generated/restoreio.scan.rst
 docs/source/notebooks/quick_start.ipynb
 examples/restore/main_VaryingNumModes.py
 examples/restore/plot_coverage.py
 examples/restore/plot_fixed_size_artificial_mask.py
 examples/restore/plot_variable_d_artificial_masks.py
 examples/restore/plot_variable_size_artificial_masks.py
 examples/uncertainty_quant/_display_utilities.py
@@ -124,21 +125,23 @@
 restoreio/_plots_uq/plot_valid_vector_ensembles_stat.py
 restoreio/_restore/__init__.py
 restoreio/_restore/_make_array_masked.py
 restoreio/_restore/refine_grid.py
 restoreio/_restore/restore_generated_ensembles.py
 restoreio/_restore/restore_main_ensemble.py
 restoreio/_scripts/__init__.py
-restoreio/_scripts/scan_netcdf.py
+restoreio/_scripts/examples.py
+restoreio/_scripts/scan.py
 restoreio/_subset/__init__.py
 restoreio/_subset/_array_utilities.py
 restoreio/_subset/subset_datetime.py
 restoreio/_subset/subset_domain.py
 restoreio/_uncertainty_quant/__init__.py
 restoreio/_uncertainty_quant/_compute_correlation_matrix.py
 restoreio/_uncertainty_quant/_generate_valid_vector_ensembles.py
 restoreio/_uncertainty_quant/_image_utils.py
 restoreio/_uncertainty_quant/_statistical_distances.py
 restoreio/_uncertainty_quant/generate_image_ensembles.py
 restoreio/_uncertainty_quant/get_ensembles_stat.py
 tests/test_restore_local_data.py
-tests/test_restore_remote_data.py
+tests/test_restore_remote_data.py
+tests/test_scan.py
```

### Comparing `restoreio-0.3.1/setup.py` & `restoreio-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         extras_require={
             'test': test_requirements,
             'docs': docs_requirements,
         },
         entry_points={
             "console_scripts": [
                 "restore = restoreio.__main__:main",
-                "scan = restoreio._scripts.scan_netcdf:main"
+                "restore-scan = restoreio._scripts.scan:main"
             ]
         },
         classifiers=[
             'Programming Language :: Python',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
```

### Comparing `restoreio-0.3.1/tests/test_restore_local_data.py` & `restoreio-0.3.2/tests/test_restore_local_data.py`

 * *Files identical despite different names*

### Comparing `restoreio-0.3.1/tests/test_restore_remote_data.py` & `restoreio-0.3.2/tests/test_restore_remote_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,16 +44,19 @@
 # ============
 
 def test_restore():
     """
     Test for `restore` function.
     """
 
+    # The Monterey bay data is commented since often their server is down and
+    # causes this test script to halt.
     # Monterey Bay data
-    # input = 'http://hfrnet-tds.ucsd.edu/thredds/dodsC/HFR/USWC/2km/hourly/' + \
+    # input = 'http://hfrnet-tds.ucsd.edu/thredds/dodsC/HFR/USWC/2km/' + \
+    #         'hourly/' + \
     #         'RTV/HFRADAR_US_West_Coast_2km_Resolution_Hourly_RTV_best.ncd'
     # min_lon = -122.344
     # max_lon = -121.781
     # min_lat = 36.507
     # max_lat = 36.9925
     # time = '2017-01-25T03:00:00'
 
@@ -76,14 +79,15 @@
     # Restore main file
     restore(input, min_file_index='', max_file_index='', output=output,
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
             time=time, sweep=False, detect_land=True, fill_coast=False,
             convex_hull=False, alpha=20, refine_grid=1,
             uncertainty_quant=False, plot=True, verbose=True)
 
+    # These lines are commented since WHOI-HFR data don't have error variables.
     # Uncertainty quantification
     restore(input, min_file_index='', max_file_index='', output=output,
             min_lon=min_lon, max_lon=max_lon, min_lat=min_lat, max_lat=max_lat,
             time=time, sweep=False, detect_land=True, fill_coast=False,
             convex_hull=False, alpha=20, refine_grid=1, uncertainty_quant=True,
             num_ensembles=200, ratio_num_modes=1, kernel_width=5,
             scale_error=0.08, plot=True, verbose=True)
```

### Comparing `restoreio-0.3.1/tox.ini` & `restoreio-0.3.2/tox.ini`

 * *Files identical despite different names*

