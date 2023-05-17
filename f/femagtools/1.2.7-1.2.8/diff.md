# Comparing `tmp/femagtools-1.2.7.tar.gz` & `tmp/femagtools-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femagtools-1.2.7.tar", last modified: Thu Apr 13 07:50:58 2023, max compression
+gzip compressed data, was "femagtools-1.2.8.tar", last modified: Wed May 17 15:20:50 2023, max compression
```

## Comparing `femagtools-1.2.7.tar` & `femagtools-1.2.8.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.694537 femagtools-1.2.7/
--rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.2.7/LICENSE
--rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.2.7/MANIFEST.in
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-04-13 07:50:58.694537 femagtools-1.2.7/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.2.7/README.md
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.677537 femagtools-1.2.7/femagtools/
--rw-r--r--   0 tar        (210) tar        (210)     1630 2023-04-13 07:48:48.000000 femagtools-1.2.7/femagtools/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/airgap.py
--rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/amazon.py
--rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/amela.py
--rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    68684 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/bch.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/bchxml.py
--rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/condor.py
--rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/config.py
--rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/convert.py
--rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dakota.py
--rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dakota_femag.py
--rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dakotaout.py
--rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.2.7/femagtools/docker.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.680537 femagtools-1.2.7/femagtools/dxfsl/
--rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/area.py
--rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/conv.py
--rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/converter.py
--rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/corner.py
--rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/dumprenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/fslrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/functions.py
--rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/geom.py
--rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/machine.py
--rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/plotrenderer.py
--rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/dxfsl/shape.py
--rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/erg.py
--rw-r--r--   0 tar        (210) tar        (210)    40619 2023-04-13 07:48:25.000000 femagtools-1.2.7/femagtools/femag.py
--rw-r--r--   0 tar        (210) tar        (210)     7466 2023-02-15 20:03:56.000000 femagtools-1.2.7/femagtools/forcedens.py
--rw-r--r--   0 tar        (210) tar        (210)    28180 2023-02-21 19:53:03.000000 femagtools-1.2.7/femagtools/fsl.py
--rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/getset.py
--rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/gmsh.py
--rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/google.py
--rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/grid.py
--rw-r--r--   0 tar        (210) tar        (210)    41556 2023-04-13 07:48:25.000000 femagtools-1.2.7/femagtools/isa7.py
--rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/jcf2msh.py
--rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/jhb.py
--rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/job.py
--rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.2.7/femagtools/losscoeffs.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.681537 femagtools-1.2.7/femagtools/machine/
--rw-r--r--   0 tar        (210) tar        (210)     5613 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5604 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/machine/effloss.py
--rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/im.py
--rwxr-xr-x   0 tar        (210) tar        (210)    30631 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/machine/pm.py
--rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    14584 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/sm.py
--rw-r--r--   0 tar        (210) tar        (210)    16143 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/machine/utils.py
--rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.2.7/femagtools/magnet.py
--rw-r--r--   0 tar        (210) tar        (210)    38043 2023-02-16 09:09:33.000000 femagtools-1.2.7/femagtools/mcv.py
--rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/me.py
--rw-r--r--   0 tar        (210) tar        (210)    14106 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/model.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.682537 femagtools-1.2.7/femagtools/moo/
--rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moo/__init__.py
--rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moo/algorithm.py
--rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moo/population.py
--rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moo/problem.py
--rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/moproblem.py
--rw-r--r--   0 tar        (210) tar        (210)     8265 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/multiproc.py
--rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/mxw2msh.py
--rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/nc.py
--rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/netlist.py
--rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/ntib.py
--rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.2.7/femagtools/opt.py
--rw-r--r--   0 tar        (210) tar        (210)    18733 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/parstudy.py
--rw-r--r--   0 tar        (210) tar        (210)    57795 2023-04-05 06:37:05.000000 femagtools-1.2.7/femagtools/plot.py
--rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/poc.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.688537 femagtools-1.2.7/femagtools/templates/
--rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/FE-losses.mako
--rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/airgapinduc.mako
--rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/asyn_motor.mako
--rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/basic_modpar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/calc_field_ts.mako
--rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/cogg_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/colorgrad.mako
--rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/com_motor_sim.mako
--rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/conduct-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      437 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/connect_models.mako
--rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/cu_losses.mako
--rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/ec-rotorbar.mako
--rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/fe-contr.mako
--rw-r--r--   0 tar        (210) tar        (210)     4289 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/gen_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/inductances.mako
--rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/ld_lq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/leak_dist_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/leak_evol_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/leak_tooth_wind.mako
--rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnet-data.mako
--rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetFC2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1372 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron.mako
--rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron2.mako
--rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron4.mako
--rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIron5.mako
--rw-r--r--   0 tar        (210) tar        (210)     2208 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetIronV.mako
--rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetSector.mako
--rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetSectorLinear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetShell.mako
--rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/magnetShell2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/mesh-airgap.mako
--rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/modal_analysis.mako
--rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/mult_cal_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/new_model.mako
--rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/noloadflux-rot.mako
--rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/noloadflux.mako
--rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/noloadfluxdc.mako
--rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/open.mako
--rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/plots.mako
--rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/pm_sym_f_cur.mako
--rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/pm_sym_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/pm_sym_loss.mako
--rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/psd_psq_fast.mako
--rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/ring.mako
--rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/rot_hsm.mako
--rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/rotorAsyn.mako
--rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/rotorKs2.mako
--rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/rotor_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.2.7/femagtools/templates/rotor_winding.mako
--rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/shortcircuit.mako
--rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/srm.mako
--rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator1.mako
--rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator2.mako
--rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator3Linear.mako
--rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator4.mako
--rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/statorBG.mako
--rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/statorRing.mako
--rw-r--r--   0 tar        (210) tar        (210)     4073 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/templates/statorRotor3.mako
--rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/stator_msh.mako
--rw-r--r--   0 tar        (210) tar        (210)     1761 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/templates/torq_calc.mako
--rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.2.7/femagtools/tks.py
--rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.2.7/femagtools/ts.py
--rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/vbf.py
--rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.2.7/femagtools/vtu.py
--rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.2.7/femagtools/windings.py
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.678537 femagtools-1.2.7/femagtools.egg-info/
--rw-r--r--   0 tar        (210) tar        (210)     5262 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/PKG-INFO
--rw-r--r--   0 tar        (210) tar        (210)     4861 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/SOURCES.txt
--rw-r--r--   0 tar        (210) tar        (210)        1 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/dependency_links.txt
--rw-r--r--   0 tar        (210) tar        (210)      191 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/entry_points.txt
--rw-r--r--   0 tar        (210) tar        (210)      144 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/requires.txt
--rw-r--r--   0 tar        (210) tar        (210)       11 2023-04-13 07:50:58.000000 femagtools-1.2.7/femagtools.egg-info/top_level.txt
--rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.2.7/pyproject.toml
--rw-r--r--   0 tar        (210) tar        (210)       38 2023-04-13 07:50:58.694537 femagtools-1.2.7/setup.cfg
-drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-04-13 07:50:58.694537 femagtools-1.2.7/tests/
--rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_airgap_induction.py
--rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_amela.py
--rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_asm.py
--rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_bchreader.py
--rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_conductor.py
--rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_convert.py
--rw-r--r--   0 tar        (210) tar        (210)     1077 2023-04-05 06:37:05.000000 femagtools-1.2.7/tests/test_effloss.py
--rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_erg.py
--rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.2.7/tests/test_femag.py
--rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_forcedens.py
--rwxr-xr-x   0 tar        (210) tar        (210)    16079 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_fsl.py
--rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_im.py
--rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_isa7.py
--rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_jhb.py
--rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_job.py
--rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.2.7/tests/test_losscoeffs.py
--rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_machine.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_magncurv.py
--rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_magnet.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_mcvreader.py
--rwxr-xr-x   0 tar        (210) tar        (210)     3922 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_mcvwriter.py
--rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_me.py
--rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_model.py
--rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_nc.py
--rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_parident.py
--rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.2.7/tests/test_parstudy.py
--rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_pocfile.py
--rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.2.7/tests/test_sizing.py
--rw-r--r--   0 tar        (210) tar        (210)    83510 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_sm.py
--rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.2.7/tests/test_tksreader.py
--rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_ts.py
--rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_vbfreader.py
--rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.2.7/tests/test_vtu.py
--rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.2.7/tests/test_windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.052667 femagtools-1.2.8/
+-rw-r--r--   0 tar        (210) tar        (210)     1316 2023-02-15 20:03:56.000000 femagtools-1.2.8/LICENSE
+-rw-r--r--   0 tar        (210) tar        (210)       35 2023-02-15 20:03:56.000000 femagtools-1.2.8/MANIFEST.in
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-05-17 15:20:50.051667 femagtools-1.2.8/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     3072 2023-02-14 18:11:00.000000 femagtools-1.2.8/README.md
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.030667 femagtools-1.2.8/femagtools/
+-rw-r--r--   0 tar        (210) tar        (210)     1630 2023-05-17 15:13:04.000000 femagtools-1.2.8/femagtools/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     2250 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/airgap.py
+-rw-r--r--   0 tar        (210) tar        (210)    12122 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/amazon.py
+-rw-r--r--   0 tar        (210) tar        (210)     9741 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     7706 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    68684 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/bch.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/bchxml.py
+-rw-r--r--   0 tar        (210) tar        (210)    10766 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/condor.py
+-rw-r--r--   0 tar        (210) tar        (210)     1076 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     3087 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/config.py
+-rw-r--r--   0 tar        (210) tar        (210)    23706 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     7017 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dakota.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     4064 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dakota_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     5573 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dakotaout.py
+-rw-r--r--   0 tar        (210) tar        (210)     7460 2023-03-24 14:45:00.000000 femagtools-1.2.8/femagtools/docker.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.034667 femagtools-1.2.8/femagtools/dxfsl/
+-rw-r--r--   0 tar        (210) tar        (210)        0 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)    52503 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/area.py
+-rw-r--r--   0 tar        (210) tar        (210)     8990 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/conv.py
+-rw-r--r--   0 tar        (210) tar        (210)    18787 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/converter.py
+-rw-r--r--   0 tar        (210) tar        (210)     1266 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/corner.py
+-rw-r--r--   0 tar        (210) tar        (210)     1861 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/dumprenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    23233 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/fslrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)     9835 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/functions.py
+-rw-r--r--   0 tar        (210) tar        (210)   132506 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/geom.py
+-rw-r--r--   0 tar        (210) tar        (210)    27661 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/machine.py
+-rw-r--r--   0 tar        (210) tar        (210)    12311 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/plotrenderer.py
+-rw-r--r--   0 tar        (210) tar        (210)    43088 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/dxfsl/shape.py
+-rw-r--r--   0 tar        (210) tar        (210)     1224 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/erg.py
+-rw-r--r--   0 tar        (210) tar        (210)    40619 2023-04-13 07:48:25.000000 femagtools-1.2.8/femagtools/femag.py
+-rw-r--r--   0 tar        (210) tar        (210)     7415 2023-05-17 15:12:10.000000 femagtools-1.2.8/femagtools/forcedens.py
+-rw-r--r--   0 tar        (210) tar        (210)    28180 2023-02-21 19:53:03.000000 femagtools-1.2.8/femagtools/fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)     3017 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/getset.py
+-rw-r--r--   0 tar        (210) tar        (210)     3903 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/gmsh.py
+-rw-r--r--   0 tar        (210) tar        (210)    17166 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/google.py
+-rw-r--r--   0 tar        (210) tar        (210)     1561 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/grid.py
+-rw-r--r--   0 tar        (210) tar        (210)    41556 2023-04-13 07:48:25.000000 femagtools-1.2.8/femagtools/isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)     2790 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/jcf2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)     1779 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)    11320 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2261 2022-08-24 07:36:25.000000 femagtools-1.2.8/femagtools/losscoeffs.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.035667 femagtools-1.2.8/femagtools/machine/
+-rw-r--r--   0 tar        (210) tar        (210)     5613 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5466 2023-05-17 15:12:10.000000 femagtools-1.2.8/femagtools/machine/effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)    34847 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/im.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    30815 2023-05-17 15:12:10.000000 femagtools-1.2.8/femagtools/machine/pm.py
+-rw-r--r--   0 tar        (210) tar        (210)    21743 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    14584 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/sm.py
+-rw-r--r--   0 tar        (210) tar        (210)    16143 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/machine/utils.py
+-rw-r--r--   0 tar        (210) tar        (210)     1093 2023-02-15 20:03:56.000000 femagtools-1.2.8/femagtools/magnet.py
+-rw-r--r--   0 tar        (210) tar        (210)    38043 2023-02-16 09:09:33.000000 femagtools-1.2.8/femagtools/mcv.py
+-rw-r--r--   0 tar        (210) tar        (210)     1833 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/me.py
+-rw-r--r--   0 tar        (210) tar        (210)    14106 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/model.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.036667 femagtools-1.2.8/femagtools/moo/
+-rw-r--r--   0 tar        (210) tar        (210)      175 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moo/__init__.py
+-rw-r--r--   0 tar        (210) tar        (210)     5493 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moo/algorithm.py
+-rw-r--r--   0 tar        (210) tar        (210)    10100 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moo/population.py
+-rw-r--r--   0 tar        (210) tar        (210)     2391 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moo/problem.py
+-rw-r--r--   0 tar        (210) tar        (210)     2825 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/moproblem.py
+-rw-r--r--   0 tar        (210) tar        (210)     8265 2023-04-05 06:37:05.000000 femagtools-1.2.8/femagtools/multiproc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1841 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/mxw2msh.py
+-rw-r--r--   0 tar        (210) tar        (210)    12781 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     2052 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/netlist.py
+-rw-r--r--   0 tar        (210) tar        (210)     3099 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/ntib.py
+-rw-r--r--   0 tar        (210) tar        (210)     8685 2023-02-21 19:53:03.000000 femagtools-1.2.8/femagtools/opt.py
+-rw-r--r--   0 tar        (210) tar        (210)    18733 2023-04-05 06:37:05.000000 femagtools-1.2.8/femagtools/parstudy.py
+-rw-r--r--   0 tar        (210) tar        (210)    58040 2023-05-17 15:12:10.000000 femagtools-1.2.8/femagtools/plot.py
+-rw-r--r--   0 tar        (210) tar        (210)     6536 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/poc.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.045667 femagtools-1.2.8/femagtools/templates/
+-rw-r--r--   0 tar        (210) tar        (210)      874 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/FE-losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)      242 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/airgapinduc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2879 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/asyn_motor.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2483 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/basic_modpar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1911 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/calc_field_ts.mako
+-rw-r--r--   0 tar        (210) tar        (210)      997 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/cogg_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      400 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/colorgrad.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1264 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/com_motor_sim.mako
+-rw-r--r--   0 tar        (210) tar        (210)      472 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/conduct-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      437 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/connect_models.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1350 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/cu_losses.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1672 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/ec-rotorbar.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1983 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/fe-contr.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4289 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/gen_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)      560 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/inductances.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1270 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/ld_lq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      600 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/leak_dist_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      770 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/leak_evol_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)      431 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/leak_tooth_wind.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1271 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnet-data.mako
+-rw-r--r--   0 tar        (210) tar        (210)      788 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetFC2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1372 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1426 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2315 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1413 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron4.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1376 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIron5.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2208 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetIronV.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2010 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetSector.mako
+-rw-r--r--   0 tar        (210) tar        (210)      727 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetSectorLinear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1295 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetShell.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4080 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/magnetShell2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1094 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/mesh-airgap.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2298 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/modal_analysis.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1202 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/mult_cal_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      345 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/new_model.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3209 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/noloadflux-rot.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4661 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/noloadflux.mako
+-rw-r--r--   0 tar        (210) tar        (210)     3146 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/noloadfluxdc.mako
+-rw-r--r--   0 tar        (210) tar        (210)      313 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/open.mako
+-rw-r--r--   0 tar        (210) tar        (210)      630 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/plots.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1373 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/pm_sym_f_cur.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2319 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/pm_sym_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      925 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/pm_sym_loss.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1251 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/psd_psq_fast.mako
+-rw-r--r--   0 tar        (210) tar        (210)      643 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/ring.mako
+-rw-r--r--   0 tar        (210) tar        (210)      973 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/rot_hsm.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2280 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/rotorAsyn.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1908 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/rotorKs2.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1910 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/rotor_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)      753 2022-09-28 06:51:55.000000 femagtools-1.2.8/femagtools/templates/rotor_winding.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1981 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/shortcircuit.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2077 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/srm.mako
+-rw-r--r--   0 tar        (210) tar        (210)      761 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator1.mako
+-rw-r--r--   0 tar        (210) tar        (210)      599 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator2.mako
+-rw-r--r--   0 tar        (210) tar        (210)      724 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator3Linear.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1179 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator4.mako
+-rw-r--r--   0 tar        (210) tar        (210)      893 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/statorBG.mako
+-rw-r--r--   0 tar        (210) tar        (210)     2071 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/statorRing.mako
+-rw-r--r--   0 tar        (210) tar        (210)     4073 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/templates/statorRotor3.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1799 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/stator_msh.mako
+-rw-r--r--   0 tar        (210) tar        (210)     1761 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/templates/torq_calc.mako
+-rw-r--r--   0 tar        (210) tar        (210)     5791 2022-08-24 07:36:25.000000 femagtools-1.2.8/femagtools/tks.py
+-rw-r--r--   0 tar        (210) tar        (210)    47280 2023-02-14 18:11:00.000000 femagtools-1.2.8/femagtools/ts.py
+-rw-r--r--   0 tar        (210) tar        (210)     2444 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/vbf.py
+-rw-r--r--   0 tar        (210) tar        (210)     8595 2022-08-07 12:24:45.000000 femagtools-1.2.8/femagtools/vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)    22279 2023-03-24 14:45:00.000000 femagtools-1.2.8/femagtools/windings.py
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.031667 femagtools-1.2.8/femagtools.egg-info/
+-rw-r--r--   0 tar        (210) tar        (210)     5262 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/PKG-INFO
+-rw-r--r--   0 tar        (210) tar        (210)     4861 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/SOURCES.txt
+-rw-r--r--   0 tar        (210) tar        (210)        1 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/dependency_links.txt
+-rw-r--r--   0 tar        (210) tar        (210)      191 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/entry_points.txt
+-rw-r--r--   0 tar        (210) tar        (210)      144 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/requires.txt
+-rw-r--r--   0 tar        (210) tar        (210)       11 2023-05-17 15:20:50.000000 femagtools-1.2.8/femagtools.egg-info/top_level.txt
+-rw-r--r--   0 tar        (210) tar        (210)     1369 2023-02-15 20:03:56.000000 femagtools-1.2.8/pyproject.toml
+-rw-r--r--   0 tar        (210) tar        (210)       38 2023-05-17 15:20:50.052667 femagtools-1.2.8/setup.cfg
+drwxr-xr-x   0 tar        (210) tar        (210)        0 2023-05-17 15:20:50.051667 femagtools-1.2.8/tests/
+-rw-r--r--   0 tar        (210) tar        (210)     1065 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_airgap_induction.py
+-rw-r--r--   0 tar        (210) tar        (210)      646 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_amela.py
+-rw-r--r--   0 tar        (210) tar        (210)     1398 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_asm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    14755 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_bchreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      332 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_conductor.py
+-rw-r--r--   0 tar        (210) tar        (210)     6171 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_convert.py
+-rw-r--r--   0 tar        (210) tar        (210)     1138 2023-05-17 15:12:10.000000 femagtools-1.2.8/tests/test_effloss.py
+-rw-r--r--   0 tar        (210) tar        (210)      523 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_erg.py
+-rw-r--r--   0 tar        (210) tar        (210)     1934 2023-02-16 09:09:33.000000 femagtools-1.2.8/tests/test_femag.py
+-rw-r--r--   0 tar        (210) tar        (210)      533 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_forcedens.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    16079 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_fsl.py
+-rw-r--r--   0 tar        (210) tar        (210)      662 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_im.py
+-rw-r--r--   0 tar        (210) tar        (210)     2923 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_isa7.py
+-rw-r--r--   0 tar        (210) tar        (210)      824 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_jhb.py
+-rw-r--r--   0 tar        (210) tar        (210)      981 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_job.py
+-rw-r--r--   0 tar        (210) tar        (210)     2012 2022-08-24 07:36:25.000000 femagtools-1.2.8/tests/test_losscoeffs.py
+-rwxr-xr-x   0 tar        (210) tar        (210)    12906 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_machine.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2608 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_magncurv.py
+-rw-r--r--   0 tar        (210) tar        (210)      276 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_magnet.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2118 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_mcvreader.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     3922 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_mcvwriter.py
+-rw-r--r--   0 tar        (210) tar        (210)      192 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_me.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     2372 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_model.py
+-rw-r--r--   0 tar        (210) tar        (210)     3116 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_nc.py
+-rw-r--r--   0 tar        (210) tar        (210)     1323 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_parident.py
+-rw-r--r--   0 tar        (210) tar        (210)     3200 2023-03-02 15:44:17.000000 femagtools-1.2.8/tests/test_parstudy.py
+-rwxr-xr-x   0 tar        (210) tar        (210)     5816 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_pocfile.py
+-rw-r--r--   0 tar        (210) tar        (210)     1109 2023-02-14 18:11:00.000000 femagtools-1.2.8/tests/test_sizing.py
+-rw-r--r--   0 tar        (210) tar        (210)    83510 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_sm.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      766 2022-08-24 07:36:25.000000 femagtools-1.2.8/tests/test_tksreader.py
+-rw-r--r--   0 tar        (210) tar        (210)     1825 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_ts.py
+-rwxr-xr-x   0 tar        (210) tar        (210)      832 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_vbfreader.py
+-rw-r--r--   0 tar        (210) tar        (210)      868 2022-08-07 12:24:45.000000 femagtools-1.2.8/tests/test_vtu.py
+-rw-r--r--   0 tar        (210) tar        (210)     4912 2023-03-24 14:45:00.000000 femagtools-1.2.8/tests/test_windings.py
```

### Comparing `femagtools-1.2.7/LICENSE` & `femagtools-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/PKG-INFO` & `femagtools-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.2.7
+Version: 1.2.8
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.2.7/README.md` & `femagtools-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/__init__.py` & `femagtools-1.2.8/femagtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
     Python bindings for FEMAG
 
 
 
 """
 __title__ = 'femagtools'
-__version__ = '1.2.7'
+__version__ = '1.2.8'
 __author__ = 'Ronald Tanner'
 __license__ = 'BSD'
 __copyright__ = 'Copyright 2016-2022 SEMAFOR Informatik & Energie AG'
 
 from .asm import read
 from .bch import Reader
 from .model import MachineModel
```

### Comparing `femagtools-1.2.7/femagtools/airgap.py` & `femagtools-1.2.8/femagtools/airgap.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/amazon.py` & `femagtools-1.2.8/femagtools/amazon.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/amela.py` & `femagtools-1.2.8/femagtools/amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/asm.py` & `femagtools-1.2.8/femagtools/asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/bch.py` & `femagtools-1.2.8/femagtools/bch.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/bchxml.py` & `femagtools-1.2.8/femagtools/bchxml.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/condor.py` & `femagtools-1.2.8/femagtools/condor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/conductor.py` & `femagtools-1.2.8/femagtools/conductor.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/config.py` & `femagtools-1.2.8/femagtools/config.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/convert.py` & `femagtools-1.2.8/femagtools/convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dakota.py` & `femagtools-1.2.8/femagtools/dakota.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dakota_femag.py` & `femagtools-1.2.8/femagtools/dakota_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dakotaout.py` & `femagtools-1.2.8/femagtools/dakotaout.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/docker.py` & `femagtools-1.2.8/femagtools/docker.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/area.py` & `femagtools-1.2.8/femagtools/dxfsl/area.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/conv.py` & `femagtools-1.2.8/femagtools/dxfsl/conv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/converter.py` & `femagtools-1.2.8/femagtools/dxfsl/converter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/corner.py` & `femagtools-1.2.8/femagtools/dxfsl/corner.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/dumprenderer.py` & `femagtools-1.2.8/femagtools/dxfsl/dumprenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/fslrenderer.py` & `femagtools-1.2.8/femagtools/dxfsl/fslrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/functions.py` & `femagtools-1.2.8/femagtools/dxfsl/functions.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/geom.py` & `femagtools-1.2.8/femagtools/dxfsl/geom.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/machine.py` & `femagtools-1.2.8/femagtools/dxfsl/machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/plotrenderer.py` & `femagtools-1.2.8/femagtools/dxfsl/plotrenderer.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/dxfsl/shape.py` & `femagtools-1.2.8/femagtools/dxfsl/shape.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/erg.py` & `femagtools-1.2.8/femagtools/erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/femag.py` & `femagtools-1.2.8/femagtools/femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/forcedens.py` & `femagtools-1.2.8/femagtools/forcedens.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,45 +60,45 @@
 
     def __read_version(self, content):
         rec = content[0].split(' ')
         if len(rec) > 3:
             self.version = rec[3]
         else:
             self.version = rec[-1]
-            
+
     def __read_project_filename(self, content):
         self.project = content[1].strip()
-        
+
     def __read_nodes_and_mesh(self, content):
         self.nodes, self.elements, self.quality = \
             [float(r[0]) for r in [num_pat.findall(l)
                                    for l in content[:3]]]
         for l in content[3:]:
             m = re.match(r'\*+([^\*]+)\*+', l)
             if m:
                 self.type = m.group(1).strip()
                 return
-            
+
     def __read_date_and_title(self, content):
         d = content[0].split(':')[1].strip().split()
         dd, MM, yy = d[0].split('.')
         hh, mm = ''.join(d[1:-1]).split('.')
         self.date = '{}-{}-{}T{:02}:{:02}'.format(
             yy, MM, dd, int(hh), int(mm))
 
         if len(content) > 6:
             self.title = content[2].strip() + ', ' + content[6].strip()
         else:
             self.title = content[2].strip()
-            
+
         self.current = float(num_pat.findall(content[4])[0])
-        
+
     def __read_filename(self, content):
         self.filename = content[0].split(':')[1].strip()
-        
+
     def __read_position(self, content):
         d = dict(position=float(num_pat.findall(content[0])[-1]),
                  unit=unit_pat.findall(content[0].split()[1])[0])
         cols = content[2].split()
         labels = cols[::2] # either X, FN, FT, B_N, B_T
                            # or X FX FY B_X B_Y
         d['column_units'] = {k: u for k, u in zip(labels,
@@ -113,57 +113,57 @@
 
         self.positions.append(d)
 
     def read(self, filename):
         with open(filename) as f:
             for s in _readSections(f.readlines()):
                 logger.debug('Section %s' % s[0:2])
-                if s[0].startswith('FEMAG'):
+                if s[0].lower().startswith('femag'):
                     self.__read_version(s)
                 elif s[0].startswith('Project'):
                     self.__read_project_filename(s)
                 elif s[0].startswith('Number'):
                     self.__read_nodes_and_mesh(s)
                 elif s[0].startswith('File'):
                     self.__read_filename(s)
                 elif s[0].startswith('Date'):
                     self.__read_date_and_title(s)
                 elif s[0].startswith('POSITION'):
                     self.__read_position(s)
 
-    def _prepare(self): 
+    def _prepare(self):
         """return FN and FT Matrix"""
         ntiles = int(360/self.positions[0]['X'][-1])
         try:
             FN = np.tile(
                 np.array([p['FN'][:-1] for p in self.positions[:-1]]).T,
                 (ntiles, 1))
             FT = np.tile(
                 np.array([p['FT'][:-1] for p in self.positions[:-1]]).T,
                 (ntiles, 1))
         except AttributeError:
             return []
         return [FN, FT]
-    
+
     def fft(self):
         """return 2D FFT of the Force Density"""
         fdens = self._prepare()
-        FN, FT= fdens[0], fdens[1] 
+        FN, FT= fdens[0], fdens[1]
         N = FN.size
         dim = FN.shape[0]//2
         # Dimension [Position °] X [Time Steps s]
         FN_MAG = np.fft.fft2(FN)[0:dim, :]/N
         FT_MAG = np.fft.fft2(FT)[0:dim, :]/N
 
-        return dict(fn_harm=dict(amplitude=np.abs(FN_MAG), 
-                                phase=np.angle(FN_MAG)), 
-                    ft_harm=dict(amplitude=np.abs(FT_MAG), 
-                                phase=np.angle(FT_MAG)) 
+        return dict(fn_harm=dict(amplitude=np.abs(FN_MAG),
+                                phase=np.angle(FN_MAG)),
+                    ft_harm=dict(amplitude=np.abs(FT_MAG),
+                                phase=np.angle(FT_MAG))
                     )
-    
+
     def items(self):
         return [(k, getattr(self, k)) for k in ('version',
                                                 'type',
                                                 'title',
                                                 'current',
                                                 'filename',
                                                 'date',
@@ -217,20 +217,20 @@
         filename = sys.argv[1]
     else:
         filename = sys.stdin.readline().strip()
 
     fdens = read(filename)
 
     # Show the results
+    print(fdens.version)
 
     title = '{}, Rotor position {}'.format(
         fdens.title, fdens.positions[0]['position'])
     pos = fdens.positions[0]['X']
     FT_FN = (fdens.positions[0]['FT'],
              fdens.positions[0]['FN'])
-    femagtools.plot.forcedens(title, pos, FT_FN)    
+    femagtools.plot.forcedens(title, pos, FT_FN)
     pl.show()
 
     title = 'Force Density Harmonics'
     femagtools.plot.forcedens_fft(title, fdens)
     pl.show()
-
```

### Comparing `femagtools-1.2.7/femagtools/fsl.py` & `femagtools-1.2.8/femagtools/fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/getset.py` & `femagtools-1.2.8/femagtools/getset.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/gmsh.py` & `femagtools-1.2.8/femagtools/gmsh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/google.py` & `femagtools-1.2.8/femagtools/google.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/grid.py` & `femagtools-1.2.8/femagtools/grid.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/isa7.py` & `femagtools-1.2.8/femagtools/isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/jcf2msh.py` & `femagtools-1.2.8/femagtools/jcf2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/jhb.py` & `femagtools-1.2.8/femagtools/jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/job.py` & `femagtools-1.2.8/femagtools/job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/losscoeffs.py` & `femagtools-1.2.8/femagtools/losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/machine/__init__.py` & `femagtools-1.2.8/femagtools/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/machine/effloss.py` & `femagtools-1.2.8/femagtools/machine/effloss.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import scipy.interpolate as ip
 import logging
 from .utils import betai1
-from .pm import PmRelMachineLdq
+from .pm import PmRelMachineLdq, PmRelMachinePsidq, PmRelMachine
 from . import create_from_eecpars
 
 logger = logging.getLogger("femagtools.effloss")
 
 
 def _generate_mesh(n, T, nb, Tb, npoints):
     """return speed and torque list for driving/braking speed range
