# Comparing `tmp/edalize-0.5.0.tar.gz` & `tmp/edalize-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edalize-0.5.0.tar", last modified: Fri Mar 24 22:07:08 2023, max compression
+gzip compressed data, was "edalize-0.5.1.tar", last modified: Wed May 17 08:31:29 2023, max compression
```

## Comparing `edalize-0.5.0.tar` & `edalize-0.5.1.tar`

### file list

```diff
@@ -1,740 +1,747 @@
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.821589 edalize-0.5.0/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.638592 edalize-0.5.0/.github/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.658592 edalize-0.5.0/.github/workflows/
--rw-r--r--   0 olof      (1000) olof      (1000)     1425 2023-03-06 16:31:40.000000 edalize-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 olof      (1000) olof      (1000)      116 2023-02-28 12:38:03.000000 edalize-0.5.0/.gitignore
--rw-r--r--   0 olof      (1000) olof      (1000)      234 2022-06-11 20:28:55.000000 edalize-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 olof      (1000) olof      (1000)      271 2020-11-17 21:53:11.000000 edalize-0.5.0/.readthedocs.yml
--rw-r--r--   0 olof      (1000) olof      (1000)     1349 2021-03-28 21:01:38.000000 edalize-0.5.0/LICENSE
--rw-r--r--   0 olof      (1000) olof      (1000)     1590 2023-03-24 22:06:41.000000 edalize-0.5.0/NEWS
--rw-r--r--   0 olof      (1000) olof      (1000)     7697 2023-03-24 22:07:08.821589 edalize-0.5.0/PKG-INFO
--rw-r--r--   0 olof      (1000) olof      (1000)     7033 2023-03-06 16:31:40.000000 edalize-0.5.0/README.rst
--rw-r--r--   0 olof      (1000) olof      (1000)       22 2021-11-14 22:20:16.000000 edalize-0.5.0/dev-requirements.txt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.661592 edalize-0.5.0/doc/
--rw-r--r--   0 olof      (1000) olof      (1000)      581 2019-01-17 08:09:28.000000 edalize-0.5.0/doc/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)     6344 2021-12-20 23:32:01.000000 edalize-0.5.0/doc/conf.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.662592 edalize-0.5.0/doc/dev/
--rw-r--r--   0 olof      (1000) olof      (1000)    11320 2023-03-06 16:31:40.000000 edalize-0.5.0/doc/dev/extend.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      360 2023-03-06 16:31:40.000000 edalize-0.5.0/doc/dev/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1832 2021-12-20 23:33:36.000000 edalize-0.5.0/doc/dev/setup.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      106 2021-12-20 23:33:36.000000 edalize-0.5.0/doc/dev/tests.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     3529 2023-02-23 16:54:50.000000 edalize-0.5.0/doc/edalize.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.663592 edalize-0.5.0/doc/edam/
--rw-r--r--   0 olof      (1000) olof      (1000)    19643 2022-07-06 15:41:17.000000 edalize-0.5.0/doc/edam/api.rst
--rw-r--r--   0 olof      (1000) olof      (1000)       66 2021-12-20 23:33:36.000000 edalize-0.5.0/doc/genindex.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     2206 2023-03-06 16:31:40.000000 edalize-0.5.0/doc/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      787 2019-01-17 07:54:32.000000 edalize-0.5.0/doc/make.bat
--rw-r--r--   0 olof      (1000) olof      (1000)       78 2021-12-20 23:33:36.000000 edalize-0.5.0/doc/py-modindex.rst
--rw-r--r--   0 olof      (1000) olof      (1000)       64 2020-11-17 21:53:11.000000 edalize-0.5.0/doc/requirements.txt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.664592 edalize-0.5.0/doc/user/
--rw-r--r--   0 olof      (1000) olof      (1000)       52 2023-03-06 16:31:40.000000 edalize-0.5.0/doc/user/build.rst
--rw-r--r--   0 olof      (1000) olof      (1000)       64 2023-03-06 16:31:40.000000 edalize-0.5.0/doc/user/configure.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      416 2023-03-06 16:31:40.000000 edalize-0.5.0/doc/user/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)       46 2023-03-06 16:31:40.000000 edalize-0.5.0/doc/user/run.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.675592 edalize-0.5.0/edalize/
--rw-r--r--   0 olof      (1000) olof      (1000)     2653 2021-12-20 23:33:36.000000 edalize-0.5.0/edalize/apicula.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1864 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/ascentlint.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4940 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/diamond.py
--rw-r--r--   0 olof      (1000) olof      (1000)    18486 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/edatool.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2180 2023-02-28 12:25:40.000000 edalize-0.5.0/edalize/f4pga.py
--rw-r--r--   0 olof      (1000) olof      (1000)     7214 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/filelist.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.678592 edalize-0.5.0/edalize/flows/
--rw-r--r--   0 olof      (1000) olof      (1000)    12358 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/flows/edaflow.py
--rw-r--r--   0 olof      (1000) olof      (1000)     8251 2023-02-28 12:38:03.000000 edalize-0.5.0/edalize/flows/f4pga.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1919 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/flows/generic.py
--rw-r--r--   0 olof      (1000) olof      (1000)     3566 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/flows/gls.py
--rw-r--r--   0 olof      (1000) olof      (1000)     3033 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/flows/icestorm.py
--rw-r--r--   0 olof      (1000) olof      (1000)      464 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/flows/lint.py
--rw-r--r--   0 olof      (1000) olof      (1000)      545 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/flows/sim.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1935 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/flows/vivado.py
--rw-r--r--   0 olof      (1000) olof      (1000)      944 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/flows/vpr.py
--rw-r--r--   0 olof      (1000) olof      (1000)     3476 2022-07-06 15:41:17.000000 edalize-0.5.0/edalize/gatemate.py
--rw-r--r--   0 olof      (1000) olof      (1000)     6680 2021-12-20 23:33:36.000000 edalize-0.5.0/edalize/ghdl.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5418 2023-02-28 12:38:03.000000 edalize-0.5.0/edalize/icarus.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2133 2022-07-09 21:04:13.000000 edalize-0.5.0/edalize/icestorm.py
--rw-r--r--   0 olof      (1000) olof      (1000)     6959 2023-02-28 12:38:03.000000 edalize-0.5.0/edalize/ise.py
--rw-r--r--   0 olof      (1000) olof      (1000)    10673 2021-11-14 22:19:47.000000 edalize-0.5.0/edalize/ise_reporting.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5573 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/isim.py
--rw-r--r--   0 olof      (1000) olof      (1000)     7727 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/libero.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2343 2022-05-31 20:24:45.000000 edalize-0.5.0/edalize/mistral.py
--rw-r--r--   0 olof      (1000) olof      (1000)     8484 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/modelsim.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2551 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/morty.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5267 2022-05-31 20:24:45.000000 edalize-0.5.0/edalize/nextpnr.py
--rw-r--r--   0 olof      (1000) olof      (1000)     7701 2023-03-06 17:03:51.000000 edalize-0.5.0/edalize/openfpga.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1572 2023-02-28 12:38:03.000000 edalize-0.5.0/edalize/openlane.py
--rw-r--r--   0 olof      (1000) olof      (1000)     6744 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/openroad.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2514 2021-12-20 23:43:00.000000 edalize-0.5.0/edalize/oxide.py
--rw-r--r--   0 olof      (1000) olof      (1000)    10974 2023-02-28 12:25:13.000000 edalize-0.5.0/edalize/quartus.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4330 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/quartus_reporting.py
--rw-r--r--   0 olof      (1000) olof      (1000)     6853 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/questaformal.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4267 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/radiant.py
--rw-r--r--   0 olof      (1000) olof      (1000)    16824 2021-11-14 22:19:47.000000 edalize-0.5.0/edalize/reporting.py
--rw-r--r--   0 olof      (1000) olof      (1000)     8832 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/rivierapro.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4630 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/sandpipersaas.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4224 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/slang.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4716 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/spyglass.py
--rw-r--r--   0 olof      (1000) olof      (1000)    14978 2022-05-31 20:22:09.000000 edalize-0.5.0/edalize/symbiflow.py
--rw-r--r--   0 olof      (1000) olof      (1000)    10375 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/symbiyosys.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.640592 edalize-0.5.0/edalize/templates/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.678592 edalize-0.5.0/edalize/templates/ascentlint/
--rw-r--r--   0 olof      (1000) olof      (1000)      516 2020-08-18 09:53:24.000000 edalize-0.5.0/edalize/templates/ascentlint/Makefile.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      493 2020-08-18 10:08:08.000000 edalize-0.5.0/edalize/templates/ascentlint/run-ascentlint.tcl.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.679592 edalize-0.5.0/edalize/templates/ghdl/
--rw-r--r--   0 olof      (1000) olof      (1000)      853 2021-12-20 23:33:36.000000 edalize-0.5.0/edalize/templates/ghdl/Makefile.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.679592 edalize-0.5.0/edalize/templates/libero/
--rw-r--r--   0 olof      (1000) olof      (1000)     4302 2021-11-14 22:20:16.000000 edalize-0.5.0/edalize/templates/libero/libero-project.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      544 2021-02-23 18:44:32.000000 edalize-0.5.0/edalize/templates/libero/libero-run.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      601 2021-02-23 18:44:32.000000 edalize-0.5.0/edalize/templates/libero/libero-syn-user.tcl.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.680591 edalize-0.5.0/edalize/templates/openfpga/
--rw-r--r--   0 olof      (1000) olof      (1000)      788 2022-05-31 20:22:09.000000 edalize-0.5.0/edalize/templates/openfpga/task_simulation.conf.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.680591 edalize-0.5.0/edalize/templates/openlane/
--rw-r--r--   0 olof      (1000) olof      (1000)      137 2021-05-12 14:25:08.000000 edalize-0.5.0/edalize/templates/openlane/openlane-makefile.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      159 2021-05-21 08:20:00.000000 edalize-0.5.0/edalize/templates/openlane/openlane-script-tcl.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.681591 edalize-0.5.0/edalize/templates/quartus/
--rw-r--r--   0 olof      (1000) olof      (1000)      928 2021-03-24 13:14:25.000000 edalize-0.5.0/edalize/templates/quartus/quartus-pro-makefile.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      967 2019-07-02 20:03:32.000000 edalize-0.5.0/edalize/templates/quartus/quartus-project.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)     1751 2021-03-24 13:15:48.000000 edalize-0.5.0/edalize/templates/quartus/quartus-std-makefile.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.683591 edalize-0.5.0/edalize/templates/spyglass/
--rw-r--r--   0 olof      (1000) olof      (1000)      276 2018-05-20 19:57:58.000000 edalize-0.5.0/edalize/templates/spyglass/Makefile.j2
--rw-r--r--   0 olof      (1000) olof      (1000)     1444 2018-11-27 22:35:12.000000 edalize-0.5.0/edalize/templates/spyglass/spyglass-project.prj.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      575 2018-11-27 22:35:12.000000 edalize-0.5.0/edalize/templates/spyglass/spyglass-run-goal.tcl.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.683591 edalize-0.5.0/edalize/templates/vcs/
--rw-r--r--   0 olof      (1000) olof      (1000)      359 2023-02-28 12:25:13.000000 edalize-0.5.0/edalize/templates/vcs/Makefile.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.684591 edalize-0.5.0/edalize/templates/vivado/
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2020-04-21 11:13:14.000000 edalize-0.5.0/edalize/templates/vivado/vivado-program.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)     2643 2022-01-20 08:25:17.000000 edalize-0.5.0/edalize/templates/vivado/vivado-project.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)     1652 2021-11-14 22:18:49.000000 edalize-0.5.0/edalize/templates/vivado/vivado-run.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      152 2021-05-07 11:37:51.000000 edalize-0.5.0/edalize/templates/vivado/vivado-synth.tcl.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.684591 edalize-0.5.0/edalize/templates/vunit/
--rw-r--r--   0 olof      (1000) olof      (1000)     1509 2022-12-15 21:24:52.000000 edalize-0.5.0/edalize/templates/vunit/run.py.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.685591 edalize-0.5.0/edalize/templates/yosys/
--rw-r--r--   0 olof      (1000) olof      (1000)      530 2021-05-07 11:37:51.000000 edalize-0.5.0/edalize/templates/yosys/edalize_yosys_procs.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      238 2022-07-06 15:41:17.000000 edalize-0.5.0/edalize/templates/yosys/yosys-script-tcl.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.688591 edalize-0.5.0/edalize/tools/
--rw-r--r--   0 olof      (1000) olof      (1000)     5076 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/tools/edatool.py
--rw-r--r--   0 olof      (1000) olof      (1000)     6196 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/tools/ghdl.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4067 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/tools/icarus.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1805 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/tools/icepack.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1799 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/tools/icetime.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1749 2023-01-06 22:11:46.000000 edalize-0.5.0/edalize/tools/ipxact2v.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5246 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/tools/nextpnr.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2184 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/tools/surelog.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1383 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/tools/sv2v.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.641592 edalize-0.5.0/edalize/tools/templates/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.690591 edalize-0.5.0/edalize/tools/templates/vivado/
--rw-r--r--   0 olof      (1000) olof      (1000)       84 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/tools/templates/vivado/vivado-netlist.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2022-05-31 20:24:45.000000 edalize-0.5.0/edalize/tools/templates/vivado/vivado-program.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)     2643 2022-12-15 23:35:36.000000 edalize-0.5.0/edalize/tools/templates/vivado/vivado-project.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)     1599 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/tools/templates/vivado/vivado-run.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      344 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/tools/templates/vivado/vivado-synth.tcl.j2
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.690591 edalize-0.5.0/edalize/tools/templates/yosys/
--rw-r--r--   0 olof      (1000) olof      (1000)      601 2021-12-20 23:33:36.000000 edalize-0.5.0/edalize/tools/templates/yosys/edalize_yosys_procs.tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)      273 2021-12-20 23:33:36.000000 edalize-0.5.0/edalize/tools/templates/yosys/yosys-script-tcl.j2
--rw-r--r--   0 olof      (1000) olof      (1000)     5025 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/tools/verilator.py
--rw-r--r--   0 olof      (1000) olof      (1000)    10066 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/tools/vivado.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5609 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/tools/vpr.py
--rw-r--r--   0 olof      (1000) olof      (1000)     6774 2023-03-24 22:06:41.000000 edalize-0.5.0/edalize/tools/yosys.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2176 2021-12-20 23:33:36.000000 edalize-0.5.0/edalize/trellis.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2474 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/utils.py
--rw-r--r--   0 olof      (1000) olof      (1000)     3386 2022-07-06 15:41:17.000000 edalize-0.5.0/edalize/vcs.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2199 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/veribleformat.py
--rw-r--r--   0 olof      (1000) olof      (1000)     3543 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/veriblelint.py
--rw-r--r--   0 olof      (1000) olof      (1000)     8570 2022-07-06 15:41:17.000000 edalize-0.5.0/edalize/verilator.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4772 2023-02-28 12:25:29.000000 edalize-0.5.0/edalize/vivado.py
--rw-r--r--   0 olof      (1000) olof      (1000)    10553 2021-11-14 22:19:47.000000 edalize-0.5.0/edalize/vivado_reporting.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1684 2022-05-31 20:24:45.000000 edalize-0.5.0/edalize/vpr.py
--rw-r--r--   0 olof      (1000) olof      (1000)     4465 2022-12-15 21:24:52.000000 edalize-0.5.0/edalize/vunit.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1237 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/vunit_hooks.py
--rw-r--r--   0 olof      (1000) olof      (1000)     7058 2021-12-20 23:32:01.000000 edalize-0.5.0/edalize/xcelium.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5842 2022-05-31 20:24:45.000000 edalize-0.5.0/edalize/xsim.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5584 2023-03-06 16:31:40.000000 edalize-0.5.0/edalize/yosys.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.676591 edalize-0.5.0/edalize.egg-info/
--rw-r--r--   0 olof      (1000) olof      (1000)     7697 2023-03-24 22:07:08.000000 edalize-0.5.0/edalize.egg-info/PKG-INFO
--rw-r--r--   0 olof      (1000) olof      (1000)    21242 2023-03-24 22:07:08.000000 edalize-0.5.0/edalize.egg-info/SOURCES.txt
--rw-r--r--   0 olof      (1000) olof      (1000)        1 2023-03-24 22:07:08.000000 edalize-0.5.0/edalize.egg-info/dependency_links.txt
--rw-r--r--   0 olof      (1000) olof      (1000)       40 2023-03-24 22:07:08.000000 edalize-0.5.0/edalize.egg-info/requires.txt
--rw-r--r--   0 olof      (1000) olof      (1000)        8 2023-03-24 22:07:08.000000 edalize-0.5.0/edalize.egg-info/top_level.txt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.690591 edalize-0.5.0/scripts/
--rwxr-xr-x   0 olof      (1000) olof      (1000)    11051 2023-02-28 12:38:03.000000 edalize-0.5.0/scripts/el_docker
--rw-r--r--   0 olof      (1000) olof      (1000)       38 2023-03-24 22:07:08.821589 edalize-0.5.0/setup.cfg
--rwxr-xr-x   0 olof      (1000) olof      (1000)     3218 2023-03-24 22:06:41.000000 edalize-0.5.0/setup.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.703591 edalize-0.5.0/tests/
--rw-r--r--   0 olof      (1000) olof      (1000)     1843 2021-12-20 23:33:36.000000 edalize-0.5.0/tests/README.rst
--rw-r--r--   0 olof      (1000) olof      (1000)       70 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/__init__.py
--rw-r--r--   0 olof      (1000) olof      (1000)     8691 2023-03-06 17:03:51.000000 edalize-0.5.0/tests/edalize_common.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1644 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/edalize_flow_common.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1650 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/edalize_tool_common.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.641592 edalize-0.5.0/tests/flows/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.703591 edalize-0.5.0/tests/flows/gls/
--rw-r--r--   0 olof      (1000) olof      (1000)      495 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/flows/gls/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      212 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/flows/gls/design.scr
--rw-r--r--   0 olof      (1000) olof      (1000)      665 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/flows/gls/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/flows/gls/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.716591 edalize-0.5.0/tests/mock_commands/
--rwxr-xr-x   0 olof      (1000) olof      (1000)      375 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/arachne-pnr
--rwxr-xr-x   0 olof      (1000) olof      (1000)      199 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/ascentlint
--rwxr-xr-x   0 olof      (1000) olof      (1000)      125 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/diamondc
--rwxr-xr-x   0 olof      (1000) olof      (1000)      272 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/ecppack
--rwxr-xr-x   0 olof      (1000) olof      (1000)       35 2021-05-12 14:30:34.000000 edalize-0.5.0/tests/mock_commands/flow.tcl
--rwxr-xr-x   0 olof      (1000) olof      (1000)      518 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/ghdl
--rwxr-xr-x   0 olof      (1000) olof      (1000)      298 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/gowin_pack
--rwxr-xr-x   0 olof      (1000) olof      (1000)      272 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/icepack
--rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/ip-generate
--rwxr-xr-x   0 olof      (1000) olof      (1000)      302 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/iverilog
--rwxr-xr-x   0 olof      (1000) olof      (1000)      286 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/iverilog-vpi
--rwxr-xr-x   0 olof      (1000) olof      (1000)       32 2020-09-07 21:04:53.000000 edalize-0.5.0/tests/mock_commands/morty
--rwxr-xr-x   0 olof      (1000) olof      (1000)      248 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/nextpnr-ecp5
--rwxr-xr-x   0 olof      (1000) olof      (1000)      247 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/nextpnr-gowin
--rwxr-xr-x   0 olof      (1000) olof      (1000)      245 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/nextpnr-ice40
--rwxr-xr-x   0 olof      (1000) olof      (1000)      247 2022-05-31 20:24:45.000000 edalize-0.5.0/tests/mock_commands/nextpnr-mistral
--rwxr-xr-x   0 olof      (1000) olof      (1000)      246 2022-01-20 07:26:39.000000 edalize-0.5.0/tests/mock_commands/nextpnr-nexus
--rwxr-xr-x   0 olof      (1000) olof      (1000)      291 2022-07-06 15:41:17.000000 edalize-0.5.0/tests/mock_commands/p_r
--rwxr-xr-x   0 olof      (1000) olof      (1000)      273 2022-01-20 07:26:39.000000 edalize-0.5.0/tests/mock_commands/prjoxide
--rwxr-xr-x   0 olof      (1000) olof      (1000)      130 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/qsys-generate
--rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/quartus_asm
--rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/quartus_dse
--rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/quartus_fit
--rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/quartus_map
--rwxr-xr-x   0 olof      (1000) olof      (1000)       30 2018-05-09 20:12:54.000000 edalize-0.5.0/tests/mock_commands/quartus_pgm
--rwxr-xr-x   0 olof      (1000) olof      (1000)      601 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/quartus_sh
--rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/quartus_sta
--rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/quartus_syn
--rwxr-xr-x   0 olof      (1000) olof      (1000)      124 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/mock_commands/qverify
--rwxr-xr-x   0 olof      (1000) olof      (1000)      125 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/radiantc
--rwxr-xr-x   0 olof      (1000) olof      (1000)      110 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/sby
--rwxr-xr-x   0 olof      (1000) olof      (1000)      125 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/sg_shell
--rwxr-xr-x   0 olof      (1000) olof      (1000)      122 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/mock_commands/slang
--rwxr-xr-x   0 olof      (1000) olof      (1000)      619 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/vcs
--rwxr-xr-x   0 olof      (1000) olof      (1000)      129 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/verible-verilog-format
--rwxr-xr-x   0 olof      (1000) olof      (1000)      127 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/verible-verilog-lint
--rwxr-xr-x   0 olof      (1000) olof      (1000)      123 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/vivado
--rwxr-xr-x   0 olof      (1000) olof      (1000)      121 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/vsim
--rwxr-xr-x   0 olof      (1000) olof      (1000)       30 2018-05-09 20:12:54.000000 edalize-0.5.0/tests/mock_commands/vvp
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.717591 edalize-0.5.0/tests/mock_commands/xcelium/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.641592 edalize-0.5.0/tests/mock_commands/xcelium/tools/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.717591 edalize-0.5.0/tests/mock_commands/xcelium/tools/bin/
--rwxr-xr-x   0 olof      (1000) olof      (1000)      152 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/xcelium/tools/bin/xrun
--rwxr-xr-x   0 olof      (1000) olof      (1000)       86 2020-08-18 09:49:05.000000 edalize-0.5.0/tests/mock_commands/xcelium/xmroot
--rwxr-xr-x   0 olof      (1000) olof      (1000)       32 2018-05-09 20:12:54.000000 edalize-0.5.0/tests/mock_commands/xelab
--rwxr-xr-x   0 olof      (1000) olof      (1000)       31 2018-05-09 20:12:54.000000 edalize-0.5.0/tests/mock_commands/xsim
--rwxr-xr-x   0 olof      (1000) olof      (1000)      313 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/xtclsh
--rwxr-xr-x   0 olof      (1000) olof      (1000)      458 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/mock_commands/yosys
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.718591 edalize-0.5.0/tests/test_apicula/
--rw-r--r--   0 olof      (1000) olof      (1000)      692 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      721 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      212 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       62 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/gowin_pack.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.720591 edalize-0.5.0/tests/test_apicula/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      648 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      332 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/minimal/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      212 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/minimal/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       62 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/minimal/gowin_pack.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       94 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/minimal/nextpnr-gowin.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/minimal/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      116 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/nextpnr-gowin.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_apicula/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1709 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_apicula.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.642592 edalize-0.5.0/tests/test_ascentlint/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.721591 edalize-0.5.0/tests/test_ascentlint/defaults/
--rw-r--r--   0 olof      (1000) olof      (1000)      497 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_ascentlint/defaults/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       42 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_ascentlint/defaults/ascentlint.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      289 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_ascentlint/defaults/run-ascentlint.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      147 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_ascentlint/defaults/sources.f
--rw-r--r--   0 olof      (1000) olof      (1000)      488 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_ascentlint.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.721591 edalize-0.5.0/tests/test_diamond/
--rw-r--r--   0 olof      (1000) olof      (1000)       42 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_diamond/diamondc.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.722591 edalize-0.5.0/tests/test_diamond/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)       58 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_diamond/minimal/diamondc.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      156 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_diamond/minimal/test_diamond_minimal_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      147 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_diamond/minimal/test_diamond_minimal_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      871 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_diamond/test_diamond_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      139 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_diamond/test_diamond_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1386 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_diamond.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.722591 edalize-0.5.0/tests/test_edam/
--rwxr-xr-x   0 olof      (1000) olof      (1000)        7 2021-11-14 22:18:49.000000 edalize-0.5.0/tests/test_edam/exit_1_script
--rw-r--r--   0 olof      (1000) olof      (1000)     4374 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_edam.py
--rw-r--r--   0 olof      (1000) olof      (1000)      415 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_flow_gls.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.723591 edalize-0.5.0/tests/test_gatemate/
--rw-r--r--   0 olof      (1000) olof      (1000)      351 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      699 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      219 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.724591 edalize-0.5.0/tests/test_gatemate/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      329 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      311 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/minimal/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      219 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/minimal/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       61 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/minimal/p_r.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/minimal/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       84 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/p_r.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_gatemate/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     2437 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_gatemate.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.643592 edalize-0.5.0/tests/test_ghdl/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.725591 edalize-0.5.0/tests/test_ghdl/test01/
--rw-r--r--   0 olof      (1000) olof      (1000)      956 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_ghdl/test01/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      152 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_ghdl/test01/analyze.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      181 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_ghdl/test01/elab-run.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.726590 edalize-0.5.0/tests/test_ghdl/test02/
--rw-r--r--   0 olof      (1000) olof      (1000)      929 2022-09-22 21:31:10.000000 edalize-0.5.0/tests/test_ghdl/test02/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      140 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_ghdl/test02/analyze.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      183 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_ghdl/test02/elab-run.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.726590 edalize-0.5.0/tests/test_ghdl/test03/
--rw-r--r--   0 olof      (1000) olof      (1000)      923 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_ghdl/test03/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      128 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_ghdl/test03/analyze.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      171 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_ghdl/test03/elab-run.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.727590 edalize-0.5.0/tests/test_ghdl/test04/
--rw-r--r--   0 olof      (1000) olof      (1000)      984 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_ghdl/test04/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      152 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_ghdl/test04/analyze.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      239 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_ghdl/test04/elab-run.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     3229 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_ghdl.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.729591 edalize-0.5.0/tests/test_icarus/
--rw-r--r--   0 olof      (1000) olof      (1000)      884 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_icarus/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       87 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icarus/iverilog-vpi.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       73 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icarus/iverilog.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.730590 edalize-0.5.0/tests/test_icarus/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      394 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_icarus/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       60 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icarus/minimal/iverilog.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icarus/minimal/test_icarus_minimal_0.scr
--rw-r--r--   0 olof      (1000) olof      (1000)       44 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icarus/minimal/vvp.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      281 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icarus/test_icarus_0.scr
--rw-r--r--   0 olof      (1000) olof      (1000)       19 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icarus/timescale.v
--rw-r--r--   0 olof      (1000) olof      (1000)      101 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icarus/vvp.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1403 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_icarus.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.731590 edalize-0.5.0/tests/test_icestorm/
--rw-r--r--   0 olof      (1000) olof      (1000)     1123 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_icestorm/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       97 2020-11-17 21:59:44.000000 edalize-0.5.0/tests/test_icestorm/arachne-pnr.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      722 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       40 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/icepack.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.733590 edalize-0.5.0/tests/test_icestorm/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)     1041 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_icestorm/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       71 2020-11-17 21:59:44.000000 edalize-0.5.0/tests/test_icestorm/minimal/arachne-pnr.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      358 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_icestorm/minimal/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/minimal/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       40 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/minimal/icepack.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       85 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/minimal/nextpnr-ice40.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/minimal/yosys.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.734590 edalize-0.5.0/tests/test_icestorm/nextpnr/
--rw-r--r--   0 olof      (1000) olof      (1000)     1197 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_icestorm/nextpnr/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      747 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_icestorm/nextpnr/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/nextpnr/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       64 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_icestorm/nextpnr/icepack.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      110 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_icestorm/nextpnr/nextpnr-ice40.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_icestorm/nextpnr/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       85 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/nextpnr-ice40.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:11.000000 edalize-0.5.0/tests/test_icestorm/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     2857 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_icestorm.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.735590 edalize-0.5.0/tests/test_ise/
--rw-r--r--   0 olof      (1000) olof      (1000)      204 2023-02-28 12:25:13.000000 edalize-0.5.0/tests/test_ise/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       46 2022-12-18 19:44:28.000000 edalize-0.5.0/tests/test_ise/config.mk
--rw-r--r--   0 olof      (1000) olof      (1000)     1009 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_ise/test_ise_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       88 2022-12-18 19:44:28.000000 edalize-0.5.0/tests/test_ise/test_ise_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       50 2022-12-18 19:44:28.000000 edalize-0.5.0/tests/test_ise/xtclsh.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1006 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_ise.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.737590 edalize-0.5.0/tests/test_isim/
--rw-r--r--   0 olof      (1000) olof      (1000)      348 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_isim/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      491 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_isim/config.mk
--rw-r--r--   0 olof      (1000) olof      (1000)      136 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_isim/run.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       54 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_isim/run_test_isim_0.tcl
--rwxr-xr-x   0 olof      (1000) olof      (1000)       30 2018-05-09 20:12:54.000000 edalize-0.5.0/tests/test_isim/test_isim_0
--rw-r--r--   0 olof      (1000) olof      (1000)      167 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_isim/test_isim_0.prj
--rw-r--r--   0 olof      (1000) olof      (1000)      506 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_isim.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.738590 edalize-0.5.0/tests/test_libero/
--rw-r--r--   0 olof      (1000) olof      (1000)     3064 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_libero/libero-test-all-project.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      541 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_libero/libero-test-all-run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      387 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_libero/libero-test-all-syn-user.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     2978 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_libero/libero-test-project.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      537 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_libero/libero-test-run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      387 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_libero/libero-test-syn-user.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1161 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_libero.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.739590 edalize-0.5.0/tests/test_mistral/
--rw-r--r--   0 olof      (1000) olof      (1000)      606 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      699 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      212 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.740590 edalize-0.5.0/tests/test_mistral/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      502 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      311 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/minimal/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      212 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/minimal/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       86 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/minimal/nextpnr-mistral.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/minimal/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      138 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/nextpnr-mistral.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_mistral/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1690 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_mistral.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.741590 edalize-0.5.0/tests/test_modelsim/
--rw-r--r--   0 olof      (1000) olof      (1000)     1343 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_modelsim/Makefile
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.743590 edalize-0.5.0/tests/test_modelsim/common_compilation/
--rw-r--r--   0 olof      (1000) olof      (1000)     1343 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_modelsim/common_compilation/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      394 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_modelsim/common_compilation/edalize_build_rtl.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       67 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_modelsim/common_compilation/edalize_main.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       33 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_modelsim/common_compilation/vsim.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      287 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_modelsim/common_compilation/vsim2.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      789 2023-01-01 22:22:02.000000 edalize-0.5.0/tests/test_modelsim/edalize_build_rtl.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       67 2023-01-01 22:22:02.000000 edalize-0.5.0/tests/test_modelsim/edalize_main.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       33 2023-01-01 22:22:02.000000 edalize-0.5.0/tests/test_modelsim/vsim.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      287 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_modelsim/vsim2.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1999 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_modelsim.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.743590 edalize-0.5.0/tests/test_morty/
--rw-r--r--   0 olof      (1000) olof      (1000)      141 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_morty/morty.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      332 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_morty.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.644592 edalize-0.5.0/tests/test_openfpga/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.744590 edalize-0.5.0/tests/test_openfpga/config/
--rw-r--r--   0 olof      (1000) olof      (1000)     1116 2023-03-06 17:03:51.000000 edalize-0.5.0/tests/test_openfpga/config/task.conf
--rw-r--r--   0 olof      (1000) olof      (1000)      572 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_openfpga.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.746590 edalize-0.5.0/tests/test_openlane/
--rw-r--r--   0 olof      (1000) olof      (1000)      140 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_openlane/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      261 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_openlane/config.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       45 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_openlane/flow.tcl.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      371 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_openlane.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.748590 edalize-0.5.0/tests/test_oxide/
--rw-r--r--   0 olof      (1000) olof      (1000)      708 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      693 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      210 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.749590 edalize-0.5.0/tests/test_oxide/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      604 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      305 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/minimal/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      210 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/minimal/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       90 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/minimal/nextpnr-nexus.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       40 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/minimal/prjoxide.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/minimal/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      142 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/nextpnr-nexus.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       40 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/prjoxide.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_oxide/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1654 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_oxide.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.645592 edalize-0.5.0/tests/test_plugin/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.749590 edalize-0.5.0/tests/test_plugin/edalize/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.749590 edalize-0.5.0/tests/test_plugin/edalize/flows/
--rw-r--r--   0 olof      (1000) olof      (1000)      352 2023-03-06 16:31:58.000000 edalize-0.5.0/tests/test_plugin/edalize/flows/customexternalflow.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1034 2023-03-06 16:31:58.000000 edalize-0.5.0/tests/test_plugin/edalize/testplugin.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.750590 edalize-0.5.0/tests/test_plugin/edalize/tools/
--rw-r--r--   0 olof      (1000) olof      (1000)     2183 2023-03-06 16:31:58.000000 edalize-0.5.0/tests/test_plugin/edalize/tools/customtool.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1519 2023-03-06 16:31:58.000000 edalize-0.5.0/tests/test_plugin.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.645592 edalize-0.5.0/tests/test_quartus/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.752590 edalize-0.5.0/tests/test_quartus/Pro/
--rw-r--r--   0 olof      (1000) olof      (1000)      760 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      106 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/qsys-generate.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/quartus_asm.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       32 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/quartus_dse.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/quartus_fit.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       43 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/quartus_sh.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/quartus_sta.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/quartus_syn.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1158 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Pro/test_quartus_0.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.755590 edalize-0.5.0/tests/test_quartus/Standard/
--rw-r--r--   0 olof      (1000) olof      (1000)     1366 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_quartus/Standard/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      438 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Standard/ip-generate.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_quartus/Standard/quartus_asm.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       32 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Standard/quartus_dse.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_quartus/Standard/quartus_fit.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Standard/quartus_map.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       43 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_quartus/Standard/quartus_sh.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_quartus/Standard/quartus_sta.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1176 2022-09-22 21:31:12.000000 edalize-0.5.0/tests/test_quartus/Standard/test_quartus_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     2536 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_quartus.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1080 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_questa_formal.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.756590 edalize-0.5.0/tests/test_questaformal/
--rw-r--r--   0 olof      (1000) olof      (1000)      270 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_questaformal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      789 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_questaformal/edalize_build_rtl.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       67 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_questaformal/edalize_main.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       33 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_questaformal/qverify.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       57 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_questaformal/qverify2.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.757590 edalize-0.5.0/tests/test_radiant/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.758590 edalize-0.5.0/tests/test_radiant/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)       58 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_radiant/minimal/radiantc.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      140 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_radiant/minimal/test_radiant_minimal_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      201 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_radiant/minimal/test_radiant_minimal_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       42 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_radiant/radiantc.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      704 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_radiant/test_radiant_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      193 2022-09-22 21:31:13.000000 edalize-0.5.0/tests/test_radiant/test_radiant_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1384 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_radiant.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.646592 edalize-0.5.0/tests/test_reporting/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.647592 edalize-0.5.0/tests/test_reporting/data/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.647592 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.761590 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/
--rw-r--r--   0 olof      (1000) olof      (1000)   730139 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/top_timing.rpt
--rw-r--r--   0 olof      (1000) olof      (1000)    10825 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/top_utilization_place.rpt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.763590 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/
--rw-r--r--   0 olof      (1000) olof      (1000)   614846 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/top.fit.rpt
--rw-r--r--   0 olof      (1000) olof      (1000)   212904 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/top.sta.rpt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.764590 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/
--rw-r--r--   0 olof      (1000) olof      (1000)    76972 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/top.twr
--rw-r--r--   0 olof      (1000) olof      (1000)    72356 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/top_map.mrp
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.765590 edalize-0.5.0/tests/test_reporting/data/picorv32/
--rw-r--r--   0 olof      (1000) olof      (1000)      720 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/README.md
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.766590 edalize-0.5.0/tests/test_reporting/data/picorv32/ise-spartan6/
--rw-r--r--   0 olof      (1000) olof      (1000)    35151 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/ise-spartan6/top.twr
--rw-r--r--   0 olof      (1000) olof      (1000)    21326 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/ise-spartan6/top_map.mrp
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.767590 edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone10/
--rw-r--r--   0 olof      (1000) olof      (1000)   216939 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone10/picorv32_wrap_0_1.fit.rpt
--rw-r--r--   0 olof      (1000) olof      (1000)    26320 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone10/picorv32_wrap_0_1.sta.rpt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.769590 edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone4/
--rw-r--r--   0 olof      (1000) olof      (1000)   150697 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone4/picorv32_wrap_0_1.fit.rpt
--rw-r--r--   0 olof      (1000) olof      (1000)   142009 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone4/picorv32_wrap_0_1.sta.rpt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.648592 edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-artix7/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.770590 edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-artix7/impl/
--rw-r--r--   0 olof      (1000) olof      (1000)    99238 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-artix7/impl/top_timing_summary_routed.rpt
--rw-r--r--   0 olof      (1000) olof      (1000)     9783 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-artix7/impl/top_utilization_placed.rpt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.648592 edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-kintex_usp/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.771590 edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/
--rw-r--r--   0 olof      (1000) olof      (1000)   102752 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/top_timing_summary_routed.rpt
--rw-r--r--   0 olof      (1000) olof      (1000)    10698 2021-01-26 21:20:02.000000 edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/top_utilization_placed.rpt
--rw-r--r--   0 olof      (1000) olof      (1000)    20571 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_reporting.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.773590 edalize-0.5.0/tests/test_rivierapro/
--rw-r--r--   0 olof      (1000) olof      (1000)      732 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_rivierapro/edalize_build_rtl.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      125 2018-05-09 20:12:54.000000 edalize-0.5.0/tests/test_rivierapro/edalize_build_vpi.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      146 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_rivierapro/edalize_launch.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       41 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_rivierapro/edalize_main.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       36 2018-05-13 18:01:33.000000 edalize-0.5.0/tests/test_rivierapro/edalize_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       33 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_rivierapro/vsim.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       30 2018-05-13 18:01:37.000000 edalize-0.5.0/tests/test_rivierapro/vsim2.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      964 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_rivierapro.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.650592 edalize-0.5.0/tests/test_slang/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.774590 edalize-0.5.0/tests/test_slang/lint/
--rw-r--r--   0 olof      (1000) olof      (1000)      219 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_slang/lint/slang.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.774590 edalize-0.5.0/tests/test_slang/preprocess/
--rw-r--r--   0 olof      (1000) olof      (1000)      220 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_slang/preprocess/slang.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.774590 edalize-0.5.0/tests/test_slang/slang_options/
--rw-r--r--   0 olof      (1000) olof      (1000)      219 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_slang/slang_options/slang.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1262 2023-02-28 12:38:03.000000 edalize-0.5.0/tests/test_slang.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.650592 edalize-0.5.0/tests/test_spyglass/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.779590 edalize-0.5.0/tests/test_spyglass/defaults/
--rw-r--r--   0 olof      (1000) olof      (1000)      307 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/defaults/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      581 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/defaults/spyglass-run-design_read.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      583 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/defaults/spyglass-run-lint_lint_rtl.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      583 2018-11-27 22:35:12.000000 edalize-0.5.0/tests/test_spyglass/defaults/spyglass-run-some_othergoal.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      118 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/defaults/spyglass.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1262 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/defaults/test_spyglass_0.prj
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.782590 edalize-0.5.0/tests/test_spyglass/tooloptions/
--rw-r--r--   0 olof      (1000) olof      (1000)      428 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/tooloptions/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      581 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/tooloptions/spyglass-run-design_read.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      583 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/tooloptions/spyglass-run-lint_lint_rtl.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      584 2020-04-23 21:14:25.000000 edalize-0.5.0/tests/test_spyglass/tooloptions/spyglass-run-some_othergoal.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      179 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/tooloptions/spyglass.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1345 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_spyglass/tooloptions/test_spyglass_0.prj
--rw-r--r--   0 olof      (1000) olof      (1000)     1195 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_spyglass.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.651592 edalize-0.5.0/tests/test_symbiflow/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.651592 edalize-0.5.0/tests/test_symbiflow/nextpnr/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.783589 edalize-0.5.0/tests/test_symbiflow/nextpnr/fpga_interchange/
--rw-r--r--   0 olof      (1000) olof      (1000)     1777 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiflow/nextpnr/fpga_interchange/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      529 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiflow/nextpnr/fpga_interchange/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      239 2023-02-28 12:25:13.000000 edalize-0.5.0/tests/test_symbiflow/nextpnr/fpga_interchange/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.783589 edalize-0.5.0/tests/test_symbiflow/nextpnr/xilinx/
--rw-r--r--   0 olof      (1000) olof      (1000)      772 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiflow/nextpnr/xilinx/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      519 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiflow/nextpnr/xilinx/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      229 2023-02-28 12:25:13.000000 edalize-0.5.0/tests/test_symbiflow/nextpnr/xilinx/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.784589 edalize-0.5.0/tests/test_symbiflow/vtr/
--rw-r--r--   0 olof      (1000) olof      (1000)     1141 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiflow/vtr/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)     2919 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_symbiflow.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.785589 edalize-0.5.0/tests/test_symbiyosys/
--rw-r--r--   0 olof      (1000) olof      (1000)      195 2020-09-07 21:04:53.000000 edalize-0.5.0/tests/test_symbiyosys/config.sby.j2
--rw-r--r--   0 olof      (1000) olof      (1000)       56 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiyosys/files.txt
--rw-r--r--   0 olof      (1000) olof      (1000)        2 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiyosys/incdirs.txt
--rw-r--r--   0 olof      (1000) olof      (1000)       30 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiyosys/sby.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      668 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_symbiyosys/test.sby
--rw-r--r--   0 olof      (1000) olof      (1000)     1160 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_symbiyosys.py
--rw-r--r--   0 olof      (1000) olof      (1000)      477 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_tool_icarus.py
--rw-r--r--   0 olof      (1000) olof      (1000)      917 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_tool_vivado.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1580 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_tool_yosys.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.787589 edalize-0.5.0/tests/test_trellis/
--rw-r--r--   0 olof      (1000) olof      (1000)      689 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       66 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/ecppack.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      694 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      212 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.788589 edalize-0.5.0/tests/test_trellis/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      607 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       66 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_trellis/minimal/ecppack.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      306 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/minimal/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      212 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/minimal/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       71 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_trellis/minimal/nextpnr-ecp5.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_trellis/minimal/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      112 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/nextpnr-ecp5.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2022-09-22 21:31:34.000000 edalize-0.5.0/tests/test_trellis/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1301 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_trellis.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.652592 edalize-0.5.0/tests/test_vcs/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.789589 edalize-0.5.0/tests/test_vcs/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      234 2023-02-28 12:25:13.000000 edalize-0.5.0/tests/test_vcs/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       11 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/minimal/run.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/minimal/test_vcs_minimal_0.scr
--rw-r--r--   0 olof      (1000) olof      (1000)       65 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/minimal/vcs.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.790589 edalize-0.5.0/tests/test_vcs/no_tool_options/
--rw-r--r--   0 olof      (1000) olof      (1000)      247 2023-02-28 12:25:13.000000 edalize-0.5.0/tests/test_vcs/no_tool_options/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       60 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/no_tool_options/run.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      282 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/no_tool_options/test_vcs_0.scr
--rw-r--r--   0 olof      (1000) olof      (1000)       66 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/no_tool_options/vcs.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.791589 edalize-0.5.0/tests/test_vcs/tool_options/
--rw-r--r--   0 olof      (1000) olof      (1000)      383 2023-02-28 12:25:13.000000 edalize-0.5.0/tests/test_vcs/tool_options/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)       70 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/tool_options/run.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      282 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/tool_options/test_vcs_tool_options_0.scr
--rw-r--r--   0 olof      (1000) olof      (1000)      127 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_vcs/tool_options/vcs.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1520 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_vcs.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.652592 edalize-0.5.0/tests/test_veribleformat/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.791589 edalize-0.5.0/tests/test_veribleformat/default/
--rw-r--r--   0 olof      (1000) olof      (1000)       56 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_veribleformat/default/verible-verilog-format.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      434 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_veribleformat.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.652592 edalize-0.5.0/tests/test_veriblelint/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.791589 edalize-0.5.0/tests/test_veriblelint/lint/
--rw-r--r--   0 olof      (1000) olof      (1000)      484 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_veriblelint/lint/verible-verilog-lint.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      423 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_veriblelint.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.792589 edalize-0.5.0/tests/test_verilator/
--rw-r--r--   0 olof      (1000) olof      (1000)      361 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_verilator/Makefile
--rwxr-xr-x   0 olof      (1000) olof      (1000)       30 2020-03-16 21:28:04.000000 edalize-0.5.0/tests/test_verilator/Vtop_module
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.793589 edalize-0.5.0/tests/test_verilator/cc/
--rw-r--r--   0 olof      (1000) olof      (1000)      175 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_verilator/cc/config.mk
--rw-r--r--   0 olof      (1000) olof      (1000)      286 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_verilator/cc/test_verilator_0.vc
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.794589 edalize-0.5.0/tests/test_verilator/lint-only/
--rw-r--r--   0 olof      (1000) olof      (1000)      145 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_verilator/lint-only/config.mk
--rw-r--r--   0 olof      (1000) olof      (1000)      151 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_verilator/lint-only/test_verilator_0.vc
--rw-r--r--   0 olof      (1000) olof      (1000)      114 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_verilator/run.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.794589 edalize-0.5.0/tests/test_verilator/sc/
--rw-r--r--   0 olof      (1000) olof      (1000)      145 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_verilator/sc/config.mk
--rw-r--r--   0 olof      (1000) olof      (1000)      144 2022-09-22 21:31:35.000000 edalize-0.5.0/tests/test_verilator/sc/test_verilator_0.vc
--rw-r--r--   0 olof      (1000) olof      (1000)     1262 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_verilator.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.796589 edalize-0.5.0/tests/test_vivado/
--rw-r--r--   0 olof      (1000) olof      (1000)     1159 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/Makefile
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.798589 edalize-0.5.0/tests/test_vivado/board_file/
--rw-r--r--   0 olof      (1000) olof      (1000)     1159 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/board_file/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)     1966 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/board_file/test_vivado_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/board_file/test_vivado_0_pgm.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/board_file/test_vivado_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/board_file/test_vivado_0_synth.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      203 2022-06-11 20:28:55.000000 edalize-0.5.0/tests/test_vivado/board_file/test_vivado_minimal_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2022-06-11 20:28:55.000000 edalize-0.5.0/tests/test_vivado/board_file/test_vivado_minimal_0_pgm.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1619 2022-06-11 20:28:55.000000 edalize-0.5.0/tests/test_vivado/board_file/test_vivado_minimal_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      142 2022-06-11 20:28:55.000000 edalize-0.5.0/tests/test_vivado/board_file/test_vivado_minimal_0_synth.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      140 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/board_file/vivado.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.799589 edalize-0.5.0/tests/test_vivado/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)     1207 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      203 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/minimal/test_vivado_minimal_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/minimal/test_vivado_minimal_0_pgm.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/minimal/test_vivado_minimal_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/minimal/test_vivado_minimal_0_synth.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      172 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/minimal/vivado.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1721 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/test_vivado_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/test_vivado_0_pgm.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/test_vivado_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/test_vivado_0_synth.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      140 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/vivado.cmd
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.800589 edalize-0.5.0/tests/test_vivado/yosys/
--rw-r--r--   0 olof      (1000) olof      (1000)     1033 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/yosys/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      331 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/yosys/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      243 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/yosys/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      295 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/yosys/test_vivado_yosys_0.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/yosys/test_vivado_yosys_0_pgm.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/yosys/test_vivado_yosys_0_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      164 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/test_vivado/yosys/vivado.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-03-06 16:37:18.000000 edalize-0.5.0/tests/test_vivado/yosys/yosys.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     2726 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_vivado.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.653592 edalize-0.5.0/tests/test_vpr/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.801589 edalize-0.5.0/tests/test_vpr/vpr/
--rw-r--r--   0 olof      (1000) olof      (1000)      771 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_vpr/vpr/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      948 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_vpr.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.801589 edalize-0.5.0/tests/test_vunit/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.801589 edalize-0.5.0/tests/test_vunit/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      534 2019-11-26 22:04:06.000000 edalize-0.5.0/tests/test_vunit/minimal/tb_minimal.vhd
--rw-r--r--   0 olof      (1000) olof      (1000)     1485 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_vunit/run.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.654592 edalize-0.5.0/tests/test_vunit/vunit_mock/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.802589 edalize-0.5.0/tests/test_vunit/vunit_mock/vunit/
--rw-r--r--   0 olof      (1000) olof      (1000)       67 2019-11-26 22:04:06.000000 edalize-0.5.0/tests/test_vunit/vunit_mock/vunit/__init__.py
--rw-r--r--   0 olof      (1000) olof      (1000)      326 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/test_vunit/vunit_mock/vunit/ui.py
--rw-r--r--   0 olof      (1000) olof      (1000)      122 2021-12-20 23:32:01.000000 edalize-0.5.0/tests/test_vunit/vunit_mock/vunit/vhdl_standard.py
--rw-r--r--   0 olof      (1000) olof      (1000)     3556 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_vunit.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.802589 edalize-0.5.0/tests/test_xcelium/
--rw-r--r--   0 olof      (1000) olof      (1000)     1041 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xcelium/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      795 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xcelium/edalize_build_rtl.f
--rw-r--r--   0 olof      (1000) olof      (1000)       43 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xcelium/edalize_main.f
--rw-r--r--   0 olof      (1000) olof      (1000)      228 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xcelium/xrun.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1232 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_xcelium.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.803589 edalize-0.5.0/tests/test_xsim/
--rw-r--r--   0 olof      (1000) olof      (1000)      398 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xsim/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      489 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xsim/config.mk
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.805589 edalize-0.5.0/tests/test_xsim/mfc/
--rw-r--r--   0 olof      (1000) olof      (1000)      398 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xsim/mfc/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      489 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xsim/mfc/config.mk
--rw-r--r--   0 olof      (1000) olof      (1000)      162 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xsim/mfc/test_xsim_0.prj
--rw-r--r--   0 olof      (1000) olof      (1000)      348 2021-01-26 20:36:10.000000 edalize-0.5.0/tests/test_xsim/mfc/xelab.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      127 2021-01-26 20:36:10.000000 edalize-0.5.0/tests/test_xsim/mfc/xsim.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      171 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xsim/test_xsim_0.prj
--rw-r--r--   0 olof      (1000) olof      (1000)      348 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xsim/xelab.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)      127 2022-09-22 21:31:36.000000 edalize-0.5.0/tests/test_xsim/xsim.cmd
--rw-r--r--   0 olof      (1000) olof      (1000)     1610 2022-07-11 20:19:55.000000 edalize-0.5.0/tests/test_xsim.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.654592 edalize-0.5.0/tests/test_yosys/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.805589 edalize-0.5.0/tests/test_yosys/custom_output_name/
--rw-r--r--   0 olof      (1000) olof      (1000)      158 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_yosys/custom_output_name/Makefile
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.805589 edalize-0.5.0/tests/test_yosys/default_output_name/
--rw-r--r--   0 olof      (1000) olof      (1000)      174 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_yosys/default_output_name/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      580 2023-03-06 16:31:40.000000 edalize-0.5.0/tests/test_yosys.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.655592 edalize-0.5.0/tests/tools/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.806589 edalize-0.5.0/tests/tools/icarus/
--rw-r--r--   0 olof      (1000) olof      (1000)      270 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/icarus/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      269 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/icarus/design.scr
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.807589 edalize-0.5.0/tests/tools/icarus/multitop/
--rw-r--r--   0 olof      (1000) olof      (1000)      271 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/icarus/multitop/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      355 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/icarus/multitop/design.scr
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.808589 edalize-0.5.0/tests/tools/vivado/
--rw-r--r--   0 olof      (1000) olof      (1000)      865 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)     1564 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/design.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       84 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/design_netlist.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/design_pgm.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/design_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/design_synth.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.812589 edalize-0.5.0/tests/tools/vivado/tags/
--rw-r--r--   0 olof      (1000) olof      (1000)      877 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/tags/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)     1768 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/tags/design.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       84 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/tags/design_netlist.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/tags/design_pgm.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/tags/design_run.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/vivado/tags/design_synth.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.656592 edalize-0.5.0/tests/tools/yosys/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.812589 edalize-0.5.0/tests/tools/yosys/ecp5-blif/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-blif/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      712 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-blif/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-blif/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.813589 edalize-0.5.0/tests/tools/yosys/ecp5-edif/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-edif/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      712 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-edif/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-edif/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.814589 edalize-0.5.0/tests/tools/yosys/ecp5-json/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-json/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      712 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-json/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-json/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.815589 edalize-0.5.0/tests/tools/yosys/ecp5-verilog/
--rw-r--r--   0 olof      (1000) olof      (1000)      238 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-verilog/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      712 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-verilog/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ecp5-verilog/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.815589 edalize-0.5.0/tests/tools/yosys/ice40-blif/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-blif/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      713 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-blif/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-blif/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.816589 edalize-0.5.0/tests/tools/yosys/ice40-edif/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-edif/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      713 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-edif/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-edif/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.817589 edalize-0.5.0/tests/tools/yosys/ice40-json/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-json/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      713 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-json/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-json/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.817589 edalize-0.5.0/tests/tools/yosys/ice40-verilog/
--rw-r--r--   0 olof      (1000) olof      (1000)      238 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-verilog/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      713 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-verilog/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/ice40-verilog/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.818589 edalize-0.5.0/tests/tools/yosys/minimal/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/minimal/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      689 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/minimal/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/minimal/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.818589 edalize-0.5.0/tests/tools/yosys/template/
--rw-r--r--   0 olof      (1000) olof      (1000)      218 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/template/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      689 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/template/edalize_yosys_procs.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.819589 edalize-0.5.0/tests/tools/yosys/xilinx-blif/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-blif/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      714 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-blif/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-blif/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.819589 edalize-0.5.0/tests/tools/yosys/xilinx-edif/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-edif/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      714 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-edif/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      243 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-edif/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.820589 edalize-0.5.0/tests/tools/yosys/xilinx-json/
--rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-json/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      714 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-json/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-json/edalize_yosys_template.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-24 22:07:08.821589 edalize-0.5.0/tests/tools/yosys/xilinx-verilog/
--rw-r--r--   0 olof      (1000) olof      (1000)      238 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-verilog/Makefile
--rw-r--r--   0 olof      (1000) olof      (1000)      714 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-verilog/edalize_yosys_procs.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-03-24 22:06:41.000000 edalize-0.5.0/tests/tools/yosys/xilinx-verilog/edalize_yosys_template.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)       92 2021-01-26 21:20:02.000000 edalize-0.5.0/tox.ini
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.366881 edalize-0.5.1/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.185882 edalize-0.5.1/.github/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.205882 edalize-0.5.1/.github/workflows/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1425 2023-03-06 16:31:40.000000 edalize-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0 olof      (1000) olof      (1000)      116 2023-02-28 12:38:03.000000 edalize-0.5.1/.gitignore
+-rw-r--r--   0 olof      (1000) olof      (1000)      234 2022-06-11 20:28:55.000000 edalize-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 olof      (1000) olof      (1000)      271 2020-11-17 21:53:11.000000 edalize-0.5.1/.readthedocs.yml
+-rw-r--r--   0 olof      (1000) olof      (1000)     1349 2021-03-28 21:01:38.000000 edalize-0.5.1/LICENSE
+-rw-r--r--   0 olof      (1000) olof      (1000)     1854 2023-05-17 08:24:36.000000 edalize-0.5.1/NEWS
+-rw-r--r--   0 olof      (1000) olof      (1000)     7697 2023-05-17 08:31:29.366881 edalize-0.5.1/PKG-INFO
+-rw-r--r--   0 olof      (1000) olof      (1000)     7033 2023-03-06 16:31:40.000000 edalize-0.5.1/README.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)       22 2021-11-14 22:20:16.000000 edalize-0.5.1/dev-requirements.txt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.208882 edalize-0.5.1/doc/
+-rw-r--r--   0 olof      (1000) olof      (1000)      581 2019-01-17 08:09:28.000000 edalize-0.5.1/doc/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)     6344 2021-12-20 23:32:01.000000 edalize-0.5.1/doc/conf.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.209882 edalize-0.5.1/doc/dev/
+-rw-r--r--   0 olof      (1000) olof      (1000)    11320 2023-03-06 16:31:40.000000 edalize-0.5.1/doc/dev/extend.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      360 2023-03-06 16:31:40.000000 edalize-0.5.1/doc/dev/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1832 2021-12-20 23:33:36.000000 edalize-0.5.1/doc/dev/setup.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      106 2021-12-20 23:33:36.000000 edalize-0.5.1/doc/dev/tests.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     3529 2023-02-23 16:54:50.000000 edalize-0.5.1/doc/edalize.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.209882 edalize-0.5.1/doc/edam/
+-rw-r--r--   0 olof      (1000) olof      (1000)    19643 2022-07-06 15:41:17.000000 edalize-0.5.1/doc/edam/api.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)       66 2021-12-20 23:33:36.000000 edalize-0.5.1/doc/genindex.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     2206 2023-03-06 16:31:40.000000 edalize-0.5.1/doc/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      787 2019-01-17 07:54:32.000000 edalize-0.5.1/doc/make.bat
+-rw-r--r--   0 olof      (1000) olof      (1000)       78 2021-12-20 23:33:36.000000 edalize-0.5.1/doc/py-modindex.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)       64 2020-11-17 21:53:11.000000 edalize-0.5.1/doc/requirements.txt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.211882 edalize-0.5.1/doc/user/
+-rw-r--r--   0 olof      (1000) olof      (1000)       52 2023-03-06 16:31:40.000000 edalize-0.5.1/doc/user/build.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)       64 2023-03-06 16:31:40.000000 edalize-0.5.1/doc/user/configure.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      416 2023-03-06 16:31:40.000000 edalize-0.5.1/doc/user/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)       46 2023-03-06 16:31:40.000000 edalize-0.5.1/doc/user/run.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.224882 edalize-0.5.1/edalize/
+-rw-r--r--   0 olof      (1000) olof      (1000)     2653 2021-12-20 23:33:36.000000 edalize-0.5.1/edalize/apicula.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1864 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/ascentlint.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4940 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/diamond.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    18486 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/edatool.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2180 2023-02-28 12:25:40.000000 edalize-0.5.1/edalize/f4pga.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.226882 edalize-0.5.1/edalize/flows/
+-rw-r--r--   0 olof      (1000) olof      (1000)    12358 2023-05-17 07:07:04.000000 edalize-0.5.1/edalize/flows/edaflow.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     8251 2023-02-28 12:38:03.000000 edalize-0.5.1/edalize/flows/f4pga.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1919 2023-03-24 22:06:41.000000 edalize-0.5.1/edalize/flows/generic.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     3566 2023-03-24 22:06:41.000000 edalize-0.5.1/edalize/flows/gls.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     3033 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/flows/icestorm.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      464 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/flows/lint.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      545 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/flows/sim.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2328 2023-05-17 08:07:03.000000 edalize-0.5.1/edalize/flows/vivado.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      944 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/flows/vpr.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     3476 2022-07-06 15:41:17.000000 edalize-0.5.1/edalize/gatemate.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6680 2021-12-20 23:33:36.000000 edalize-0.5.1/edalize/ghdl.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5418 2023-02-28 12:38:03.000000 edalize-0.5.1/edalize/icarus.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2133 2022-07-09 21:04:13.000000 edalize-0.5.1/edalize/icestorm.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6959 2023-02-28 12:38:03.000000 edalize-0.5.1/edalize/ise.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    10673 2021-11-14 22:19:47.000000 edalize-0.5.1/edalize/ise_reporting.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5573 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/isim.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     7727 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/libero.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2343 2022-05-31 20:24:45.000000 edalize-0.5.1/edalize/mistral.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     8484 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/modelsim.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2551 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/morty.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5267 2022-05-31 20:24:45.000000 edalize-0.5.1/edalize/nextpnr.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     7701 2023-03-06 17:03:51.000000 edalize-0.5.1/edalize/openfpga.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1572 2023-02-28 12:38:03.000000 edalize-0.5.1/edalize/openlane.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6744 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/openroad.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2514 2021-12-20 23:43:00.000000 edalize-0.5.1/edalize/oxide.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    10974 2023-02-28 12:25:13.000000 edalize-0.5.1/edalize/quartus.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4330 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/quartus_reporting.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6853 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/questaformal.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4267 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/radiant.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    16824 2021-11-14 22:19:47.000000 edalize-0.5.1/edalize/reporting.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     8832 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/rivierapro.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4630 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/sandpipersaas.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4224 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/slang.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4716 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/spyglass.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    14978 2022-05-31 20:22:09.000000 edalize-0.5.1/edalize/symbiflow.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    10375 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/symbiyosys.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.188882 edalize-0.5.1/edalize/templates/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.227882 edalize-0.5.1/edalize/templates/ascentlint/
+-rw-r--r--   0 olof      (1000) olof      (1000)      516 2020-08-18 09:53:24.000000 edalize-0.5.1/edalize/templates/ascentlint/Makefile.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      493 2020-08-18 10:08:08.000000 edalize-0.5.1/edalize/templates/ascentlint/run-ascentlint.tcl.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.227882 edalize-0.5.1/edalize/templates/ghdl/
+-rw-r--r--   0 olof      (1000) olof      (1000)      853 2021-12-20 23:33:36.000000 edalize-0.5.1/edalize/templates/ghdl/Makefile.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.228882 edalize-0.5.1/edalize/templates/libero/
+-rw-r--r--   0 olof      (1000) olof      (1000)     4302 2021-11-14 22:20:16.000000 edalize-0.5.1/edalize/templates/libero/libero-project.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      544 2021-02-23 18:44:32.000000 edalize-0.5.1/edalize/templates/libero/libero-run.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      601 2021-02-23 18:44:32.000000 edalize-0.5.1/edalize/templates/libero/libero-syn-user.tcl.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.228882 edalize-0.5.1/edalize/templates/openfpga/
+-rw-r--r--   0 olof      (1000) olof      (1000)      788 2022-05-31 20:22:09.000000 edalize-0.5.1/edalize/templates/openfpga/task_simulation.conf.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.228882 edalize-0.5.1/edalize/templates/openlane/
+-rw-r--r--   0 olof      (1000) olof      (1000)      137 2021-05-12 14:25:08.000000 edalize-0.5.1/edalize/templates/openlane/openlane-makefile.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      159 2021-05-21 08:20:00.000000 edalize-0.5.1/edalize/templates/openlane/openlane-script-tcl.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.229882 edalize-0.5.1/edalize/templates/quartus/
+-rw-r--r--   0 olof      (1000) olof      (1000)      928 2021-03-24 13:14:25.000000 edalize-0.5.1/edalize/templates/quartus/quartus-pro-makefile.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      967 2019-07-02 20:03:32.000000 edalize-0.5.1/edalize/templates/quartus/quartus-project.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)     1751 2021-03-24 13:15:48.000000 edalize-0.5.1/edalize/templates/quartus/quartus-std-makefile.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.230882 edalize-0.5.1/edalize/templates/spyglass/
+-rw-r--r--   0 olof      (1000) olof      (1000)      276 2018-05-20 19:57:58.000000 edalize-0.5.1/edalize/templates/spyglass/Makefile.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)     1444 2018-11-27 22:35:12.000000 edalize-0.5.1/edalize/templates/spyglass/spyglass-project.prj.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      575 2018-11-27 22:35:12.000000 edalize-0.5.1/edalize/templates/spyglass/spyglass-run-goal.tcl.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.230882 edalize-0.5.1/edalize/templates/vcs/
+-rw-r--r--   0 olof      (1000) olof      (1000)      359 2023-02-28 12:25:13.000000 edalize-0.5.1/edalize/templates/vcs/Makefile.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.231882 edalize-0.5.1/edalize/templates/vivado/
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2020-04-21 11:13:14.000000 edalize-0.5.1/edalize/templates/vivado/vivado-program.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)     2643 2022-01-20 08:25:17.000000 edalize-0.5.1/edalize/templates/vivado/vivado-project.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)     1652 2021-11-14 22:18:49.000000 edalize-0.5.1/edalize/templates/vivado/vivado-run.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      152 2021-05-07 11:37:51.000000 edalize-0.5.1/edalize/templates/vivado/vivado-synth.tcl.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.231882 edalize-0.5.1/edalize/templates/vunit/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1509 2022-12-15 21:24:52.000000 edalize-0.5.1/edalize/templates/vunit/run.py.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.232882 edalize-0.5.1/edalize/templates/yosys/
+-rw-r--r--   0 olof      (1000) olof      (1000)      530 2021-05-07 11:37:51.000000 edalize-0.5.1/edalize/templates/yosys/edalize_yosys_procs.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      238 2022-07-06 15:41:17.000000 edalize-0.5.1/edalize/templates/yosys/yosys-script-tcl.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.234882 edalize-0.5.1/edalize/tools/
+-rw-r--r--   0 olof      (1000) olof      (1000)     5076 2023-03-24 22:06:41.000000 edalize-0.5.1/edalize/tools/edatool.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6196 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/tools/ghdl.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4250 2023-04-18 17:29:07.000000 edalize-0.5.1/edalize/tools/icarus.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1805 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/tools/icepack.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1799 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/tools/icetime.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1749 2023-01-06 22:11:46.000000 edalize-0.5.1/edalize/tools/ipxact2v.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6537 2023-04-02 17:56:50.000000 edalize-0.5.1/edalize/tools/modelsim.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5246 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/tools/nextpnr.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2184 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/tools/surelog.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1383 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/tools/sv2v.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.188882 edalize-0.5.1/edalize/tools/templates/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.235882 edalize-0.5.1/edalize/tools/templates/vivado/
+-rw-r--r--   0 olof      (1000) olof      (1000)       84 2023-03-24 22:06:41.000000 edalize-0.5.1/edalize/tools/templates/vivado/vivado-netlist.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2022-05-31 20:24:45.000000 edalize-0.5.1/edalize/tools/templates/vivado/vivado-program.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)     2643 2022-12-15 23:35:36.000000 edalize-0.5.1/edalize/tools/templates/vivado/vivado-project.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)     1599 2023-03-24 22:06:41.000000 edalize-0.5.1/edalize/tools/templates/vivado/vivado-run.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      344 2023-03-24 22:06:41.000000 edalize-0.5.1/edalize/tools/templates/vivado/vivado-synth.tcl.j2
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.235882 edalize-0.5.1/edalize/tools/templates/yosys/
+-rw-r--r--   0 olof      (1000) olof      (1000)      601 2021-12-20 23:33:36.000000 edalize-0.5.1/edalize/tools/templates/yosys/edalize_yosys_procs.tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)      273 2021-12-20 23:33:36.000000 edalize-0.5.1/edalize/tools/templates/yosys/yosys-script-tcl.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)     5069 2023-04-10 13:48:34.000000 edalize-0.5.1/edalize/tools/verilator.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    10066 2023-05-17 07:06:58.000000 edalize-0.5.1/edalize/tools/vivado.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5609 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/tools/vpr.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6723 2023-03-31 23:11:32.000000 edalize-0.5.1/edalize/tools/yosys.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2176 2021-12-20 23:33:36.000000 edalize-0.5.1/edalize/trellis.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2474 2023-04-01 00:57:34.000000 edalize-0.5.1/edalize/utils.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     3386 2022-07-06 15:41:17.000000 edalize-0.5.1/edalize/vcs.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2199 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/veribleformat.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     3543 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/veriblelint.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     8570 2022-07-06 15:41:17.000000 edalize-0.5.1/edalize/verilator.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4772 2023-02-28 12:25:29.000000 edalize-0.5.1/edalize/vivado.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    10553 2021-11-14 22:19:47.000000 edalize-0.5.1/edalize/vivado_reporting.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1684 2022-05-31 20:24:45.000000 edalize-0.5.1/edalize/vpr.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     4465 2022-12-15 21:24:52.000000 edalize-0.5.1/edalize/vunit.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1237 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/vunit_hooks.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     7058 2021-12-20 23:32:01.000000 edalize-0.5.1/edalize/xcelium.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5842 2022-05-31 20:24:45.000000 edalize-0.5.1/edalize/xsim.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5584 2023-03-06 16:31:40.000000 edalize-0.5.1/edalize/yosys.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.225882 edalize-0.5.1/edalize.egg-info/
+-rw-r--r--   0 olof      (1000) olof      (1000)     7697 2023-05-17 08:31:28.000000 edalize-0.5.1/edalize.egg-info/PKG-INFO
+-rw-r--r--   0 olof      (1000) olof      (1000)    21396 2023-05-17 08:31:29.000000 edalize-0.5.1/edalize.egg-info/SOURCES.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)        1 2023-05-17 08:31:28.000000 edalize-0.5.1/edalize.egg-info/dependency_links.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)       40 2023-05-17 08:31:28.000000 edalize-0.5.1/edalize.egg-info/requires.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)        8 2023-05-17 08:31:28.000000 edalize-0.5.1/edalize.egg-info/top_level.txt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.235882 edalize-0.5.1/scripts/
+-rwxr-xr-x   0 olof      (1000) olof      (1000)    11051 2023-02-28 12:38:03.000000 edalize-0.5.1/scripts/el_docker
+-rw-r--r--   0 olof      (1000) olof      (1000)       38 2023-05-17 08:31:29.366881 edalize-0.5.1/setup.cfg
+-rwxr-xr-x   0 olof      (1000) olof      (1000)     3218 2023-05-17 08:19:06.000000 edalize-0.5.1/setup.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.249882 edalize-0.5.1/tests/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1843 2021-12-20 23:33:36.000000 edalize-0.5.1/tests/README.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)       70 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/__init__.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     8691 2023-03-06 17:03:51.000000 edalize-0.5.1/tests/edalize_common.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1644 2023-03-24 22:06:41.000000 edalize-0.5.1/tests/edalize_flow_common.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1650 2023-03-24 22:06:41.000000 edalize-0.5.1/tests/edalize_tool_common.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.189882 edalize-0.5.1/tests/flows/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.250882 edalize-0.5.1/tests/flows/gls/
+-rw-r--r--   0 olof      (1000) olof      (1000)      495 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/flows/gls/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      212 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/flows/gls/design.scr
+-rw-r--r--   0 olof      (1000) olof      (1000)      665 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/flows/gls/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/flows/gls/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.264882 edalize-0.5.1/tests/mock_commands/
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      375 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/arachne-pnr
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      199 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/ascentlint
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      125 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/diamondc
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      272 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/ecppack
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       35 2021-05-12 14:30:34.000000 edalize-0.5.1/tests/mock_commands/flow.tcl
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      518 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/ghdl
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      298 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/gowin_pack
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      272 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/icepack
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/ip-generate
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      302 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/iverilog
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      286 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/iverilog-vpi
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       32 2020-09-07 21:04:53.000000 edalize-0.5.1/tests/mock_commands/morty
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      248 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/nextpnr-ecp5
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      247 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/nextpnr-gowin
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      245 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/nextpnr-ice40
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      247 2022-05-31 20:24:45.000000 edalize-0.5.1/tests/mock_commands/nextpnr-mistral
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      246 2022-01-20 07:26:39.000000 edalize-0.5.1/tests/mock_commands/nextpnr-nexus
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      291 2022-07-06 15:41:17.000000 edalize-0.5.1/tests/mock_commands/p_r
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      273 2022-01-20 07:26:39.000000 edalize-0.5.1/tests/mock_commands/prjoxide
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      130 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/qsys-generate
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/quartus_asm
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/quartus_dse
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/quartus_fit
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/quartus_map
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       30 2018-05-09 20:12:54.000000 edalize-0.5.1/tests/mock_commands/quartus_pgm
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      601 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/quartus_sh
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/quartus_sta
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      128 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/quartus_syn
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      124 2023-02-28 12:38:03.000000 edalize-0.5.1/tests/mock_commands/qverify
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      125 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/radiantc
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      110 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/sby
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      125 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/sg_shell
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      122 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/mock_commands/slang
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      619 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/vcs
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      129 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/verible-verilog-format
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      127 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/verible-verilog-lint
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      123 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/vivado
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      121 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/vsim
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       30 2018-05-09 20:12:54.000000 edalize-0.5.1/tests/mock_commands/vvp
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.264882 edalize-0.5.1/tests/mock_commands/xcelium/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.189882 edalize-0.5.1/tests/mock_commands/xcelium/tools/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.264882 edalize-0.5.1/tests/mock_commands/xcelium/tools/bin/
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      152 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/xcelium/tools/bin/xrun
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       86 2020-08-18 09:49:05.000000 edalize-0.5.1/tests/mock_commands/xcelium/xmroot
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       32 2018-05-09 20:12:54.000000 edalize-0.5.1/tests/mock_commands/xelab
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       31 2018-05-09 20:12:54.000000 edalize-0.5.1/tests/mock_commands/xsim
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      313 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/xtclsh
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      458 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/mock_commands/yosys
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.266882 edalize-0.5.1/tests/test_apicula/
+-rw-r--r--   0 olof      (1000) olof      (1000)      692 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      721 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      212 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       62 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/gowin_pack.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.267882 edalize-0.5.1/tests/test_apicula/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      648 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      332 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/minimal/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      212 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/minimal/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       62 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/minimal/gowin_pack.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       94 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/minimal/nextpnr-gowin.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/minimal/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      116 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/nextpnr-gowin.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_apicula/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1709 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_apicula.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.190882 edalize-0.5.1/tests/test_ascentlint/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.268882 edalize-0.5.1/tests/test_ascentlint/defaults/
+-rw-r--r--   0 olof      (1000) olof      (1000)      497 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ascentlint/defaults/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       42 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ascentlint/defaults/ascentlint.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      289 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ascentlint/defaults/run-ascentlint.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      147 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ascentlint/defaults/sources.f
+-rw-r--r--   0 olof      (1000) olof      (1000)      488 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_ascentlint.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.269882 edalize-0.5.1/tests/test_diamond/
+-rw-r--r--   0 olof      (1000) olof      (1000)       42 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_diamond/diamondc.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.269882 edalize-0.5.1/tests/test_diamond/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)       58 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_diamond/minimal/diamondc.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      156 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_diamond/minimal/test_diamond_minimal_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      147 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_diamond/minimal/test_diamond_minimal_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      871 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_diamond/test_diamond_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      139 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_diamond/test_diamond_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1386 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_diamond.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.270882 edalize-0.5.1/tests/test_edam/
+-rwxr-xr-x   0 olof      (1000) olof      (1000)        7 2021-11-14 22:18:49.000000 edalize-0.5.1/tests/test_edam/exit_1_script
+-rw-r--r--   0 olof      (1000) olof      (1000)     4374 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_edam.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      415 2023-03-24 22:06:41.000000 edalize-0.5.1/tests/test_flow_gls.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.271882 edalize-0.5.1/tests/test_gatemate/
+-rw-r--r--   0 olof      (1000) olof      (1000)      351 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      699 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      219 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.272882 edalize-0.5.1/tests/test_gatemate/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      329 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      311 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/minimal/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      219 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/minimal/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       61 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/minimal/p_r.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/minimal/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       84 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/p_r.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_gatemate/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     2437 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_gatemate.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.191882 edalize-0.5.1/tests/test_ghdl/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.273882 edalize-0.5.1/tests/test_ghdl/test01/
+-rw-r--r--   0 olof      (1000) olof      (1000)      956 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test01/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      152 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test01/analyze.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      181 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test01/elab-run.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.275882 edalize-0.5.1/tests/test_ghdl/test02/
+-rw-r--r--   0 olof      (1000) olof      (1000)      929 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test02/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      140 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test02/analyze.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      183 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test02/elab-run.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.277881 edalize-0.5.1/tests/test_ghdl/test03/
+-rw-r--r--   0 olof      (1000) olof      (1000)      923 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test03/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      128 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test03/analyze.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      171 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test03/elab-run.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.277881 edalize-0.5.1/tests/test_ghdl/test04/
+-rw-r--r--   0 olof      (1000) olof      (1000)      984 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test04/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      152 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test04/analyze.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      239 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_ghdl/test04/elab-run.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     3229 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_ghdl.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.279882 edalize-0.5.1/tests/test_icarus/
+-rw-r--r--   0 olof      (1000) olof      (1000)      884 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_icarus/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       87 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icarus/iverilog-vpi.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       73 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icarus/iverilog.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.280882 edalize-0.5.1/tests/test_icarus/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      394 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icarus/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       60 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icarus/minimal/iverilog.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icarus/minimal/test_icarus_minimal_0.scr
+-rw-r--r--   0 olof      (1000) olof      (1000)       44 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icarus/minimal/vvp.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      281 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_icarus/test_icarus_0.scr
+-rw-r--r--   0 olof      (1000) olof      (1000)       19 2023-04-10 13:36:24.000000 edalize-0.5.1/tests/test_icarus/timescale.v
+-rw-r--r--   0 olof      (1000) olof      (1000)      101 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icarus/vvp.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1403 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_icarus.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.282882 edalize-0.5.1/tests/test_icestorm/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1123 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       97 2020-11-17 21:59:44.000000 edalize-0.5.1/tests/test_icestorm/arachne-pnr.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      722 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       40 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/icepack.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.283882 edalize-0.5.1/tests/test_icestorm/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1041 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       71 2020-11-17 21:59:44.000000 edalize-0.5.1/tests/test_icestorm/minimal/arachne-pnr.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      358 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/minimal/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/minimal/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       40 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/minimal/icepack.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       85 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/minimal/nextpnr-ice40.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/minimal/yosys.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.285882 edalize-0.5.1/tests/test_icestorm/nextpnr/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1197 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/nextpnr/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      747 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/nextpnr/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/nextpnr/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       64 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/nextpnr/icepack.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      110 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/nextpnr/nextpnr-ice40.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/nextpnr/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       85 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/nextpnr-ice40.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_icestorm/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     2857 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_icestorm.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.286882 edalize-0.5.1/tests/test_ise/
+-rw-r--r--   0 olof      (1000) olof      (1000)      204 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_ise/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       46 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_ise/config.mk
+-rw-r--r--   0 olof      (1000) olof      (1000)     1009 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_ise/test_ise_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       88 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_ise/test_ise_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       50 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_ise/xtclsh.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1006 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_ise.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.288882 edalize-0.5.1/tests/test_isim/
+-rw-r--r--   0 olof      (1000) olof      (1000)      348 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_isim/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      491 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_isim/config.mk
+-rw-r--r--   0 olof      (1000) olof      (1000)      136 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_isim/run.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       54 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_isim/run_test_isim_0.tcl
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       30 2018-05-09 20:12:54.000000 edalize-0.5.1/tests/test_isim/test_isim_0
+-rw-r--r--   0 olof      (1000) olof      (1000)      167 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_isim/test_isim_0.prj
+-rw-r--r--   0 olof      (1000) olof      (1000)      506 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_isim.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.289882 edalize-0.5.1/tests/test_libero/
+-rw-r--r--   0 olof      (1000) olof      (1000)     3064 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_libero/libero-test-all-project.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      541 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_libero/libero-test-all-run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      387 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_libero/libero-test-all-syn-user.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     2978 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_libero/libero-test-project.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      537 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_libero/libero-test-run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      387 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_libero/libero-test-syn-user.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1161 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_libero.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.291882 edalize-0.5.1/tests/test_mistral/
+-rw-r--r--   0 olof      (1000) olof      (1000)      606 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      699 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      212 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.292882 edalize-0.5.1/tests/test_mistral/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      502 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      311 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/minimal/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      212 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/minimal/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       86 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/minimal/nextpnr-mistral.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/minimal/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      138 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/nextpnr-mistral.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_mistral/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1690 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_mistral.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.293882 edalize-0.5.1/tests/test_modelsim/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1343 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_modelsim/Makefile
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.294881 edalize-0.5.1/tests/test_modelsim/common_compilation/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1343 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_modelsim/common_compilation/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      394 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_modelsim/common_compilation/edalize_build_rtl.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       67 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_modelsim/common_compilation/edalize_main.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       33 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_modelsim/common_compilation/vsim.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      287 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_modelsim/common_compilation/vsim2.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      789 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_modelsim/edalize_build_rtl.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       67 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_modelsim/edalize_main.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       33 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_modelsim/vsim.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      287 2023-02-28 12:38:03.000000 edalize-0.5.1/tests/test_modelsim/vsim2.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1999 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_modelsim.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.295882 edalize-0.5.1/tests/test_morty/
+-rw-r--r--   0 olof      (1000) olof      (1000)      141 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_morty/morty.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      332 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_morty.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.192882 edalize-0.5.1/tests/test_openfpga/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.295882 edalize-0.5.1/tests/test_openfpga/config/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1116 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_openfpga/config/task.conf
+-rw-r--r--   0 olof      (1000) olof      (1000)      572 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_openfpga.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.296882 edalize-0.5.1/tests/test_openlane/
+-rw-r--r--   0 olof      (1000) olof      (1000)      140 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_openlane/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      261 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_openlane/config.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       45 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_openlane/flow.tcl.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      371 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_openlane.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.298882 edalize-0.5.1/tests/test_oxide/
+-rw-r--r--   0 olof      (1000) olof      (1000)      708 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      693 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      210 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.299882 edalize-0.5.1/tests/test_oxide/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      604 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      305 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/minimal/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      210 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/minimal/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       90 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/minimal/nextpnr-nexus.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       40 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/minimal/prjoxide.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/minimal/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      142 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/nextpnr-nexus.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       40 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/prjoxide.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_oxide/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1654 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_oxide.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.192882 edalize-0.5.1/tests/test_plugin/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.299882 edalize-0.5.1/tests/test_plugin/edalize/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.300881 edalize-0.5.1/tests/test_plugin/edalize/flows/
+-rw-r--r--   0 olof      (1000) olof      (1000)      352 2023-03-06 16:31:58.000000 edalize-0.5.1/tests/test_plugin/edalize/flows/customexternalflow.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1034 2023-03-06 16:31:58.000000 edalize-0.5.1/tests/test_plugin/edalize/testplugin.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.300881 edalize-0.5.1/tests/test_plugin/edalize/tools/
+-rw-r--r--   0 olof      (1000) olof      (1000)     2183 2023-03-06 16:31:58.000000 edalize-0.5.1/tests/test_plugin/edalize/tools/customtool.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1519 2023-03-06 16:31:58.000000 edalize-0.5.1/tests/test_plugin.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.193882 edalize-0.5.1/tests/test_quartus/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.302882 edalize-0.5.1/tests/test_quartus/Pro/
+-rw-r--r--   0 olof      (1000) olof      (1000)      760 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      106 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/qsys-generate.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/quartus_asm.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       32 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/quartus_dse.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/quartus_fit.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       43 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/quartus_sh.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/quartus_sta.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/quartus_syn.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1158 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Pro/test_quartus_0.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.304881 edalize-0.5.1/tests/test_quartus/Standard/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1366 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_quartus/Standard/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      438 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Standard/ip-generate.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_quartus/Standard/quartus_asm.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       32 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Standard/quartus_dse.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_quartus/Standard/quartus_fit.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Standard/quartus_map.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       43 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_quartus/Standard/quartus_sh.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_quartus/Standard/quartus_sta.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1176 2023-04-10 13:36:25.000000 edalize-0.5.1/tests/test_quartus/Standard/test_quartus_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     2536 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_quartus.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1080 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_questa_formal.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.305882 edalize-0.5.1/tests/test_questaformal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      270 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_questaformal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      789 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_questaformal/edalize_build_rtl.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       67 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_questaformal/edalize_main.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       33 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_questaformal/qverify.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       57 2023-02-28 12:38:03.000000 edalize-0.5.1/tests/test_questaformal/qverify2.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.307881 edalize-0.5.1/tests/test_radiant/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.308882 edalize-0.5.1/tests/test_radiant/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)       58 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_radiant/minimal/radiantc.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      140 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_radiant/minimal/test_radiant_minimal_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      201 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_radiant/minimal/test_radiant_minimal_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       42 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_radiant/radiantc.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      704 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_radiant/test_radiant_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      193 2023-04-10 13:36:26.000000 edalize-0.5.1/tests/test_radiant/test_radiant_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1384 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_radiant.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.193882 edalize-0.5.1/tests/test_reporting/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.194882 edalize-0.5.1/tests/test_reporting/data/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.194882 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.310881 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/
+-rw-r--r--   0 olof      (1000) olof      (1000)   730139 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/top_timing.rpt
+-rw-r--r--   0 olof      (1000) olof      (1000)    10825 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/top_utilization_place.rpt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.312882 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/
+-rw-r--r--   0 olof      (1000) olof      (1000)   614846 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/top.fit.rpt
+-rw-r--r--   0 olof      (1000) olof      (1000)   212904 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/top.sta.rpt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.314881 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/
+-rw-r--r--   0 olof      (1000) olof      (1000)    76972 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/top.twr
+-rw-r--r--   0 olof      (1000) olof      (1000)    72356 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/top_map.mrp
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.314881 edalize-0.5.1/tests/test_reporting/data/picorv32/
+-rw-r--r--   0 olof      (1000) olof      (1000)      720 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/README.md
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.315882 edalize-0.5.1/tests/test_reporting/data/picorv32/ise-spartan6/
+-rw-r--r--   0 olof      (1000) olof      (1000)    35151 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/ise-spartan6/top.twr
+-rw-r--r--   0 olof      (1000) olof      (1000)    21326 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/ise-spartan6/top_map.mrp
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.316882 edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone10/
+-rw-r--r--   0 olof      (1000) olof      (1000)   216939 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone10/picorv32_wrap_0_1.fit.rpt
+-rw-r--r--   0 olof      (1000) olof      (1000)    26320 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone10/picorv32_wrap_0_1.sta.rpt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.317881 edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone4/
+-rw-r--r--   0 olof      (1000) olof      (1000)   150697 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone4/picorv32_wrap_0_1.fit.rpt
+-rw-r--r--   0 olof      (1000) olof      (1000)   142009 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone4/picorv32_wrap_0_1.sta.rpt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.194882 edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-artix7/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.319882 edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-artix7/impl/
+-rw-r--r--   0 olof      (1000) olof      (1000)    99238 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-artix7/impl/top_timing_summary_routed.rpt
+-rw-r--r--   0 olof      (1000) olof      (1000)     9783 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-artix7/impl/top_utilization_placed.rpt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.195882 edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-kintex_usp/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.320881 edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/
+-rw-r--r--   0 olof      (1000) olof      (1000)   102752 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/top_timing_summary_routed.rpt
+-rw-r--r--   0 olof      (1000) olof      (1000)    10698 2021-01-26 21:20:02.000000 edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/top_utilization_placed.rpt
+-rw-r--r--   0 olof      (1000) olof      (1000)    20571 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_reporting.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.321881 edalize-0.5.1/tests/test_rivierapro/
+-rw-r--r--   0 olof      (1000) olof      (1000)      732 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_rivierapro/edalize_build_rtl.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      125 2018-05-09 20:12:54.000000 edalize-0.5.1/tests/test_rivierapro/edalize_build_vpi.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      146 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_rivierapro/edalize_launch.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       41 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_rivierapro/edalize_main.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       36 2018-05-13 18:01:33.000000 edalize-0.5.1/tests/test_rivierapro/edalize_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       33 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_rivierapro/vsim.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       30 2018-05-13 18:01:37.000000 edalize-0.5.1/tests/test_rivierapro/vsim2.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      964 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_rivierapro.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.195882 edalize-0.5.1/tests/test_slang/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.321881 edalize-0.5.1/tests/test_slang/lint/
+-rw-r--r--   0 olof      (1000) olof      (1000)      219 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_slang/lint/slang.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.322882 edalize-0.5.1/tests/test_slang/preprocess/
+-rw-r--r--   0 olof      (1000) olof      (1000)      220 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_slang/preprocess/slang.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.322882 edalize-0.5.1/tests/test_slang/slang_options/
+-rw-r--r--   0 olof      (1000) olof      (1000)      219 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_slang/slang_options/slang.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1262 2023-02-28 12:38:03.000000 edalize-0.5.1/tests/test_slang.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.196882 edalize-0.5.1/tests/test_spyglass/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.323881 edalize-0.5.1/tests/test_spyglass/defaults/
+-rw-r--r--   0 olof      (1000) olof      (1000)      307 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/defaults/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      581 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/defaults/spyglass-run-design_read.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      583 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/defaults/spyglass-run-lint_lint_rtl.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      583 2018-11-27 22:35:12.000000 edalize-0.5.1/tests/test_spyglass/defaults/spyglass-run-some_othergoal.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      118 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/defaults/spyglass.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1262 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/defaults/test_spyglass_0.prj
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.325882 edalize-0.5.1/tests/test_spyglass/tooloptions/
+-rw-r--r--   0 olof      (1000) olof      (1000)      428 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/tooloptions/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      581 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/tooloptions/spyglass-run-design_read.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      583 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/tooloptions/spyglass-run-lint_lint_rtl.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      584 2020-04-23 21:14:25.000000 edalize-0.5.1/tests/test_spyglass/tooloptions/spyglass-run-some_othergoal.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      179 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/tooloptions/spyglass.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1345 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_spyglass/tooloptions/test_spyglass_0.prj
+-rw-r--r--   0 olof      (1000) olof      (1000)     1195 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_spyglass.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.196882 edalize-0.5.1/tests/test_symbiflow/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.196882 edalize-0.5.1/tests/test_symbiflow/nextpnr/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.325882 edalize-0.5.1/tests/test_symbiflow/nextpnr/fpga_interchange/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1777 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_symbiflow/nextpnr/fpga_interchange/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      529 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_symbiflow/nextpnr/fpga_interchange/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      239 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_symbiflow/nextpnr/fpga_interchange/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.326882 edalize-0.5.1/tests/test_symbiflow/nextpnr/xilinx/
+-rw-r--r--   0 olof      (1000) olof      (1000)      772 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_symbiflow/nextpnr/xilinx/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      519 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_symbiflow/nextpnr/xilinx/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      229 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_symbiflow/nextpnr/xilinx/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.326882 edalize-0.5.1/tests/test_symbiflow/vtr/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1141 2023-04-10 13:36:44.000000 edalize-0.5.1/tests/test_symbiflow/vtr/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)     2919 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_symbiflow.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.327881 edalize-0.5.1/tests/test_symbiyosys/
+-rw-r--r--   0 olof      (1000) olof      (1000)      195 2020-09-07 21:04:53.000000 edalize-0.5.1/tests/test_symbiyosys/config.sby.j2
+-rw-r--r--   0 olof      (1000) olof      (1000)       56 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_symbiyosys/files.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)        2 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_symbiyosys/incdirs.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)       30 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_symbiyosys/sby.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      668 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_symbiyosys/test.sby
+-rw-r--r--   0 olof      (1000) olof      (1000)     1160 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_symbiyosys.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      679 2023-04-18 17:27:33.000000 edalize-0.5.1/tests/test_tool_icarus.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1019 2023-03-31 23:11:32.000000 edalize-0.5.1/tests/test_tool_icepack.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      249 2023-04-10 13:47:28.000000 edalize-0.5.1/tests/test_tool_verilator.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      917 2023-03-24 22:06:41.000000 edalize-0.5.1/tests/test_tool_vivado.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1957 2023-03-31 23:11:32.000000 edalize-0.5.1/tests/test_tool_yosys.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.328881 edalize-0.5.1/tests/test_trellis/
+-rw-r--r--   0 olof      (1000) olof      (1000)      689 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       66 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/ecppack.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      694 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      212 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.330881 edalize-0.5.1/tests/test_trellis/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      607 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       66 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/minimal/ecppack.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      306 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/minimal/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      212 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/minimal/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       71 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/minimal/nextpnr-ecp5.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/minimal/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      112 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/nextpnr-ecp5.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_trellis/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1301 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_trellis.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.198882 edalize-0.5.1/tests/test_vcs/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.331881 edalize-0.5.1/tests/test_vcs/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      234 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       11 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/minimal/run.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/minimal/test_vcs_minimal_0.scr
+-rw-r--r--   0 olof      (1000) olof      (1000)       65 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/minimal/vcs.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.331881 edalize-0.5.1/tests/test_vcs/no_tool_options/
+-rw-r--r--   0 olof      (1000) olof      (1000)      247 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/no_tool_options/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       60 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/no_tool_options/run.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      282 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/no_tool_options/test_vcs_0.scr
+-rw-r--r--   0 olof      (1000) olof      (1000)       66 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/no_tool_options/vcs.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.333881 edalize-0.5.1/tests/test_vcs/tool_options/
+-rw-r--r--   0 olof      (1000) olof      (1000)      383 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/tool_options/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)       70 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/tool_options/run.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      282 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/tool_options/test_vcs_tool_options_0.scr
+-rw-r--r--   0 olof      (1000) olof      (1000)      127 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vcs/tool_options/vcs.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1520 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_vcs.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.198882 edalize-0.5.1/tests/test_veribleformat/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.333881 edalize-0.5.1/tests/test_veribleformat/default/
+-rw-r--r--   0 olof      (1000) olof      (1000)       56 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_veribleformat/default/verible-verilog-format.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      434 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_veribleformat.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.198882 edalize-0.5.1/tests/test_veriblelint/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.333881 edalize-0.5.1/tests/test_veriblelint/lint/
+-rw-r--r--   0 olof      (1000) olof      (1000)      484 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_veriblelint/lint/verible-verilog-lint.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      423 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_veriblelint.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.334881 edalize-0.5.1/tests/test_verilator/
+-rw-r--r--   0 olof      (1000) olof      (1000)      361 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_verilator/Makefile
+-rwxr-xr-x   0 olof      (1000) olof      (1000)       30 2020-03-16 21:28:04.000000 edalize-0.5.1/tests/test_verilator/Vtop_module
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.335882 edalize-0.5.1/tests/test_verilator/cc/
+-rw-r--r--   0 olof      (1000) olof      (1000)      175 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_verilator/cc/config.mk
+-rw-r--r--   0 olof      (1000) olof      (1000)      286 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_verilator/cc/test_verilator_0.vc
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.336881 edalize-0.5.1/tests/test_verilator/lint-only/
+-rw-r--r--   0 olof      (1000) olof      (1000)      145 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_verilator/lint-only/config.mk
+-rw-r--r--   0 olof      (1000) olof      (1000)      151 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_verilator/lint-only/test_verilator_0.vc
+-rw-r--r--   0 olof      (1000) olof      (1000)      114 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_verilator/run.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.336881 edalize-0.5.1/tests/test_verilator/sc/
+-rw-r--r--   0 olof      (1000) olof      (1000)      145 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_verilator/sc/config.mk
+-rw-r--r--   0 olof      (1000) olof      (1000)      144 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_verilator/sc/test_verilator_0.vc
+-rw-r--r--   0 olof      (1000) olof      (1000)     1262 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_verilator.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.339882 edalize-0.5.1/tests/test_vivado/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1159 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/Makefile
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.343881 edalize-0.5.1/tests/test_vivado/board_file/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1159 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/board_file/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)     1966 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/board_file/test_vivado_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/board_file/test_vivado_0_pgm.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/board_file/test_vivado_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/board_file/test_vivado_0_synth.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      203 2022-06-11 20:28:55.000000 edalize-0.5.1/tests/test_vivado/board_file/test_vivado_minimal_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2022-06-11 20:28:55.000000 edalize-0.5.1/tests/test_vivado/board_file/test_vivado_minimal_0_pgm.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1619 2022-06-11 20:28:55.000000 edalize-0.5.1/tests/test_vivado/board_file/test_vivado_minimal_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      142 2022-06-11 20:28:55.000000 edalize-0.5.1/tests/test_vivado/board_file/test_vivado_minimal_0_synth.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      140 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/board_file/vivado.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.344881 edalize-0.5.1/tests/test_vivado/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1207 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      203 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/minimal/test_vivado_minimal_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/minimal/test_vivado_minimal_0_pgm.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/minimal/test_vivado_minimal_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/minimal/test_vivado_minimal_0_synth.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      172 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/minimal/vivado.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1721 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/test_vivado_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/test_vivado_0_pgm.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/test_vivado_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/test_vivado_0_synth.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      140 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/vivado.cmd
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.346881 edalize-0.5.1/tests/test_vivado/yosys/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1033 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/yosys/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      331 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/yosys/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      243 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/yosys/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      295 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/yosys/test_vivado_yosys_0.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/yosys/test_vivado_yosys_0_pgm.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/yosys/test_vivado_yosys_0_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      164 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/yosys/vivado.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)       47 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vivado/yosys/yosys.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     2726 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_vivado.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.200882 edalize-0.5.1/tests/test_vpr/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.346881 edalize-0.5.1/tests/test_vpr/vpr/
+-rw-r--r--   0 olof      (1000) olof      (1000)      771 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vpr/vpr/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      948 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_vpr.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.346881 edalize-0.5.1/tests/test_vunit/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.347881 edalize-0.5.1/tests/test_vunit/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      534 2019-11-26 22:04:06.000000 edalize-0.5.1/tests/test_vunit/minimal/tb_minimal.vhd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1485 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_vunit/run.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.200882 edalize-0.5.1/tests/test_vunit/vunit_mock/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.347881 edalize-0.5.1/tests/test_vunit/vunit_mock/vunit/
+-rw-r--r--   0 olof      (1000) olof      (1000)       67 2019-11-26 22:04:06.000000 edalize-0.5.1/tests/test_vunit/vunit_mock/vunit/__init__.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      326 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/test_vunit/vunit_mock/vunit/ui.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      122 2021-12-20 23:32:01.000000 edalize-0.5.1/tests/test_vunit/vunit_mock/vunit/vhdl_standard.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     3556 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_vunit.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.348881 edalize-0.5.1/tests/test_xcelium/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1041 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_xcelium/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      795 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_xcelium/edalize_build_rtl.f
+-rw-r--r--   0 olof      (1000) olof      (1000)       43 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/test_xcelium/edalize_main.f
+-rw-r--r--   0 olof      (1000) olof      (1000)      228 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xcelium/xrun.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1232 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_xcelium.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.349882 edalize-0.5.1/tests/test_xsim/
+-rw-r--r--   0 olof      (1000) olof      (1000)      398 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xsim/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      489 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xsim/config.mk
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.350881 edalize-0.5.1/tests/test_xsim/mfc/
+-rw-r--r--   0 olof      (1000) olof      (1000)      398 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xsim/mfc/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      489 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xsim/mfc/config.mk
+-rw-r--r--   0 olof      (1000) olof      (1000)      162 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xsim/mfc/test_xsim_0.prj
+-rw-r--r--   0 olof      (1000) olof      (1000)      348 2021-01-26 20:36:10.000000 edalize-0.5.1/tests/test_xsim/mfc/xelab.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      127 2021-01-26 20:36:10.000000 edalize-0.5.1/tests/test_xsim/mfc/xsim.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      171 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xsim/test_xsim_0.prj
+-rw-r--r--   0 olof      (1000) olof      (1000)      348 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xsim/xelab.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)      127 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_xsim/xsim.cmd
+-rw-r--r--   0 olof      (1000) olof      (1000)     1610 2022-07-11 20:19:55.000000 edalize-0.5.1/tests/test_xsim.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.201882 edalize-0.5.1/tests/test_yosys/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.351881 edalize-0.5.1/tests/test_yosys/custom_output_name/
+-rw-r--r--   0 olof      (1000) olof      (1000)      158 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_yosys/custom_output_name/Makefile
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.351881 edalize-0.5.1/tests/test_yosys/default_output_name/
+-rw-r--r--   0 olof      (1000) olof      (1000)      174 2023-04-10 13:36:46.000000 edalize-0.5.1/tests/test_yosys/default_output_name/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      580 2023-03-06 16:31:40.000000 edalize-0.5.1/tests/test_yosys.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.202882 edalize-0.5.1/tests/tools/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.351881 edalize-0.5.1/tests/tools/icarus/
+-rw-r--r--   0 olof      (1000) olof      (1000)      310 2023-04-18 17:27:55.000000 edalize-0.5.1/tests/tools/icarus/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      281 2023-04-18 17:27:55.000000 edalize-0.5.1/tests/tools/icarus/design.scr
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.352882 edalize-0.5.1/tests/tools/icarus/multitop/
+-rw-r--r--   0 olof      (1000) olof      (1000)      271 2023-04-18 17:27:55.000000 edalize-0.5.1/tests/tools/icarus/multitop/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      355 2023-04-18 17:27:55.000000 edalize-0.5.1/tests/tools/icarus/multitop/design.scr
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.352882 edalize-0.5.1/tests/tools/icepack/
+-rw-r--r--   0 olof      (1000) olof      (1000)      129 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/icepack/Makefile
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.352882 edalize-0.5.1/tests/tools/verilator/
+-rw-r--r--   0 olof      (1000) olof      (1000)      280 2023-04-10 13:48:38.000000 edalize-0.5.1/tests/tools/verilator/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      272 2023-04-10 13:48:38.000000 edalize-0.5.1/tests/tools/verilator/design.vc
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.354881 edalize-0.5.1/tests/tools/vivado/
+-rw-r--r--   0 olof      (1000) olof      (1000)      865 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)     1564 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/design.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       84 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/design_netlist.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/design_pgm.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/design_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/design_synth.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.355881 edalize-0.5.1/tests/tools/vivado/tags/
+-rw-r--r--   0 olof      (1000) olof      (1000)      877 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/tags/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)     1768 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/tags/design.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       84 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/tags/design_netlist.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     3142 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/tags/design_pgm.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)     1589 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/tags/design_run.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/vivado/tags/design_synth.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.203882 edalize-0.5.1/tests/tools/yosys/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.356881 edalize-0.5.1/tests/tools/yosys/ecp5-blif/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-blif/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      712 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-blif/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-blif/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.357881 edalize-0.5.1/tests/tools/yosys/ecp5-edif/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-edif/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      712 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-edif/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-edif/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.358881 edalize-0.5.1/tests/tools/yosys/ecp5-json/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-json/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      712 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-json/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-json/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.358881 edalize-0.5.1/tests/tools/yosys/ecp5-verilog/
+-rw-r--r--   0 olof      (1000) olof      (1000)      238 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-verilog/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      712 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-verilog/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ecp5-verilog/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.359881 edalize-0.5.1/tests/tools/yosys/ice40-blif/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-blif/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      713 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-blif/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-blif/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.360881 edalize-0.5.1/tests/tools/yosys/ice40-edif/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-edif/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      713 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-edif/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-edif/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.361881 edalize-0.5.1/tests/tools/yosys/ice40-json/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-json/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      713 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-json/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-json/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.361881 edalize-0.5.1/tests/tools/yosys/ice40-verilog/
+-rw-r--r--   0 olof      (1000) olof      (1000)      238 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-verilog/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      713 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-verilog/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/ice40-verilog/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.362882 edalize-0.5.1/tests/tools/yosys/minimal/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/minimal/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      689 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/minimal/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/minimal/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.363881 edalize-0.5.1/tests/tools/yosys/template/
+-rw-r--r--   0 olof      (1000) olof      (1000)      218 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/template/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      689 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/template/edalize_yosys_procs.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.363881 edalize-0.5.1/tests/tools/yosys/xilinx-blif/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-blif/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      714 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-blif/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-blif/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.364881 edalize-0.5.1/tests/tools/yosys/xilinx-edif/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-edif/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      714 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-edif/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      243 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-edif/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.365881 edalize-0.5.1/tests/tools/yosys/xilinx-json/
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-json/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      714 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-json/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-json/edalize_yosys_template.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-05-17 08:31:29.365881 edalize-0.5.1/tests/tools/yosys/xilinx-verilog/
+-rw-r--r--   0 olof      (1000) olof      (1000)      238 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-verilog/Makefile
+-rw-r--r--   0 olof      (1000) olof      (1000)      714 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-verilog/edalize_yosys_procs.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)      230 2023-04-10 13:36:45.000000 edalize-0.5.1/tests/tools/yosys/xilinx-verilog/edalize_yosys_template.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)       92 2021-01-26 21:20:02.000000 edalize-0.5.1/tox.ini
```

### Comparing `edalize-0.5.0/.github/workflows/ci.yml` & `edalize-0.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/LICENSE` & `edalize-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/NEWS` & `edalize-0.5.1/NEWS`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+0.5.1 2023-05-17 Olof Kindgren
+======================================================
+* yosys: Fix yosys_template option
+* verilator: Fix dependencies on testbench files
+* icarus: Add missing vvp_options
+* Remove filelist backend
+* vivado: Add programming option
+
 0.5.0 2023-03-24 Olof Kindgren
 ======================================================
 * New flows: generic, gate-level simulation
 * New backends: filelist, sandpipersaas, openroad
 * modelsim: Support mfcu mode
 * icarus: Support multiple toplevels
 * yosys : Support verilog output and simulation tag
```

