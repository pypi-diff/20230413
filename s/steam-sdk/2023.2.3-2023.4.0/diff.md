# Comparing `tmp/steam_sdk-2023.2.3.tar.gz` & `tmp/steam_sdk-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam_sdk-2023.2.3.tar", last modified: Fri Feb 24 11:28:38 2023, max compression
+gzip compressed data, was "dist\steam_sdk-2023.4.0.tar", last modified: Thu Apr 13 16:02:05 2023, max compression
```

## Comparing `steam_sdk-2023.2.3.tar` & `steam_sdk-2023.4.0.tar`

### file list

```diff
@@ -1,177 +1,202 @@
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.933519 steam_sdk-2023.2.3/
--rw-rw-rw-   0        0        0      122 2023-02-02 15:29:21.000000 steam_sdk-2023.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1498 2023-02-24 11:28:38.933519 steam_sdk-2023.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-02-24 11:28:38.933519 steam_sdk-2023.2.3/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-02-24 11:26:14.000000 steam_sdk-2023.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.543722 steam_sdk-2023.2.3/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.543722 steam_sdk-2023.2.3/steam_sdk/analyses/
--rw-rw-rw-   0        0        0    90927 2023-02-22 11:48:29.000000 steam_sdk-2023.2.3/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.559348 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.559348 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-10-12 14:45:26.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.574866 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-10-06 23:30:28.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-09-12 16:26:14.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-09-10 00:21:21.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-10-24 19:22:58.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-09-09 21:29:03.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-09-09 21:29:03.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.590491 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.590491 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.606113 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-09-30 09:15:14.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.621734 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-26 06:59:06.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.621734 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-10 00:27:54.000000 steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.668598 steam_sdk-2023.2.3/steam_sdk/builders/
--rw-rw-rw-   0        0        0    10098 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160973 2023-01-17 14:05:49.000000 steam_sdk-2023.2.3/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    32420 2023-02-23 13:00:16.000000 steam_sdk-2023.2.3/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-09-07 00:41:51.000000 steam_sdk-2023.2.3/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-08-22 11:29:04.000000 steam_sdk-2023.2.3/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    25338 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0    11689 2023-01-18 09:46:00.000000 steam_sdk-2023.2.3/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-06 11:41:34.000000 steam_sdk-2023.2.3/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.668598 steam_sdk-2023.2.3/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.668598 steam_sdk-2023.2.3/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.668598 steam_sdk-2023.2.3/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.684220 steam_sdk-2023.2.3/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0    32890 2022-10-04 12:05:12.000000 steam_sdk-2023.2.3/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0     1426 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.684220 steam_sdk-2023.2.3/steam_sdk/cosims/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.746705 steam_sdk-2023.2.3/steam_sdk/data/
--rw-rw-rw-   0        0        0     9267 2023-02-20 16:23:09.000000 steam_sdk-2023.2.3/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     8004 2023-02-24 08:35:20.000000 steam_sdk-2023.2.3/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-09-30 09:15:14.000000 steam_sdk-2023.2.3/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     3169 2023-01-19 08:55:39.000000 steam_sdk-2023.2.3/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0     8492 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10767 2022-10-04 11:56:26.000000 steam_sdk-2023.2.3/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-08-22 11:29:04.000000 steam_sdk-2023.2.3/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    34073 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2102 2023-02-08 16:15:27.000000 steam_sdk-2023.2.3/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-09-07 00:41:51.000000 steam_sdk-2023.2.3/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-03-07 20:47:17.000000 steam_sdk-2023.2.3/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     7899 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     1450 2023-02-02 08:17:41.000000 steam_sdk-2023.2.3/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-05 21:02:33.000000 steam_sdk-2023.2.3/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    22928 2022-10-04 11:58:22.000000 steam_sdk-2023.2.3/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-08-23 08:56:30.000000 steam_sdk-2023.2.3/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 09:57:32.000000 steam_sdk-2023.2.3/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0    27540 2022-10-04 11:54:05.000000 steam_sdk-2023.2.3/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-03-30 17:37:43.000000 steam_sdk-2023.2.3/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.777948 steam_sdk-2023.2.3/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-12-06 11:41:34.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-12-06 11:41:34.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-02-02 08:17:41.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2022-12-16 13:26:54.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-10-31 08:36:49.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-26 06:59:06.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-06-02 08:33:55.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     5729 2023-02-02 08:17:41.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-10-31 08:36:49.000000 steam_sdk-2023.2.3/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.840433 steam_sdk-2023.2.3/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-08-22 11:29:04.000000 steam_sdk-2023.2.3/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0     2290 2022-06-24 07:36:06.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1077 2022-08-29 08:22:53.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2023-01-16 11:54:48.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-13 08:48:18.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     8536 2023-02-02 15:29:22.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-09-30 09:15:14.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48056 2023-02-03 13:14:21.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-11-21 14:56:04.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10602 2023-02-20 11:15:56.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    67894 2023-02-07 07:36:54.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     3142 2023-01-27 15:21:24.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-02-03 13:16:35.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-09-26 06:59:06.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    92213 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11707 2022-09-07 14:38:46.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-02-02 12:20:26.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4195 2023-02-24 11:23:16.000000 steam_sdk-2023.2.3/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-09-02 10:44:52.000000 steam_sdk-2023.2.3/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.856054 steam_sdk-2023.2.3/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    12853 2023-02-16 13:45:53.000000 steam_sdk-2023.2.3/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-09-26 06:59:06.000000 steam_sdk-2023.2.3/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    58585 2023-02-24 08:37:11.000000 steam_sdk-2023.2.3/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-24 08:05:20.000000 steam_sdk-2023.2.3/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.871677 steam_sdk-2023.2.3/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    39596 2022-06-20 13:00:15.000000 steam_sdk-2023.2.3/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-06 11:41:34.000000 steam_sdk-2023.2.3/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8871 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0    18478 2023-02-02 15:39:34.000000 steam_sdk-2023.2.3/steam_sdk/plotters/PlotterSIGMA.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.871677 steam_sdk-2023.2.3/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-09-26 06:59:06.000000 steam_sdk-2023.2.3/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-14 13:30:58.000000 steam_sdk-2023.2.3/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.911407 steam_sdk-2023.2.3/steam_sdk/utils/
--rw-rw-rw-   0        0        0    14942 2022-06-30 20:06:54.000000 steam_sdk-2023.2.3/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     5145 2023-02-20 16:23:11.000000 steam_sdk-2023.2.3/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2023-02-16 13:22:34.000000 steam_sdk-2023.2.3/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-03-01 14:21:51.000000 steam_sdk-2023.2.3/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-06-12 12:41:34.000000 steam_sdk-2023.2.3/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-02-03 13:26:48.000000 steam_sdk-2023.2.3/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      167 2022-06-11 12:54:31.000000 steam_sdk-2023.2.3/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-04-12 00:42:08.000000 steam_sdk-2023.2.3/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-05-02 08:49:48.000000 steam_sdk-2023.2.3/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0      388 2022-04-11 18:20:26.000000 steam_sdk-2023.2.3/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-07 20:16:27.000000 steam_sdk-2023.2.3/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-04-11 18:20:26.000000 steam_sdk-2023.2.3/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-06-07 19:34:59.000000 steam_sdk-2023.2.3/steam_sdk/utils/unique.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.918949 steam_sdk-2023.2.3/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    34456 2023-02-23 17:01:52.000000 steam_sdk-2023.2.3/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-06-13 00:34:14.000000 steam_sdk-2023.2.3/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-06-20 13:06:20.000000 steam_sdk-2023.2.3/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.923479 steam_sdk-2023.2.3/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.923479 steam_sdk-2023.2.3/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.923479 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SIGMA/
--rw-rw-rw-   0        0        0     8031 2022-03-29 14:47:53.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SIGMA/WrapperSIGMA.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SIGMA/__init__.py
--rw-rw-rw-   0        0        0      133 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SIGMA/checkJava.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.931502 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SIGMA/jars/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SIGMA/jars/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.931502 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.933519 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0        0 2022-02-23 07:50:41.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-07-05 13:48:59.000000 steam_sdk-2023.2.3/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-02-24 11:28:38.543722 steam_sdk-2023.2.3/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1498 2023-02-24 11:28:38.000000 steam_sdk-2023.2.3/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6423 2023-02-24 11:28:38.000000 steam_sdk-2023.2.3/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-24 11:28:38.000000 steam_sdk-2023.2.3/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1557 2023-02-24 11:28:38.000000 steam_sdk-2023.2.3/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-24 11:28:38.000000 steam_sdk-2023.2.3/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.057289 steam_sdk-2023.4.0/
+-rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam_sdk-2023.4.0/.gitignore
+-rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam_sdk-2023.4.0/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam_sdk-2023.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-04-13 16:02:05.055294 steam_sdk-2023.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam_sdk-2023.4.0/Readme.md
+-rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam_sdk-2023.4.0/mkdocs.yaml
+-rw-rw-rw-   0        0        0     1684 2023-04-13 15:56:12.000000 steam_sdk-2023.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 16:02:05.059284 steam_sdk-2023.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-13 15:54:56.000000 steam_sdk-2023.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.829896 steam_sdk-2023.4.0/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.836882 steam_sdk-2023.4.0/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0    99466 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.837875 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.839870 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.850853 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.852835 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.861812 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.864803 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.870787 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.872782 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.886745 steam_sdk-2023.4.0/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160973 2023-01-17 16:22:36.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    32596 2023-04-13 15:48:40.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    37964 2023-04-13 15:57:32.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/builders/Readme.md
+-rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam_sdk-2023.4.0/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam_sdk-2023.4.0/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.888740 steam_sdk-2023.4.0/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.891732 steam_sdk-2023.4.0/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.895720 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.898712 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
+-rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/Readme.md
+-rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.900714 steam_sdk-2023.4.0/steam_sdk/configs/users/
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/users/Readme.md
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.902701 steam_sdk-2023.4.0/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/cosims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.938606 steam_sdk-2023.4.0/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10029 2023-04-03 16:34:32.000000 steam_sdk-2023.4.0/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     8004 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam_sdk-2023.4.0/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2862 2023-03-30 16:17:31.000000 steam_sdk-2023.4.0/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     3169 2023-01-20 13:20:13.000000 steam_sdk-2023.4.0/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35518 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2609 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam_sdk-2023.4.0/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam_sdk-2023.4.0/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam_sdk-2023.4.0/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/Readme.md
+-rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.953566 steam_sdk-2023.4.0/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     5329 2023-04-13 15:48:42.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.957555 steam_sdk-2023.4.0/steam_sdk/drivers/temp/
+-rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/temp/postLEDET.py
+-rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/temp/runLEDET.py
+-rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/temp/simLEDET.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.994456 steam_sdk-2023.4.0/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10602 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.995453 steam_sdk-2023.4.0/steam_sdk/parsers/templates/
+-rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam_sdk-2023.4.0/steam_sdk/parsers/templates/template_Dakota.in
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.005427 steam_sdk-2023.4.0/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    41232 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    49099 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    59958 2023-04-03 16:34:32.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.013407 steam_sdk-2023.4.0/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-02 17:12:04.000000 steam_sdk-2023.4.0/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0    18478 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/plotters/PlotterSIGMA.py
+-rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.015401 steam_sdk-2023.4.0/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.031358 steam_sdk-2023.4.0/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam_sdk-2023.4.0/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     6745 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.035347 steam_sdk-2023.4.0/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam_sdk-2023.4.0/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.038339 steam_sdk-2023.4.0/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.039349 steam_sdk-2023.4.0/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.048312 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.051304 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.834883 steam_sdk-2023.4.0/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-04-13 16:01:37.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7134 2023-04-13 16:02:03.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 16:01:37.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1595 2023-04-13 16:01:37.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 16:01:37.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam_sdk-2023.2.3/PKG-INFO` & `steam_sdk-2023.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam_sdk
-Version: 2023.2.3
+Version: 2023.4.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,API,SDK
+Keywords: SDK,CERN,API,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
 
@@ -24,14 +24,17 @@
 Important: Before running the tests, make sure to set up your user settings.
 
 * The settings file must be located in the subfolder steam_sdk\tests
 * The file must be called settings.username.yaml, where username is your user name in the machine on which you are running the analysis.
 It is recommended to start by making a copy of the example settings.SYSTEM.yaml file.
 * Note: It is not recommended to change other settings files within this project (some files are generated by the software).
 
+# Documentation
+https://steam-sdk.docs.cern.ch/
+
 # Installation
 
 ## Released version:
 pip install steam-sdk
 
 ## Test version:
 pip install -i https://test.pypi.org/simple/ steam-sdk
```

### Comparing `steam_sdk-2023.2.3/setup.py` & `steam_sdk-2023.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam_sdk',
-    version="2023.2.3",
+    version="2023.4.0",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/AnalysisSTEAM.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import csv
 import sys
 import ntpath
 import os
+import pathlib
 import shutil
 import importlib
 import importlib.util
 import pandas as pd
 import pickle
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
 from ast import literal_eval
 
 from steam_sdk.data.DataSettings import DataSettings
 from steam_sdk.builders.BuilderModel import BuilderModel
-from steam_sdk.data.DataAnalysis import DataAnalysis, ModifyModel, ModifyModelMultipleVariables, ParametricSweep
+from steam_sdk.data.DataAnalysis import DataAnalysis, ModifyModel, ModifyModelMultipleVariables, ParametricSweep, LoadCircuitParameters, WriteStimulusFile
 from steam_sdk.drivers.DriverFiQuS import DriverFiQuS
 from steam_sdk.drivers.DriverLEDET import DriverLEDET
 from steam_sdk.drivers.DriverPSPICE import DriverPSPICE
 from steam_sdk.drivers.DriverPyBBQ import DriverPyBBQ
+from steam_sdk.drivers.DriverSIGMA import DriverSIGMA
 from steam_sdk.drivers.DriverXYCE import DriverXYCE
 from steam_sdk.parsers.ParserYAML import dict_to_yaml, yaml_to_data
 from steam_sdk.parsims.ParsimConductor import ParsimConductor
+from steam_sdk.parsims.ParsimEventCircuit import ParsimEventCircuit
 from steam_sdk.parsims.ParsimEventMagnet import ParsimEventMagnet
 from steam_sdk.parsims.ParsimSweep import ParsimSweep
 from steam_sdk.postprocs.PostprocsMetrics import PostprocsMetrics
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.rgetattr import rgetattr
 from steam_sdk.utils.sgetattr import rsetattr
 from steam_sdk.utils.rhasattr import rhasattr
 from steam_sdk.viewers.Viewer import Viewer
-from steam_sdk.parsers.ParserPSPICE import writeStimuliFromInterpolation, writeStimuliFromInterpolation_general
+from steam_sdk.parsers.ParserPSPICE import writeStimuliFromInterpolation
 
 
 class AnalysisSTEAM:
     """
         Class to run analysis based on STEAM_SDK
     """
 
@@ -63,24 +66,25 @@
 
         self.list_sims = []  # this list will be populated with integers indicating simulations to run
         self.list_viewers = {}  # this dictionary will be populated with Viewer objects and their names
         self.list_metrics = {}  # this dictionary will be populated with calculated metrics
         self.verbose = verbose
         self.summary = None  # float representing the overall outcome of a simulation for parsims
 
-        if file_name_analysis:
+        if isinstance(file_name_analysis, str) or isinstance(file_name_analysis, pathlib.PurePath):
             self.data_analysis = yaml_to_data(file_name_analysis, DataAnalysis)  # Load yaml keys into DataAnalysis dataclass
             # Read working folders and set them up
             self._set_up_working_folders()
             # Read analysis settings
             self._load_and_write_settings(relative_path_settings)
-        else:
+        elif file_name_analysis is None:
             self.data_analysis = DataAnalysis()
             if verbose: print('Empty AnalysisSTEAM() object generated.')
 
+
     def setAttribute(self, dataclassSTEAM, attribute: str, value):
         try:
             setattr(dataclassSTEAM, attribute, value)
         except:
             setattr(getattr(self, dataclassSTEAM), attribute, value)
 
     def getAttribute(self, dataclassSTEAM, attribute):