@@ -32,28 +32,23 @@
     else:
         def tbip(x): return 0
 
     nxtx = []
     for nx in np.linspace(1, nmax, npoints[0]):
         t0 = tbip(nx)
         t1 = tip(nx)
-        try:
-            npnts = round((t1-t0) / (tmax-tmin) * npoints[1])
-            if npnts > 2:
-                for t in np.concatenate(
-                        (np.linspace(t0, 0.015*tmin, tnum),
-                         np.linspace(0.015*tmax, t1, tnum))):
-                    nxtx.append((nx, t))
-        except ValueError as ex:
-            logger.warning("n, t0, t1 %s tmin, tmax %s, npoints %d",
-                           (n, t0, t1), (tmin, tmax), npoints[1])
+        npnts = max(round((t1-t0) / (tmax-tmin) * tnum), 2)
+        for t in np.concatenate(
+                (np.linspace(t0, 0.015*tmin, npnts),
+                 np.linspace(0.015*tmax, t1, npnts))):
+            nxtx.append((nx, t))
     return np.array(nxtx).T
 
 
-def efficiency_losses_map(eecpars, u1, T, temp, n, npoints=(50, 40)):
+def efficiency_losses_map(eecpars, u1, T, temp, n, npoints=(60, 40)):
     """return speed, torque efficiency and losses
 
     arguments:
     eecpars: (dict) EEC Parameter with
       dicts at different temperatures (or machine object)
     u1: (float) phase voltage (V rms)
     T: (float) starting torque (Nm)
@@ -69,31 +64,32 @@
             xtemp = [temp, temp]
         m = create_from_eecpars(xtemp, eecpars)
     else:  # must be an instance of Machine
         m = eecpars
     if isinstance(T, list):
         r = {'T': T, 'n': n}
         rb = {'T': [], 'n': []}
-    else: # calculate speed,torque charactersics
+    else:  # calculate speed,torque charactersics
         nmax = n
+        rb = {}
         r = m.characteristics(T, nmax, u1)  # driving mode
         if isinstance(m, PmRelMachineLdq):
             if min(m.betarange) >= -np.pi/2:  # driving mode only
-                rb = {}
                 rb['n'] = None
                 rb['T'] = None
-            else:
-                rb = m.characteristics(-T, max(r['n']), u1)  # braking mode
-        else:
+        if isinstance(m, PmRelMachinePsidq):
+            if min(m.iqrange) >= 0:  # driving mode only
+                rb['n'] = None
+                rb['T'] = None
+        if 'n' not in rb:
             rb = m.characteristics(-T, max(r['n']), u1)  # braking mode
-
     ntmesh = _generate_mesh(r['n'], r['T'],
                             rb['n'], rb['T'], npoints)
 
-    if isinstance(m, PmRelMachineLdq):
+    if isinstance(m, PmRelMachine):
         iqd = np.array([
             m.iqd_torque_umax(
                 nt[1],
                 2*np.pi*nt[0]*m.p,
                 u1)[:-1]
             for nt in ntmesh.T]).T
         beta, i1 = betai1(iqd[0], iqd[1])
@@ -115,15 +111,15 @@
             r['i1'].append(np.abs(i1))
             r['plfe1'].append(m.m*np.abs(u1)**2/m.rfe(w1, m.psi))
             i2 = m.i2(w1, m.psi, wm)
             r['plcu1'].append(m.m*np.abs(i1)**2*m.rstat(w1))
             r['plcu2'].append(m.m*np.abs(i2)**2*m.rrot(w1-m.p*wm))
 
 
-    if isinstance(m, PmRelMachineLdq):
+    if isinstance(m, PmRelMachine):
         plfe1 = m.iqd_plfe1(*iqd, f1)
         plfe2 = m.iqd_plfe2(iqd[0], iqd[1], f1)
         plmag = m.iqd_plmag(iqd[0], iqd[1], f1)
         plcu1 = m.iqd_plcu1(iqd[0], iqd[1], 2*np.pi*f1)
         plcu2 = m.iqd_plcu2(*iqd)
         try:
             tfric = eecpars['kfric_b']*eecpars['rotor_mass']*30e-3/np.pi
```

### Comparing `femagtools-1.2.7/femagtools/machine/im.py` & `femagtools-1.2.8/femagtools/machine/im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/machine/pm.py` & `femagtools-1.2.8/femagtools/machine/pm.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,17 @@
     def w1_umax(self, u, iq, id):
         """return frequency w1 at given voltage u and id, iq current
 
         Keyword arguments:
         u -- the maximum voltage (RMS)
         iq, id -- the d-q currents"""
         w10 = np.sqrt(2)*u/la.norm(self.psi(iq, id))
-        return so.fsolve(lambda w1:
-                         la.norm(self.uqd(w1, iq, id))-u*np.sqrt(2), w10)[0]
+        return so.fsolve(
+            lambda w1: la.norm(self.uqd(w1, iq, id))-u*np.sqrt(2),
+            w10)[0]
 
     def w1_u(self, u, iq, id):
         """return frequency w1 at given voltage u and id, iq current
         (obsolete, use w1_umax)"""
         return self.w1_umax(u, iq, id)
 
     def w1max(self, u, iq, id):
@@ -212,15 +213,16 @@
     def iqd_imax_umax(self, i1max, w1, u1max, maxtorque=True):
         """return d-q current at stator frequency and max voltage
         and max current (for motor operation if maxtorque else generator operation)"""
 
         if maxtorque:
             btab = np.linspace(max(-np.pi/2, self.betarange[0]), 0)
         else:
-            btab = np.linspace(max(-np.pi, self.betarange[0]), -np.pi/2)
+            btab = np.linspace(min(-np.pi/2, self.betarange[1]),
+                               self.betarange[0])
         u1b = [np.linalg.norm(self.uqd(w1, *iqd(b, i1max)))
                for b in btab]
         if np.max(u1b) > np.sqrt(2)*u1max:
             beta0=btab[0]
             for bx, ux in zip(btab, u1b):
                 if ux/np.sqrt(2)>u1max:
                     break
@@ -313,17 +315,19 @@
         """
         r = dict(id=[], iq=[], uq=[], ud=[], u1=[], i1=[], T=[],
                  beta=[], gamma=[], phi=[], cosphi=[], pmech=[], n=[])
         if np.isscalar(T):
             iq, id = self.iqd_torque(T)
             i1max = betai1(iq, id)[1]
             w1 = self.w1_umax(u1max, iq, id)
