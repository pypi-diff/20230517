# Comparing `tmp/LiquidDiffract-1.1.8.tar.gz` & `tmp/LiquidDiffract-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiquidDiffract-1.1.8.tar", last modified: Tue Dec 21 16:23:20 2021, max compression
+gzip compressed data, was "LiquidDiffract-1.1.9.tar", last modified: Thu Jul 14 12:10:28 2022, max compression
```

## Comparing `LiquidDiffract-1.1.8.tar` & `LiquidDiffract-1.1.9.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.698390 LiquidDiffract-1.1.8/
--rw-r--r--   0 benedict  (1000) users      (100)    32473 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LICENSE
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.674390 LiquidDiffract-1.1.8/LiquidDiffract/
--rwxr-xr-x   0 benedict  (1000) users      (100)      788 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/LiquidDiffract.py
--rw-r--r--   0 benedict  (1000) users      (100)     1068 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/__init__.py
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.678390 LiquidDiffract-1.1.8/LiquidDiffract/core/
--rw-r--r--   0 benedict  (1000) users      (100)        0 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/core/__init__.py
--rw-r--r--   0 benedict  (1000) users      (100)    43927 2021-12-21 15:53:23.000000 LiquidDiffract-1.1.8/LiquidDiffract/core/core.py
--rw-r--r--   0 benedict  (1000) users      (100)     8857 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/core/data_utils.py
--rwxr-xr-x   0 benedict  (1000) users      (100)     4333 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/core/peak_fit.py
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.678390 LiquidDiffract-1.1.8/LiquidDiffract/gui/
--rw-r--r--   0 benedict  (1000) users      (100)       24 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/gui/__init__.py
--rw-r--r--   0 benedict  (1000) users      (100)    21584 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/gui/bkg_ui.py
--rw-r--r--   0 benedict  (1000) users      (100)    12098 2021-12-21 15:53:23.000000 LiquidDiffract-1.1.8/LiquidDiffract/gui/main_widget.py
--rw-r--r--   0 benedict  (1000) users      (100)    42833 2021-12-21 15:53:11.000000 LiquidDiffract-1.1.8/LiquidDiffract/gui/optim_ui.py
--rw-r--r--   0 benedict  (1000) users      (100)    42884 2021-12-21 15:53:23.000000 LiquidDiffract-1.1.8/LiquidDiffract/gui/plot_widgets.py
--rw-r--r--   0 benedict  (1000) users      (100)     8603 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/gui/results_ui.py
--rwxr-xr-x   0 benedict  (1000) users      (100)    50709 2021-12-21 15:53:23.000000 LiquidDiffract-1.1.8/LiquidDiffract/gui/structure_ui.py
--rw-r--r--   0 benedict  (1000) users      (100)    33945 2021-12-21 15:53:23.000000 LiquidDiffract-1.1.8/LiquidDiffract/gui/utility.py
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.678390 LiquidDiffract-1.1.8/LiquidDiffract/resources/
--rw-r--r--   0 benedict  (1000) users      (100)        0 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/__init__.py
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.682390 LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/
--rw-r--r--   0 benedict  (1000) users      (100)    89172 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/4_and_25_iterations.png
--rw-r--r--   0 benedict  (1000) users      (100)   156661 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/LiquidDiffract v1.1.6-dev_refinement_tab.png
--rw-r--r--   0 benedict  (1000) users      (100)        0 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/__init__.py
--rw-r--r--   0 benedict  (1000) users      (100)   124484 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/chi_squared_minimum_map.png
--rw-r--r--   0 benedict  (1000) users      (100)   270384 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/fitting_region.png
--rw-r--r--   0 benedict  (1000) users      (100)   137664 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/optimal_n_iter.png
--rw-r--r--   0 benedict  (1000) users      (100)    18608 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/form_factors.npy
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.694390 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/A.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ag.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Al.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ar.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/As.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/At.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Au.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/B.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ba.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Be.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Bi.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Bk.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Br.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/C.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ca.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cd.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ce.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cf.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cl.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Co.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cr.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cs.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cu.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Dy.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Er.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Es.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Eu.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/F.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Fe.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Fr.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ga.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Gd.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ge.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/H.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/He.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Hf.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ho.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/I.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/In.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ir.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/K.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Kr.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/La.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Li.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Lu.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Mg.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Mn.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Mo.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/N.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Na.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Nb.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Nd.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ne.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ni.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/O.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Os.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/P.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pa.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pb.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pd.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Po.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pr.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pt.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pu.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ra.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Rb.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Re.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Rh.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Rn.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ru.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/S.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Sb.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Se.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Si.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Sn.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Sr.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/T.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ta.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Tb.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Te.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Th.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ti.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Tl.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/U.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/V.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/W.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Xe.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Y.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Yb.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Zn.npy
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Zr.npy
--rw-r--r--   0 benedict  (1000) users      (100)        0 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/__init__.py
--rw-r--r--   0 benedict  (1000) users      (100)      968 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/hg.npy
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.694390 LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/
--rw-r--r--   0 benedict  (1000) users      (100)        0 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/__init__.py
--rw-r--r--   0 benedict  (1000) users      (100)      955 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/browser.png
--rw-r--r--   0 benedict  (1000) users      (100)     1429 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/config.png
--rw-r--r--   0 benedict  (1000) users      (100)     6111 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/gs_icon.png
--rw-r--r--   0 benedict  (1000) users      (100)     3561 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/info.png
--rw-r--r--   0 benedict  (1000) users      (100)    15697 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/logo.png
--rw-r--r--   0 benedict  (1000) users      (100)     2071 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/mass_data.npy
--rw-r--r--   0 benedict  (1000) users      (100)     1560 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/resources/pt_data.npy
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.694390 LiquidDiffract-1.1.8/LiquidDiffract/scripts/
--rw-r--r--   0 benedict  (1000) users      (100)        0 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/scripts/__init__.py
--rw-r--r--   0 benedict  (1000) users      (100)     7091 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/scripts/brute.py
--rw-r--r--   0 benedict  (1000) users      (100)    14987 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/scripts/example_data.dat
--rw-r--r--   0 benedict  (1000) users      (100)     8489 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/LiquidDiffract/scripts/example_usage.py
--rw-r--r--   0 benedict  (1000) users      (100)       77 2021-12-21 15:53:23.000000 LiquidDiffract-1.1.8/LiquidDiffract/version.py
-drwxr-xr-x   0 benedict  (1000) users      (100)        0 2021-12-21 16:23:20.678390 LiquidDiffract-1.1.8/LiquidDiffract.egg-info/
--rw-r--r--   0 benedict  (1000) users      (100)    35401 2021-12-21 16:23:20.000000 LiquidDiffract-1.1.8/LiquidDiffract.egg-info/PKG-INFO
--rw-r--r--   0 benedict  (1000) users      (100)     6014 2021-12-21 16:23:20.000000 LiquidDiffract-1.1.8/LiquidDiffract.egg-info/SOURCES.txt
--rw-r--r--   0 benedict  (1000) users      (100)        1 2021-12-21 16:23:20.000000 LiquidDiffract-1.1.8/LiquidDiffract.egg-info/dependency_links.txt
--rw-r--r--   0 benedict  (1000) users      (100)       71 2021-12-21 16:23:20.000000 LiquidDiffract-1.1.8/LiquidDiffract.egg-info/entry_points.txt
--rw-r--r--   0 benedict  (1000) users      (100)       81 2021-12-21 16:23:20.000000 LiquidDiffract-1.1.8/LiquidDiffract.egg-info/requires.txt
--rw-r--r--   0 benedict  (1000) users      (100)       15 2021-12-21 16:23:20.000000 LiquidDiffract-1.1.8/LiquidDiffract.egg-info/top_level.txt
--rw-r--r--   0 benedict  (1000) users      (100)        1 2021-12-21 16:23:20.000000 LiquidDiffract-1.1.8/LiquidDiffract.egg-info/zip-safe
--rw-r--r--   0 benedict  (1000) users      (100)    35401 2021-12-21 16:23:20.694390 LiquidDiffract-1.1.8/PKG-INFO
--rw-r--r--   0 benedict  (1000) users      (100)    35046 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/README.md
--rw-r--r--   0 benedict  (1000) users      (100)      105 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/pyproject.toml
--rw-r--r--   0 benedict  (1000) users      (100)       38 2021-12-21 16:23:20.698390 LiquidDiffract-1.1.8/setup.cfg
--rw-r--r--   0 benedict  (1000) users      (100)     1361 2021-12-20 18:29:40.000000 LiquidDiffract-1.1.8/setup.py
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.920179 LiquidDiffract-1.1.9/
+-rw-r--r--   0 benedict  (1000) users      (100)    32473 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LICENSE
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.896179 LiquidDiffract-1.1.9/LiquidDiffract/
+-rwxr-xr-x   0 benedict  (1000) users      (100)      788 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/LiquidDiffract.py
+-rw-r--r--   0 benedict  (1000) users      (100)     1068 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/__init__.py
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.896179 LiquidDiffract-1.1.9/LiquidDiffract/core/
+-rw-r--r--   0 benedict  (1000) users      (100)        0 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/core/__init__.py
+-rw-r--r--   0 benedict  (1000) users      (100)    48955 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/core/core.py
+-rw-r--r--   0 benedict  (1000) users      (100)     8857 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/core/data_utils.py
+-rwxr-xr-x   0 benedict  (1000) users      (100)     4333 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/core/peak_fit.py
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.900179 LiquidDiffract-1.1.9/LiquidDiffract/gui/
+-rw-r--r--   0 benedict  (1000) users      (100)       24 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/gui/__init__.py
+-rw-r--r--   0 benedict  (1000) users      (100)    21145 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/gui/bkg_ui.py
+-rw-r--r--   0 benedict  (1000) users      (100)    13025 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/gui/main_widget.py
+-rw-r--r--   0 benedict  (1000) users      (100)    54675 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/gui/optim_ui.py
+-rw-r--r--   0 benedict  (1000) users      (100)    43134 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/gui/plot_widgets.py
+-rw-r--r--   0 benedict  (1000) users      (100)     8603 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/gui/results_ui.py
+-rwxr-xr-x   0 benedict  (1000) users      (100)    50709 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/gui/structure_ui.py
+-rw-r--r--   0 benedict  (1000) users      (100)    34644 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/gui/utility.py
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.900179 LiquidDiffract-1.1.9/LiquidDiffract/resources/
+-rw-r--r--   0 benedict  (1000) users      (100)        0 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/__init__.py
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.900179 LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/
+-rw-r--r--   0 benedict  (1000) users      (100)    89172 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/4_and_25_iterations.png
+-rw-r--r--   0 benedict  (1000) users      (100)   156661 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/LiquidDiffract v1.1.6-dev_refinement_tab.png
+-rw-r--r--   0 benedict  (1000) users      (100)        0 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/__init__.py
+-rw-r--r--   0 benedict  (1000) users      (100)   124484 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/chi_squared_minimum_map.png
+-rw-r--r--   0 benedict  (1000) users      (100)   270384 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/fitting_region.png
+-rw-r--r--   0 benedict  (1000) users      (100)   137664 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/optimal_n_iter.png
+-rw-r--r--   0 benedict  (1000) users      (100)    18608 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/form_factors.npy
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.920179 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/A.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ag.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Al.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ar.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/As.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/At.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Au.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/B.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ba.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Be.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Bi.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Bk.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Br.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/C.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ca.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cd.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ce.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cf.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cl.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Co.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cr.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cs.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cu.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Dy.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Er.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Es.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Eu.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/F.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Fe.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Fr.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ga.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Gd.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ge.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/H.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/He.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Hf.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ho.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/I.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/In.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ir.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/K.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Kr.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/La.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Li.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Lu.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Mg.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Mn.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Mo.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/N.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Na.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Nb.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Nd.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ne.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ni.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/O.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Os.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/P.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pa.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pb.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pd.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Po.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pr.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pt.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pu.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ra.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Rb.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Re.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Rh.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Rn.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ru.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/S.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Sb.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Se.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Si.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Sn.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Sr.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/T.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ta.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Tb.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Te.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Th.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ti.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Tl.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/U.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/V.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/W.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Xe.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Y.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Yb.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Zn.npy
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Zr.npy
+-rw-r--r--   0 benedict  (1000) users      (100)        0 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/__init__.py
+-rw-r--r--   0 benedict  (1000) users      (100)      968 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/hg.npy
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.920179 LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/
+-rw-r--r--   0 benedict  (1000) users      (100)        0 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/__init__.py
+-rw-r--r--   0 benedict  (1000) users      (100)      955 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/browser.png
+-rw-r--r--   0 benedict  (1000) users      (100)     1429 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/config.png
+-rw-r--r--   0 benedict  (1000) users      (100)     6111 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/gs_icon.png
+-rw-r--r--   0 benedict  (1000) users      (100)     3561 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/info.png
+-rw-r--r--   0 benedict  (1000) users      (100)    15697 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/logo.png
+-rw-r--r--   0 benedict  (1000) users      (100)     2071 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/mass_data.npy
+-rw-r--r--   0 benedict  (1000) users      (100)     1560 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/resources/pt_data.npy
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.920179 LiquidDiffract-1.1.9/LiquidDiffract/scripts/
+-rw-r--r--   0 benedict  (1000) users      (100)        0 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/scripts/__init__.py
+-rw-r--r--   0 benedict  (1000) users      (100)     7088 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/scripts/brute.py
+-rw-r--r--   0 benedict  (1000) users      (100)    14987 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/scripts/example_data.dat
+-rw-r--r--   0 benedict  (1000) users      (100)     8763 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/scripts/example_usage.py
+-rw-r--r--   0 benedict  (1000) users      (100)       77 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/LiquidDiffract/version.py
+drwxr-xr-x   0 benedict  (1000) users      (100)        0 2022-07-14 12:10:28.896179 LiquidDiffract-1.1.9/LiquidDiffract.egg-info/
+-rw-r--r--   0 benedict  (1000) users      (100)    36360 2022-07-14 12:10:28.000000 LiquidDiffract-1.1.9/LiquidDiffract.egg-info/PKG-INFO
+-rw-r--r--   0 benedict  (1000) users      (100)     6014 2022-07-14 12:10:28.000000 LiquidDiffract-1.1.9/LiquidDiffract.egg-info/SOURCES.txt
+-rw-r--r--   0 benedict  (1000) users      (100)        1 2022-07-14 12:10:28.000000 LiquidDiffract-1.1.9/LiquidDiffract.egg-info/dependency_links.txt
+-rw-r--r--   0 benedict  (1000) users      (100)       70 2022-07-14 12:10:28.000000 LiquidDiffract-1.1.9/LiquidDiffract.egg-info/entry_points.txt
+-rw-r--r--   0 benedict  (1000) users      (100)       81 2022-07-14 12:10:28.000000 LiquidDiffract-1.1.9/LiquidDiffract.egg-info/requires.txt
+-rw-r--r--   0 benedict  (1000) users      (100)       15 2022-07-14 12:10:28.000000 LiquidDiffract-1.1.9/LiquidDiffract.egg-info/top_level.txt
+-rw-r--r--   0 benedict  (1000) users      (100)        1 2022-07-14 12:10:28.000000 LiquidDiffract-1.1.9/LiquidDiffract.egg-info/zip-safe
+-rw-r--r--   0 benedict  (1000) users      (100)    36360 2022-07-14 12:10:28.920179 LiquidDiffract-1.1.9/PKG-INFO
+-rw-r--r--   0 benedict  (1000) users      (100)    36025 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/README.md
+-rw-r--r--   0 benedict  (1000) users      (100)      105 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/pyproject.toml
+-rw-r--r--   0 benedict  (1000) users      (100)       38 2022-07-14 12:10:28.920179 LiquidDiffract-1.1.9/setup.cfg
+-rw-r--r--   0 benedict  (1000) users      (100)     1361 2022-07-14 12:09:28.000000 LiquidDiffract-1.1.9/setup.py
```

### Comparing `LiquidDiffract-1.1.8/LICENSE` & `LiquidDiffract-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/LiquidDiffract.py` & `LiquidDiffract-1.1.9/LiquidDiffract/LiquidDiffract.py`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/__init__.py` & `LiquidDiffract-1.1.9/LiquidDiffract/__init__.py`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/core/core.py` & `LiquidDiffract-1.1.9/LiquidDiffract/core/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     from importlib import resources as importlib_resources
 except ImportError:
     import importlib_resources
 
 # Get version number from version.py
 from LiquidDiffract.version import __appname__, __version__
 from LiquidDiffract.core.data_utils import data_cache