### Comparing `edalize-0.5.0/PKG-INFO` & `edalize-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edalize
-Version: 0.5.0
+Version: 0.5.1
 Summary: Library for interfacing EDA tools such as simulators, linters or synthesis tools, using a common interface
 Home-page: https://github.com/olofk/edalize
 Author: Olof Kindgren
 Author-email: olof.kindgren@gmail.com
 License: BSD-2-Clause
 Keywords: VHDL,verilog,EDA,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `edalize-0.5.0/README.rst` & `edalize-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/doc/Makefile` & `edalize-0.5.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/doc/conf.py` & `edalize-0.5.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/doc/dev/extend.rst` & `edalize-0.5.1/doc/dev/extend.rst`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/doc/dev/setup.rst` & `edalize-0.5.1/doc/dev/setup.rst`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/doc/edalize.rst` & `edalize-0.5.1/doc/edalize.rst`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/doc/edam/api.rst` & `edalize-0.5.1/doc/edam/api.rst`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/doc/index.rst` & `edalize-0.5.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/doc/make.bat` & `edalize-0.5.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/apicula.py` & `edalize-0.5.1/edalize/apicula.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/ascentlint.py` & `edalize-0.5.1/edalize/ascentlint.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/diamond.py` & `edalize-0.5.1/edalize/diamond.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/edatool.py` & `edalize-0.5.1/edalize/edatool.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/f4pga.py` & `edalize-0.5.1/edalize/f4pga.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/flows/edaflow.py` & `edalize-0.5.1/edalize/flows/edaflow.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/flows/f4pga.py` & `edalize-0.5.1/edalize/flows/f4pga.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/flows/generic.py` & `edalize-0.5.1/edalize/flows/generic.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/flows/gls.py` & `edalize-0.5.1/edalize/flows/gls.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/flows/icestorm.py` & `edalize-0.5.1/edalize/flows/icestorm.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/flows/sim.py` & `edalize-0.5.1/edalize/flows/sim.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/flows/vivado.py` & `edalize-0.5.1/edalize/flows/vivado.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 
     FLOW_OPTIONS = {
         "frontends": {
             "type": "str",
             "desc": "Tools to run before yosys (e.g. sv2v)",
             "list": True,
         },
+        "pgm": {
+            "type": "bool",
+            "desc": "Program board after bitstream is complete",
+        },
         "pnr": {
             "type": "str",
             "desc": "Select Place & Route tool.",
         },
         "synth": {
             "type": "str",
             "desc": "Synthesis tool. Allowed values are vivado (default) and yosys.",
@@ -59,7 +63,15 @@
             flow["vivado"] = {"deps": ["yosys"], "fdto": {"synth": "none"}}
         else:
             flow["vivado"] = {"deps": deps}
 
         name = self.edam["name"]
         self.commands.set_default_target(name + ".bit")
         return FlowGraph.fromdict(flow)
+
+    def run(self):
+        if self.flow_options.get("pgm"):
+
+            # Get run command from tool instance
+            vivado_inst = self.flow.get_node("vivado").inst
+            (cmd, args, cwd) = vivado_inst.run()
+            self._run_tool(cmd, args=args, cwd=cwd)
```

