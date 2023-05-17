# Comparing `tmp/nef_pipelines-0.1.38.tar.gz` & `tmp/nef_pipelines-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.38.tar", last modified: Sat May  6 21:01:46 2023, max compression
+gzip compressed data, was "nef_pipelines-0.1.39.tar", last modified: Tue May 16 10:03:16 2023, max compression
```

## Comparing `nef_pipelines-0.1.38.tar` & `nef_pipelines-0.1.39.tar`

### file list

```diff
@@ -1,366 +1,368 @@
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.171207 nef_pipelines-0.1.38/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:44.935970 nef_pipelines-0.1.38/.github/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.025175 nef_pipelines-0.1.38/.github/workflows/
--rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.38/.github/workflows/ci.yml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.043286 nef_pipelines-0.1.38/.idea/
--rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.38/.idea/.gitignore
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.38/.idea/.name
--rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.38/.idea/NFC.iml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.050392 nef_pipelines-0.1.38/.idea/inspectionProfiles/
--rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.38/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.38/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.38/.idea/modules.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.38/.idea/vcs.xml
--rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.38/.pre-commit-config.yaml
--rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.38/.readthedocs.yml
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.38/AUTHORS.md
--rw-r--r--   0 garythompson   (501) staff       (20)     3449 2023-05-06 21:00:36.000000 nef_pipelines-0.1.38/CHANGELOG.md
--rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.38/CONTRIBUTING.md
--rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.38/LICENSE.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-06 21:01:46.171784 nef_pipelines-0.1.38/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.38/README.md
--rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.38/TODO.md
--rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.38/pyproject.toml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.060018 nef_pipelines-0.1.38/references/
--rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.38/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.38/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.38/release_to_pypi.sh
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.38/requirements.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-05-06 21:01:46.176699 nef_pipelines-0.1.38/setup.cfg
--rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.38/setup.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:44.937801 nef_pipelines-0.1.38/src/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.080949 nef_pipelines-0.1.38/src/nef_pipelines/
--rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.38/src/nef_pipelines/VERSION
--rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.125773 nef_pipelines-0.1.38/src/nef_pipelines/data/
--rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.210481 nef_pipelines-0.1.38/src/nef_pipelines/lib/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16143 2023-04-15 16:57:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15051 2023-05-04 07:18:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    21187 2023-04-30 15:31:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4083 2023-05-04 07:17:17.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10234 2023-04-26 19:21:33.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.214172 nef_pipelines-0.1.38/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1049 2023-05-06 20:57:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/translation_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garythompson   (501) staff       (20)    22250 2023-04-17 20:19:05.000000 nef_pipelines-0.1.38/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5288 2023-05-06 20:58:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/main.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.214750 nef_pipelines-0.1.38/src/nef_pipelines/nef_app/
--rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.234775 nef_pipelines-0.1.38/src/nef_pipelines/tests/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.246964 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.252581 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.254075 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.258135 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.260577 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.263880 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_import_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.265031 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.270850 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.306073 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.310770 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_delete.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1123 2023-04-15 16:57:25.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_rename.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_tabulate.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.314581 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.337521 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.352620 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.406764 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.492861 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.541714 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.546386 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.551612 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.553516 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.585378 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.586647 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.589043 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.624615 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.679737 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4153 2023-05-04 20:25:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2305 2023-05-06 20:53:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.717273 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/header.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/test_test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.719578 nef_pipelines-0.1.38/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.733654 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.770664 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.798408 nef_pipelines-0.1.38/src/nef_pipelines/tools/
--rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.826900 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.834609 nef_pipelines-0.1.38/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.852593 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6996 2023-04-15 16:55:03.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.858711 nef_pipelines-0.1.38/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.862605 nef_pipelines-0.1.38/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7095 2023-04-26 16:43:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.865449 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.866205 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.873805 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.875599 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/
--rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.877932 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15615 2023-05-06 20:59:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/importers/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.883579 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.890425 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.894256 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.901099 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.913219 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.932653 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.941429 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.950577 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.959305 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.978678 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.994877 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.000877 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.011540 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    10961 2023-05-06 20:57:59.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.016721 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.018785 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.023576 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.035619 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.038668 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.049482 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.065195 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.071701 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-04 07:46:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.090210 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16125 2023-05-06 20:58:05.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-04-26 18:39:25.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8510 2023-05-06 14:33:01.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.093904 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.119815 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.130306 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.144091 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:46.169709 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-06 21:01:45.099802 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)    13928 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-05-06 21:01:44.000000 nef_pipelines-0.1.38/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.38/tox.ini
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.654550 nef_pipelines-0.1.39/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.257539 nef_pipelines-0.1.39/.github/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.400923 nef_pipelines-0.1.39/.github/workflows/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.39/.github/workflows/ci.yml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.427490 nef_pipelines-0.1.39/.idea/
+-rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.39/.idea/.gitignore
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.39/.idea/.name
+-rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.39/.idea/NFC.iml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.440363 nef_pipelines-0.1.39/.idea/inspectionProfiles/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.39/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.39/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.39/.idea/modules.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.39/.idea/vcs.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.39/.pre-commit-config.yaml
+-rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.39/.readthedocs.yml
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.39/AUTHORS.md
+-rw-r--r--   0 garythompson   (501) staff       (20)     3525 2023-05-16 10:02:27.000000 nef_pipelines-0.1.39/CHANGELOG.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.39/CONTRIBUTING.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.39/LICENSE.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-16 10:03:16.654852 nef_pipelines-0.1.39/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.39/README.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.39/TODO.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.39/pyproject.toml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.449967 nef_pipelines-0.1.39/references/
+-rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.39/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.39/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.39/release_to_pypi.sh
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.39/requirements.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-05-16 10:03:16.657678 nef_pipelines-0.1.39/setup.cfg
+-rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.39/setup.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.260283 nef_pipelines-0.1.39/src/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.471566 nef_pipelines-0.1.39/src/nef_pipelines/
+-rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.39/src/nef_pipelines/VERSION
+-rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.529039 nef_pipelines-0.1.39/src/nef_pipelines/data/
+-rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.39/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.604557 nef_pipelines-0.1.39/src/nef_pipelines/lib/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    18119 2023-05-07 11:12:00.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15051 2023-05-04 07:18:02.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    21187 2023-04-30 15:31:02.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4109 2023-05-16 09:41:48.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10234 2023-04-26 19:21:33.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.608008 nef_pipelines-0.1.39/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    23686 2023-05-16 09:41:30.000000 nef_pipelines-0.1.39/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5288 2023-05-06 20:58:23.000000 nef_pipelines-0.1.39/src/nef_pipelines/main.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.616052 nef_pipelines-0.1.39/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.634927 nef_pipelines-0.1.39/src/nef_pipelines/tests/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.666715 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.670521 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.676994 nef_pipelines-0.1.39/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.680217 nef_pipelines-0.1.39/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.682555 nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.688547 nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.690512 nef_pipelines-0.1.39/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.696600 nef_pipelines-0.1.39/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.705655 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.721716 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_delete.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1884 2023-05-16 09:49:59.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_tabulate.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.735070 nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.737833 nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.764179 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.811591 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.849730 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.918908 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.939524 nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.944593 nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.946597 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.985101 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.987020 nef_pipelines-0.1.39/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.001618 nef_pipelines-0.1.39/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.022564 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.069876 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4153 2023-05-04 20:25:28.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2322 2023-05-16 09:41:29.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.112949 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/header.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/test_test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.127541 nef_pipelines-0.1.39/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.165855 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.188887 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.265871 nef_pipelines-0.1.39/src/nef_pipelines/tools/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.288584 nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.296474 nef_pipelines-0.1.39/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.317878 nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7414 2023-05-16 09:49:59.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.332234 nef_pipelines-0.1.39/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.338358 nef_pipelines-0.1.39/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7095 2023-04-26 16:43:57.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.39/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.341389 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.344513 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.349551 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.352933 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.355400 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15316 2023-05-07 11:13:51.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.361461 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.376473 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.418567 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.424527 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.438836 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.442637 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.454882 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.477410 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.486871 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.502988 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.515813 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.518875 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.534344 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10943 2023-05-07 09:41:03.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.538295 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.539772 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pdbx/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.545582 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.550466 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.554008 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.557513 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.566586 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.573656 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-04 07:46:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.588613 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16125 2023-05-07 09:39:01.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-04-26 18:39:25.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8328 2023-05-15 12:35:13.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.595085 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.604035 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.606073 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xeasy/
+-rw-r--r--   0 garythompson   (501) staff       (20)    18357 2023-05-16 09:57:46.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.617826 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.624798 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:16.652974 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-16 10:03:15.498002 nef_pipelines-0.1.39/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-16 10:03:15.000000 nef_pipelines-0.1.39/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)    13977 2023-05-16 10:03:15.000000 nef_pipelines-0.1.39/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-05-16 10:03:15.000000 nef_pipelines-0.1.39/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-05-16 10:03:15.000000 nef_pipelines-0.1.39/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.39/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-05-16 10:03:15.000000 nef_pipelines-0.1.39/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-05-16 10:03:15.000000 nef_pipelines-0.1.39/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.39/tox.ini
```

### Comparing `nef_pipelines-0.1.38/.github/workflows/ci.yml` & `nef_pipelines-0.1.39/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.39/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/.pre-commit-config.yaml` & `nef_pipelines-0.1.39/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/CHANGELOG.md` & `nef_pipelines-0.1.39/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -137,10 +137,14 @@
 sparky peak import fully supported with all fields shown in the spark manual
 
 ## version 0.1.37
 
 improved sparky assignment parsing which is also refactored into a reusable
 library
 