@@ -100,36 +104,40 @@
         """
 
         # Raise exceptions if folders are not defined.
         if self.data_analysis.WorkingFolders.library_path == 'gitlab':
             import steam_models
             steam_models_path = steam_models.__path__[0]
             self.data_analysis.WorkingFolders.library_path = steam_models_path
+        elif self.data_analysis.WorkingFolders.library_path in ['same_as_analysis_yaml']:
+            self.data_analysis.WorkingFolders.library_path = '.' + os.sep + self.data_analysis.GeneralParameters.model.name + os.sep + 'input'
         if not self.data_analysis.WorkingFolders.library_path:
             raise Exception('Model library path must be defined. Key to provide: WorkingFolders.library_path')
         if not self.data_analysis.WorkingFolders.output_path:
             raise Exception('Output folder path must be defined. Key to provide: WorkingFolders.output_path')
         if not self.data_analysis.WorkingFolders.temp_path:
             raise Exception('Temporary folder path must be defined. Key to provide: WorkingFolders.temp_path')
 
         # Resolve all paths and re-assign them to the self variables
-
-        self.library_path = Path(self.data_analysis.WorkingFolders.library_path).resolve()
+        if self.data_analysis.WorkingFolders.library_path == 'same_as_analysis_yaml_use_model_name':
+            self.library_path = 'same_as_analysis_yaml_use_model_name'
+        else:
+            self.library_path = Path(self.data_analysis.WorkingFolders.library_path).resolve()
         self.output_path = Path(self.data_analysis.WorkingFolders.output_path).resolve()
         self.temp_path = Path(self.data_analysis.WorkingFolders.temp_path).resolve()
 
         if self.verbose:
             print('Model library path:    {}'.format(self.library_path))
             print('Output folder path:    {}'.format(self.output_path))
             print('Temporary folder path: {}'.format(self.temp_path))
 
         # Check if model library folder is present. If not, raise an exception.
-        if not os.path.isdir(self.library_path):
-            raise Exception(
-                f'Model library path refers to a not-existing folder: {self.library_path}. Key to change: WorkingFolders.library_path')
+        if self.library_path != 'same_as_analysis_yaml_use_model_name':
+            if not os.path.isdir(self.library_path):
+                raise Exception(f'Model library path refers to a not-existing folder: {self.library_path}. Key to change: WorkingFolders.library_path')
 
         # Check if output folder is present. If not, make it.
         make_folder_if_not_existing(self.output_path, verbose=self.verbose)
 
         # Check if temporary folder is present. If so, delete it.
         if os.path.isdir(self.temp_path):
             shutil.rmtree(self.temp_path)
@@ -237,32 +245,32 @@
         # Run analysis (and re-print analysis steps)
         if verbose: print('Analysis started.')
         for s, seq_step in enumerate(self.data_analysis.AnalysisStepSequence):
             if verbose: print('Step {}/{}: {}'.format(s + 1, len(self.data_analysis.AnalysisStepSequence), seq_step))
             step = step_definitions[seq_step]  # this is the object containing the information about the current step
             if step.type == 'MakeModel':
                 self.step_make_model(step, verbose=verbose)
-            elif step.type == 'ModifyModel':
+            elif step.type == 'ModifyModel': #
                 self.step_modify_model(step, verbose=verbose)
-            elif step.type == 'ModifyModelMultipleVariables':
+            elif step.type == 'ModifyModelMultipleVariables':  #
                 self.step_modify_model_multiple_variables(step, verbose=verbose)
             elif step.type == 'RunSimulation':
                 self.step_run_simulation(step, verbose=verbose)
             elif step.type == 'PostProcess':
                 self.step_postprocess(step, verbose=verbose)
             elif step.type == 'SetUpFolder':
                 self.step_setup_folder(step, verbose=verbose)
             elif step.type == 'AddAuxiliaryFile':
                 self.add_auxiliary_file(step, verbose=verbose)
             elif step.type == 'CopyFile':
                 self.copy_file_to_target(step, verbose=verbose)
             elif step.type == 'RunCustomPyFunction':
                 self.run_custom_py_function(step, verbose=verbose)
             elif step.type == 'RunViewer':
-                self.run_viewer(step, verbose=verbose)
+                self.run_viewer(step, verbose=verbose) # Add elif plot_map2d,  two paths save plot to folder png
             elif step.type == 'CalculateMetrics':
                 self.calculate_metrics(step, verbose=verbose)
             elif step.type == 'LoadCircuitParameters':
                 self.load_circuit_parameters(step, verbose=verbose)
             elif step.type == 'WriteStimulusFile':
                 self.write_stimuli_from_interpolation(step, verbose=verbose)
             elif step.type == 'ParsimEvent':
@@ -279,16 +287,20 @@
             print('Making model object named {}'.format(str(step.model_name)))
         ## Assuming the steam-models directory structure if 'steam-models' or model_library found at the end of library path.
         # Else assuming library path directs straight to the model
         if (str(self.library_path).endswith('steam_models')) or (str(self.library_path).endswith('steam-models')) or (
                 str(self.library_path).endswith('model_library')):
             file_model_data = os.path.join(self.library_path, step.case_model + 's', step.file_model_data, 'input',
                                            'modelData_' + step.file_model_data + '.yaml')
-        else:
-            file_model_data = os.path.join(self.library_path, 'modelData_' + step.file_model_data + '.yaml')
+        elif isinstance(self.library_path, str):
+            if self.library_path == 'same_as_analysis_yaml_use_model_name':
+                file_model_data = '.' + os.sep + step.file_model_data + os.sep + 'input' + os.sep + 'modelData_' + step.file_model_data + '.yaml'
+                file_model_data = Path(file_model_data).resolve()
+            else:
+                file_model_data = os.path.join(self.library_path, 'modelData_' + step.file_model_data + '.yaml')
 
         case_model = step.case_model
         software = step.software  # remember this is a list, not a string
         verbose_of_step = step.verbose
         flag_build = step.flag_build
         flag_dump_all = step.flag_dump_all
         flag_plot_all = step.flag_plot_all
@@ -405,24 +417,30 @@
                                              'Options_FiQuS.') else None)
                 if 'LEDET' in step.software:
                     flag_json = BM.flag_json
                     flag_yaml = True  # Hard-coded for the moment
                     BM.buildLEDET()
                     self.setup_sim_LEDET(simulation_name=step.simulation_name, sim_number=simulation_number,
                                          flag_yaml=flag_yaml, flag_json=flag_json)
+                if 'SIGMA' in step.software:
+                    for sim_num in step.simulation_numbers:
+                        make_folder_if_not_existing(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}") )#ADDED
+                        BM.buildSIGMA(output_path=os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}"))
+                    #self.setup_sim_SIGMA(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PyBBQ' in step.software:
                     BM.buildPyBBQ()
                     self.setup_sim_PyBBQ(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PSPICE' in step.software:
                     BM.buildPSPICE()
                     self.setup_sim_PSPICE(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'XYCE' in step.software:
                     BM.buildXYCE()
                     self.setup_sim_XYCE(simulation_name=step.simulation_name, sim_number=simulation_number)
 
+
     def get_attribute_model(self, case_model: str, builder_model: BuilderModel, name_variable: str,
                             idx_conductor: int = None):
         """
         Helper function used to get an attribute from a key of the model data.
         Depending on the model type (circuit, magnet, conductor), the data structure to access is different.
         Also, there is a special case when the variable to read is a sub-key of the Conductors key. In such a case, an additional parameter idx_conductor must be defined (see below).
         :param case_model: Model type
@@ -510,19 +528,25 @@
         if verbose:
             print('All variables of step {} were changed.'.format(step))
 
     def step_run_simulation(self, step, verbose: bool = False):
         software = step.software
         simulation_name = step.simulation_name
         simFileType = step.simFileType
-        for sim_number in step.simulation_numbers:
+        sim_numbers = step.simulation_numbers
+        if simulation_name == 'from_last_parametric_list':
+            sim_numbers = list(self.input_parsim_sweep_df.simulation_number.to_numpy())
+            sim_names = list(self.input_parsim_sweep_df.simulation_name.to_numpy())
+        else:
+            sim_names = [simulation_name] * len(sim_numbers)
+        for sim_name, sim_number in zip(sim_names, sim_numbers):
             if verbose:
                 print('Running simulation of model {} #{} using {}.'.format(simulation_name, sim_number, software))
             # Run simulation
-            self.run_sim(software, simulation_name, sim_number, simFileType, verbose)
+            self.run_sim(software, sim_name, sim_number, simFileType, verbose)
 
     def step_postprocess(self, step, verbose: bool = False):
         if verbose: print('postprocessing')
         print('Not implemented yet.')
         pass
 
     def step_setup_folder(self, step, verbose: bool = False):
@@ -601,14 +625,21 @@
                                   (simulation_name in entry) and ('.stl' in entry)]
                 for stl_file in list_stl_files:
                     file_to_copy = os.path.join(self.output_path, stl_file)
                     file_copied = os.path.join(local_model_folder, stl_file)
                     shutil.copyfile(file_to_copy, file_copied)
                     if verbose: print('Stl file {} copied to {}.'.format(file_to_copy, file_copied))
 
+            elif 'SIGMA' in software:
+                # make top level output folder
+               # make_folder_if_not_existing(self.settings.local_SIGMA_folder, verbose=verbose)
+
+                # make simulation name folder inside top level folder
+                make_folder_if_not_existing(os.path.join(self.settings.local_SIGMA_folder, step.simulation_name))
+
             elif 'XYCE' in software:
                 local_XYCE_folder = Path(self.settings.local_XYCE_folder)
                 local_model_folder = str(Path(local_XYCE_folder / simulation_name).resolve())
                 # Make circuit input folder
                 make_folder_if_not_existing(local_model_folder, verbose=verbose)
 
                 # Copy lib files from the output folder
@@ -725,14 +756,15 @@
 
     def run_viewer(self, step, verbose: bool = False):
         """
             Make a steam_sdk.viewers.Viewer.Viewer() object and run its analysis
         """
 
         # Unpack variables
+        # Unpack variables
         viewer_name = step.viewer_name
 
         if verbose: print(f'Making Viewer object named {viewer_name}.')
 
         # Make a steam_sdk.viewers.Viewer.Viewer() object and run its analysis
         V = Viewer(file_name_transients=step.file_name_transients,
                    list_events=step.list_events,
@@ -964,14 +996,42 @@
 
             shutil.copyfile(file_name_temp, file_name_local)
             if self.verbose: print('Simulation file {} copied.'.format(file_name_local))
 
             # os.remove(file_name_temp)
             # print('Temporary file {} deleted.'.format(file_name_temp))
 
+    def setup_sim_SIGMA(self, simulation_name, sim_number, magnet_type=None):
+        """
+        Set up a SIGMA simulation by copying the last file generated by BuilderModel to the output folder and to the
+        local SIGMA working folder.
+        The original file is then deleted.
+        """
+
+        # Add simulation number to the list
+        self.list_sims.append(sim_number)
+
+        # Make simulation folder
+        local_model_folder = os.path.join(self.settings.local_SIGMA_folder, f'{simulation_name}_{str(sim_number)}')
+        make_folder_if_not_existing(local_model_folder)
+
+        # Copy all simulation file
+        files = os.listdir(self.output_path)
+
+        # iterating over all the files in
+        # the source directory
+        for fname in files:
+            file_name_temp = os.path.join(self.output_path, fname)
+            file_name_local = os.path.join(local_model_folder, fname)
+            shutil.copyfile(file_name_temp, file_name_local)
+
+
+        if self.verbose: print('Simulation files {} generated.'.format(file_name_temp))
+        if self.verbose: print('Simulation files {} copied.'.format(file_name_local))
+
     def setup_sim_PSPICE(self, simulation_name, sim_number):
         """
         Set up a PSPICE simulation by copying the last file generated by BuilderModel to the output folder and to the
         local PSPICE working folder.
         The simulation netlist and auxiliary files are copied in a new numbered subfoldered.
         The original file is then deleted.
         """
@@ -1192,14 +1252,20 @@
                                    verbose=verbose)
             dPSPICE.run_PSPICE(simulation_name, suffix='')
         elif software == 'XYCE':
             local_model_folder = Path(
                 Path(self.settings.local_XYCE_folder) / simulation_name / str(sim_number)).resolve()
             dXYCE = DriverXYCE(path_exe=self.settings.XYCE_path, path_folder_XYCE=local_model_folder, verbose=verbose)
             dXYCE.run_XYCE(simulation_name, suffix='')
+        elif software == 'SIGMA':
+            simulation_name_temp = simulation_name + f"_{str(sim_number)}"
+            local_model_folder = Path(
+                Path(self.settings.local_SIGMA_folder) / simulation_name_temp).resolve()
+            ds = DriverSIGMA(simulation_name, path_folder_SIGMA=local_model_folder)
+            ds.run_SIGMA()
         else:
             raise Exception(f'Software {software} not supported for automated running.')
 
 
     def write_stimuli_from_interpolation(self, step, verbose: bool = False):
         '''
         Function to write a resistance stimuli for n apertures of a magnet for any current level. Resistance will be interpolated
@@ -1235,15 +1301,15 @@
             InterpolationType = 'Linear'
         if not type_stl:
             type_stl = 'w'
         if not sparseTimeStepping:
             sparseTimeStepping = 1  # Note: This will ovrewrite the default value of 100 used in the writeStimuliFromInterpolation_general() function
 
         # Call coil-resistance interpolation function
-        writeStimuliFromInterpolation_general(current_level, n_total_magnets, n_apertures, magnets, tShift, Outputfile,
+        writeStimuliFromInterpolation(current_level, n_total_magnets, n_apertures, magnets, tShift, Outputfile,
                                               path_resources, InterpolationType, type_stl, sparseTimeStepping,
                                               magnet_type)
 
         if verbose:
             print(f'Output stimulus file {Outputfile} written.')
 
     def run_parsim_event(self, step, verbose: bool = False):
@@ -1302,79 +1368,130 @@
             # TODO: add flag to write yaml analysis with all steps
             # TODO: parse Conductor Data - but what are the names in Quenchdict? (Parsim Sweep can handly conductor changes)
 
             # Write a .csv file that can be used to run a STEAM Viewer analysis
             for current_software, current_path_viewer_csv in zip(software, path_output_viewer_csv):
                 pem.set_up_viewer(current_path_viewer_csv, default_keys, simulation_numbers, simulation_name, current_software)
                 if verbose: print(f'File {current_path_viewer_csv} written. It can be used to run a STEAM Viewer analysis.')
+        elif case_model == 'circuit':
+            pec = ParsimEventCircuit(ref_model=self.list_models[model_name], verbose=verbose)
+            pec.read_from_input(path_input_file=input_file, flag_append=False)
+            pec.write_event_file(simulation_name=simulation_name, simulation_numbers=simulation_numbers,
+                                 path_outputfile_event_csv=path_output_event_csv)
+            for event_number in range(len(pec.list_events)):
+                circuit_name = pec.list_events[event_number].GeneralParameters.name
+                circuit_family_name = self.__get_circuit_family_name(circuit_name)
+                magnet_name = self.__get_magnet_name(circuit_name)
+                circuit_type = self.__get_circuit_type(circuit_name)
+                number_of_magnets = self.__get_number_of_magnets(circuit_name)
+                number_of_apertures = self.__get_number_of_apertures(circuit_name)
+                current_level = pec.list_events[event_number].PoweredCircuits[circuit_name].current_at_discharge
+                magnets_list = self.__get_magnets_list(number_of_magnets)
+                t_PC_off = pec.list_events[event_number].PoweredCircuits[circuit_name].delta_t_FGC_PIC
+                magnet_types = self.__get_magnet_types_list(number_of_magnets)
+                load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.abspath(f"../../../steam_models/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
+                if circuit_family_name == "IPD":
+                    stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_family_name}', f'{event_number + 1}', 'coil_resistances.stl')
+                else:
+                    stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', f'{event_number + 1}', 'coil_resistances.stl')
+                write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.abspath(f'../../../steam_models/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                # start parsim sweep step with newly created event file
+                parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv,
+                                                    model_name=model_name, case_model=case_model, software=software, verbose=verbose)
+                self.load_circuit_parameters(load_circuit_parameters_step, verbose=verbose)
+                self.write_stimuli_from_interpolation(write_stimuli_file_step, verbose=verbose)
+                self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
+
+            # Write a .csv file that can be used to run a STEAM Viewer analysis #TODO consider adding set_up_viewer() method
+            # for current_software, current_path_viewer_csv in zip(software, path_output_viewer_csv):
+            #     pec.set_up_viewer(current_path_viewer_csv, default_keys, simulation_numbers, simulation_name, current_software)
+            #     if verbose: print(f'File {current_path_viewer_csv} written. It can be used to run a STEAM Viewer analysis.')
         else:
             raise Exception(f'case_model {case_model} not supported by ParsimEvent.')
 
         if verbose:
             print(f'ParsimEvent called using input file {input_file}.')
 
     def run_parsim_conductor(self, step, verbose):
+        '''
+        Function to generate steps to change the conductor data of a magnet using a csv database
+
+        :param step:
+        :param verbose: if true displays more information
+        '''
         # Unpack inputs
         model_name = step.model_name
         case_model = step.case_model
         software = step.software
         groups_to_coils = step.groups_to_coils
         simulation_number = step.simulation_number
         input_file = step.input_file
         path_output_sweeper_csv = step.path_output_sweeper_csv
+        strand_critical_current_measurements = step.strand_critical_current_measurements
 
-        # check paths and make them paths global
+        # check inputs
         if not path_output_sweeper_csv:
             raise Exception('File path path_output_event_csv must be defined for an analysis step of type ParsimEvent.')
         if not input_file:
             raise Exception('File path path_output_event_csv must be defined for an analysis step of type ParsimEvent.')
 
+
+        # make a copy of the respective conductor for every coil and store it in the magnet model
+        # NOTE: if a coil consists of 2 different conductors the user has to treat them as 2 different coils (so a coil is not always a coil but rather a subcoil with the same conductor)
+        new_conductors = [None] * len(groups_to_coils)
+        dict_coilname_to_conductorindex = {}
+        new_conductor_to_group = [None] * len(self.list_models[model_name].model_data.CoilWindings.conductor_to_group)
+        for idx, (coil_name, group_numbers) in enumerate(groups_to_coils.items()):
+            # store the conductor indices of the groups that make up this coil
+            conductor_indices = [self.list_models[model_name].model_data.CoilWindings.conductor_to_group[i-1] for i in group_numbers]
+
+            # check if all the groups in the coil have the same conductor
+            if len(set(conductor_indices)) != 1:
+                raise Exception(f'Not every group in the coil {coil_name} has the same conductor. \n'
+                                f'If a coil consists of more then one conductor it has to be treated like 2 separate coils.')
+            else:
+                # make a copy of the Conductor for this coil and overwrite the name
+                # since all the entries in conductor_indices are the same, conductor_indices[0] can be used
+                new_conductors[idx] = deepcopy(self.list_models[model_name].model_data.Conductors[conductor_indices[0]-1])
+                new_conductors[idx].name = f'conductor_{coil_name}'
+
+            # store what coilname belongs to what conductor index to later check in database
+            dict_coilname_to_conductorindex[coil_name] = idx
+
+            # change the entries in conductor_to_group with the new Conductor
+            for group_number in group_numbers:
+                new_conductor_to_group[group_number-1] = idx+1
+
+        # check if all the values could be written
+        if None in new_conductors or None in new_conductor_to_group:
+            raise Exception(f'The given groups_to_coils did not contain all the group indices (1-{len(new_conductor_to_group)})!')
+
+        # overwrite the information in the DataModelMagnet instance of the BuilderModel
+        self.list_models[model_name].model_data.Conductors = new_conductors
+        self.list_models[model_name].model_data.CoilWindings.conductor_to_group = new_conductor_to_group
+        # NOTE: so far no parameters of the model_data were altered, just copies of the conductor have been made and connected to the specified groups
+        del new_conductors, new_conductor_to_group
+
+
         if case_model == 'magnet':
-            pc = ParsimConductor(verbose=verbose)
-            magnet_name = self.list_models[model_name].model_data.GeneralParameters.magnet_name
-            pc.read_from_input(path_input_file=input_file, groups_to_coils=groups_to_coils, magnet_name=magnet_name)
+            # create instance of ParsimConductor
+            pc = ParsimConductor(verbose=verbose, model_data_conductors=self.list_models[model_name].model_data.Conductors)
+            # read the conductor database
+            pc.read_from_input(path_input_file=input_file, magnet_name=self.list_models[model_name].model_data.GeneralParameters.magnet_name,
+                               strand_critical_current_measurements=strand_critical_current_measurements)
+            # write a sweeper csv file
             pc.write_conductor_parameter_file(path_output_file=path_output_sweeper_csv, simulation_name=model_name,
-                                              simulation_number=simulation_number)
+                                              simulation_number=simulation_number, dict_coilname_to_conductorindex=dict_coilname_to_conductorindex)
 
-            # start parsim sweep step with newly created event file
-            parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_sweeper_csv,
+            # create parsim sweep step with newly created sweeper csv file and run it
+            parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_sweeper_csv, # TODO rename teh class to ParametricSweepStep? ParsimConductor is no step class and ParametricSweep is
                                                 model_name=model_name, case_model=case_model, software=software, verbose=verbose)
             self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
         else:
-            raise Exception(f'case_model {case_model} not supported by ParsimConductor.')
-
-    def run_parsim_sweep_OLD(self, step, verbose: bool = False):
-        '''
-        Function to generate steps based on list of events from external file
-
-        :param step:
-        :param verbose: if true displays more information
-        :return:
-        '''
-        input_sweep_file = step.input_sweep_file
-        model_name = step.model_name
-        case_model = step.case_model
-        verbose = step.verbose
-
-        # path to ideal Quench dict
-        input_sweep_file_abs = os.path.join(os.getcwd(), input_sweep_file)
-        # Read input file and run the ParsimEvent analysis
-        if case_model == 'magnet':
-            ps = ParsimSweep(ref_model=self.list_models[model_name], verbose=verbose)
-            ps.read_from_input(file_path=input_sweep_file_abs, flag_append=False)
-            # ps.set_up_analysis(...)
-            for step_name in ps.list_AnalysisStepSequence:
-                step = ps.dict_AnalysisStepDefinition[step_name]
-                self.step_modify_model_multiple_variables(step, verbose=verbose)
-        else:
-            raise Exception(f'case_model {case_model} not supported by parsim events')
-
-        if verbose:
-            print(f'Parsim Event called using input file {input_sweep_file}.')
-
+            raise Exception(f'Case_model "{case_model}" not supported by ParsimConductor.')
 
     def run_parsim_sweep(self, step, verbose: bool = False):
         '''
         Function to generate steps based on list of models read from external file
         :param step:
         :param verbose: if true displays more information
         :return:
@@ -1383,37 +1500,38 @@
         input_sweep_file = step.input_sweep_file
         default_model_name = step.model_name
         case_model = step.case_model
         software = step.software
         verbose = step.verbose
 
         # read input sweeper file
-        input_parsim_sweep_df = pd.read_csv(input_sweep_file)
+        self.input_parsim_sweep_df = pd.read_csv(input_sweep_file)
 
         # loop through every row and run ModifyMultipleVariables step for every row (=event)
-        for i, row in input_parsim_sweep_df.iterrows():
+        for i, row in self.input_parsim_sweep_df.iterrows():
             # check if model_name is provided in sweeper. csv file - if not use the default one
             if 'simulation_name' in row and row['simulation_name'] in self.list_models:
                 # use sweeper model_name only if model_name is existing in list_models
                 model_name = row['simulation_name']
-                if verbose: print(f'row {i + 1}: Using magnet {model_name} as specified in the input file {input_sweep_file}.')
+                if verbose: print(f'row {i + 1}: Using model {model_name} as specified in the input file {input_sweep_file}.')
             else:
                 model_name = default_model_name
-                if verbose: print(f'row {i + 1}: Using default magnet {default_model_name} as magnet model.')
+                if verbose: print(f'row {i + 1}: Using default model {default_model_name} as initial model.')
 
             # check if simulation number is provided and extract it from file
             try:
                 # number has to be present & has to be an int (or be parsable into one) for the rest of the code to work
                 simulation_number = int(row['simulation_number'])
             except:
                 raise Exception(f'ERROR: no simulation_number provided in csv file {input_sweep_file}.')
             if verbose: print(f'changing these fields row # {i + 1}: {row}')
 
             # save the earliest starting time of Quench Heaters to definitely start the simulation beforehand
-            new_start_time = self.__get_earliest_QH_starting_time(row)
+            if case_model == 'magnet':
+                new_start_time = self.__get_earliest_QH_starting_time(row)
 
             # set simulation start time 50 ms before the start time of the first Quench Heater
             dict_variables_to_change = dict()
             if case_model == 'magnet' and 'LEDET' in software:
                 time_vec = rgetattr(self.list_models[model_name].model_data,'Options_LEDET.time_vector.time_vector_params')
                 if new_start_time: time_vec[0] = new_start_time
                 dict_variables_to_change['Options_LEDET.time_vector.time_vector_params'] = time_vec
@@ -1427,42 +1545,60 @@
                 next_simulation_name = model_data.GeneralParameters.circuit_name
             elif case_model == 'conductor':
                 model_data = self.list_models[model_name].conductor_data
                 next_simulation_name = model_data.GeneralParameters.conductor_name
             else:
                 raise Exception(f'case_model {case_model} not supported by ParsimSweep.')
 
+            # Initialize this variable, which is only used in the special case where circuit parameters are set to be changed (key "GlobalParameters.global_parameters")
+            dict_circuit_param_to_change = {}
+
             # Iterate through the keys and values in the data dictionary & store all variables to change
             for j, (var_name, var_value) in enumerate(row.items()):
                 # if value is null, skip this row
                 if not pd.notnull(var_value): continue
 
-                # handle the change of a variable in the conductor list
+                # Handle the change of a variable in the conductor list
                 if 'Conductors[' in var_name:
                     # to check if var_name is valid (meaning it is the name of a variable in model_data)
                     try:
                         # try if eval is able to find the variable in model_data - if not: an Exception will be raised
                         eval('model_data.' + var_name)
                         dict_variables_to_change[var_name] = var_value
                     except:
-                        print(f'WARNING: Column name "{var_name}" with value "{var_value}" in csv file {input_sweep_file} is skipped.')
+                        print(f'WARNING: Sweeper skipped Column name "{var_name}" with value "{var_value}" in csv file {input_sweep_file}')
+
+                # Handle the change of the special-case key GlobalParameters.global_parameters (dictionary of circuit global parameters)
+                elif case_model == 'circuit' and var_name.startswith('GlobalParameters.global_parameters'):
+                    # dict_global_parameters = deepcopy(model_data.GlobalParameters.global_parameters)  # original dictionary of circuit global parameters
+                    circuit_param_to_change = var_name.split('GlobalParameters.global_parameters.')[-1]
+                    # dict_global_parameters[circuit_param_to_change] = var_value
+                    # dict_variables_to_change['GlobalParameters.global_parameters'] = dict_global_parameters
+                    dict_circuit_param_to_change[circuit_param_to_change] = var_value
 
                 # Check if the current variable is present in the model data structure & value in csv is not empty
                 elif rhasattr(model_data, var_name):
                     # save valid new variable names and values to change them later
                     if type(var_value) == int or type(var_value) == float:
                         dict_variables_to_change[var_name] = var_value
                     elif type(var_value) == str:
                         dict_variables_to_change[var_name] = self.__parse_string(var_value)
                     else:
                         raise Exception(f'ERROR: Datatype of Element in Column "{var_value}" Row "{j + 2}" of csv file {input_sweep_file} is invalid.')
 
                 # print when columns have been skipped
                 elif not rhasattr(model_data, var_name) and var_name != 'simulation_number':
-                    print(f'WARNING: Columnname "{var_name}" with value "{var_value}" in csv file {input_sweep_file} is skipped.')
+                    print(f'WARNING: Column name "{var_name}" with value "{var_value}" in csv file {input_sweep_file} is skipped.')
+            
+            # Special case: If circuit parameters were set to change, add the key "GlobalParameters.global_parameters" to the dictionary of variables to change
+            if len(dict_circuit_param_to_change) > 0:
+                dict_global_parameters = deepcopy(model_data.GlobalParameters.global_parameters)  # original dictionary of circuit global parameters
+                for key, value in dict_circuit_param_to_change.items():
+                    dict_global_parameters[key] = value
+                dict_variables_to_change['GlobalParameters.global_parameters'] = dict_global_parameters
 
             # if no variable to change is found, the simulation should run none the less, so dict_variables_to_change has to have an entry
             if not dict_variables_to_change:
                 if case_model == 'magnet':
                     dict_variables_to_change['GeneralParameters.magnet_name'] = rgetattr(model_data, 'GeneralParameters.magnet_name')
                 elif case_model == 'circuit':
                     dict_variables_to_change['GeneralParameters.circuit_name'] = rgetattr(model_data, 'GeneralParameters.circuit_name')
@@ -1485,93 +1621,14 @@
             next_step.software = software
             self.step_modify_model_multiple_variables(next_step, verbose=verbose)
 
             # reset changes to the model in self
             self.list_models[model_name] = deepcopy(local_model_copy)
         del local_model_copy
 
-        # # Open the CSV file
-        # with open(input_sweep_file, 'r') as csv_file:
-        #     # Generate a CSV reader
-        #     reader = csv.DictReader(csv_file)
-        #     # Iterate through the rows (parametric simulations to set up)
-        #     for i, row in enumerate(reader):
-        #         simulation_number = row['simulation_number']
-        #         simulation_name = row['simulation_name']
-        #         if verbose: print(f'changing these fields row # {i+1}: {row}')
-        #
-        #         if case_model == 'magnet':
-        #             model_data = self.list_models[model_name].model_data
-        #         else:
-        #             raise Exception(f'case_model {case_model} not supported by ParsimSweep.')
-        #
-        #         # Iterate through the keys and values in the data dictionary
-        #         for var_name, var_value in row.items():
-        #             # Check if the current variable is present in the model data structure
-        #             if rhasattr(model_data, var_name):
-        #                 # For each variable to change, make an instance of an ModifyModel step and call the step_modify_model() method
-        #                 next_step                    = ModifyModel(type='ModifyModel')
-        #                 next_step.model_name         = model_name
-        #                 next_step.variable_to_change = var_name
-        #                 next_step.variable_value     = [var_value]
-        #                 next_step.simulation_numbers = [simulation_number]
-        #                 next_step.simulation_name    = simulation_name
-        #                 next_step.software           = software
-        #                 self.step_modify_model(next_step, verbose=verbose)
-
-        #
-        #
-        #
-        #
-        #             # Set the class variable using the key and value
-        #             try:
-        #                 rsetattr(new_BM, key, value)
-        #             except:
-        #                 try:
-        #                     rsetattr(new_BM.model_data, key, value)
-        #                 except:
-        #                     print(f'Skipped column {key} - no corresponding entry in BuilderModel found.')
-        #         # Append the row as a dictionary to the list
-        #         self.dict_BuilderModels[self.simulation_numbers[i]] = new_BM
-        # if verbose:
-        #     print('csv file read.')
-        #
-        # # Read input file and run the ParsimEvent analysis
-        # if case_model == 'magnet':
-        #
-        #     # Loop through the list of variables to change
-        #     for v, variable_to_change in enumerate(step.variables_to_change):
-        #         # For each variable to change, make an instance of an ModifyModel step and call the step_modify_model() method
-        #         next_step = ModifyModel(type='ModifyModel')
-        #         next_step.model_name = step.model_name
-        #         next_step.variable_to_change = variable_to_change
-        #         next_step.variable_value = step.variables_value[v]
-        #         if v + 1 == len_variables_to_change:  # If this is the last variable to change, import new_model_name and simulation_numbers from the step
-        #             next_step.new_model_name = step.new_model_name
-        #             next_step.simulation_numbers = step.simulation_numbers
-        #         else:  # else, set new_model_name and simulation_numbers to empty lists to avoid making models/simulations for intermediate changes
-        #             next_step.new_model_name = []
-        #             next_step.simulation_numbers = []
-        #         next_step.simulation_name = step.simulation_name
-        #         next_step.software = step.software
-        #         self.step_modify_model(next_step, verbose=verbose)
-        #     if verbose:
-        #         print('All variables of step {} were changed.'.format(step))
-        #
-        #
-        #
-        #     ps = ParsimSweep(ref_model=self.list_models[model_name], verbose=verbose)
-        #     ps.read_from_input(file_path=input_sweep_file, flag_append=False)
-        #     # ps.set_up_analysis(...)
-        #     for step_name in pem.list_AnalysisStepSequence:
-        #         step = pem.dict_AnalysisStepDefinition[step_name]
-        #         self.step_modify_model_multiple_variables(step, verbose=verbose)
-        # else:
-        #     raise Exception(f'case_model {case_model} not supported by ParsimSweep.')
-
         if verbose:
             print(f'Parsim Event called using input file {input_sweep_file}.')
 
     def __get_earliest_QH_starting_time(self, row: pd.Series, t_before_QH_start: float = 0.05, t_earliest_starting_time: float = -10):
         if 'Quench_Protection.Quench_Heaters.t_trigger' in row:
             min_value = (min(self.__parse_string(row['Quench_Protection.Quench_Heaters.t_trigger'])))
             # start simulation t_before_QH_start seconds before the first Quench Heater starts
@@ -1601,7 +1658,53 @@
                 except ValueError:
                     # If that also fails, return the original string
                     raise Exception(
                         f'The entry ({s}) in the csv file cant be read. Vector with different datatypes used.')
         else:
             # if no list: use normal string
             return s
+
+    def __get_circuit_family_name(self, circuit_name: str):
+        if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
+            return "60A"
+        elif circuit_name.startswith("RD"):
+            return "IPD"
+
+    def __get_magnet_name(self, circuit_name: str):
+        if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
+            return "MCBH"
+        elif circuit_name.startswith("RD"):
+            circuit_type = self.__get_circuit_type(circuit_name)
+            magnet_dict = {"RD1": "MBX", "RD2": "MBRC", "RD3": "MBRS", "RD4": "MBRB"}
+            return magnet_dict.get(circuit_type, "")
+
+    def __get_number_of_magnets(self, circuit_name: str):
+        circuit_family_name = self.__get_circuit_family_name(circuit_name)
+        if circuit_family_name in ["60A", "IPD"]:
+            return 1
+
+    def __get_number_of_apertures(self, circuit_name: str):
+        circuit_family_name = self.__get_circuit_family_name(circuit_name)
+        if circuit_family_name == "IPQ":
+            return 2
+        else:
+            return 1
+
+    def __get_magnets_list(self, number_of_magnets: int):
+        list = []
+        for i in range(1, number_of_magnets+1):
+            list.append(i)
+        return list
+
+    def __get_magnet_types_list(self, number_of_magnets: int):
+        list = []
+        for i in range(1, number_of_magnets+1):
+            list.append(1)
+        return list
+
+    def __get_circuit_type(self, circuit_name: str):
+        if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
+            return "RCB"
+        elif circuit_name.startswith(("RD1", "RD2", "RD3", "RD4")):
+            return {"RD1": "RD1", "RD2": "RD2", "RD3": "RD3", "RD4": "RD4"}.get(circuit_name[:3], "No match found")
+
+
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/builders/BuilderFiQuS.py` & `steam_sdk-2023.4.0/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/builders/BuilderLEDET.py` & `steam_sdk-2023.4.0/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/builders/BuilderModel.py` & `steam_sdk-2023.4.0/steam_sdk/builders/BuilderModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -520,22 +520,26 @@
                                      verbose=self.verbose)
 
         # Write output yaml file
         parser_PyBBQ = ParserPyBBQ(builder_PyBBQ)
         nameFilePyBBQ = os.path.join(self.output_path, conductor_name + '.yaml')  # full path of the PyBBQ input file to write
         parser_PyBBQ.writePyBBQ2yaml(full_path_file_name=nameFilePyBBQ, verbose=self.verbose)
 