### Comparing `edalize-0.5.0/edalize/flows/vpr.py` & `edalize-0.5.1/edalize/flows/vpr.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/gatemate.py` & `edalize-0.5.1/edalize/gatemate.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/ghdl.py` & `edalize-0.5.1/edalize/ghdl.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/icarus.py` & `edalize-0.5.1/edalize/icarus.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/icestorm.py` & `edalize-0.5.1/edalize/icestorm.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/ise.py` & `edalize-0.5.1/edalize/ise.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/ise_reporting.py` & `edalize-0.5.1/edalize/ise_reporting.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/isim.py` & `edalize-0.5.1/edalize/isim.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/libero.py` & `edalize-0.5.1/edalize/libero.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/mistral.py` & `edalize-0.5.1/edalize/mistral.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/modelsim.py` & `edalize-0.5.1/edalize/modelsim.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/morty.py` & `edalize-0.5.1/edalize/morty.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/nextpnr.py` & `edalize-0.5.1/edalize/nextpnr.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/openfpga.py` & `edalize-0.5.1/edalize/openfpga.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/openlane.py` & `edalize-0.5.1/edalize/openlane.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/openroad.py` & `edalize-0.5.1/edalize/openroad.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/oxide.py` & `edalize-0.5.1/edalize/oxide.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/quartus.py` & `edalize-0.5.1/edalize/quartus.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/quartus_reporting.py` & `edalize-0.5.1/edalize/quartus_reporting.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/questaformal.py` & `edalize-0.5.1/edalize/questaformal.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/radiant.py` & `edalize-0.5.1/edalize/radiant.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/reporting.py` & `edalize-0.5.1/edalize/reporting.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/rivierapro.py` & `edalize-0.5.1/edalize/rivierapro.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/sandpipersaas.py` & `edalize-0.5.1/edalize/sandpipersaas.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/slang.py` & `edalize-0.5.1/edalize/slang.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/spyglass.py` & `edalize-0.5.1/edalize/spyglass.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/symbiflow.py` & `edalize-0.5.1/edalize/symbiflow.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/symbiyosys.py` & `edalize-0.5.1/edalize/symbiyosys.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/ascentlint/Makefile.j2` & `edalize-0.5.1/edalize/templates/ascentlint/Makefile.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/ghdl/Makefile.j2` & `edalize-0.5.1/edalize/templates/ghdl/Makefile.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/libero/libero-project.tcl.j2` & `edalize-0.5.1/edalize/templates/libero/libero-project.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/libero/libero-run.tcl.j2` & `edalize-0.5.1/edalize/templates/libero/libero-run.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/libero/libero-syn-user.tcl.j2` & `edalize-0.5.1/edalize/templates/libero/libero-syn-user.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/openfpga/task_simulation.conf.j2` & `edalize-0.5.1/edalize/templates/openfpga/task_simulation.conf.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/quartus/quartus-pro-makefile.j2` & `edalize-0.5.1/edalize/templates/quartus/quartus-pro-makefile.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/quartus/quartus-project.tcl.j2` & `edalize-0.5.1/edalize/templates/quartus/quartus-project.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/quartus/quartus-std-makefile.j2` & `edalize-0.5.1/edalize/templates/quartus/quartus-std-makefile.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/spyglass/spyglass-project.prj.j2` & `edalize-0.5.1/edalize/templates/spyglass/spyglass-project.prj.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/spyglass/spyglass-run-goal.tcl.j2` & `edalize-0.5.1/edalize/templates/spyglass/spyglass-run-goal.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/vivado/vivado-program.tcl.j2` & `edalize-0.5.1/edalize/templates/vivado/vivado-program.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/vivado/vivado-project.tcl.j2` & `edalize-0.5.1/edalize/templates/vivado/vivado-project.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/vivado/vivado-run.tcl.j2` & `edalize-0.5.1/edalize/templates/vivado/vivado-run.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/vunit/run.py.j2` & `edalize-0.5.1/edalize/templates/vunit/run.py.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/templates/yosys/edalize_yosys_procs.tcl.j2` & `edalize-0.5.1/edalize/templates/yosys/edalize_yosys_procs.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/edatool.py` & `edalize-0.5.1/edalize/tools/edatool.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/ghdl.py` & `edalize-0.5.1/edalize/tools/ghdl.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/icarus.py` & `edalize-0.5.1/edalize/tools/icarus.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,18 @@
             "type": "str",
             "desc": "Default timescale",
         },
         "iverilog_options": {
             "type": "str",
             "desc": "Additional options for iverilog",
         },