-## version 0.1.37
+## version 0.1.38
 
 initial experiments support for echidna peaks files
+
+## version 0.1.39
+
+fixed a bug in frames list (verbose option was ignored)
```

### Comparing `nef_pipelines-0.1.38/CONTRIBUTING.md` & `nef_pipelines-0.1.39/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/LICENSE.txt` & `nef_pipelines-0.1.39/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/PKG-INFO` & `nef_pipelines-0.1.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.38
+Version: 0.1.39
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.38/README.md` & `nef_pipelines-0.1.39/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/TODO.md` & `nef_pipelines-0.1.39/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.39/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.39/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/release_to_pypi.sh` & `nef_pipelines-0.1.39/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/setup.cfg` & `nef_pipelines-0.1.39/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/setup.py` & `nef_pipelines-0.1.39/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.39/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/nef_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 from argparse import Namespace
 from enum import auto
 from fnmatch import fnmatch
+from itertools import zip_longest
 from pathlib import Path
-from typing import Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
 # from pandas import DataFrame
 from pynmrstar import Entry, Loop, Saveframe
 from pynmrstar.definitions import STR_CONVERSION_DICT
 from pynmrstar.exceptions import ParsingError
 from strenum import LowercaseStrEnum
 
@@ -43,14 +44,18 @@
     as an example the molecular system should be a singleton
     ths doesn't imply the file has invalid star syntax, the star syntax will be valid
     """
 
     pass
 
 
+class NoSuchColumnException(Exception):
+    pass
+
+
 # what the selection type is for Star SaveFrames
 class SelectionType(LowercaseStrEnum):
     NAME = auto()
     CATEGORY = auto()
     ANY = auto()
 
     # see https://github.com/irgeek/StrEnum/issues/9
@@ -532,7 +537,73 @@
     frame_in_entry = False
     try:
         entry.get_saveframe_by_name(frame_name)
     except KeyError:
         frame_in_entry = False
 
     return frame_in_entry
+
+
+def set_column(loop: Loop, column: Union[int, str], values: List[Any]) -> Loop:
+    """
+    set the values of a column in a loop from a list
+    :param loop:  the loop
+    :param column: the name or index of the column to modify
+    :param values: the values to put into the column
+    :return: the loop (same instance)
+    """
+
+    column = _ensure_column_is_index(loop, column)
+
+    SENTINEL = "!!SENTINEL!!"
+    for row, merit in zip_longest(loop, values, fillvalue=SENTINEL):
+        if row is SENTINEL:
+            break
+        row[column] = merit
+
+    return loop
+
+
+def _ensure_column_is_index(loop: Loop, column: Union[str, int]) -> int:
+    if isinstance(column, str):
+        if column in loop.tags:
+            column = loop.tag_index(column)
+        else:
+            msg = f"""
+                the column {column} wasn't found in the loop {loop.category}
+
+                the available columns are {', '.join(loop.tags)}
+            """
+            raise NoSuchColumnException(msg)
+    return column
+
+
+def set_column_to_value(loop: Loop, column: Union[str, int], value: Any) -> Loop:
+    """
+
+    set the values of a column in a loop to a single value
+
+    :param loop:  the loop
+    :param column: the name or index of the column to modify
+    :param values: the values to put
+    :return: the loop (same instance)
+    """
+    column = _ensure_column_is_index(loop, column)
+    for row in loop:
+        row[column] = value
+
+    return loop
+
+
+def extract_column(loop: Loop, column: Union[str, int]) -> Loop:
+    """
+    Extract all the values in the column of a loop into a list
+
+    :param the loop
+    :param column: the name or index of the column to modify
+    :return: the values in the column as a list in row order
+    """
+    column = _ensure_column_is_index(loop, column)
+    values = []
+    for row in loop:
+        values.append(row[column])
+    return values
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/peak_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,8 +181,9 @@
     figure_of_merit: Optional[float] = None
     comment: str = ""
 
 
 @dataclass
 class DimensionInfo:
     axis_code: str  # this is the isotope code for us...
+    axis_name: str = None
     axis_unit: Optional[str] = "ppm"
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.39/src/nef_pipelines/lib/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import traceback
 from argparse import Namespace
 from enum import auto
 from math import floor
 from pathlib import Path
 from textwrap import dedent
-from typing import Any, Dict, Iterator, List, Optional, TextIO, TypeVar, Union
+from typing import Any, Dict, Iterator, List, Optional, TextIO, Tuple, TypeVar, Union
 
 import click
 from cacheable_iter import iter_cache
 from pynmrstar import Entry, Loop, Saveframe
 from strenum import StrEnum
 from tabulate import tabulate
 
@@ -840,7 +840,54 @@
     fallback_terminal_width: int = 100,
 ):
 
     table = strings_to_table_terminal_sensitive(
         strings, used_width, min_width, fallback_terminal_width
     )
     return tabulate(table, tablefmt="plain")
+
+
+def strip_characters_left(target: str, letters: str) -> Tuple[str, str]:
+
+    """
+     strip the characters from letters from the left of the target and return a tuple containing
+        1. the string without the stripped letters
+        2. the letters that were stripped off
+
+    :param target: the string to strip
+    :param letters:  the letters to be stripper
+    :return: a tuple of the form (<stripped-string>, <stripped-letters>)
+    """
+
+    remaining = target.lstrip(letters)
+
+    stripped = target[: len(target) - len(remaining)]
+
+    return stripped, remaining
+
+
+def strip_characters_right(target: str, letters: str) -> Tuple[str, str]:
+    """
+    strip the characters from letters from the right of the target and return a tuple containing
+        1. the string without the stripped letters
+        2. the letters that were stripped off
+
+    :param target: the string to strip
+    :param letters:  the letters to be stripper
+    :return: a tuple of the form (<stripped-string>, <stripped-letters>)
+    """
+
+    remaining = target.rstrip(letters)
+
+    stripped = target[(len(target) - len(remaining)) - 1 :]
+
+    return stripped, remaining
+
+
+def strip_line_comment(line: str, comment_character: str = "#") -> Tuple[str, str]:
+    comment = None
+    if comment_character in line:
+        index = line.index(comment_character)
+        comment = line[index + 1 :]
+        line = line[:index]
+
+    return line, comment
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/main.py` & `nef_pipelines-0.1.39/src/nef_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/echidna/test_import_peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/echidna/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_list.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from pathlib import Path
+
 import typer
 
 from nef_pipelines.lib.test_lib import (
     assert_lines_match,
     path_in_test_data,
     run_and_report,
 )
@@ -51,7 +53,35 @@
     EXPECTED = """\
         entry test
 
         nef_nmr_meta_data
     """
 
     assert_lines_match(EXPECTED, result.stdout)
+
+
+def test_frame_no_file():
+
+    path = Path("NO_SUCH_FILE")
+    run_and_report(app, [path], expected_exit_code=1)
+
+
+def test_frame_basic_verbose():
+
+    path = path_in_test_data(__file__, "frames.nef")
+    result = run_and_report(app, ["--in", path, "--verbose"])
+
+    EXPECTED_VERBOSE = """
+        entry test
+            lines: 48 frames: 2 checksum: d6235a487cbdb33cb1ed5d2f5f3f2635 [md5]
+        1. nef_nmr_meta_data
+            category: nef_nmr_meta_data
+            loops: 1 [lengths: 19]
+            is nef frame: True
+        2. nef_molecular_system
+            category: nef_molecular_system
+            loops: 1 [lengths: 13]
+            is nef frame: True
+
+    """
+
+    assert_lines_match(EXPECTED_VERBOSE, result.stdout)
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/pdbx/test_sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/pdbx/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/shifts/test_make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 import string
 
 import pytest
 
-from nef_pipelines.transcoders.sparky.sparky_lib import (
-    _strip_characters_left,
-    parse_single_assignment,
-)
+from nef_pipelines.lib.util import strip_characters_left
+from nef_pipelines.transcoders.sparky.sparky_lib import parse_single_assignment
 
 
 def test_strip_characters_left_empty():
 
     test = ""
 
-    stripped, remaining = _strip_characters_left(test, string.digits)
+    stripped, remaining = strip_characters_left(test, string.digits)
 
     assert stripped == ""
     assert remaining == ""
 
 
 def test_strip_characters_left_partial():
 
     test = "123abc"
 
-    stripped, remaining = _strip_characters_left(test, string.digits)
+    stripped, remaining = strip_characters_left(test, string.digits)
 
     assert stripped == "123"
     assert remaining == "abc"
 
 
 def test_strip_characters_left_all():
 
     test = "123456"
 
-    stripped, remaining = _strip_characters_left(test, string.digits)
+    stripped, remaining = strip_characters_left(test, string.digits)
 
     assert stripped == "123456"
     assert remaining == ""
 
 
 @pytest.mark.parametrize(
     """input,expected_residue_name, expected_residue_number, expected_atom_name, previous_residue_name,
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import contextlib
+import sys
 from pathlib import Path
 from textwrap import dedent
 from typing import List, Optional
 
 import typer
 from pynmrstar import Entry
 from tabulate import tabulate
 
 from nef_pipelines.lib.nef_lib import (
     SelectionType,
-    read_or_create_entry_exit_error_on_bad_file,
+    read_entry_from_file_or_stdin_or_exit_error,
     select_frames,
 )
 from nef_pipelines.lib.sequence_lib import count_residues, frame_to_chains
 from nef_pipelines.lib.typer_utils import get_args
 from nef_pipelines.lib.util import exit_error, strings_to_table_terminal_sensitive
 from nef_pipelines.tools.frames import frames_app
 
