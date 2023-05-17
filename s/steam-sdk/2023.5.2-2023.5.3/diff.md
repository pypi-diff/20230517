# Comparing `tmp/steam-sdk-2023.5.2.tar.gz` & `tmp/steam-sdk-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-sdk-2023.5.2.tar", last modified: Thu May 11 20:05:11 2023, max compression
+gzip compressed data, was "dist\steam-sdk-2023.5.3.tar", last modified: Wed May 17 07:33:20 2023, max compression
```

## Comparing `steam-sdk-2023.5.2.tar` & `steam-sdk-2023.5.3.tar`

### file list

```diff
@@ -1,211 +1,183 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.137557 steam-sdk-2023.5.2/
--rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam-sdk-2023.5.2/.gitignore
--rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam-sdk-2023.5.2/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam-sdk-2023.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-05-11 20:05:11.134565 steam-sdk-2023.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam-sdk-2023.5.2/Readme.md
--rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam-sdk-2023.5.2/mkdocs.yaml
--rw-rw-rw-   0        0        0     1685 2023-05-11 15:44:13.000000 steam-sdk-2023.5.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 20:05:11.137557 steam-sdk-2023.5.2/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-05-11 20:04:23.000000 steam-sdk-2023.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.831355 steam-sdk-2023.5.2/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.846315 steam-sdk-2023.5.2/steam_sdk/analyses/
--rw-rw-rw-   0        0        0   120112 2023-05-11 20:01:59.000000 steam-sdk-2023.5.2/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.847313 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.849307 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.856289 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.858282 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.863270 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.865270 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.871248 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.873243 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.886208 steam-sdk-2023.5.2/steam_sdk/builders/
--rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   162619 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    34260 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12076 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/builders/Readme.md
--rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam-sdk-2023.5.2/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam-sdk-2023.5.2/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.887205 steam-sdk-2023.5.2/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.890197 steam-sdk-2023.5.2/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.893190 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.896182 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
--rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/Readme.md
--rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.897179 steam-sdk-2023.5.2/steam_sdk/configs/users/
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/users/Readme.md
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.900172 steam-sdk-2023.5.2/steam_sdk/cosims/
--rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/cosims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.937072 steam-sdk-2023.5.2/steam_sdk/data/
--rw-rw-rw-   0        0        0    10200 2023-05-11 20:01:58.000000 steam-sdk-2023.5.2/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     8040 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam-sdk-2023.5.2/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2865 2023-04-20 15:50:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4193 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35546 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2636 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam-sdk-2023.5.2/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     6791 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataSIGMA.py
--rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam-sdk-2023.5.2/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/Readme.md
--rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.947045 steam-sdk-2023.5.2/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     2832 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.953030 steam-sdk-2023.5.2/steam_sdk/drivers/temp/
--rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/temp/postLEDET.py
--rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/temp/runLEDET.py
--rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/temp/simLEDET.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.987936 steam-sdk-2023.5.2/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10920 2023-05-11 15:23:35.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0     1928 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserSIGMA.py
--rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.988935 steam-sdk-2023.5.2/steam_sdk/parsers/templates/
--rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam-sdk-2023.5.2/steam_sdk/parsers/templates/template_Dakota.in
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.007883 steam-sdk-2023.5.2/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    61649 2023-05-11 20:01:58.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    70148 2023-05-11 15:13:46.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    47683 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.014864 steam-sdk-2023.5.2/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     2329 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
--rw-rw-rw-   0        0        0     2016 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/parsims/translation_dicts/event_column_names.yaml
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.042789 steam-sdk-2023.5.2/steam_sdk/plotters/
--rw-rw-rw-   0        0        0     8134 2023-05-11 20:01:59.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0    20399 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2023-05-11 15:23:13.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.054758 steam-sdk-2023.5.2/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.119605 steam-sdk-2023.5.2/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam-sdk-2023.5.2/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      590 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/create_coordinate_file_SIGMA.py
--rw-rw-rw-   0        0        0     1279 2023-04-20 15:50:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1592 2023-04-20 15:50:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.122597 steam-sdk-2023.5.2/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam-sdk-2023.5.2/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.125589 steam-sdk-2023.5.2/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.126587 steam-sdk-2023.5.2/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.127584 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.129578 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.842326 steam-sdk-2023.5.2/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-05-11 20:04:42.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7480 2023-05-11 20:05:09.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 20:04:42.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1596 2023-05-11 20:04:42.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 20:04:42.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:20.054190 steam-sdk-2023.5.3/
+-rw-rw-rw-   0        0        0      122 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-05-17 07:33:20.053191 steam-sdk-2023.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-17 07:33:20.054190 steam-sdk-2023.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-05-17 07:28:41.000000 steam-sdk-2023.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.668270 steam-sdk-2023.5.3/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.684682 steam-sdk-2023.5.3/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   125622 2023-05-17 07:23:11.000000 steam-sdk-2023.5.3/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.686682 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.690682 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.707945 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.713089 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.721090 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.726217 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.734377 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.737376 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.759606 steam-sdk-2023.5.3/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    12924 2023-05-12 15:08:26.000000 steam-sdk-2023.5.3/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   162619 2023-05-12 15:08:26.000000 steam-sdk-2023.5.3/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    34698 2023-05-17 07:25:05.000000 steam-sdk-2023.5.3/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12076 2023-05-10 14:13:23.000000 steam-sdk-2023.5.3/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0    11689 2023-01-18 15:24:33.000000 steam-sdk-2023.5.3/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-19 08:13:58.000000 steam-sdk-2023.5.3/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.762853 steam-sdk-2023.5.3/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.764853 steam-sdk-2023.5.3/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.768854 steam-sdk-2023.5.3/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.773994 steam-sdk-2023.5.3/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0    32890 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0     1426 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.775995 steam-sdk-2023.5.3/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.840119 steam-sdk-2023.5.3/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10200 2023-05-12 13:31:31.000000 steam-sdk-2023.5.3/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     8040 2023-05-05 12:54:05.000000 steam-sdk-2023.5.3/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-04-24 12:48:33.000000 steam-sdk-2023.5.3/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4193 2023-05-09 14:50:49.000000 steam-sdk-2023.5.3/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0    12762 2023-05-12 15:08:26.000000 steam-sdk-2023.5.3/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10767 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35579 2023-05-12 15:08:26.000000 steam-sdk-2023.5.3/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2636 2023-05-09 14:50:49.000000 steam-sdk-2023.5.3/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     7899 2023-03-21 08:33:21.000000 steam-sdk-2023.5.3/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     6791 2023-05-09 14:51:04.000000 steam-sdk-2023.5.3/steam_sdk/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0     1650 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-11 12:50:11.000000 steam-sdk-2023.5.3/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    22928 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0    27540 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.891734 steam-sdk-2023.5.3/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-12-19 08:13:58.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-12-19 08:13:58.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2022-12-19 08:13:58.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     3905 2023-05-17 07:23:11.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.975715 steam-sdk-2023.5.3/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-03-29 12:41:10.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1077 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-13 08:06:15.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48056 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10920 2023-05-12 13:31:31.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    61567 2023-04-13 09:38:44.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0    92213 2023-03-27 14:04:47.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0     1928 2023-05-09 14:51:03.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserSIGMA.py
+-rw-rw-rw-   0        0        0    11707 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.986866 steam-sdk-2023.5.3/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    61764 2023-05-12 13:31:31.000000 steam-sdk-2023.5.3/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    72533 2023-05-17 07:23:09.000000 steam-sdk-2023.5.3/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    47819 2023-05-12 13:31:31.000000 steam-sdk-2023.5.3/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-25 14:04:47.000000 steam-sdk-2023.5.3/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.999083 steam-sdk-2023.5.3/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0     8053 2023-05-12 13:31:31.000000 steam-sdk-2023.5.3/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0    20399 2023-05-09 14:51:04.000000 steam-sdk-2023.5.3/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39596 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-19 08:13:58.000000 steam-sdk-2023.5.3/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8871 2023-04-24 12:43:05.000000 steam-sdk-2023.5.3/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:20.002215 steam-sdk-2023.5.3/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:20.037611 steam-sdk-2023.5.3/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4762 2023-05-17 07:23:11.000000 steam-sdk-2023.5.3/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-03-15 09:29:53.000000 steam-sdk-2023.5.3/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      590 2023-05-09 14:50:57.000000 steam-sdk-2023.5.3/steam_sdk/utils/create_coordinate_file_SIGMA.py
+-rw-rw-rw-   0        0        0     1279 2023-04-24 12:48:33.000000 steam-sdk-2023.5.3/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-24 12:48:33.000000 steam-sdk-2023.5.3/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-11 12:50:11.000000 steam-sdk-2023.5.3/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2023-05-11 09:21:50.000000 steam-sdk-2023.5.3/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:20.046038 steam-sdk-2023.5.3/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-23 12:53:02.000000 steam-sdk-2023.5.3/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:20.048039 steam-sdk-2023.5.3/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:42.000000 steam-sdk-2023.5.3/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:20.050038 steam-sdk-2023.5.3/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:20.051039 steam-sdk-2023.5.3/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.5.3/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:20.052189 steam-sdk-2023.5.3/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.5.3/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-11-02 10:29:43.000000 steam-sdk-2023.5.3/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-11-02 10:29:43.000000 steam-sdk-2023.5.3/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:33:19.677565 steam-sdk-2023.5.3/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-05-17 07:33:17.000000 steam-sdk-2023.5.3/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6686 2023-05-17 07:33:17.000000 steam-sdk-2023.5.3/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:33:17.000000 steam-sdk-2023.5.3/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1597 2023-05-17 07:33:17.000000 steam-sdk-2023.5.3/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-17 07:33:17.000000 steam-sdk-2023.5.3/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2023.5.2/PKG-INFO` & `steam-sdk-2023.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.5.2
+Version: 2023.5.3
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SDK,STEAM,API,CERN
+Keywords: API,SDK,STEAM,CERN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.5.2/requirements.txt` & `steam-sdk-2023.5.3/steam_sdk.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-asttokens==2.0.8
-attrs==22.1.0
-Babel==2.10.3
-backcall==0.2.0
-certifi==2022.9.14
-charset-normalizer==2.1.1
-click==8.1.3
-colorama==0.4.5
-contourpy==1.0.5
-coverage==6.4.4
-coverage-badge==1.1.0
-cycler==0.11.0
-decorator==5.1.1
-deepdiff==5.8.1
-et-xmlfile==1.1.0
-executing==1.0.0
-fonttools==4.37.3
-ghp-import==2.1.0
-gitdb==4.0.9
-GitPython==3.1.27
-gmsh==4.10.5
-griffe==0.22.1
-h5py==3.7.0
-idna==3.4
-importlib-metadata==4.12.0
-iniconfig==1.1.1
-ipython==8.5.0
-jedi==0.18.1
-Jinja2==3.1.2
-kiwisolver==1.4.4
-Markdown==3.3.7
-markdown-include==0.7.0
-MarkupSafe==2.1.1
-matplotlib==3.6.0
-matplotlib-inline==0.1.6
-mergedeep==1.3.4
-mkdocs==1.3.1
-mkdocs-autorefs==0.4.1
-mkdocs-git-revision-date-localized-plugin==1.1.0
-mkdocs-include-markdown-plugin==3.8.1
-mkdocs-material==8.5.3
-mkdocs-material-extensions==1.0.3
-mkdocstrings==0.19.0
-mkdocstrings-python==0.7.1
-npTDMS==1.6.0
-numpy==1.23.3
-openpyxl==3.0.10
-ordered-set==4.1.0
-packaging==21.3
-pandas==1.5.0
-parso==0.8.3
-pickleshare==0.7.5
-Pillow==9.2.0
-pluggy==1.0.0
-prompt-toolkit==3.0.31
-pure-eval==0.2.2
-py==1.11.0
-py4j==0.10.9.7
-pydantic==1.10.2
-Pygments==2.13.0
-pymdown-extensions==9.5
-pyparsing==3.0.9
-pysoleno==0.0.8
-pytest==7.1.3
-pytest-cov==3.0.0
-python-dateutil==2.8.2
-pytz==2022.2.1
-PyYAML==6.0
-pyyaml_env_tag==0.1
-reportlab==3.6.12
-requests==2.28.1
-ruamel.yaml==0.17.21
-ruamel.yaml.clib==0.2.6
-scipy==1.9.1
-seaborn==0.12.0
-six==1.16.0
-smmap==5.0.0
-stack-data==0.5.0
-STEAM-materials==0.0.33
-svglib == 1.5.1
-tomli==2.0.1
-tqdm==4.64.1
-traitlets==5.4.0
-typing_extensions==4.3.0
-urllib3==1.26.12
-watchdog==2.1.9
-wcwidth==0.2.5
-zipp==3.8.1
-steam-pysigma==2023.5.7
+asttokens==2.0.8
+attrs==22.1.0
+Babel==2.10.3
+backcall==0.2.0
+certifi==2022.9.14
+charset-normalizer==2.1.1
+click==8.1.3
+colorama==0.4.5
+contourpy==1.0.5
+coverage==6.4.4
+coverage-badge==1.1.0
+cycler==0.11.0
+decorator==5.1.1
+deepdiff==5.8.1
+et-xmlfile==1.1.0
+executing==1.0.0
+fonttools==4.37.3
+ghp-import==2.1.0
+gitdb==4.0.9
+GitPython==3.1.27
+gmsh==4.10.5
+griffe==0.22.1
+h5py==3.7.0
+idna==3.4
+importlib-metadata==4.12.0
+iniconfig==1.1.1
+ipython==8.5.0
+jedi==0.18.1
+Jinja2==3.1.2
+kiwisolver==1.4.4
+Markdown==3.3.7
+markdown-include==0.7.0
+MarkupSafe==2.1.1
+matplotlib==3.6.0
+matplotlib-inline==0.1.6
+mergedeep==1.3.4
+mkdocs==1.3.1
+mkdocs-autorefs==0.4.1
+mkdocs-git-revision-date-localized-plugin==1.1.0
+mkdocs-include-markdown-plugin==3.8.1
+mkdocs-material==8.5.3
+mkdocs-material-extensions==1.0.3
+mkdocstrings==0.19.0
+mkdocstrings-python==0.7.1
+npTDMS==1.6.0
+numpy==1.23.3
+openpyxl==3.0.10
+ordered-set==4.1.0
+packaging==21.3
+pandas==1.5.0
+parso==0.8.3
+pickleshare==0.7.5
+Pillow==9.2.0
+pluggy==1.0.0
+prompt-toolkit==3.0.31
+pure-eval==0.2.2
+py==1.11.0
+py4j==0.10.9.7
+pydantic==1.10.2
+Pygments==2.13.0
+pymdown-extensions==9.5
+pyparsing==3.0.9
+pysoleno==0.0.8
+pytest==7.1.3
+pytest-cov==3.0.0
+python-dateutil==2.8.2
+pytz==2022.2.1
+PyYAML==6.0
+pyyaml_env_tag==0.1
+reportlab==3.6.12
+requests==2.28.1
+ruamel.yaml==0.17.21
+ruamel.yaml.clib==0.2.6
+scipy==1.9.1
+seaborn==0.12.0
+six==1.16.0
+smmap==5.0.0
+stack-data==0.5.0
+STEAM-materials==0.0.33
+svglib==1.5.1
+tomli==2.0.1
+tqdm==4.64.1
+traitlets==5.4.0
+typing_extensions==4.3.0
+urllib3==1.26.12
+watchdog==2.1.9
+wcwidth==0.2.5
+zipp==3.8.1
+steam-pysigma==2023.5.11
```

### Comparing `steam-sdk-2023.5.2/setup.py` & `steam-sdk-2023.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-sdk',
-    version="2023.5.2",
+    version="2023.5.3",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from steam_sdk.data.DataSettings import DataSettings
 from steam_sdk.builders.BuilderModel import BuilderModel
 from steam_sdk.data.DataAnalysis import DataAnalysis, ModifyModel, ModifyModelMultipleVariables, ParametricSweep, LoadCircuitParameters, WriteStimulusFile
 from steam_sdk.drivers.DriverFiQuS import DriverFiQuS
 from steam_sdk.drivers.DriverLEDET import DriverLEDET
 from steam_sdk.drivers.DriverPSPICE import DriverPSPICE
 from steam_sdk.drivers.DriverPyBBQ import DriverPyBBQ