+        "vvp_options": {
+            "type": "str",
+            "desc": "Additional options for vvp",
+        },
     }
 
     def setup(self, edam):
         super().setup(edam)
 
         scr_file = StringIO()
         incdirs = []
@@ -96,15 +100,17 @@
             [self.name],
             depfiles + [f"{self.name}.scr"],
         )
 
         # How should the run target be handled?
         # Add VPI support
         commands.add(
-            ["vvp", "-n", "-M.", self.name, "-fst", "$(EXTRA_OPTIONS)"],
+            ["vvp", "-n", "-M."]
+            + self.tool_options.get("vvp_options", [])
+            + [self.name, "-fst", "$(EXTRA_OPTIONS)"],
             ["run"],
             [self.name],
         )
 
         commands.set_default_target(self.name)
         self.commands = commands
         self.scr_file = scr_file
```

### Comparing `edalize-0.5.0/edalize/tools/icepack.py` & `edalize-0.5.1/edalize/tools/icepack.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/icetime.py` & `edalize-0.5.1/edalize/tools/icetime.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/ipxact2v.py` & `edalize-0.5.1/edalize/tools/ipxact2v.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/nextpnr.py` & `edalize-0.5.1/edalize/tools/nextpnr.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/surelog.py` & `edalize-0.5.1/edalize/tools/surelog.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/sv2v.py` & `edalize-0.5.1/edalize/tools/sv2v.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/templates/vivado/vivado-program.tcl.j2` & `edalize-0.5.1/edalize/tools/templates/vivado/vivado-program.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/templates/vivado/vivado-project.tcl.j2` & `edalize-0.5.1/edalize/tools/templates/vivado/vivado-project.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/templates/vivado/vivado-run.tcl.j2` & `edalize-0.5.1/edalize/tools/templates/vivado/vivado-run.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/templates/yosys/edalize_yosys_procs.tcl.j2` & `edalize-0.5.1/edalize/tools/templates/yosys/edalize_yosys_procs.tcl.j2`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/verilator.py` & `edalize-0.5.1/edalize/tools/verilator.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             depfile = True
             if file_type.startswith("systemVerilogSource") or file_type.startswith(
                 "verilogSource"
             ):
                 if not self._add_include_dir(f, incdirs):
                     vlog_files.append(f["name"])
             elif file_type in ["cppSource", "systemCSource", "cSource"]:
+                depfile = False
                 if not self._add_include_dir(f, incdirs):
                     opt_c_files.append(f["name"])
             elif file_type == "vlt":
                 vlt_files.append(f["name"])
             elif file_type == "uhdm":
                 uhdm_files.append(f["name"])
             else:
@@ -105,15 +106,15 @@
         vc += opt_c_files
 
         for k, v in self.vlogparam.items():
             vc.append(
                 "-G{}={}".format(k, self._param_value_str(v, str_quote_style='\\"'))
             )
         for k, v in self.vlogdefine.items():
-            vc.append("-D{}={}\n".format(k, self._param_value_str(v)))
+            vc.append("-D{}={}".format(k, self._param_value_str(v)))
 
         self.vc = vc
 
         mk_file = f"V{self.toplevel}.mk"
         exe_file = f"V{self.toplevel}"
         commands = EdaCommands()
         commands.add(
@@ -124,15 +125,15 @@
 
         if mode == "lint-only":
             commands.set_default_target(mk_file)
         else:
             commands.add(
                 ["make", "-f", mk_file] + self.tool_options.get("make_options", []),
                 [exe_file],
-                [mk_file],
+                [mk_file] + opt_c_files,
             )
             commands.set_default_target(exe_file)
 
         self.commands = commands
 
     def write_config_files(self):
         self.update_config_file(self.name + ".vc", "\n".join(self.vc) + "\n")
```

