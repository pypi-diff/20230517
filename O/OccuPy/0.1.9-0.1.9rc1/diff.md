# Comparing `tmp/OccuPy-0.1.9.tar.gz` & `tmp/OccuPy-0.1.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OccuPy-0.1.9.tar", last modified: Tue Nov 15 11:46:40 2022, max compression
+gzip compressed data, was "OccuPy-0.1.9rc1.tar", last modified: Fri Nov 11 09:59:08 2022, max compression
```

## Comparing `OccuPy-0.1.9.tar` & `OccuPy-0.1.9rc1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.200821 OccuPy-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.188821 OccuPy-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.188821 OccuPy-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2990 2022-11-15 11:46:23.000000 OccuPy-0.1.9/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-11-15 11:46:23.000000 OccuPy-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-15 11:46:23.000000 OccuPy-0.1.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-15 11:46:23.000000 OccuPy-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-15 11:46:23.000000 OccuPy-0.1.9/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.188821 OccuPy-0.1.9/OccuPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-11-15 11:46:40.000000 OccuPy-0.1.9/OccuPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-11-15 11:46:40.000000 OccuPy-0.1.9/OccuPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 11:46:40.000000 OccuPy-0.1.9/OccuPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-15 11:46:40.000000 OccuPy-0.1.9/OccuPy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 11:46:40.000000 OccuPy-0.1.9/OccuPy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-15 11:46:40.000000 OccuPy-0.1.9/OccuPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-15 11:46:40.000000 OccuPy-0.1.9/OccuPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-11-15 11:46:40.200821 OccuPy-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-15 11:46:23.000000 OccuPy-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:23.000000 OccuPy-0.1.9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.188821 OccuPy-0.1.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.192821 OccuPy-0.1.9/docs/Troubleshooting/
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Troubleshooting/chimX_trbl.md
--rw-r--r--   0 runner    (1001) docker     (121)     8197 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Troubleshooting/install_trbl.md
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Troubleshooting/other_trbl.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.192821 OccuPy-0.1.9/docs/Tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.192821 OccuPy-0.1.9/docs/Tutorials/case/
--rw-r--r--   0 runner    (1001) docker     (121)     8146 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Tutorials/case/est_occ.md
--rw-r--r--   0 runner    (1001) docker     (121)     6622 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Tutorials/case/est_res.md
--rw-r--r--   0 runner    (1001) docker     (121)     7816 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Tutorials/case/modification.md
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Tutorials/case/soldef.md
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Tutorials/case/sub_mask.md
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Tutorials/case/supp_solv.md
--rw-r--r--   0 runner    (1001) docker     (121)     6156 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Tutorials/gui.md
--rw-r--r--   0 runner    (1001) docker     (121)    10440 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/Tutorials/intro.md
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-11-15 11:46:23.000000 OccuPy-0.1.9/docs/about.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.192821 OccuPy-0.1.9/docs/gallery/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.192821 OccuPy-0.1.9/docs/gallery/full/
--rw-r--r--   0 runner    (1001) docker     (121)   187920 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/full/14085_1.png
--rw-r--r--   0 runner    (1001) docker     (121)   665788 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/full/14085_2.png
--rw-r--r--   0 runner    (1001) docker     (121)   446444 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/full/14085_3.png
--rw-r--r--   0 runner    (1001) docker     (121)   327224 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/full/14085_4.png
--rw-r--r--   0 runner    (1001) docker     (121)   326839 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/full/14085_5.png
--rw-r--r--   0 runner    (1001) docker     (121)   505703 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/full/14085_6.png
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/highres.md
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/mass.md
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/membrane.md
--rw-r--r--   0 runner    (1001) docker     (121)     2551 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/modification.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.196821 OccuPy-0.1.9/docs/gallery/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/synthetic.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.196821 OccuPy-0.1.9/docs/gallery/thumbs/
--rw-r--r--   0 runner    (1001) docker     (121)   180249 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/actin.png
--rw-r--r--   0 runner    (1001) docker     (121)   200507 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/high-res.png
--rw-r--r--   0 runner    (1001) docker     (121)    30602 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/linux_thumb.png
--rw-r--r--   0 runner    (1001) docker     (121)     9322 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/mac_thumb.png
--rw-r--r--   0 runner    (1001) docker     (121)    84397 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/mass.png
--rw-r--r--   0 runner    (1001) docker     (121)   104152 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/membrane.png
--rw-r--r--   0 runner    (1001) docker     (121)   122562 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/modification.png
--rw-r--r--   0 runner    (1001) docker     (121)    97809 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/resolution.png
--rw-r--r--   0 runner    (1001) docker     (121)   157265 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/ribo.png
--rw-r--r--   0 runner    (1001) docker     (121)   391665 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/spike.png
--rw-r--r--   0 runner    (1001) docker     (121)   146265 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/synthetic.png
--rw-r--r--   0 runner    (1001) docker     (121)     3719 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/gallery/thumbs/win_thumb.png
--rw-r--r--   0 runner    (1001) docker     (121)     3643 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)    12447 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/install.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.196821 OccuPy-0.1.9/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-11-15 11:46:24.000000 OccuPy-0.1.9/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (121)     4321 2022-11-15 11:46:24.000000 OccuPy-0.1.9/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.200821 OccuPy-0.1.9/occupy_lib/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-15 11:46:40.000000 OccuPy-0.1.9/occupy_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     9711 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/args.py
--rw-r--r--   0 runner    (1001) docker     (121)    32291 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/estimate.py
--rw-r--r--   0 runner    (1001) docker     (121)     8938 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/extras.py
--rw-r--r--   0 runner    (1001) docker     (121)    13928 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/map_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    32343 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/occupancy.py
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/occupy.py
--rw-r--r--   0 runner    (1001) docker     (121)   132959 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/occupy_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/percentile_maxima.py
--rw-r--r--   0 runner    (1001) docker     (121)     8843 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/solvent.py
--rw-r--r--   0 runner    (1001) docker     (121)     7727 2022-11-15 11:46:24.000000 OccuPy-0.1.9/occupy_lib/vis.py
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-15 11:46:24.000000 OccuPy-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-15 11:46:24.000000 OccuPy-0.1.9/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-11-15 11:46:24.000000 OccuPy-0.1.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.200821 OccuPy-0.1.9/resources/
--rw-r--r--   0 runner    (1001) docker     (121)   227392 2022-11-15 11:46:24.000000 OccuPy-0.1.9/resources/chimX.png
--rw-r--r--   0 runner    (1001) docker     (121)     7468 2022-11-15 11:46:24.000000 OccuPy-0.1.9/resources/help.txt
--rw-r--r--   0 runner    (1001) docker     (121)    76614 2022-11-15 11:46:24.000000 OccuPy-0.1.9/resources/occupy_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)     5546 2022-11-15 11:46:24.000000 OccuPy-0.1.9/resources/occupy_icon_small.png
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-11-15 11:46:40.200821 OccuPy-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-15 11:46:24.000000 OccuPy-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 11:46:40.200821 OccuPy-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-15 11:46:24.000000 OccuPy-0.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-11-15 11:46:24.000000 OccuPy-0.1.9/tests/test_something.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.166799 OccuPy-0.1.9rc1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.146799 OccuPy-0.1.9rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.150799 OccuPy-0.1.9rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2990 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.154799 OccuPy-0.1.9rc1/OccuPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-11-11 09:59:08.000000 OccuPy-0.1.9rc1/OccuPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-11-11 09:59:08.000000 OccuPy-0.1.9rc1/OccuPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 09:59:08.000000 OccuPy-0.1.9rc1/OccuPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-11 09:59:08.000000 OccuPy-0.1.9rc1/OccuPy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 09:59:08.000000 OccuPy-0.1.9rc1/OccuPy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-11-11 09:59:08.000000 OccuPy-0.1.9rc1/OccuPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-11 09:59:08.000000 OccuPy-0.1.9rc1/OccuPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1877 2022-11-11 09:59:08.166799 OccuPy-0.1.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.154799 OccuPy-0.1.9rc1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.154799 OccuPy-0.1.9rc1/docs/Troubleshooting/
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Troubleshooting/chimX_trbl.md
+-rw-r--r--   0 runner    (1001) docker     (121)     7025 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Troubleshooting/install_trbl.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6024 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Troubleshooting/other_trbl.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.154799 OccuPy-0.1.9rc1/docs/Tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.158799 OccuPy-0.1.9rc1/docs/Tutorials/case/
+-rw-r--r--   0 runner    (1001) docker     (121)     8109 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Tutorials/case/est_occ.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6574 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Tutorials/case/est_res.md
+-rw-r--r--   0 runner    (1001) docker     (121)     7813 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Tutorials/case/modification.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Tutorials/case/soldef.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Tutorials/case/sub_mask.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Tutorials/case/supp_solv.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6182 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Tutorials/gui.md
+-rw-r--r--   0 runner    (1001) docker     (121)    10452 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/Tutorials/intro.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/about.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.158799 OccuPy-0.1.9rc1/docs/gallery/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.162799 OccuPy-0.1.9rc1/docs/gallery/full/
+-rw-r--r--   0 runner    (1001) docker     (121)   187920 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/full/14085_1.png
+-rw-r--r--   0 runner    (1001) docker     (121)   665788 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/full/14085_2.png
+-rw-r--r--   0 runner    (1001) docker     (121)   446444 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/full/14085_3.png
+-rw-r--r--   0 runner    (1001) docker     (121)   327224 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/full/14085_4.png
+-rw-r--r--   0 runner    (1001) docker     (121)   326839 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/full/14085_5.png
+-rw-r--r--   0 runner    (1001) docker     (121)   505703 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/full/14085_6.png
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/highres.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/mass.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/membrane.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/modification.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.162799 OccuPy-0.1.9rc1/docs/gallery/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2837 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/synthetic.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.166799 OccuPy-0.1.9rc1/docs/gallery/thumbs/
+-rw-r--r--   0 runner    (1001) docker     (121)   180249 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/actin.png
+-rw-r--r--   0 runner    (1001) docker     (121)   200507 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/high-res.png
+-rw-r--r--   0 runner    (1001) docker     (121)    30602 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/linux_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (121)     9322 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/mac_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (121)    84397 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/mass.png
+-rw-r--r--   0 runner    (1001) docker     (121)   104152 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/membrane.png
+-rw-r--r--   0 runner    (1001) docker     (121)   122562 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/modification.png
+-rw-r--r--   0 runner    (1001) docker     (121)    97809 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/resolution.png
+-rw-r--r--   0 runner    (1001) docker     (121)   157265 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/ribo.png
+-rw-r--r--   0 runner    (1001) docker     (121)   391665 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/spike.png
+-rw-r--r--   0 runner    (1001) docker     (121)   146265 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/synthetic.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3719 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/gallery/thumbs/win_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3643 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)    12447 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/install.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.166799 OccuPy-0.1.9rc1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (121)     4321 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.166799 OccuPy-0.1.9rc1/occupy_lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-11 09:59:08.000000 OccuPy-0.1.9rc1/occupy_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9711 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/args.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32288 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/estimate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8938 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/extras.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13928 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/map_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32289 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/occupancy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/occupy.py
+-rw-r--r--   0 runner    (1001) docker     (121)   132728 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/occupy_gui.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2157 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/percentile_maxima.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8843 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/solvent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7716 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/occupy_lib/vis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.166799 OccuPy-0.1.9rc1/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)   227392 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/resources/chimX.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7468 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/resources/help.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    76614 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/resources/occupy_icon.png
+-rw-r--r--   0 runner    (1001) docker     (121)     5546 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/resources/occupy_icon_small.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2022-11-11 09:59:08.166799 OccuPy-0.1.9rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 09:59:08.166799 OccuPy-0.1.9rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-11-11 09:58:44.000000 OccuPy-0.1.9rc1/tests/test_something.py
```

### Comparing `OccuPy-0.1.9/.github/workflows/test_and_deploy.yml` & `OccuPy-0.1.9rc1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/.gitignore` & `OccuPy-0.1.9rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/LICENSE` & `OccuPy-0.1.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/OccuPy.egg-info/PKG-INFO` & `OccuPy-0.1.9rc1/OccuPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OccuPy
-Version: 0.1.9
+Version: 0.1.9rc1
 Summary: OccuPy: Estimation of local scale in cryo-EM maps
 Home-page: https://occupy.readthedocs.io/
 Author: Bjoern O. Forsberg
 Author-email: bjorn.forsberg@ki.se
 License: GPLv3
 Project-URL: Source Code, https://github.com/bforsbe/OccuPy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `OccuPy-0.1.9/OccuPy.egg-info/SOURCES.txt` & `OccuPy-0.1.9rc1/OccuPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/PKG-INFO` & `OccuPy-0.1.9rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OccuPy