@@ -81,130 +83,133 @@
         ]
 
     args = get_args()
 
     if entry is None:
 
         try:
-            entry = read_or_create_entry_exit_error_on_bad_file(pipe)
+            entry = read_entry_from_file_or_stdin_or_exit_error(pipe)
         except Exception as e:
             exit_error(f"failed to read nef file {args.pipe} because", e)
         lines = str(entry)
 
     if entry is None:
         if args.pipe is not None:
             exit_error(f"couldn't read a nef stream from the file: {args.pipe}")
         elif len(filters) > 0:
             exit_error(f"couldn't read a nef stream from either {filters[0]} or stdin")
         else:
             exit_error("couldn't read a nef stream from stdin")
 
-    print(f"entry {entry.entry_id}")
-    if verbose:
-
-        import hashlib
-
-        md5 = hashlib.md5(lines.encode("ascii")).hexdigest()
-        num_lines = len(lines.split("\n"))
-        print(f"    lines: {num_lines} frames: {len(entry)} checksum: {md5} [md5]")
-    print()
-
-    frames = select_frames(entry, selector_type, filters)
-
-    if verbose == 0:
-        frame_names = [frame.name for frame in frames]
-        if number:
-            frame_names = [
-                f"{i}. {frame_name}"
-                for i, frame_name in enumerate(frame_names, start=1)
-            ]
+    with contextlib.redirect_stdout(sys.stderr):
+        print(f"entry {entry.entry_id}")
+        if verbose:
+
+            import hashlib
+
+            md5 = hashlib.md5(lines.encode("ascii")).hexdigest()
+            num_lines = len(lines.split("\n"))
+            print(f"    lines: {num_lines} frames: {len(entry)} checksum: {md5} [md5]")
+        print()
+
+        frames = select_frames(entry, selector_type, filters)
+
+        if verbose == 0:
+            frame_names = [frame.name for frame in frames]
+            if number:
+                frame_names = [
+                    f"{i}. {frame_name}"
+                    for i, frame_name in enumerate(frame_names, start=1)
+                ]
 