### Comparing `edalize-0.5.0/edalize/tools/vivado.py` & `edalize-0.5.1/edalize/tools/vivado.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/vpr.py` & `edalize-0.5.1/edalize/tools/vpr.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/tools/yosys.py` & `edalize-0.5.1/edalize/tools/yosys.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,18 +181,17 @@
 
         commands.add(command, targets, depends, variables=variables)
         commands.set_default_target(targets[0])
         self.commands = commands
 
     def write_config_files(self):
         yosys_template = self.tool_options.get("yosys_template")
-        if not yosys_template:
-            self.render_template(
-                "edalize_yosys_procs.tcl.j2",
-                "edalize_yosys_procs.tcl",
-                self.template_vars,
-            )
+        self.render_template(
+            "edalize_yosys_procs.tcl.j2",
+            "edalize_yosys_procs.tcl",
+            self.template_vars,
+        )
 
         if not yosys_template:
             self.render_template(
                 "yosys-script-tcl.j2", "edalize_yosys_template.tcl", self.template_vars
             )
```

### Comparing `edalize-0.5.0/edalize/trellis.py` & `edalize-0.5.1/edalize/trellis.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/utils.py` & `edalize-0.5.1/edalize/utils.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/vcs.py` & `edalize-0.5.1/edalize/vcs.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/veribleformat.py` & `edalize-0.5.1/edalize/veribleformat.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/veriblelint.py` & `edalize-0.5.1/edalize/veriblelint.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/verilator.py` & `edalize-0.5.1/edalize/verilator.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/vivado.py` & `edalize-0.5.1/edalize/vivado.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/vivado_reporting.py` & `edalize-0.5.1/edalize/vivado_reporting.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/vpr.py` & `edalize-0.5.1/edalize/vpr.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/vunit.py` & `edalize-0.5.1/edalize/vunit.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/vunit_hooks.py` & `edalize-0.5.1/edalize/vunit_hooks.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/xcelium.py` & `edalize-0.5.1/edalize/xcelium.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/xsim.py` & `edalize-0.5.1/edalize/xsim.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize/yosys.py` & `edalize-0.5.1/edalize/yosys.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/edalize.egg-info/PKG-INFO` & `edalize-0.5.1/edalize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edalize
-Version: 0.5.0
+Version: 0.5.1
 Summary: Library for interfacing EDA tools such as simulators, linters or synthesis tools, using a common interface
 Home-page: https://github.com/olofk/edalize
 Author: Olof Kindgren
 Author-email: olof.kindgren@gmail.com
 License: BSD-2-Clause
 Keywords: VHDL,verilog,EDA,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `edalize-0.5.0/edalize.egg-info/SOURCES.txt` & `edalize-0.5.1/edalize.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 doc/user/index.rst
 doc/user/run.rst
 edalize/apicula.py
 edalize/ascentlint.py
 edalize/diamond.py
 edalize/edatool.py
 edalize/f4pga.py
-edalize/filelist.py
 edalize/gatemate.py
 edalize/ghdl.py
 edalize/icarus.py
 edalize/icestorm.py
 edalize/ise.py
 edalize/ise_reporting.py
 edalize/isim.py
@@ -111,14 +110,15 @@
 edalize/templates/yosys/yosys-script-tcl.j2
 edalize/tools/edatool.py
 edalize/tools/ghdl.py
 edalize/tools/icarus.py
 edalize/tools/icepack.py
 edalize/tools/icetime.py
 edalize/tools/ipxact2v.py
+edalize/tools/modelsim.py
 edalize/tools/nextpnr.py
 edalize/tools/surelog.py
 edalize/tools/sv2v.py
 edalize/tools/verilator.py
 edalize/tools/vivado.py
 edalize/tools/vpr.py
 edalize/tools/yosys.py
@@ -160,14 +160,16 @@
 tests/test_reporting.py
 tests/test_rivierapro.py
 tests/test_slang.py
 tests/test_spyglass.py
 tests/test_symbiflow.py
 tests/test_symbiyosys.py
 tests/test_tool_icarus.py
+tests/test_tool_icepack.py
+tests/test_tool_verilator.py
 tests/test_tool_vivado.py
 tests/test_tool_yosys.py
 tests/test_trellis.py
 tests/test_vcs.py
 tests/test_veribleformat.py
 tests/test_veriblelint.py
 tests/test_verilator.py
@@ -525,14 +527,17 @@
 tests/test_xsim/mfc/xsim.cmd
 tests/test_yosys/custom_output_name/Makefile
 tests/test_yosys/default_output_name/Makefile
 tests/tools/icarus/Makefile
 tests/tools/icarus/design.scr
 tests/tools/icarus/multitop/Makefile
 tests/tools/icarus/multitop/design.scr
+tests/tools/icepack/Makefile
+tests/tools/verilator/Makefile
+tests/tools/verilator/design.vc
 tests/tools/vivado/Makefile
 tests/tools/vivado/design.tcl
 tests/tools/vivado/design_netlist.tcl
 tests/tools/vivado/design_pgm.tcl
 tests/tools/vivado/design_run.tcl
 tests/tools/vivado/design_synth.tcl
 tests/tools/vivado/tags/Makefile
```