-Version: 0.1.9
+Version: 0.1.9rc1
 Summary: OccuPy: Estimation of local scale in cryo-EM maps
 Home-page: https://occupy.readthedocs.io/
 Author: Bjoern O. Forsberg
 Author-email: bjorn.forsberg@ki.se
 License: GPLv3
 Project-URL: Source Code, https://github.com/bforsbe/OccuPy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `OccuPy-0.1.9/README.md` & `OccuPy-0.1.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/Troubleshooting/chimX_trbl.md` & `OccuPy-0.1.9rc1/docs/Troubleshooting/chimX_trbl.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/Troubleshooting/install_trbl.md` & `OccuPy-0.1.9rc1/docs/Troubleshooting/install_trbl.md`

 * *Files 19% similar despite different names*

```diff
@@ -32,55 +32,23 @@
     We are not aware of how the installation might have failed on linux. Please submit an 
     <a href="https://github.com/bforsbe/OccuPy/issues">issue</a>, describing your system and observations.
 
 ## The GUI windows looks too big/small/...
 
 On some (e.g. 4K) screens, the high resolution causes graphical elements to be re-scaled. OccuPy knows about this 
 and does its best to get it right, but we have not been able to test on a wide range of screen sizes and resolutions.  
-
-
-=== "On Windows"
-
-    1. Locate the installed occupy.exe program file.  
-    2. Right-click the binary file and choose properties. 
-    3. Under "Compatability", Click "Change high DPI settings"
-    4. Select "Override high DPI scaling behaviour", and change the setting so that scaling is performed by "system". 
-    5. Apply and close.
-    6. Restart OccuPy.
-    
-    If the problem remains unresolved, please <a href="https://github.com/bforsbe/OccuPy/issues">report</a> this to 
-    the developers so that we can make sure that it doesn't happen in the future.
-
-=== "On Mac"
-
-    <br>
-    We have not had any reports of poor scaling of the GUI on Mac.
-    <br>
-    <div class="admonition bug">
-    <p class="admonition-title">Report any issues</p>
-    <p>
-    If your GUI does not look like the image in the "GUI overview" tutorial, please 
-    <a href="https://github.com/bforsbe/OccuPy/issues">report</a> this to the developers so that we can make sure 
-    that it doesn't happen in the future.
-    </p>
-    </div>
-
-=== "On Linux (ubuntu)"
-
-    <br>
-    We have not had any reports of poor scaling of the GUI on Linux systems.
-    <br>
-    <div class="admonition bug">
-    <p class="admonition-title">Report any issues</p>
-    <p>
-    If your GUI does not look like the image in the "GUI overview" tutorial, please 
-    <a href="https://github.com/bforsbe/OccuPy/issues">report</a> this to the developers so that we can make sure 
-    that it doesn't happen in the future.
-    </p>
-    </div>
+<br>
+<div class="admonition bug">
+<p class="admonition-title">Report any issues</p>
+<p>
+If your GUI does not look like the image in the "GUI overview" tutorial, please 
+<a href="https://github.com/bforsbe/OccuPy/issues">report</a> this to the developers so that we can make sure 
+that it doesn't happen in the future.
+</p>
+</div>
 
 
 ## I'd like to install with pip but I don't know how
 To help us make the installation instructions better and help you use python and pip, you can request help 
 <a href="https://form.jotform.com/223012138013033" target="_blank" rel="noopener noreferrer">here</a>. 
 Please try to complete the installation by the instructions
 provided in the install section first, and see if the below can resolve any issues.
```