+from LiquidDiffract.core.data_utils import smooth_data
 
 
 def calc_mol_mass(composition):
     '''
     Calculates the molecular mass for a given composition and returns
     the average molecular mass for one atom
 
@@ -883,14 +884,16 @@
         chi_squared - Value of chi^2
     '''
     # Square to remove negatives
     f = delta_D_r ** 2
     if method == 'simps':
         # Integrate using simpson's rule
         chi_squared = simps(f, x=r_intra)
+    else:
+        raise NotImplementedError()
     return chi_squared * 1e6
 
 
 def stop_iteration(stop_condition='count', count=None,
                    iter_limit=5, chi_squared=None):
     '''Helper function for checking stop condition of iteration
 
@@ -899,79 +902,55 @@
     easier to implement (i.e. checking for chi^2 convergence)
     '''
     if stop_condition == 'count':
         if count < iter_limit:
             return False
         else:
             return True
+    else:
+        raise NotImplementedError()
 
 
-def calc_impr_interference_func(rho, *args):
+def calc_impr_interference_func(q_data, interference_func,
+                                composition, rho,
+                                r_min, iter_limit,
+                                method, mod_func, window_start, fft_N):
     '''
     Calculates an improved estimate of the interference function via the
     iterative procedure described in Eggert et al., 2002. This is done by
     scaling the data and forcing its behaviour in the low r region to some
     modelled behaviour.
 
-    The form of this function also enables it to be passed to an optimisation
-    routine to estimate rho by minimising chi^2.
+    The function also returns a chi^2 figure of merit which can be passed
+    to a minimisation routine to estimate rho/b.
 
     Args:
-        rho - density
-
-        args - tuple of static parameters and arguments
-
-            If opt_flag == False, expected form is:
-            (q_data, interference_func, composition, r_min, iter_limit,
-             method, mod_func, window_start, opt_flag)
-
-            If opt_flag == True, expected form is:
-            (q_data, I_data, composition, r_min, iter_limit,
-             method, mod_func, window_start, opt_flag)
-
         q_data - Numpy array of Q space data
-        I_data - Background corrected/scaled intensity data for the sample
-        interference_func - Initial interference function (if using fixed rho)
+        interference_func - Initial interference function
         composition - Dict of elements, values as tuples of form (Z,charge,n)
+        rho - Density (average number density in atoms/angstrom^3)
         r_min - Intramolecular distance cut-off
         iter_limit - Iteration limit for S(Q) refinement. iter_limit >= 3 is
                      recommended for convergence. If optimising for minimum
                      chi^2 then 3 <= iter_limit <= 10 is recommended. Please
                      see the LiquidDiffract README for more information
         method - Formalisation of total scattering structure factor to use
                  ('ashcroft-langreth' or 'faber-ziman')
         mod_func - Modification function to scale data before fft
                    None, 'Cosine-window' or 'Lorch'
         window_start - Start of Cosine-window function needed if
                        mod_func == 'Cosine-window'
         fft_N - Sets size of array for fft where array_size = 2^N
-        opt_flag - Function returns chi_squared to minimisation routine if true
-                   Returns improved interference_func and chi squared if false
 
     Returns:
-        interference_func_impr, chi_sq (when opt_flag == 0)
-        chi_sq (when opt_flag == 1)
+        interference_func_impr - Interference function after iter_limit iterations
+        chi_sq - Figure of merit (see calc_chi_squared)
     '''
     # Unpack rho - solver passes rho as a single element array
     rho = np.float64(rho)
-    # Unpack static parameters & arguments
-    *_, opt_flag = args
-    if opt_flag == False:
-        (q_data, interference_func, composition, r_min, iter_limit,
-         method, mod_func, window_start, fft_N, opt_flag) = args
-    elif opt_flag == True:
-        (q_data, I_data, composition, r_min, iter_limit,
-         method, mod_func, window_start, fft_N, opt_flag) = args
-        # Calculate initial interference func for rho value
-        structure_factor = calc_structure_factor(q_data, I_data,
-                                                 composition, rho,
-                                                 method=method)
-        interference_func = structure_factor - calc_S_inf(composition, q_data, method=method)
-    else:
-        raise ValueError('Arg - opt_flag - must be boolean')
 
     dq = q_data[1] - q_data[0]
     # Calculate initial D(r)
     r, D_r = calc_correlation_func(q_data, interference_func, rho,
                       mod_func=mod_func, window_start=window_start,
                       dx=dq, N=fft_N)
     # Calculate expected behaviour of D(r) for intramolecular distances (r<r_min)
@@ -1013,25 +992,153 @@
         t3 = calc_D_r_iteration_term(delta_D_r, N=fft_N, dq=dq)[:len(interference_func)]
         t2 = (interference_func/t2_divisor) + 1
         with np.errstate(invalid='ignore'):
             interference_func_impr = interference_func - (t1 * t2 * t3)
 
         count += 1
 
-    # Check if opt_flag == 1 (True) or 0 (False)
-    # Checking against number value is preferred because of *args usage
-    # This meanse it would be easy to pass another value to the function by
-    # mistake. In this case bool() could return a false positive.
-    # i.e. bool(4) == True
-    if opt_flag == 1:
-        return chi_squared
-    elif opt_flag == 0:
-        return interference_func_impr, chi_squared
+    return interference_func_impr, chi_squared
+
+
+def refinement_objfun(minvar, *args):
+    '''
+    Wrapper objective function to pass to a solver to refine density (rho)
+    and/or background scaling factor (b) by minimising a chi^2 figure of merit.
+
+    This function provides set-up and logic for dealing with refinement of
+    different variables, including recalculating the background subtraction
+    when refining b. The actual calculations for the optimisation objective
+    function are in core.calc_impr_interference_func
+
+    Args:
+
+        minvar - independent variable(s) in the optimisation (numpy array with shape (n,))
+                 Can be one or both of:
+                    rho - average (bulk) number density (atoms/angstrom^3)
+                    bkg_scale - background scaling factor
+
+        *args - The expected arguments depend on if the background scaling factor
+                is being refined. The last two arguments should be opt_rho and
+                opt_bkg, i.e.:
+
+                    *_, opt_rho, opt_bkg = args
+
+                These should be boolean flags indicating if the density and
+                background scale factor are being refined respectively.
+
+                If opt_bkg == True (1), the expected args are:
+
+                    (*_, q_data, I_data_uncorrected, I_bkg,
+                     qmin, qmax,
+                     smooth_flag, smooth_window_length, smooth_poly_order,
+                     composition, r_min, iter_limit,
+                     method, mod_func, window_start, fft_N,
+                     opt_rho, opt_bkg) = args
+
+                If opt_rho == False (0), the density should precede q_data
+
+                If opt_bkg == False (0), the expected args are:
+
+                    (q_data, I_data_corrected,
+                     composition, r_min, iter_limit,
+                     method, mod_func, window_start, fft_N,
+                     opt_rho, opt_bkg) = args
+
+            The individual arguments are:
+
+                q_data - Numpy array of Q space data
+
+                I_data_uncorrected - Numpy array of intensity (I(Q)) values
+                                     prior to background subtraction
+                I_data_corrected - Numpy array of background subtracted I(Q) values
+                I_bkg - Numpy array of background intensities
+                qmin - Minimum Q value of useable data (float or None)
+                qmax - Maximum Q value to truncate data (float or None)
+                smooth_flag - Boolean flag to apply savitzky golay filter
+                smooth_window_length - Window length for optional smoothing filter
+                smooth_poly_order - Polynomial order for optional smoothing filter
+                composition - Dict of elements, values as tuples of form (Z,charge,n)
+                r_min - Intramolecular distance cut-off
+                iter_limit - Iteration limit for S(Q) refinement. iter_limit >= 3 is
+                             recommended for convergence. If optimising for minimum
+                             chi^2 then 3 <= iter_limit <= 10 is recommended. Please
+                             see the LiquidDiffract README for more information
+                method - Formalisation of total scattering structure factor to use
+                         ('ashcroft-langreth' or 'faber-ziman')
+                mod_func - Modification function to scale data before fft
+                           None, 'Cosine-window' or 'Lorch'
+                window_start - Start of Cosine-window function needed if
+                               mod_func == 'Cosine-window'
+                fft_N - Sets size of array for fft where array_size = 2^N
+
+    Returns:
+        chi_sq - Figure of merit (see calc_chi_squared)
+                 This is the value to be minimised by optimising
+                 the independent variable(s) minvar
+    '''
+    *_, opt_rho, opt_bkg = args
+    # Unpack optimisation variables (rho and/or bkg_scale)
+    if opt_rho == True and opt_bkg == True:
+        rho = np.float64(minvar[0])
+        bkg_scale = np.float64(minvar[1])
+    # Unpack rho - solver passes rho as a single element array
+    elif opt_rho == True and opt_bkg == False:
+        rho = np.float64(minvar)
+    # Unpack bkg_scale as abovs
+    elif opt_rho == False and opt_bkg == True:
+        bkg_scale = np.float64(minvar)
     else:
-        raise ValueError('Argument - opt_flag - must be boolean')
+        raise NotImplementedError()
+
+    if opt_rho == False:
+        rho, *_ = args
+        rho = np.float64(rho)
+
+    if opt_bkg == True:
+        # Unpack args - additional args needed when refining bkg_scale
+        (*_,
+         q_data, I_data_uncorrected, I_bkg,
+         qmin, qmax, smooth_flag, smooth_window_length, smooth_poly_order,
+         composition, r_min, iter_limit,
+         method, mod_func, window_start, fft_N, _, _) = args
+        I_data_corrected = I_data_uncorrected - (I_bkg * bkg_scale)
+        # Cut at qmax if qmax is != None
+        if qmax:
+            # Cut data at qmax
+            cut_max = np.where(q_data < qmax)
+            q_data = q_data[cut_max]
+            I_data_corrected = I_data_corrected[cut_max]
+        # Similarly cut at qmin if present
+        if qmin:
+            # Cut data to qmin - setting I(q<qmin)=I(qmin)
+            fill_val = I_data_corrected[np.argmax(q_data > qmin)]
+            cut_min = I_data_corrected[np.where(q_data > qmin)]
+            padding = np.asarray([fill_val] * (len(q_data) - len(cut_min)))
+            I_data_corrected = np.concatenate((padding, cut_min))
+        # smooth data if smooth_flag == 1
+        if smooth_flag == True:
+            I_data_corrected = smooth_data(I_data_corrected,
+                                      window_length=smooth_window_length,
+                                      poly_order=smooth_poly_order)
+    else:
+        # Unpack args here for opt_bkg == False
+        # (if opt_bkg is 0, opt_rho is always 1)
+        (q_data, I_data_corrected, composition, r_min, iter_limit,
+         method, mod_func, window_start, fft_N, _, _) = args
+
+    structure_factor = calc_structure_factor(q_data, I_data_corrected,
+                                             composition, rho,
+                                             method=method)
+    interference_func = structure_factor - calc_S_inf(composition, q_data, method=method)
+
+    _, chi_squared = calc_impr_interference_func(q_data, interference_func,
+                                                 composition, rho, r_min, iter_limit,
+                                                 method, mod_func, window_start, fft_N)
+
+    return chi_squared
 
 
 def integrate_coordination_sphere(r, rdf,
                                   r_0=None, rp_max=None,
                                   r_max=None, r_min=None, method=0):
     '''
     Calculates the 1st coordination number, N_1, for a monatomic sample by
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/core/data_utils.py` & `LiquidDiffract-1.1.9/LiquidDiffract/core/data_utils.py`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/core/peak_fit.py` & `LiquidDiffract-1.1.9/LiquidDiffract/core/peak_fit.py`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/gui/bkg_ui.py` & `LiquidDiffract-1.1.9/LiquidDiffract/gui/bkg_ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,25 +57,14 @@
         self.hsplitter = QSplitter(Qt.Horizontal)
         self.hsplitter.addWidget(self.config_scroll_area)
         self.hsplitter.addWidget(self.plot_scroll_area)
         self.hsplitter.setStretchFactor(0, 2)
         self.hsplitter.setStretchFactor(1, 5)
         self.layout.addWidget(self.hsplitter)
 
-        # Could add a separate scroll area > test on dif. screen sizes
-        # self.layout.addWidget(self.config_scroll_area)
-        # self.layout.addWidget(self.vline)
-        # self.layout.addWidget(QWidget())
-        # self.layout.addWidget(self.plot_scroll_area)
-
-        # Similarly could manually set stretch > test on dif. screens
-        # self.layout.setStretch(0,1)
-        # self.layout.setStretch(1,0)
-        # self.layout.setStretch(2,5)
-
         self.setLayout(self.layout)
 
         self.data_file = os.path.abspath(os.getcwd())
         self.file_name_changed.emit()
 
         __a = np.asarray([])
         self.data = {'data_raw_x': __a, 'data_raw_y':   __a,
@@ -201,15 +190,15 @@
             else:
                 self.data['cor_y'] = self.data['data_y']
         if self.bkg_config_widget.data_files_gb.plot_raw_check.isChecked():
             _plot_raw = 1
         else:
             _plot_raw = 0
         self.bkg_plot_widget.update_plots(self.data, _plot_raw)
-        # emit signal that data has changed to be picked up by tab2
+        # emit signal that data has changed to be picked up by second tab (optim_ui)
         self.plots_changed.emit()
 
     def sub_bkg(self):
         # Cor x = data x
         self.data['cor_x'] = self.data['data_x']
         self.plot_data()
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/gui/main_widget.py` & `LiquidDiffract-1.1.9/LiquidDiffract/gui/main_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,26 +180,33 @@
         self.create_signal_tab_links()
 
     def create_signal_tab_links(self):
         self.bkg_ui.plots_changed.connect(self.bkg_plots_changed_slot)
         self.optim_ui.results_changed.connect(self.results_changed_slot)
         self.optim_ui.results_cleared.connect(self.results_cleared_slot)
         self.bkg_ui.file_name_changed.connect(self.update_filename)
+        self.optim_ui.optim_config_widget.optim_results_gb.bkg_scale_copy_btn.clicked.connect(self.copy_bkg_scale_result)
 
     def bkg_plots_changed_slot(self):
         # Clear data from Optim UI (as S(Q) etc. need to be recalculated)
-        self.optim_ui.data = {'cor_x': np.asarray([]), 'cor_y': np.asarray([]),
+        self.optim_ui.data = {'uncorrected_y': np.asarray([]), 'bkg_y': np.asarray([]), 'bkg_scale': None,
+                              'cor_x': np.asarray([]), 'cor_y': np.asarray([]),
                               'cor_x_cut': np.asarray([]), 'cor_y_cut': np.asarray([]),
                               'sq_x': np.asarray([]), 'sq_y': np.asarray([]),
                               'dr_x': np.asarray([]), 'dr_y': np.asarray([]),
-                              'mod_func': 'None'
+                              'rescaled_cor_y_cut': np.asarray([]),
+                              'mod_func': 'None', 'qmin': None, 'qmax': None
                               }
         # Pass data to Optim UI
         self.optim_ui.data['cor_x'] = self.bkg_ui.data['cor_x']
         self.optim_ui.data['cor_y'] = self.bkg_ui.data['cor_y']
+        if self.bkg_ui.bkg_config_widget.bkg_subtract_gb.isChecked() and self.bkg_ui.data['bkg_y'].size:
+            self.optim_ui.data['uncorrected_y'] = self.bkg_ui.data['data_y']
+            self.optim_ui.data['bkg_y'] = self.bkg_ui.data['bkg_y']
+            self.optim_ui.data['bkg_scale'] = self.bkg_ui.bkg_config_widget.bkg_subtract_gb.scale_sb.value()
         self.optim_ui.plot_data()
 
     def results_changed_slot(self):
         # Clear old s(q), g(r), rdf(r)
         self.results_ui.clear_data()
         # Set rho
         if (self.optim_ui.optim_config_widget.optim_options_gb.opt_check.isChecked()) & (self.optim_ui.optim_config_widget.optim_options_gb.isChecked()):
@@ -247,7 +254,11 @@
     def update_filename(self):
         _base_name, _ext = os.path.splitext(self.bkg_ui.data_file)
         self.results_ui.base_filename = _base_name
         self.optim_ui.base_filename = _base_name
         self.structure_ui.base_filename = _base_name
         self.optim_ui.filename_ext = _ext
         self.structure_ui.filename_ext = _ext
+
+    def copy_bkg_scale_result(self):
+        _bkg_scale_result = self.optim_ui.optim_config_widget.optim_results_gb.bkg_scale_output.text()
+        self.bkg_ui.bkg_config_widget.bkg_subtract_gb.scale_sb.setValue(np.float64(_bkg_scale_result))
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/gui/optim_ui.py` & `LiquidDiffract-1.1.9/LiquidDiffract/gui/optim_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 
         self.data = {'cor_x': np.asarray([]), 'cor_y': np.asarray([]),
                      'cor_x_cut': np.asarray([]), 'cor_y_cut': np.asarray([]),
                      'sq_x': np.asarray([]), 'sq_y': np.asarray([]),
                      'dr_x': np.asarray([]), 'dr_y': np.asarray([]),
                      'int_func': np.asarray([]), 'impr_int_func': np.asarray([]),
                      'impr_dr_x': np.asarray([]), 'impr_dr_y': np.asarray([]),
-                     'impr_iq_x': np.asarray([]), 'mod_func': 'None'}
+                     'impr_iq_x': np.asarray([]), 'mod_func': 'None',
+                     'rescaled_cor_y_cut': np.asarray([]),
+                     'qmin': None, 'qmax': None}
 
         self.create_signals()
 
     def create_signals(self):
         self.optim_config_widget.data_options_gb.qmax_check.stateChanged.connect(self.plot_data)
         self.optim_config_widget.data_options_gb.qmax_input.textChanged.connect(self.plot_data)
         self.optim_config_widget.data_options_gb.qmin_check.stateChanged.connect(self.plot_data)
@@ -102,48 +104,51 @@
         self.data['dr_y'] = _ea
         self.data['int_func'] = _ea
         self.data['impr_int_func'] = _ea
         self.data['impr_dr_x'] = _ea
         self.data['impr_dr_y'] = _ea
         self.data['cor_x_cut'] = _ea
         self.data['cor_y_cut'] = _ea
+        self.data['rescaled_cor_y_cut'] = _ea
+        self.data['qmin'] = None
+        self.data['qmax'] = None
 
         qmax_cut = (
             self.optim_config_widget.data_options_gb.qmax_check.isChecked()
             and self.optim_config_widget.data_options_gb.qmax_input.text()
             and self.optim_config_widget.data_options_gb.qmax_input.hasAcceptableInput()
         )
         qmin_cut = (
             self.optim_config_widget.data_options_gb.qmin_check.isChecked()
             and self.optim_config_widget.data_options_gb.qmin_input.text()
             and self.optim_config_widget.data_options_gb.qmin_input.hasAcceptableInput()
         )
 
-        # Cut q at qman first (if selected) and define cor_x_cut
+        # Cut q at qmax first (if selected) and define cor_x_cut
         if qmax_cut:
             # Get q_max to cut at
-            _qmax = np.float(self.optim_config_widget.data_options_gb.qmax_input.text())
+            self.data['qmax'] = np.float(self.optim_config_widget.data_options_gb.qmax_input.text())
             # cut q data at qmax
-            _cut = np.where(self.data['cor_x'] < _qmax)
+            _cut = np.where(self.data['cor_x'] < self.data['qmax'])
             self.data['cor_x_cut'] = self.data['cor_x'][_cut]
             self.data['cor_y_cut'] = self.data['cor_y'][_cut]
 
         # Define cor_x_cut = cor_x for simpler plotting logic
         else:
             self.data['cor_x_cut'] = self.data['cor_x']
             self.data['cor_y_cut'] = self.data['cor_y']
 
         # Cut at qmin if selected
         if qmin_cut:
-            _qmin = np.float(self.optim_config_widget.data_options_gb.qmin_input.text())
+            self.data['qmin'] = np.float(self.optim_config_widget.data_options_gb.qmin_input.text())
             # Take first intensity value after q_min
             # Catch empty array error caused by no data:
             try:
-                _fill_val = self.data['cor_y'][np.argmax(self.data['cor_x_cut'] > _qmin)]
-                _cut = self.data['cor_y'][np.where(self.data['cor_x_cut'] > _qmin)]
+                _fill_val = self.data['cor_y'][np.argmax(self.data['cor_x_cut'] > self.data['qmin'])]
+                _cut = self.data['cor_y'][np.where(self.data['cor_x_cut'] > self.data['qmin'])]
                 _padding = np.asarray([_fill_val] * (len(self.data['cor_x_cut']) - len(_cut)))
                 self.data['cor_y_cut'] = np.concatenate((_padding, _cut))
             except ValueError:
                 pass
 
         # this method is only used for 'raw' S(Q) actual data so mod_func = 1
         self.data['modification'] = 1
@@ -208,25 +213,25 @@
     def on_click_refine(self):
         # Delete previous chi_sq & refined density
         try:
             del self.data['chi_sq']
             del self.data['refined_rho']
         except KeyError:
             pass
+        # Don't run if sq/int_func not calculated yet
+        if not self.data['int_func'].size:
+            return
         # Check validity of input fields before continuing
         if not (
             self.optim_config_widget.composition_gb.density_input.hasAcceptableInput()
             and self.optim_config_widget.optim_options_gb.rmin_input.hasAcceptableInput()
             and self.optim_config_widget.optim_options_gb.niter_input.hasAcceptableInput()
         ):
             print('Error: Please ensure values are set for density, r_min, and n_iterations')
             return
-        # Don't run if sq/int_func not calculated yet
-        if not self.data['int_func'].size:
-            return
         # Get modification function to use again
         self.data['mod_func'] = self.optim_config_widget.data_options_gb.mod_func_input.currentText()
         if self.data['mod_func'] == 'Cosine-window':
             try:
                 self.data['window_start'] = np.float(self.optim_config_widget.data_options_gb.window_start_input.text())
             except ValueError:
                 self.window_func_error()
@@ -244,130 +249,267 @@
         _rho_0 = np.float(self.optim_config_widget.composition_gb.density_input.text())
         # Get r_min
         _r_min = np.float(self.optim_config_widget.optim_options_gb.rmin_input.text())
         # Get no. iterations for Eggert refinement
         _n_iter = np.int(self.optim_config_widget.optim_options_gb.niter_input.text())
         if _n_iter < 2:
             print('Warning: n_iter >= 2 is recommended for convergence!')
-        if self.optim_config_widget.optim_options_gb.opt_check.isChecked():
+        if (
+            self.optim_config_widget.optim_options_gb.opt_check.isChecked() or
+            self.optim_config_widget.optim_options_gb.opt_check_bkg.isChecked()
+            ):
             # Get bounds but don't continue if none set
             try:
-                _lb = np.float(self.optim_config_widget.optim_options_gb.lb_input.text())
-                _ub = np.float(self.optim_config_widget.optim_options_gb.ub_input.text())
+                if self.optim_config_widget.optim_options_gb.opt_check_bkg.isChecked():
+                    # Check bkg scaling factor, uncorrected data, and bkg are present
+                    if not self.data['uncorrected_y'].size or not self.data['bkg_y'].size or not self.data['bkg_scale']:
+                        self.bkg_error()
+                        return
+                    # Get bounds on background scaling factor - return if none set
+                    _lb_bkg = np.float(self.optim_config_widget.optim_options_gb.lb_input_bkg.text())
+                    _ub_bkg = np.float(self.optim_config_widget.optim_options_gb.ub_input_bkg.text())
+                    _bkg_scale_0 = self.data['bkg_scale']
+                    opt_bkg = 1
+                else:
+                    opt_bkg = 0
+                if self.optim_config_widget.optim_options_gb.opt_check.isChecked():
+                    _lb_rho = np.float(self.optim_config_widget.optim_options_gb.lb_input.text())
+                    _ub_rho = np.float(self.optim_config_widget.optim_options_gb.ub_input.text())
+                    opt_rho = 1
+                else:
+                    opt_rho = 0
             except ValueError:
                 self.limits_error()
                 return
             if _n_iter > 10:
                  print('Warning: n_iter <= 10 is recommended for convergence!')
             # Only use mod_func in refinement if option is set (default is no)
             if self.mod_func_mode:
                 _mod_func = self.data['mod_func']
             else:
                 _mod_func = None
-            _args = (self.data['cor_x_cut'], self.data['cor_y_cut'],
-                     _composition, _r_min, _n_iter, _method,
-                     _mod_func, self.data['window_start'],
-                     self.fft_N, 1)
+            # Set arguments for objective function
+            # Additional arguments required if refining the background
+            if opt_bkg == True:
+                _smooth_flag = self.optim_config_widget.data_options_gb.smooth_data_check.isChecked()
+                _args = (self.data['cor_x'], self.data['uncorrected_y'], self.data['bkg_y'],
+                         self.data['qmin'], self.data['qmax'],
+                         _smooth_flag, self.window_length, self.poly_order,
+                         _composition, _r_min, _n_iter,
+                         _method, _mod_func, self.data['window_start'], self.fft_N, opt_rho, opt_bkg)
+                # Setup independent variable to pass to minimisation routine
+                if opt_rho == True:
+                    _minvar = np.array([_rho_0, _bkg_scale_0])
+                else:
+                    _minvar = _bkg_scale_0
+                    # rho must be passed as argument if *only* refining the background
+                    _args = (_rho_0, *_args)
+            else:
+                _args = (self.data['cor_x_cut'], self.data['cor_y_cut'], _composition, _r_min, _n_iter,
+                         _method, _mod_func, self.data['window_start'], self.fft_N, opt_rho, opt_bkg)
+                _minvar = _rho_0
+            # Set up kw arguments for solver
             _solver_kwargs = {'args': _args,
                               'options': dict(self.minimisation_options),
                               'method': self.op_method}
+            # Set up bounds for minimisation
             if self.op_method == 'COBYLA':
                 # Construct constraints for COBYLA method. The COBYLA solver
                 # does not use the 'bounds' kwarg, and requires lb & ub passed
                 # as a constraint function
-                _cons = [{'type': 'ineq', 'fun': lambda x: x - _lb},
-                         {'type': 'ineq', 'fun': lambda x: _ub - x}
-                         ]
+                if opt_rho == True:
+                    _cons = [{'type': 'ineq', 'fun': lambda x: x - _lb_rho},
+                             {'type': 'ineq', 'fun': lambda x: _ub_rho - x}
+                             ]
+                    if opt_bkg == True:
+                        _cons.extend([
+                                    {'type': 'ineq', 'fun': lambda x: x - _lb_bkg},
+                                    {'type': 'ineq', 'fun': lambda x: _ub_bkg - x}
+                                    ])
+                else:
+                    _cons = [{'type': 'ineq', 'fun': lambda x: x - _lb_bkg},
+                             {'type': 'ineq', 'fun': lambda x: _ub_bkg - x}
+                             ]
                 _solver_kwargs['constraints'] = _cons
                 # Handle different name of solver option ftol (tol)
                 _solver_kwargs['options']['tol'] = _solver_kwargs['options'].pop('ftol')
             else:
-                _solver_kwargs['bounds'] = ((_lb, _ub),)
+                if opt_rho == True:
+                    _solver_kwargs['bounds'] = ((_lb_rho, _ub_rho),)
+                    if opt_bkg == True:
+                        _solver_kwargs['bounds'] = (*_solver_kwargs['bounds'], (_lb_bkg, _ub_bkg))
+                else:
+                    _solver_kwargs['bounds'] = ((_lb_bkg, _ub_bkg),)
 
             print('\n*************************\n')
-            print('Finding optimal density...')
+            print('Finding optimal density/background...')
 
             if self.global_minimisation == 1:
                 # Grey out config panel while refining
                 self.enable_config_panel(False)
                 print('\nRunning basin-hopping algorithm to find global minimum')
                 _global_min_kwargs = dict(self.global_min_options)
                 _global_min_kwargs['minimizer_kwargs'] = _solver_kwargs
-                _opt_result = basinhopping(core.calc_impr_interference_func,
-                                           _rho_0,
+                _opt_result = basinhopping(core.refinement_objfun,
+                                           _minvar,
                                            **_global_min_kwargs)
                 # Re-enable config panel
                 self.enable_config_panel(True)
             else:
-                _opt_result = minimize(core.calc_impr_interference_func,
-                                       _rho_0,
+                _opt_result = minimize(core.refinement_objfun,
+                                       _minvar,
                                        **_solver_kwargs)
-            # Handle for anomalous solver behaviour
-            # e.g. (COBYLA opt_result.x is scalar)
-            try:
-                self.data['refined_rho'] = _opt_result.x[0]
-            except IndexError:
-                self.data['refined_rho'] = _opt_result.x
-            _rho_temp = self.data['refined_rho']
-            print('Refined density = ', _rho_temp)
+            # Extract optimised variables from _opt_result
+            if opt_rho == True:
+                if opt_bkg == True:
+                    self.data['refined_rho'] = _opt_result.x[0]
+                    _refined_bkg_scale = _opt_result.x[1]
+                    print('Refined background scaling = ', _refined_bkg_scale)
+                else:
+                    # Handle for anomalous solver behaviour
+                    # e.g. (COBYLA opt_result.x is scalar)
+                    try:
+                        self.data['refined_rho'] = _opt_result.x[0]
+                    except IndexError:
+                        self.data['refined_rho'] = _opt_result.x
+                # Set optimised rho result
+                _rho_temp = self.data['refined_rho']
+                print('Refined density = ', _rho_temp)
+                self.optim_config_widget.optim_results_gb.density_output.setText('{:.4e}'.format(self.data['refined_rho']))
+                _mass_density = core.conv_density(_rho_temp, _composition)
+                self.optim_config_widget.optim_results_gb.mass_density.setText('{0:.3f}'.format(_mass_density))
+            else:
+                # Set _rho_temp to _rho_0 if not refining rho
+                _rho_temp = _rho_0
+                # Handle for anomalous solver behaviour
+                # e.g. (COBYLA opt_result.x is scalar)
+                try:
+                    _refined_bkg_scale = _opt_result.x[0]
+                except IndexError:
+                    _refined_bkg_scale = _opt_result.x
+                print('Refined background scaling = ', _refined_bkg_scale)
+            # Set optimised bkg scaling output
+            if opt_bkg == True:
+                self.optim_config_widget.optim_results_gb.bkg_scale_output.setText('{:.4e}'.format(_refined_bkg_scale))
+
+            # Print Chi^2 to screen
             print('Chi^2 = ', _opt_result.fun, '\n')
-            self.optim_config_widget.optim_results_gb.density_output.setText('{:.4e}'.format(self.data['refined_rho']))
-            _mass_density = core.conv_density(_rho_temp, _composition)
-            self.optim_config_widget.optim_results_gb.mass_density.setText('{0:.3f}'.format(_mass_density))
+
+            # Recalculate interference function with new background scaling and/or rho
+            if opt_bkg == True:
+                _I_data_corrected = self.data['uncorrected_y'] - (self.data['bkg_y'] * _refined_bkg_scale)
+                # Cut data at qmax/qmin
+                if self.data['qmax']:
+                    _cut_max = np.where(self.data['cor_x'] < self.data['qmax'])
+                    _cut_q_data = self.data['cor_x'][_cut_max]
+                    _I_data_corrected = _I_data_corrected[_cut_max]
+                else:
+                    _cut_q_data = self.data['cor_x']
+                if self.data['qmin']:
+                    # Cut data to qmin - setting I(q<qmin)=I(qmin)
+                    _fill_val = _I_data_corrected[np.argmax(_cut_q_data > self.data['qmin'])]
+                    _cut_min = _I_data_corrected[np.where(_cut_q_data > self.data['qmin'])]
+                    _padding = np.asarray([_fill_val] * (len(_cut_q_data) - len(_cut_min)))
+                    _I_data_corrected = np.concatenate((_padding, _cut_min))
+                # smooth data if smooth_flag == 1
+                if _smooth_flag == True:
+                    _I_data_corrected = data_utils.smooth_data(_I_data_corrected,
+                                            window_length=self.window_length,
+                                            poly_order=self.poly_order)
+                _structure_factor = core.calc_structure_factor(_cut_q_data, _I_data_corrected,
+                                                               _composition, _rho_temp, method=_method)
+                _int_func_temp = _structure_factor - core.calc_S_inf(_composition, _cut_q_data, method=_method)
+                self.data['rescaled_cor_y_cut'] = _I_data_corrected
+            else:
+                _structure_factor = core.calc_structure_factor(self.data['cor_x_cut'], self.data['cor_y_cut'],
+                                                               _composition, _rho_temp, method=_method)
+                _int_func_temp = _structure_factor - core.calc_S_inf(_composition, self.data['cor_x_cut'], method=_method)
         else:
             _rho_temp = _rho_0
-
+            _int_func_temp = self.data['int_func']
         # Only use mod_func in refinement if option is set (default is no)
         if self.mod_func_mode:
             _mod_func = self.data['mod_func']
         else:
             _mod_func = None
-        _args = (self.data['cor_x_cut'], self.data['int_func'],
-                 _composition, _r_min, _n_iter, _method,
-                 _mod_func, self.data['window_start'],
-                 self.fft_N, 0)
-        self.data['impr_int_func'], self.data['chi_sq'] = core.calc_impr_interference_func(_rho_temp, *_args)
+        _args = (self.data['cor_x_cut'], _int_func_temp,
+                 _composition, _rho_temp, _r_min, _n_iter, _method,
+                 _mod_func, self.data['window_start'], self.fft_N)
+        self.data['impr_int_func'], self.data['chi_sq'] = core.calc_impr_interference_func(*_args)
         self.optim_config_widget.optim_results_gb.chi_sq_output.setText('{:.4e}'.format(self.data['chi_sq']))
         # Calculated improved F_r
         self.data['impr_dr_x'], self.data['impr_dr_y'] = core.calc_correlation_func(self.data['iq_x'], self.data['impr_int_func'], _rho_temp, N=self.fft_N,
                                                                        mod_func=self.data['mod_func'], window_start=self.data['window_start'])
         self.data['impr_iq_x'] = self.data['iq_x']
         # Set modification function to None so it is not plotted this time
         _mod_func = self.data['mod_func']
         self.data['mod_func'] = 'None'
         # Plot data
         self.optim_plot_widget.update_plots(self.data)
         self.data['mod_func'] = _mod_func
         self.data['sq_method'] = _method
+        # Reset rescaled I(Q) data to prevent plot persistence
+        self.data['rescaled_cor_y_cut'] = np.asarray([])
 
         # Save refinement parameters to file
         if self.optim_config_widget.data_options_gb.smooth_data_check.isChecked():
             _smooth_bool = 'Y'
         else:
             _smooth_bool = 'N'
         if self.mod_func_mode:
             _mod_func_mode_bool = 'Y'
         else:
             _mod_func_mode_bool = 'N'
         if self.optim_config_widget.optim_options_gb.opt_check.isChecked():
             _refine_density_bool = 'Y'
-            _refine_density_log = (
-                f'Solver : {self.op_method}\n'
-                f'Lower bound : {_lb}\n'
-                f'Upper bound : {_ub}\n'
-                f'{"*"*25}\n'
-                f'{_opt_result}\n'
-                f'{"*"*25}\n\n'
+            _refine_density_bounds = (
+                f'Lower bound (rho) : {_lb_rho}\n'
+                f'Upper bound (rho) : {_ub_rho}\n'
+            )
+            _refine_density_res = (
                 f'Refined density : {self.data["refined_rho"]} (at/A^3)\n'
                 f'{" "*18}{_mass_density} (g/cm3)\n'
-                f'Chi^2 : {self.data["chi_sq"]}\n'
             )
         else:
             _refine_density_bool = 'N'
-            _refine_density_log = (f'Chi^2 : {self.data["chi_sq"]}\n')
+            _refine_density_bounds = ''
+            _refine_density_res = ''
+        if self.optim_config_widget.optim_options_gb.opt_check_bkg.isChecked():
+            _refine_bkg_bool = 'Y'
+            _refine_bkg_bounds = (
+                f'Lower bound (b) : {_lb_bkg}\n'
+                f'Upper bound (b) : {_ub_bkg}\n'
+            )
+            _refine_bkg_res = (
+                f'Refined background scaling : {_refined_bkg_scale}\n'
+            )
+        else:
+            _refine_bkg_bool = 'N'
+            _refine_bkg_bounds = ''
+            _refine_bkg_res = ''
+
+        if (
+            self.optim_config_widget.optim_options_gb.opt_check.isChecked() or
+            self.optim_config_widget.optim_options_gb.opt_check_bkg.isChecked()
+            ):
+            _refine_log = (
+                f'Solver : {self.op_method}\n' +
+                _refine_density_bounds +
+                _refine_bkg_bounds +
+                f'{"*"*25}\n'
+                f'{_opt_result}\n'
+                f'{"*"*25}\n\n' +
+                _refine_bkg_res +
+                _refine_density_res +
+                f'Chi^2 : {self.data["chi_sq"]}\n'
+            )
+        else:
+            _refine_log = (
+                f'Chi^2 : {self.data["chi_sq"]}\n'
+            )
 
         log_string = (
             f'refinement_log\n'
             f'{__appname__} v{__version__}\n\n'
             f'{"-"*25}\n'
             f'Data File : {self.base_filename}{self.filename_ext}\n'
             f'Composition [Element: (Z, Charge, n)]: {_composition}\n'
@@ -378,16 +520,17 @@
             f'Modification func used in iterative refinement? : {_mod_func_mode_bool}\n'
             f'Cosine window start : {self.data["window_start"]}\n'
             f'S(Q) formulation : {_method}\n'
             f'Density : {_rho_0}\n'
             f'r_min : {_r_min}\n'
             f'Number iterations (Eggert) : {_n_iter}\n'
             f'{"*"*25}\n'
-            f'Density refined? : {_refine_density_bool}\n' +
-            _refine_density_log
+            f'Density refined? : {_refine_density_bool}\n'
+            f'Background refined? : {_refine_bkg_bool}\n' +
+            _refine_log
         )
 
         # Append to log file or overwrite?
         if self.append_log_mode:
             _log_file = open(os.path.join(os.path.dirname(self.base_filename), 'refinement.log'), 'ab')
             # Add timestamp to top of log_string
             log_string = (f'{"#"*30}\n'
@@ -423,14 +566,21 @@
 
     def limits_error(self):
         print('Warning: Must set bounds to refine density!')
         _message = ['Refinement error!', 'Must set bounds to refine density!']
         _error_msg = utility.ErrorMessageBox(_message)
         _error_msg.exec_()
 
+    def bkg_error(self):
+        print('Warning: Must load background file to refine background scaling factor')
+        _message = ['Missing background!', 'Must load background to refine background scale factor']
+        _error_msg = utility.ErrorMessageBox(_message)
+        _error_msg.exec_()
+
+
 class OptimConfigWidget(QWidget):
 
     def __init__(self):
         super(OptimConfigWidget, self).__init__()
 
         self.vlayout = QVBoxLayout()
         self.vlayout.setContentsMargins(0, 0, 5, 0)
@@ -449,26 +599,42 @@
         self.setLayout(self.vlayout)
 
         self.create_signals()
 
     def create_signals(self):
         self.optim_options_gb.toggled.connect(self._toggle_results_gb)
         self.optim_options_gb.opt_check.stateChanged.connect(self._toggle_density_refine)
+        self.optim_options_gb.opt_check_bkg.stateChanged.connect(self._toggle_bkg_scale_refine)
+        self.optim_results_gb.bkg_scale_copy_btn.clicked.connect(self._copy_bkg_scale_output)
         self.optim_results_gb.density_copy_btn.clicked.connect(self._copy_density_output)
 
     def _toggle_results_gb(self, on):
         self.optim_results_gb.setEnabled(on)
 
     def _toggle_density_refine(self, state):
         self.optim_results_gb.density_output.setEnabled(state)
         self.optim_results_gb.density_output_label.setEnabled(state)
         self.optim_results_gb.mass_density.setEnabled(state)
         self.optim_results_gb.mass_density_label.setEnabled(state)
         self.optim_results_gb.density_copy_btn.setEnabled(state)
+
+    def _toggle_bkg_scale_refine(self, state):
+        self.optim_results_gb.bkg_scale_output.setEnabled(state)
+        self.optim_results_gb.bkg_scale_output_label.setEnabled(state)
+        self.optim_results_gb.bkg_scale_copy_btn.setEnabled(state)
     
+    def _copy_bkg_scale_output(self):
+        # Copying of data to bkg_ui is handled by
+        # gui.main_widget.table_widget.copy_bkg_scale_result
+        # This function notifies the user that the bkg_ui tab has been updated
+        print('Background subtraction tab updated with refined scaling factor!')
+        _message = ['Background subtraction tab updated!', 'The background subtration tab has been updated with the refined scaling factor']
+        _error_msg = utility.ErrorMessageBox(_message)
+        _error_msg.exec_()
+
     def _copy_density_output(self):
         self.composition_gb.density_input.setText(self.optim_results_gb.density_output.text())
 
 
 class CompositionGroupBox(QGroupBox):
 
     with importlib_resources.open_binary('LiquidDiffract.resources', 'pt_data.npy') as fp:
@@ -812,22 +978,29 @@
         self.niter_label = QLabel('No. iterations: ')
         self.niter_input = QLineEdit('5')
         self.opt_check = QCheckBox('Refine density? ')
         self.lb_label = QLabel('Lower bound: ')
         self.lb_input = QLineEdit()
         self.ub_label = QLabel('Upper bound: ')
         self.ub_input = QLineEdit()
+        self.opt_check_bkg = QCheckBox('Refine background scale factor?')
+        self.lb_label_bkg = QLabel('Lower bound: ')
+        self.lb_input_bkg = QLineEdit()
+        self.ub_label_bkg = QLabel('Upper bound: ')
+        self.ub_input_bkg = QLineEdit()
         self.opt_button = QPushButton('Refine S(Q)')
 
     def style_widgets(self):
 
         self.rmin_label.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
         self.niter_label.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
         self.lb_label.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
         self.ub_label.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
+        self.lb_label_bkg.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
+        self.ub_label_bkg.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
 
         self.rmin_input.setAlignment(Qt.AlignRight)
         self.rmin_input.setValidator(QDoubleValidator())
         self.rmin_input.setMaximumWidth(70)
         self.rmin_input.setToolTip('Intramolecular distance cut-off')
         self.rmin_label.setToolTip('Intramolecular distance cut-off')
 
@@ -839,20 +1012,33 @@
         self.lb_input.setValidator(QDoubleValidator())
         self.lb_input.setMaximumWidth(70)
 
         self.ub_input.setAlignment(Qt.AlignRight)
         self.ub_input.setValidator(QDoubleValidator())
         self.ub_input.setMaximumWidth(70)
 
+        self.lb_input_bkg.setAlignment(Qt.AlignRight)
+        self.lb_input_bkg.setValidator(QDoubleValidator())
+        self.lb_input_bkg.setMaximumWidth(70)
+
+        self.ub_input_bkg.setAlignment(Qt.AlignRight)
+        self.ub_input_bkg.setValidator(QDoubleValidator())
+        self.ub_input_bkg.setMaximumWidth(70)
+
         self.opt_check.setChecked(False)
+        self.opt_check_bkg.setChecked(False)
 
         self.lb_label.setEnabled(False)
         self.lb_input.setEnabled(False)
         self.ub_label.setEnabled(False)
         self.ub_input.setEnabled(False)
+        self.lb_label_bkg.setEnabled(False)
+        self.lb_input_bkg.setEnabled(False)
+        self.ub_label_bkg.setEnabled(False)
+        self.ub_input_bkg.setEnabled(False)
 
     def create_layout(self):
 
         self.main_layout = QVBoxLayout()
         self.main_layout.setContentsMargins(20, 10, 20, 7)
         self.main_layout.setSpacing(25)
 
@@ -871,35 +1057,53 @@
         self.bottom_grid.setSpacing(15)
         self.bottom_grid.addWidget(self.opt_check, 0, 0)
         self.bottom_grid.addWidget(self.lb_label, 1, 0)
         self.bottom_grid.addWidget(self.lb_input, 1, 1)
         self.bottom_grid.addWidget(self.ub_label, 2, 0)
         self.bottom_grid.addWidget(self.ub_input, 2, 1)
 
+        self.bottom_grid.addWidget(self.opt_check_bkg, 3, 0)
+        self.bottom_grid.addWidget(self.lb_label_bkg, 4, 0)
+        self.bottom_grid.addWidget(self.lb_input_bkg, 4, 1)
+        self.bottom_grid.addWidget(self.ub_label_bkg, 5, 0)
+        self.bottom_grid.addWidget(self.ub_input_bkg, 5, 1)
+
         self.main_layout.addLayout(self.top_grid)
         self.main_layout.addLayout(self.bottom_grid)
         self.main_layout.addWidget(self.opt_button)
 
         self.setLayout(self.main_layout)
 
     def create_signals(self):
         self.opt_check.stateChanged.connect(self.opt_state_changed)
+        self.opt_check_bkg.stateChanged.connect(self.opt_bkg_state_changed)
 
     def opt_state_changed(self):
         if self.opt_check.isChecked():
             self.lb_input.setEnabled(True)
             self.lb_label.setEnabled(True)
             self.ub_input.setEnabled(True)
             self.ub_label.setEnabled(True)
         else:
             self.lb_input.setEnabled(False)
             self.lb_label.setEnabled(False)
             self.ub_input.setEnabled(False)
             self.ub_label.setEnabled(False)
 
+    def opt_bkg_state_changed(self):
+        if self.opt_check_bkg.isChecked():
+            self.lb_input_bkg.setEnabled(True)
+            self.lb_label_bkg.setEnabled(True)
+            self.ub_input_bkg.setEnabled(True)
+            self.ub_label_bkg.setEnabled(True)
+        else:
+            self.lb_input_bkg.setEnabled(False)
+            self.lb_label_bkg.setEnabled(False)
+            self.ub_input_bkg.setEnabled(False)
+            self.ub_label_bkg.setEnabled(False)
 
 class OptimResultsGroupBox(QGroupBox):
 
     def __init__(self, *args):
         super(OptimResultsGroupBox, self).__init__(*args)
         self.setTitle('Results')
         self.setAlignment(Qt.AlignLeft)
@@ -910,41 +1114,53 @@
         self.style_widgets()
         self.create_layout()
 
     def create_widgets(self):
 
         self.chi_sq_label = QLabel('Final Chi-squared: ')
         self.chi_sq_output = QLineEdit()
+        self.bkg_scale_output_label = QLabel('Refined background scale factor: ')
+        self.bkg_scale_output = QLineEdit()
+        self.bkg_scale_copy_btn = QPushButton()
         self.density_output_label = QLabel('Refined density (at/A<sup>3</sup>): ')
         self.density_output = QLineEdit()        
         self.density_copy_btn = QPushButton()
         self.mass_density_label = QLabel('(g/cm<sup>3</sup>): ')
         self.mass_density = QLineEdit()
 
     def style_widgets(self):
 
         self.chi_sq_label.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
+        self.bkg_scale_output_label.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
         self.density_output_label.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
         self.mass_density_label.setAlignment(Qt.AlignVCenter | Qt.AlignRight)
+        self.bkg_scale_copy_btn.setIcon(self.style().standardIcon(getattr(QStyle, 'SP_BrowserReload')))
         self.density_copy_btn.setIcon(self.style().standardIcon(getattr(QStyle, 'SP_BrowserReload')))
 
         self.chi_sq_output.isReadOnly()
+        self.bkg_scale_output.isReadOnly()
         self.density_output.isReadOnly()
         self.mass_density.isReadOnly()
         self.chi_sq_output.setMaximumWidth(82)
+        self.bkg_scale_output.setMaximumWidth(82)
         self.density_output.setMaximumWidth(82)
         self.mass_density.setMaximumWidth(82)
+        self.bkg_scale_copy_btn.setMaximumWidth(30)
         self.density_copy_btn.setMaximumWidth(30)
 
+        self.bkg_scale_output.setEnabled(False)
+        self.bkg_scale_output_label.setEnabled(False)
         self.density_output.setEnabled(False)
         self.density_output_label.setEnabled(False)
         self.mass_density.setEnabled(False)
         self.mass_density_label.setEnabled(False)
+        self.bkg_scale_copy_btn.setEnabled(False)
         self.density_copy_btn.setEnabled(False)
 
+        self.bkg_scale_output.setReadOnly(True)
         self.density_output.setReadOnly(True)
         self.chi_sq_output.setReadOnly(True)
         self.mass_density.setReadOnly(True)
 
     def create_layout(self):
 
         self.main_layout = QVBoxLayout()
@@ -952,16 +1168,19 @@
         self.main_layout.setSpacing(25)
 
         self.grid_layout = QGridLayout()
         self.grid_layout.setSpacing(15)
 
         self.grid_layout.addWidget(self.chi_sq_label, 0, 1)
         self.grid_layout.addWidget(self.chi_sq_output, 0, 2)
-        self.grid_layout.addWidget(self.density_copy_btn, 1, 0)
-        self.grid_layout.addWidget(self.density_output_label, 1, 1)
-        self.grid_layout.addWidget(self.density_output, 1, 2)
-        self.grid_layout.addWidget(self.mass_density_label, 2, 1)
-        self.grid_layout.addWidget(self.mass_density, 2, 2)
+        self.grid_layout.addWidget(self.bkg_scale_copy_btn, 1, 0)
+        self.grid_layout.addWidget(self.bkg_scale_output_label, 1, 1)
+        self.grid_layout.addWidget(self.bkg_scale_output, 1, 2)
+        self.grid_layout.addWidget(self.density_copy_btn, 2, 0)
+        self.grid_layout.addWidget(self.density_output_label, 2, 1)
+        self.grid_layout.addWidget(self.density_output, 2, 2)
+        self.grid_layout.addWidget(self.mass_density_label, 3, 1)
+        self.grid_layout.addWidget(self.mass_density, 3, 2)
 
         self.main_layout.addLayout(self.grid_layout)
 
         self.setLayout(self.main_layout)
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/gui/plot_widgets.py` & `LiquidDiffract-1.1.9/LiquidDiffract/gui/plot_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,20 +168,24 @@
         self.dr_plot.setLabel('left', text='D(r)')
 
         self.pos_label = pg.LabelItem(justify='right')
         self.pg_layout.addItem(self.pos_label, col=0, row=0)
 
     def update_plots(self, _data):
         try:
-            self.p1.clear()
+            self.p1_a.clear()
             self.p2_a.clear()
             self.p3_a.clear()
         except AttributeError:
             pass
         try:
+            self.p1_b.clear()
+        except AttributeError:
+            pass
+        try:
             self.p2_b.clear()
             self.p3_b.clear()
         except AttributeError:
             pass
         try:
             self.p2_c.clear()
         except AttributeError:
@@ -214,15 +218,16 @@
             try:
                 _window = np.argmax(_data['dr_x'] >= (1/_dq))
             except ValueError:
                  pass
         except IndexError:
             pass
 
-        self.p1 = self.data_plot.plot(x=_data['cor_x_cut'], y=_data['cor_y_cut'], pen={'color': 0.1, 'width': 1.2})
+        self.p1_a = self.data_plot.plot(x=_data['cor_x_cut'], y=_data['cor_y_cut'], pen={'color': 0.1, 'width': 1.2})
+        self.p1_b = self.data_plot.plot(x=_data['cor_x_cut'], y=_data['rescaled_cor_y_cut'], pen={'color': '#342256', 'width': 1.2, 'style': Qt.DashLine})
         self.p2_a = self.iq_plot.plot(x=_data['iq_x'], y=_data['int_func'], pen={'color': 0.1, 'width': 1.2})
         self.p2_b = self.iq_plot.plot(x=_data['impr_iq_x'], y=_data['impr_int_func'], pen={'color': '#342256', 'width': 1.2, 'style': Qt.DashLine})
         self.p3_a = self.dr_plot.plot(x=_data['dr_x'][:_window], y=_data['dr_y'][:_window], pen={'color': 0.1, 'width': 1.2})
         self.p3_b = self.dr_plot.plot(x=_data['impr_dr_x'][:_window], y=_data['impr_dr_y'][:_window], pen={'color': '#342256', 'width': 1.2, 'style': Qt.DashLine})
 
         if _data['mod_func'] != 'None':
             # Apply modification function and handle any nans that arise
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/gui/results_ui.py` & `LiquidDiffract-1.1.9/LiquidDiffract/gui/results_ui.py`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/gui/structure_ui.py` & `LiquidDiffract-1.1.9/LiquidDiffract/gui/structure_ui.py`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/gui/utility.py` & `LiquidDiffract-1.1.9/LiquidDiffract/gui/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -725,15 +725,15 @@
 class AboutDialog(QDialog):
     def __init__(self):
         super(AboutDialog, self).__init__()
         self.setAttribute(Qt.WA_DeleteOnClose)
         self.setWindowTitle
         self.title = __appname__ + ' v' + __version__
         self.setWindowTitle(self.title)
-        self.resize(595, 630)
+        self.resize(595, 675)
 
         self.vlayout = QVBoxLayout()
         self.vlayout.setContentsMargins(5, 15, 5, 7)
         self.vlayout.setSpacing(10)
 
         self.logo_box = QLabel()
 
@@ -746,14 +746,15 @@
         self.text_display = QTextBrowser()
         self.text_display.setReadOnly(True)
         self.text_display.setFrameStyle(QFrame.NoFrame)
         self.text_display.setStyleSheet("* { background-color: rgba(0, 0, 0, 0); }")
         self.text_display.setOpenExternalLinks(True)
 
         _app_url = 'https://github.com/bjheinen/LiquidDiffract'
+        _paper_url = 'https://doi.org/10.1007/s00269-022-01186-6'
         _gpl_url = 'https://www.gnu.org/licenses/gpl.html'
         _pstr = '<p class="western" align="center">'
         _description = ('LiquidDiffract is a graphical application for '
                         'X-ray total-scattering analysis of liquids and '
                         'disordered solids.\n'
                         'It implements procedures to obtain information on '
                         'macroscopic bulk properties and local atomic-scale '
@@ -761,19 +762,27 @@
                         'LiquidDiffract provides tools for  background '
                         'subtraction; calculation, normalisation, and '
                         'refinement of the reciprocal-space structure factor '
                         'and real-space correlation functions; '
                         'and extraction of structural information such as '
                         'bond lengths, coordination number and bulk density.'
                         )
+        _paper_str = (f'Heinen, B. J., & Drewitt, J. W. (2022). '
+                      f'LiquidDiffract: Software for liquid total scattering analysis. '
+                      f'<em>Physics and Chemistry of Minerals, 49:9</em>. doi:10.1007/s00269-022-01186-6')
 
         _app_url_str = (f'{_pstr}<a class="western" href="{_app_url}">'
                         f'<span style="color: #000080;"><span lang="zxx">'
                         f'<u>{_app_url}</u></span></span></a></p>'
                         )
+        _cite_str = (f'{_pstr}If you use LiquidDiffract in your work please cite it as:<br><br>'
+                     f'<a class="western" href="{_paper_url}">'
+                     f'<span style="color: #000080;"><span lang="zxx">'
+                     f'<u>{_paper_str}</u></span></span></a></p>')
+
         _copyright = 'Copyright &copy; 2018-2021 &ndash; Benedict J. Heinen'
         _warranty = ('This program comes with absolutely no '
                      'warranty or guarantee.')
         _license = '<u>GNU General Public Licence, version 3 or later</u>'
 
         _l_str = (f'See the </span><a class="western" href="{_gpl_url}">'
                   f'<span style="color: #000080;"><span style='
@@ -785,14 +794,16 @@
         _text = (f'{_pstr}<strong>{__appname__}</strong></p>'
                  f'{_pstr}v{__version__}</p>'
                  f'{_pstr}&nbsp;</p>'
                  f'{_pstr}<em>{_description}</em></p>'
                  f'{_pstr}&nbsp;</p>'
                  f'{_app_url_str}'
                  f'{_pstr}&nbsp;</p>'
+                 f'{_cite_str}'
+                 f'{_pstr}&nbsp;</p>'
                  f'{_pstr}<span style="font-size: small;">{_copyright}</span></p>'
                  f'{_pstr}<span style="font-size: small;">{_warranty}<br>'
                  f'{_l_str}'
                  )
         self.text_display.textCursor().insertHtml(_text)
 
         self.vlayout.addWidget(self.logo_box)
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/4_and_25_iterations.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/4_and_25_iterations.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/LiquidDiffract v1.1.6-dev_refinement_tab.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/LiquidDiffract v1.1.6-dev_refinement_tab.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/chi_squared_minimum_map.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/chi_squared_minimum_map.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/fitting_region.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/fitting_region.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/docs/optimal_n_iter.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/docs/optimal_n_iter.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/form_factors.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/form_factors.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/A.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/A.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ag.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ag.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Al.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Al.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ar.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ar.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/As.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/As.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/At.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/At.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Au.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Au.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/B.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/B.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ba.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ba.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Be.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Be.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Bi.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Bi.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Bk.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Bk.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Br.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Br.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/C.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/C.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ca.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ca.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cd.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cd.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ce.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ce.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cf.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cf.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cl.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cl.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Co.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Co.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cr.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cr.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cs.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cs.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Cu.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Cu.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Dy.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Dy.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Er.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Er.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Es.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Es.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Eu.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Eu.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/F.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/F.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Fe.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Fe.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Fr.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Fr.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ga.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ga.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Gd.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Gd.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ge.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ge.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/H.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/H.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/He.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/He.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Hf.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Hf.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ho.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ho.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/I.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/I.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/In.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/In.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ir.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ir.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/K.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/K.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Kr.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Kr.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/La.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/La.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Li.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Li.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Lu.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Lu.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Mg.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Mg.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Mn.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Mn.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Mo.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Mo.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/N.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/N.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Na.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Na.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Nb.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Nb.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Nd.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Nd.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ne.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ne.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ni.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ni.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/O.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/O.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Os.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Os.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/P.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/P.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pa.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pa.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pb.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pb.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pd.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pd.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Po.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Po.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pr.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pr.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pt.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pt.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Pu.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Pu.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ra.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ra.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Rb.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Rb.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Re.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Re.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Rh.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Rh.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Rn.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Rn.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ru.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ru.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/S.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/S.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Sb.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Sb.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Se.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Se.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Si.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Si.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Sn.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Sn.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Sr.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Sr.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/T.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/T.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ta.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ta.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Tb.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Tb.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Te.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Te.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Th.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Th.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Ti.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Ti.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Tl.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Tl.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/U.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/U.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/V.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/V.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/W.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/W.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Xe.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Xe.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Y.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Y.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Yb.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Yb.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Zn.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Zn.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/Zr.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/Zr.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/hubbel_compton/hg.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/hubbel_compton/hg.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/browser.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/browser.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/config.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/config.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/gs_icon.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/gs_icon.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/info.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/info.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/icons/logo.png` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/icons/logo.png`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/mass_data.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/mass_data.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/resources/pt_data.npy` & `LiquidDiffract-1.1.9/LiquidDiffract/resources/pt_data.npy`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/scripts/brute.py` & `LiquidDiffract-1.1.9/LiquidDiffract/scripts/brute.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,28 @@
             res.append(brute_slice)
         return np.asarray(res)
     else:
         pass
     func_args = tuple(func_args.values())
     res = []
     for iteration, rho in enumerate(brute_array):
-        chi_sq = liquid.calc_impr_interference_func(rho, *func_args)
+        chi_sq = liquid.refinement_objfun(rho, *func_args)
         elapsed_time = time.time() - start_time
         iteration_num = (iteration + 1) + (len(brute_array)*slice_number)
         update_progress_bar(iteration_num, brute_iterations, elapsed_time, estimated_total_time)
         res.append(chi_sq)
     res = np.asarray(res)
     return res
 
 # Data Options
 data_file = 'example_data.dat'
 q_max = 11.8
 comp = {'Ga':(31,0,1)}
 dq = 0.02
-sq_form = 'ashcroft-langreth'
+sq_form = 'faber-ziman'
 mod_func = None
 window_start = None
 r_min = 2.3
 fft_N = 12
 
 # Set the array of values to compute X^2
 brute_rho_array = np.arange(0.01, 0.08, 0.001)
@@ -103,15 +103,15 @@
 # Cut data at Q_max
 x, y = x[np.where(x < q_max)], y[np.where(x < q_max)]
 
 func_args = {'Q_data': x, 'I_data': y, 'comp': comp,
              'r_min': r_min, 'n_iter': int(np.mean(brute_eggert_iterations_array)),
              'method': sq_form, 'mod_func': mod_func,
              'window_start': window_start, 'fft_N': fft_N,
-             'opt_flag': 1}
+             'opt_rho': 1, 'opt_bkg': 0}
 
 brute_array = (brute_eggert_iterations_array, brute_rho_array)
 brute_iterations = len(brute_rho_array) * len(brute_eggert_iterations_array)
 # Here we calculate the time to make 1 iteration
 t_start = time.time()
 brute_compute([1], func_args, 1, 1, 1, 1)
 t_end = time.time()
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/scripts/example_data.dat` & `LiquidDiffract-1.1.9/LiquidDiffract/scripts/example_data.dat`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract/scripts/example_usage.py` & `LiquidDiffract-1.1.9/LiquidDiffract/scripts/example_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 calc_impr_interference_func optimises the interference function, S(Q) - S_inf,
 based on the iterative method developed by Eggert et al., 2002, Phy Rev B, 65(17).
 
 See <https://github.com/bjheinen/LiquidDiffract> for more details.
 """
 __author__ = 'Benedict J. Heinen'
-__copyright__ = 'Copyright 2018-2021, Benedict J. Heinen'
+__copyright__ = 'Copyright 2018-2022, Benedict J. Heinen'
 __email__ = 'benedict.heinen@gmail.com'
 __license__='GPLv3'
 
 # Import required python modules
 import numpy as np
 # Import optional python modules used in this example
 import matplotlib.pyplot as plt
@@ -92,53 +92,60 @@
 #
 # The last positional argument (opt_flag) signals that you only want the chi_squared value to be returned.
 # This is useful if using a solver to refine the density by minimising the chi_squared value
 
 # e.g.
 # Return the improved i(Q) & chi^2 at density = rho_0
 iter_limit = 25
-method = 'ashcroft-langreth'
+method = 'faber-ziman'
 mod_func = 'Cosine-window'
 window_start = 7
 fft_N = 12
-args = (q_data, interference_func_0, composition, r_min,
-        iter_limit, method, mod_func, window_start, fft_N, 0)
+args = (q_data, interference_func_0, composition, rho_0,
+        r_min, iter_limit, method, mod_func, window_start, fft_N)
 # Store the refined interference function at rho_0
-interference_func_1, chi_sq_1 = liquid.calc_impr_interference_func(rho_0, *args)
+interference_func_1, chi_sq_1 = liquid.calc_impr_interference_func(*args)
 
-# Next we use opt_flag = 1 and pass the function calc_impr_interference_func to
-# a solver to estimate the density
+# Next we pass the function calc_impr_interference_func to
+# a solver to estimate the density. We use a separate objective function
+# core.redinement_objfun to make this simpler.
+# The argument opt_rho is set to 1 to indicate we are refining the density
+opt_rho = 1
+# The argument opt_bkg is set to 0 to indicate we are not refining
+# the background sclaing factor.
+opt_bkg = 0
 # When refinind the density an iter_limit <= 10 is recommended
 iter_limit_refine = 7
 args = (q_data, I_data, composition, r_min,
-        iter_limit_refine, method, mod_func, window_start, fft_N, 1)
+        iter_limit_refine, method,
+        mod_func, window_start, fft_N,
+        opt_rho, opt_bkg)
 # Set-up bounds and other options according to the documentation of solver/minimisation routine
 bounds = ((0.045, 0.065),)
 op_method = 'L-BFGS-B'
 optimisation_options = {'disp': 0,
                         'maxiter': 15000,
                         'maxfun': 15000,
                         'ftol': 2.22e-12,
                         'gtol': 1e-12
                         }
-opt_result = minimize(liquid.calc_impr_interference_func, rho_0,
+opt_result = minimize(liquid.refinement_objfun, rho_0,
                       bounds=bounds, args=args,
                       options=optimisation_options,
                       method=op_method)
 # The solver finds the value of rho that gives the smallest chi^2
 rho_refined = opt_result.x[0]
 
 # The interference function can then be re-calculated using the new value for rho,
 # and the F(r) refined as above.
-interference_func = (liquid.calc_structure_factor(q_data,I_data, composition, rho_refined) - 
+interference_func = (liquid.calc_structure_factor(q_data, I_data, composition, rho_refined) -
                      liquid.calc_S_inf(composition, q_data))
-
-args = (q_data, interference_func, composition, r_min,
-        iter_limit, method, mod_func, window_start, fft_N, 0)
-interference_func_2, chi_sq_2 = liquid.calc_impr_interference_func(rho_refined, *args)
+args = (q_data, interference_func_0, composition, rho_refined,
+        r_min, iter_limit, method, mod_func, window_start, fft_N)
+interference_func_2, chi_sq_2 = liquid.calc_impr_interference_func(*args)
 
 # Calculate the corresponding pair distribution functions g(r)
 r, g_r_0 = liquid.calc_correlation_func(q_data, interference_func_0, rho_0, dx=dq,
                                         mod_func=mod_func, window_start=window_start,
                                         function='pair_dist_func')
 # r values will be the same
 _, g_r_1 = liquid.calc_correlation_func(q_data, interference_func_1, rho_0, dx=dq,
@@ -173,8 +180,8 @@
 # Optimised g(r) at rho_0
 plt.plot(r[:window], g_r_1[:window], color='r', label=r'Optimised g(r) | $ρ = {rho:.2f}$ & $χ^{{2}} = {chisq:.2f}$'.format(rho=rho_0, chisq=chi_sq_1))
 # Optimised g(r), using refined density estimate
 plt.plot(r[:window], g_r_2[:window], color='b', label=r'Optimised g(r) | $ρ = {rho:.3f}$ & $χ^{{2}} = {chisq:.2f}$'.format(rho=rho_refined, chisq=chi_sq_2))
 # Add a legend
 plt.legend(loc='best')
 # Show the plots
-plt.show()
+plt.show()
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract.egg-info/PKG-INFO` & `LiquidDiffract-1.1.9/LiquidDiffract.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: LiquidDiffract
-Version: 1.1.8
+Version: 1.1.9
 Summary: Liquid structure/total X-ray scattering analysis
 Home-page: https://github.com/bjheinen/LiquidDiffract
 Author: Benedict J Heinen
 Author-email: benedict.heinen@gmail.com
 License: GPL
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![DOI](https://zenodo.org/badge/147495370.svg)](https://zenodo.org/badge/latestdoi/147495370)
 
@@ -22,28 +21,35 @@
 </p>
 
 
 ### Maintainer
 
 Benedict J. Heinen (benedict.heinen@gmail.com)
 
+### Citing LiquidDiffract
+
+LiquidDiffract is described in an open access paper published in Physics and Chemistry of Minerals:
+
+[Heinen, B. J., & Drewitt, J. W. (2022). LiquidDiffract: Software for liquid total scattering analysis. *Physics and Chemistry of Minerals, 49:9*. doi:10.1007/s00269-022-01186-6](https://link.springer.com/content/pdf/10.1007/s00269-022-01186-6.pdf)
+
+Please cite this article if you use LiquidDiffract in your work.
 
 ## Table of Contents
 
 * [Requirements](#requirements)
 * [Installation](#installation)
 * [Usage](#usage)
 	* [Loading the GUI](#loading-the-gui)
 	* [Basic Usage](#basic-usage)
 	* [Background Subtraction Tab](#background-subtraction-tab)
 	* [Refinement Tab](#refinement-tab)
 		* [Composition Toolbox](#composition-toolbox)
 		* [Data Options](#data-options)
 		* [Iterative Structure Factor Refinement](#iterative-structure-factor-refinement)
-		* [Density (&rho;) Refinement](#density-%CF%81-refinement)
+		* [Density (&rho;) and background scaling (b) Refinement](#density-%CF%81-and-background-scaling-factor-b-refinement)
 			* [Global optimisation capability](#global-optimisation-capability)
 		* [Note on Number of Iterations in the Eggert Procedure & *&Chi;<sup>2</sup>* Minimisation](#note-on-number-of-iterations-in-the-eggert-procedure--χ2-minimisation)
 		* [Terminal & Log-file Output](#terminal--log-file-output)
 	* [PDF Calculation (Output) Tab](#pdf-calculation-output-tab)
 	* [Structural Information Tab](#structural-information-tab)
 		* [Integration Toolbox (monatomic compositions)](#integration-toolbox)
 		* [Curve-fitting Toolbox (polyatomic compositions)](#curve-fitting-toolbox)
@@ -186,31 +192,33 @@
 
 To refine *S(Q)* the value of *r*-min should be set carefully, as it has a strong influence. The position of *r*-min should correspond to the base of the first coordinence sphere in the *g(r)*.
 
 The number of iterations in the procedure can also be set; a minimum of 3 is normally required for convergence.
 
 A *&Chi;<sup>2</sup>* figure of merit, defined as the area under the curve *&Delta;D(r) for r<r-min*, is used to rate the refinement.
 
-><img src='http://latex.codecogs.com/svg.latex?\chi^{2}_{\left(n\right)}(\rho)=\int_{0}^{r_{min}}\left[\Delta{D}_{(n)}(r)\right]^2dr'/>
+><img src='http://latex.codecogs.com/svg.latex?\chi^{2}_{\left(n\right)}(\rho;b)=\int_{0}^{r_{min}}\left[\Delta{D}_{(n)}(r)\right]^2dr'/>
 
 Where,
 
 ><img src='http://latex.codecogs.com/svg.latex?\Delta{D}_{(n)}(r)= D_{(n)}(r)-\left(-4\pi\rho{r}\right),\;for\;r<r_{min}'/>
 
-#### Density (&rho;) Refinement
+#### Density (&rho;) and background scaling factor (*b*) Refinement
 
-The sample density can be determined by finding the value of &rho; that provides the best convergence of the iterative procedure described above. This is done by minimising the resultant value of *&Chi;<sup>2</sup>*. LiquidDiffract supports several different solvers to do this. The solver in use, along with specific options like convergence criteria and number of iterations, can be selected from the *Additional Preferences* dialog. The solvers currently supported are:
+The sample density and/or background scaling factor can be determined by finding the values of &rho; and or b that provides the best convergence of the iterative procedure described above. This is done by minimising the resultant value of *&Chi;<sup>2</sup>*. LiquidDiffract supports several different solvers to do this. The solver in use, along with specific options like convergence criteria and number of iterations, can be selected from the *Additional Preferences* dialog. The solvers currently supported are:
 
 * L-BFGS-B [16-17]
 
 * SLSQP [18]
 
 * COBYLA [19-21]
 
-All solvers require upper and lower bounds on the density to be set.
+All solvers require upper and lower bounds on the density and or background scaling factor to be set.
+
+The density and background scaling factor can be refined independently or simultaneously.
 
 For more information on these optimisation algorithms please see the [SciPy documentation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html), or consult the references listed.
 
 ##### Global optimisation capability
 
 The optimisation algorithms used to estimate density work best when the initial guess, &rho;<sub>0</sub> is close to the true value. If the density of the material is very poorly known it is recommended to use the global optimisation option provided. It is not recommended if a good initial guess can be made, due to slower, and sometimes poor, convergence.
 
@@ -395,53 +403,61 @@
 #
 # The last positional argument (opt_flag) signals that you only want the chi_squared value to be returned.
 # This is useful if using a solver to refine the density by minimising the chi_squared value
 
 # e.g.
 # Return the improved i(Q) & chi^2 at density = rho_0
 iter_limit = 25
-method = 'ashcroft-langreth'
+method = 'faber-ziman'
 mod_func = 'Cosine-window'
 window_start = 7
 fft_N = 12
-args = (q_data, interference_func_0, composition, r_min,
-        iter_limit, method, mod_func, window_start, fft_N, 0)
+args = (q_data, interference_func_0, composition, rho_0,
+        r_min, iter_limit, method, mod_func, window_start, fft_N)
 # Store the refined interference function at rho_0
-interference_func_1, chi_sq_1 = liquid.calc_impr_interference_func(rho_0, *args)
+interference_func_1, chi_sq_1 = liquid.calc_impr_interference_func(*args)
 
-# Next we use opt_flag = 1 and pass the function calc_impr_interference_func to
-# a solver to estimate the density
+# Next we pass the function calc_impr_interference_func to
+# a solver to estimate the density. We use a separate objective function
+# core.redinement_objfun to make this simpler.
+# The argument opt_rho is set to 1 to indicate we are refining the density
+opt_rho = 1
+# The argument opt_bkg is set to 0 to indicate we are not refining
+# the background sclaing factor.
+opt_bkg = 0
 # When refinind the density an iter_limit <= 10 is recommended
 iter_limit_refine = 7
 args = (q_data, I_data, composition, r_min,
-        iter_limit_refine, method, mod_func, window_start, fft_N, 1)
+        iter_limit_refine, method,
+        mod_func, window_start, fft_N,
+        opt_rho, opt_bkg)
 # Set-up bounds and other options according to the documentation of solver/minimisation routine
 bounds = ((0.045, 0.065),)
 op_method = 'L-BFGS-B'
 optimisation_options = {'disp': 0,
                         'maxiter': 15000,
                         'maxfun': 15000,
                         'ftol': 2.22e-12,
                         'gtol': 1e-12
                         }
-opt_result = minimize(liquid.calc_impr_interference_func, rho_0,
+opt_result = minimize(liquid.refinement_objfun, rho_0,
                       bounds=bounds, args=args,
                       options=optimisation_options,
                       method=op_method)
 # The solver finds the value of rho that gives the smallest chi^2
 rho_refined = opt_result.x[0]
 
 # The interference function can then be re-calculated using the new value for rho,
 # and the F(r) refined as above.
 interference_func = (liquid.calc_structure_factor(q_data,I_data, composition, rho_refined) - 
                      liquid.calc_S_inf(composition, q_data))
 
-args = (q_data, interference_func, composition, r_min,
-        iter_limit, method, mod_func, window_start, fft_N, 0)
-interference_func_2, chi_sq_2 = liquid.calc_impr_interference_func(rho_refined, *args)
+args = (q_data, interference_func, composition, rho_refined,
+        r_min, iter_limit, method, mod_func, window_start, fft_N)
+interference_func_2, chi_sq_2 = liquid.calc_impr_interference_func(*args)
 
 # Calculate the corresponding pair distribution functions g(r)
 r, g_r_0 = liquid.calc_correlation_func(q_data, interference_func_0, rho_0, dx=dq,
                                         mod_func=mod_func, window_start=window_start,
                                         function='pair_dist_func')
 # r values will be the same
 _, g_r_1 = liquid.calc_correlation_func(q_data, interference_func_1, rho_0, dx=dq,
@@ -551,10 +567,8 @@
 
 Licensed under the GNU General Public License (GPL), version 3 or later.
 
 See the [license file](../master/LICENSE) for more information.
 
 This program comes with absolutely no warranty or guarantee.
 
-Copyright © 2018-2021 – Benedict J Heinen
-
-
+Copyright © 2018-2022 – Benedict J Heinen
```

### Comparing `LiquidDiffract-1.1.8/LiquidDiffract.egg-info/SOURCES.txt` & `LiquidDiffract-1.1.9/LiquidDiffract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LiquidDiffract-1.1.8/PKG-INFO` & `LiquidDiffract-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: LiquidDiffract
-Version: 1.1.8
+Version: 1.1.9
 Summary: Liquid structure/total X-ray scattering analysis
 Home-page: https://github.com/bjheinen/LiquidDiffract
 Author: Benedict J Heinen
 Author-email: benedict.heinen@gmail.com
 License: GPL
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![DOI](https://zenodo.org/badge/147495370.svg)](https://zenodo.org/badge/latestdoi/147495370)
 
@@ -22,28 +21,35 @@
 </p>
 
 
 ### Maintainer
 
 Benedict J. Heinen (benedict.heinen@gmail.com)
 
+### Citing LiquidDiffract
+
+LiquidDiffract is described in an open access paper published in Physics and Chemistry of Minerals:
+
+[Heinen, B. J., & Drewitt, J. W. (2022). LiquidDiffract: Software for liquid total scattering analysis. *Physics and Chemistry of Minerals, 49:9*. doi:10.1007/s00269-022-01186-6](https://link.springer.com/content/pdf/10.1007/s00269-022-01186-6.pdf)
+
+Please cite this article if you use LiquidDiffract in your work.
 
 ## Table of Contents
 
 * [Requirements](#requirements)
 * [Installation](#installation)
 * [Usage](#usage)
 	* [Loading the GUI](#loading-the-gui)
 	* [Basic Usage](#basic-usage)
 	* [Background Subtraction Tab](#background-subtraction-tab)
 	* [Refinement Tab](#refinement-tab)
 		* [Composition Toolbox](#composition-toolbox)
 		* [Data Options](#data-options)
 		* [Iterative Structure Factor Refinement](#iterative-structure-factor-refinement)
-		* [Density (&rho;) Refinement](#density-%CF%81-refinement)
+		* [Density (&rho;) and background scaling (b) Refinement](#density-%CF%81-and-background-scaling-factor-b-refinement)
 			* [Global optimisation capability](#global-optimisation-capability)
 		* [Note on Number of Iterations in the Eggert Procedure & *&Chi;<sup>2</sup>* Minimisation](#note-on-number-of-iterations-in-the-eggert-procedure--χ2-minimisation)
 		* [Terminal & Log-file Output](#terminal--log-file-output)
 	* [PDF Calculation (Output) Tab](#pdf-calculation-output-tab)
 	* [Structural Information Tab](#structural-information-tab)
 		* [Integration Toolbox (monatomic compositions)](#integration-toolbox)
 		* [Curve-fitting Toolbox (polyatomic compositions)](#curve-fitting-toolbox)
@@ -186,31 +192,33 @@
 
 To refine *S(Q)* the value of *r*-min should be set carefully, as it has a strong influence. The position of *r*-min should correspond to the base of the first coordinence sphere in the *g(r)*.
 
 The number of iterations in the procedure can also be set; a minimum of 3 is normally required for convergence.
 
 A *&Chi;<sup>2</sup>* figure of merit, defined as the area under the curve *&Delta;D(r) for r<r-min*, is used to rate the refinement.
 
-><img src='http://latex.codecogs.com/svg.latex?\chi^{2}_{\left(n\right)}(\rho)=\int_{0}^{r_{min}}\left[\Delta{D}_{(n)}(r)\right]^2dr'/>
+><img src='http://latex.codecogs.com/svg.latex?\chi^{2}_{\left(n\right)}(\rho;b)=\int_{0}^{r_{min}}\left[\Delta{D}_{(n)}(r)\right]^2dr'/>
 
 Where,
 
 ><img src='http://latex.codecogs.com/svg.latex?\Delta{D}_{(n)}(r)= D_{(n)}(r)-\left(-4\pi\rho{r}\right),\;for\;r<r_{min}'/>
 
-#### Density (&rho;) Refinement
+#### Density (&rho;) and background scaling factor (*b*) Refinement
 
-The sample density can be determined by finding the value of &rho; that provides the best convergence of the iterative procedure described above. This is done by minimising the resultant value of *&Chi;<sup>2</sup>*. LiquidDiffract supports several different solvers to do this. The solver in use, along with specific options like convergence criteria and number of iterations, can be selected from the *Additional Preferences* dialog. The solvers currently supported are:
+The sample density and/or background scaling factor can be determined by finding the values of &rho; and or b that provides the best convergence of the iterative procedure described above. This is done by minimising the resultant value of *&Chi;<sup>2</sup>*. LiquidDiffract supports several different solvers to do this. The solver in use, along with specific options like convergence criteria and number of iterations, can be selected from the *Additional Preferences* dialog. The solvers currently supported are:
 
 * L-BFGS-B [16-17]
 
 * SLSQP [18]
 
 * COBYLA [19-21]
 
-All solvers require upper and lower bounds on the density to be set.
+All solvers require upper and lower bounds on the density and or background scaling factor to be set.
+
+The density and background scaling factor can be refined independently or simultaneously.
 
 For more information on these optimisation algorithms please see the [SciPy documentation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html), or consult the references listed.
 
 ##### Global optimisation capability
 
 The optimisation algorithms used to estimate density work best when the initial guess, &rho;<sub>0</sub> is close to the true value. If the density of the material is very poorly known it is recommended to use the global optimisation option provided. It is not recommended if a good initial guess can be made, due to slower, and sometimes poor, convergence.
 
@@ -395,53 +403,61 @@
 #
 # The last positional argument (opt_flag) signals that you only want the chi_squared value to be returned.
 # This is useful if using a solver to refine the density by minimising the chi_squared value
 
 # e.g.
 # Return the improved i(Q) & chi^2 at density = rho_0
 iter_limit = 25
-method = 'ashcroft-langreth'
+method = 'faber-ziman'
 mod_func = 'Cosine-window'
 window_start = 7
 fft_N = 12
-args = (q_data, interference_func_0, composition, r_min,
-        iter_limit, method, mod_func, window_start, fft_N, 0)
+args = (q_data, interference_func_0, composition, rho_0,
+        r_min, iter_limit, method, mod_func, window_start, fft_N)
 # Store the refined interference function at rho_0
-interference_func_1, chi_sq_1 = liquid.calc_impr_interference_func(rho_0, *args)
+interference_func_1, chi_sq_1 = liquid.calc_impr_interference_func(*args)
 
-# Next we use opt_flag = 1 and pass the function calc_impr_interference_func to
-# a solver to estimate the density
+# Next we pass the function calc_impr_interference_func to
+# a solver to estimate the density. We use a separate objective function
+# core.redinement_objfun to make this simpler.
+# The argument opt_rho is set to 1 to indicate we are refining the density
+opt_rho = 1
+# The argument opt_bkg is set to 0 to indicate we are not refining
+# the background sclaing factor.
+opt_bkg = 0
 # When refinind the density an iter_limit <= 10 is recommended
 iter_limit_refine = 7
 args = (q_data, I_data, composition, r_min,
-        iter_limit_refine, method, mod_func, window_start, fft_N, 1)
+        iter_limit_refine, method,
+        mod_func, window_start, fft_N,
+        opt_rho, opt_bkg)
 # Set-up bounds and other options according to the documentation of solver/minimisation routine
 bounds = ((0.045, 0.065),)
 op_method = 'L-BFGS-B'
 optimisation_options = {'disp': 0,
                         'maxiter': 15000,
                         'maxfun': 15000,
                         'ftol': 2.22e-12,
                         'gtol': 1e-12
                         }
-opt_result = minimize(liquid.calc_impr_interference_func, rho_0,
+opt_result = minimize(liquid.refinement_objfun, rho_0,
                       bounds=bounds, args=args,
                       options=optimisation_options,
                       method=op_method)
 # The solver finds the value of rho that gives the smallest chi^2
 rho_refined = opt_result.x[0]
 
 # The interference function can then be re-calculated using the new value for rho,
 # and the F(r) refined as above.
 interference_func = (liquid.calc_structure_factor(q_data,I_data, composition, rho_refined) - 
                      liquid.calc_S_inf(composition, q_data))
 
-args = (q_data, interference_func, composition, r_min,
-        iter_limit, method, mod_func, window_start, fft_N, 0)
-interference_func_2, chi_sq_2 = liquid.calc_impr_interference_func(rho_refined, *args)
+args = (q_data, interference_func, composition, rho_refined,
+        r_min, iter_limit, method, mod_func, window_start, fft_N)
+interference_func_2, chi_sq_2 = liquid.calc_impr_interference_func(*args)
 
 # Calculate the corresponding pair distribution functions g(r)
 r, g_r_0 = liquid.calc_correlation_func(q_data, interference_func_0, rho_0, dx=dq,
                                         mod_func=mod_func, window_start=window_start,
                                         function='pair_dist_func')
 # r values will be the same
 _, g_r_1 = liquid.calc_correlation_func(q_data, interference_func_1, rho_0, dx=dq,
@@ -551,10 +567,8 @@
 
 Licensed under the GNU General Public License (GPL), version 3 or later.
 
 See the [license file](../master/LICENSE) for more information.
 
 This program comes with absolutely no warranty or guarantee.
 
-Copyright © 2018-2021 – Benedict J Heinen
-
-
+Copyright © 2018-2022 – Benedict J Heinen
```

### Comparing `LiquidDiffract-1.1.8/README.md` & `LiquidDiffract-1.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,35 @@
 </p>
 
 
 ### Maintainer
 
 Benedict J. Heinen (benedict.heinen@gmail.com)
 
+### Citing LiquidDiffract
+
+LiquidDiffract is described in an open access paper published in Physics and Chemistry of Minerals:
+
+[Heinen, B. J., & Drewitt, J. W. (2022). LiquidDiffract: Software for liquid total scattering analysis. *Physics and Chemistry of Minerals, 49:9*. doi:10.1007/s00269-022-01186-6](https://link.springer.com/content/pdf/10.1007/s00269-022-01186-6.pdf)
+
+Please cite this article if you use LiquidDiffract in your work.
 
 ## Table of Contents
 
 * [Requirements](#requirements)
 * [Installation](#installation)
 * [Usage](#usage)
 	* [Loading the GUI](#loading-the-gui)
 	* [Basic Usage](#basic-usage)
 	* [Background Subtraction Tab](#background-subtraction-tab)
 	* [Refinement Tab](#refinement-tab)
 		* [Composition Toolbox](#composition-toolbox)
 		* [Data Options](#data-options)
 		* [Iterative Structure Factor Refinement](#iterative-structure-factor-refinement)
-		* [Density (&rho;) Refinement](#density-%CF%81-refinement)
+		* [Density (&rho;) and background scaling (b) Refinement](#density-%CF%81-and-background-scaling-factor-b-refinement)
 			* [Global optimisation capability](#global-optimisation-capability)
 		* [Note on Number of Iterations in the Eggert Procedure & *&Chi;<sup>2</sup>* Minimisation](#note-on-number-of-iterations-in-the-eggert-procedure--χ2-minimisation)
 		* [Terminal & Log-file Output](#terminal--log-file-output)
 	* [PDF Calculation (Output) Tab](#pdf-calculation-output-tab)
 	* [Structural Information Tab](#structural-information-tab)
 		* [Integration Toolbox (monatomic compositions)](#integration-toolbox)
 		* [Curve-fitting Toolbox (polyatomic compositions)](#curve-fitting-toolbox)
@@ -173,31 +180,33 @@
 
 To refine *S(Q)* the value of *r*-min should be set carefully, as it has a strong influence. The position of *r*-min should correspond to the base of the first coordinence sphere in the *g(r)*.
 
 The number of iterations in the procedure can also be set; a minimum of 3 is normally required for convergence.
 
 A *&Chi;<sup>2</sup>* figure of merit, defined as the area under the curve *&Delta;D(r) for r<r-min*, is used to rate the refinement.
 
-><img src='http://latex.codecogs.com/svg.latex?\chi^{2}_{\left(n\right)}(\rho)=\int_{0}^{r_{min}}\left[\Delta{D}_{(n)}(r)\right]^2dr'/>
+><img src='http://latex.codecogs.com/svg.latex?\chi^{2}_{\left(n\right)}(\rho;b)=\int_{0}^{r_{min}}\left[\Delta{D}_{(n)}(r)\right]^2dr'/>
 
 Where,
 
 ><img src='http://latex.codecogs.com/svg.latex?\Delta{D}_{(n)}(r)= D_{(n)}(r)-\left(-4\pi\rho{r}\right),\;for\;r<r_{min}'/>
 
-#### Density (&rho;) Refinement
+#### Density (&rho;) and background scaling factor (*b*) Refinement
 
-The sample density can be determined by finding the value of &rho; that provides the best convergence of the iterative procedure described above. This is done by minimising the resultant value of *&Chi;<sup>2</sup>*. LiquidDiffract supports several different solvers to do this. The solver in use, along with specific options like convergence criteria and number of iterations, can be selected from the *Additional Preferences* dialog. The solvers currently supported are:
+The sample density and/or background scaling factor can be determined by finding the values of &rho; and or b that provides the best convergence of the iterative procedure described above. This is done by minimising the resultant value of *&Chi;<sup>2</sup>*. LiquidDiffract supports several different solvers to do this. The solver in use, along with specific options like convergence criteria and number of iterations, can be selected from the *Additional Preferences* dialog. The solvers currently supported are:
 
 * L-BFGS-B [16-17]
 
 * SLSQP [18]
 
 * COBYLA [19-21]
 
-All solvers require upper and lower bounds on the density to be set.
+All solvers require upper and lower bounds on the density and or background scaling factor to be set.
+
+The density and background scaling factor can be refined independently or simultaneously.
 
 For more information on these optimisation algorithms please see the [SciPy documentation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html), or consult the references listed.
 
 ##### Global optimisation capability
 
 The optimisation algorithms used to estimate density work best when the initial guess, &rho;<sub>0</sub> is close to the true value. If the density of the material is very poorly known it is recommended to use the global optimisation option provided. It is not recommended if a good initial guess can be made, due to slower, and sometimes poor, convergence.
 
@@ -382,53 +391,61 @@
 #
 # The last positional argument (opt_flag) signals that you only want the chi_squared value to be returned.
 # This is useful if using a solver to refine the density by minimising the chi_squared value
 
 # e.g.
 # Return the improved i(Q) & chi^2 at density = rho_0
 iter_limit = 25
-method = 'ashcroft-langreth'
+method = 'faber-ziman'
 mod_func = 'Cosine-window'
 window_start = 7
 fft_N = 12
-args = (q_data, interference_func_0, composition, r_min,
-        iter_limit, method, mod_func, window_start, fft_N, 0)
+args = (q_data, interference_func_0, composition, rho_0,
+        r_min, iter_limit, method, mod_func, window_start, fft_N)
 # Store the refined interference function at rho_0
-interference_func_1, chi_sq_1 = liquid.calc_impr_interference_func(rho_0, *args)
+interference_func_1, chi_sq_1 = liquid.calc_impr_interference_func(*args)
 
-# Next we use opt_flag = 1 and pass the function calc_impr_interference_func to
-# a solver to estimate the density
+# Next we pass the function calc_impr_interference_func to
+# a solver to estimate the density. We use a separate objective function
+# core.redinement_objfun to make this simpler.
+# The argument opt_rho is set to 1 to indicate we are refining the density
+opt_rho = 1
+# The argument opt_bkg is set to 0 to indicate we are not refining
+# the background sclaing factor.
+opt_bkg = 0
 # When refinind the density an iter_limit <= 10 is recommended
 iter_limit_refine = 7
 args = (q_data, I_data, composition, r_min,
-        iter_limit_refine, method, mod_func, window_start, fft_N, 1)
+        iter_limit_refine, method,
+        mod_func, window_start, fft_N,
+        opt_rho, opt_bkg)
 # Set-up bounds and other options according to the documentation of solver/minimisation routine
 bounds = ((0.045, 0.065),)
 op_method = 'L-BFGS-B'
 optimisation_options = {'disp': 0,
                         'maxiter': 15000,
                         'maxfun': 15000,
                         'ftol': 2.22e-12,
                         'gtol': 1e-12
                         }
-opt_result = minimize(liquid.calc_impr_interference_func, rho_0,
+opt_result = minimize(liquid.refinement_objfun, rho_0,
                       bounds=bounds, args=args,
                       options=optimisation_options,
                       method=op_method)
 # The solver finds the value of rho that gives the smallest chi^2
 rho_refined = opt_result.x[0]
 
 # The interference function can then be re-calculated using the new value for rho,
 # and the F(r) refined as above.
 interference_func = (liquid.calc_structure_factor(q_data,I_data, composition, rho_refined) - 
                      liquid.calc_S_inf(composition, q_data))
 
-args = (q_data, interference_func, composition, r_min,
-        iter_limit, method, mod_func, window_start, fft_N, 0)
-interference_func_2, chi_sq_2 = liquid.calc_impr_interference_func(rho_refined, *args)
+args = (q_data, interference_func, composition, rho_refined,
+        r_min, iter_limit, method, mod_func, window_start, fft_N)
+interference_func_2, chi_sq_2 = liquid.calc_impr_interference_func(*args)
 
 # Calculate the corresponding pair distribution functions g(r)
 r, g_r_0 = liquid.calc_correlation_func(q_data, interference_func_0, rho_0, dx=dq,
                                         mod_func=mod_func, window_start=window_start,
                                         function='pair_dist_func')
 # r values will be the same
 _, g_r_1 = liquid.calc_correlation_func(q_data, interference_func_1, rho_0, dx=dq,
@@ -538,8 +555,8 @@
 
 Licensed under the GNU General Public License (GPL), version 3 or later.
 
 See the [license file](../master/LICENSE) for more information.
 
 This program comes with absolutely no warranty or guarantee.
 
-Copyright © 2018-2021 – Benedict J Heinen
+Copyright © 2018-2022 – Benedict J Heinen
```

### Comparing `LiquidDiffract-1.1.8/setup.py` & `LiquidDiffract-1.1.9/setup.py`

 * *Files identical despite different names*