-            w1max = self.w1_umax(u1max, *self.iqdmin(i1max))
+            iqmin, idmin = self.iqdmin(i1max)
+            if (iqmin < 0):
+                iqmin = 0
+            w1max = self.w1_umax(u1max, iqmin, idmin)
             nmax = max(w1, w1max)/2/np.pi/self.p
-
             n1 = min(w1/2/np.pi/self.p, nmax)
             r['n_type'] = n1
             logger.info("Type speed %f n: %f nmax %f",
                         60*n1, 60*n, 60*nmax)
             try:
                 w1 = self.w2_imax_umax(i1max, u1max, maxtorque=(T > 0))
                 n2 = w1/2/np.pi/self.p
@@ -343,15 +347,16 @@
                     n2 = nmax
             if n > 0:
                 nmax = min(nmax, n)
                 speedrange = sorted(
                     list(set([nx for nx in [n1, n2, n] if nx < 1.01*nmax])))
             else:
                 speedrange = sorted(list(set([n1, n2])))
-            logger.info("speedrange %s", speedrange)
+            logger.info("speedrange %s (T = %s Nm)",
+                        speedrange, T)
             speedrange.insert(0, 0)
             n3 = speedrange[-1]
             nstab = [int(nsamples*(x1-x2)/n3)
                      for x1, x2 in zip(speedrange[1:],
                                        speedrange)]
             for nx in np.linspace(0, n1, nstab[0]):
                 r['id'].append(id)