### Comparing `edalize-0.5.0/scripts/el_docker` & `edalize-0.5.1/scripts/el_docker`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/setup.py` & `edalize-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="edalize",
-    version="0.5.0",
+    version="0.5.1",
     packages=["edalize", "edalize.tools", "edalize.flows"],
     package_data={
         "edalize": [
             "templates/yosys/edalize_yosys_procs.tcl.j2",
             "templates/yosys/yosys-script-tcl.j2",
             "templates/openfpga/task_simulation.conf.j2",
             "templates/spyglass/Makefile.j2",
```

### Comparing `edalize-0.5.0/tests/README.rst` & `edalize-0.5.1/tests/README.rst`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/edalize_common.py` & `edalize-0.5.1/tests/edalize_common.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/edalize_flow_common.py` & `edalize-0.5.1/tests/edalize_flow_common.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/edalize_tool_common.py` & `edalize-0.5.1/tests/edalize_tool_common.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/flows/gls/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/flows/gls/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/mock_commands/ghdl` & `edalize-0.5.1/tests/mock_commands/ghdl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/mock_commands/quartus_sh` & `edalize-0.5.1/tests/mock_commands/quartus_sh`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/mock_commands/vcs` & `edalize-0.5.1/tests/mock_commands/vcs`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_apicula/Makefile` & `edalize-0.5.1/tests/test_apicula/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_apicula/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_apicula/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_apicula/minimal/Makefile` & `edalize-0.5.1/tests/test_apicula/minimal/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_apicula.py` & `edalize-0.5.1/tests/test_apicula.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_diamond/test_diamond_0.tcl` & `edalize-0.5.1/tests/test_diamond/test_diamond_0.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_diamond.py` & `edalize-0.5.1/tests/test_diamond.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_edam.py` & `edalize-0.5.1/tests/test_edam.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_gatemate/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_gatemate/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_gatemate.py` & `edalize-0.5.1/tests/test_gatemate.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_ghdl/test01/Makefile` & `edalize-0.5.1/tests/test_ghdl/test01/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_ghdl/test02/Makefile` & `edalize-0.5.1/tests/test_ghdl/test02/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_ghdl/test03/Makefile` & `edalize-0.5.1/tests/test_ghdl/test03/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_ghdl/test04/Makefile` & `edalize-0.5.1/tests/test_ghdl/test04/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_ghdl.py` & `edalize-0.5.1/tests/test_ghdl.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_icarus/Makefile` & `edalize-0.5.1/tests/test_icarus/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_icarus.py` & `edalize-0.5.1/tests/test_icarus.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_icestorm/Makefile` & `edalize-0.5.1/tests/test_icestorm/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_icestorm/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_icestorm/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_icestorm/minimal/Makefile` & `edalize-0.5.1/tests/test_icestorm/minimal/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_icestorm/nextpnr/Makefile` & `edalize-0.5.1/tests/test_icestorm/nextpnr/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_icestorm/nextpnr/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_icestorm/nextpnr/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_icestorm.py` & `edalize-0.5.1/tests/test_icestorm.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_ise/test_ise_0.tcl` & `edalize-0.5.1/tests/test_ise/test_ise_0.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_ise.py` & `edalize-0.5.1/tests/test_ise.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_libero/libero-test-all-project.tcl` & `edalize-0.5.1/tests/test_libero/libero-test-all-project.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_libero/libero-test-all-run.tcl` & `edalize-0.5.1/tests/test_libero/libero-test-all-run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_libero/libero-test-project.tcl` & `edalize-0.5.1/tests/test_libero/libero-test-project.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_libero/libero-test-run.tcl` & `edalize-0.5.1/tests/test_libero/libero-test-run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_libero.py` & `edalize-0.5.1/tests/test_libero.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_mistral/Makefile` & `edalize-0.5.1/tests/test_mistral/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_mistral/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_mistral/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_mistral.py` & `edalize-0.5.1/tests/test_mistral.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_modelsim/Makefile` & `edalize-0.5.1/tests/test_modelsim/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_modelsim/common_compilation/Makefile` & `edalize-0.5.1/tests/test_modelsim/common_compilation/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_modelsim/edalize_build_rtl.tcl` & `edalize-0.5.1/tests/test_modelsim/edalize_build_rtl.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_modelsim.py` & `edalize-0.5.1/tests/test_modelsim.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_openfpga/config/task.conf` & `edalize-0.5.1/tests/test_openfpga/config/task.conf`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_openfpga.py` & `edalize-0.5.1/tests/test_openfpga.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_oxide/Makefile` & `edalize-0.5.1/tests/test_oxide/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_oxide/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_oxide/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_oxide/minimal/Makefile` & `edalize-0.5.1/tests/test_oxide/minimal/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_oxide.py` & `edalize-0.5.1/tests/test_oxide.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_plugin/edalize/testplugin.py` & `edalize-0.5.1/tests/test_plugin/edalize/testplugin.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_plugin/edalize/tools/customtool.py` & `edalize-0.5.1/tests/test_plugin/edalize/tools/customtool.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_plugin.py` & `edalize-0.5.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_quartus/Pro/Makefile` & `edalize-0.5.1/tests/test_quartus/Pro/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_quartus/Pro/test_quartus_0.tcl` & `edalize-0.5.1/tests/test_quartus/Pro/test_quartus_0.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_quartus/Standard/Makefile` & `edalize-0.5.1/tests/test_quartus/Standard/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_quartus/Standard/test_quartus_0.tcl` & `edalize-0.5.1/tests/test_quartus/Standard/test_quartus_0.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_quartus.py` & `edalize-0.5.1/tests/test_quartus.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_questa_formal.py` & `edalize-0.5.1/tests/test_questa_formal.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_questaformal/edalize_build_rtl.tcl` & `edalize-0.5.1/tests/test_questaformal/edalize_build_rtl.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_radiant/test_radiant_0.tcl` & `edalize-0.5.1/tests/test_radiant/test_radiant_0.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_radiant.py` & `edalize-0.5.1/tests/test_radiant.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/top_timing.rpt` & `edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/top_timing.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/top_utilization_place.rpt` & `edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/arty_a7/top_utilization_place.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/top.fit.rpt` & `edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/top.fit.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/top.sta.rpt` & `edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/de10nano/top.sta.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/top.twr` & `edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/top.twr`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/top_map.mrp` & `edalize-0.5.1/tests/test_reporting/data/linux-on-litex-vexriscv/pipistrello/top_map.mrp`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/README.md` & `edalize-0.5.1/tests/test_reporting/data/picorv32/README.md`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/ise-spartan6/top.twr` & `edalize-0.5.1/tests/test_reporting/data/picorv32/ise-spartan6/top.twr`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/ise-spartan6/top_map.mrp` & `edalize-0.5.1/tests/test_reporting/data/picorv32/ise-spartan6/top_map.mrp`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone10/picorv32_wrap_0_1.fit.rpt` & `edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone10/picorv32_wrap_0_1.fit.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone10/picorv32_wrap_0_1.sta.rpt` & `edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone10/picorv32_wrap_0_1.sta.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone4/picorv32_wrap_0_1.fit.rpt` & `edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone4/picorv32_wrap_0_1.fit.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/quartus-cyclone4/picorv32_wrap_0_1.sta.rpt` & `edalize-0.5.1/tests/test_reporting/data/picorv32/quartus-cyclone4/picorv32_wrap_0_1.sta.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-artix7/impl/top_timing_summary_routed.rpt` & `edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-artix7/impl/top_timing_summary_routed.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-artix7/impl/top_utilization_placed.rpt` & `edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-artix7/impl/top_utilization_placed.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/top_timing_summary_routed.rpt` & `edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/top_timing_summary_routed.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/top_utilization_placed.rpt` & `edalize-0.5.1/tests/test_reporting/data/picorv32/vivado-kintex_usp/impl/top_utilization_placed.rpt`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_reporting.py` & `edalize-0.5.1/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_rivierapro/edalize_build_rtl.tcl` & `edalize-0.5.1/tests/test_rivierapro/edalize_build_rtl.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_rivierapro.py` & `edalize-0.5.1/tests/test_rivierapro.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_slang.py` & `edalize-0.5.1/tests/test_slang.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass/defaults/spyglass-run-design_read.tcl` & `edalize-0.5.1/tests/test_spyglass/defaults/spyglass-run-design_read.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass/defaults/spyglass-run-lint_lint_rtl.tcl` & `edalize-0.5.1/tests/test_spyglass/defaults/spyglass-run-lint_lint_rtl.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass/defaults/spyglass-run-some_othergoal.tcl` & `edalize-0.5.1/tests/test_spyglass/defaults/spyglass-run-some_othergoal.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass/defaults/test_spyglass_0.prj` & `edalize-0.5.1/tests/test_spyglass/defaults/test_spyglass_0.prj`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass/tooloptions/spyglass-run-design_read.tcl` & `edalize-0.5.1/tests/test_spyglass/tooloptions/spyglass-run-design_read.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass/tooloptions/spyglass-run-lint_lint_rtl.tcl` & `edalize-0.5.1/tests/test_spyglass/tooloptions/spyglass-run-lint_lint_rtl.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass/tooloptions/spyglass-run-some_othergoal.tcl` & `edalize-0.5.1/tests/test_spyglass/tooloptions/spyglass-run-some_othergoal.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass/tooloptions/test_spyglass_0.prj` & `edalize-0.5.1/tests/test_spyglass/tooloptions/test_spyglass_0.prj`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_spyglass.py` & `edalize-0.5.1/tests/test_spyglass.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_symbiflow/nextpnr/fpga_interchange/Makefile` & `edalize-0.5.1/tests/test_symbiflow/nextpnr/fpga_interchange/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_symbiflow/nextpnr/fpga_interchange/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_symbiflow/nextpnr/fpga_interchange/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_symbiflow/nextpnr/xilinx/Makefile` & `edalize-0.5.1/tests/test_symbiflow/nextpnr/xilinx/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_symbiflow/nextpnr/xilinx/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_symbiflow/nextpnr/xilinx/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_symbiflow/vtr/Makefile` & `edalize-0.5.1/tests/test_symbiflow/vtr/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_symbiflow.py` & `edalize-0.5.1/tests/test_symbiflow.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_symbiyosys/test.sby` & `edalize-0.5.1/tests/test_symbiyosys/test.sby`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_symbiyosys.py` & `edalize-0.5.1/tests/test_symbiyosys.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_tool_vivado.py` & `edalize-0.5.1/tests/test_tool_vivado.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_tool_yosys.py` & `edalize-0.5.1/tests/test_tool_yosys.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,7 +46,19 @@
 
     tf = tool_fixture(
         "yosys", tool_options=tool_options, files=files, ref_subdir="minimal"
     )
 
     tf.tool.configure()
     tf.compare_config_files(["edalize_yosys_template.tcl", "edalize_yosys_procs.tcl"])
+
+
+def test_tool_yosys_template(tool_fixture):
+    import os
+
+    tool_options = {"arch": "ice40", "yosys_template": "some_file.tcl"}
+
+    tf = tool_fixture("yosys", tool_options=tool_options, ref_subdir="template")
+
+    tf.tool.configure()
+    tf.compare_config_files(["edalize_yosys_procs.tcl"])
+    assert not os.path.exists(tf.tool.work_root / "edalize_yosys_template.tcl")
```

### Comparing `edalize-0.5.0/tests/test_trellis/Makefile` & `edalize-0.5.1/tests/test_trellis/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_trellis/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/test_trellis/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_trellis/minimal/Makefile` & `edalize-0.5.1/tests/test_trellis/minimal/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_trellis.py` & `edalize-0.5.1/tests/test_trellis.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vcs.py` & `edalize-0.5.1/tests/test_vcs.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_verilator.py` & `edalize-0.5.1/tests/test_verilator.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/Makefile` & `edalize-0.5.1/tests/test_vivado/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/board_file/Makefile` & `edalize-0.5.1/tests/test_vivado/board_file/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/board_file/test_vivado_0.tcl` & `edalize-0.5.1/tests/test_vivado/board_file/test_vivado_0.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/board_file/test_vivado_0_pgm.tcl` & `edalize-0.5.1/tests/test_vivado/board_file/test_vivado_0_pgm.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/board_file/test_vivado_0_run.tcl` & `edalize-0.5.1/tests/test_vivado/board_file/test_vivado_0_run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/board_file/test_vivado_minimal_0_pgm.tcl` & `edalize-0.5.1/tests/test_vivado/board_file/test_vivado_minimal_0_pgm.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/board_file/test_vivado_minimal_0_run.tcl` & `edalize-0.5.1/tests/test_vivado/board_file/test_vivado_minimal_0_run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/minimal/Makefile` & `edalize-0.5.1/tests/test_vivado/minimal/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/minimal/test_vivado_minimal_0_pgm.tcl` & `edalize-0.5.1/tests/test_vivado/minimal/test_vivado_minimal_0_pgm.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/minimal/test_vivado_minimal_0_run.tcl` & `edalize-0.5.1/tests/test_vivado/minimal/test_vivado_minimal_0_run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/test_vivado_0.tcl` & `edalize-0.5.1/tests/test_vivado/test_vivado_0.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/test_vivado_0_pgm.tcl` & `edalize-0.5.1/tests/test_vivado/test_vivado_0_pgm.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/test_vivado_0_run.tcl` & `edalize-0.5.1/tests/test_vivado/test_vivado_0_run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/yosys/Makefile` & `edalize-0.5.1/tests/test_vivado/yosys/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/yosys/test_vivado_yosys_0_pgm.tcl` & `edalize-0.5.1/tests/test_vivado/yosys/test_vivado_yosys_0_pgm.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado/yosys/test_vivado_yosys_0_run.tcl` & `edalize-0.5.1/tests/test_vivado/yosys/test_vivado_yosys_0_run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vivado.py` & `edalize-0.5.1/tests/test_vivado.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vpr/vpr/Makefile` & `edalize-0.5.1/tests/test_vpr/vpr/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vpr.py` & `edalize-0.5.1/tests/test_vpr.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vunit/minimal/tb_minimal.vhd` & `edalize-0.5.1/tests/test_vunit/minimal/tb_minimal.vhd`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vunit/run.py` & `edalize-0.5.1/tests/test_vunit/run.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_vunit.py` & `edalize-0.5.1/tests/test_vunit.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_xcelium/Makefile` & `edalize-0.5.1/tests/test_xcelium/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_xcelium/edalize_build_rtl.f` & `edalize-0.5.1/tests/test_xcelium/edalize_build_rtl.f`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_xcelium.py` & `edalize-0.5.1/tests/test_xcelium.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_xsim.py` & `edalize-0.5.1/tests/test_xsim.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/test_yosys.py` & `edalize-0.5.1/tests/test_yosys.py`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/vivado/Makefile` & `edalize-0.5.1/tests/tools/vivado/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/vivado/design.tcl` & `edalize-0.5.1/tests/tools/vivado/design.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/vivado/design_pgm.tcl` & `edalize-0.5.1/tests/tools/vivado/design_pgm.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/vivado/design_run.tcl` & `edalize-0.5.1/tests/tools/vivado/design_run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/vivado/tags/Makefile` & `edalize-0.5.1/tests/tools/vivado/tags/Makefile`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/vivado/tags/design.tcl` & `edalize-0.5.1/tests/tools/vivado/tags/design.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/vivado/tags/design_pgm.tcl` & `edalize-0.5.1/tests/tools/vivado/tags/design_pgm.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/vivado/tags/design_run.tcl` & `edalize-0.5.1/tests/tools/vivado/tags/design_run.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/ecp5-blif/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/ecp5-blif/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/ecp5-edif/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/ecp5-edif/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/ecp5-json/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/ecp5-json/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/ecp5-verilog/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/ecp5-verilog/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/ice40-blif/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/ice40-blif/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/ice40-edif/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/ice40-edif/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/ice40-json/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/ice40-json/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/ice40-verilog/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/ice40-verilog/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/minimal/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/minimal/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/template/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/template/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/xilinx-blif/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/xilinx-blif/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/xilinx-edif/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/xilinx-edif/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/xilinx-json/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/xilinx-json/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

### Comparing `edalize-0.5.0/tests/tools/yosys/xilinx-verilog/edalize_yosys_procs.tcl` & `edalize-0.5.1/tests/tools/yosys/xilinx-verilog/edalize_yosys_procs.tcl`

 * *Files identical despite different names*