#### html2text {}

```diff
@@ -17,28 +17,15 @@
 look through existing issues, and submit a new issue/question if you still
 can't make it work. === "On Linux (ubuntu)"
 We are not aware of how the installation might have failed on linux. Please
 submit an issue, describing your system and observations. ## The GUI windows
 looks too big/small/... On some (e.g. 4K) screens, the high resolution causes
 graphical elements to be re-scaled. OccuPy knows about this and does its best
 to get it right, but we have not been able to test on a wide range of screen
-sizes and resolutions. === "On Windows" 1. Locate the installed occupy.exe
-program file. 2. Right-click the binary file and choose properties. 3. Under
-"Compatability", Click "Change high DPI settings" 4. Select "Override high DPI
-scaling behaviour", and change the setting so that scaling is performed by
-"system". 5. Apply and close. 6. Restart OccuPy. If the problem remains
-unresolved, please report this to the developers so that we can make sure that
-it doesn't happen in the future. === "On Mac"
-We have not had any reports of poor scaling of the GUI on Mac.
-Report any issues
-If your GUI does not look like the image in the "GUI overview" tutorial, please
-report this to the developers so that we can make sure that it doesn't happen
-in the future.
-=== "On Linux (ubuntu)"
-We have not had any reports of poor scaling of the GUI on Linux systems.
+sizes and resolutions.
 Report any issues
 If your GUI does not look like the image in the "GUI overview" tutorial, please
 report this to the developers so that we can make sure that it doesn't happen
 in the future.
 ## I'd like to install with pip but I don't know how To help us make the
 installation instructions better and help you use python and pip, you can
 request help here. Please try to complete the installation by the instructions
```

### Comparing `OccuPy-0.1.9/docs/Troubleshooting/other_trbl.md` & `OccuPy-0.1.9rc1/docs/Troubleshooting/other_trbl.md`

 * *Files 12% similar despite different names*