@@ -360,31 +365,31 @@
                 r['T'].append(T)
 
             n1 = speedrange[1]
             try:
                 n2 = speedrange[2]
             except IndexError:
                 n2 = n1
-            if n1 < n2: # find id, iq, torque in fieldweakening range
+            if n1 < n2:  # find id, iq, torque in fieldweakening range
                 dn = r['n'][-1] - r['n'][-2]
                 for nn in np.linspace(r['n'][-1]+dn, n2, nstab[1]):
                     w1 = 2*np.pi*nn*self.p
                     logger.debug("fieldweakening: n %g T %g i1max %g w1 %g u1 %g",
                                  nn*60, T, i1max, w1, u1max)
                     iq, id = self.iqd_imax_umax(i1max, w1, u1max,
                                                 maxtorque=T > 0)
                     tq = self.torque_iqd(iq, id)
                     if (T > 0 and tq > 0) or (T < 0 and tq < 0):
                         r['id'].append(id)
                         r['iq'].append(iq)
                         r['n'].append(nn)
                         r['T'].append(tq)
                     else:
-                        logger.warning("fieldweakening: n %g T %g i1max %g w1 %g u1 %g",
-                                       nn*60, T, i1max, w1, u1max)
+                        logger.warning("fieldweakening: n %g T %g tq %g i1max %g w1 %g u1 %g",
+                                       nn*60, T, tq, i1max, w1, u1max)
 
             if n2 < n3:
                 for nn in np.linspace(r['n'][-1]+dn/2, n3, nstab[2]):
                     w1 = 2*np.pi*nn*self.p
                     try:
                         iq, id, tq = self.mtpv(
                             w1, u1max, i1max, maxtorque=T > 0)