-    def buildSIGMA(self):
+    def buildSIGMA(self, output_path = None):
         """
             Building a SIGMA model
         """
+        file_working_directory = os.getcwd()
+        if not output_path:
+            output_path = self.output_path
 
         BuilderSIGMA(input_model_data=self.model_data, input_roxie_data=self.roxie_data,
-                     settings_dict=self.settings_dict, output_path=self.output_path,
+                     settings_dict=self.settings_dict, output_path=output_path,
                      flag_build=self.flag_build, verbose=self.verbose)
+        os.chdir(file_working_directory)
 
 
     def load_circuit_parameters_from_csv(self, input_file_name: str, selected_circuit_name: str = None):
         '''
             Load circuit parameters from a csv file into a case=circuit object
             :param input_file_name: full path to the csv file
             :param selected_circuit_name: name of the circuit name whose parameters will be loaded
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/builders/BuilderProteCCT.py` & `steam_sdk-2023.4.0/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/builders/BuilderPyBBQ.py` & `steam_sdk-2023.4.0/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam_sdk-2023.4.0/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/builders/Solenoids.py` & `steam_sdk-2023.4.0/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/builders/geometricFunctions.py` & `steam_sdk-2023.4.0/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataAnalysis.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataAnalysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,25 @@
     """
         Level 1: Class for general information on the case study
     """
     analysis_name: str = None
     flag_permanent_settings: bool = None
     model: Model = Model()
 
+class StrandCriticalCurrentMeasurement(BaseModel):
+    """
+        Level 1: Class for essential parameters for a critical current measurement to adjust Jc fit parameters
+    """
+    column_name_I_critical: str = None
+    reference_mag_field: float = None
+    reference_temperature: float = None
+    column_name_CuNoCu_short_sample: str = None
+    coil_names: List[str] = []
+
+
 
 ############################
 # Working folders
 class WorkingFolders(BaseModel):
     """
         Level 1: Class for information on the working folders
     """
@@ -194,14 +205,26 @@
     t_offset: List[float] = []
     interpolation_type: str = None  # 'Linear' or 'Spline'
     type_file_writing: str = None  # 'w' or 'a'
     n_sampling: int = None
     magnet_types: List[int] = []
 
 
+class DefaultParsimEventKeys(BaseModel):
+    """
+        Level 3: Class for default keys of ParsimEventMagnet
+    """
+    local_LEDET_folder: str = None
+    path_config_file: str = None
+    default_configs: List[str] = []
+    path_tdms_files: str = None
+    path_output_measurement_files: str = None
+    path_output: str = None
+
+
 class ParsimEvent(BaseModel):
     """
         Level 2: Analysis step to write stimulus file from coil resistance csv file
     """
     type: Literal['ParsimEvent']
     input_file: str = None
     path_output_event_csv: str = None
@@ -211,15 +234,15 @@
     case_model: str = None
     simulation_name: str = None
     software: List[str] = []
     t_PC_off: float = None  # TODO: consider making list of floats
     rel_quench_heater_trip_threshold: float = None
     current_polarities_CLIQ: List[int] = []  # TODO: consider making list of lists
     dict_QH_circuits_to_QH_strips: Dict[str, List[int]] = {}
-    default_keys: Dict = {}  # TODO Consider making this a dataclass
+    default_keys: DefaultParsimEventKeys = DefaultParsimEventKeys()
 
 
 class ParametricSweep(BaseModel):
     """
         Level 2: Analysis step to write stimulus file from sweep input csv file
     """
     type: Literal['ParametricSweep']
@@ -236,15 +259,16 @@
     """
     type: Literal['ParsimConductor']
     model_name: str = None
     case_model: str = None
     input_file: str = None
     software: List[str] = []
     simulation_number: int = None
-    groups_to_coils: Dict[str, List[int]] = {}  # TODO: keys have to match Coil names in input file
+    strand_critical_current_measurements: List[StrandCriticalCurrentMeasurement] = []
+    groups_to_coils: Dict[str, List[int]] = {}
     path_output_sweeper_csv: str = None
 
 # class AnalysisStep(BaseModel):
 #     """
 #         Level 1: Class for information on the analysis step
 #         Objects of this class will be defined in AnalysisStepDefinition
 #     """
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataConductor.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataDakota.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataEventMagnet.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataFiQuS.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataLEDET.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataModelCircuit.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataModelConductor.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataModelMagnet.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataModelMagnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         Level 2: Class for the quench heater parameters
     """
     N_strips: int = None                              # nHeaterStrips
     t_trigger: List[float] = []                        # tQH
     U0: List[float] = []
     C: List[float] = []
     R_warm: List[float] = []
-    w: List[float] = []
+    w: List[float] = []                             # In Sigma this
     h: List[float] = []
     s_ins: List[float] = []
     type_ins: List[int] = []
     s_ins_He: List[float] = []
     type_ins_He: List[int] = []
     l: List[float] = []
     l_copper: List[float] = []
@@ -897,29 +897,35 @@
     physics: PhysicsProteCCT = PhysicsProteCCT()
     post_processing: PostProcessingProteCCT = PostProcessingProteCCT()
     plots: PlotsProteCCT = PlotsProteCCT()
 
 
 ############################
 # SIGMA options
+
+class TimeVectorSolutionSIGMA(BaseModel):
+    """
+        Level 2: Class for simulation time vector in SIGMA
+    """
+    time_step: List[List[float]] = None
+
 class TimeVectorSIGMA(BaseModel):
     """
         Level 2: Class for simulation time vector in SIGMA
     """
-    time_step: float = None
+    time_vector_solution: TimeVectorSolutionSIGMA =TimeVectorSolutionSIGMA()
 
 
 class SimulationSIGMA(BaseModel):
     """
         Level 2: Class for simulation parameters in SIGMA
     """
     generate_study: bool = None
-    run_study: bool = None
-    conductor_current: float = None
-    generate_report: bool = None
+    study_type: str = None
+    make_batch_mode_executable: bool = None
     nbr_elements_mesh_width: int = None
     nbr_elements_mesh_height: int = None
     max_mesh_size: float = None
 
 
 class PhysicsSIGMA(BaseModel):
     """
@@ -936,24 +942,61 @@
 class QuenchInitializationSIGMA(BaseModel):
     """
         Level 2: Class for quench initialization parameters in SIGMA
     """
     PARAM_time_quench: float = None
     FLAG_quench_all: int = None
     FLAG_quench_off: int = None
+    num_qh_div: List[int] = None
+    quench_init_heat: List[float] = None
+    quench_init_HT: List[str] = None
+    quench_stop_temp: float = None
+
+class Out2DAtPointsSIGMA(BaseModel):
+    coordinate_source: List[str] = None
+    variables: List[str] = None
+    time_transient: List[List[float]] = None
+    time: List[List[float]] = None
+
+
+class Out1DVsTimeSIGMA(BaseModel):
+    variables: List[str] = None
+    time: List[List[float]] = None
+
+
+class Out1DVsAllTimesSIGMA(BaseModel):
+    variables: List[str] = None
+
+class QuenchHeatersSIGMA(BaseModel):
+    """
+        Level 2: Class for postprocessing parameters in SIGMA
+    """
+    quench_heater_positions: List[List[int]] = None
+    th_coils: List[float] = None
+
+
+class PostprocessingSIGMA(BaseModel):
+    """
+        Level 2: Class for postprocessing parameters in SIGMA
+    """
+    out_2D_at_points: Out2DAtPointsSIGMA = Out2DAtPointsSIGMA()
+    out_1D_vs_times: Out1DVsTimeSIGMA = Out1DVsTimeSIGMA()
+    out_1D_vs_all_times: Out1DVsAllTimesSIGMA = Out1DVsAllTimesSIGMA()
 
 
 class SIGMA(BaseModel):
     """
         Level 1: Class for SIGMA options
     """
-    time_vector: TimeVectorSIGMA = TimeVectorSIGMA()
+    time_vector_solution: TimeVectorSolutionSIGMA = TimeVectorSolutionSIGMA()
     simulation: SimulationSIGMA = SimulationSIGMA()
     physics: PhysicsSIGMA = PhysicsSIGMA()
     quench_initialization: QuenchInitializationSIGMA = QuenchInitializationSIGMA()
+    postprocessing: PostprocessingSIGMA = PostprocessingSIGMA()
+    quench_heaters: QuenchHeatersSIGMA=QuenchHeatersSIGMA()
 
 
 ############################
 # Highest level
 class DataModelMagnet(BaseModel):
     """
         **Class for the STEAM inputs**
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataParsimConductor.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataParsimConductor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import (List, Dict)
+from typing import (List, Dict, Union, Literal)
 from pydantic import BaseModel
 
 ############################
 # General parameters
-class GeneralParameters(BaseModel):
+class GeneralParameters(BaseModel):  # TODO do we need this?
     magnet_name: str = None
     circuit_name: str = None
     state: str = None  # measured, deduced from short-samples, deduced from design
 
 ############################
 # Magnet
 class Magnet(BaseModel):
@@ -21,48 +21,70 @@
     cable_ID: str = None
     coil_length: float = None
     coil_RRR: float = None
     T_ref_RRR_low: float = None
     T_ref_RRR_high: float = None
     coil_resistance_room_T: float = None
     T_ref_coil_resistance: float = None
-    conductors: List[str] = []  # TODO: make sure that names correspond to conductor instances
-    weight_conductors: List[float] = []  # TODO: make sure the length is the same as of the list before
+    conductors: List[str] = []  # TODO: make sure that names correspond to conductor instances - maybe call it sample?
+    weight_conductors: List[float] = []
 
 ############################
 # Conductors
-class Conductor(BaseModel):
+class IcMeasurement(BaseModel):
+    """
+        Level 1: Class for parameters of a critical current measurement to adjust Jc fit parameters
+    """
+    Ic: float = None
+    T_ref_Ic: float = None
+    B_ref_Ic: float = None
+    Cu_noCu_sample: float = None
+
+
+class Round(BaseModel):
+    """
+        Level 2: Class for strand parameters
+    """
+    type: Literal['Round']
+    diameter: float = None
+
+class Rectangular(BaseModel):
+    """
+        Level 2: Class for strand parameters
+    """
+    type: Literal['Rectangular']
+    bare_width: float = None
+    bare_height: float = None
+
+
+class ConductorSample(BaseModel):
+    # TODO think of using other conductor class
     ID: str = None
-    shape: str = None # round, rectangular
     number_of_strands: int = None
-    strand_diameter: float = None
     width: float = None
     height: float = None
     Cu_noCu: float = None
     RRR: float = None
     strand_twist_pitch: float = None
     filament_twist_pitch: float = None
-    Ic_1: float = None
-    T_ref_Ic_1: float = None
-    B_ref_Ic_1: float = None
-    Cu_noCu_sample_1: float = None
-    Ic_2: float = None
-    T_ref_Ic_2: float = None
-    B_ref_Ic_2: float = None
-    Cu_noCu_sample_2: float = None
+    Ic_measurements: List[IcMeasurement] = []
+    Tc0: float = None
+    Bc20: float = None
     f_rho_eff: float = None
     Ra: float = None
     Rc: float = None
+    strand_geometry: Union[Round, Rectangular] = None
+
 
 class DataParsimConductor(BaseModel):
     '''
-        **Class for the STEAM magnet**
+        **Class for the STEAM conductor**
 