-        frame_list = strings_to_table_terminal_sensitive(frame_names)
-        print(tabulate(frame_list, tablefmt="plain"))
+            frame_list = strings_to_table_terminal_sensitive(frame_names)
+            print(tabulate(frame_list, tablefmt="plain"))
 
-    else:
+        else:
 
-        for frame in enumerate(frames, start=1):
+            for i, frame in enumerate(frames, start=1):
 
-            filters = [f"*{filter}*" for filter in filters]
+                filters = [f"*{filter}*" for filter in filters]
 
-            if verbose == 0:
-                frame_names = [
-                    f"{i}. {frame.name}" for i, frame_name in enumerate(frames, start=1)
-                ]
-
-                frame_list = strings_to_table_terminal_sensitive(frame_names)
-                print(tabulate(frame_list, tablefmt="plain"))
+                if verbose > 0:
+                    frame_names = [
+                        f"{i}. {frame.name}"
+                        for i, frame_name in enumerate(frames, start=1)
+                    ]
 
-                print(f"    category: {frame.category}")
-                if len(frame.name) != len(frame.category):
-                    print(
-                        f"    name: {frame.name[len(frame.category):].lstrip(UNDERSCORE)}"
-                    )
-
-                loop_lengths = []
-                for loop in frame.loop_dict:
-                    loop_lengths.append(str(len(loop)))
-
-                loops = ""
-                if len(loops) == 1:
-                    loops = " [length: 1]"
-                else:
-                    loops = f' [lengths: {", ".join(loop_lengths)}]'
-
-                print(f"    loops: {len(frame.loop_dict)}{loops}")
-
-                frame_standard = frame.name[: len("nef")]
-                is_standard_frame = frame_standard == "nef"
-                print(f"    is nef frame: {is_standard_frame}")
-
-                # ccpn_compound_name
-                if verbose == 2 and frame.category == "nef_molecular_system":
-                    chains = frame_to_chains(frame)
-
-                    print(f'    chains: {len(chains)} [{", ".join(chains)}]')
-
-                    residue_counts = {}
-                    for chain in chains:
-                        residue_counts[chain] = count_residues(frame, chain)
-
-                    residue_count_per_chain = {}
-                    for chain in chains:
-                        residue_count_per_chain[chain] = sum(
-                            residue_counts[chain].values()
+                    frame_list = strings_to_table_terminal_sensitive(frame_names)
+                    print(f"{i}. {frame.name}")
+                    print(f"    category: {frame.category}")
+                    if len(frame.name) != len(frame.category):
+                        print(
+                            f"    name: {frame.name[len(frame.category):].lstrip(UNDERSCORE)}"
                         )
 
-                    output = [
-                        f"{chain} {num_residues}"
-                        for chain, num_residues in residue_count_per_chain.items()
-                    ]
-                    print(f'    residues: {", ".join(output)}')
+                    loop_lengths = []
+                    for loop in frame.loop_dict:
+                        loop_lengths.append(str(len(loop)))
+
+                    loops = ""
+                    if len(loops) == 1:
+                        loops = " [length: 1]"
+                    else:
+                        loops = f' [lengths: {", ".join(loop_lengths)}]'
+
+                    print(f"    loops: {len(frame.loop_dict)}{loops}")
+
+                    frame_standard = frame.name[: len("nef")]
+                    is_standard_frame = frame_standard == "nef"
+                    print(f"    is nef frame: {is_standard_frame}")
+
+                    # ccpn_compound_name
+                    if verbose == 2 and frame.category == "nef_molecular_system":
+                        chains = frame_to_chains(frame)
+
+                        print(f'    chains: {len(chains)} [{", ".join(chains)}]')
+
+                        residue_counts = {}
+                        for chain in chains:
+                            residue_counts[chain] = count_residues(frame, chain)
+
+                        residue_count_per_chain = {}
+                        for chain in chains:
+                            residue_count_per_chain[chain] = sum(
+                                residue_counts[chain].values()
+                            )
 
-                    for chain in chains:
-                        counts_and_percentages = []
+                        output = [
+                            f"{chain} {num_residues}"
+                            for chain, num_residues in residue_count_per_chain.items()
+                        ]
+                        print(f'    residues: {", ".join(output)}')
+
+                        for chain in chains:
+                            counts_and_percentages = []
+
+                            for residue, count in residue_counts[chain].items():
+                                percentage = (
+                                    f"{count/ residue_count_per_chain[chain]*100:5.2f}"
+                                )
+                                counts_and_percentages.append(
+                                    f"{residue}: {count} [{percentage}%]"
+                                )
 
-                        for residue, count in residue_counts[chain].items():
-                            percentage = (
-                                f"{count/ residue_count_per_chain[chain]*100:5.2f}"
-                            )
-                            counts_and_percentages.append(
-                                f"{residue}: {count} [{percentage}%]"
-                            )
+                            pre_string = f"              {chain}. "
+                            pre_string_width = len(pre_string)
 
-                        pre_string = f"              {chain}. "
-                        pre_string_width = len(pre_string)
+                            tabulation = strings_to_table_terminal_sensitive(
+                                counts_and_percentages, pre_string_width
+                            )
+                            table = tabulate(tabulation, tablefmt="plain")
 
-                        tabulation = strings_to_table_terminal_sensitive(
-                            counts_and_percentages, pre_string_width
-                        )
-                        table = tabulate(tabulation, tablefmt="plain")
+                            print(_indent_with_prestring(table, pre_string))
 
-                        print(_indent_with_prestring(table, pre_string))
+                print()
 
-    print()
+        print()
 
 
 def _indent_with_prestring(text_block, pre_string):
     raw_result = []
     empty_prestring = " " * len(pre_string)
     for i, string in enumerate(text_block.split("\n")):
         if i == 0:
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.39/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/echidna/importers/peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/echidna/importers/peaks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,40 @@
-# import string
-# import sys
 from collections import OrderedDict
 from dataclasses import dataclass
-from itertools import zip_longest
 from pathlib import Path
-
-# from itertools import zip_longest
-# from pathlib import Path
-# from textwrap import dedent
 from typing import Iterator, List
 
 import typer
 from fyeah import f
 from pynmrstar import Saveframe
 
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
+    extract_column,
     read_or_create_entry_exit_error_on_bad_file,
+    set_column,
+    set_column_to_value,
 )
 from nef_pipelines.lib.sequence_lib import MoleculeTypes, sequence_from_entry