```

### Comparing `femagtools-1.2.7/femagtools/machine/sizing.py` & `femagtools-1.2.8/femagtools/machine/sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/machine/sm.py` & `femagtools-1.2.8/femagtools/machine/sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/machine/utils.py` & `femagtools-1.2.8/femagtools/machine/utils.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/magnet.py` & `femagtools-1.2.8/femagtools/magnet.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/mcv.py` & `femagtools-1.2.8/femagtools/mcv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/me.py` & `femagtools-1.2.8/femagtools/me.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/model.py` & `femagtools-1.2.8/femagtools/model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/moo/algorithm.py` & `femagtools-1.2.8/femagtools/moo/algorithm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/moo/population.py` & `femagtools-1.2.8/femagtools/moo/population.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/moo/problem.py` & `femagtools-1.2.8/femagtools/moo/problem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/moproblem.py` & `femagtools-1.2.8/femagtools/moproblem.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/multiproc.py` & `femagtools-1.2.8/femagtools/multiproc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/mxw2msh.py` & `femagtools-1.2.8/femagtools/mxw2msh.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/nc.py` & `femagtools-1.2.8/femagtools/nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/netlist.py` & `femagtools-1.2.8/femagtools/netlist.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/ntib.py` & `femagtools-1.2.8/femagtools/ntib.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/opt.py` & `femagtools-1.2.8/femagtools/opt.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/parstudy.py` & `femagtools-1.2.8/femagtools/parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/plot.py` & `femagtools-1.2.8/femagtools/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1721,58 +1721,64 @@
             bnd[0].append((nx, tx))
             n0 = nx
         t0 = tx
     bnd[1].append((nx, tx))
     return np.array(bnd[0] + bnd[1][::-1])
 
 