-        This class contains the data structure of a Conductor parsim event analyzed with STEAM_SDK.
+        This class contains the data structure of a Conductor parsim  analyzed with STEAM_SDK.
 
         :return: DataParsimConductor object
     '''
 
     GeneralParameters: GeneralParameters = GeneralParameters()
     Magnet: Magnet = Magnet()
     Coils: Dict[str, Coil] = {}
-    Conductors: Dict[str, Conductor] = {}
+    ConductorSamples: Dict[str, ConductorSample] = {}
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataProteCCT.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataPyBBQ.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataRoxieParser.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataSettings.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataSettings.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 
 class DataSettings(BaseModel):
     """
         Dataclass of settings for STEAM analyses
         This will be populated either form a local settings file (if flag_permanent_settings=False)
         or from the keys in the input analysis file (if flag_permanent_settings=True)
     """
-    comsolexe_path:      str = None  # full path to comsol.exe, only COMSOL53a is supported
-    JAVA_jdk_path:       str = None  # full path to folder with java jdk
-    CFunLibPath:         str = None  # path to dll files with material properties
-    COSIM_path:          str = None  #
-    Dakota_path:         str = None  #
-    FiQuS_path:          str = None  #
-    GetDP_path:          str = None  # full path to CERN GetDP build executable
-    LEDET_path:          str = None  #
-    ProteCCT_path:       str = None  #
-    PSPICE_path:         str = None  #
-    PyBBQ_path:          str = None  #
-    XYCE_path:           str = None  #
-    PSPICE_library_path: str = None  #
-    local_Dakota_path:   str = None  # full path to local Dakota folder
-    local_FiQuS_folder:  str = None  # full path to local FiQuS folder
-    local_LEDET_folder:  str = None  # full path to local LEDET folder
-    local_PyBBQ_folder:  str = None  # full path to local PyBBQ folder
-    local_PSPICE_folder: str = None  # full path to local PSPICE folder
-    local_XYCE_folder:   str = None  # full path to local PSPICE folder
+    comsolexe_path:       str = None  # full path to comsol.exe, only COMSOL53a is supported
+    JAVA_jdk_path:        str = None  # full path to folder with java jdk
+    CFunLibPath:          str = None  # path to dll files with material properties
+    COSIM_path:           str = None  #
+    Dakota_path:          str = None  #
+    FiQuS_path:           str = None  #
+    GetDP_path:           str = None  # full path to CERN GetDP build executable
+    LEDET_path:           str = None  #
+    ProteCCT_path:        str = None  #
+    PSPICE_path:          str = None  #
+    PyBBQ_path:           str = None  #
+    XYCE_path:            str = None  #
+    PSPICE_library_path:  str = None  #
+    local_Dakota_path:    str = None  # full path to local Dakota folder
+    local_FiQuS_folder:   str = None  # full path to local FiQuS folder
+    local_LEDET_folder:   str = None  # full path to local LEDET folder
+    local_PyBBQ_folder:   str = None  # full path to local PyBBQ folder
+    local_PSPICE_folder:  str = None  # full path to local PSPICE folder
+    local_SIGMA_folder:   str = None  # full path to local SIGMA folder
+    local_XYCE_folder:    str = None  # full path to local PSPICE folder
+    MTF_credentials_path: str = None  # full path to the txt file containing the credentials for MTF login
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DataSignal.py` & `steam_sdk-2023.4.0/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DictionaryLEDET.py` & `steam_sdk-2023.4.0/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DictionaryProteCCT.py` & `steam_sdk-2023.4.0/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/DictionaryPyBBQ.py` & `steam_sdk-2023.4.0/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/TemplateLEDET.py` & `steam_sdk-2023.4.0/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/data/TemplateProteCCT.py` & `steam_sdk-2023.4.0/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverAnalysis.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverDakota.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverFiQuS.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverLEDET.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverPSPICE.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverProteCCT.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverPyBBQ.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverSIGMA.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverSIGMA.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,31 @@
+import glob
 import os
 import subprocess
 
 import pandas as pd
 
 from steam_sdk.builders.BuilderSIGMA import BuilderSIGMA
+from steam_sdk.parsers.ParserCOMSOLToTxt import ParserCOMSOLToTxt
+
 
 class DriverSIGMA:
     """
         Class to drive SIGMA models
     """
     def __init__(self, magnet_name, SIGMA_path='', path_folder_SIGMA=None, path_folder_SIGMA_input=None, verbose=False):
         self.SIGMA_path = SIGMA_path
         self.path_folder_SIGMA = path_folder_SIGMA
         self.path_folder_SIGMA_input = path_folder_SIGMA_input
         self.verbose = verbose
         self.magnet_name = magnet_name
-        self.working_dir_path = os.getcwd()
+        if path_folder_SIGMA is None:
+            self.working_dir_path = os.getcwd()
+        else:
+            self.working_dir_path = path_folder_SIGMA
         if verbose:            print('path_exe =          {}'.format(SIGMA_path))
 
 
     def create_coordinate_file(self, path_map2d, coordinate_file_path):
         """
         Creates a csv file with same coordinates as the map2d.
 
@@ -68,45 +74,48 @@
                 fill = f"{fill:.4f}"
                 content.append(
                     "{0:>6}{1:>6}{2:>7}{3:>13}{4:>13}{5:>11}{6:>11}{7:>11}{8:>9}{9:>8}\n".format(bl, cond, no, x, y, Bx,
                                                                                                  By,
                                                                                                  area, curr, fill))
             file.writelines(content)
 
+    @staticmethod
+    def export_all_txt_to_concat_csv():
+        """
+        Export 1D plots vs time to a concatenated csv file. This file can be utilized with the Viewer.
+        :return:
+        """
+        keyword = "all_times"
+        files_to_concat = []
+        for filename in os.listdir():
+            if keyword in filename:
+                files_to_concat.append(filename)
+        df_concat = pd.DataFrame()
+        for file in files_to_concat:
+            df = ParserCOMSOLToTxt().loadTxtCOMSOL(file, header=["time", file.replace(".txt", "")])
+            df_concat = pd.concat([df_concat, df], axis = 1)
+            df_concat= df_concat.loc[:, ~df_concat.columns.duplicated()]
+            print(df_concat)
+        df_concat=df_concat.reset_index(drop=True)
+        df_concat.to_csv("SIGMA_transient_concat_output_1234567890MF.csv", index = False)
 
 
-
-    def run_SIGMA(self, model_data: dict, roxie_data: dict , settings: dict, coordinate_file_path: str='', map2d_path_ref: str='', map2d_path: str='', output_txt_path: str=''):
+    def run_SIGMA(self, concat_time_frames = True):
         """
         Run the BuilderSigma with given params.
-        :param model_data: Model data in dict format.
-        :param roxie_data: Roxie data in dict format.
-        :param settings: Settings file containg comsol and material library path.
-        :param coordinate_file_path: Path to location where coordinate file is to be saved to.
-        :param map2d_path_ref: Reference map2d file path to create coordinate file which COMSOL can evaluate the field in.
-        :param map2d_path: The path which the result map2d is saved to.
-        :param output_txt_path: Path to where COMSOL puts the output txt.
+        :param concat_time_frames:???
         :return:
         """
-        if not model_data.Options_SIGMA.simulation.generate_study and model_data.Options_SIGMA.simulation.run_study: #Change?
-            raise ValueError("Can not run study without generating one.")
-        if model_data.Options_SIGMA.simulation.run_study:
-            self.create_coordinate_file(map2d_path_ref, coordinate_file_path)
-
-        result_txt_path = output_txt_path.replace("\\", "\\\\\\\\")
-        coordinate_file_path = coordinate_file_path.replace("\\", "\\\\\\\\")
-        BuilderSIGMA(settings_dict=settings, input_model_data=model_data, input_roxie_data=roxie_data,
-                     generate_study=model_data.Options_SIGMA.simulation.generate_study,
-                     coordinate_file_path=coordinate_file_path, result_txt_path=result_txt_path)
-
-        if model_data.Options_SIGMA.simulation.run_study:
-            batch_file_path = os.path.join(self.working_dir_path, f"{self.magnet_name}_Model_Compile_and_Open.bat")
-            proc = subprocess.Popen([batch_file_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
-            (stdout, stderr) = proc.communicate()
-
-            if proc.returncode != 0:
-                print(stderr)
-            else:
-                print(stdout)
 
-        if model_data.Options_SIGMA.simulation.run_study and model_data.Options_SIGMA.simulation.generate_study:
-            self.export_B_field_txt_to_map2d(map2d_path_ref, output_txt_path, map2d_path)
+        os.chdir(self.working_dir_path)
+        batch_file_path = os.path.join(self.working_dir_path, f"{self.magnet_name}_Model_Compile_and_Open.bat")
+        print(f'Running Comsol model via: {batch_file_path}')
+        subprocess.call(batch_file_path)
+        # proc = subprocess.Popen([batch_file_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
+        # (stdout, stderr) = proc.communicate()
+        #
+        # if proc.returncode != 0:
+        #     print(stderr)
+        # else:
+        #     print(stdout)
+        if concat_time_frames:
+            self.export_all_txt_to_concat_csv()
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/drivers/DriverXYCE.py` & `steam_sdk-2023.4.0/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/CSD_Reader.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserCond2d.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserCsd.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserCsv.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserDakota.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserExcel.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserFiQuS.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserLEDET.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserMap2d.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserMat.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserPSPICE.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserPSPICE.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-import os
+import ast
 import csv
 import datetime
 import ntpath
+import os
 import shutil
 import textwrap
 from itertools import zip_longest
 from pathlib import Path
 from typing import Union, List
+
 import matplotlib.pyplot as plt
-from scipy.interpolate import UnivariateSpline
-from scipy.interpolate import interp1d
-import pandas as pd
 import numpy as np
+import pandas as pd
 import yaml
+from scipy.interpolate import UnivariateSpline
+from scipy.interpolate import interp1d
 
 from steam_sdk.data.DataModelCircuit import DataModelCircuit, Component
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 
 
 class ParserPSPICE:
     """
@@ -762,14 +764,18 @@
 
 def add_transient_time_schedule(time_schedule):
     ''' Format transient time schedule rows '''
     # If time_schedule is not defined, output will be None
     if time_schedule == None or len(time_schedule) == 0:
         return None
 
+    # If the variable is a string, convert it to a dictionary
+    if isinstance(time_schedule, str):
+        time_schedule = ast.literal_eval(time_schedule)
+
     formatted_text = '+ {SCHEDULE(\n'
     for time_window_start, time_step_in_window in time_schedule.items():
         if time_window_start == list(time_schedule.keys())[-1]:
             formatted_text = formatted_text + '+ ' + time_window_start + ', ' + time_step_in_window + '\n'  # the last entry must not have the comma
         else:
             formatted_text = formatted_text + '+ ' + time_window_start + ', ' + time_step_in_window + ',' + '\n'
     formatted_text = formatted_text + '+)}'
@@ -961,131 +967,15 @@
         f.suptitle(str(current_level[0][0]) + 'A', fontsize=16)
         plt.show()
     if n_apertures == 2:
         return [time, new_R1, new_R2]
     else:
         return [time, new_R1]
 
-
-def writeStimuliFromInterpolation(current_level: list, n_total_magnets: int, n_apertures: int, magnets: list, tShift: list, Outputfile: str, path_resources: str,
-                                  InterpolationType: str = 'Linear', type_stl: str = 'a', sparseTimeStepping: int = 100):
-    '''
-    Function to write a resistance stimuli for n apertures of a magnet for any current level. Resistance will be interpolated
-    from pre-calculated values (see InterpolateResistance for closer explanation). Stimuli is then written in a .stl file for PSPICE
-
-    :param current_level: list, all current level that shall be used for interpolation (each magnet has 1 current level)
-    :param n_total_magnets: int, Number of total magnets in the circuit (A stimuli will be written for each, non-quenching = 0)
-    :param n_apertures: int, Number of apertures per magnet. A stimuli will be written for each aperture for each magnet
-    :param magnets: list, magnet numbers for which the stimuli shall be written
-    :param tShift: list, time shift that needs to be applied to each stimuli
-    (e.g. if magnet 1 quenches at 0.05s, magnet 2 at 1s etc.), so that the stimuli are applied at the correct time in the simulation
-    :param Outputfile: str, name of the stimuli-file
-    :param path_resources: str, path to the file with pre-calculated values
-    :param Type: str, either Linear or Spline, type of interpolation
-    :param type_stl: str, how to write the stimuli file (either 'a' (append) or 'w' (write))
-    :param sparseTimeStepping: int, every x-th time value only a stimuli point is written (to reduce size of stimuli)
-    :return:
-    '''
-    if n_apertures>2: raise Exception('Maximum of 2 apertures supported yet.')
-    # Ensure consistency of inputs
-    if len(magnets) != len(tShift): raise Exception(f'Please provide a time shift for each magnet. '
-                                                    f'Size of magnet list is {len(magnets)}, but size of tShift is {len(tShift)}')
-
-    R1 = np.array([])
-    R2 = np.array([])
-    print("Interpolating Coil-Resistances")
-    # Interpolate data for each current level and ensure correct data format
-    for k in current_level:
-        if n_apertures == 2:
-            [time, data_R1, data_R2] = InterpolateResistance(k, path_resources, n_apertures=n_apertures, Type = InterpolationType)
-        else:
-            [time, data_R1] = InterpolateResistance(k, path_resources, n_apertures=n_apertures, Type=InterpolationType)
-        if not R1.size > 0:
-            R1 = data_R1[np.newaxis, ...]
-        else:
-            R1 = np.vstack((R1, data_R1))
-        if n_apertures == 2:
-            if not R2.size > 0:
-                R2 = data_R2[np.newaxis, ...]
-            else:
-                R2 = np.vstack((R2, data_R2))
-    stlString = ''
-
-    # Loop through all current level
-    for k in range(1, n_total_magnets+1):
-        if k in magnets:
-            index = magnets.index(k)
-            timeShift = tShift[index]
-            if timeShift < 0: timeShift = 0
-
-            # Start with generating stimulus for first aperture
-            stlString = stlString + f'\n.STIMULUS R_coil_{str(1)}_M{str(magnets[index])} ' \
-                                    f'PWL \n+ TIME_SCALE_FACTOR = 1 \n+ VALUE_SCALE_FACTOR = 1 \n'
-            stlString = stlString + "+ ( 0s, 0.0 )\n"
-            count = 0
-            # Set a resistance value in the stimuli for each sparseTimeStepping * TimeValue
-            for l in range(1, R1.shape[1] - 1):
-                if np.isnan(R1[index, l]): continue
-                # Ensure starting at 0 (No negative time in PSPICE allowed
-                if float(time[l]) < 0:  timeShift = timeShift + abs(float(time[l])) - 0.03
-                if float(time[l]) + timeShift < 0:
-                    tt = 0
-                else:
-                    tt = float(time[l]) + timeShift
-                # If every sparseTimeStepping* time value reached, write an entry
-                if count >= sparseTimeStepping:
-                    stlString = stlString + "+ ( " + str(tt) + "s, " + str(R1[index, l]) + " )\n"
-                    count = 0
-                count = count + 1
-            # Write last time value to be 10000 s, with last resistance (resistance is assumed to stay constant)
-            R1_last = R1[index]
-            R1_last = R1_last[~np.isnan(R1_last)]
-            stlString = stlString + "+ ( " + str(10000) + "s," + str(R1_last[-1]) + " ) \n"
-            stlString = stlString + " \n"
-
-            if n_apertures == 2:
-                # Repeat procedure for second aperture
-                stlString = stlString + f'\n.STIMULUS R_coil_{str(2)}_M{str(magnets[index])} ' \
-                                        f'PWL \n+ TIME_SCALE_FACTOR = 1 \n+ VALUE_SCALE_FACTOR = 1 \n'
-                stlString = stlString + "+ ( 0s, 0.0 )\n"
-                count = 0
-                for l in range(1, R2.shape[1] - 1):
-                    if np.isnan(R2[index, l]): continue
-                    if float(time[l]) < 0:  timeShift = timeShift + abs(float(time[l])) - 0.03
-                    if float(time[l]) + timeShift < 0:
-                        tt = 0
-                    else:
-                        tt = float(time[l]) + timeShift
-                    if count >= sparseTimeStepping:
-                        stlString = stlString + "+ ( " + str(tt) + "s, " + str(R2[index, l]) + " )\n"
-                        count = 0
-                    count = count + 1
-                R2_last = R2[index]
-                R2_last = R2_last[~np.isnan(R2_last)]
-                stlString = stlString + "+ ( " + str(10000) + "s," + str(R2_last[-1]) + " ) \n"
-                stlString = stlString + " \n"
-        else:
-            stlString = stlString + f'\n.STIMULUS R_coil_{str(1)}_M{str(k)} ' \
-                                    f'PWL \n+ TIME_SCALE_FACTOR = 1 \n+ VALUE_SCALE_FACTOR = 1 \n'
-            stlString = stlString + "+ ( 0s, 0.0 )\n"
-            stlString = stlString + "+ ( 10000s, 0.0 )\n"
-
-            if n_apertures == 2:
-                stlString = stlString + f'\n.STIMULUS R_coil_{str(2)}_M{str(k)} ' \
-                                        f'PWL \n+ TIME_SCALE_FACTOR = 1 \n+ VALUE_SCALE_FACTOR = 1 \n'
-                stlString = stlString + "+ ( 0s, 0.0 )\n"
-                stlString = stlString + "+ ( 10000s, 0.0 )\n"
-
-    # Write the stimuli as a txt(stl) file
-    with open(Outputfile, type_stl) as ofile:
-        ofile.write(stlString)
-
-
-
-def writeStimuliFromInterpolation_general(current_level: list, n_total_magnets: int, n_apertures: int, magnets: list, tShift: list, Outputfile: str, path_resources: Union[str,list],
+def writeStimuliFromInterpolation(current_level: list, n_total_magnets: int, n_apertures: int, magnets: list, tShift: list, Outputfile: str, path_resources: Union[str,list],
                                   InterpolationType: str = 'Linear', type_stl: str = 'a', sparseTimeStepping: int = 100, magnet_type: list = None):
     '''
     Function to write a resistance stimuli for n apertures of a magnet for any current level. Resistance will be interpolated
     from pre-calculated values (see InterpolateResistance for closer explanation). Stimuli is then written in a .stl file for PSPICE
 
     :param current_level: list, all current level that shall be used for interpolation (each magnet has 1 current level)
     :param n_total_magnets: int, Number of total magnets in the circuit (A stimuli will be written for each, non-quenching = 0)