-from steam_sdk.drivers.DriverSIGMA import DriverSIGMA_new
+from steam_sdk.drivers.DriverSIGMA import DriverSIGMA
 from steam_sdk.drivers.DriverXYCE import DriverXYCE
 from steam_sdk.parsers.ParserYAML import dict_to_yaml, yaml_to_data
 from steam_sdk.parsims.ParsimConductor import ParsimConductor
 from steam_sdk.parsims.ParsimEventCircuit import ParsimEventCircuit
 from steam_sdk.parsims.ParsimEventMagnet import ParsimEventMagnet
 from steam_sdk.utils import parse_str_to_list
 from steam_sdk.postprocs.PostprocsMetrics import PostprocsMetrics
@@ -424,17 +424,16 @@
                 if 'LEDET' in step.software:
                     flag_json = BM.flag_json
                     flag_yaml = True  # Hard-coded for the moment
                     BM.buildLEDET()
                     self.setup_sim_LEDET(simulation_name=step.simulation_name, sim_number=simulation_number,
                                          flag_yaml=flag_yaml, flag_json=flag_json)
                 if 'SIGMA' in step.software:
-                    for sim_num in step.simulation_numbers:
-                        make_folder_if_not_existing(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}") )#ADDED
-                        BM.buildSIGMA(f"{step.simulation_name}_{sim_num}")
+                    make_folder_if_not_existing(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{simulation_number}") )#ADDED
+                    BM.buildSIGMA(f"{step.simulation_name}_{simulation_number}")
                     self.setup_sim_SIGMA(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PyBBQ' in step.software:
                     BM.buildPyBBQ()
                     self.setup_sim_PyBBQ(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PSPICE' in step.software:
                     BM.buildPSPICE()
                     self.setup_sim_PSPICE(simulation_name=step.simulation_name, sim_number=simulation_number)
@@ -557,29 +556,35 @@
             self.run_sim(software, sim_name, sim_number, simFileType, verbose)
 
     def step_postprocess(self, step, verbose: bool = False):
         if verbose: print('postprocessing')
         if step.software and 'SIGMA' in step.software:
             for sim_num in step.simulation_numbers:
                 # Check if files exist
-                path_result_txt_Bx = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", 'mf.Bx.txt')
-                path_result_txt_By = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", 'mf.By.txt')
-                path_new_file = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", 'B_field_map2d.map2d')
-                path_reference_roxie = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", f"{step.simulation_name}_ROXIE_REFERENCE.map2d")
-
+                path_result_txt_Bx = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}","output", "mf.Bx.txt")
+                path_result_txt_By = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}","output", "mf.By.txt")
+                path_new_file = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}","output", "B_field_map2d.map2d")
+                path_reference_roxie = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", "sources", f"{step.simulation_name}_{sim_num}_ROXIE_REFERENCE.map2d")
                 if not os.path.exists(path_result_txt_Bx):
                     raise Warning("No Bx file is found, please check that simulation ran successfully.")
                 elif not os.path.exists(path_result_txt_By):
                     raise Warning("No By file is found, please check that simulation ran successfully.")
                 elif not os.path.exists(path_reference_roxie):
+                    print(path_reference_roxie)
                     raise Warning("No Roxie reference file is found, please check model_data.yaml in options_sigma that key map2d is specified.")
                 else:
-                    export_B_field_txt_to_map2d_SIGMA(path_reference_roxie, path_result_txt_Bx, path_result_txt_By,
-                                                path_new_file)
-                    generate_report_from_map2d(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}"), path_reference_roxie, "Roxie Data", path_new_file, "SIGMA DATA", "coil", save=True)
+                    try:
+                        export_B_field_txt_to_map2d_SIGMA(path_reference_roxie, path_result_txt_Bx, path_result_txt_By,
+                                                    path_new_file)
+                    except:
+                        print("Can't generate map2d output. This can only be done for stationary studies and with the same coordinate in output files and roxie reference")
+                    try:
+                        generate_report_from_map2d(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", "output"), path_reference_roxie, "Roxie Data", path_new_file, "SIGMA DATA", "coil", save=True)
+                    except:
+                        print("Can't generate report from map2d. This can only be done for stationary studies")
         else:
             print('Not implemented yet.')
 
     def step_setup_folder(self, step, verbose: bool = False):
         """
         Set up simulation working folder.
         The function applies a different logic for each simulation software.
@@ -710,28 +715,28 @@
 
         # If no new name is provided, use the old file name
         if new_file_name == None:
             new_file_name = ntpath.basename(full_path_aux_file)
 
         # Copy auxiliary file to the output folder
         full_path_output_file = os.path.join(output_path, new_file_name)
+        make_folder_if_not_existing(os.path.dirname(full_path_output_file))  # in case the output folder does not exist, make it
         shutil.copyfile(full_path_aux_file, full_path_output_file)
         if verbose: print(f'File {full_path_aux_file} was copied to {full_path_output_file}.')
 
         # Build simulation file
         len_simulation_numbers = len(step.simulation_numbers)
         if len_simulation_numbers > 0:
             for simulation_number in step.simulation_numbers:
                 if 'FiQuS' in step.software:
                     self.setup_sim_FiQuS(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'LEDET' in step.software:
                     flag_yaml = True  # Hard-coded for the moment
                     flag_json = False  # Hard-coded for the moment
-                    self.setup_sim_LEDET(simulation_name=step.simulation_name, sim_number=simulation_number,
-                                         flag_yaml=flag_yaml, flag_json=flag_json)
+                    self.setup_sim_LEDET(simulation_name=step.simulation_name, sim_number=simulation_number, flag_yaml=flag_yaml, flag_json=flag_json)
                 if 'PyBBQ' in step.software:
                     self.setup_sim_PyBBQ(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PSPICE' in step.software:
                     self.setup_sim_PSPICE(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PSPICE' in step.software:
                     self.setup_sim_XYCE(simulation_name=step.simulation_name, sim_number=simulation_number)
 
@@ -1039,28 +1044,50 @@
 
         # Add simulation number to the list
         self.list_sims.append(sim_number)
 
         # Make simulation folder
         local_model_folder = os.path.join(self.settings.local_SIGMA_folder, f'{simulation_name}_{str(sim_number)}')
         make_folder_if_not_existing(local_model_folder)
-
+        sources_folder = os.path.join(local_model_folder, 'sources')
+        make_folder_if_not_existing(sources_folder)
+        input_folder = os.path.join(local_model_folder, 'input')
+        make_folder_if_not_existing(input_folder)
+        output_folder = os.path.join(local_model_folder, 'output')
+        make_folder_if_not_existing(output_folder)
         # Copy all simulation file
         files = os.listdir(self.output_path)
+        # Copy all files ending with csv, map2d or bhdata to sources
 
-        # iterating over all the files in
-        # the source directory
-        for fname in files:
-            file_name_temp = os.path.join(self.output_path, fname)
-            file_name_local = os.path.join(local_model_folder, fname)
-            shutil.copyfile(file_name_temp, file_name_local)
+        string_simulation = f"{simulation_name}_{sim_number}"
 
+        suffixes_sources = ['.map2d', '.csv']  # List of suffixes to filter files
+        suffixes_input = ['.geom', '.set', '.yaml']  # List of suffixes to filter files
 
-        if self.verbose: print('Simulation files {} generated.'.format(file_name_temp))
-        if self.verbose: print('Simulation files {} copied.'.format(file_name_local))
+
+        # Iterate over files in the source directory
+        for fname in files:
+            if any(fname.endswith(suffix) for suffix in
+                   suffixes_sources) and string_simulation in fname:  # Check if the file has any of the desired suffixes
+                source_path = os.path.join(self.output_path, fname)
+                destination_path = os.path.join(sources_folder, fname)
+                shutil.copy2(source_path, destination_path)  # Copy
+
+            if any(fname.endswith(suffix) for suffix in
+                   suffixes_input) and string_simulation in fname:  # Check if the file has any of the desired suffixes
+                source_path = os.path.join(self.output_path, fname)
+                destination_path = os.path.join(input_folder, fname)
+                shutil.copy2(source_path, destination_path)  # Copy
+            if fname.endswith('roxie.bhdata'):
+                source_path = os.path.join(self.output_path, fname)
+                destination_path = os.path.join(sources_folder, fname)
+                shutil.copy2(source_path, destination_path)  # Copy
+
+        # if self.verbose: print('Simulation files {} generated.'.format(file_name_temp))
+        # if self.verbose: print('Simulation files {} copied.'.format(file_name_local))
 
     def setup_sim_PSPICE(self, simulation_name, sim_number):
         """
         Set up a PSPICE simulation by copying the last file generated by BuilderModel to the output folder and to the
         local PSPICE working folder.
         The simulation netlist and auxiliary files are copied in a new numbered subfoldered.
         The original file is then deleted.
@@ -1284,16 +1311,16 @@
         elif software == 'XYCE':
             local_model_folder = Path(
                 Path(self.settings.local_XYCE_folder) / simulation_name / str(sim_number)).resolve()
             dXYCE = DriverXYCE(path_exe=self.settings.XYCE_path, path_folder_XYCE=local_model_folder, verbose=verbose)
             dXYCE.run_XYCE(simulation_name, suffix='')
         elif software == 'SIGMA':
             local_analysis_folder = simulation_name + '_' + str(sim_number)
-            ds = DriverSIGMA_new(path_folder_SIGMA=self.settings.local_SIGMA_folder,
-                                 path_folder_SIGMA_input=os.path.join(self.settings.local_SIGMA_folder,
+            ds = DriverSIGMA(path_folder_SIGMA=self.settings.local_SIGMA_folder,
+                             path_folder_SIGMA_input=os.path.join(self.settings.local_SIGMA_folder,
                                                                       local_analysis_folder), local_analysis_folder=local_analysis_folder, system_settings=self.settings, verbose=verbose)
             ds.run_SIGMA(simulation_name)
         else:
             raise Exception(f'Software {software} not supported for automated running.')
 
 
     def write_stimuli_from_interpolation(self, step, verbose: bool = False):
@@ -1435,32 +1462,43 @@
                     # modify model diode step used to change diodes across the quenching magnets with heating
                     modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name, variable_to_change=f'Netlist.x_D{quenching_magnet[0]}.value', variable_value=["RQ_Protection_Diode"], simulation_numbers=[], simulation_name=simulation_name, software=software)
                 elif circuit_type == "RCBX":
                     circuit_name_1 = circuit_name.replace("X", "XH")
                     circuit_name_2 = circuit_name.replace("X", "XV")
                     load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
                     load_circuit_parameters_step_2 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_2)
+                elif circuit_type in ["RCD", "RCO"]:
+                    parts = circuit_name.split("-")
+                    last_part = parts[-1]
+                    string1 = parts[0] + "." + last_part.split(".")[1]
+                    string2 = last_part
+                    if circuit_type == "RCD":
+                        load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=string1)
+                    else:
+                        load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=string2)
                 else:
                     load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
 
                 # choosing stimulus output file location
                 if circuit_family_name == "IPD":
-                    stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_family_name}', f'{event_number + 1}', 'coil_resistances.stl')
+                    stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_family_name}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
                 elif circuit_family_name == "RQ":
                     stimulus_output_file_1 = os.path.join(default_keys.path_output, f'{circuit_type}_47magnets', f'{event_number + 1}', 'coil_resistances.stl')
                     stimulus_output_file_2 = os.path.join(default_keys.path_output, f'{circuit_type}_47magnets',f'{event_number + 2}', 'coil_resistances.stl')
                 elif circuit_type == "RCBX":
                     stimulus_output_file_1 = os.path.join(default_keys.path_output, 'RCBX', f'{event_number + 1}', 'coil_resistances.stl')
                     stimulus_output_file_2 = os.path.join(default_keys.path_output, 'RCBX', f'{event_number + 2}', 'coil_resistances.stl')
                 elif simulation_name.startswith("IPQ"):
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{simulation_name}', f'{event_number + 1}', 'coil_resistances.stl')
                 elif circuit_name.startswith("RCBY"):
                     stimulus_output_file = os.path.join(default_keys.path_output, 'RCBY', f'{event_number + 1}', 'coil_resistances.stl')