-
-# from fyeah import f
-#
-# from nef_pipelines.lib.isotope_lib import ATOM_TO_ISOTOPE
-# from nef_pipelines.lib.nef_lib import (
-#     UNUSED,
-#     add_frames_to_entry,
-#     read_or_create_entry_exit_error_on_bad_file,
-# )
-# from nef_pipelines.lib.peak_lib import peaks_to_frame
-# from nef_pipelines.lib.sequence_lib import (
-#     TRANSLATIONS_1_3,
-#     MoleculeTypes,
-#     chain_code_iter,
-#     residues_to_residue_name_lookup,
-#     sequence_from_entry,
-# )
-# from nef_pipelines.lib.structures import (
-#     AtomLabel,
-#     LineInfo,
-#     NewPeak,
-#     PeakFitMethod,
-#     Residue,
-#     SequenceResidue,
-#     ShiftData,
-# )
 from nef_pipelines.lib.util import (  # STDIN,; exit_error,; parse_comma_separated_options,
     STDIN,
     is_float,
     parse_comma_separated_options,
 )
 from nef_pipelines.transcoders.echidna import import_app
 from nef_pipelines.transcoders.sparky.importers.peaks import (
     pipe as sparky_peak_import_pipe,
 )
 
 DEFAULT_MERIT_FUNTION = "round(x**(1.0/6.0),5)"
 