@@ -1098,15 +988,15 @@
     :param magnet_type: list, contains numbers from 1 to len(path_resources) for each magnet
     (e.g. if there are three items in the path_resources list and four magnets, then magnet_type can be [2,2,1,1] or [1,2,3,3] telling us which path_resource file to use for each magnet
     :param Type: str, either Linear or Spline, type of interpolation
     :param type_stl: str, how to write the stimuli file (either 'a' (append) or 'w' (write))
     :param sparseTimeStepping: int, every x-th time value only a stimuli point is written (to reduce size of stimuli)
     :return:
     '''
-    # Check inputs and set default vaues
+    # Check inputs and set default values
     if type(path_resources) == str:
         path_resources = [path_resources] * len(magnets)  # make a list out of the string
 
     if not magnet_type:
         magnet_type = [1] * len(magnets)  # make a list of 1's (to maintain the same behavior as the older version fo the function)
 
     if n_apertures>2: raise Exception('Maximum of 2 apertures supported yet.')
@@ -1137,35 +1027,32 @@
                 else:
                     R1 = np.vstack((R1, data_R1))
                 if n_apertures == 2:
                     if not R2.size > 0:
                         R2 = data_R2[np.newaxis, ...]
                     else:
                         R2 = np.vstack((R2, data_R2))
-        #stlString = ''
 
-    # Loop through all current level
-    #for k in range(1, n_total_magnets+1):
-        #if k in magnets:
             index = magnets.index(k)
             timeShift = tShift[index]
             if timeShift < 0: timeShift = 0
 
             # Start with generating stimulus for first aperture
             stlString = stlString + f'\n.STIMULUS R_coil_{str(1)}_M{str(magnets[index])} ' \
                                     f'PWL \n+ TIME_SCALE_FACTOR = 1 \n+ VALUE_SCALE_FACTOR = 1 \n'
             stlString = stlString + "+ ( 0s, 0.0 )\n"
             count = 0
             # Set a resistance value in the stimuli for each sparseTimeStepping * TimeValue
             for l in range(1, R1.shape[1] - 1):
                 if np.isnan(R1[index, l]): continue
                 # Ensure starting at 0 (No negative time in PSPICE allowed
-                if float(time[l]) < 0:  timeShift = timeShift + abs(float(time[l]))
+                # if float(time[l]) < 0:  timeShift = timeShift + abs(float(time[l]))
+
                 if float(time[l]) + timeShift < 0:
-                    tt = 0
+                    raise Exception ("PSPICE can't process negative times, please provide a greater timeshift")
                 else:
                     tt = float(time[l]) + timeShift
                 # If every sparseTimeStepping* time value reached, write an entry
                 if count >= sparseTimeStepping:
                     stlString = stlString + "+ ( " + str(tt) + "s, " + str(R1[index, l]) + " )\n"
                     count = 0
                 count = count + 1
@@ -1180,17 +1067,18 @@
                 # Repeat procedure for second aperture
                 stlString = stlString + f'\n.STIMULUS R_coil_{str(2)}_M{str(magnets[index])} ' \
                                         f'PWL \n+ TIME_SCALE_FACTOR = 1 \n+ VALUE_SCALE_FACTOR = 1 \n'
                 stlString = stlString + "+ ( 0s, 0.0 )\n"
                 count = 0
                 for h in range(1, R2.shape[1] - 1):
                     if np.isnan(R2[index, h]): continue
-                    if float(time[h]) < 0:  timeShift = timeShift + abs(float(time[h]))
+                    #if float(time[h]) < 0:  timeShift = timeShift + abs(float(time[h]))
                     if float(time[h]) + timeShift < 0:
-                        tt = 0
+                        raise Exception("PSPICE can't process negative times, please provide a greater timeshift")
+                        #tt = 0
                     else:
                         tt = float(time[h]) + timeShift
                     if count >= sparseTimeStepping:
                         stlString = stlString + "+ ( " + str(tt) + "s, " + str(R2[index, h]) + " )\n"
                         count = 0
                     count = count + 1
                 R2_last = R2[index]
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserProteCCT.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserRoxie.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserTdms.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserXYCE.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsers/ParserYAML.py` & `steam_sdk-2023.4.0/steam_sdk/parsers/ParserYAML.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,11 +89,8 @@
     data_dict = list_single_row_recursively(data_dict, list_exceptions=list_exceptions)
 
     # Make sure the target folder exists
     make_folder_if_not_existing(os.path.dirname(name_output_file), verbose=False)
 
     # Write yaml file
     with open(name_output_file, 'w') as yaml_file:
-        if with_comments:
-            ruamel.yaml.round_trip_dump(data_dict, yaml_file)
-        else:
-            ruamel_yaml.dump(data_dict, yaml_file)
+        ruamel_yaml.dump(data_dict, yaml_file)
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsims/ParsimDakota.py` & `steam_sdk-2023.4.0/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsims/ParsimEventMagnet.py` & `steam_sdk-2023.4.0/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import csv
 from typing import List, Dict
 import pandas as pd
 import yaml
 from pathlib import Path
 
 from steam_sdk.builders.BuilderModel import BuilderModel
+from steam_sdk.data.DataAnalysis import DefaultParsimEventKeys
 from steam_sdk.parsers.ParserTdms import ParserTdms
 from steam_sdk.data.DataEventMagnet import DataEventMagnet, QuenchHeaterCircuit
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.sgetattr import rsetattr, rgetattr
 
 
 class ParsimEventMagnet:
@@ -26,15 +27,14 @@
         # Unpack arguments
         self.verbose: bool = verbose
         self.list_events: List[DataEventMagnet] = []
         self.dict_AnalysisStepDefinition = {}
         self.list_AnalysisStepSequence = []
         # save local reference model, so that empty field in EventData.csv can be populated with default ones
         self.ref_model = ref_model
-        # TODO add a dictionary of default values?
 
     def read_from_input(self, path_input_file: str, flag_append: bool, rel_quench_heater_trip_threshold: bool):
         '''
         Read a list of events from an input .csv file and assign its content to a list of DataEventMagnet() objects.
         This method is used to read and set the variables that can be expressed with one or a limited amount of values.
         More complex variables are covered by dedicated methods.
 
@@ -50,15 +50,15 @@
             df_events = pd.read_excel(path_input_file)
         else:
             raise Exception(f'The extension of the file {path_input_file} is not supported.')
         df_events = df_events.dropna(axis=1, how='all')
 
         # validate dataframe - if csv file has a headline or empty rows on the top, skip row until there all columnnames have values
         skip_rows = 0
-        while any(['Unnamed: '  in s for s in df_events.columns]): # pandas assigns the columname 'Unnamed: i' when no name can be found
+        while any(['Unnamed: ' in s for s in df_events.columns]): # pandas assigns the columname 'Unnamed: i' when no name can be found
             skip_rows += 1
             if path_input_file.endswith('.csv'):
                 df_events = pd.read_csv(path_input_file, skiprows=skip_rows)
             elif path_input_file.endswith('.xlsx'):
                 df_events = pd.read_excel(path_input_file, skiprows=skip_rows)
             df_events = df_events.dropna(axis=1, how='all')
             if skip_rows == 2:  # check only for the first 2 rows
@@ -120,15 +120,15 @@
             new_row = dict()
             # loop trough each element of self.list_events and write parameters to csv
             for i, event in enumerate(self.list_events):
                 new_row.clear()
                 new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
                 new_row.update(self.__write_analysis_powering(event, t_PC_off))
                 new_row.update(self.__write_analysis_CLIQ(event, current_polarities_CLIQ))
-                new_row.update(self.__write_analysis_QH(event, dict_QH_circuits_to_QH_strips)) #TODO: case when dict_QH is empty
+                new_row.update(self.__write_analysis_QH(event, dict_QH_circuits_to_QH_strips))
                 new_row.update(self.__write_analysis_general_parameters(event))
                 # self.__read_analysis_general_parameters(model_name, simulation_numbers, simulation_name, software, event,i)
                 writer = csv.DictWriter(csv_file, fieldnames=new_row.keys())
                 if i == 0: writer.writeheader()
                 writer.writerow(new_row)
 
     # def set_up_analysis(self, model_name: str, simulation_numbers: List[int], simulation_name: str, software : List[str],
@@ -179,41 +179,37 @@
     #             # check if there are columns in the csv for every variable to change
     #             missing_keys = [key for key in new_row.keys() if key not in fieldnames]
     #             if missing_keys:
     #                 raise ValueError(f"The following keys are missing from the list: {', '.join(missing_keys)}")
     #             writer.writerow(new_row)
 
 
-    def set_up_viewer(self, path_output_viewer_csv: str, default_keys: Dict, simulation_numbers: List[int], simulation_name: str, software: str):
+    def set_up_viewer(self, path_output_viewer_csv: str, default_keys: DefaultParsimEventKeys, simulation_numbers: List[int], simulation_name: str, software: str):
         '''
         Write a .csv file that can be used to run a STEAM Viewer analysis
         
         :param path_output_viewer_csv:
         :param default_keys: 
         :param simulation_numbers: 
         :param simulation_name: 
         :param software:
         '''
-        # Unpack input dictionary with default key values. If keys are not present in the dictionary, set default values to empty strings
-        path_config_file              = default_keys['path_config_file']              if 'path_config_file' in default_keys else ''
-        default_configs               = default_keys['default_configs']               if 'default_configs' in default_keys else ''
-        default_config_sim            = default_keys['default_config_sim']            if 'default_config_sim' in default_keys else ''
-        path_tdms_files               = default_keys['path_tdms_files']               if 'path_tdms_files' in default_keys else ''
-        path_output_measurement_files = default_keys['path_output_measurement_files'] if 'path_output_measurement_files' in default_keys else ''
-        path_output                   = default_keys['path_output']                   if 'path_output' in default_keys else ''
-
-        # Make default_configs to a list if only one config is given by user
-        if not isinstance(default_configs, list): default_configs = [default_configs]
+        # Unpack input dictionary with default key values
+        path_config_file              = default_keys.path_config_file
+        default_configs               = default_keys.default_configs
+        path_tdms_files               = default_keys.path_tdms_files
+        path_output_measurement_files = default_keys.path_output_measurement_files
+        path_output                   = default_keys.path_output
 
         # Read the signal names needed for the different configurations to later check which configuration can be used
         dict_configs_with_signals = self.__read_signals_of_configs(default_configs, path_config_file)
 
         # Identify software-specific folder and file names
         if software == 'LEDET':
-            local_LEDET_folder = default_keys['local_LEDET_folder']
+            local_LEDET_folder = default_keys.local_LEDET_folder
             # Identify simulation folder based on the software
             path_simulation_folder = f'{local_LEDET_folder}\{simulation_name}\Output\Mat Files'
             # Identify simulation file names based on the software
             list_simulation_names = []
             for sim in simulation_numbers:
                 list_simulation_names.append(f'SimulationResults_LEDET_{sim}.mat')
         else:
@@ -232,45 +228,56 @@
                 "Simulation folder": path_simulation_folder,
                 "Simulation file": list_simulation_names[i],
                 "path_output_figures": path_output,
                 "path_output_simulation_files": "not_used",
                 "Comments": "no comments"
             }
 
-            # Find all 10-digit sequences of integers in the name string (this is the timestamp of the measurement)
+            # Find all 10-digit sequences of integers in the name string (this is the timestamp at which the measurement was taken)
             list_integer_sequences = re.findall(r'\d{10}', event.GeneralParameters.name)
+            if len(list_integer_sequences) == 0:
+                raise Exception(f'Timestamp in Event {event.GeneralParameters.name} could not be clearly identified. A sequence of 10 integers should be present to define a unique timestamp.')
+            elif len(list_integer_sequences) == 1:
+                timestamp = list_integer_sequences[0]
+            else:
+                raise Exception(f'More then one timestamp ({list_integer_sequences}) could be found in Event {event.GeneralParameters.name}. A sequence of 10 integers should be present to define a unique timestamp.')
 
-            # Look into the tdms test campaign folders and search for a files containing timestamp
-            campaign_name_tdms, name_file_found_tdms = self.search_file_in_subfolders(list_integer_sequences, path_tdms_files, '.tdms')
+
+            # Look into the tdms test campaign folders and search for files containing timestamp
+            campaign_name_tdms, name_file_found_tdms = search_file_in_subfolders(timestamp, path_tdms_files, '.tdms')
 
             # if a tdms file could be found, append remaining values to dataframe - this event is finished
             if campaign_name_tdms and name_file_found_tdms:
                 new_row["Test name"] = name_file_found_tdms
                 new_row["Test campaign"] = campaign_name_tdms
-                new_row["Configuration"] = self.get_config_tdms(path_tdms_files, campaign_name_tdms, name_file_found_tdms, dict_configs_with_signals)
+                new_row["Configuration"] = get_config_tdms(path_tdms_files, campaign_name_tdms, name_file_found_tdms,
+                                                           dict_configs_with_signals, self.verbose)
                 new_row["flag_convert_meas_csv"] = '1'  # csv will be generated by viewer if not present
                 df = pd.concat([df, pd.DataFrame([new_row])], ignore_index=True)  # Append the new row to the DataFrame
                 continue
 
+
             # if no tdms file present, search for csv file containing the timestamp
-            campaign_name_csv, name_file_found_csv = self.search_file_in_subfolders(list_integer_sequences, path_output_measurement_files, '.csv')
+            campaign_name_csv, name_file_found_csv = search_file_in_subfolders(timestamp, path_output_measurement_files,'.csv')
 
             # if a csv file could be found, append remaining values to dataframe - this event is finished
             if campaign_name_csv and name_file_found_csv:
                 new_row["Test name"] = name_file_found_csv
                 new_row["Test campaign"] = campaign_name_csv
-                new_row["Configuration"] = self.get_config_csv(dict_configs_with_signals, name_file_found_csv, dict_configs_with_signals)
+                new_row["Configuration"] = get_config_csv(path_output_measurement_files, campaign_name_csv,
+                                                          name_file_found_csv, dict_configs_with_signals, self.verbose)
                 new_row["flag_convert_meas_csv"] = '0'  # Viewer will not try to convert data
                 df = pd.concat([df, pd.DataFrame([new_row])], ignore_index=True)  # Append the new row to the DataFrame
                 continue
 
+
             # if neither tdms nor csv is found, no measurement data is attached - Viewer shows only simulation results
             new_row["Test name"] = ''
             new_row["Test campaign"] = ''
-            new_row["Configuration"] = default_config_sim
+            new_row["Configuration"] = default_configs[-1]
             new_row["flag_convert_meas_csv"] = ''
             df = pd.concat([df, pd.DataFrame([new_row])], ignore_index=True)  # Append the new row to the DataFrame
             if self.verbose: print(f'NOTE: No measurement data for event {event.GeneralParameters.name} found.')
 
         # If the parent folder is not present, make it and save the dataframe as the viewer setup csv
         make_folder_if_not_existing(os.path.dirname(path_output_viewer_csv))
         df.to_csv(path_output_viewer_csv, index=False)
@@ -450,15 +457,15 @@
             'QuenchProtection.CLIQ.U0': 'Quench_Protection.CLIQ.U0',
             'QuenchProtection.CLIQ.C': 'Quench_Protection.CLIQ.C',
             'QuenchProtection.CLIQ.R': 'Quench_Protection.CLIQ.R',
             'QuenchProtection.CLIQ.L': 'Quench_Protection.CLIQ.L',
         }
         for old_name, new_name in dict_param.items():
             if rgetattr(event, old_name) and not math.isnan(rgetattr(event, old_name)):
-                    event_dict[new_name] = rgetattr(event, old_name)
+                event_dict[new_name] = rgetattr(event, old_name)
             if not new_name in event_dict:
                 event_dict[new_name] = ''
 
         # add current_polarities_CLIQ if provided
         if current_polarities_CLIQ:
             event_dict['Quench_Protection.CLIQ.current_direction'] = current_polarities_CLIQ
         else:
@@ -634,14 +641,18 @@
             'Temperature [K]': 'GeneralParameters.initial_temperature',
         }
 
         for param in dict_params:
             if param in event_info:
                 rsetattr(new_event, dict_params[param], event_info[param])
 
+        if not new_event.GeneralParameters.name:
+            keys_for_name = [key for key, value in dict_params.items() if value == 'GeneralParameters.name']
+            raise Exception(f'No file name for the test could be found in the csv file. A column with one of the following keys should have a valid name: {keys_for_name}.')
+
         return list(dict_params.keys())
 
     def __read_powering(self, event_info: pd.Series, new_event: DataEventMagnet):
         '''
         Function to set Powering keys
 
         :param event_info: Series of parameters
@@ -762,27 +773,28 @@
         if rel_quench_heater_trip_threshold is not None:
             for QH_name, QH in dict_QH.items():
                 # Calculate the time constant for the discharge
                 tau = QH.C * QH.R_total
                 # Calculate the corrected voltage based on the relative trip threshold
                 U_corrected = QH.U0 / rel_quench_heater_trip_threshold
                 # calculate time difference: U_meas(t_meas)/U_correct(t_corrected) = rel_quench_heater_trip_threshold
-                delta_t = math.log(U_corrected / QH.U0) * tau  # delta_t = t_meas-t_corrected  #TODO: what if this is smaller then step size of measurement
+                delta_t = math.log(U_corrected / QH.U0) * tau  # delta_t = t_meas-t_corrected
                 # Update the voltage of the quench heater and the trigger time with the corrected values
+                if self.verbose: print(f'Corrected QuenchHeater trigger time from {QH.t_trigger} to {QH.t_trigger - delta_t} and U0 from {QH.U0} to {U_corrected}.')
                 QH.t_trigger = QH.t_trigger - delta_t
                 QH.U0 = U_corrected
-            del U_corrected, delta_t
+            del U_corrected, delta_t, QH_name, QH
 
         # Add QH circuit dictionary to the event data
         rsetattr(new_event, 'QuenchProtection.Quench_Heaters', dict_QH)
 
         return column_names + ['QH Name']
 
 
-    def __read_signals_of_configs(self, default_configs, path_config_file):
+    def __read_signals_of_configs(self, default_configs, path_config_file: str):
         '''
             Reads signal data from a YAML configuration file and returns a dictionary of the unique signals for each specified configuration.
 
             Args:
                 default_configs (str or list): Names of the configurations to retrieve signal data for.
                 path_config_file (str): Path to the YAML configuration file.
 
@@ -803,166 +815,196 @@
         for config in default_configs:
             # check if specified config name is valid
             if config not in dict_configs['ConfigurationList'].keys():
                 raise Exception(f'The configuration {config} is not defined in the configurations file {path_config_file}.')
             # Loop through each signal in the 'SignalList' for the configuration
             for signal in dict_configs['ConfigurationList'][config]['SignalList'].values():
                 # both 'meas_signals_to_add_x' and 'meas_signals_to_add_y' have to be present in the measurement file
-                dict_configs_with_signals[config].extend(signal['meas_signals_to_add_x'])
-                dict_configs_with_signals[config].extend(signal['meas_signals_to_add_y'])
+                if 'meas_signals_to_add_x' in signal:
+                    dict_configs_with_signals[config].extend(signal['meas_signals_to_add_x'])
+                if 'meas_signals_to_add_y' in signal:
+                    dict_configs_with_signals[config].extend(signal['meas_signals_to_add_y'])
             # only store the unique values
             dict_configs_with_signals[config] = list(set(dict_configs_with_signals[config]))
         del yaml_string, dict_configs
 
+        # check if config has been read correctly (at least one configuration has a list of measurement names)
+        if all(value == [] for value in dict_configs_with_signals.values()):
+            raise Exception(f'No valid configuration found in configurations file {path_config_file}')
+
         return dict_configs_with_signals
     
 
-    def remove_frequency_suffix(self, name_file_found_csv):
-        """
-            Removes a frequency suffix ("_MF", "_HF", "_LF") from the end of a file name if existing
-        """
-        for suffix in ["_MF", "_HF", "_LF"]:
-            if name_file_found_csv.endswith(suffix):
-                name_file_found_csv = name_file_found_csv[:-len(suffix)]
-        return name_file_found_csv
+def remove_frequency_suffix(name_file_found_csv):
+    """
+        Removes a frequency suffix ("_MF", "_HF", "_LF") from the end of a file name if existing
+    """
+    for suffix in ["_MF", "_HF", "_LF"]:
+        if name_file_found_csv.endswith(suffix):
+            name_file_found_csv = name_file_found_csv[:-len(suffix)]
+    return name_file_found_csv
 
 
-    def search_file_in_subfolders(self, list_integer_sequences, path_to_parent_dir, datatype):
-        """
-            Search for a file in subfolders of a given directory.
+def search_file_in_subfolders(timestamp, path_to_parent_dir, datatype):
+    """
+        Search for a file in subfolders of a given directory.
 
-            Parameters:
-            - list_integer_sequences (list): A list of integer sequences to search for in the file names.
-            - path_to_parent_dir (str): The path to the parent directory.
-            - datatype (str): The file extension to search for.
+        Parameters:
+        - timestamp (str): A string of integer sequences (timestamp) to search for in the file names.
+        - path_to_parent_dir (str): The path to the parent directory.
+        - datatype (str): The file extension to search for.
 