```diff
@@ -27,46 +27,50 @@
    increase it, but this is a bad idea. It is rather better to increase the `--kernel` so that the value of tau 
    is automatically increased. You may also waent to increase `--lowpass/-lp` ot increase the number of sampled 
    pixel `nv`. You can see what paramters were calculated and used by checking the output log file or using the 
    `--verbose` option. Increasing the kernel size and/or lowpass setting permits more confident sampling of the local 
    scale, but does increase the granularity. Usually a kernel size of 5 or 7 is adequate, with nv-values in the 
    range 30-100. Low-pass defaults to 8 or 3*pixel-size, which ever is larger, but depending on resolution and 
    pixel-size this may be adjusted depending on the sought granularity.  
-3. OccuPy puts everything on a scale based on what it estimates as "full" through a non-exhaustive search. It 
+3. **OccuPy** puts everything on a scale based on what it estimates as "full" through a non-exhaustive search. It 
   is non-exhaustive because it's much faster. If the "full" scale is under-estimated, lots of regions will be 
   "over-full", i.e. over-estimated as full. YOu can reduce the `--tile-size ` from its default value 12 to reduce 
   the area of what defines "full" scale, which will narrow the definition and in general increase the value of full 
   occupancy, thus stretching the range of the estimated scale. For high-resolution maps, a very small tile-size 
   makes the local scale approximate the mass of individual atoms.   
 ## There is a sphere of noise surrounding the amplified map
 4. If the confidence is over-estimated, low-scale components will be permitted to be amplified. You can hedge the 
    confidence by using `--hedge-confidence <val>`, where `<val>` is a power, meaning that higher values hedge 
    more. 10 is a reasonable value to try.
 5. Another possible reason for the confidence being over-estimated is that the solvent model mean and/or variance is 
    under-estimated. A typical reason for this is that the solvent has been flattened, such that the solvent is not 
-   gaussian. OccuPy was not designed for this type of reconstruction, since such flattening is typically enforced 
+   gaussian. **OccuPy** was not designed for this type of reconstruction, since such flattening is typically enforced 
    using a mask which has thus already delineated solvent vs non-solvent. 
 6. If the map is not solvent-flattened, and confidence-hedging does not alleviate solvent-amplification surrounding 
    the main map component, use `--solvent-def <mask.mrc>` where the mask is a conventional solvent-mask. This will 
    allow these regions to be omitted during solvent fitting. _This mask does not need to be perfect, and does 
    not limit the modification to areas inside it_. 
 
 ## The estimated scale looks like my local resolution
-OccuPy estimates the scale. The scale decreases due to **both** lower resolution and lower occupancy. Since it 
+**OccuPy** estimates the scale. The scale decreases due to **both** lower resolution and lower occupancy. Since it 
 is not possible to trivially separate these factors, the current approach to estimate occupancy as separate from 
-lower resolution is to low-pass filter the input before estimating the local scale. This is turned on  
+lower resolution is to low-pass filter the input before estimating the local scale. This is turned on by default 
 when amplifying or attenuating the map, to minimize over-amplification of low-scale components that are simply low 
-resolution. If one is just estimating scale, but still wants to reduce resolution-dependent effects, the low-pass 
-filtration before scale-estimation can be used. It should then be combined a low-pass filter 
-to specify the worst resolution among the components for which occupancy is to 
+resolution. If one is just estimating scale but wants to reduce resolution-dependent effects, the low-pass 
+filtration before scale-estimation can be activated by either --lp-scale or --occupancy. It should then be combined 
+with --lowpass/-lp or --resolution/-r to specify the worst resolution among the components for which occupancy is to 
 be estimated. For membrane proteins, see [here](#my-membrane-or-detergent-looks-funny).
 
+In the absence of variable occupancy, local scale does actually approximate the local resolution. If you would like 
+to include resolution-dependent factors during amplification or attenuation (which is not recommended), you can do 
+so by using --raw_scale, which does the opposite of --lp-scale. 
+
 ## My membrane or detergent looks funny 
 Membranes are lower in resolution due to their amorphous nature which cannot be coherently averaged. Because this 
 reduces the local scale, membranes are estimated at low scale. The estimated scale of membranes are thus **not** a 
 measure of relative density or occupancy. The low-pass filtration intended to reduce influence of 
 resolution-dependent scale factors is only an approximate measure, so that the precise meaning of the local scale of 
-membrane and another amorphous regions (as estimated by OccuPy) is not well-defined. The lower scale generally 
+membrane and another amorphous regions (as estimated by **OccuPy**) is not well-defined. The lower scale generally 
 reflects intuition however, and permits weak attenuation to de-emphasize these regions to make visualization easier.
```

### Comparing `OccuPy-0.1.9/docs/Tutorials/case/est_occ.md` & `OccuPy-0.1.9rc1/docs/Tutorials/case/est_occ.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 The following steps highlight factors influencing this, and how to make the necessary adjustments to fit your purpose. 
 
 ---
 
 ## 1. First pass estimate
 1. Open the input map. 