-def plot_contour(speed, torque, z, ax, title='', levels=[]):
+def plot_contour(speed, torque, z, ax, title='', levels=[], clabel=True):
     from matplotlib.path import Path
     from matplotlib.patches import PathPatch
     x = [60*n for n in speed]
     y = torque
     if not levels:
         if max(z) <= 1:
             levels = [0.25, 0.5, 0.75, 0.8, 0.84,
                       0.88, 0.9, 0.92, 0.94, 0.96]
             if max(z) > levels[-1]:
                 levels.append(np.ceil(max(z)*100)/100)
         else:
             levels = 14
     cont = ax.tricontour(x, y, z,
                          linewidths=0.4, levels=levels, colors='k')
-    ax.clabel(cont, inline=True, colors='k')
+    if clabel:
+        ax.clabel(cont, inline=True, colors='k', fontsize=8)
     contf = ax.tricontourf(x, y, z,
                            levels=levels, cmap='YlOrRd')
     #
+    ax.spines['top'].set_color('none')
+    ax.spines['right'].set_color('none')
+
     clippath = Path(get_nT_boundary(x, y))
     patch = PathPatch(clippath, facecolor='none')
     ax.add_patch(patch)
     for c in cont.collections:
         c.set_clip_path(patch)
     for c in contf.collections:
         c.set_clip_path(patch)
     #ax.plot(x, y, "k.", ms=3)
     ax.set_ylabel('Torque / Nm')
     ax.set_xlabel('Speed / rpm')
     ax.set_title(title)