-            Returns:
-            - Tuple: A tuple containing the names of the subfolders the file was found in, and the name of the file without the extension.
-              If the file is not found, both elements will be empty
-        """
-        # check for datatypes
-        supported_filetypes = ['.tdms', '.csv']
-        if datatype not in supported_filetypes:
-            raise Exception(f'Datatype {datatype} not supported for measurement files.')
-
-        # initialize lists to store subfolder names and file names
-        list_campaign_names, list_file_names = [], []
-
-        # get the names of all subfolders
-        subfolders = [os.path.basename(f.path) for f in os.scandir(path_to_parent_dir) if f.is_dir()]
-
-        # loop through all subfolders and search for file with given integer sequences and datatype
-        for subfolder in subfolders:
-            # list with all filesnames in the subfolder
-            list_files = os.listdir(os.path.join(path_to_parent_dir, subfolder))
-            for file in list_files:
-                # check for every file if it has given datatype and contains the integer sequences in its name
-                if file.endswith(datatype) and (len(list_integer_sequences) > 0) and all([sequence in file for sequence in list_integer_sequences]):
-                    list_campaign_names.append(subfolder) # add subfolder name to list of subfolders where file was found
-                    list_file_names.append(file.split(datatype)[0]) # add file name without extension to list of file names found
-
-        # evaluate names of files that have been found
-        campaign_name, name_file_found = None, None
-        if datatype is supported_filetypes[0]: # for tdms files only one file should be found
-            if len(list_campaign_names) == 1:
-                campaign_name, name_file_found = list_campaign_names[0], list_file_names[0]
-            elif len(list_campaign_names) > 1:
-                raise Exception(f'More then one then one tdms file with the specified timestamp found: {list_file_names}')
-        # for csv files a timestamp can be found multiple times (e.g. meas2210051743_MF.csv and meas2210051743_HF.csv)
-        elif datatype is supported_filetypes[1]:
-            list_file_names = [self.remove_frequency_suffix(name) for name in list_file_names]
-            if len(list_campaign_names) == 1:
+        Returns:
+        - Tuple: A tuple containing the names of the subfolders the file was found in, and the name of the file without the extension.
+          If the file is not found, both elements will be empty
+    """
+    # if no path for the folder to search in is provided, don't search and return None
+    if path_to_parent_dir == '':
+        return None, None
+
+    # check for datatypes
+    supported_filetypes = ['.tdms', '.csv']
+    if datatype not in supported_filetypes:
+        raise Exception(f'Datatype {datatype} not supported for measurement files.')
+
+    # initialize lists to store subfolder names and file names
+    list_campaign_names, list_file_names = [], []
+
+    # get the names of all subfolders
+    subfolders = [os.path.basename(f.path) for f in os.scandir(path_to_parent_dir) if f.is_dir()]
+
+    # loop through all subfolders and search for file with given integer sequences and datatype
+    for subfolder in subfolders:
+        # list with all filesnames in the subfolder
+        list_files = os.listdir(os.path.join(path_to_parent_dir, subfolder))
+        for file in list_files:
+            # check for every file if it has given datatype and contains the integer sequences in its name
+            if file.endswith(datatype) and timestamp in file:
+                list_campaign_names.append(subfolder)  # add subfolder name to list of subfolders where file was found
+                list_file_names.append(
+                    file.split(datatype)[0])  # add file name without extension to list of file names found
+
+    # evaluate names of files that have been found
+    campaign_name, name_file_found = None, None
+    # for tdms files only one file should be found
+    if datatype == supported_filetypes[0]:
+        if len(list_campaign_names) == 1:
+            campaign_name, name_file_found = list_campaign_names[0], list_file_names[0]
+        elif len(list_campaign_names) > 1:
+            raise Exception(f'More then one then one tdms file with the specified timestamp found: {list_file_names}')
+    # for csv files a timestamp can be found multiple times (e.g. meas2210051743_MF.csv and meas2210051743_HF.csv)
+    elif datatype == supported_filetypes[1]:
+        list_file_names = [remove_frequency_suffix(name) for name in list_file_names]
+        if len(list_campaign_names) == 1:
+            campaign_name, name_file_found = list_campaign_names[0], list_file_names[0]
+        elif len(list_campaign_names) > 1:
+            # check if names without the frequency suffix are the same
+            if all(element == list_file_names[0] for element in list_file_names):
                 campaign_name, name_file_found = list_campaign_names[0], list_file_names[0]
-            elif len(list_campaign_names) > 1:
-                # check if names without the frequency suffix are the same
-                if all(element == list_file_names[0] for element in list_file_names):
-                    campaign_name, name_file_found = list_campaign_names[0], list_file_names[0]
-                else:
-                    raise Exception(f'More then one then one csv file with the specified timestamp found: {list_file_names}')
+            else:
+                raise Exception(
+                    f'More then one then one csv file with the specified timestamp found: {list_file_names}')
 
-        # return tuple with lists of subfolder and file names
-        return campaign_name, name_file_found
-    
-    def get_config_tdms(self, path_tdms_files, campaign_name_tdms, filename_tdms, dict_configs_with_signals):
-        """
-            Read the TDMS file specified by the `path_tdms_files`, `campaign_name_tdms` and `filename_tdms` arguments
-            using the ParserTdms class to make a list of all the measurement signal names in the TDMS file
-            the function returns the most advanced configuration by using the get_most_advanced_viewer_config function
-        
-            Args:
-            - path_tdms_files: str representing the path to the TDMS folder
-            - campaign_name_tdms: str representing the name of the campaign
-            - filename_tdms: str representing the name of the TDMS file to be found#
-            - dict_configs_with_signals: dict holding all configurations (keys) and their needed signals (values)
-        
-            Returns:
-            - most advanced viewer configuration
-        """
-        # define full path
-        full_path = Path(os.path.join(path_tdms_files, campaign_name_tdms, filename_tdms + '.tdms')).resolve()
-        
-        # init list 
-        list_meas_signals = []
-        
-        # for each group (LF, MF, HF) there can be different signals, dict keys are groups and values respective signals
-        dict_meas_signals_with_groups = ParserTdms(full_path).getNames()[2]
-        
-        # loop through the dict
-        for group, signal_list in dict_meas_signals_with_groups.items():
-            # append the group name with the signal name and a . in between, as in the tdms files
-            for signal in signal_list:
-                list_meas_signals.append(group + '.' + signal)
-            # the time is not in signal list from the .getNames() function and has to be added here
-            list_meas_signals.append(group + '.Time [s]')
+    # return tuple with lists of subfolder and file names
+    return campaign_name, name_file_found
 
-        return self.get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, filename_tdms)
 
+def get_config_tdms(path_tdms_files, campaign_name, file_name, dict_configs_with_signals, verbose):
+    """
+        Read the TDMS file specified by the `path_tdms_files`, `campaign_name` and `file_name` arguments
+        using the ParserTdms class to make a list of all the measurement signal names present in the TDMS file
+        the function returns the most advanced configuration by using the get_most_advanced_viewer_config function
+
+        Args:
+        - path_tdms_files: str representing the path to the TDMS folder
+        - campaign_name: str representing the name of the campaign
+        - file_name: str representing the name of the TDMS file to be found#
+        - dict_configs_with_signals: dict holding all configurations (keys) and their needed signals (values)
 
-    def get_config_csv(self, campaign_name_csv, name_file_found_csv, dict_configs_with_signals):
-        """
-            this function reads all the signals present in a csv measurement file and returns the most advanced
-            configuration by using the get_most_advanced_viewer_config function
-        """
-        # init list
-        list_meas_signals = []
+        Returns:
+        - most advanced viewer configuration
+    """
+    # define full path
+    full_path = Path(os.path.join(path_tdms_files, campaign_name, file_name + '.tdms')).resolve()
+
+    # init list
+    list_meas_signals = []
+
+    # for each group (LF, MF, HF) there can be different signals, dict keys are groups and values respective signals
+    dict_meas_signals_with_groups = ParserTdms(full_path).getNames()[2]
+
+    # loop through the dict
+    for group, signal_list in dict_meas_signals_with_groups.items():
+        # append the group name with the signal name and a . in between, as in the tdms files
+        for signal in signal_list:
+            list_meas_signals.append(group + '.' + signal)
+        # the time is not in signal list from the .getNames() function and has to be added here
+        list_meas_signals.append(group + '.Time [s]')
+
+    return get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, file_name, verbose=verbose)
+
+
+def get_config_csv(path_parent_dir, campaign_name, file_name, dict_configs_with_signals, verbose):
+    """
+        Read all the signals present in a csv measurement file and return the most advanced configuration
+        by using the get_most_advanced_viewer_config function.
+
+        Parameters:
+            path_parent_dir (str): path to the folder with all the campaigns in it
+            campaign_name (str): The name of the campaign to look for csv files
+            file_name (str): The name of the csv file
+            dict_configs_with_signals (dict): A dictionary containing the configurations with signals
 
-        for campaign, name in zip(campaign_name_csv, name_file_found_csv):
-            full_path = Path(os.path.join(campaign, name + '.csv')).resolve()  # TODO falsch
+        Returns:
+            dict: A dictionary representing the most advanced configuration
+    """
+    # Initialization of list to store measurement signals
+    list_meas_signals = []
+
+    # Loop over campaign names and file names to get full path of csv file and extract signal names
+    for suffix in ["MF", "HF", "LF"]:
+        full_path = Path(os.path.join(path_parent_dir, campaign_name, file_name + '_' + suffix + '.csv')).resolve()
+        if os.path.isfile(full_path):
+            # read all the names of the columns (=names of the present signals)
             csv_header = pd.read_csv(full_path, nrows=1).columns.tolist()
-            for suffix in ["MF", "HF", "LF"]:
-                if name_file_found_csv.endswith(suffix):
-                    csv_header = [suffix + '.' + headername for headername in csv_header]
 
-            list_meas_signals.append(csv_header)
+            # Append the suffix to the header names
+            csv_header = [suffix + '.' + header_name for header_name in csv_header]
 
-        return self.get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, name_file_found_csv)
+            # Append the signal names to the list
+            list_meas_signals = list_meas_signals + csv_header
 
+    # Call the function to get the most advanced configuration
+    return get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, file_name, verbose=verbose)
 
-    def get_most_advanced_viewer_config(self, dict_configs_with_signals, list_meas_signals, filename):
-        """
-            Return the configuration name of the first dict where all signal names in its list of values are present in `list_meas_signals`.
 
-            Parameters:
-                dict_configs_with_signals (dict): A dictionary with configuration names as keys and lists of signal names as values - Ordered from most advanced to least advanced
-                list_meas_signals (list): A list of signal names found in tdms/csv measurement files
-                filename (str): name of the measurement file
+def get_most_advanced_viewer_config(dict_configs_with_signals, list_meas_signals, filename, verbose):
+    """
+        Return the configuration name of the first dict where all signal names in its list of values are present in `list_meas_signals`.
 
-            Returns:
-                str: most advanced viewer configuration
-        """
+        Parameters:
+            dict_configs_with_signals (dict): A dictionary with configuration names as keys and lists of signal names as values - Ordered from most advanced to least advanced
+            list_meas_signals (list): A list of signal names found in tdms/csv measurement files
+            filename (str): name of the measurement file
 
-        # check for the configurations if all the needed signals are present and return the most advanced one
-        for config_name, signal_list in dict_configs_with_signals.items():
-            # check whether all the signal names in the configuration's list are present in the measurement signal list
-            if set(signal_list).issubset(set(list_meas_signals)):
-                # if all the signal names are present, return the configuration name
-                if self.verbose: print(f'{filename}: configuration {config_name} is used.')
-                return config_name
-            else:
-                # print missing signals and skip to the next configuration
-                missing_signals = set(signal_list).difference(set(list_meas_signals))
-                if self.verbose: print(f'{filename}: configuration {config_name} skipped. Could not find {missing_signals}')
+        Returns:
+            str: most advanced viewer configuration
+    """
 
-        # if no valid configuration could be found, raise an exception with an error message indicating the missing signals for the simplest configuration
+    # check for the configurations if all the needed signals are present and return the most advanced one
+    for config_name, signal_list in dict_configs_with_signals.items():
+        # check whether all the signal names in the configuration's list are present in the measurement signal list
+        if set(signal_list).issubset(set(list_meas_signals)):
+            # if all the signal names are present, return the configuration name
+            if verbose: print(f'{filename}: configuration {config_name} is used.')
+            return config_name
+        else:
+            # print missing signals and skip to the next configuration
+            missing_signals = set(signal_list).difference(set(list_meas_signals))
+            if verbose: print(f'{filename}: configuration {config_name} skipped. Could not find {missing_signals}')
+
+    # if no valid configuration could be found, raise an exception with an error message indicating the missing signals for the simplest configuration
+    if config_name and missing_signals:
         raise Exception(f'No valid configuration could be found for measurement {filename}.\n'
                         f'Missing signals for simplest configuration {config_name}: {missing_signals}')
-
+    else:
+        raise Exception(f'No valid configuration could be found for measurement {filename}.')
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/parsims/ParsimSweep.py` & `steam_sdk-2023.4.0/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/plotters/PlotterModel.py` & `steam_sdk-2023.4.0/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/plotters/PlotterParametric.py` & `steam_sdk-2023.4.0/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/plotters/PlotterRoxie.py` & `steam_sdk-2023.4.0/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/plotters/PlotterSIGMA.py` & `steam_sdk-2023.4.0/steam_sdk/plotters/PlotterSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/postprocs/PostprocsMetrics.py` & `steam_sdk-2023.4.0/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/utils/ModifyModelData.py` & `steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import os
 from pathlib import Path
 import yaml
-import ruamel.yaml
 from steam_sdk.data.DataModelMagnet import DataModelMagnet
 from steam_sdk.parsers.ParserYAML import dict_to_yaml
 
 if __name__ == "__main__":
     # path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'C:\\Users\emm\cernbox\SWAN_projects\steam_models\magnets')
     path_models = Path.joinpath(Path(__file__).parent.parent.parent, r'E:\Python\steam_models\magnets')
     path_models = Path.joinpath(Path(__file__).parent.parent.parent, 'tests/builders/model_library/magnets')
     models = [x.parts[-1] for x in Path(path_models).iterdir() if x.is_dir()]
     #models = ['MCBRD']
 
-    for mm in ['MB_2COILS']:#models:
+    for mm in models:
         # Read file
         file_model_data = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '.yaml')
         if os.path.isfile(file_model_data):
             # Load yaml keys into DataAnalysis dataclass
             with open(file_model_data, "r") as stream:
-                dictionary_yaml = ruamel.yaml.round_trip_load(stream)
-            with open(file_model_data, "r") as stream:
-                dictionary_yaml_without_comments = yaml.safe_load(stream)
-            model_data = DataModelMagnet(**dictionary_yaml)  # TODO here we're ignoring any comment present in the file and forgetting about them
-            model_data_without_comments = DataModelMagnet(**dictionary_yaml_without_comments)  # TODO here we're ignoring any comment present in the file and forgetting about them
+                dictionary_yaml = yaml.safe_load(stream)
+                model_data = DataModelMagnet(**dictionary_yaml)  # TODO here we're ignoring any comment present in the file and forgetting about them
             print(f'Read file: {file_model_data}')
 
             # Note: Obsolete keys in yaml file will automatically be deleted
 
             # Note: New keys added to DataModelMagnet will automatically be added to the yaml file (UNLESS A VALUE IS ASSIGNED BELOW, THEIR VALUES WILL BE INITIALIZED TO DEFAULT)
 
             # Example to assign value to new keys in model data