-2. Make sure "occupancy" (just below the modification options is enabled, and estimate the scale. 
+2. Set the scale mode to "occupancy" and estimate the scale. 
 3. Click the button "Launch ChimeraX" to view the output. 
 
 ---
 
 ## 2. Sanity check
 1. Check that the output log does not show any warnings (or errors).
 2. Check the "Conf." tab in the viewer. It should be white where there is "stuff", and black where there is solvent.
```

### Comparing `OccuPy-0.1.9/docs/Tutorials/case/est_res.md` & `OccuPy-0.1.9rc1/docs/Tutorials/case/est_res.md`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 </p>
 </div>
 
 ---
 
 ## 1. First pass estimate
 1. Open the input map. 
-2. Make sure that "occupancy" (just below the modifications options) is **disabled**, and estimate the scale. 
+2. Set the scale mode to "resolution" and estimate the scale. 
 3. Click the button "Launch ChimeraX" to view the output. 
 
 ---
 
 ## 2. Sanity check
 1. Check that the output log does not show any warnings (or errors).
```

### Comparing `OccuPy-0.1.9/docs/Tutorials/case/modification.md` & `OccuPy-0.1.9rc1/docs/Tutorials/case/modification.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 1. Create a solvent definition. There is a separate tutorial for this. 
 2. Alter the input lowpass setting. If you have just optimized your scale-kernel settings, this might be annoying.
 
 ---
 
 ## 3. Estimate occupancy
-Make sure occupancy-mode (just below the modification tabs) is activated, and click "Estimate scale". This will 
+Make sure occupancy-mode is selected just below the modification tabs, and click "Estimate scale". This will 
 re-estimate and set the occupancy-mode estimate as active.
 
 ---
 
 ## 4. Optimize modification
 Consider which modification to use. More than one type can be generated at the same time to generate multiple output 
 maps. The effect of multiple modification types are not additive, i.e. they are not compounded or combined.
```

### Comparing `OccuPy-0.1.9/docs/Tutorials/case/soldef.md` & `OccuPy-0.1.9rc1/docs/Tutorials/case/soldef.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/Tutorials/case/sub_mask.md` & `OccuPy-0.1.9rc1/docs/Tutorials/case/sub_mask.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/Tutorials/case/supp_solv.md` & `OccuPy-0.1.9rc1/docs/Tutorials/case/supp_solv.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 To accurately suppress solvent you primarily have to make sure that the solvent model and confidence is accurate. 
 The following steps highlight factors influencing this, and how to make the necessary adjustments. 
 
 ---
 
 ## 1. Set up the run
 1. Open the input map. 
-2. Estimate the scale. We don't need the scale at this point, but estimating it will 
+2. Set the desired scale mode and estimate the scale. We don't need the scale at this point, but estimating it will 
    also generate the solvent model and confidence. 
 3. Check the solvent model tab next to the output log. You want to see that the green parabola coincides well with 
    the solvent peak around ~0, and that it drops significantly faster than the voxel intensity distribution in black.
    If not, you may need to low-pass the input to a higher value as in step 2 of this tutorial, or use a solvent 
    definition as per this other tutorial. 
 4. Click the confidence tab of the viewer labeled "Conf.", and inspect it. Toggle between this tab and the input to 
    evaluate how well the confidence was estimated.
```

### Comparing `OccuPy-0.1.9/docs/Tutorials/gui.md` & `OccuPy-0.1.9rc1/docs/Tutorials/gui.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,20 +53,20 @@
 </div>
 
 ---
 
 ## Modification options
 In some cases you may want to change the input map based on the scale estimate. This is where you do that. 
 <br><br>
-If the scale you have selected (below the viewer) is in "occupancy" mode (has 'occ' in its name), OccuPy will
-let you use it to modify maps. The active modification will be interactively approximated in the "preview" and "plot"
+If the scale you have selected (below the viewer) is in "occupancy" mode (name has 'occ' in it), OccuPy will
+let you use it to modify. The active modification will be interactively approximated in the "preview" and "plot"
 tab of the viewer.
 <br><br>
-If the scale you have selected (below the viewer) has 'res' in its name, OccuPy will *not* 
-let you use it to modify, and inactivate the "preview" tab of the viewer and the "Modify Map" button.  
+If the scale you have selected (below the viewer) is in "resolution" mode (name has 'res' in it), OccuPy will *not* 
+let you use it to modify, which will inactivate the "preview" tab of the viewer and the "Modify Map" button.  
 <div class="admonition hint">
 <p class="admonition-title">It's easier done than said</p>
 <p>
 If you try it out and follow one or more tutorials, this will make more sense than any explanation. More detailed 
 specification of the modification options are e.g. described in the tutorial on map modification.
 </p>
 </div>
```

### Comparing `OccuPy-0.1.9/docs/Tutorials/intro.md` & `OccuPy-0.1.9rc1/docs/Tutorials/intro.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
 - a region of 12 pixels (voxels) in each dimension will be used to determine the scale-normalizing value. This value 
   is always 12 by default, and not estimated. 
 
 **Do not change these settings for this tutorial.**
 
 ---
 
-## 4. Estimate local scale 
-1. Make sure "occupancy" (just below the modification options) is **not** selected. 
+## 4. Estimate resolution-mode local scale 
+1. Make sure "resolution" is checked under the "Modification options". 
 
 2. Run OccuPy by clicking the Big button labeled "Estimate scale" just above the output log. 
 
 3. This should finish in a few seconds. Notice that the run is individually numbered as "1-1" in the output log. 
 
 <video class="center" width="400"  controls>
   <source src="https://drive.google.com/uc?export=view&id=1pRwqFaDtIcn2tSYHJ15UkQDiAEEjtzzg" type="video/mp4">
@@ -130,16 +130,16 @@
 viewer should update interactively, showing you how scale will be modified in the output compared to the input. 
 
 2. Click on the "Preview" tab of the viewer. There should be a notice to the effect that this is a bad idea. This is 
    because the scale we have estimated includes contrast degradation due to poor resolution and flexibility. OccuPy 
    does not allow you to use this for modifying maps, because it can't "compensate" for flexibility.  The big button 
    "modify map" should also be inactivated. 
 
-3. When you enabled any modification, the occupancy-mode just below the modification options was enabled and 
-   can't be disabled as long as you want to modify. Again, this is because OccuPy can't modify poor resolution, so 
+3. When you enabled any modification, the scale-mode just below the modification options was changed to "occupancy" and 
+   can't be changed as long as you want to modify. This is again because OccuPy can't modify poor resolution, so 
    it forces occupancy-mode. Click "Estimate scale" again to estimate the occupancy-mode local scale. This should 
    take a few seconds and then the new scale should be selected in the "scale map" drop-down menu, now containing 
    "occ" in its name. 
 
 
 <video class="center" width="400"  controls>
   <source src="https://drive.google.com/uc?export=view&id=1jY_CfRcixJB3jTNyVp4cAfKYA8sScY5W" type="video/mp4">
```

#### html2text {}

```diff
@@ -39,19 +39,19 @@
 pixels (voxels) in each dimension will hold a binary mask with the above radial
 cutoff. - of all the pixels selected by the binary mask, the scale will be
 proportional to the bottom 96.47% percentile, or the top 3.53% percentile - the
 above parameters results in 93 pixels (voxels) being sampled around each map
 pixel (voxel). - a region of 12 pixels (voxels) in each dimension will be used
 to determine the scale-normalizing value. This value is always 12 by default,
 and not estimated. **Do not change these settings for this tutorial.** --- ##
-4. Estimate local scale 1. Make sure "occupancy" (just below the modification
-options) is **not** selected. 2. Run OccuPy by clicking the Big button labeled
-"Estimate scale" just above the output log. 3. This should finish in a few
-seconds. Notice that the run is individually numbered as "1-1" in the output
-log.
+4. Estimate resolution-mode local scale 1. Make sure "resolution" is checked
+under the "Modification options". 2. Run OccuPy by clicking the Big button
+labeled "Estimate scale" just above the output log. 3. This should finish in a
+few seconds. Notice that the run is individually numbered as "1-1" in the
+output log.
 There's more to this
 To learn how parameter adjustment can help you get a better estimate, consult
 the tutorial_on_relative_resolution_estimation later.
 --- ## 5. Assess the scale 1. You will find that the estimated scale has been
 added to the "scale map" drop-down and is thus also rendered in the viewer tab
 "Scale". Click this viewer tab and drag the slider to check the estimated
 scale. 2. To further inspect the local scale, click the big button labeled
@@ -75,21 +75,21 @@
 drag the slider. The "plot" tab in the viewer should update interactively,
 showing you how scale will be modified in the output compared to the input. 2.
 Click on the "Preview" tab of the viewer. There should be a notice to the
 effect that this is a bad idea. This is because the scale we have estimated
 includes contrast degradation due to poor resolution and flexibility. OccuPy
 does not allow you to use this for modifying maps, because it can't
 "compensate" for flexibility. The big button "modify map" should also be
-inactivated. 3. When you enabled any modification, the occupancy-mode just
-below the modification options was enabled and can't be disabled as long as you
-want to modify. Again, this is because OccuPy can't modify poor resolution, so
-it forces occupancy-mode. Click "Estimate scale" again to estimate the
-occupancy-mode local scale. This should take a few seconds and then the new
-scale should be selected in the "scale map" drop-down menu, now containing
-"occ" in its name.
+inactivated. 3. When you enabled any modification, the scale-mode just below
+the modification options was changed to "occupancy" and can't be changed as
+long as you want to modify. This is again because OccuPy can't modify poor
+resolution, so it forces occupancy-mode. Click "Estimate scale" again to
+estimate the occupancy-mode local scale. This should take a few seconds and
+then the new scale should be selected in the "scale map" drop-down menu, now
+containing "occ" in its name.
 There's more to this
 To learn how parameter adjustment can help you get a better estimate, consult
 the tutorial_on_occupancy_estimation later.
 --- ## 8. Modify by local scale 1. Click the "Preview" tab of the viewer. Note
 that this preview is rough. 2. Try to remove the membrane by enabling
 attenuation and inspecting the preview as you alter the attenuation power by
 dragging the slider. 3. Try the same by sigmoid modification. Note that sigmoid
```

### Comparing `OccuPy-0.1.9/docs/about.md` & `OccuPy-0.1.9rc1/docs/about.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/full/14085_1.png` & `OccuPy-0.1.9rc1/docs/gallery/full/14085_1.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/full/14085_2.png` & `OccuPy-0.1.9rc1/docs/gallery/full/14085_2.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/full/14085_3.png` & `OccuPy-0.1.9rc1/docs/gallery/full/14085_3.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/full/14085_4.png` & `OccuPy-0.1.9rc1/docs/gallery/full/14085_4.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/full/14085_5.png` & `OccuPy-0.1.9rc1/docs/gallery/full/14085_5.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/full/14085_6.png` & `OccuPy-0.1.9rc1/docs/gallery/full/14085_6.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/highres.md` & `OccuPy-0.1.9rc1/docs/gallery/highres.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```
 
 # As in thumbnail
 
 ## In OccuPy
 
 1. Fetch EMDB 33707
-2. Set scale occupancy = checked
+2. Set scale mode = occupancy
 3. Estimate scale 
 4. Launch ChimeraX (open chimX_emd_33707.cxc through ChimeraX)
 
 ## In chimeraX 
 
 ```commandline
 vol gaussian #1 sdev 0.8
```

### Comparing `OccuPy-0.1.9/docs/gallery/index.md` & `OccuPy-0.1.9rc1/docs/gallery/index.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/mass.md` & `OccuPy-0.1.9rc1/docs/gallery/mass.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,12 +44,12 @@
 ## Other Views
 ### Waters 
 ![image](https://drive.google.com/uc?export=view&id=1QpIHuV5keCZLflykUYZLBohWao1WRU-F)
 ## In OccuPy
 
 1. Set extra option "Naive normalization" = **unchecked**
 2. Set input lowpass = 3Å
-3. Set occupancy = checked
+3. Set scale_mode = occupancy
 4. Estimate scale 
 5. Set sigmoid power = 30 , pivot = 0.05 
 6. Modify map
 7. Launch ChimeraX (open chimX_emd_11638.cxc through ChimeraX)
```

### Comparing `OccuPy-0.1.9/docs/gallery/membrane.md` & `OccuPy-0.1.9rc1/docs/gallery/membrane.md`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## In OccuPy
 
 1. Fetch EMDB 23015.
 2. Set the input lowpass to 5Å. This is too low to provide a reasonable occupancy estimate, but it's the value used 
    in the paper to show modification when occupancy is under-estimated. A better value for fidelity is probably 
    around 10Å. 
-3. Set scale occupancy = checked
+3. Set scale mode = occupancy
 4. Click "Estimate scale" 
 5. Enable Amplification and set Power=3
 6. Enable Attenuation and set Power=3
 7. Enable Sigmoid and set Power=30 and Pivot=0.50
 8. Click "Modify Map"
 9. Launch ChimeraX (open chimX_emd_23015.cxc through ChimeraX)
```

### Comparing `OccuPy-0.1.9/docs/gallery/modification.md` & `OccuPy-0.1.9rc1/docs/gallery/modification.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 OccuPy 1.8.0rc2
 ChimeraX 1.4 (2022-06-03)
 ```
 
 ## In OccuPy
 
 1. Fetch EMDB 14085. This may take a minute, as the map is 384px.
-2. Set scale occupancy = checked
+2. Set scale mode = occupancy
 3. Click "Estimate scale" 
 4. Enable amplification and set Power=30
 5. Enable Attenuation and set Power=2
 6. Enable Sigmoid and set Power=5 and Pivot=0.22
 7. Click "Modify Map"
 8. Launch ChimeraX (open chimX_emd_14085.cxc through ChimeraX)
```

### Comparing `OccuPy-0.1.9/docs/gallery/stylesheets/extra.css` & `OccuPy-0.1.9rc1/docs/gallery/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/synthetic.md` & `OccuPy-0.1.9rc1/docs/gallery/synthetic.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/actin.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/actin.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/high-res.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/high-res.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/linux_thumb.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/linux_thumb.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/mac_thumb.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/mac_thumb.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/mass.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/mass.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/membrane.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/membrane.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/modification.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/modification.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/resolution.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/resolution.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/ribo.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/ribo.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/spike.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/spike.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/synthetic.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/synthetic.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/gallery/thumbs/win_thumb.png` & `OccuPy-0.1.9rc1/docs/gallery/thumbs/win_thumb.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/index.md` & `OccuPy-0.1.9rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/install.md` & `OccuPy-0.1.9rc1/docs/install.md`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/docs/stylesheets/extra.css` & `OccuPy-0.1.9rc1/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/mkdocs.yml` & `OccuPy-0.1.9rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/occupy_lib/args.py` & `OccuPy-0.1.9rc1/occupy_lib/args.py`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/occupy_lib/estimate.py` & `OccuPy-0.1.9rc1/occupy_lib/estimate.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         n_lev=levels
     )
 
     # --------------- SCALE ESTIMATION ------------------------------------------------------
 
     scale_map = f'scale_{options.scale_mode}_{new_name}'
     if options.s0:
-        scale_map = f'scale_naive_{options.scale_mode}_{new_name}'
+        scale_map = f'scale_S0_{options.scale_mode}_{new_name}'
     scale, max_val, tiles_raw = occupancy.get_map_scale(
         scale_data,
         scale_kernel=scale_kernel,
         tau=options.tau,
         save_occ_map=scale_map,
         s0=options.s0,
         tile_size=options.tile_size,
@@ -353,19 +353,19 @@
     # A high value of lowest confident scale means a wide solvent model compared to the overall histogram
     lowest_confident_scale = sol_limits[3] / max_val
     if options.verbose:
         print(f'Min c.sc :\t[0,1]\t {lowest_confident_scale:.3f}', file=f_log)
 
     # Dirty check on the solvent model, could be more rigorous
     if lowest_confident_scale > 0.5:
-        warnings = "Solvent model fit is likely bad. Check output log for warnings and"
+        warnings = "Solvent model fit is likely bad. Check terminal output and"
         if not options.plot:
             warnings = f'{warnings} run with --plot and check solModel*.png'
         else:
-            warnings = f'{warnings} check the solvent model'
+            warnings = f'{warnings} check the output solModel*.png '
         solvent.warn_bad(lowest_confident_scale, file=f_log, verbose=options.verbose, kernel_warn=kernel_warn)
 
 
 
     fake_solvent = None  # Will not  add fake solvent during amplify
 
     ampl_name = None
```

### Comparing `OccuPy-0.1.9/occupy_lib/extras.py` & `OccuPy-0.1.9rc1/occupy_lib/extras.py`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/occupy_lib/map_tools.py` & `OccuPy-0.1.9rc1/occupy_lib/map_tools.py`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/occupy_lib/occupancy.py` & `OccuPy-0.1.9rc1/occupy_lib/occupancy.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,16 +429,14 @@
         s0=s0,
         tile_sz=tile_size,
         verbose=verbose)
 
     # Perform max-filter normalisation
     scale_map = np.clip(scale_map / map_val_at_full_scale, 0, 1)
 
-    if s0:
-        scale_mode = f'naive_{scale_mode}'
     # Save the scale
     if save_occ_map is not None:
         map_tools.new_mrc(
             scale_map,
             save_occ_map,
             vox_sz=1.0,
             verbose=verbose,
```

### Comparing `OccuPy-0.1.9/occupy_lib/occupy.py` & `OccuPy-0.1.9rc1/occupy_lib/occupy.py`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/occupy_lib/occupy_gui.py` & `OccuPy-0.1.9rc1/occupy_lib/occupy_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -802,23 +802,22 @@
         self.horizontalLayoutWidget_4.setObjectName("horizontalLayoutWidget_4")
         self.horizontalLayout_scaleMode = QtWidgets.QHBoxLayout(self.horizontalLayoutWidget_4)
         self.horizontalLayout_scaleMode.setContentsMargins(0, 0, 0, 0)
         self.horizontalLayout_scaleMode.setObjectName("horizontalLayout_scaleMode")
         self.checkBox_scaleOcc = QtWidgets.QCheckBox(self.horizontalLayoutWidget_4)
         self.checkBox_scaleOcc.setObjectName("checkBox_scaleOcc")
         self.horizontalLayout_scaleMode.addWidget(self.checkBox_scaleOcc)
-        # self.label_slash = QtWidgets.QLabel(self.horizontalLayoutWidget_4)
-        # self.label_slash.setEnabled(True)
-        # self.label_slash.setTextInteractionFlags(QtCore.Qt.NoTextInteraction)
-        # self.label_slash.setObjectName("label_slash")
-        # self.horizontalLayout_scaleMode.addWidget(self.label_slash)
+        self.label_slash = QtWidgets.QLabel(self.horizontalLayoutWidget_4)
+        self.label_slash.setEnabled(True)
+        self.label_slash.setTextInteractionFlags(QtCore.Qt.NoTextInteraction)
+        self.label_slash.setObjectName("label_slash")
+        self.horizontalLayout_scaleMode.addWidget(self.label_slash)
         self.checkBox_scaleRes = QtWidgets.QCheckBox(self.horizontalLayoutWidget_4)
         self.checkBox_scaleRes.setChecked(True)
         self.checkBox_scaleRes.setObjectName("checkBox_scaleRes")
-        self.checkBox_scaleRes.hide()
         self.horizontalLayout_scaleMode.addWidget(self.checkBox_scaleRes)
         self.gridLayoutWidget_7 = QtWidgets.QWidget(MainWindow)
         self.gridLayoutWidget_7.setGeometry(QtCore.QRect(110, 520, 561, 80))
         self.gridLayoutWidget_7.setObjectName("gridLayoutWidget_7")
         self.gridLayout_extraInputMaps = QtWidgets.QGridLayout(self.gridLayoutWidget_7)
         self.gridLayout_extraInputMaps.setContentsMargins(0, 0, 0, 0)
         self.gridLayout_extraInputMaps.setObjectName("gridLayout_extraInputMaps")
@@ -1129,15 +1128,15 @@
 
         self.checkBox_histMatch.setText(_translate("MainWindow", "Histogram-match to input"))
         self.checkBox_S0.setText(_translate("MainWindow", "Naive normalization"))
         self.checkBox_suppresSolvent.setText(_translate("MainWindow", "Supress solvent"))
         self.checkBox_maxBox.setText(_translate("MainWindow", "Limit box size"))
         self.checkBox_outputLowpass.setText(_translate("MainWindow", "Output lowpass"))
         self.checkBox_scaleOcc.setText(_translate("MainWindow", "occupancy"))
-        # self.label_slash.setText(_translate("MainWindow", "      or"))
+        self.label_slash.setText(_translate("MainWindow", "      or"))
         self.checkBox_scaleRes.setText(_translate("MainWindow", "resolution"))
 
         self.checkBox_histMatch.setToolTip(_translate("MainWindow", "When selected, the greyscale is matched\n"
                                                                     "against the input. This will may distort \n"
                                                                     "the continuity of the histogram. \n\n"
                                                                     "Expert/trial feature."))
         self.checkBox_S0.setToolTip(_translate("MainWindow", "When selected, the scale is normalized\n"
@@ -2266,20 +2265,14 @@
         if self.groupBox_amplification.isChecked():
             modifying = True
         if self.groupBox_attenuation.isChecked():
             modifying = True
         if self.groupBox_sigmoid.isChecked():
             modifying = True
 
-        if not modifying:
-            # Don't un-toggle if set
-            self.checkBox_scaleOcc.setEnabled(True)
-            if self.checkBox_scaleOcc:
-                return
-
         if modifying:
             self.checkBox_scaleOcc.setChecked(True)
             self.checkBox_scaleRes.setChecked(False)
             self.checkBox_scaleOcc.setEnabled(False)
             self.checkBox_scaleRes.setEnabled(False)
         else:
             self.checkBox_scaleOcc.setChecked(False)
@@ -2643,15 +2636,15 @@
         new_name = f'{Path(new_name).stem}.mrc'
         self.confidence_file_name = f'conf_{Path(new_name).stem}.mrc'
 
         scale_mode = 'res'
         if self.checkBox_scaleOcc.isChecked():
             scale_mode = 'occ'
         if options.s0:
-            scale_mode = f'naive_{scale_mode}'
+            scale_mode = f'S0_{scale_mode}'
 
         self.add_scale_file(f'scale_{scale_mode}_{Path(new_name).stem}.mrc')
 
         self.chimerax_file_name = f'chimX_{Path(new_name).stem}.cxc'
         if self.chimerax_name is not None:
             self.toolButton_chimerax.setEnabled(True)
             self.toolButton_chimerax.setToolTip(f'Run the chimerax command script \n to visualize the most recent  \n output from occupy. \n\n ({self.chimerax_file_name})')
```

### Comparing `OccuPy-0.1.9/occupy_lib/percentile_maxima.py` & `OccuPy-0.1.9rc1/occupy_lib/percentile_maxima.py`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/occupy_lib/solvent.py` & `OccuPy-0.1.9rc1/occupy_lib/solvent.py`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/occupy_lib/vis.py` & `OccuPy-0.1.9rc1/occupy_lib/vis.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             key_labels = f'{key_labels} :{key_vals[i]:.2f}'
         turbo_l = f'\'{turbo_l[:-1]}\''
         #turbo_l = '\'0.0,#d23105:0.1667,#fb8022:0.3333,#edd03a:0.5,#a3fd3d:0.6667,#31f199:0.8333,#29bbec:1.0,#29bbec\''
 
         clr = turbo_l
 
         key_str = f'key {clr} '
-        key_str = f'{key_str} {key_labels} size 0.5, 0.04 pos 0.25, 0.08 ticks true tickThickness 2 fontSize 20\n'
+        key_str = f'{key_str} {key_labels} size 0.5, 0.04 pos 0.25, 0.08 ticks true tickThickness 2 \n'
 
         print(f'alias scale_color color sample $1 map $2 palette {clr} range {min_scale},1.0 \n', file=the_file)
 
         print(f'alias set_scale_color_range color sample $1 map $2 palette {clr} range {min_scale},1.0 \n', file=the_file)
 
         print(f'volume #1 color #d3d7cf \n', file=the_file)
```

### Comparing `OccuPy-0.1.9/requirements.txt` & `OccuPy-0.1.9rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/resources/chimX.png` & `OccuPy-0.1.9rc1/resources/chimX.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/resources/help.txt` & `OccuPy-0.1.9rc1/resources/help.txt`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/resources/occupy_icon.png` & `OccuPy-0.1.9rc1/resources/occupy_icon.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/resources/occupy_icon_small.png` & `OccuPy-0.1.9rc1/resources/occupy_icon_small.png`

 * *Files identical despite different names*

### Comparing `OccuPy-0.1.9/setup.cfg` & `OccuPy-0.1.9rc1/setup.cfg`

 * *Files identical despite different names*