+# TODO: rationalise these into lib
 CCPN_COMMENT = "ccpn_comment"
-
 HEIGHT = "height"
-
 CCPN_MERIT = "ccpn_merit"
-
 NEF_PEAK = "nef_peak"
 
 app = typer.Typer()
 
 DEFAULT_NUCLEI_HELP = (
     "nuclei to use for each dimension, if not defined they are guessed from the assignments"
     "or an error is reported"
@@ -329,15 +297,15 @@
 
 @import_app.command(no_args_is_help=True)
 def peaks(
     frame_name: str = typer.Option(
         "nef_nmr_spectrum_{file_name}",
         "-f",
         "--frame-name",
-        help="a templated name for the frame {file_name} will be replaced by input filename",
+        help="a templated name for the frame {file_name} will be replaced by input filename without its extension",
     ),
     input: Path = typer.Option(
         STDIN,
         "-i",
         "--in",
         metavar="|PIPE|",
         help="input to read NEF data from [- is stdin]",
@@ -403,15 +371,15 @@
 
     return result
 
 
 #
 def pipe(
     entry,
-    frame_name,
+    frame_name_template,
     file_names_and_lines,
     chain_code,
     sequence,
     input_dimensions,
     spectrometer_frequency,
     molecule_type=MoleculeTypes.PROTEIN,
     merit_function=DEFAULT_MERIT_FUNTION,
@@ -419,116 +387,124 @@
 
     for file_name, lines in file_names_and_lines.items():
 
         lines, tensor, atom_position = _parse_echidna(lines, file_name)
 
         entry = sparky_peak_import_pipe(
             entry,
-            frame_name,
+            frame_name_template,
             {file_name: lines},
             chain_code,
             sequence,
             input_dimensions,
             spectrometer_frequency,
             molecule_type=molecule_type,
         )
 
-        file_name = file_name.stem
-        frame = entry.get_saveframe_by_name(f(frame_name))
+        file_name = file_name.stem  # used by f()
+        frame = entry.get_saveframe_by_name(f(frame_name_template))
+
+        frame_name = file_name
 
         loop = frame.get_loop(NEF_PEAK)
         loop.add_tag(CCPN_MERIT, update_data=True)
 
-        comment_index = loop.tag_index(CCPN_COMMENT)
-        comment_values = extract_column(loop, comment_index)
-        comment_values = [
-            comment.lstrip().lstrip(";").lstrip() for comment in comment_values
-        ]
-        loop.remove_tag(CCPN_COMMENT)
+        comment_values = _remove_and_store_comments(loop)
 
         height_index = loop.tag_index(HEIGHT)
         merit_index = loop.tag_index(CCPN_MERIT)
 
-        heights = extract_column(loop, height_index)
-        heights = [float(height) for height in heights]
-        set_column_to_value(loop, height_index, UNUSED)
-        merits = [eval(merit_function) for x in heights]
-        set_column(loop, merit_index, merits)
-
-        loop.add_tag(CCPN_COMMENT, update_data=True)
-        comment_index = loop.tag_index(CCPN_COMMENT)
-        set_column(loop, comment_index, comment_values)
-
-        merits_for_large_violations = []
-        for row in loop:
-            if "large violation!" in row[comment_index]:
-                merits_for_large_violations.append(float(row[merit_index]))
-
-        lowest_large_violation_merit = min(merits_for_large_violations)
-
-        note = f"NOTE: merits with values > {lowest_large_violation_merit} are flagged as large violations"
-        frame.add_tag(CCPN_COMMENT, note)
-
-        tensor_frame_category = "np_tensor_frame"
-        tensor_frame_name = f"{tensor_frame_category}_{file_name}"
-        frame.add_tag("np_tensor_frame_name", tensor_frame_name)
-
-        tag_values = {
-            "restraint_origin": "measured",
-            "ccpn_format": "angles_euler",
-            "restraint_magnitude": tensor.amplitude,
-            "restraint_rhomicity": tensor.rhombicity,
-            "ccpn_phi": tensor.phi,
-            "ccpn_psi": tensor.psi,
-            "ccpn_theta": tensor.theta,
-        }
-        tensor_save_frame = create_simple_frame(
-            tensor_frame_category, tensor_frame_name, tag_values
+        _convert_heights_to_figure_of_merit(
+            loop, height_index, merit_index, merit_function
         )
-        entry.add_saveframe(tensor_save_frame)
 
-        atom_position_category = "np_atom_position"
-        atom_position_name = f"{atom_position_category}_{file_name}"
-        frame.add_tag("np_atom_position_name", atom_position_name)
-
-        tag_values = {"x": atom_position.x, "y": atom_position.y, "z": atom_position.z}
-        atom_position_save_frame = create_simple_frame(
-            atom_position_category, atom_position_name, tag_values
+        comment_index = _append_stored_comments(loop, comment_values)
+
+        _add_frame_comment_for_large_violation_limit(
+            frame, loop, comment_index, merit_index
         )
-        entry.add_saveframe(atom_position_save_frame)
+
+        _add_tensor_frame_saveframe(entry, frame, tensor, frame_name)
+
+        _add_atom_position_saveframe(entry, frame, atom_position, frame_name)
 
     return entry
 
 
-def create_simple_frame(atom_position_category, atom_position_name, tag_values):
-    save_frame = Saveframe.from_scratch(atom_position_name, atom_position_category)
+def _add_atom_position_saveframe(entry, frame, atom_position, frame_name):
+    atom_position_category = "np_atom_position"
+    atom_position_name = f"{atom_position_category}_{frame_name}"
+    frame.add_tag("np_atom_position_name", atom_position_name)
+    tag_values = {"x": atom_position.x, "y": atom_position.y, "z": atom_position.z}
+    atom_position_save_frame = create_simple_frame(
+        atom_position_category, atom_position_name, tag_values
+    )
+    entry.add_saveframe(atom_position_save_frame)
+
+
+def _add_tensor_frame_saveframe(entry, frame, tensor, frame_name):
+    tensor_frame_category = "np_tensor_frame"
+    tensor_frame_name = f"{tensor_frame_category}_{frame_name}"
+    frame.add_tag("np_tensor_frame_name", tensor_frame_name)
+    tag_values = {
+        "restraint_origin": "measured",
+        "ccpn_format": "angles_euler",
+        "restraint_magnitude": tensor.amplitude,
+        "restraint_rhomicity": tensor.rhombicity,
+        "ccpn_phi": tensor.phi,
+        "ccpn_psi": tensor.psi,
+        "ccpn_theta": tensor.theta,
+    }
+    tensor_save_frame = create_simple_frame(
+        tensor_frame_category, tensor_frame_name, tag_values
+    )
+    entry.add_saveframe(tensor_save_frame)
 
-    save_frame.add_tag("sf_category", atom_position_category)
-    save_frame.add_tag("sf_framecode", atom_position_name)
-    for tag, value in tag_values.items():
-        save_frame.add_tag(tag, value)
 
-    return save_frame
+def _add_frame_comment_for_large_violation_limit(
+    frame, loop, comment_index, merit_index
+):
+    merits_for_large_violations = []
+    for row in loop:
+        if "large violation!" in row[comment_index]:
+            merits_for_large_violations.append(float(row[merit_index]))
+    lowest_large_violation_merit = min(merits_for_large_violations)
+    note = f"NOTE: merits with values > {lowest_large_violation_merit} are flagged as large violations"
+    frame.add_tag(CCPN_COMMENT, note)
+
+
+def _append_stored_comments(loop, comment_values):
+    loop.add_tag(CCPN_COMMENT, update_data=True)
+    comment_index = loop.tag_index(CCPN_COMMENT)
+    set_column(loop, comment_index, comment_values)
+    return comment_index
 
 
-def set_column(loop, merit_index, merits):
-    SENTINEL = "!!SENTINEL!!"
-    for row, merit in zip_longest(loop, merits, fillvalue=SENTINEL):
-        if row is SENTINEL:
-            break
-        row[merit_index] = merit
+def _convert_heights_to_figure_of_merit(
+    loop, height_index, merit_index, merit_function
+):
+    heights = extract_column(loop, height_index)
+    heights = [float(height) for height in heights]
+    set_column_to_value(loop, height_index, UNUSED)
+    merits = [eval(merit_function) for x in heights]
+    set_column(loop, merit_index, merits)
 
-    return loop
 
+def _remove_and_store_comments(loop):
+    comment_index = loop.tag_index(CCPN_COMMENT)
+    comment_values = extract_column(loop, comment_index)
+    comment_values = [
+        comment.lstrip().lstrip(";").lstrip() for comment in comment_values
+    ]
+    loop.remove_tag(CCPN_COMMENT)
+    return comment_values
 
-def set_column_to_value(loop, height_index, value):
-    for row in loop:
-        row[height_index] = value
 
-    return loop
+def create_simple_frame(atom_position_category, atom_position_name, tag_values):
+    save_frame = Saveframe.from_scratch(atom_position_name, atom_position_category)
 
+    save_frame.add_tag("sf_category", atom_position_category)
+    save_frame.add_tag("sf_framecode", atom_position_name)
+    for tag, value in tag_values.items():
+        save_frame.add_tag(tag, value)
 
-def extract_column(loop, columns_index):
-    values = []
-    for row in loop:
-        values.append(row[columns_index])
-    return values
+    return save_frame
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     UNUSED,
     loop_row_dict_iter,
     read_entry_from_file_or_stdin_or_exit_error,
     select_frames_by_name,
 )
 from nef_pipelines.lib.sequence_lib import sequence_from_entry, sequence_to_chains
 from nef_pipelines.lib.structures import AtomLabel, RdcRestraint, SequenceResidue
-from nef_pipelines.lib.translation_lib import translate_atom_label
+from nef_pipelines.lib.translation_lib import IUPAC_XPLOR, translate_atom_label
 from nef_pipelines.lib.util import (
     STDIN,
     exit_error,
     flatten,
     get_display_file_name,
     read_float_or_exit,
 )
@@ -123,34 +123,33 @@
 
     _exit_if_user_chains_not_in_restraints(rdc_chains, user_chains, input, rdc_frames)
 
     for frame_name, restraints in rdc_restaints_by_frame.items():
 
         _exit_if_mixed_chain_restraints(restraints, frame_name, input)
 
-        restraints = _translate_atom_names(restraints, "xplor")
+        restraints = _translate_atom_names(restraints, IUPAC_XPLOR)
 
         restraints = _update_restraint_uncertainty(restraints, default_uncertainty)
 
         print()
 
         _print_restraints(restraints, weights, segids)
 
 
 def _translate_atom_names(
-    restraints: List[RdcRestraint], naming_scheme="xplor_to_iupac"
+    restraints: List[RdcRestraint], naming_scheme=IUPAC_XPLOR
 ) -> List[RdcRestraint]:
     result = []
     for restraint in restraints:
         atom_1 = restraint.atom_1
         atom_2 = restraint.atom_2
 
-        translation = {"H": "HN"}
-        atom_1 = translate_atom_label(atom_1, translation)
-        atom_2 = translate_atom_label(atom_2, translation)
+        atom_1 = translate_atom_label(atom_1, naming_scheme)
+        atom_2 = translate_atom_label(atom_2, naming_scheme)
 
         restraint = replace(restraint, atom_1=atom_1)
         restraint = replace(restraint, atom_2=atom_2)
         restraint.atom_1 = atom_1
 
         result.append(restraint)
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/pdbx/importers/sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/pdbx/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/sparky/sparky_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nef_pipelines.lib.nef_lib import UNUSED
 from nef_pipelines.lib.sequence_lib import (
     TRANSLATIONS_1_3,
     MoleculeType,
     residues_to_residue_name_lookup,
 )
 from nef_pipelines.lib.structures import AtomLabel, LineInfo, Residue, SequenceResidue
-from nef_pipelines.lib.util import exit_error
+from nef_pipelines.lib.util import exit_error, strip_characters_left
 
 #
 # sparky docs
 #
 # Make peaks on a spectrum from a peak list file (rp).
 #
 # Peaks are read from a peak list file and placed on the selected spectrum.
@@ -46,23 +46,14 @@
 # how does sparky cope with complexes where peaks are between chains
 # which it doesn't define
 #
 
 SparkyAtomLabel = namedtuple("SparkyAtomLabel", "residue_number residue_name atom_name")
 
 
-def _strip_characters_left(target: str, letters: str) -> Tuple[str, str]:
-
-    remaining = target.lstrip(letters)
-
-    stripped = target[: len(target) - len(remaining)]
-
-    return stripped, remaining
-
-
 def parse_single_assignment(
     assignment: str,
     previous_residue_name: str = None,
     previous_residue_number: str = None,
 ) -> Tuple[str, str, str]:
 
     """
@@ -75,25 +66,25 @@
     :param previous_residue_number: a previous residue number to use for an abbreviated assignment
     :return: a tuple of the form (residue_number, residue_name , atom_name)
     """
 
     target = assignment
 
     # remove a residue name or question mark
-    residue_name, target = _strip_characters_left(target, string.ascii_letters)
+    residue_name, target = strip_characters_left(target, string.ascii_letters)
     if len(target) == 0:
         target = residue_name
         residue_name = ""
 
     if target[0] == "?" and len(target) > 0:
         target = target[1:]
         residue_name = ""
 
     # remove residue numbers or question mark
-    residue_number, target = _strip_characters_left(target, string.digits)
+    residue_number, target = strip_characters_left(target, string.digits)
 
     if len(residue_number) == 0 and len(target) != 0 and target[0] == "?":
         target = target[1:]
         residue_number = ""
 
     if len(target) > 0:
         atom_name = target
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.39/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.39/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef-pipelines
-Version: 0.1.38
+Version: 0.1.39
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.38/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.39/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,15 @@
 src/nef_pipelines/transcoders/sparky/importers/__init__.py
 src/nef_pipelines/transcoders/sparky/importers/peaks.py
 src/nef_pipelines/transcoders/sparky/importers/sequence.py
 src/nef_pipelines/transcoders/sparky/importers/shifts.py
 src/nef_pipelines/transcoders/xcamshift/__init__.py
 src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
 src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
 src/nef_pipelines/transcoders/xplor/__init__.py
 src/nef_pipelines/transcoders/xplor/psf_lib.py
 src/nef_pipelines/transcoders/xplor/xplor_lib.py
 src/nef_pipelines/transcoders/xplor/exporters/__init__.py
 src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
 src/nef_pipelines/transcoders/xplor/importers/__init__.py
 src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
```

### Comparing `nef_pipelines-0.1.38/tox.ini` & `nef_pipelines-0.1.39/tox.ini`

 * *Files identical despite different names*