@@ -47,18 +43,16 @@
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.alphaDEG_ht = dictionary_yaml['CoilWindings']['multipole']['alphaDEG_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.rotation_ht = dictionary_yaml['CoilWindings']['multipole']['rotation_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirror_ht = dictionary_yaml['CoilWindings']['multipole']['mirror_ht']
             # model_data.Options_LEDET.conductor_geometry_used_for_ISCL.mirrorY_ht = dictionary_yaml['CoilWindings']['multipole']['mirrorY_ht']
 
             # Check and reformat the key values
             model_data = DataModelMagnet(**model_data.dict())
-            model_data_without_comments = DataModelMagnet(**model_data_without_comments.dict())
 
             # Write file
             # file_model_data_output = Path.joinpath(path_models, mm, 'input', 'modelData_' + mm + '_MODIFIED.yaml')  # use this line if you wish to test the results of this script
             file_model_data_output = file_model_data  # use this line if you wish to really update all yaml input files
             all_data_dict = {**model_data.dict()}
-            all_data_dict_without_comments = {**model_data_without_comments.dict()}
-            dict_to_yaml(all_data_dict, file_model_data_output, list_exceptions=['Conductors'], with_comments=True)
+            dict_to_yaml(all_data_dict, file_model_data_output, list_exceptions=['Conductors'])
             print(f'Written file: {file_model_data_output}')
         else:
             print(f'WARNING: File {file_model_data} not found.')
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/utils/ModifyModelDataconductor.py` & `steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/utils/clean_NaN_from_signal.py` & `steam_sdk-2023.4.0/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/utils/compare_two_parameters.py` & `steam_sdk-2023.4.0/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/utils/misc.py` & `steam_sdk-2023.4.0/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/utils/tic_toc.py` & `steam_sdk-2023.4.0/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/viewers/Viewer.py` & `steam_sdk-2023.4.0/steam_sdk/viewers/Viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from pathlib import Path
 from typing import List, Union
 import numpy as np
 import pandas as pd
 import yaml
+import time
 
 from steam_sdk.data.DataSignal import DataSignal
 
 import matplotlib
 import matplotlib.pyplot as plt
 
 from steam_sdk.parsers.ParserMat import get_signals_from_mat
@@ -71,15 +72,15 @@
         self.dict_configs = {}  # this dictionary will contain all configurations, which define which measured and simulated signals are acquired
         self.dict_data    = {}  # this dictionary will contain all event data. Each event includes a combination of measured data, simulated data, or both, including multipliers
         self.dict_figures = {}  # this dictionary will contain as many keys as the events, and each key will contain a list with the paths of all generated figures
 
         # Initialize by reading the input file
         if self.verbose:
             print(f'Reading file {file_name_transients}')
-            data_events_df = pd.read_csv(file_name_transients)  # read file into a dataframe
+        data_events_df = pd.read_csv(file_name_transients)  # read file into a dataframe
         self.dict_events = dict(zip(data_events_df, data_events_df.values.T))  # convert dataframe to dictionary
         if self.verbose:
             print('Read dictionary:')
             for key, value in self.dict_events.items():
                 print(f'{key}: {value}')
         n_events = len(data_events_df.index)
 
@@ -156,15 +157,15 @@
 
         if verbose: print('### Check whether measurement files are required to be converted to .csv files. ###')
 
         for t in list_events:
             # get flag indicating whether the measurement file should be converted to csv & check if it is valid
             flag_convert_meas_csv = dict_events['flag_convert_meas_csv'][t-1]
             if flag_convert_meas_csv not in [0, 1, 2] and not pd.isna(flag_convert_meas_csv):
-                raise Exception(f'Invalid parameter. flag_convert_meas_csv can either be 0, 1, 2 or empty in Viewer input file.')
+                raise Exception(f'Invalid parameter. flag_convert_meas_csv can only be 0, 1, 2 or empty in Viewer input file, but it was set to {flag_convert_meas_csv}.')
 
             # if flag_convert_meas_csv=0, the file of this event will not be converted: go to the next event
             if flag_convert_meas_csv == 0 or isNaN(flag_convert_meas_csv):
                 if verbose: print(f'Row {t}: flag_convert_meas_csv={flag_convert_meas_csv}: Measurement file not converted to csv.')
                 continue
 
             # Identify measurement file
@@ -340,15 +341,14 @@
                 sim_multipliers_x    = signal.sim_multipliers_x
                 sim_multipliers_y    = signal.sim_multipliers_y
                 sim_offsets_x        = signal.sim_offsets_x
                 sim_offsets_y        = signal.sim_offsets_y
                 # Calculate the sum of signals after applying multipliers (first) and offsets (after)
                 combined_signal_sim_x = self._multipliers_offsets_sum(df_sim_data, sim_signals_to_add_x, sim_multipliers_x, sim_offsets_x, data_type='dataframe')
                 combined_signal_sim_y = self._multipliers_offsets_sum(df_sim_data, sim_signals_to_add_y, sim_multipliers_y, sim_offsets_y, data_type='dataframe')
-                print(' ----- ' + str(df_sim_data.keys()))
 
                 # Assign signals to the main dictionary
                 meas_label = signal.meas_label
                 sim_label  = signal.sim_label
                 if (len(temp_dict_meas) > 0) and (len(combined_signal_meas_x) > 0) and (len(combined_signal_meas_y) > 0):
                     self.dict_data[event_label][meas_label] = {}
                     self.dict_data[event_label][meas_label]['x_meas'] = combined_signal_meas_x
@@ -357,41 +357,52 @@
                     self.dict_data[event_label][sim_label] = {}
                     self.dict_data[event_label][sim_label]['x_sim']  = combined_signal_sim_x
                     self.dict_data[event_label][sim_label]['y_sim']  = combined_signal_sim_y
 
 
                 # Plot current signal (meas, or sim, or both) of the current event
                 path_output_figures = Path(dict_events['path_output_figures'][t-1]).resolve()
+                fig_options = {
+                    'fig_title': signal.fig_title,
+                    'fig_label_x': signal.fig_label_x,
+                    'fig_label_y': signal.fig_label_y,
+                    'fig_range_x': signal.fig_range_x,
+                    'fig_range_y': signal.fig_range_y,
+                }
                 if self.flag_save_figures:
                     fig_name    = sig_name
                     figure_name = f'{event_label}_{fig_name}'  # note that the file extension is missing
                     full_path_figure_to_save = os.path.join(path_output_figures, event_label, figure_name)  # note that the file extension is missing
                     if verbose: print(f'Figure {full_path_figure_to_save} will be saved.')
-                    fig_options = {
-                        'fig_title':   signal.fig_title,
-                        'fig_label_x': signal.fig_label_x,
-                        'fig_label_y': signal.fig_label_y,
-                        'fig_range_x': signal.fig_range_x,
-                        'fig_range_y': signal.fig_range_y,
-                    }
-                    self.dict_figures[event_label].append(figure_name)
-
+                    # # calculate x lim: display only overlapping x values
+                    # x_lim = [max(combined_signal_sim_x.iloc[0], combined_signal_meas_x.iloc[0]), min(combined_signal_sim_x.iloc[-1], combined_signal_meas_x.iloc[-1])]
+                    # # calculate y lim: smallest and largest value with 10% spacing up and down
+                    # y_lim = [1.1*min(combined_signal_sim_y.min(), combined_signal_meas_y.min()), 1.1*max(combined_signal_sim_y.max(), combined_signal_meas_y.max())]
+                    self.dict_figures[event_label].append(figure_name)  # make this a list of figures
                 else:
                     full_path_figure_to_save = None
                 self.plot_signal(event_label, meas_label, sim_label, fig_options, self.flag_display, full_path_figure_to_save, figure_types=figure_types)
 
         if path_output_html_report:
             if verbose:
                 print('Html report generation started.')
             self.make_html_report(path_output_html_report)  # TODO Known issue: in order for the figures to be displayed correctly, they all need to be in subfolders of the same folder, and the path of the html file needs correspond to it
 
         if path_output_pdf_report:
             if verbose:
                 print('Pdf report generation started.')
+
+            # measure the time it takes to make the report
+            start_time = time.time()
             self.make_pdf_report(path_output_pdf_report)
+            end_time = time.time()
+
+            if self.verbose:
+                time_taken = (end_time - start_time) / 60  # Calculate the time taken and convert from sec to min
+                print(f"It took {time_taken:.2f} min to create PDF report.")  # Print the time taken with 2 decimal places
         ## TODO Analyze metrics
 
 
     def plot_signal(self, event_label: str, meas_label: str, sim_label: str, fig_options: dict, flag_display: bool = True, full_path_figure_to_save: str = None, figure_types: Union[List[str], str] = 'png'):
         '''
         # Plot a selected signal (meas, or sim, or both) of a selected event
         :param event_label: Name identifying the event to plot
@@ -538,17 +549,19 @@
 
 
     def make_pdf_report(self, path_pdf_report: str = None, default_width: float = None, default_height: float = None):
         '''
         Generate a pdf report using the generated figures
         :return:
         '''
+
         # If output folder is missing, make it
         make_folder_if_not_existing(os.path.dirname(path_pdf_report))
 
+        # svg not used any more due to long pdf loading times (functionality working for small pdf files)
         order_of_preference_figure_type = ['png']  # hard-coded
 
         # Start the pdf file
         ppdf = ParserPdf(path_pdf_report)
 
         # Loop through all events
         for t in self.list_events:
@@ -557,18 +570,24 @@
             # Add figures
             for fig_name in self.dict_figures[event_label]:
                 current_path_output_figure = Path(self.dict_events['path_output_figures'][t-1]).resolve()
                 for d_type in order_of_preference_figure_type:
                     if os.path.isfile(os.path.join(current_path_output_figure, event_label, f'{fig_name}.{d_type}')):  # check if the figures exist
                         fig_path = os.path.join(current_path_output_figure, event_label, f'{fig_name}.{d_type}')  # Write relative path
                         break
-                ppdf.add_image(fig_path)
+                ppdf.add_header(event_label, level=2)
+                ppdf.add_header(fig_name, level=3)
+                if d_type == 'png': ppdf.add_image(fig_path)
+                elif d_type == 'svg': ppdf.add_svg_image(fig_path)
+                else: raise Exception(f'{d_type} in no valid datatype.')
                 ppdf.add_page_break()
+            if self.verbose: print(f'Collecting figures for pdf Report: {round(t/len(self.list_events)*100, 2)}% done')
 
         # Write pdf
+        if self.verbose: print('Building PDF report.')
         ppdf.generate_pdf()
 
         if self.verbose:
             print(f'Report file {os.path.abspath(path_pdf_report)} generated.')
 
 
     # Helper functions
```

### Comparing `steam_sdk-2023.2.3/steam_sdk/viewers/ViewerMeas.py` & `steam_sdk-2023.4.0/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/viewers/ViewerSim.py` & `steam_sdk-2023.4.0/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk/wrappers/wrapper_yaml.py` & `steam_sdk-2023.4.0/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.2.3/steam_sdk.egg-info/PKG-INFO` & `steam_sdk-2023.4.0/steam_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.2.3
+Version: 2023.4.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,API,SDK
+Keywords: SDK,CERN,API,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
 
@@ -24,14 +24,17 @@
 Important: Before running the tests, make sure to set up your user settings.
 
 * The settings file must be located in the subfolder steam_sdk\tests
 * The file must be called settings.username.yaml, where username is your user name in the machine on which you are running the analysis.
 It is recommended to start by making a copy of the example settings.SYSTEM.yaml file.
 * Note: It is not recommended to change other settings files within this project (some files are generated by the software).
 
+# Documentation
+https://steam-sdk.docs.cern.ch/
+
 # Installation
 
 ## Released version:
 pip install steam-sdk
 
 ## Test version:
 pip install -i https://test.pypi.org/simple/ steam-sdk
```

### Comparing `steam_sdk-2023.2.3/steam_sdk.egg-info/SOURCES.txt` & `steam_sdk-2023.4.0/steam_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+.gitignore
+.gitlab-ci.yml
 MANIFEST.in
+Readme.md
+mkdocs.yaml
+requirements.txt
 setup.py
 steam_sdk/__init__.py
 steam_sdk.egg-info/PKG-INFO
 steam_sdk.egg-info/SOURCES.txt
 steam_sdk.egg-info/dependency_links.txt
 steam_sdk.egg-info/requires.txt
 steam_sdk.egg-info/top_level.txt
@@ -34,28 +39,35 @@
 steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
 steam_sdk/builders/BuilderFiQuS.py
 steam_sdk/builders/BuilderLEDET.py
 steam_sdk/builders/BuilderModel.py
 steam_sdk/builders/BuilderProteCCT.py
 steam_sdk/builders/BuilderPyBBQ.py
 steam_sdk/builders/BuilderSIGMA.py
+steam_sdk/builders/Readme.md
 steam_sdk/builders/SelfMutualInductanceCalculation.py
 steam_sdk/builders/Solenoids.py
 steam_sdk/builders/__init__.py
 steam_sdk/builders/geometricFunctions.py
 steam_sdk/configs/__init__.py
+steam_sdk/configs/plotters/Readme.md
 steam_sdk/configs/plotters/__init__.py
+steam_sdk/configs/tools_defaults/Readme.md
 steam_sdk/configs/tools_defaults/ToolDefaultReader.py
 steam_sdk/configs/tools_defaults/__init__.py
 steam_sdk/configs/tools_defaults/LEDET/__init__.py
+steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
 steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+steam_sdk/configs/users/Readme.md
+steam_sdk/cosims/Readme.md
 steam_sdk/cosims/__init__.py
 steam_sdk/data/DataAnalysis.py
 steam_sdk/data/DataConductor.py
 steam_sdk/data/DataDakota.py
+steam_sdk/data/DataEventCircuit.py
 steam_sdk/data/DataEventMagnet.py
 steam_sdk/data/DataFiQuS.py
 steam_sdk/data/DataLEDET.py
 steam_sdk/data/DataModelCircuit.py
 steam_sdk/data/DataModelConductor.py
 steam_sdk/data/DataModelMagnet.py
 steam_sdk/data/DataParsimConductor.py
@@ -64,59 +76,72 @@
 steam_sdk/data/DataPyBBQ.py
 steam_sdk/data/DataRoxieParser.py
 steam_sdk/data/DataSettings.py
 steam_sdk/data/DataSignal.py
 steam_sdk/data/DictionaryLEDET.py
 steam_sdk/data/DictionaryProteCCT.py
 steam_sdk/data/DictionaryPyBBQ.py
+steam_sdk/data/Readme.md
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
+steam_sdk/drivers/Readme.md
 steam_sdk/drivers/__init__.py
+steam_sdk/drivers/temp/postLEDET.py
+steam_sdk/drivers/temp/runLEDET.py
+steam_sdk/drivers/temp/simLEDET.py
 steam_sdk/parsers/CSD_Reader.py
+steam_sdk/parsers/ParserCOMSOLToTxt.py
 steam_sdk/parsers/ParserCond2d.py
 steam_sdk/parsers/ParserCsd.py
 steam_sdk/parsers/ParserCsv.py
 steam_sdk/parsers/ParserDakota.py
+steam_sdk/parsers/ParserDatToCsv.py
 steam_sdk/parsers/ParserExcel.py
 steam_sdk/parsers/ParserFiQuS.py
 steam_sdk/parsers/ParserLEDET.py
 steam_sdk/parsers/ParserMap2d.py
 steam_sdk/parsers/ParserMat.py
 steam_sdk/parsers/ParserPSPICE.py
 steam_sdk/parsers/ParserPdf.py
 steam_sdk/parsers/ParserProteCCT.py
 steam_sdk/parsers/ParserProtePyBBQ.py
 steam_sdk/parsers/ParserRoxie.py
 steam_sdk/parsers/ParserTdms.py
 steam_sdk/parsers/ParserXYCE.py
 steam_sdk/parsers/ParserYAML.py
+steam_sdk/parsers/Readme.md
 steam_sdk/parsers/__init__.py
 steam_sdk/parsers/dict_to_in.py
+steam_sdk/parsers/templates/template_Dakota.in
 steam_sdk/parsims/ParsimConductor.py
 steam_sdk/parsims/ParsimDakota.py
+steam_sdk/parsims/ParsimEventCircuit.py
 steam_sdk/parsims/ParsimEventMagnet.py
 steam_sdk/parsims/ParsimSweep.py
+steam_sdk/parsims/Readme.md
 steam_sdk/parsims/__init__.py
 steam_sdk/plotters/PlotterModel.py
 steam_sdk/plotters/PlotterParametric.py
 steam_sdk/plotters/PlotterRoxie.py
 steam_sdk/plotters/PlotterSIGMA.py
+steam_sdk/plotters/Readme.md
 steam_sdk/plotters/__init__.py
 steam_sdk/postprocs/PostprocsMetrics.py
 steam_sdk/postprocs/__init__.py
+steam_sdk/utils/MTF_reading_functions.py
 steam_sdk/utils/ModifyModelData.py
 steam_sdk/utils/ModifyModelDataMagnet.py
 steam_sdk/utils/ModifyModelDataconductor.py
 steam_sdk/utils/NumpyEncoder.py
 steam_sdk/utils/__init__.py
 steam_sdk/utils/clean_NaN_from_signal.py
 steam_sdk/utils/compare_two_parameters.py
@@ -124,20 +149,19 @@
 steam_sdk/utils/make_folder_if_not_existing.py
 steam_sdk/utils/misc.py
 steam_sdk/utils/rgetattr.py
 steam_sdk/utils/rhasattr.py
 steam_sdk/utils/sgetattr.py
 steam_sdk/utils/tic_toc.py
 steam_sdk/utils/unique.py
+steam_sdk/utils/utils_PC.py
 steam_sdk/viewers/Viewer.py
 steam_sdk/viewers/ViewerMeas.py
 steam_sdk/viewers/ViewerSim.py
 steam_sdk/viewers/__init__.py
+steam_sdk/wrappers/Readme.md
 steam_sdk/wrappers/__init__.py
 steam_sdk/wrappers/wrapper_yaml.py
 steam_sdk/wrappers/java/__init__.py
-steam_sdk/wrappers/java/SIGMA/WrapperSIGMA.py
-steam_sdk/wrappers/java/SIGMA/__init__.py
-steam_sdk/wrappers/java/SIGMA/checkJava.py
-steam_sdk/wrappers/java/SIGMA/jars/__init__.py
 steam_sdk/wrappers/java/SING/__init__.py
-steam_sdk/wrappers/java/SING/jars/__init__.py
+steam_sdk/wrappers/java/SING/jars/__init__.py
+steam_sdk/wrappers/java/SING/jars/steam-sing.jar
```

### Comparing `steam_sdk-2023.2.3/steam_sdk.egg-info/requires.txt` & `steam_sdk-2023.4.0/steam_sdk.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -73,15 +73,17 @@
 ruamel.yaml.clib==0.2.6
 scipy==1.9.1
 seaborn==0.12.0
 six==1.16.0
 smmap==5.0.0
 stack-data==0.5.0
 STEAM-materials==0.0.2
+svglib==1.5.1
 tomli==2.0.1
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
 wcwidth==0.2.5
 zipp==3.8.1
+steam-pysigma==2023.4.8
```

