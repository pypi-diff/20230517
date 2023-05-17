# Comparing `tmp/usdm-0.26.0.tar.gz` & `tmp/usdm-0.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.26.0.tar", last modified: Mon May 15 06:15:29 2023, max compression
+gzip compressed data, was "usdm-0.27.0.tar", last modified: Wed May 17 10:33:50 2023, max compression
```

## Comparing `usdm-0.26.0.tar` & `usdm-0.27.0.tar`

### file list

```diff
@@ -1,140 +1,141 @@
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.536518 usdm-0.26.0/
--rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.26.0/LICENSE
--rw-r--r--   0 daveih     (501) staff       (20)    21059 2023-05-15 06:15:29.536306 usdm-0.26.0/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)    20609 2023-05-08 14:51:48.000000 usdm-0.26.0/README.md
--rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.26.0/pyproject.toml
--rw-r--r--   0 daveih     (501) staff       (20)       38 2023-05-15 06:15:29.536562 usdm-0.26.0/setup.cfg
--rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.26.0/setup.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.479967 usdm-0.26.0/src/
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.484608 usdm-0.26.0/src/usdm.egg-info/
--rw-r--r--   0 daveih     (501) staff       (20)    21059 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/PKG-INFO
--rw-r--r--   0 daveih     (501) staff       (20)     4469 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/SOURCES.txt
--rw-r--r--   0 daveih     (501) staff       (20)        1 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/dependency_links.txt
--rw-r--r--   0 daveih     (501) staff       (20)       45 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/requires.txt
--rw-r--r--   0 daveih     (501) staff       (20)       32 2023-05-15 06:15:29.000000 usdm-0.26.0/src/usdm.egg-info/top_level.txt
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.492327 usdm-0.26.0/src/usdm_excel/
--rw-r--r--   0 daveih     (501) staff       (20)     1330 2023-05-15 06:05:22.000000 usdm-0.26.0/src/usdm_excel/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.26.0/src/usdm_excel/alias.py
--rw-r--r--   0 daveih     (501) staff       (20)     8852 2023-05-09 10:09:13.000000 usdm-0.26.0/src/usdm_excel/base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     4667 2023-05-01 12:04:14.000000 usdm-0.26.0/src/usdm_excel/cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.26.0/src/usdm_excel/cdisc_ct.py
--rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.26.0/src/usdm_excel/cdisc_ct_library.py
--rw-r--r--   0 daveih     (501) staff       (20)     1564 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/cross_ref.py
--rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/ct_version_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.493768 usdm-0.26.0/src/usdm_excel/data/
--rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.26.0/src/usdm_excel/data/cdisc_ct_config.yaml
--rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/data/iso_3166.json
--rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.26.0/src/usdm_excel/data/missing_ct.yaml
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.494952 usdm-0.26.0/src/usdm_excel/errors/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.26.0/src/usdm_excel/errors/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      715 2023-05-09 05:56:05.000000 usdm-0.26.0/src/usdm_excel/errors/error.py
--rw-r--r--   0 daveih     (501) staff       (20)      672 2023-05-09 05:53:57.000000 usdm-0.26.0/src/usdm_excel/errors/errors.py
--rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/id_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.26.0/src/usdm_excel/iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.26.0/src/usdm_excel/logger.py
--rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.26.0/src/usdm_excel/ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     5161 2023-05-15 06:05:22.000000 usdm-0.26.0/src/usdm_excel/nodes_and_edges.py
--rw-r--r--   0 daveih     (501) staff       (20)      824 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/option_manager.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.495696 usdm-0.26.0/src/usdm_excel/study_design_activity_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.26.0/src/usdm_excel/study_design_activity_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1404 2023-05-08 14:51:48.000000 usdm-0.26.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.496435 usdm-0.26.0/src/usdm_excel/study_design_arm_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.26.0/src/usdm_excel/study_design_arm_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1457 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.497172 usdm-0.26.0/src/usdm_excel/study_design_element_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_element_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1841 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.497925 usdm-0.26.0/src/usdm_excel/study_design_encounter_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2338 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.498537 usdm-0.26.0/src/usdm_excel/study_design_epoch_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.26.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1131 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.499513 usdm-0.26.0/src/usdm_excel/study_design_estimands_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2273 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.501243 usdm-0.26.0/src/usdm_excel/study_design_ii_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_ii_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1662 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.502396 usdm-0.26.0/src/usdm_excel/study_design_objective_endpoint_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2024 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.503691 usdm-0.26.0/src/usdm_excel/study_design_population_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_population_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1638 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.504454 usdm-0.26.0/src/usdm_excel/study_design_procedure_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     1499 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.505451 usdm-0.26.0/src/usdm_excel/study_design_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_design_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     5094 2023-04-14 12:14:15.000000 usdm-0.26.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.506870 usdm-0.26.0/src/usdm_excel/study_identifiers_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_identifiers_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     2559 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.507731 usdm-0.26.0/src/usdm_excel/study_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)     7614 2023-05-08 13:47:22.000000 usdm-0.26.0/src/usdm_excel/study_sheet/study_sheet.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.512223 usdm-0.26.0/src/usdm_excel/study_soa_sheet/
--rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/activities.py
--rw-r--r--   0 daveih     (501) staff       (20)     3498 2023-05-09 06:07:57.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/cycle.py
--rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/cycles.py
--rw-r--r--   0 daveih     (501) staff       (20)      993 2023-04-05 14:06:46.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/encounters.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
--rw-r--r--   0 daveih     (501) staff       (20)     4645 2023-04-13 09:55:50.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     5048 2023-04-13 04:26:45.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/timepoint.py
--rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-13 04:26:45.000000 usdm-0.26.0/src/usdm_excel/study_soa_sheet/timepoints.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.512615 usdm-0.26.0/src/usdm_info/
--rw-r--r--   0 daveih     (501) staff       (20)       59 2023-05-01 12:04:14.000000 usdm-0.26.0/src/usdm_info/__init__.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.529281 usdm-0.26.0/src/usdm_model/
--rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/__init__.py
--rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/activity.py
--rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/address.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/aliasCode.py
--rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/alias_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/analysis_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/api_base_model.py
--rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/biomedical_concept_category.py
--rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/biomedical_concept_property.py
--rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/biomedical_concept_surrogate.py
--rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/code.py
--rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/encounter.py
--rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/endpoint.py
--rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/estimand.py
--rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/indication.py
--rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/intercurrent_event.py
--rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/investigational_intervention.py
--rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/objective.py
--rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/organisation.py
--rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/procedure.py
--rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/response_code.py
--rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/schedule_timeline.py
--rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/schedule_timeline_exit.py
--rw-r--r--   0 daveih     (501) staff       (20)      691 2023-04-13 04:26:45.000000 usdm-0.26.0/src/usdm_model/scheduled_instance.py
--rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study.py
--rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/study_arm.py
--rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_cell.py
--rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/study_design.py
--rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_design_population.py
--rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_element.py
--rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_epoch.py
--rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_identifier.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/study_protocol_version.py
--rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 13:59:38.000000 usdm-0.26.0/src/usdm_model/timing.py
--rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 13:46:27.000000 usdm-0.26.0/src/usdm_model/transition_rule.py
-drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-15 06:15:29.535679 usdm-0.26.0/tests/
--rw-r--r--   0 daveih     (501) staff       (20)    13402 2023-05-08 13:47:22.000000 usdm-0.26.0/tests/test_base_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.26.0/tests/test_cdisc_biomedical_concept.py
--rw-r--r--   0 daveih     (501) staff       (20)     1517 2023-05-08 13:47:22.000000 usdm-0.26.0/tests/test_configuration_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)      679 2023-04-11 13:28:11.000000 usdm-0.26.0/tests/test_error.py
--rw-r--r--   0 daveih     (501) staff       (20)     1126 2023-04-11 13:28:11.000000 usdm-0.26.0/tests/test_errors.py
--rw-r--r--   0 daveih     (501) staff       (20)      762 2023-05-09 10:48:00.000000 usdm-0.26.0/tests/test_integration.py
--rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.26.0/tests/test_iso_3166.py
--rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.26.0/tests/test_ncit.py
--rw-r--r--   0 daveih     (501) staff       (20)     1098 2023-05-08 13:47:22.000000 usdm-0.26.0/tests/test_option_manager.py
--rw-r--r--   0 daveih     (501) staff       (20)     3199 2023-05-08 14:51:48.000000 usdm-0.26.0/tests/test_study_design_activity_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.26.0/tests/test_study_design_arm_sheet.py
--rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.26.0/tests/test_study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.722452 usdm-0.27.0/
+-rw-r--r--   0 daveih     (501) staff       (20)    35149 2023-03-30 07:33:41.000000 usdm-0.27.0/LICENSE
+-rw-r--r--   0 daveih     (501) staff       (20)    21536 2023-05-17 10:33:50.722225 usdm-0.27.0/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)    21086 2023-05-16 13:32:48.000000 usdm-0.27.0/README.md
+-rw-r--r--   0 daveih     (501) staff       (20)       97 2023-03-31 13:46:27.000000 usdm-0.27.0/pyproject.toml
+-rw-r--r--   0 daveih     (501) staff       (20)       38 2023-05-17 10:33:50.722509 usdm-0.27.0/setup.cfg
+-rw-r--r--   0 daveih     (501) staff       (20)      932 2023-04-12 12:31:13.000000 usdm-0.27.0/setup.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.638826 usdm-0.27.0/src/
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.653855 usdm-0.27.0/src/usdm.egg-info/
+-rw-r--r--   0 daveih     (501) staff       (20)    21536 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/PKG-INFO
+-rw-r--r--   0 daveih     (501) staff       (20)     4507 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/SOURCES.txt
+-rw-r--r--   0 daveih     (501) staff       (20)        1 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/dependency_links.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       45 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/requires.txt
+-rw-r--r--   0 daveih     (501) staff       (20)       32 2023-05-17 10:33:50.000000 usdm-0.27.0/src/usdm.egg-info/top_level.txt
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.668920 usdm-0.27.0/src/usdm_excel/
+-rw-r--r--   0 daveih     (501) staff       (20)     1611 2023-05-17 09:09:09.000000 usdm-0.27.0/src/usdm_excel/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      269 2023-03-31 14:50:16.000000 usdm-0.27.0/src/usdm_excel/alias.py
+-rw-r--r--   0 daveih     (501) staff       (20)    10630 2023-05-17 09:48:28.000000 usdm-0.27.0/src/usdm_excel/base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4667 2023-05-01 12:04:14.000000 usdm-0.27.0/src/usdm_excel/cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      787 2023-03-31 14:50:16.000000 usdm-0.27.0/src/usdm_excel/cdisc_ct.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4349 2023-04-11 15:59:49.000000 usdm-0.27.0/src/usdm_excel/cdisc_ct_library.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1564 2023-05-08 13:47:22.000000 usdm-0.27.0/src/usdm_excel/configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      400 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/cross_ref.py
+-rw-r--r--   0 daveih     (501) staff       (20)      337 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/ct_version_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.670521 usdm-0.27.0/src/usdm_excel/data/
+-rw-r--r--   0 daveih     (501) staff       (20)      963 2023-04-14 12:14:15.000000 usdm-0.27.0/src/usdm_excel/data/cdisc_ct_config.yaml
+-rw-r--r--   0 daveih     (501) staff       (20)    83279 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/data/iso_3166.json
+-rw-r--r--   0 daveih     (501) staff       (20)     3453 2023-04-11 15:59:49.000000 usdm-0.27.0/src/usdm_excel/data/missing_ct.yaml
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.672238 usdm-0.27.0/src/usdm_excel/errors/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-06 07:20:00.000000 usdm-0.27.0/src/usdm_excel/errors/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      933 2023-05-17 09:15:41.000000 usdm-0.27.0/src/usdm_excel/errors/error.py
+-rw-r--r--   0 daveih     (501) staff       (20)      732 2023-05-17 09:15:52.000000 usdm-0.27.0/src/usdm_excel/errors/errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1189 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/id_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)      744 2023-04-13 09:34:38.000000 usdm-0.27.0/src/usdm_excel/iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      111 2023-04-03 10:43:35.000000 usdm-0.27.0/src/usdm_excel/logger.py
+-rw-r--r--   0 daveih     (501) staff       (20)      309 2023-03-31 14:50:16.000000 usdm-0.27.0/src/usdm_excel/ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5161 2023-05-15 06:05:22.000000 usdm-0.27.0/src/usdm_excel/nodes_and_edges.py
+-rw-r--r--   0 daveih     (501) staff       (20)      824 2023-05-08 13:47:22.000000 usdm-0.27.0/src/usdm_excel/option_manager.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.673239 usdm-0.27.0/src/usdm_excel/study_design_activity_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-05-03 10:02:41.000000 usdm-0.27.0/src/usdm_excel/study_design_activity_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1570 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.675122 usdm-0.27.0/src/usdm_excel/study_design_arm_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.27.0/src/usdm_excel/study_design_arm_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1617 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_arm_sheet/study_design_arm_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.678503 usdm-0.27.0/src/usdm_excel/study_design_element_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_element_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2003 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.680194 usdm-0.27.0/src/usdm_excel/study_design_encounter_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_encounter_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2503 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.684651 usdm-0.27.0/src/usdm_excel/study_design_epoch_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-04-14 12:14:15.000000 usdm-0.27.0/src/usdm_excel/study_design_epoch_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1289 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.686650 usdm-0.27.0/src/usdm_excel/study_design_estimands_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_estimands_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2794 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.689357 usdm-0.27.0/src/usdm_excel/study_design_ii_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_ii_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1991 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.690943 usdm-0.27.0/src/usdm_excel/study_design_objective_endpoint_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_objective_endpoint_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2475 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.693078 usdm-0.27.0/src/usdm_excel/study_design_population_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_population_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1778 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.694041 usdm-0.27.0/src/usdm_excel/study_design_procedure_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_procedure_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1645 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.694646 usdm-0.27.0/src/usdm_excel/study_design_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_design_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     6218 2023-05-17 09:41:38.000000 usdm-0.27.0/src/usdm_excel/study_design_sheet/study_design_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.695169 usdm-0.27.0/src/usdm_excel/study_identifiers_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_identifiers_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3435 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.695942 usdm-0.27.0/src/usdm_excel/study_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)     7892 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_sheet/study_sheet.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.701901 usdm-0.27.0/src/usdm_excel/study_soa_sheet/
+-rw-r--r--   0 daveih     (501) staff       (20)        0 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      637 2023-04-03 10:43:35.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/activities.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3498 2023-05-09 06:07:57.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      888 2023-04-05 14:06:46.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/cycle.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1864 2023-04-05 14:06:46.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/cycles.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1056 2023-05-17 05:14:14.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/encounters.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/soa_column_rows.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4645 2023-04-13 09:55:50.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     5048 2023-04-13 04:26:45.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/timepoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2748 2023-04-13 04:26:45.000000 usdm-0.27.0/src/usdm_excel/study_soa_sheet/timepoints.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.702326 usdm-0.27.0/src/usdm_info/
+-rw-r--r--   0 daveih     (501) staff       (20)       59 2023-05-16 13:26:16.000000 usdm-0.27.0/src/usdm_info/__init__.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.715353 usdm-0.27.0/src/usdm_model/
+-rw-r--r--   0 daveih     (501) staff       (20)     1685 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/__init__.py
+-rw-r--r--   0 daveih     (501) staff       (20)      545 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/activity.py
+-rw-r--r--   0 daveih     (501) staff       (20)      210 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/address.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/aliasCode.py
+-rw-r--r--   0 daveih     (501) staff       (20)      229 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/alias_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      139 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/analysis_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      844 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/api_base_model.py
+-rw-r--r--   0 daveih     (501) staff       (20)      375 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)      315 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/biomedical_concept_category.py
+-rw-r--r--   0 daveih     (501) staff       (20)      394 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/biomedical_concept_property.py
+-rw-r--r--   0 daveih     (501) staff       (20)      216 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/biomedical_concept_surrogate.py
+-rw-r--r--   0 daveih     (501) staff       (20)      152 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      642 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/encounter.py
+-rw-r--r--   0 daveih     (501) staff       (20)      262 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/endpoint.py
+-rw-r--r--   0 daveih     (501) staff       (20)      543 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/estimand.py
+-rw-r--r--   0 daveih     (501) staff       (20)      224 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/indication.py
+-rw-r--r--   0 daveih     (501) staff       (20)      206 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/intercurrent_event.py
+-rw-r--r--   0 daveih     (501) staff       (20)      260 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/investigational_intervention.py
+-rw-r--r--   0 daveih     (501) staff       (20)      311 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/objective.py
+-rw-r--r--   0 daveih     (501) staff       (20)      347 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/organisation.py
+-rw-r--r--   0 daveih     (501) staff       (20)      274 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/procedure.py
+-rw-r--r--   0 daveih     (501) staff       (20)      186 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/response_code.py
+-rw-r--r--   0 daveih     (501) staff       (20)      509 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/schedule_timeline.py
+-rw-r--r--   0 daveih     (501) staff       (20)      114 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/schedule_timeline_exit.py
+-rw-r--r--   0 daveih     (501) staff       (20)      691 2023-04-13 04:26:45.000000 usdm-0.27.0/src/usdm_model/scheduled_instance.py
+-rw-r--r--   0 daveih     (501) staff       (20)      677 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study.py
+-rw-r--r--   0 daveih     (501) staff       (20)      296 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/study_arm.py
+-rw-r--r--   0 daveih     (501) staff       (20)      380 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_cell.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1583 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/study_design.py
+-rw-r--r--   0 daveih     (501) staff       (20)      351 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_design_population.py
+-rw-r--r--   0 daveih     (501) staff       (20)      359 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_element.py
+-rw-r--r--   0 daveih     (501) staff       (20)      401 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_epoch.py
+-rw-r--r--   0 daveih     (501) staff       (20)      583 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_identifier.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/study_protocol_version.py
+-rw-r--r--   0 daveih     (501) staff       (20)      336 2023-04-11 13:59:38.000000 usdm-0.27.0/src/usdm_model/timing.py
+-rw-r--r--   0 daveih     (501) staff       (20)      134 2023-03-31 13:46:27.000000 usdm-0.27.0/src/usdm_model/transition_rule.py
+drwxr-xr-x   0 daveih     (501) staff       (20)        0 2023-05-17 10:33:50.721753 usdm-0.27.0/tests/
+-rw-r--r--   0 daveih     (501) staff       (20)    14241 2023-05-16 13:26:16.000000 usdm-0.27.0/tests/test_base_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2129 2023-04-05 14:43:30.000000 usdm-0.27.0/tests/test_cdisc_biomedical_concept.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1517 2023-05-08 13:47:22.000000 usdm-0.27.0/tests/test_configuration_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)      880 2023-05-17 09:18:36.000000 usdm-0.27.0/tests/test_error.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2234 2023-05-17 09:18:13.000000 usdm-0.27.0/tests/test_errors.py
+-rw-r--r--   0 daveih     (501) staff       (20)      811 2023-05-16 13:26:16.000000 usdm-0.27.0/tests/test_integration.py
+-rw-r--r--   0 daveih     (501) staff       (20)      971 2023-04-13 09:35:41.000000 usdm-0.27.0/tests/test_iso_3166.py
+-rw-r--r--   0 daveih     (501) staff       (20)      412 2023-04-05 14:06:46.000000 usdm-0.27.0/tests/test_ncit.py
+-rw-r--r--   0 daveih     (501) staff       (20)     1098 2023-05-08 13:47:22.000000 usdm-0.27.0/tests/test_option_manager.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3199 2023-05-08 14:51:48.000000 usdm-0.27.0/tests/test_study_design_activity_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     3320 2023-04-14 12:14:15.000000 usdm-0.27.0/tests/test_study_design_arm_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     2716 2023-04-14 12:14:15.000000 usdm-0.27.0/tests/test_study_design_epoch_sheet.py
+-rw-r--r--   0 daveih     (501) staff       (20)     4884 2023-05-16 13:26:16.000000 usdm-0.27.0/tests/test_study_identifiers_sheet.py
```

### Comparing `usdm-0.26.0/LICENSE` & `usdm-0.27.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/PKG-INFO` & `usdm-0.27.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usdm
-Version: 0.26.0
+Version: 0.27.0
 Summary: A python package for using the CDISC TransCelerate USDM
 Author: D Iberson-Hurst
 Author-email: 
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -77,17 +77,21 @@
 
 The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
 
 ### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