+    return contf
 
-
-def efficiency_map(rmap, ax=0, title='Efficiency Map'):
+def efficiency_map(rmap, ax=0, title='Efficiency Map', clabel=True):
     if ax == 0:
         fig, ax = plt.subplots(figsize=(12, 12))
-    plot_contour(rmap['n'], rmap['T'], rmap['eta'], ax,
-                 title=title)
+    contf = plot_contour(rmap['n'], rmap['T'], rmap['eta'], ax,
+                         title=title, clabel=clabel)
+    return contf
 
 
-def losses_map(rmap, ax=0, title='Losses Map / kW'):
+def losses_map(rmap, ax=0, title='Losses Map / kW', clabel=True):
     if ax == 0:
         fig, ax = plt.subplots(figsize=(12, 12))
-    plot_contour(rmap['n'], rmap['T'], np.asarray(rmap['losses'])/1e3, ax,
-                 title=title, levels=14)
+    return plot_contour(rmap['n'], rmap['T'], np.asarray(rmap['losses'])/1e3, ax,
+                        title=title, levels=14, clabel=clabel)
+
 
 def eigenmode(reigen, num_modes=12):
     """plot eigenmode"""
     cols = 4
     rows = int((num_modes - num_modes%cols)/cols + 1)
     fig, ax = plt.subplots(rows, cols)
     ctr = 0