+                elif circuit_name.startswith(("RCBH", "RCBV")):
+                    stimulus_output_file = os.path.join(default_keys.path_output, 'RCB', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
                 else:
-                    stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', f'{event_number + 1}', 'coil_resistances.stl')
+                    stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', f"{self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_numbers[0]}", 'coil_resistances.stl')
 
                 # making appropriate directory if it doesn't exist for the stimulus output file
                 if circuit_family_name == "RQ" or circuit_type == "RCBX":
                     for file_path in [stimulus_output_file_1, stimulus_output_file_2]:
                         directory = os.path.dirname(file_path)
                         if not os.path.exists(directory):
                             os.makedirs(directory)
@@ -1489,16 +1527,20 @@
                     position = pec.list_events[event_number].QuenchEvents[circuit_name].magnet_electrical_position
                     quenching_magnet = [self.__get_quenching_magnet_number(position, circuit_family_name)]
                     quenching_magnet_list.append(quenching_magnet[0])
                     quenching_magnet_list.sort()
                     # modify model diode step used to change diodes across the quenching magnets with heating
                     modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name, variable_to_change=f'Netlist.x_D{quenching_magnet[0]}.value', variable_value=["RB_Protection_Diode"], simulation_numbers=[], simulation_name=simulation_name, software=software)
                     write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level]*(event_number + 1), magnets=quenching_magnet_list, t_offset=[t_PC_off]*(event_number + 1), interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_type == "RCD":
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[1]]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_type == "RCO":
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 else:
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[abs(current_level)], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
 
                 # parsim sweep step with newly created event file
                 if circuit_family_name == "RQ" or circuit_type == "RCBX":
                     output_files = self.__split_csv(path_output_event_csv)
                     parsim_sweep_step_1 = ParametricSweep(type='ParametricSweep', input_sweep_file=output_files[0],
                                                         model_name=model_name, case_model=case_model, software=software, verbose=verbose)
                     parsim_sweep_step_2 = ParametricSweep(type='ParametricSweep', input_sweep_file=output_files[1],
@@ -1771,15 +1813,15 @@
             return "60A"
         elif circuit_name.startswith("RD"):
             return "IPD"
         elif circuit_name.startswith("RQX"):
             return "RQX"
         elif circuit_name.startswith(("RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
             return "IPQ"
-        elif circuit_name.startswith(("RQT12", "RQT13", "RQS", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RCBX", "RQSX3", "RCS", "ROD", "ROF", "RQ6", "RSD", "RSF", "RQTL9", "RQTD", "RQTF")):
+        elif circuit_name.startswith(("RQT12", "RQT13", "RQS", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RCBX", "RQSX3", "RCS", "ROD", "ROF", "RQ6", "RSD", "RSF", "RQTL9", "RQTD", "RQTF", "RCD", "RCO")):
             return "600A"
         elif circuit_name.startswith("RQ"):
             return "RQ"
         elif circuit_name.startswith(("RCBY", "RCBC", "RCTX")):
             return "80-120A"
         elif circuit_name.startswith("RB"):
             return "RB"
@@ -1807,21 +1849,27 @@
             return "MQT"
         elif circuit_name.startswith("RCS"):
             return ["MCS", "MCS_quenchback"]
         elif circuit_name.startswith("RB"):
             return "MB"
         elif circuit_name.startswith("RCBX"):
             return ["MCBXH", "MCBXV"]
+        elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RCD":
+            return ["MCD", "MCD_quenchback"]
+        elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RCO":
+            return ["MCO", "MCO_quenchback"]
 
     def __get_number_of_magnets(self, circuit_name: str):
         circuit_family_name = self.__get_circuit_family_name(circuit_name)
         circuit_type = self.__get_circuit_type(circuit_name)
         if circuit_type in ["RCS", "RB"]:
             return 154
-        elif circuit_family_name in ["60A", "IPD", "80-120A", "600A"]: #RCO (77) out of ambit
+        elif circuit_type in ["RCD", "RCO"]:
+            return 77
+        elif circuit_family_name in ["60A", "IPD", "80-120A", "600A"]:
             return 1
         elif circuit_family_name == "RQ":
             return 47  # deal with 51 later
         elif circuit_family_name == "RQX":
             return 4
         elif circuit_family_name == "IPQ":
             return int(int(re.search(r'_(\d+)_', self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name).group(1))/2)
@@ -1870,14 +1918,18 @@
             return "RQ"
         elif circuit_name.startswith("RCS"):
             return "RCS"
         elif circuit_name.startswith("RB"):
             return "RB"
         elif circuit_name.startswith("RCBX"):
             return "RCBX"
+        elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RCD":
+            return "RCD"
+        elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name == "RCO":
+            return "RCO"
 
     def __get_quenching_magnet_number(self, position: str, circuit_family_name: str):
         df = pd.read_csv(os.path.join(f"../../tests/analyses/input/run_parsim_event_circuit/{circuit_family_name}_LayoutDetails.csv"))
         mask = df['Magnet'].str.split('.').str[1] == position
         result = df.loc[mask, '#Electric_circuit'].iloc[0]
         return result
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2023.5.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2023.5.3/steam_sdk/builders/BuilderFiQuS.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.data.DataRoxieParser import RoxieData
-from steam_sdk.data.DataFiQuS import DataFiQuS, MultipoleRoxieGeometry, MultipoleSettings, MultipoleConductor
+from steam_sdk.data.DataFiQuS import DataFiQuS, MultipoleRoxieGeometry, MultipoleSettings, MultipoleConductor, \
+    MultipoleConductorSet
 
 
 class BuilderFiQuS:
     """
         Class to generate FiQuS models
     """
 
@@ -41,40 +42,80 @@
                 self.data_FiQuS_geo = MultipoleRoxieGeometry()
                 self.data_FiQuS_set = MultipoleSettings()
                 self.buildDataMultipole(model_data, roxie_data)
             elif model_data.GeneralParameters.magnet_type == 'CCT_straight':
                 self.buildDataCCT(model_data)
             else:
                 raise Exception(f'Magnet type: {model_data.GeneralParameters.magnet_type} is incompatible with FiQuS.')
+                # ------------- circuit ---------
+            for key, value in model_data.Circuit.dict().items():  # for keys that are present in the model data and in data FiQuS - they are the same
+                self.data_FiQuS.circuit.__setattr__(key, value)
+
+                # ------------- power_supply ---------
+            for key, value in model_data.Power_Supply.dict().items():  # for keys that are present in the model data and in data FiQuS - they are the same
+                self.data_FiQuS.power_supply.__setattr__(key, value)
+
+                # ------------- quench_protection ---------
+            for key, value in model_data.Quench_Protection.Energy_Extraction.dict().items():  # for keys that are present in the model data and in data FiQuS - they are the same
+                self.data_FiQuS.quench_protection.energy_extraction.__setattr__(key, value)
+
+            for key, value in model_data.Quench_Protection.Quench_Heaters.dict().items():  # for keys that are present in the model data and in data FiQuS - they are the same
+                if key in self.data_FiQuS.quench_protection.quench_heaters.dict().keys():
+                    self.data_FiQuS.quench_protection.quench_heaters.__setattr__(key, value)
+            # set the params that are renamed in FiQuS
+            self.data_FiQuS.quench_protection.quench_heaters.ids = model_data.Quench_Protection.Quench_Heaters.iQH_toHalfTurn_From
+            self.data_FiQuS.quench_protection.quench_heaters.turns = model_data.Quench_Protection.Quench_Heaters.iQH_toHalfTurn_To
+
+            for key, value in model_data.Quench_Protection.CLIQ.dict().items():  # for keys that are present in the model data and in data FiQuS - they are the same
+                self.data_FiQuS.quench_protection.cliq.__setattr__(key, value)
+
+            for key, value in model_data.Quench_Protection.FQPCs.dict().items():  # for keys that are present in the model data and in data FiQuS - they are the same
+                self.data_FiQuS.quench_protection.FQPCs.__setattr__(key, value)
+            # ------------- Conductors ---------
+            for cond in model_data.Conductors:
+                self.data_FiQuS.conductors[cond.name] = MultipoleConductor(
+                    cable={'type': cond.cable.type})
+                conductor = self.data_FiQuS.conductors[cond.name]
+                for key, value in cond.cable.dict().items():
+                    conductor.cable.__setattr__(key, value)
+
+                print(conductor.strand['type'])
+                for key, value in cond.strand.dict().items():
+                    conductor.strand[key] = value
 
-    def buildDataCCT(self, model_data): #TODO: good idea to make them private?
+                for key, value in cond.Jc_fit.dict().items():
+                    conductor.Jc_fit[key] = value
+
+
+
+    def buildDataCCT(self, model_data):  # TODO: good idea to make them private?
         """
             Load selected conductor data from DataModelMagnet keys, check inputs, calculate and set missing variables
         """
         # --------- geometry ----------
         # windings
         for key, value in model_data.Options_FiQuS.cct.geometry.windings.dict().items():       # for keys that are present in the FiQUS Options model data (but not all keys in data FiQuS)
             self.data_FiQuS.magnet.geometry.windings.__setattr__(key, value)
         self.data_FiQuS.magnet.geometry.windings.n_turnss = model_data.CoilWindings.CCT_straight.winding_numberTurnsFormers  # additional, picked form other places in model data
 
         self.data_FiQuS.magnet.postproc.windings_wwns = model_data.CoilWindings.CCT_straight.winding_numRowStrands
         self.data_FiQuS.magnet.postproc.windings_whns = model_data.CoilWindings.CCT_straight.winding_numColumnStrands
         self.data_FiQuS.magnet.postproc.winding_order = model_data.CoilWindings.CCT_straight.winding_order
 
         # fqpls
-        self.data_FiQuS.magnet.geometry.fqpls.fndpls = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.fndpls, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.fwhs = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.fwhs, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.fwws = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.fwws, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.n_sbs = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.n_sbs, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.names = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.names, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.r_bs = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.r_bs, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.r_ins = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.r_ins, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.thetas = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.thetas, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.z_ends = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.z_ends, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.geometry.fqpls.z_starts = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.z_starts, model_data.Quench_Protection.FQPLs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.fndpls = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.fndpls, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.fwhs = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.fwhs, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.fwws = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.fwws, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.n_sbs = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.n_sbs, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.names = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.names, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.r_bs = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.r_bs, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.r_ins = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.r_ins, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.thetas = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.thetas, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.z_ends = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.z_ends, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.geometry.fqpls.z_starts = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.z_starts, model_data.Quench_Protection.FQPCs.enabled) if flag]
 
         # formers
         for key, value in model_data.Options_FiQuS.cct.geometry.formers.dict().items():       # for keys that are present in the model data (but not all keys in data FiQuS)
             self.data_FiQuS.magnet.geometry.formers.__setattr__(key, value)
         self.data_FiQuS.magnet.geometry.formers.r_ins = model_data.CoilWindings.CCT_straight.former_inner_radiuses  # additional, picked form other places in model data
         self.data_FiQuS.magnet.geometry.formers.r_outs = model_data.CoilWindings.CCT_straight.former_outer_radiuses  # additional, picked form other places in model data
 
@@ -82,17 +123,17 @@
         self.data_FiQuS.magnet.geometry.air = model_data.Options_FiQuS.cct.geometry.air   # for keys that are present in the model data and in data FiQuS - they are the same
 
         # ------------- mesh --------------
         self.data_FiQuS.magnet.mesh = model_data.Options_FiQuS.cct.mesh                # for keys that are present in the model data and in data FiQuS - they are the same
 
         # ------------- solve -------------
         self.data_FiQuS.magnet.solve.windings = model_data.Options_FiQuS.cct.solve.windings              # for keys that are present in the model data and in data FiQuS - they are the same
-        self.data_FiQuS.magnet.solve.fqpls.mu_rs = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.mu_rs, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.solve.fqpls.currents = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.currents, model_data.Quench_Protection.FQPLs.enabled) if flag]
-        self.data_FiQuS.magnet.solve.fqpls.sigmas = [val for val, flag in zip(model_data.Quench_Protection.FQPLs.sigmas, model_data.Quench_Protection.FQPLs.enabled) if flag]
+        self.data_FiQuS.magnet.solve.fqpls.mu_rs = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.mu_rs, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.solve.fqpls.currents = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.currents, model_data.Quench_Protection.FQPCs.enabled) if flag]
+        self.data_FiQuS.magnet.solve.fqpls.sigmas = [val for val, flag in zip(model_data.Quench_Protection.FQPCs.sigmas, model_data.Quench_Protection.FQPCs.enabled) if flag]
         self.data_FiQuS.magnet.solve.formers = model_data.Options_FiQuS.cct.solve.formers
         self.data_FiQuS.magnet.solve.air = model_data.Options_FiQuS.cct.solve.air
         self.data_FiQuS.magnet.solve.file_exts = model_data.Options_FiQuS.cct.solve.file_exts
         self.data_FiQuS.magnet.solve.pro_template = model_data.Options_FiQuS.cct.solve.pro_template
         self.data_FiQuS.magnet.solve.variables = model_data.Options_FiQuS.cct.solve.variables
         self.data_FiQuS.magnet.solve.volumes = model_data.Options_FiQuS.cct.solve.volumes
 
@@ -108,15 +149,16 @@
         # geom file
         self.data_FiQuS_geo.Roxie_Data = RoxieData(**roxie_data.dict())
 
         # set file
         self.data_FiQuS_set.Model_Data_GS.general_parameters.I_ref = \
             [model_data.Options_LEDET.field_map_files.Iref] * len(self.data_FiQuS_geo.Roxie_Data.coil.coils)
         for cond in model_data.Conductors:
-            self.data_FiQuS_set.Model_Data_GS.conductors[cond.name] = MultipoleConductor(cable={'type': cond.cable.type})
+            self.data_FiQuS_set.Model_Data_GS.conductors[cond.name] = MultipoleConductorSet(
+                cable={'type': cond.cable.type})
             conductor = self.data_FiQuS_set.Model_Data_GS.conductors[cond.name]
             conductor.cable.bare_cable_width = cond.cable.bare_cable_width
             conductor.cable.bare_cable_height_mean = cond.cable.bare_cable_height_mean
 
         # --------- run ----------
         self.data_FiQuS.run = model_data.Options_FiQuS.run
 
@@ -137,7 +179,8 @@
         self.data_FiQuS.magnet.solve.electromagnetics.solved = model_data.Options_FiQuS.multipole.solve.electromagnetics.solved
         self.data_FiQuS.magnet.solve.electromagnetics.transient = model_data.Options_FiQuS.multipole.solve.electromagnetics.transient
         self.data_FiQuS.magnet.solve.electromagnetics.boundary_conditions.currents = \
             [model_data.Power_Supply.I_initial] * len(self.data_FiQuS_geo.Roxie_Data.coil.coils)
 
         # ------------- postproc ---------
         self.data_FiQuS.magnet.postproc = model_data.Options_FiQuS.multipole.postproc
+
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2023.5.3/steam_sdk/builders/BuilderLEDET.py`

 * *Files 0% similar despite different names*

```diff
@@ -692,15 +692,15 @@
             pass        # electricall order calculated in assignSolenoidValuesWindings method of this class
         elif typeWindings in ['CCT_straight']:
 
             wwns = self.model_data.CoilWindings.CCT_straight.winding_numRowStrands  # number of wires in width direction
             whns = self.model_data.CoilWindings.CCT_straight.winding_numColumnStrands  # number of wires in height direction
             n_turns_formers = self.model_data.CoilWindings.CCT_straight.winding_numberTurnsFormers  # number of turns [-]
             winding_order = self.model_data.CoilWindings.CCT_straight.winding_order
-            fqpl_names = [val for val, flag in zip(self.model_data.Quench_Protection.FQPLs.names, self.model_data.Quench_Protection.FQPLs.enabled) if flag]
+            fqpl_names = [val for val, flag in zip(self.model_data.Quench_Protection.FQPCs.names, self.model_data.Quench_Protection.FQPCs.enabled) if flag]
 
             # ----- formers' turns -----
             all_turns_magnet = []  # list for all turns of the former
             for former_i in range(len(n_turns_formers)):  # for each former of cct
                 all_turns_former = []  # list of lists of lists for actual turns positions
                 former_start_offset = former_i * wwns[former_i] * whns[former_i] * n_turns_formers[former_i]  # offset for the first turn on the next former
                 for channel_turn in range(n_turns_formers[former_i]):  # for number of turns in each former
@@ -822,16 +822,16 @@
 
         elif typeWindings in ['CCT_straight']:
             # --- get inputs used for windings and fqpls ---
             wwns = self.model_data.CoilWindings.CCT_straight.winding_numRowStrands  # number of wires in width direction
             whns = self.model_data.CoilWindings.CCT_straight.winding_numColumnStrands  # number of wires in height direction
             n_turns_formers = self.model_data.CoilWindings.CCT_straight.winding_numberTurnsFormers  # number of turns [-]
             # get variables used here from model data
-            fqpl_names = [val for val, flag in zip(self.model_data.Quench_Protection.FQPLs.names, self.model_data.Quench_Protection.FQPLs.enabled) if flag]  # trim only to enabled fqpls
-            fqpl_th_conns_def_bool = [val for val, flag in zip(self.model_data.Quench_Protection.FQPLs.th_conns_def, self.model_data.Quench_Protection.FQPLs.enabled) if flag]  # trim only to enabled fqpls
+            fqpl_names = [val for val, flag in zip(self.model_data.Quench_Protection.FQPCs.names, self.model_data.Quench_Protection.FQPCs.enabled) if flag]  # trim only to enabled fqpls
+            fqpl_th_conns_def_bool = [val for val, flag in zip(self.model_data.Quench_Protection.FQPCs.th_conns_def, self.model_data.Quench_Protection.FQPCs.enabled) if flag]  # trim only to enabled fqpls
             #fqpl_th_conns_def_bool = self.model_data.Quench_Protection.FQPLs.th_conns_def # not trimming here to FQPLs enabled, but later after expanding into a full set.
             gr_dict = {0: 'go', 1: 'return'}  # go-return dictionary used for printing helpful error messages
             tb_dict = {0: 'bottom', 1: 'top'}  # top-bottom dictionary used for printing helpful error messages
 
             # ----- windings thermal connections ------
             # define the connections on general position in turn, on 1-based numbering as in ProteCCT (to avoid confusion)
             th_conns_h_def_1 = []
@@ -1605,15 +1605,15 @@
         """
         Function is specific to CCT magnets windings.
         It assigns values listed in list_of_attr_names below + it sets self.model_data.CoilWindings.conductor_to_group
         """
         wwns = self.model_data.CoilWindings.CCT_straight.winding_numRowStrands  # number of wires in width direction
         whns = self.model_data.CoilWindings.CCT_straight.winding_numColumnStrands  # number of wires in height direction
         n_turns_formers = self.model_data.CoilWindings.CCT_straight.winding_numberTurnsFormers  # number of turns [-]
-        fqpl_names = [val for val, flag in zip(self.model_data.Quench_Protection.FQPLs.names, self.model_data.Quench_Protection.FQPLs.enabled) if flag]
+        fqpl_names = [val for val, flag in zip(self.model_data.Quench_Protection.FQPCs.names, self.model_data.Quench_Protection.FQPCs.enabled) if flag]
 
         turn_to_inductance_block = []
         turn_number = 0
         for winding_i in range(len(n_turns_formers)):
             for _ in range(n_turns_formers[winding_i]):
                 turn_number += 1
                 for turn in range(wwns[winding_i] * whns[winding_i]):
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2023.5.3/steam_sdk/builders/BuilderModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,31 +525,37 @@
         # Write output yaml file
         parser_PyBBQ = ParserPyBBQ(builder_PyBBQ)
         nameFilePyBBQ = os.path.join(self.output_path, conductor_name + '.yaml')  # full path of the PyBBQ input file to write
         parser_PyBBQ.writePyBBQ2yaml(full_path_file_name=nameFilePyBBQ, verbose=self.verbose)
 
     def buildSIGMA(self, simulation_name = None):
         """
-                  Building a FiQuS model
+                  Building a SIGMA model
                   :param simulation_name: This is used in analysis steam to change yaml name from magnet name to simulation name
-              """
+        """
+        # Copy necessary files to working folder
+        bh_data_file_path = os.path.join(Path(__file__).parent.parent.parent, 'tests', 'builders', 'model_library', 'magnets', 'roxie.bhdata')
+        shutil.copyfile(bh_data_file_path, os.path.join(self.output_path, 'roxie.bhdata'))
+
+        coord_source_prev=self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source
         if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source == None:
             if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d != None:
                 path_map2d = os.path.join(Path(self.path_bh).parent, self.model_data.GeneralParameters.magnet_name, 'input', self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d )
-                destination_map2d = os.path.join(self.output_path, self.model_data.GeneralParameters.magnet_name + "_ROXIE_REFERENCE.map2d")
+                destination_map2d = os.path.join(self.output_path, simulation_name + "_ROXIE_REFERENCE.map2d")
                 # Copy map2d file
                 shutil.copyfile(path_map2d, destination_map2d)
-                coordinate_file_path = os.path.join(self.output_path, self.model_data.GeneralParameters.magnet_name + "_ROXIE_COORD.csv")
+                coordinate_file_path = os.path.join(self.output_path, simulation_name + "_ROXIE_COORD.csv")
                 # Create coordinate file
                 create_coordinate_file(path_map2d, coordinate_file_path)
                 # Set file as coordinate_source
                 self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source = coordinate_file_path
 
         builder_SIGMA = BuilderSIGMA(model_data=self.model_data, roxie_data=self.roxie_data,
                                      flag_build=self.flag_build, flag_plot_all=self.flag_plot_all, verbose=self.verbose)
+        self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source = coord_source_prev
 
         # if map2d specified then copy to working folder,
 
         # Write output files
         self.parser_SIGMA = ParserSIGMA(builder_SIGMA, verbose=self.verbose)
         self.parser_SIGMA.writeSIGMA2yaml(output_path=self.output_path, simulation_name=simulation_name,
                                           append_str_to_magnet_name='_SIGMA')
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2023.5.3/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2023.5.3/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/BuilderSIGMA.py` & `steam-sdk-2023.5.3/steam_sdk/builders/BuilderSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2023.5.3/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/Solenoids.py` & `steam-sdk-2023.5.3/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2023.5.3/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam-sdk-2023.5.3/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2023.5.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataConductor.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataDakota.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataFiQuS.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,195 @@
 from pydantic import BaseModel
 from typing import (Dict, List, Union, Literal)
+
+from steam_sdk.data.DataConductor import ConstantJc, Bottura, CUDI3, Bordini, BSCCO_2212_LBNL, CUDI1, Summers, Round, \
+    Rectangular, Rutherford, Mono, Ribbon
 from steam_sdk.data.DataRoxieParser import RoxieData
 from steam_sdk.data.DataModelMagnet import RunFiQuS
 from steam_sdk.data.DataModelMagnet import MeshCCT
 from steam_sdk.data.DataModelMagnet import Air_g
 from steam_sdk.data.DataModelMagnet import MultipoleGeometry
 from steam_sdk.data.DataModelMagnet import MultipoleMesh
 from steam_sdk.data.DataModelMagnet import MultipoleSolve
 from steam_sdk.data.DataModelMagnet import MultipolePostProc
 
 
-class MultipoleMono(BaseModel):
+class QuenchHeaters(BaseModel):
+    """
+        Level 2: Class for FiQuS input (.yaml)
+    """
+    N_strips: int = None
+    t_trigger: List[float] = None
+    U0: List[float] = None
+    C: List[float] = None
+    R_warm: List[float] = None
+    w: List[float] = None
+    h: List[float] = None
+    s_ins: List[float] = None
+    type_ins: List[str] = None
+    s_ins_He: List[float] = None
+    type_ins_He: List[str] = None
+    l: List[float] = None
+    l_copper: List[float] = None
+    l_stainless_steel: List[float] = None
+    ids: List[int] = None
+    turns: List[int] = None
+    turns_sides: List[str] = None
+
+
+class Cliq(BaseModel):
+    """
+        Level 2: Class for FiQuS input (.yaml)
+    """
+    t_trigger: float = None
+    current_direction: List[int] = None
+    sym_factor: int = None
+    N_units: int = None
+    U0: float = None
+    C: float = None
+    R: float = None
+    L: float = None
+    I0: float = None
+
+
+class FQPCs(BaseModel):
+    """
+        Level 2: Class for FiQuS input (.yaml)
     """
-        Rutherford cable type
+    enabled: List[bool] = None  # list specifying which fqpc is enabled
+    names: List[str] = None  # name to use in gmsh and getdp
+    fndpls: List[int] = None  # fqpc number of divisions per length
+    fwws: List[float] = None  # fqpc wire widths (assuming rectangular) for theta = 0 this is x dimension
+    fwhs: List[float] = None  # fqpc wire heights (assuming rectangular) for theta = 0 this is y dimension
+    r_ins: List[
+        float] = None  # radiuses for inner diameter for fqpc (radial (or x direction for theta=0) for placing the fqpc
+    r_bs: List[float] = None  # radiuses for bending the fqpc by 180 degrees
+    n_sbs: List[int] = None  # number of 'bending segmetns' for the 180 degrees turn
+    thetas: List[float] = None  # rotation in deg from x+ axis towards y+ axis about z axis.
+    z_starts: List[
+        str] = None  # which air boundary to start at. These is string with either: z_min or z_max key from the Air region.
+    z_ends: List[float] = None  # z coordinate of loop end
+    currents: List[float] = None  # current in the wire
+    sigmas: List[float] = None  # electrical conductivity
+    mu_rs: List[float] = None  # relative permeability
+    th_conns_def: List[List] = None
+
+
+class Circuit(BaseModel):
+    """
+        Level 1: Class for FiQuS input (.yaml)
+    """
+    R_circuit: float = None
+    L_circuit: float = None
+    R_parallel: float = None
+
+
+class EnergyExtraction(BaseModel):
+    """
+        Level 1: Class for FiQuS input (.yaml)
+    """
+    t_trigger: float = None
+    R_EE: float = None
+    power_R_EE: float = None
+    L: float = None
+    C: float = None
+
+
+class PowerSupply(BaseModel):
+    """
+        Level 1: Class for FiQuS input (.yaml)
+    """
+    I_initial: float = None
+    t_off: float = None
+    t_control_LUT: List[float] = None
+    I_control_LUT: List[float] = None
+    R_crowbar: float = None
+    Ud_crowbar: float = None
+
+
+class QuenchProtection(BaseModel):
+    """
+        Level 1: Class for FiQuS Multipole
+    """
+    energy_extraction: EnergyExtraction = EnergyExtraction()
+    quench_heaters: QuenchHeaters = QuenchHeaters()
+    cliq: Cliq = Cliq()
+    FQPCs: FQPCs = FQPCs()
+
+
+class MultipoleMonoSet(BaseModel):
+    """
+        Rutherford cable type for settings (.set)
     """
     type: Literal['Mono']
     bare_cable_width: float = None
     bare_cable_height_mean: float = None
 
 
-class MultipoleRibbon(BaseModel):
+class MultipoleRibbonSet(BaseModel):
     """
-        Rutherford cable type
+        Rutherford cable type for settings (.set)
     """
     type: Literal['Ribbon']
     bare_cable_width: float = None
     bare_cable_height_mean: float = None
 
 
-class MultipoleRutherford(BaseModel):
+class MultipoleRutherfordSet(BaseModel):
     """
-        Rutherford cable type
+        Rutherford cable type for settings (.set)
     """
     type: Literal['Rutherford']
     bare_cable_width: float = None
     bare_cable_height_mean: float = None
 
 
+class MultipoleConductorSet(BaseModel):
+    """
+        Class for conductor type for settings (.set)
+    """
+    cable: Union[MultipoleRutherfordSet, MultipoleRibbonSet, MultipoleMonoSet] = {'type': 'Rutherford'}
+
+
 class MultipoleConductor(BaseModel):
     """
-        Class for conductor type
+        Class for conductor type for FiQuS input (.yaml)
     """
-    cable: Union[MultipoleRutherford, MultipoleRibbon, MultipoleMono] = {'type': 'Rutherford'}
+    version: str = None
+    case: str = None
+    state: str = None
+    cable: Union[Rutherford, Ribbon, Mono] = {'type': 'Rutherford'}
+    strand: Union[Round, Rectangular] = {'type': 'Round'}  # TODO: Tape, WIC
+    Jc_fit: Union[ConstantJc, Bottura, CUDI1, CUDI3, Summers, Bordini, BSCCO_2212_LBNL] = {
+        'type': 'CUDI1'}  # TODO: CUDI other numbers? , Roxie?
+
+
+class MultipoleRoxieGeometry(BaseModel):
+    """
+        Class for FiQuS multipole Roxie data (.geom)
+    """
+    Roxie_Data: RoxieData = RoxieData()
 
 
 class MultipoleGeneralSetting(BaseModel):
     """
         Class for general information on the case study
     """
     I_ref: List[float] = None
 
 
 class MultipoleModelDataSetting(BaseModel):
     """
-        Class for model data
+        Class for model data for settings (.set)
     """
     general_parameters: MultipoleGeneralSetting = MultipoleGeneralSetting()
-    conductors: Dict[str, MultipoleConductor] = {}
-
-#######################################################################################################################
+    conductors: Dict[str, MultipoleConductorSet] = {}
 
 
-class MultipoleRoxieGeometry(BaseModel):
-    """
-        Class for FiQuS multipole Roxie data (.geom)
-    """
-    Roxie_Data: RoxieData = RoxieData()
+#######################################################################################################################
 
 
 class MultipoleSettings(BaseModel):
     """
         Class for FiQuS multipole settings (.set)
     """
     Model_Data_GS: MultipoleModelDataSetting = MultipoleModelDataSetting()
@@ -112,19 +232,21 @@
     """
         Level 2: Class for FiQuS CCT
     """
     names: List[str] = None  # name to use in gmsh and getdp
     fndpls: List[int] = None  # fqpl number of divisions per length
     fwws: List[float] = None  # fqpl wire widths (assuming rectangular) for theta = 0 this is x dimension
     fwhs: List[float] = None  # fqpl wire heights (assuming rectangular) for theta = 0 this is y dimension
-    r_ins: List[float] = None  # radiuses for inner diameter for fqpl (radial (or x direction for theta=0) for placing the fqpl
+    r_ins: List[
+        float] = None  # radiuses for inner diameter for fqpl (radial (or x direction for theta=0) for placing the fqpl
     r_bs: List[float] = None  # radiuses for bending the fqpl by 180 degrees
     n_sbs: List[int] = None  # number of 'bending segmetns' for the 180 degrees turn
     thetas: List[float] = None  # rotation in deg from x+ axis towards y+ axis about z axis.
-    z_starts: List[str] = None  # which air boundary to start at. These is string with either: z_min or z_max key from the Air region.
+    z_starts: List[
+        str] = None  # which air boundary to start at. These is string with either: z_min or z_max key from the Air region.
     z_ends: List[float] = None  # z coordinate of loop end
 
 
 class CCTGeometry(BaseModel):
     """
         Level 2: Class for FiQuS CCT for FiQuS input
     """
@@ -170,15 +292,15 @@
 
 class SolveCCT(BaseModel):
     """
         Level 2: Class for FiQuS CCT
     """
     windings: Winding_s = Winding_s()  # windings solution time _inputs
     formers: Former_s = Former_s()  # former solution time _inputs
-    fqpls: FQPL_s = FQPL_s() # fqpls solution time _inputs
+    fqpls: FQPL_s = FQPL_s()  # fqpls solution time _inputs
     air: Air_s = Air_s()  # air solution time _inputs
     pro_template: str = None  # file name of .pro template file
     variables: List[str] = None  # Name of variable to post-process by GetDP, like B for magnetic flux density
     volumes: List[str] = None  # Name of volume to post-process by GetDP, line Winding_1
     file_exts: List[str] = None  # Name of file extensions to post-process by GetDP, like .pos
 
 
@@ -186,18 +308,21 @@
     """
         Class for FiQuS CCT input file
     """
     windings_wwns: List[int] = None  # wires in width direction numbers
     windings_whns: List[int] = None  # wires in height direction numbers
     additional_outputs: List[str] = None  # Name of software specific input files to prepare, like :LEDET3D
     winding_order: List[int] = None
-    fqpl_export_trim_tol: List[float] = None  # this multiplier times winding extend gives 'z' coordinate above(below) which hexes are exported for LEDET, length of this list must match number of fqpls
+    fqpl_export_trim_tol: List[
+        float] = None  # this multiplier times winding extend gives 'z' coordinate above(below) which hexes are exported for LEDET, length of this list must match number of fqpls
     variables: List[str] = None  # Name of variable to post-process by python Gmsh API, like B for magnetic flux density
     volumes: List[str] = None  # Name of volume to post-process by python Gmsh API, line Winding_1
     file_exts: List[str] = None  # Name of file extensions o post-process by python Gmsh API, like .pos
+
+
 ############################
 
 
 class CCTDM(BaseModel):
     """
         Class for FiQuS CCT
     """
@@ -229,9 +354,11 @@
 class DataFiQuS(BaseModel):
     """
         Class for FiQuS
     """
     general: General = General()
     run: RunFiQuS = RunFiQuS()
     magnet: Union[MPDM, CCTDM] = {'type': 'multipole'}
-
-
+    circuit: Circuit = Circuit()
+    power_supply: PowerSupply = PowerSupply()
+    quench_protection: QuenchProtection = QuenchProtection()
+    conductors: Dict[str, MultipoleConductor] = {}
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataLEDET.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataModelMagnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     type_ins_He: Union[List[str], List[List[str]]] = []
     l: List[float] = []
     l_copper: List[float] = []
     l_stainless_steel: List[float] = []
     f_cover: List[float] = []
     iQH_toHalfTurn_From: List[int] = []
     iQH_toHalfTurn_To: List[int] = []
+    turns_sides: List[str] = []
 
 
 class CLIQ(BaseModel):
     """
         Level 2: Class for the CLIQ parameters
     """
     t_trigger: float = None                        # tCLIQ
@@ -204,15 +205,15 @@
     U0: float = None                       # V_cliq_0 (SIGMA)
     C: float = None                        # C_cliq (SIGMA)
     R: float = None                        # Rcapa (LEDET), R_cliq (SIGMA)
     L: float = None                        # L_cliq
     I0: float = None                       # I_cliq_0
 
 
-class FQPLs(BaseModel):  # Geometry related fqpls _inputs
+class FQPCs(BaseModel):  # Geometry related fqpls _inputs
     """
         Level 2: Class for the FQPLs parameters for protection
     """
     enabled: List[bool] = None  # list specifying which fqpl is enabled
     names: List[str] = None  # name to use in gmsh and getdp
     fndpls: List[int] = None  # fqpl number of divisions per length
     fwws: List[float] = None  # fqpl wire widths (assuming rectangular) for theta = 0 this is x dimension
@@ -232,15 +233,15 @@
 class QuenchProtection(BaseModel):
     """
         Level 1: Class for quench protection
     """
     Energy_Extraction: EnergyExtraction = EnergyExtraction()
     Quench_Heaters: QuenchHeater = QuenchHeater()
     CLIQ: CLIQ = CLIQ()
-    FQPLs: FQPLs = FQPLs()
+    FQPCs: FQPCs = FQPCs()
 
 
 ############################
 # BBQ options
 class GeometryBBQ(BaseModel):
     """
         Level 2: Class for geometry options in BBQ
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataSIGMA.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataSettings.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DataSignal.py` & `steam-sdk-2023.5.3/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2023.5.3/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2023.5.3/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2023.5.3/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2023.5.3/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2023.5.3/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2023.5.3/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2023.5.3/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2023.5.3/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2023.5.3/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2023.5.3/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2023.5.3/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2023.5.3/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2023.5.3/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserDatToCsv.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserSIGMA.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2023.5.3/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2023.5.3/steam_sdk/parsims/ParsimConductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,14 +546,15 @@
                 if not coil.coil_resistance_room_T:
                     warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database. Not optimizing fraction of copper.')
                     continue
                 # calculate Cu_noCu for every conductor sample and use mean value
                 list_optimized_Cu_noCu = []
                 for sample in coil.conductorSamples:
                     list_optimized_Cu_noCu.append(self.__optimize_fCu_with_resistance_meas(sample, coil_name, self.model_data.Conductors[idx], coil))
+                # if the Cu no Cu ratio could be parsed directly from a column, overwrite it with optimized value
                 dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = np.mean(list_optimized_Cu_noCu)
 
     def __optimize_fCu_with_resistance_meas(self, conductor_sample: ConductorSample, coil_name: str,
                                             original_conductor: Conductor, coil: Coil):
         """
         Optimizes the fraction of copper (fCu) using the room temperature resistance measurements using the formula:
         R_RT = rho * L / (fCu * A_cond) * f_twist_pitch -> solving for fCu
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2023.5.3/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2023.5.3/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,18 @@
         # Read the input file
         if path_input_file.endswith('.csv'):
             df_events = pd.read_csv(path_input_file)
         elif path_input_file.endswith('.xlsx'):
             df_events = pd.read_excel(path_input_file)
         else:
             raise Exception(f'The extension of the file {path_input_file} is not supported.')
-        df_events = pd.DataFrame([[None if pd.isna(x) else x for x in row] for row in df_events.values], columns=df_events.columns)
+        if df_events["Circuit Name"][0].startswith(("RCD-RCO", "RCBH", "RCBV")):
+            df_events = pd.DataFrame([[0 if pd.isna(x) else x for x in row] for row in df_events.values], columns=df_events.columns)
+        else:
+            df_events = pd.DataFrame([[None if pd.isna(x) else x for x in row] for row in df_events.values], columns=df_events.columns)
         #df_events = df_events.dropna(axis=1, how='all')
 
         # validate dataframe - if csv file has a headline or empty rows on the top, skip row until there all columnnames have values
         skip_rows = 0
         while any(['Unnamed: ' in s for s in
                    df_events.columns]):  # pandas assigns the columname 'Unnamed: i' when no name can be found
             skip_rows += 1
@@ -77,15 +80,15 @@
             new_event = DataEventCircuit()
             circuit_type = event_info["Circuit Family"]
             circuit_name = event_info["Circuit Name"]
             rsetattr(new_event, 'GeneralParameters.circuit_type', circuit_type)
 
             if self.verbose:
                 print(f"circuit type: {circuit_type}")
-            if circuit_type in ["RCBH", "RCBV"]:
+            if circuit_type.startswith(('RCBH', 'RCBV')):
                 parsed_columns += self.__read_60A(event_info, new_event)
             elif circuit_type == "RQX":
                 parsed_columns += self.__read_RQX(event_info, new_event)
             elif circuit_type in ["RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
                 parsed_columns += self.__read_IPQ(event_info, new_event)
             elif circuit_type in ["RD1", "RD2", "RD3", "RD4"]:
                 parsed_columns += self.__read_IPD(event_info, new_event)
@@ -150,15 +153,24 @@
 
         # Loop trough each element of self.list_events and write parameters to csv
         for i, event in enumerate(self.list_events):
             print(i, event)
             new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
             event_data = self.__write_event(event)
             event_data_counter = 0
-            if isinstance(event_data, list):
+            if simulation_name == "RCD":
+                new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
+                new_row.update(event_data[1][0])
+                all_rows.append(new_row)
+                list_paramerers = list(set(list_paramerers + list(new_row.keys())))
+            elif simulation_name == "RCO":
+                new_row.update(event_data[0])
+                all_rows.append(new_row)
+                list_paramerers = list(set(list_paramerers + list(new_row.keys())))
+            elif isinstance(event_data, list):
                 for data in event_data:
                     new_row.update(data)
                     if simulation_name in ["RQ_47magnets", "RQ_51magnets", "RCBX"] and event_data_counter % 2 != 0:
                         new_row['simulation_number'] = 2
                     all_rows.append(new_row.copy())
                     list_paramerers = list(set(list_paramerers + list(new_row.keys())))
                     event_data_counter = event_data_counter + 1
@@ -878,28 +890,30 @@
                 return_list.append(key)
 
         return return_list
 
     def __write_event(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         circuit_type = event.GeneralParameters.circuit_type
         circuit_name = event.GeneralParameters.name
-        if circuit_type in ['RCBH', 'RCBV', "RQT12", "RQT13", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RQSX3", "RCBYV", "RCBYH", "RCBCH", "RCBCV", "RD1", "RD2", "RD3", "RD4"]:
+        if circuit_type in ["RQT12", "RQT13", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RQSX3", "RCBYV", "RCBYH", "RCBCH", "RCBCV", "RD1", "RD2", "RD3", "RD4"] or circuit_type.startswith(('RCBH', 'RCBV')):
             event_dict = self.__write_common_circuit_family(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RQ":
             event_dict = self.__write_RQ(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type in ["RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
             event_dict = self.__write_IPQ(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RQX":
             event_dict = self.__write_RQX(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type in ["RCS", "ROD", "ROF", "RSD", "RSF", "RQTL9", "RQTD", "RQTF"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8):
             event_dict = self.__write_600A_with_EE(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RB":
             event_dict = self.__write_RB(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RCBX":
             event_dict = self.__write_RCBX(event, t_after_PC_off=t_after_PC_off)
+        elif circuit_name.startswith("RCD-RCO"):
+            event_dict = self.__write_RCD_RCO(event, t_after_PC_off=t_after_PC_off)
         return event_dict
 
     def __write_common_circuit_family(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         """
         Extract the information for an event of circuit type RCB.
 
         Parameters:
@@ -910,16 +924,20 @@
 
         """
         circuit_name = event.GeneralParameters.name
         event_dict = dict()
         t_start = 0  # hard-coded
         I_start = 0.0  # hard-coded
         dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
-        dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
-        current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
+        if circuit_name.startswith("RCD-RCO"):
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[0]
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[0]
+        else:
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
         t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
         event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
 
         # TODO
         # if dI/dt is 0:
         # read dI/dt and dI/st2 from the STEAM model
         # set the plateau length
@@ -1056,14 +1074,33 @@
             t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
             t_PC_off_list.append(t_PC_off)
             event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off_list
             list.append(event_dict)
 
         return list
 
+    def __write_RCD_RCO(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+        """
+        Extract the information for an event of circuit type RCD_RCO.
+
+        Parameters:
+            event (DataEventCircuit): The data event object to read the data.
+
+        Returns:
+            list[dict]: A list of dictionaries containing the RCD_RCO information.
+
+        """
+        list= []
+        event_dict_1 = self.__write_common_circuit_family(event, t_after_PC_off)
+        event_dict_1['GlobalParameters.global_parameters.t_plateau'] = event_dict_1['GlobalParameters.global_parameters.t_plateau'][0]
+        event_dict_2 = self.__write_600A_with_EE(event, t_after_PC_off)
+        list.append(event_dict_1)
+        list.append(event_dict_2)
+        return list
+
     def __write_RQX(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         """
         Extract the information for an event of circuit type RQX.
 
         Parameters:
             event (DataEventCircuit): The data event object to read the data.
 
@@ -1275,16 +1312,20 @@
         list= []
         t_EE_list = []
         t_PC_off_list = []
         event_dict = dict()
         t_start = 0  # hard-coded
         I_start = 0.0  # hard-coded
         dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
-        dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
-        current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
+        if circuit_name.startswith("RCD-RCO"):
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[1]
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[1]
+        else:
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
         t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
         t_PC_off_list.append(t_PC_off)
         event_dict['GlobalParameters.global_parameters.t_EE'] = t_PC_off + 0.008
         event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off_list
         event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = t_EE_list.append(t_PC_off + 0.008)
 
         list.append(event_dict)
@@ -1322,15 +1363,18 @@
 
     def __handle_ramp_rate_cases(self, event: DataEventCircuit, circuit_name: str, t_after_PC_off: float, t_start: float, I_start: float, dI_dt: float, dI_dt2: float, current_at_discharge: float, event_dict: dict ):
         if dI_dt == 0:
             I_end = current_at_discharge
             dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt'])
             time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
             t_plateau = event.PoweredCircuits[circuit_name].plateau_duration
-            t_PC_off = t_start + time_to_reach_I + t_plateau
+            if circuit_name.startswith("RCD-RCO"):
+                t_PC_off = t_start + time_to_reach_I + t_plateau[0]
+            else:
+                t_PC_off = t_start + time_to_reach_I + t_plateau
             event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
             event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
 
         elif np.sign(dI_dt) != np.sign(current_at_discharge):
             I_end_1 = 1.2*current_at_discharge
             I_end_2 = current_at_discharge
             I_target = current_at_discharge + np.sign(current_at_discharge) * 100.0
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2023.5.3/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,28 +119,30 @@
         # check inputs
         if len(simulation_numbers) != len(self.list_events):
             raise Exception(f'length of input simulation numbers ({len(simulation_numbers)}) differs from length of events found in the input file ({len(self.list_events)})')
 
         # Make target folder if it is missing
         make_folder_if_not_existing(os.path.dirname(path_outputfile_event_csv))
 
-        # open file in writing mode
+        # make dict for every row and store it in a list of dicts - loop trough each element of self.list_events and write parameters to csv
+        row_dicts = []
+        for i, event in enumerate(self.list_events):
+            new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
+            new_row.update(self.__write_analysis_powering(event, t_PC_off))
+            new_row.update(self.__write_analysis_CLIQ(event, current_polarities_CLIQ))
+            new_row.update(self.__write_analysis_QH(event, dict_QH_circuits_to_QH_strips))
+            new_row.update(self.__write_analysis_general_parameters(event))
+            row_dicts.append(new_row)
+
+        # write csv file
         with open(path_outputfile_event_csv, 'w', newline='') as csv_file:
-            new_row = dict()
-            # loop trough each element of self.list_events and write parameters to csv
-            for i, event in enumerate(self.list_events):
-                new_row.clear()
-                new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
-                new_row.update(self.__write_analysis_powering(event, t_PC_off))
-                new_row.update(self.__write_analysis_CLIQ(event, current_polarities_CLIQ))
-                new_row.update(self.__write_analysis_QH(event, dict_QH_circuits_to_QH_strips))
-                new_row.update(self.__write_analysis_general_parameters(event))
-                writer = csv.DictWriter(csv_file, fieldnames=new_row.keys())
-                if i == 0: writer.writeheader()
-                writer.writerow(new_row)
+            fieldnames = list(set(key for d in row_dicts for key in d))  # TODO what happens when value is missing in dict
+            writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
+            writer.writeheader()
+            for row in row_dicts: writer.writerow(row)
 
     def set_up_viewer(self, path_output_viewer_csv: str, default_keys: DefaultParsimEventKeys,
                       simulation_numbers: List[int], simulation_name: str, software: str):
         '''
         Writes a csv file that can be used to run a STEAM Viewer step
 
         :param path_output_viewer_csv: The path to the output csv file for the Viewer.
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimSweep.py` & `steam-sdk-2023.5.3/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2023.5.3/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,15 @@
                     if use_markers:     # user
                         marker = markers[i]
                     else:
                         marker = 'None'
                     if len(self.values) == 3:
                         label = f'{magnet_label},{value}:{leng + sim_names[sim_nr]}'
                     else:
-                        #label = f'{magnet_label}:{leng + sim_names[sim_nr]}'
-                        label = f'{sim_nr}'
+                        label = f'{magnet_label}:{leng + sim_names[sim_nr]}'
                     ax.plot(self.time_data[magnet_label][self.time_name][sim_nr], self.data[magnet_label][value][sim_nr],
                             markevery=20, marker=marker, label=label)
                     i += 1
         ax.tick_params(labelsize=self.cs['font_size'])
         ax.set_xlabel(f"Time (s)", size=self.cs['font_size'])#.set_fontproperties(font)
         if len(self.values) == 3:   # CLIQ currents plot
             value = '$I_{A}, I_{B}, I_{CLIQ}$'
@@ -113,44 +112,43 @@
         print(self.data)
 
 if __name__ == "__main__":
     base_path = r"C:\tempLEDET\LEDET"   # path to ledet folder
     model_names_list = [['robust_12T_50_mm_MQXF_cable_5_blocks_V2'], ['robust_12T_50_mm_MQXF_cable_6_blocks_V2'], ['robust_12T_56_mm_MQXF_cable_6_blocks_V2']]
     model_labels_list = [['50mm,5b'], ['50mm,6b'], ['56mm,6b']]
 
-    model_names = ['robust_12T_50_mm_MQXF_cable_5_blocks_V2']
-    model_labels = ['50mm,5b']
+    # model_names = ['robust_12T_50_mm_MQXF_cable_5_blocks_V2']
+    # model_labels = ['50mm,5b']
     # model_names = ['robust_12T_50_mm_MQXF_cable_6_blocks_V2']
     # model_labels = ['50mm,6b']
     # model_names = ['robust_12T_56_mm_MQXF_cable_6_blocks_V2']
     # model_labels = ['56mm,6b']
     # sim_nr_list_of_lists = [[13, 113], [13, 113], [13, 113]]
     # #sim_nr_list_of_lists = [[3, 103], [3, 103], [3, 103]]
     # sim_nr_list_of_lists = [[3], [3], [3]]
     # sim_nr_list_of_lists = [[3]]
     #sim_nr_list_of_lists = [[3, 13], [3, 13], [3, 13]]
     #sim_nr_list_of_lists = [[13], [13], [13]]
 
     sim_nr_list_of_lists = [[1, 2, 3, 13, 4, 14, 5, 6, 16, 7, 17]]
-    sim_nr_list_of_lists = [[303]]
     #sim_nr_list_of_lists = [[101, 102, 103, 113, 104, 114, 105, 106, 116, 107, 117]]
 
-    #sim_nr_list_of_lists = [[3, 13, 4, 14, 6, 16, 7, 17]]
-    #sim_nr_list_of_lists = [[103, 113, 104, 114, 106, 116, 107, 117]]
+    sim_nr_list_of_lists = [[3, 13, 4, 14, 6, 16, 7, 17]]
+    sim_nr_list_of_lists = [[103, 113, 104, 114, 106, 116, 107, 117]]
     #values = ['$I_{A}$', '$I_{B}$', '$I_{CLIQ}$']
 
     #values = ['$T_{max}$']
     #values = ['$T_{max adb}$']
     #values = ['$U_{max}$']
     #values = ['$U_{min}$']
     #values = ['$R_{mag}$']
-    #values = ['$I_{A}$']
+    values = ['$I_{A}$']
     values = ['$I_{CLIQ}$']
     style = 'presentation'
 
 
     pa = PlotterAnalysis(base_path)
     pa.set_plot_style(style)
     for model_names, model_labels in zip(model_names_list, model_labels_list):
         pa.read_data(model_names, model_labels, sim_nr_list_of_lists, values)
-        pa.plot_selected_vs_time(use_markers=0, save=0)
+        pa.plot_selected_vs_time(use_markers=0, save=1)
     #pa.print_data()
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2023.5.3/steam_sdk/plotters/PlotterMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2023.5.3/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2023.5.3/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2023.5.3/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2023.5.3/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2023.5.3/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2023.5.3/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2023.5.3/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from pathlib import Path
 import yaml
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 
 if __name__ == "__main__":
-    # path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'C:\\Users\emm\cernbox\SWAN_projects\steam_models\magnets')
-    path_models = Path.joinpath(Path(__file__).parent.parent.parent, r'E:\Python\steam_models\magnets')
-    path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/magnets')
+    path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'C:\\Users\emm\cernbox\SWAN_projects\steam_models\magnets')
+    path_models = Path.joinpath(Path(__file__).parent.parent.parent, r'C:\Users\jlidholm\cernbox\Git-projects\steam_models\magnets')
+    #path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/magnets')
     models = [x.parts[-1] for x in Path(path_models).iterdir() if x.is_dir()]
-    #models = ['MCBRD']
+    #models = ['MQXA']
 
     for mm in models:
         # Read file
         file_model_data = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '.yaml')
         if os.path.isfile(file_model_data):
             # Load yaml keys into DataAnalysis dataclass
             with open(file_model_data, "r") as stream:
@@ -40,14 +40,15 @@
             # model_data.Options_LEDET.heat_exchange.iContactAlongHeight_pairs_to_remove = dictionary_yaml['CoilWindings']['heat_exchange']['iContactAlongHeight_pairs_to_remove']
             # model_data.Options_LEDET.heat_exchange.th_insulationBetweenLayers = dictionary_yaml['CoilWindings']['heat_exchange']['th_insulationBetweenLayers']
             #
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.alphaDEG_ht = dictionary_yaml['CoilWindings']['multipole']['alphaDEG_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.rotation_ht = dictionary_yaml['CoilWindings']['multipole']['rotation_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirror_ht = dictionary_yaml['CoilWindings']['multipole']['mirror_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirrorY_ht = dictionary_yaml['CoilWindings']['multipole']['mirrorY_ht']
+            model_data.Quench_Protection.Quench_Heaters.turns_sides = ["O"] * len(model_data.Quench_Protection.Quench_Heaters.iQH_toHalfTurn_From)
 
             # Check and reformat the key values
             model_data = DataModelMagnet(**model_data.dict())
 
             # Write file
             # file_model_data_output = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '_MODIFIED.yaml')  # use this line if you wish to test the results of this script
             file_model_data_output = file_model_data  # use this line if you wish to really update all yaml input files
```

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2023.5.3/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2023.5.3/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2023.5.3/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/create_coordinate_file_SIGMA.py` & `steam-sdk-2023.5.3/steam_sdk/utils/create_coordinate_file_SIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2023.5.3/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/misc.py` & `steam-sdk-2023.5.3/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2023.5.3/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/tic_toc.py` & `steam-sdk-2023.5.3/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/utils/utils_PC.py` & `steam-sdk-2023.5.3/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/viewers/Viewer.py` & `steam-sdk-2023.5.3/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/viewers/ViewerMeas.py` & `steam-sdk-2023.5.3/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/viewers/ViewerSim.py` & `steam-sdk-2023.5.3/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2023.5.3/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.2/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2023.5.3/steam_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.5.2
+Version: 2023.5.3
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SDK,STEAM,API,CERN
+Keywords: API,SDK,STEAM,CERN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.5.2/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2023.5.3/steam_sdk.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-.gitignore
-.gitlab-ci.yml
 MANIFEST.in
-Readme.md
-mkdocs.yaml
-requirements.txt
 setup.py
 steam_sdk/__init__.py
 steam_sdk.egg-info/PKG-INFO
 steam_sdk.egg-info/SOURCES.txt
 steam_sdk.egg-info/dependency_links.txt
 steam_sdk.egg-info/requires.txt
 steam_sdk.egg-info/top_level.txt
@@ -39,30 +34,24 @@
 steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
 steam_sdk/builders/BuilderFiQuS.py
 steam_sdk/builders/BuilderLEDET.py
 steam_sdk/builders/BuilderModel.py
 steam_sdk/builders/BuilderProteCCT.py
 steam_sdk/builders/BuilderPyBBQ.py
 steam_sdk/builders/BuilderSIGMA.py
-steam_sdk/builders/Readme.md
 steam_sdk/builders/SelfMutualInductanceCalculation.py
 steam_sdk/builders/Solenoids.py
 steam_sdk/builders/__init__.py
 steam_sdk/builders/geometricFunctions.py
 steam_sdk/configs/__init__.py
-steam_sdk/configs/plotters/Readme.md
 steam_sdk/configs/plotters/__init__.py
-steam_sdk/configs/tools_defaults/Readme.md
 steam_sdk/configs/tools_defaults/ToolDefaultReader.py
 steam_sdk/configs/tools_defaults/__init__.py
 steam_sdk/configs/tools_defaults/LEDET/__init__.py
-steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
 steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
-steam_sdk/configs/users/Readme.md
-steam_sdk/cosims/Readme.md
 steam_sdk/cosims/__init__.py
 steam_sdk/data/DataAnalysis.py
 steam_sdk/data/DataConductor.py
 steam_sdk/data/DataDakota.py
 steam_sdk/data/DataEventCircuit.py
 steam_sdk/data/DataEventMagnet.py
 steam_sdk/data/DataFiQuS.py
@@ -77,32 +66,27 @@
 steam_sdk/data/DataRoxieParser.py
 steam_sdk/data/DataSIGMA.py
 steam_sdk/data/DataSettings.py
 steam_sdk/data/DataSignal.py
 steam_sdk/data/DictionaryLEDET.py
 steam_sdk/data/DictionaryProteCCT.py
 steam_sdk/data/DictionaryPyBBQ.py
-steam_sdk/data/Readme.md
 steam_sdk/data/TemplateLEDET.py
 steam_sdk/data/TemplateProteCCT.py
 steam_sdk/data/__init__.py
 steam_sdk/drivers/DriverAnalysis.py
 steam_sdk/drivers/DriverDakota.py
 steam_sdk/drivers/DriverFiQuS.py
 steam_sdk/drivers/DriverLEDET.py
 steam_sdk/drivers/DriverPSPICE.py
 steam_sdk/drivers/DriverProteCCT.py
 steam_sdk/drivers/DriverPyBBQ.py
 steam_sdk/drivers/DriverSIGMA.py
 steam_sdk/drivers/DriverXYCE.py
-steam_sdk/drivers/Readme.md
 steam_sdk/drivers/__init__.py
-steam_sdk/drivers/temp/postLEDET.py
-steam_sdk/drivers/temp/runLEDET.py
-steam_sdk/drivers/temp/simLEDET.py
 steam_sdk/parsers/CSD_Reader.py
 steam_sdk/parsers/ParserCOMSOLToTxt.py
 steam_sdk/parsers/ParserCond2d.py
 steam_sdk/parsers/ParserCsd.py
 steam_sdk/parsers/ParserCsv.py
 steam_sdk/parsers/ParserDakota.py
 steam_sdk/parsers/ParserDatToCsv.py
@@ -116,33 +100,27 @@
 steam_sdk/parsers/ParserProteCCT.py
 steam_sdk/parsers/ParserProtePyBBQ.py
 steam_sdk/parsers/ParserRoxie.py
 steam_sdk/parsers/ParserSIGMA.py
 steam_sdk/parsers/ParserTdms.py
 steam_sdk/parsers/ParserXYCE.py
 steam_sdk/parsers/ParserYAML.py
-steam_sdk/parsers/Readme.md
 steam_sdk/parsers/__init__.py
 steam_sdk/parsers/dict_to_in.py
-steam_sdk/parsers/templates/template_Dakota.in
 steam_sdk/parsims/ParsimConductor.py
 steam_sdk/parsims/ParsimDakota.py
 steam_sdk/parsims/ParsimEventCircuit.py
 steam_sdk/parsims/ParsimEventMagnet.py
 steam_sdk/parsims/ParsimSweep.py
-steam_sdk/parsims/Readme.md
 steam_sdk/parsims/__init__.py
-steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
-steam_sdk/parsims/translation_dicts/event_column_names.yaml
 steam_sdk/plotters/PlotterAnalysis.py
 steam_sdk/plotters/PlotterMap2d.py
 steam_sdk/plotters/PlotterModel.py
 steam_sdk/plotters/PlotterParametric.py
 steam_sdk/plotters/PlotterRoxie.py
-steam_sdk/plotters/Readme.md
 steam_sdk/plotters/__init__.py
 steam_sdk/postprocs/PostprocsMetrics.py
 steam_sdk/postprocs/__init__.py
 steam_sdk/utils/MTF_reading_functions.py
 steam_sdk/utils/ModifyModelData.py
 steam_sdk/utils/ModifyModelDataMagnet.py
 steam_sdk/utils/ModifyModelDataconductor.py
@@ -162,14 +140,12 @@
 steam_sdk/utils/tic_toc.py
 steam_sdk/utils/unique.py
 steam_sdk/utils/utils_PC.py
 steam_sdk/viewers/Viewer.py
 steam_sdk/viewers/ViewerMeas.py
 steam_sdk/viewers/ViewerSim.py
 steam_sdk/viewers/__init__.py
-steam_sdk/wrappers/Readme.md
 steam_sdk/wrappers/__init__.py
 steam_sdk/wrappers/wrapper_yaml.py
 steam_sdk/wrappers/java/__init__.py
 steam_sdk/wrappers/java/SING/__init__.py
-steam_sdk/wrappers/java/SING/jars/__init__.py
-steam_sdk/wrappers/java/SING/jars/steam-sing.jar
+steam_sdk/wrappers/java/SING/jars/__init__.py
```