+### Multiple Values
+
+Some cells allow for multiple values. These are all comma separated. If users wish to include a comma within such strings then the string can be enclosed in quotes. For example `123, "123,456", 789`.
+
 ### External Terminology
 
-For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`.
+For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`. Where multiple codes are needed then the values are separated by commas.
 
 ### Boolean Values
 
 For boolean fields the following can be used to indicate a `true` value `'Y', 'YES', 'T', 'TRUE', '1'` or the lower case equivalents.
 
 ### Identifiers and Cross References
 
@@ -145,15 +149,15 @@
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
 | F | organisationAddress | The organisation address | Formated using a pipe delimited form, see below |
 
-The organisation address is of the form: ```line|city|district|state|postal_code|<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code.
+The organisation address is of the form: ```line,city,district,state,postal_code,<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. Note that `|` can be used in place of the commas for backward compatibility.
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -467,10 +471,16 @@
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
 | SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
 | SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
 | SDR Description | Allows for the description fields within the JSON to be fillled with a string value rather than being set to an empty string if they are left blank in the excel sheets. Currently only applies to description fields | A non-empty string such as `'-', 'not set'` etc |
 
-### Issues
+# Issues
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
+
+# Build Notes
+
+Build with `python3 -m build --sdist --wheel`
+
+Upload to pypi using `twine upload dist/* `
```

### Comparing `usdm-0.26.0/README.md` & `usdm-0.27.0/src/usdm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: usdm
+Version: 0.27.0
+Summary: A python package for using the CDISC TransCelerate USDM
+Author: D Iberson-Hurst
+Author-email: 
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
 