```

### Comparing `femagtools-1.2.7/femagtools/poc.py` & `femagtools-1.2.8/femagtools/poc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/FE-losses.mako` & `femagtools-1.2.8/femagtools/templates/FE-losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/asyn_motor.mako` & `femagtools-1.2.8/femagtools/templates/asyn_motor.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/basic_modpar.mako` & `femagtools-1.2.8/femagtools/templates/basic_modpar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/calc_field_ts.mako` & `femagtools-1.2.8/femagtools/templates/calc_field_ts.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/cogg_calc.mako` & `femagtools-1.2.8/femagtools/templates/cogg_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/com_motor_sim.mako` & `femagtools-1.2.8/femagtools/templates/com_motor_sim.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/cu_losses.mako` & `femagtools-1.2.8/femagtools/templates/cu_losses.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/ec-rotorbar.mako` & `femagtools-1.2.8/femagtools/templates/ec-rotorbar.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/fe-contr.mako` & `femagtools-1.2.8/femagtools/templates/fe-contr.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/gen_winding.mako` & `femagtools-1.2.8/femagtools/templates/gen_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/inductances.mako` & `femagtools-1.2.8/femagtools/templates/inductances.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/ld_lq_fast.mako` & `femagtools-1.2.8/femagtools/templates/ld_lq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/leak_dist_wind.mako` & `femagtools-1.2.8/femagtools/templates/leak_dist_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/leak_evol_wind.mako` & `femagtools-1.2.8/femagtools/templates/leak_evol_wind.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnet-data.mako` & `femagtools-1.2.8/femagtools/templates/magnet-data.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetFC2.mako` & `femagtools-1.2.8/femagtools/templates/magnetFC2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetIron.mako` & `femagtools-1.2.8/femagtools/templates/magnetIron.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetIron2.mako` & `femagtools-1.2.8/femagtools/templates/magnetIron2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetIron3.mako` & `femagtools-1.2.8/femagtools/templates/magnetIron3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetIron4.mako` & `femagtools-1.2.8/femagtools/templates/magnetIron4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetIron5.mako` & `femagtools-1.2.8/femagtools/templates/magnetIron5.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetIronV.mako` & `femagtools-1.2.8/femagtools/templates/magnetIronV.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetSector.mako` & `femagtools-1.2.8/femagtools/templates/magnetSector.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetSectorLinear.mako` & `femagtools-1.2.8/femagtools/templates/magnetSectorLinear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetShell.mako` & `femagtools-1.2.8/femagtools/templates/magnetShell.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/magnetShell2.mako` & `femagtools-1.2.8/femagtools/templates/magnetShell2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/mesh-airgap.mako` & `femagtools-1.2.8/femagtools/templates/mesh-airgap.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/modal_analysis.mako` & `femagtools-1.2.8/femagtools/templates/modal_analysis.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/mult_cal_fast.mako` & `femagtools-1.2.8/femagtools/templates/mult_cal_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/noloadflux-rot.mako` & `femagtools-1.2.8/femagtools/templates/noloadflux-rot.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/noloadflux.mako` & `femagtools-1.2.8/femagtools/templates/noloadflux.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/noloadfluxdc.mako` & `femagtools-1.2.8/femagtools/templates/noloadfluxdc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/plots.mako` & `femagtools-1.2.8/femagtools/templates/plots.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/pm_sym_f_cur.mako` & `femagtools-1.2.8/femagtools/templates/pm_sym_f_cur.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/pm_sym_fast.mako` & `femagtools-1.2.8/femagtools/templates/pm_sym_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/pm_sym_loss.mako` & `femagtools-1.2.8/femagtools/templates/pm_sym_loss.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/psd_psq_fast.mako` & `femagtools-1.2.8/femagtools/templates/psd_psq_fast.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/ring.mako` & `femagtools-1.2.8/femagtools/templates/ring.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/rot_hsm.mako` & `femagtools-1.2.8/femagtools/templates/rot_hsm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/rotorAsyn.mako` & `femagtools-1.2.8/femagtools/templates/rotorAsyn.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/rotorKs2.mako` & `femagtools-1.2.8/femagtools/templates/rotorKs2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/rotor_msh.mako` & `femagtools-1.2.8/femagtools/templates/rotor_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/rotor_winding.mako` & `femagtools-1.2.8/femagtools/templates/rotor_winding.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/shortcircuit.mako` & `femagtools-1.2.8/femagtools/templates/shortcircuit.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/srm.mako` & `femagtools-1.2.8/femagtools/templates/srm.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/stator1.mako` & `femagtools-1.2.8/femagtools/templates/stator1.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/stator2.mako` & `femagtools-1.2.8/femagtools/templates/stator2.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/stator3Linear.mako` & `femagtools-1.2.8/femagtools/templates/stator3Linear.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/stator4.mako` & `femagtools-1.2.8/femagtools/templates/stator4.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/statorBG.mako` & `femagtools-1.2.8/femagtools/templates/statorBG.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/statorRing.mako` & `femagtools-1.2.8/femagtools/templates/statorRing.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/statorRotor3.mako` & `femagtools-1.2.8/femagtools/templates/statorRotor3.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/stator_msh.mako` & `femagtools-1.2.8/femagtools/templates/stator_msh.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/templates/torq_calc.mako` & `femagtools-1.2.8/femagtools/templates/torq_calc.mako`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/tks.py` & `femagtools-1.2.8/femagtools/tks.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/ts.py` & `femagtools-1.2.8/femagtools/ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/vbf.py` & `femagtools-1.2.8/femagtools/vbf.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/vtu.py` & `femagtools-1.2.8/femagtools/vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools/windings.py` & `femagtools-1.2.8/femagtools/windings.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/femagtools.egg-info/PKG-INFO` & `femagtools-1.2.8/femagtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femagtools
-Version: 1.2.7
+Version: 1.2.8
 Summary: Python API for FEMAG
 Author-email: Ronald Tanner <tar@semafor.ch>, Dapu Zhang <d.zhan@gtisoft.com>, Beat Holm <hob@semafor.ch>, Günther Amsler <amg@semafor.ch>, Nicolas Mauchle <mau@semafor.ch>
 License: Copyright (c) 2016-2023, Semafor Informatik & Energie AG, Basel
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
```

### Comparing `femagtools-1.2.7/femagtools.egg-info/SOURCES.txt` & `femagtools-1.2.8/femagtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/pyproject.toml` & `femagtools-1.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_airgap_induction.py` & `femagtools-1.2.8/tests/test_airgap_induction.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_amela.py` & `femagtools-1.2.8/tests/test_amela.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_asm.py` & `femagtools-1.2.8/tests/test_asm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_bchreader.py` & `femagtools-1.2.8/tests/test_bchreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_convert.py` & `femagtools-1.2.8/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_effloss.py` & `femagtools-1.2.8/tests/test_effloss.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,12 +20,14 @@
 def test_imeffloss(impars):
     nmax = 8000/60
     T = 32.9
     u1 = 230
     temp = (120, 120)
 
     r = femagtools.machine.effloss.efficiency_losses_map(
-        impars, u1, T, temp, nmax, npoints=(10, 4))
+        impars, u1, T, temp, nmax, npoints=(5, 4))
     assert r['T'] == pytest.approx(
-        [-33., -0.5, 0.4, 32.7,
-         -33., -0.5, 0.4, 32.7,
-         -28.2, -0.5, 0.4, 26], abs=1e-1)
+        [-33, -0.5, 0.5, 32.8,
+         -25, -0.5, 0.5, 23.2,
+         -12.8, -0.5, 0.5, 11.7,
+         -8.6, -0.5, 0.5, 7.8,
+         -6.5, -0.5, 0.5, 5.8], abs=1e-1)
```

### Comparing `femagtools-1.2.7/tests/test_erg.py` & `femagtools-1.2.8/tests/test_erg.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_femag.py` & `femagtools-1.2.8/tests/test_femag.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_forcedens.py` & `femagtools-1.2.8/tests/test_forcedens.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_fsl.py` & `femagtools-1.2.8/tests/test_fsl.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_im.py` & `femagtools-1.2.8/tests/test_im.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_isa7.py` & `femagtools-1.2.8/tests/test_isa7.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_jhb.py` & `femagtools-1.2.8/tests/test_jhb.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_job.py` & `femagtools-1.2.8/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_losscoeffs.py` & `femagtools-1.2.8/tests/test_losscoeffs.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_machine.py` & `femagtools-1.2.8/tests/test_machine.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_magncurv.py` & `femagtools-1.2.8/tests/test_magncurv.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_mcvreader.py` & `femagtools-1.2.8/tests/test_mcvreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_mcvwriter.py` & `femagtools-1.2.8/tests/test_mcvwriter.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_model.py` & `femagtools-1.2.8/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_nc.py` & `femagtools-1.2.8/tests/test_nc.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_parident.py` & `femagtools-1.2.8/tests/test_parident.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_parstudy.py` & `femagtools-1.2.8/tests/test_parstudy.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_pocfile.py` & `femagtools-1.2.8/tests/test_pocfile.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_sizing.py` & `femagtools-1.2.8/tests/test_sizing.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_sm.py` & `femagtools-1.2.8/tests/test_sm.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_tksreader.py` & `femagtools-1.2.8/tests/test_tksreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_ts.py` & `femagtools-1.2.8/tests/test_ts.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_vbfreader.py` & `femagtools-1.2.8/tests/test_vbfreader.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_vtu.py` & `femagtools-1.2.8/tests/test_vtu.py`

 * *Files identical despite different names*

### Comparing `femagtools-1.2.7/tests/test_windings.py` & `femagtools-1.2.8/tests/test_windings.py`

 * *Files identical despite different names*