@@ -63,17 +77,21 @@
 
 The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
 
 ### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
+### Multiple Values
+
+Some cells allow for multiple values. These are all comma separated. If users wish to include a comma within such strings then the string can be enclosed in quotes. For example `123, "123,456", 789`.
+
 ### External Terminology
 
-For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`.
+For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`. Where multiple codes are needed then the values are separated by commas.
 
 ### Boolean Values
 
 For boolean fields the following can be used to indicate a `true` value `'Y', 'YES', 'T', 'TRUE', '1'` or the lower case equivalents.
 
 ### Identifiers and Cross References
 
@@ -131,15 +149,15 @@
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
 | F | organisationAddress | The organisation address | Formated using a pipe delimited form, see below |
 
-The organisation address is of the form: ```line|city|district|state|postal_code|<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code.
+The organisation address is of the form: ```line,city,district,state,postal_code,<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. Note that `|` can be used in place of the commas for backward compatibility.
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -453,10 +471,16 @@
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
 | SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
 | SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
 | SDR Description | Allows for the description fields within the JSON to be fillled with a string value rather than being set to an empty string if they are left blank in the excel sheets. Currently only applies to description fields | A non-empty string such as `'-', 'not set'` etc |
 
-### Issues
+# Issues
+
+See the [github issues](https://github.com/data4knowledge/usdm/issues)
+
+# Build Notes
+
+Build with `python3 -m build --sdist --wheel`
 
-See the [github issues](https://github.com/data4knowledge/usdm/issues)
+Upload to pypi using `twine upload dist/* `
```

### Comparing `usdm-0.26.0/setup.py` & `usdm-0.27.0/setup.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm.egg-info/PKG-INFO` & `usdm-0.27.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: usdm
-Version: 0.26.0
-Summary: A python package for using the CDISC TransCelerate USDM
-Author: D Iberson-Hurst
-Author-email: 
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CDISC / Transcelerate DDF USDM Package
 
 This package provides an implementation of the Digital Data Flow (DDF) CDISC / TransCelerate Unified Study Definitions Model (USDM). Two main parts are provided:
 
 - Within the `usdm_model` directory are a set of classes reflecting the USDM model as transported using the DDF USDM API 
 - Within the `usdm_excel` directory is a class, `USDMExcel`, that can be used to import an entire study definition from an excel file and build the equivalent json as defined by the API
 
@@ -77,17 +63,21 @@
 
 The content of each sheet is described below. Example workbooks can be found in the [CDISC Reference Architecture repo](https://github.com/cdisc-org/DDF-RA/tree/sprint-11/Deliverables/IG/examples). *Note: the link above points to the sprint 11 branch. This will be merged into the main branch prior to public review.*
 
 ### CDISC Terminology
 
 For those cells where CDISC codes are used the user can enter either the CDISC C Code, for example `C15602`, the CDISC submission value, for example `PHASE III TRIAL`, or the preferred term, for example `Phase III Trial`
 
+### Multiple Values
+
+Some cells allow for multiple values. These are all comma separated. If users wish to include a comma within such strings then the string can be enclosed in quotes. For example `123, "123,456", 789`.
+
 ### External Terminology
 
-For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`.
+For those cells where external CT is referenced the user can enter code in the form `<code system>: <code> = <decode>`. For example `SPONSOR: A = decode 1, SPONSOR: B = decode 2`. Where multiple codes are needed then the values are separated by commas.
 
 ### Boolean Values
 
 For boolean fields the following can be used to indicate a `true` value `'Y', 'YES', 'T', 'TRUE', '1'` or the lower case equivalents.
 
 ### Identifiers and Cross References
 
@@ -145,15 +135,15 @@
 | A | organisationIdentifierScheme | The scheme for the organisation identifier. | Example would be 'DUNS' |
 | B | organisationIdentifier | Organisation identifier | Text string |
 | C | organisationName | Organisation name | Text string |
 | D | organisationType | Organisation type | CDISC code reference |
 | E | studyIdentifier | The identifier for the study | Text string |
 | F | organisationAddress | The organisation address | Formated using a pipe delimited form, see below |
 
-The organisation address is of the form: ```line|city|district|state|postal_code|<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code.
+The organisation address is of the form: ```line,city,district,state,postal_code,<country code>```. All fields are text strings except for `<country code>`. `<country code>` is either a two or three character ISO-3166 country code. Note that `|` can be used in place of the commas for backward compatibility.
 
 ### Study Design sheet
 
 #### Sheet Name
 
 `studyDesign`
 
@@ -467,10 +457,16 @@
 | Parameter | Description | Format and Values |
 | :--- | :--- | :--- |
 | CT Version | Allows for the version of a specific external CT to be set. Multiple rows can be included to set the versions for several CTs | Of the form CT name = Version value, For example `SNOMED = 21st June 2012`|
 | SDR Prev Next | Allows for next and previous ids to be set to '' rather than null values so as to accomodate the SDR validation checks | Set to 'SDR' to use '' or leave empty to set null values |
 | SDR Root | Allows for the API specification complant JSON output to be wrpaped in a root "clinicalStudy" element so as to accomodate the SDR validation checks | Set to 'SDR' to use wrapper or leave empty to just generate the API compliant JSON |
 | SDR Description | Allows for the description fields within the JSON to be fillled with a string value rather than being set to an empty string if they are left blank in the excel sheets. Currently only applies to description fields | A non-empty string such as `'-', 'not set'` etc |
 
-### Issues
+# Issues
 
 See the [github issues](https://github.com/data4knowledge/usdm/issues)
+
+# Build Notes
+
+Build with `python3 -m build --sdist --wheel`
+
+Upload to pypi using `twine upload dist/* `
```

### Comparing `usdm-0.26.0/src/usdm.egg-info/SOURCES.txt` & `usdm-0.27.0/src/usdm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -108,8 +108,9 @@
 tests/test_errors.py
 tests/test_integration.py
 tests/test_iso_3166.py
 tests/test_ncit.py
 tests/test_option_manager.py
 tests/test_study_design_activity_sheet.py
 tests/test_study_design_arm_sheet.py
-tests/test_study_design_epoch_sheet.py
+tests/test_study_design_epoch_sheet.py
+tests/test_study_identifiers_sheet.py
```

### Comparing `usdm-0.26.0/src/usdm_excel/__init__.py` & `usdm-0.27.0/src/usdm_excel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import json
 from usdm_excel.id_manager import id_manager
 from usdm_excel.configuration_sheet import ConfigurationSheet
 from usdm_excel.study_sheet.study_sheet import StudySheet
 from usdm_excel.nodes_and_edges import NodesAndEdges
 from usdm_excel.cross_ref import cross_references
 from usdm_excel.ct_version_manager import ct_version_manager
-from usdm_excel.errors.errors import error_manager
+from usdm_excel.errors.errors import error_manager, Errors
 from usdm_excel.option_manager import option_manager as om # Using 'om' as a name clash in pytest
 from usdm_excel.cdisc_biomedical_concept import cdisc_bc_library
 
 class USDMExcel():
 
   FULL_VIEW = NodesAndEdges.FULL
   TIMELINE_VIEW = NodesAndEdges.TIMELINE
@@ -29,14 +30,20 @@
     else:
       return study.study_identifier()
 
   def the_study(self):
     return self.study.the_study()
   
   def to_json(self):
-    return self.study.api_root().to_json()
-
+    try:
+      raw_json = self.study.api_root().to_json()
+    except Exception as e:
+      message = f"Failed to generate JSON output, exception {e}"
+      error_manager.add(None, None, None, message)
+      raw_json = json.dumps({'error': message}, indent = 2)
+    return raw_json
+  
   def to_nodes_and_edges(self, view=FULL_VIEW):
     return NodesAndEdges(self.study.the_study(), view).nodes_and_edges()
 
   def errors(self):
-    return error_manager
+    return error_manager.dump(Errors.WARNING)
```

### Comparing `usdm-0.26.0/src/usdm_excel/base_sheet.py` & `usdm-0.27.0/src/usdm_excel/base_sheet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+import shlex
 import pandas as pd
 from openpyxl import load_workbook
 from usdm_excel.id_manager import id_manager
 from usdm_excel.cdisc_ct import CDISCCT
 from usdm_model.code import Code
 from usdm_excel.ct_version_manager import ct_version_manager
 from usdm_excel.errors.errors import error_manager
 from usdm_excel.logger import package_logger
 from usdm_excel.option_manager import *
 
 class BaseSheet():
 
+  class StateError(Exception):
+    pass
+
+  class FormatError(Exception):
+    pass
+
   def __init__(self, file_path, sheet_name, header=0, optional=False):
     self.file_path = file_path
     self.sheet_name = sheet_name
     if optional and not self._sheet_present(file_path, sheet_name):
       self.sheet = None
     else:
       self.sheet = pd.read_excel(open(file_path, 'rb'), sheet_name=sheet_name, header=header)
@@ -53,31 +60,37 @@
 
   def read_cell_empty(self, row_index, col_index, empty_character):
     value = self.read_cell(row_index, col_index)
     value = "" if value == empty_character else value
     return value
 
   def read_cell_multiple(self, rindex, cindex):
-    results = []
-    value = self.read_cell(rindex, cindex)
-    if value.strip() == '':
+    try:
+      results = []
+      value = self.read_cell(rindex, cindex)
+      if value.strip() == '':
+        return results
+      #for part in value.split(","):
+      for part in self._state_split(value):
+        results.append(part.strip())
       return results
-    for part in value.split(","):
-      results.append(part.strip())
-    return results
+    except BaseSheet.StateError as e:
+      self._error(rindex, cindex, f"Internal state error ({e}) reading cell")
+    except BaseSheet.FormatError as e:
+      self._error(rindex, cindex, "Format error reading cell, check the format of the cell")
 
   def read_cell_with_previous(self, row_index, col_index, first_col_index):
     try:
       i = col_index
       while i >= first_col_index:
         if pd.isnull(self.sheet.iloc[row_index, i]):
           i -= 1
         else:
           return self.sheet.iloc[row_index, i].strip()
-      self._error(row_index, col_index, "Blank cell error")
+      self._warning(row_index, col_index, "No previous non-empty cell found.")
       return ""
     except Exception as e:
       self._error(row_index, col_index, "Error (%s) reading cell row '%s', field '%s'" % (e, row_index, col_index))
       return ""
 
   def read_boolean_cell_by_name(self, row_index, field_name):
     value = self.read_cell_by_name(row_index, field_name)
@@ -118,16 +131,15 @@
     return self.read_other_code_cell_mutiple(row_index, col_index)
 
   def read_other_code_cell_mutiple(self, row_index, col_index):
     value = self.read_cell(row_index, col_index)
     result = []
     if value.strip() == '':
       return result
-    items = value.split(",")
-    for item in items:
+    for item in self._state_split(value):
       code = self._decode_other_code(item.strip(), row_index, col_index)
       if not code == None:
         result.append(code)
     return result
 
   def read_cdisc_klass_attribute_cell_by_name(self, klass, attribute, row_index, field_name):
     col_index = self.sheet.columns.get_loc(field_name)
@@ -150,16 +162,15 @@
 
   def read_cdisc_klass_attribute_cell_multiple(self, klass, attribute, row_index, col_index):
     result = []
     value = self.read_cell(row_index, col_index)
     if value.strip() == "":
       self._error(row_index, col_index, "Empty cell detected where multiple CDISC CT values expected.")
       return result
-    items = value.split(",")
-    for item in items:
+    for item in self._state_split(value):
       code = CDISCCT().code_for_attribute(klass, attribute, item.strip())
       if code is not None:
         result.append(code)
       else:
         self._error(row_index, col_index, f"CDISC CT not found for value '{item.strip()}'.")
     return result
 
@@ -231,7 +242,66 @@
     wb = load_workbook(file_path, read_only=True, keep_links=False)
     return wb.sheetnames
 
   def _sheet_present(self, file_path, sheet_name):
     sheet_names = self._get_sheet_names(file_path)
     return sheet_name in sheet_names
 
+  def _state_split(self, s):
+
+    OUT = "out"
+    IN_QUOTED = "in_quoted"
+    OUT_QUOTED = "out_quoted"
+    IN_NORMAL = "in_normal"
+    ESC = "escape"
+
+    state = OUT
+    result = []
+    current = []
+    exit = ""
+    for c in s:
+      if state == OUT:
+        current = []
+        if c in ['"', "'"]:
+          state = IN_QUOTED
+          exit = c
+        elif c.isspace():
+          pass
+        else:
+          state = IN_NORMAL
+          current.append(c)
+      elif state == IN_QUOTED:
+        if c == '\\':
+          state = ESC
+        elif c == exit:
+          result.append("".join(current).strip())
+          state = OUT_QUOTED
+        else:
+          current.append(c)
+      elif state == OUT_QUOTED:
+        if c == ',':
+          state = OUT
+        else:
+          pass
+      elif state == IN_NORMAL:
+        if c == ',':
+          result.append("".join(current).strip())
+          state = OUT
+        else:
+          current.append(c)
+      elif state == ESC:
+        if c == exit:
+          current.append(c)
+          state = IN_QUOTED
+        else:
+          current.append('\\')
+          current.append(c)
+      else:
+        raise BaseSheet.StateError
+
+    if state == OUT or state == OUT_QUOTED:
+      pass
+    elif state == IN_NORMAL:
+      result.append("".join(current).strip())
+    else:
+      raise BaseSheet.FormatError
+    return result
```

### Comparing `usdm-0.26.0/src/usdm_excel/cdisc_biomedical_concept.py` & `usdm-0.27.0/src/usdm_excel/cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/cdisc_ct.py` & `usdm-0.27.0/src/usdm_excel/cdisc_ct.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/cdisc_ct_library.py` & `usdm-0.27.0/src/usdm_excel/cdisc_ct_library.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/configuration_sheet.py` & `usdm-0.27.0/src/usdm_excel/configuration_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/data/cdisc_ct_config.yaml` & `usdm-0.27.0/src/usdm_excel/data/cdisc_ct_config.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/data/iso_3166.json` & `usdm-0.27.0/src/usdm_excel/data/iso_3166.json`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/data/missing_ct.yaml` & `usdm-0.27.0/src/usdm_excel/data/missing_ct.yaml`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/errors/errors.py` & `usdm-0.27.0/src/usdm_excel/errors/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from usdm_excel.logger import package_logger
 
 class Errors():
 
   WARNING = Error.WARNING
   ERROR = Error.ERROR
   DEBUG = Error.DEBUG
+  INFO = Error.INFO
 
   def __init__(self):
     self.items = []
 
   def clear(self):
     self.items = []
 
@@ -17,14 +18,15 @@
     error = Error(sheet, row, column, message, level)
     self.items.append(error)      
     package_logger.log(level, error.to_log())
 
   def count(self) -> int:
     return len(self.items)
   
-  def dump(self):
+  def dump(self, level):
     result = []
     for item in self.items:
-      result.append(item.__dict__)
+      if item.level >= level:
+        result.append(item.to_dict())
     return result
 
 error_manager = Errors()
```

### Comparing `usdm-0.26.0/src/usdm_excel/id_manager.py` & `usdm-0.27.0/src/usdm_excel/id_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/iso_3166.py` & `usdm-0.27.0/src/usdm_excel/iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/nodes_and_edges.py` & `usdm-0.27.0/src/usdm_excel/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/option_manager.py` & `usdm-0.27.0/src/usdm_excel/option_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_activity_sheet/study_design_activity_sheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,25 @@
       self.items = []
       if self.sheet is not None:
         for index, row in self.sheet.iterrows():
           name = self.read_cell_by_name(index, 'activityName')
           description = self.read_description_by_name(index, 'activityDescription')
           conditional = self.read_boolean_cell_by_name(index, 'activityIsConditional')
           reason = self.read_cell_by_name(index, 'activityIsConditionalReason')
-          item = Activity(
-            activityId=id_manager.build_id(Activity), 
-            activityName=name,
-            activityDescription=description,
-            activityIsConditional=conditional,
-            activityIsConditionalReason=reason
-          )
-          self.items.append(item)
-          cross_references.add(name, item)     
+          try:
+            item = Activity(
+              activityId=id_manager.build_id(Activity), 
+              activityName=name,
+              activityDescription=description,
+              activityIsConditional=conditional,
+              activityIsConditionalReason=reason
+            )
+          except Exception as e:
+            self._general_error(f"Failed to create Activity object, exception {e}")
+          else:
+            self.items.append(item)
+            cross_references.add(name, item)     
         self.double_link(self.items, 'activityId', 'previousActivityId', 'nextActivityId')   
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_element_sheet/study_design_element_sheet.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,20 +21,24 @@
         description = self.read_description_by_name(index, 'studyElementDescription')
         start_rule_text = self.read_cell_by_name(index, 'transitionStartRule')
         end_rule_text = self.read_cell_by_name(index, 'transitionEndRule')
         if not start_rule_text == "":
           start_rule = TransitionRule(transitionRuleId=id_manager.build_id(TransitionRule), transitionRuleDescription=start_rule_text)
         if not end_rule_text == "":
           end_rule = TransitionRule(transitionRuleId=id_manager.build_id(TransitionRule), transitionRuleDescription=end_rule_text)
-        item = StudyElement(
-          studyElementId=id_manager.build_id(StudyElement), 
-          studyElementName=name,
-          studyElementDescription=description,
-          transitionStartRule=start_rule,
-          transitionEndRule=end_rule
-        )
-        self.items.append(item)
-        cross_references.add(xref, item)     
+        try:
+          item = StudyElement(
+            studyElementId=id_manager.build_id(StudyElement), 
+            studyElementName=name,
+            studyElementDescription=description,
+            transitionStartRule=start_rule,
+            transitionEndRule=end_rule
+          )
+        except Exception as e:
+          self._general_error(f"Failed to create StudyElement object, exception {e}")
+        else:
+          self.items.append(item)
+          cross_references.add(xref, item)     
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_encounter_sheet/study_design_encounter_sheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,28 @@
         modes = self.read_cdisc_klass_attribute_cell_multiple_by_name('Encounter', 'encounterContactModes', index, 'encounterContactModes')
         start_rule_text = self.read_cell_by_name(index, 'transitionStartRule')
         end_rule_text = self.read_cell_by_name(index, 'transitionEndRule')
         if not start_rule_text == "":
           start_rule = TransitionRule(transitionRuleId=id_manager.build_id(TransitionRule), transitionRuleDescription=start_rule_text)
         if not end_rule_text == "":
           end_rule = TransitionRule(transitionRuleId=id_manager.build_id(TransitionRule), transitionRuleDescription=end_rule_text)
-        item = Encounter(
-          encounterId=id_manager.build_id(Encounter), 
-          encounterName=name,
-          encounterDescription=description,
-          encounterType=type, 
-          encounterEnvironmentalSetting=setting,
-          encounterContactModes=modes,
-          transitionStartRule=start_rule,
-          transitionEndRule=end_rule
-        )
-        self.items.append(item)
-        cross_references.add(xref, item)     
+        try:
+          item = Encounter(
+            encounterId=id_manager.build_id(Encounter), 
+            encounterName=name,
+            encounterDescription=description,
+            encounterType=type, 
+            encounterEnvironmentalSetting=setting,
+            encounterContactModes=modes,
+            transitionStartRule=start_rule,
+            transitionEndRule=end_rule
+          )
+        except Exception as e:
+          self._general_error(f"Failed to create Encounter object, exception {e}")
+        else:
+          self.items.append(item)
+          cross_references.add(xref, item)     
       self.double_link(self.items, 'encounterId', 'previousEncounterId', 'nextEncounterId')   
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_epoch_sheet/study_design_epoch_sheet.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,22 @@
     try:
       super().__init__(file_path=file_path, sheet_name='studyDesignEpochs')
       self.items = []
       for index, row in self.sheet.iterrows():
         name = self.read_cell_by_name(index, 'studyEpochName')
         description = self.read_description_by_name(index, 'studyEpochDescription')
         epoch_type = self.read_cdisc_klass_attribute_cell_by_name('StudyEpoch', 'studyEpochType', index, 'studyEpochType')
-        item = StudyEpoch(
-          studyEpochId=id_manager.build_id(StudyEpoch), 
-          studyEpochName=name, 
-          studyEpochDescription=description,
-          studyEpochType=epoch_type
-        )
-        self.items.append(item)
-        cross_references.add(name, item)     
+        try:
+          item = StudyEpoch(
+            studyEpochId=id_manager.build_id(StudyEpoch), 
+            studyEpochName=name, 
+            studyEpochDescription=description,
+            studyEpochType=epoch_type
+          )
+        except Exception as e:
+          self._general_error(f"Failed to create StudyEpoch object, exception {e}")
+        else:
+          self.items.append(item)
+          cross_references.add(name, item)     
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_estimands_sheet/study_design_estimands_sheet.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,31 +9,46 @@
 from usdm_excel.cdisc_ct_library import cdisc_ct_library
 from usdm_excel.cdisc_ct import CDISCCT
 
 class StudyDesignEstimandsSheet(BaseSheet):
 
   def __init__(self, file_path):
     try:
-      #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyDesignEstimands'))
       super().__init__(file_path=file_path, sheet_name='studyDesignEstimands')
       self.estimands = []
       current = None
       for index, row in self.sheet.iterrows():
         e_summary = self.read_cell_by_name(index, "summaryMeasure")
         ap_description = self.read_description_by_name(index, 'populationDescription')
         ice_name = self.read_cell_by_name(index, "intercurrentEventName")
         ice_description = self.read_description_by_name(index, 'intercurrentEventDescription')
         ice_strategy = self.read_cell_by_name(index, "intercurrentEventStrategy")
         treatment_xref = self.read_cell_by_name(index, "treatmentXref")
         treatment_id = cross_references.get(treatment_xref)
         endpoint_xref = self.read_cell_by_name(index, "endpointXref")
         endpoint_id = cross_references.get(endpoint_xref)
         if not e_summary == "":
-          ap = AnalysisPopulation(analysisPopulationId=id_manager.build_id(AnalysisPopulation), populationDescription=ap_description) 
-          current = Estimand(estimandId=id_manager.build_id(Estimand), summaryMeasure=e_summary, analysisPopulation=ap, treatment=treatment_id, variableOfInterest=endpoint_id, intercurrentEvents=[])
-          self.estimands.append(current)  
-        ice = IntercurrentEvent(intercurrentEventId=id_manager.build_id(IntercurrentEvent), intercurrentEventName=ice_name, intercurrentEventDescription=ice_description, intercurrentEventStrategy=ice_strategy)
-        current.intercurrentEvents.append(ice)
+          try:
+            ap = AnalysisPopulation(analysisPopulationId=id_manager.build_id(AnalysisPopulation), populationDescription=ap_description) 
+          except Exception as e:
+            self._general_error(f"Failed to create AnalysisPopulation object, exception {e}")
+          else:
+            try:
+              current = Estimand(estimandId=id_manager.build_id(Estimand), summaryMeasure=e_summary, analysisPopulation=ap, treatment=treatment_id, variableOfInterest=endpoint_id, intercurrentEvents=[])
+            except Exception as e:
+              self._general_error(f"Failed to create Estimand object, exception {e}")
+            else:
+              self.estimands.append(current)  
+        if current is not None:
+          try:
+            ice = IntercurrentEvent(intercurrentEventId=id_manager.build_id(IntercurrentEvent), intercurrentEventName=ice_name, intercurrentEventDescription=ice_description, intercurrentEventStrategy=ice_strategy)
+          except Exception as e:
+            self._general_error(f"Failed to create IntercurrentEvent object, exception {e}")
+          else:
+            current.intercurrentEvents.append(ice)
+        else:
+          self._general_error("Failed to add IntercurrentEvent, no Estimand set")
+
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_ii_sheet/study_design_ii_sheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,18 +17,26 @@
       for index, row in self.sheet.iterrows():
         xref = self.read_cell_by_name(index, "xref")
         type = self.read_cell_by_name(index, "type")
         description = self.read_description_by_name(index, "description")
         #codes = self._build_codes(row, index)
         codes = self.read_other_code_cell_multiple_by_name(index, "codes")
         if type.upper() == "IND":
-          item = Indication(indicationId=id_manager.build_id(Indication), indicationDescription=description, codes=codes)
-          self.indications.append(item)
-          cross_references.add(xref, item.indicationId)
+          try:
+            item = Indication(indicationId=id_manager.build_id(Indication), indicationDescription=description, codes=codes)
+          except Exception as e:
+            self._general_error(f"Failed to create Indication object, exception {e}")
+          else:
+            self.indications.append(item)
+            cross_references.add(xref, item.indicationId)
         else:
-          item = InvestigationalIntervention(investigationalInterventionId=id_manager.build_id(InvestigationalIntervention), interventionDescription=description, codes=codes)
-          self.interventions.append(item)
-          cross_references.add(xref, item.investigationalInterventionId)        
+          try:
+            item = InvestigationalIntervention(investigationalInterventionId=id_manager.build_id(InvestigationalIntervention), interventionDescription=description, codes=codes)
+          except Exception as e:
+            self._general_error(f"Failed to create InvestigationalIntervention object, exception {e}")
+          else:
+            self.interventions.append(item)
+            cross_references.add(xref, item.investigationalInterventionId)        
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_objective_endpoint_sheet/study_design_objective_endpoint_sheet.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,26 +18,37 @@
         o_description = self.read_cell_by_name(index, 'objectiveDescription') # Note, dont use description read method, we need to know if really empty.
         e_xref = self.read_cell_by_name(index, "endpointXref")
         e_description = self.read_description_by_name(index, 'endpointDescription')
         e_p_description = self.read_description_by_name(index, 'endpointPurposeDescription')
         e_level = self.read_cdisc_klass_attribute_cell_by_name('Endpoint', 'endpointLevel', index, "endpointLevel")
         if not o_description == "":
           o_level = self.read_cdisc_klass_attribute_cell_by_name('Objective', 'objectiveLevel', index, "objectiveLevel")
-          current = Objective(objectiveId=id_manager.build_id(Objective),
-            objectiveDescription=o_description, 
-            objectiveLevel=o_level,
-            objectiveEndpoints=[]
-          )
-          self.objectives.append(current)
-          cross_references.add(o_xref, current.objectiveId)
-        ep = Endpoint(endpointId=id_manager.build_id(Endpoint), 
-          endpointDescription=e_description, 
-          endpointPurposeDescription=e_p_description, 
-          endpointLevel=e_level
-        )  
-        current.objectiveEndpoints.append(ep)
-        cross_references.add(e_xref, ep.endpointId)
-        
+          try:
+            current = Objective(objectiveId=id_manager.build_id(Objective),
+              objectiveDescription=o_description, 
+              objectiveLevel=o_level,
+              objectiveEndpoints=[]
+            )
+          except Exception as e:
+            self._general_error(f"Failed to create Objective object, exception {e}")
+          else:
+            self.objectives.append(current)
+            cross_references.add(o_xref, current.objectiveId)
+        if current is not None:
+          try:
+            ep = Endpoint(endpointId=id_manager.build_id(Endpoint), 
+              endpointDescription=e_description, 
+              endpointPurposeDescription=e_p_description, 
+              endpointLevel=e_level
+            )  
+          except Exception as e:
+            self._general_error(f"Failed to create Endpoint object, exception {e}")
+          else:
+            current.objectiveEndpoints.append(ep)
+            cross_references.add(e_xref, ep.endpointId)
+        else:
+          self._general_error("Failed to add Endpoint, no Objective set")
+
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_population_sheet/study_design_population_sheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,23 +13,26 @@
       self.populations = []
       for index, row in self.sheet.iterrows():
         description = self.read_description_by_name(index, 'populationDescription')
         number = self.read_cell_by_name(index, "plannedNumberOfParticipants")
         min = self.read_cell_by_name(index, "plannedMinimumAgeOfParticipants")
         max = self.read_cell_by_name(index, "plannedMaximumAgeOfParticipants")
         codes = self._build_codes(row, index)
-        self.populations.append(
-          StudyDesignPopulation(studyDesignPopulationId=id_manager.build_id(StudyDesignPopulation), 
+        try:
+          pop = StudyDesignPopulation(studyDesignPopulationId=id_manager.build_id(StudyDesignPopulation), 
             populationDescription=description, 
             plannedNumberOfParticipants=number,
             plannedMinimumAgeOfParticipants=min,
             plannedMaximumAgeOfParticipants=max,
             codes=codes
           )
-        )
+        except:
+          self._general_error(f"Failed to create StudyDesignPopulation object, exception {e}")
+        else:
+          self.populations.append(pop)
         
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
 
 
   def _build_codes(self, row, index):
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_procedure_sheet/study_design_procedure_sheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,24 @@
         xref = self.read_cell_by_name(index, "xref")
         name = self.read_cell_by_name(index, "procedureName")
         description = self.read_description_by_name(index, 'procedureDescription')
         type = self.read_cell_by_name(index, "procedureType")
         code = self.read_other_code_cell_by_name(index, 'procedureCode')
         conditional = self.read_boolean_cell_by_name(index, 'procedureIsConditional')
         reason = self.read_cell_by_name(index, 'procedureIsConditionalReason')
-        item = Procedure(procedureId=id_manager.build_id(Procedure),
-          procedureName=name,
-          procedureDescription=description,
-          procedureType=type, 
-          procedureCode=code, 
-          procedureIsConditional=conditional, 
-          procedureIsConditionalReason=reason
-        )
-        self.procedures.append(item)
-        cross_references.add(xref, item)        
+        try:
+          item = Procedure(procedureId=id_manager.build_id(Procedure),
+            procedureName=name,
+            procedureDescription=description,
+            procedureType=type, 
+            procedureCode=code, 
+            procedureIsConditional=conditional, 
+            procedureIsConditionalReason=reason
+          )
+        except:
+          self._general_error(f"Failed to create Procedure object, exception {e}")
+        else:
+          self.procedures.append(item)
+          cross_references.add(xref, item)        
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_design_sheet/study_design_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_design_sheet/study_design_sheet.py`

 * *Files 16% similar despite different names*

```diff
@@ -69,31 +69,42 @@
       elif rindex == self.MAIN_TIMELINE_ROW:
         self.main_timeline = self.read_cell(rindex, self.PARAMS_DATA_COL)
       elif rindex == self.OTHER_TIMELINES_ROW:
         self.other_timelines = self.read_cell_multiple(rindex, self.PARAMS_DATA_COL)
       else:
         pass
 
+    resolved_epochs = [None] * self.sheet.shape[1] 
+    resolved_arms = [None] * self.sheet.shape[0] 
     for rindex, row in self.sheet.iterrows():
       if rindex >= self.EPOCH_ARMS_START_ROW:
         for cindex in range(0, len(self.sheet.columns)):
+          epoch_index = cindex - 1
           cell = self.read_cell(rindex, cindex)
           if rindex == self.EPOCH_ARMS_START_ROW:
             if cindex != 0:
-              epoch = self._add_epoch(cell)
-              self.epochs.append(epoch)
+              resolved_epochs[epoch_index] = self._add_epoch(cell)
           else:
+            arm_index = rindex - self.EPOCH_ARMS_START_ROW - 1
             if cindex == 0:
-              self.arms.append(self._add_arm(cell))
+              resolved_arms[arm_index] = self._add_arm(cell)
             else:
               elements = []
               element_names = self.read_cell_multiple(rindex, cindex)
               for name in element_names:
-                elements.append(cross_references.get(name))
-              self.cells.append(self._add_cell(arm=self.arms[-1], epoch=self.epochs[cindex-1], elements=elements))
+                element = self._add_element(name)
+                if element is not None:
+                  elements.append(element)
+              arm = resolved_arms[arm_index]
+              epoch = resolved_epochs[epoch_index]
+              if arm is not None and epoch is not None:
+                self.cells.append(self._add_cell(arm=arm, epoch=epoch, elements=elements))
+              else:
+                self._general_error(f"Cannot resolve arms and/or epoch for cell [{arm_index + 1},{epoch_index + 1}]")
+              
     
     self.double_link(self.epochs, 'studyEpochId', 'previousStudyEpochId', 'nextStudyEpochId')
 
     study_design = self._add_design(
       name=self.name,
       description=self.description,
       cells=self.cells, 
@@ -103,19 +114,39 @@
       rationale=self.rationale, 
       blinding=self.blinding, 
       therapeutic_areas=self.therapeutic_areas
     )
     self.study_designs.append(study_design)
 
   def _add_arm(self, name):
-    return cross_references.get(name)
+    arm = cross_references.get(name)
+    if arm is not None:
+      self.arms.append(arm)
+      return arm
+    else:
+      self._general_error(f"No arm definition found for arm '{name}'")
+      return None
 
   def _add_epoch(self, name):
-    return cross_references.get(name)
+    epoch = cross_references.get(name)
+    if epoch is not None:
+      self.epochs.append(epoch)
+      return epoch
+    else:
+      self._general_error(f"No epoch definition found for epoch '{name}'")
+      return None
   
+  def _add_element(self, name):
+    element = cross_references.get(name)
+    if element is not None:
+      return element
+    else:
+      self._general_error(f"No element definition found for element '{name}'")
+      return None
+
   def _add_cell(self, arm, epoch, elements):
     return StudyCell(
       studyCellId=id_manager.build_id(StudyCell), 
       studyArm=arm,
       studyEpoch=epoch,
       studyElements=elements
     )
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_identifiers_sheet/study_identifiers_sheet.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,53 +7,74 @@
 import pandas as pd
 import traceback
 
 class StudyIdentifiersSheet(BaseSheet):
 
   def __init__(self, file_path: str):
     try:
-      #super().__init__(pd.read_excel(open(file_path, 'rb'), sheet_name='studyIdentifiers'))
       super().__init__(file_path=file_path, sheet_name='studyIdentifiers')
       self.identifiers = []
       self.process_sheet()
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
       
   def process_sheet(self):
     self.identifiers = []
     for index, row in self.sheet.iterrows():
-      organisation_type = self.read_cdisc_klass_attribute_cell_by_name('Organisation', 'organisationType', index, 'organisationType')
-      raw_address=self.read_cell_by_name(index, 'organisationAddress')
-      organisation = Organisation(
-        organisationId=id_manager.build_id(Organisation),
-        organisationIdentifierScheme=self.read_cell_by_name(index, 'organisationIdentifierScheme'), 
-        organisationIdentifier=self.read_cell_by_name(index, 'organisationIdentifier'),
-        organisationName=self.read_cell_by_name(index, 'organisationName'),
-        organisationType=organisation_type,
-        organizationLegalAddress=self._build_address(raw_address)
-      )
-      self.identifiers.append(StudyIdentifier(
-        studyIdentifierId=id_manager.build_id(StudyIdentifier),
-        studyIdentifier=self.read_cell_by_name(index, 'studyIdentifier'), 
-        studyIdentifierScope=organisation)
-      )
+      organisation_type = self.read_cdisc_klass_attribute_cell_by_name('Organisation', 'organisationType', index, 'organisationType')     
+      try:
+        organisation = Organisation(
+          organisationId=id_manager.build_id(Organisation),
+          organisationIdentifierScheme=self.read_cell_by_name(index, 'organisationIdentifierScheme'), 
+          organisationIdentifier=self.read_cell_by_name(index, 'organisationIdentifier'),
+          organisationName=self.read_cell_by_name(index, 'organisationName'),
+          organisationType=organisation_type,
+          organizationLegalAddress=self._build_address(index)
+        )
+      except Exception as e:
+        self._general_error(f"Failed to create Organisation object, exception {e}")
+      else:
+        try:
+          self.identifiers.append(StudyIdentifier(
+            studyIdentifierId=id_manager.build_id(StudyIdentifier),
+            studyIdentifier=self.read_cell_by_name(index, 'studyIdentifier'), 
+            studyIdentifierScope=organisation)
+          )
+        except Exception as e:
+          self._general_error(f"Failed to create StudyIdentifier object, exception {e}")
     
-  def _build_address(self, raw_address):
-    parts = raw_address.split("|")
+  def _build_address(self, row_index):
+    field_name = 'organisationAddress'
+    raw_address = self.read_cell_by_name(row_index, field_name)
+    # The '|' separator is preserved for legacy reasons but should be removed in the future
+    if '|' in raw_address:
+      sep = '|'
+      parts = raw_address.split(sep)
+    else:
+      sep = ','
+      parts = self._state_split(raw_address)
     if len(parts) == 6:
-      return self._to_address(
-            id_manager.build_id(Address),
-            parts[0].strip(), 
-            parts[1].strip(), 
-            parts[2].strip(), 
-            parts[3].strip(), 
-            parts[4].strip(), 
-            ISO3166().code(parts[5].strip())
-          )
+      result = self._to_address(
+          id_manager.build_id(Address),
+          parts[0].strip(), 
+          parts[1].strip(), 
+          parts[2].strip(), 
+          parts[3].strip(), 
+          parts[4].strip(), 
+          ISO3166().code(parts[5].strip())
+        )
+      return result
     else:
+      col_index = self.sheet.columns.get_loc(field_name)
+      self._error(row_index, col_index, f"Address does not contain the required fields (line, city, district, state, postal code and country code) using '{sep}' separator characters, only {len(parts)} found")
       return None
 
   def _to_address(self, id, line, city, district, state, postal_code, country):
     text = "%s, %s, %s, %s, %s, %s" % (line, city, district, state, postal_code, country.decode)
     text = text.replace(' ,', '')
-    return Address(addressId=id, text=text, line=line, city=city, district=district, state=state, postalCode=postal_code, country=country)
+    try:
+      result = Address(addressId=id, text=text, line=line, city=city, district=district, state=state, postalCode=postal_code, country=country)
+    except Exception as e:
+      self._general_error(f"Failed to create Address object, exception {e}")
+      result = None
+    return result
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_sheet/study_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_sheet/study_sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,19 @@
       self.soa = StudySoASheet(file_path, self.study_design.main_timeline)
       self.ii = StudyDesignIISheet(file_path)
       self.study_populations = StudyDesignPopulationSheet(file_path)
       self.oe = StudyDesignObjectiveEndpointSheet(file_path)
       self.estimands = StudyDesignEstimandsSheet(file_path)
 
       for epoch in self.study_design.epochs:
-        epoch.encounterIds = self.soa.epoch_encounter_map(epoch.studyEpochName)
+        ids = self.soa.epoch_encounter_map(epoch.studyEpochName)
+        if ids is not None:
+          epoch.encounterIds = ids
+        else:
+          self._general_info(f"No encounters found for epoch '{epoch.studyEpochName}'")
 
       study_design = self.study_design.study_designs[0]
       study_design.studyScheduleTimelines.append(self.soa.timeline)
       study_design.encounters = self.encounters.items
       study_design.activities = self.soa.activities
       study_design.biomedicalConcepts = self.soa.biomedical_concepts
       study_design.bcSurrogates = self.soa.biomedical_concept_surrogates
@@ -90,27 +94,30 @@
         study_design.bcSurrogates += tl.biomedical_concept_surrogates
       study_design.studyIndications = self.ii.indications
       study_design.studyInvestigationalInterventions = self.ii.interventions
       study_design.studyPopulations = self.study_populations.populations
       study_design.studyObjectives = self.oe.objectives
       study_design.studyEstimands = self.estimands.estimands
 
-      self.study = Study(
-        studyId=None, # No Id, will be allocated a UUID
-        studyTitle=self.title,
-        studyVersion=self.version,
-        studyType=self.type,
-        studyPhase=self.phase,
-        businessTherapeuticAreas=self.therapeutic_areas,
-        studyRationale=self.rationale,
-        studyAcronym=self.acronym,
-        studyIdentifiers=self.study_identifiers.identifiers,
-        studyProtocolVersions=self.protocols,
-        studyDesigns=self.study_design.study_designs
-      )
+      try:
+        self.study = Study(
+          studyId=None, # No Id, will be allocated a UUID
+          studyTitle=self.title,
+          studyVersion=self.version,
+          studyType=self.type,
+          studyPhase=self.phase,
+          businessTherapeuticAreas=self.therapeutic_areas,
+          studyRationale=self.rationale,
+          studyAcronym=self.acronym,
+          studyIdentifiers=self.study_identifiers.identifiers,
+          studyProtocolVersions=self.protocols,
+          studyDesigns=self.study_design.study_designs
+        )
+      except:
+        self._general_error(f"Failed to create Study object, exception {e}")
     except Exception as e:
       self._general_error(f"Exception [{e}] raised reading sheet.")
       self._traceback(f"{traceback.format_exc()}")
 
   def study_sponsor(self):
     return self.cdisc_code(code="C93453", decode="Study Registry")
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_soa_sheet/activities.py` & `usdm-0.27.0/src/usdm_excel/study_soa_sheet/activities.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/study_soa_sheet/activity.py` & `usdm-0.27.0/src/usdm_excel/study_soa_sheet/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/study_soa_sheet/cycle.py` & `usdm-0.27.0/src/usdm_excel/study_soa_sheet/cycle.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/study_soa_sheet/cycles.py` & `usdm-0.27.0/src/usdm_excel/study_soa_sheet/cycles.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/study_soa_sheet/encounters.py` & `usdm-0.27.0/src/usdm_excel/study_soa_sheet/encounters.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,8 +16,11 @@
         if not self.xref == "":
           encounter = cross_references.get(self.xref)
           if self.epoch not in self._epoch_map:
             self._epoch_map[self.epoch] = []
           self._epoch_map[self.epoch].append(encounter.encounterId)
 
   def epoch_encounter_map(self, epoch):
-    return self._epoch_map[epoch]
+    if epoch in self._epoch_map:
+      return self._epoch_map[epoch]
+    else:
+      return None
```

### Comparing `usdm-0.26.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py` & `usdm-0.27.0/src/usdm_excel/study_soa_sheet/study_soa_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/study_soa_sheet/timepoint.py` & `usdm-0.27.0/src/usdm_excel/study_soa_sheet/timepoint.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_excel/study_soa_sheet/timepoints.py` & `usdm-0.27.0/src/usdm_excel/study_soa_sheet/timepoints.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/__init__.py` & `usdm-0.27.0/src/usdm_model/__init__.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/activity.py` & `usdm-0.27.0/src/usdm_model/activity.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/api_base_model.py` & `usdm-0.27.0/src/usdm_model/api_base_model.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/encounter.py` & `usdm-0.27.0/src/usdm_model/encounter.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/estimand.py` & `usdm-0.27.0/src/usdm_model/estimand.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/scheduled_instance.py` & `usdm-0.27.0/src/usdm_model/scheduled_instance.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/study.py` & `usdm-0.27.0/src/usdm_model/study.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/study_design.py` & `usdm-0.27.0/src/usdm_model/study_design.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/src/usdm_model/study_identifier.py` & `usdm-0.27.0/src/usdm_model/study_identifier.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/tests/test_base_sheet.py` & `usdm-0.27.0/tests/test_base_sheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,22 +120,31 @@
   assert mock_error.call_args[0][1] == 2
   assert mock_error.call_args[0][2] == -1
   assert mock_error.call_args[0][3] == "Error ('Not There') reading cell"
   
 def test_read_cell_multiple(mocker):
   mocked_open = mocker.mock_open(read_data="File")
   mocker.patch("builtins.open", mocked_open)
-  data = [['tom', ''], ['nick', 'Sam'], ['juli', ' Fred, Dick,   Harry  '], ['andy', 'John  , Jane']]
+  data = [
+    ['tom', ''], 
+    ['nick', 'Sam'], 
+    ['juli', ' Fred, Dick,   Harry  '], 
+    ['andy', 'John  , Jane'], 
+    ['andy', '"John, & Fred", Jane'],
+    ['andy', '"John, \\" & Fred", Jane']
+  ]
   mock_read = mocker.patch("pandas.read_excel")
   mock_read.return_value = pd.DataFrame(data, columns=['Name', 'Children'])
   base = BaseSheet("", "sheet")
   test_data = [
     (0,1,[]),
     (2,1,['Fred', 'Dick', 'Harry']),
-    (3,1,['John', 'Jane'])
+    (3,1,['John', 'Jane']),
+    (4,1,['John, & Fred', 'Jane']),
+    (5,1,['John, " & Fred', 'Jane'])
   ]
   for test in test_data:
     assert(base.read_cell_multiple(test[0],test[1])) == test[2]
 
 # read_cell_with_previous
 
 def test_read_boolean_cell_by_name(mocker):
@@ -328,7 +337,27 @@
     assert(base._decode_other_code(test[0], test[1], test[2])) == test[3]
     if not test[4] == "":
       mock_error.assert_called()
       assert mock_error.call_args[0][0] == test[4]
       assert mock_error.call_args[0][1] == test[5]
       assert mock_error.call_args[0][2] == test[6]
       assert mock_error.call_args[0][3] == test[7]
+
+def test__state_split(mocker):
+  mocked_open = mocker.mock_open(read_data="File")
+  mocker.patch("builtins.open", mocked_open)
+  data = []
+  mock_read = mocker.patch("pandas.read_excel")
+  mock_read.return_value = pd.DataFrame(data)
+  base = BaseSheet("", "sheet")
+  test_data = [
+    ('111', ['111']),
+    ('111,    ', ['111']),
+    ('"111", 222, 333', ['111', '222', '333']),
+    ('"111", 222, 333, "4"', ['111', '222', '333', '4']),
+    ('"111 \\" quote", 222, 333', ['111 " quote', '222', '333'])
+  ]
+  for test in test_data:
+    assert(base._state_split(test[0])) == test[1]
+
+  with pytest.raises(BaseSheet.FormatError):
+    base._state_split('123, "456')
```

### Comparing `usdm-0.26.0/tests/test_cdisc_biomedical_concept.py` & `usdm-0.27.0/tests/test_cdisc_biomedical_concept.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/tests/test_configuration_sheet.py` & `usdm-0.27.0/tests/test_configuration_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/tests/test_errors.py` & `usdm-0.27.0/tests/test_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,22 @@
-from src.usdm_excel.errors.errors import Errors
+import pytest
 
-def test_create():
-  errors = Errors()
-  assert errors.items == []
+from src.usdm_excel.errors.error import Error
 
-def test_add():
-  errors = Errors()
-  assert len(errors.items) == 0
-  errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX")
-  assert len(errors.items) == 1
-  assert errors.items[0].message == "XXXXX"
-    
-def test_count():
-  errors = Errors()
-  errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX")
-  errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX")
-  assert errors.count() == 2
+def test_create():
+  error = Error(sheet="My Sheet", row=1, column=99, message="XXXXX")
+  assert error.sheet == "My Sheet"
+  assert error.row == 1
+  assert error.column == 99
+  assert error.message == "XXXXX"
 
-def test_clear():
-  errors = Errors()
-  assert len(errors.items) == 0
-  errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX")
-  assert len(errors.items) == 1
-  errors.clear()
-  assert len(errors.items) == 0
+def test_to_log():
+  error = Error(sheet="My Sheet", row=1, column=99, message="XXXXX")
+  assert(error.to_log()) == "Error in sheet My Sheet at [1,99]: XXXXX"
+  error = Error(sheet="My Sheet", row=None, column=None, message="XXXXX")
+  assert(error.to_log()) == "Error in sheet My Sheet: XXXXX"
+  error = Error(sheet=None, row=None, column=None, message="XXXXX")
+  assert(error.to_log()) == "Error: XXXXX"
 
-def test_dumo():
-  errors = Errors()
-  errors.add(sheet="My Sheet", row=1, column=99, message="XXXXX1")
-  errors.add(sheet="My Sheet", row=2, column=100, message="XXXXX2")
-  assert (errors.dump()) == [
-    {'sheet': 'My Sheet', 'row': 1, 'column': 99, 'message': 'XXXXX1', 'level': 40},
-    {'sheet': 'My Sheet', 'row': 2, 'column': 100, 'message': 'XXXXX2', 'level': 40}
-  ]
+def test_to_dict():
+  error = Error(sheet="My Sheet", row=1, column=99, message="XXXXX")
+  assert(error.to_dict()) == {'sheet': 'My Sheet', 'row': 1, 'column': 99, 'message': 'XXXXX', 'level': 'Error'}
```

### Comparing `usdm-0.26.0/tests/test_integration.py` & `usdm-0.27.0/tests/test_integration.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,7 +18,10 @@
   run_test('config_1')
 
 def test_config_2():
   run_test('config_2')
 
 def test_no_activity_sheet():
   run_test('no_activity_sheet')
+
+def test_address_comma():
+  run_test('address')
```

### Comparing `usdm-0.26.0/tests/test_iso_3166.py` & `usdm-0.27.0/tests/test_iso_3166.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/tests/test_option_manager.py` & `usdm-0.27.0/tests/test_option_manager.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/tests/test_study_design_activity_sheet.py` & `usdm-0.27.0/tests/test_study_design_activity_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/tests/test_study_design_arm_sheet.py` & `usdm-0.27.0/tests/test_study_design_arm_sheet.py`

 * *Files identical despite different names*

### Comparing `usdm-0.26.0/tests/test_study_design_epoch_sheet.py` & `usdm-0.27.0/tests/test_study_design_epoch_sheet.py`

 * *Files identical despite different names*

