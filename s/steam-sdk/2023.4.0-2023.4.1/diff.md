# Comparing `tmp/steam_sdk-2023.4.0.tar.gz` & `tmp/steam_sdk-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam_sdk-2023.4.0.tar", last modified: Thu Apr 13 16:02:05 2023, max compression
+gzip compressed data, was "dist\steam_sdk-2023.4.1.tar", last modified: Thu Apr 13 17:30:09 2023, max compression
```

## Comparing `steam_sdk-2023.4.0.tar` & `steam_sdk-2023.4.1.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.057289 steam_sdk-2023.4.0/
--rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam_sdk-2023.4.0/.gitignore
--rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam_sdk-2023.4.0/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam_sdk-2023.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-04-13 16:02:05.055294 steam_sdk-2023.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam_sdk-2023.4.0/Readme.md
--rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam_sdk-2023.4.0/mkdocs.yaml
--rw-rw-rw-   0        0        0     1684 2023-04-13 15:56:12.000000 steam_sdk-2023.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 16:02:05.059284 steam_sdk-2023.4.0/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-04-13 15:54:56.000000 steam_sdk-2023.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.829896 steam_sdk-2023.4.0/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.836882 steam_sdk-2023.4.0/steam_sdk/analyses/
--rw-rw-rw-   0        0        0    99466 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.837875 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.839870 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.850853 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.852835 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.861812 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.864803 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.870787 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.872782 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.886745 steam_sdk-2023.4.0/steam_sdk/builders/
--rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160973 2023-01-17 16:22:36.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    32596 2023-04-13 15:48:40.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    37964 2023-04-13 15:57:32.000000 steam_sdk-2023.4.0/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/builders/Readme.md
--rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam_sdk-2023.4.0/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam_sdk-2023.4.0/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.888740 steam_sdk-2023.4.0/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.891732 steam_sdk-2023.4.0/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.895720 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.898712 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
--rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/Readme.md
--rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.900714 steam_sdk-2023.4.0/steam_sdk/configs/users/
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/configs/users/Readme.md
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.902701 steam_sdk-2023.4.0/steam_sdk/cosims/
--rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/cosims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.938606 steam_sdk-2023.4.0/steam_sdk/data/
--rw-rw-rw-   0        0        0    10029 2023-04-03 16:34:32.000000 steam_sdk-2023.4.0/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     8004 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam_sdk-2023.4.0/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2862 2023-03-30 16:17:31.000000 steam_sdk-2023.4.0/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     3169 2023-01-20 13:20:13.000000 steam_sdk-2023.4.0/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35518 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2609 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam_sdk-2023.4.0/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam_sdk-2023.4.0/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam_sdk-2023.4.0/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam_sdk-2023.4.0/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/Readme.md
--rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.953566 steam_sdk-2023.4.0/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     5329 2023-04-13 15:48:42.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam_sdk-2023.4.0/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.957555 steam_sdk-2023.4.0/steam_sdk/drivers/temp/
--rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/temp/postLEDET.py
--rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/temp/runLEDET.py
--rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/drivers/temp/simLEDET.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.994456 steam_sdk-2023.4.0/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10602 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.995453 steam_sdk-2023.4.0/steam_sdk/parsers/templates/
--rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam_sdk-2023.4.0/steam_sdk/parsers/templates/template_Dakota.in
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.005427 steam_sdk-2023.4.0/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    41232 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    49099 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    59958 2023-04-03 16:34:32.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam_sdk-2023.4.0/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.013407 steam_sdk-2023.4.0/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-02 17:12:04.000000 steam_sdk-2023.4.0/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0    18478 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/plotters/PlotterSIGMA.py
--rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.015401 steam_sdk-2023.4.0/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.031358 steam_sdk-2023.4.0/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam_sdk-2023.4.0/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam_sdk-2023.4.0/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam_sdk-2023.4.0/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     6745 2023-04-13 13:06:52.000000 steam_sdk-2023.4.0/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.035347 steam_sdk-2023.4.0/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam_sdk-2023.4.0/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.038339 steam_sdk-2023.4.0/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.039349 steam_sdk-2023.4.0/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.048312 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:05.051304 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam_sdk-2023.4.0/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:02:04.834883 steam_sdk-2023.4.0/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-04-13 16:01:37.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7134 2023-04-13 16:02:03.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:01:37.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1595 2023-04-13 16:01:37.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 16:01:37.000000 steam_sdk-2023.4.0/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.675887 steam_sdk-2023.4.1/
+-rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam_sdk-2023.4.1/.gitignore
+-rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam_sdk-2023.4.1/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam_sdk-2023.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-04-13 17:30:09.675887 steam_sdk-2023.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam_sdk-2023.4.1/Readme.md
+-rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam_sdk-2023.4.1/mkdocs.yaml
+-rw-rw-rw-   0        0        0     1684 2023-04-13 15:56:12.000000 steam_sdk-2023.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 17:30:09.676884 steam_sdk-2023.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-13 17:24:12.000000 steam_sdk-2023.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.519305 steam_sdk-2023.4.1/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.526289 steam_sdk-2023.4.1/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0    99466 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.527285 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.529280 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.538255 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.539253 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.543242 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.545236 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.549226 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.550223 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.563188 steam_sdk-2023.4.1/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   160973 2023-01-17 16:22:36.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    32791 2023-04-13 17:03:42.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    38418 2023-04-13 17:10:32.000000 steam_sdk-2023.4.1/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/builders/Readme.md
+-rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam_sdk-2023.4.1/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam_sdk-2023.4.1/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.564186 steam_sdk-2023.4.1/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.566181 steam_sdk-2023.4.1/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.569172 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.572164 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
+-rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/Readme.md
+-rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.573162 steam_sdk-2023.4.1/steam_sdk/configs/users/
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/configs/users/Readme.md
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.575156 steam_sdk-2023.4.1/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/cosims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.598095 steam_sdk-2023.4.1/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10029 2023-04-03 16:34:32.000000 steam_sdk-2023.4.1/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     8004 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam_sdk-2023.4.1/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2862 2023-03-30 16:17:31.000000 steam_sdk-2023.4.1/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     3169 2023-01-20 13:20:13.000000 steam_sdk-2023.4.1/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35518 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2609 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam_sdk-2023.4.1/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam_sdk-2023.4.1/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam_sdk-2023.4.1/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam_sdk-2023.4.1/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/Readme.md
+-rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.609066 steam_sdk-2023.4.1/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     5329 2023-04-13 15:48:42.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam_sdk-2023.4.1/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.611060 steam_sdk-2023.4.1/steam_sdk/drivers/temp/
+-rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/temp/postLEDET.py
+-rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/temp/runLEDET.py
+-rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/drivers/temp/simLEDET.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.634000 steam_sdk-2023.4.1/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10602 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.634997 steam_sdk-2023.4.1/steam_sdk/parsers/templates/
+-rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam_sdk-2023.4.1/steam_sdk/parsers/templates/template_Dakota.in
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.640980 steam_sdk-2023.4.1/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    41232 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    49099 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    59958 2023-04-03 16:34:32.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam_sdk-2023.4.1/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.645968 steam_sdk-2023.4.1/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2022-12-02 17:12:04.000000 steam_sdk-2023.4.1/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0    18478 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/plotters/PlotterSIGMA.py
+-rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.647962 steam_sdk-2023.4.1/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.665914 steam_sdk-2023.4.1/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam_sdk-2023.4.1/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam_sdk-2023.4.1/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam_sdk-2023.4.1/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     6745 2023-04-13 13:06:52.000000 steam_sdk-2023.4.1/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.668905 steam_sdk-2023.4.1/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam_sdk-2023.4.1/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.671898 steam_sdk-2023.4.1/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.671898 steam_sdk-2023.4.1/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.672895 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.674889 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam_sdk-2023.4.1/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-04-13 17:30:09.524292 steam_sdk-2023.4.1/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-04-13 17:29:43.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7134 2023-04-13 17:30:08.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 17:29:43.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1595 2023-04-13 17:29:43.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-13 17:29:43.000000 steam_sdk-2023.4.1/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam_sdk-2023.4.0/.gitignore` & `steam_sdk-2023.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/.gitlab-ci.yml` & `steam_sdk-2023.4.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/PKG-INFO` & `steam_sdk-2023.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam_sdk
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SDK,CERN,API,STEAM
+Keywords: STEAM,CERN,SDK,API
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam_sdk-2023.4.0/Readme.md` & `steam_sdk-2023.4.1/Readme.md`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/mkdocs.yaml` & `steam_sdk-2023.4.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/requirements.txt` & `steam_sdk-2023.4.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/setup.py` & `steam_sdk-2023.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam_sdk',
-    version="2023.4.0",
+    version="2023.4.1",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/AnalysisSTEAM.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam_sdk-2023.4.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/BuilderFiQuS.py` & `steam_sdk-2023.4.1/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/BuilderLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/BuilderModel.py` & `steam_sdk-2023.4.1/steam_sdk/builders/BuilderModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,16 @@
                 self.path_data = Path(self.path_magnet / self.model_data.Sources.coil_fromROXIE).resolve()
             if self.model_data.Sources.magnetic_field_fromROXIE:
                 self.path_map2d = Path(self.path_magnet / self.model_data.Sources.magnetic_field_fromROXIE).resolve()
             if self.model_data.Sources.conductor_fromROXIE:
                 self.path_cadata = Path(self.path_magnet / self.model_data.Sources.conductor_fromROXIE).resolve()
             if self.model_data.Sources.iron_fromROXIE:
                 self.path_iron = Path(self.path_magnet / self.model_data.Sources.iron_fromROXIE).resolve()
+            if self.model_data.Sources.BH_fromROXIE:
+                self.path_bh = str(Path(self.path_magnet / self.model_data.Sources.BH_fromROXIE).resolve())
         elif self.case_model in 'circuit':
             pass  # no paths to assign
         elif self.case_model == 'conductor':
             if self.conductor_data.Sources.magnetic_field_fromROXIE:
                 self.path_map2d = Path(
                     self.path_magnet / self.conductor_data.Sources.magnetic_field_fromROXIE).resolve()
         else:
@@ -528,15 +530,15 @@
         """
             Building a SIGMA model
         """
         file_working_directory = os.getcwd()
         if not output_path:
             output_path = self.output_path
 
-        BuilderSIGMA(input_model_data=self.model_data, input_roxie_data=self.roxie_data,
+        BuilderSIGMA(input_model_data=self.model_data, input_roxie_data=self.roxie_data, bh_curve_database=self.path_bh,
                      settings_dict=self.settings_dict, output_path=output_path,
                      flag_build=self.flag_build, verbose=self.verbose)
         os.chdir(file_working_directory)
 
 
     def load_circuit_parameters_from_csv(self, input_file_name: str, selected_circuit_name: str = None):
         '''
```

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/BuilderProteCCT.py` & `steam_sdk-2023.4.1/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/BuilderPyBBQ.py` & `steam_sdk-2023.4.1/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/BuilderSIGMA.py` & `steam_sdk-2023.4.1/steam_sdk/builders/BuilderSIGMA.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,38 @@
 
 class BuilderSIGMA:
     """
         Class to generate SIGMA models
     """
 
     def __init__(self, input_model_data: DataModelMagnet = None,
-                 input_roxie_data: dR.RoxieData = None,
+                 input_roxie_data: dR.RoxieData = None, bh_curve_database: str = None,
                  settings_dict: dict = None, output_path: str = None, flag_build: bool = False, verbose: bool = False):
-
+        """
+        Class for making Comsol modle with SIGMA via PySIGMA library
+        :param input_model_data:
+        :type input_model_data:
+        :param input_roxie_data:
+        :type input_roxie_data:
+        :param bh_curve_database: Full path to ROXIE .bhdata file (the extension could be also .txt)
+        :type bh_curve_database: str
+        :param settings_dict:
+        :type settings_dict:
+        :param output_path:
+        :type output_path:
+        :param flag_build:
+        :type flag_build:
+        :param verbose:
+        :type verbose:
+        """
         self.verbose: bool = verbose
 
         self.model_data: DataModelMagnet = input_model_data
         self.roxie_data: dR.RoxieData = input_roxie_data
+        self.bh_curve_database = bh_curve_database
         self.settings_dict: dict = settings_dict
         if output_path:
             self.output_path: str = str(output_path).replace('/', '\\')
         else:
             self.output_path = os.getcwd()
 
         if (not self.model_data or not self.roxie_data) and flag_build:
@@ -41,21 +58,16 @@
             # self.model =
             self.coil = []
             self.elements = {}
             self.coil_areas = []
             self.wedge_areas = []
             self.show_halfTurns = True  # to be provided by the yaml in the future
             self.model_name = f"{self.model_data.GeneralParameters.magnet_name}_Model"
-
-            self.bh_curve_database = os.path.join(Path(__file__).parent.parent.parent,
-                                                  "tests", "builders", "model_library", "magnets", "bh_curve_database.txt")
-
             self.COMSOL_exe_path = Path(self.settings_dict['comsolexe_path']).parent
             self.java_jdk_path = self.settings_dict['JAVA_jdk_path']
-
             self.COMSOL_compile_path = os.path.join(self.COMSOL_exe_path, 'comsolcompile.exe')  # Change os.join()
             self.COMSOL_batch_path = os.path.join(self.COMSOL_exe_path, 'comsolbatch.exe')
             self.COMSOL_version = os.path.basename(os.path.dirname(self.COMSOL_exe_path.parent.parent)).replace("COMSOL", "")
             if self.COMSOL_version != "60" and self.COMSOL_version != "53a":
                 raise Exception("Not supporting any other versions than 6.0 and 5.3a")
             self.model_java_file_path = f"{os.path.join(self.output_path, self.model_name)}.java"
             self.compile_batch_file_path = f"{os.path.join(self.output_path, self.model_name)}_Compile_and_Open.bat"
```

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam_sdk-2023.4.1/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/Solenoids.py` & `steam_sdk-2023.4.1/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/builders/geometricFunctions.py` & `steam_sdk-2023.4.1/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml` & `steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam_sdk-2023.4.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataAnalysis.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataConductor.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataDakota.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataEventCircuit.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataEventMagnet.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataFiQuS.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataModelCircuit.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataModelConductor.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataModelMagnet.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataParsimConductor.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataProteCCT.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataPyBBQ.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataRoxieParser.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataSettings.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DataSignal.py` & `steam_sdk-2023.4.1/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DictionaryLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DictionaryProteCCT.py` & `steam_sdk-2023.4.1/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/DictionaryPyBBQ.py` & `steam_sdk-2023.4.1/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/TemplateLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/data/TemplateProteCCT.py` & `steam_sdk-2023.4.1/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverAnalysis.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverDakota.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverFiQuS.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverPSPICE.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverProteCCT.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverPyBBQ.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverSIGMA.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/DriverXYCE.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/temp/postLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/temp/postLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/temp/runLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/temp/runLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/drivers/temp/simLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/drivers/temp/simLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/CSD_Reader.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserCond2d.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserCsd.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserCsv.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserDakota.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserDatToCsv.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserExcel.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserFiQuS.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserLEDET.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserMap2d.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserMat.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserPSPICE.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserPdf.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserProteCCT.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserRoxie.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserTdms.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserXYCE.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/ParserYAML.py` & `steam_sdk-2023.4.1/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsers/templates/template_Dakota.in` & `steam_sdk-2023.4.1/steam_sdk/parsers/templates/template_Dakota.in`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsims/ParsimConductor.py` & `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsims/ParsimDakota.py` & `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsims/ParsimEventCircuit.py` & `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsims/ParsimEventMagnet.py` & `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/parsims/ParsimSweep.py` & `steam_sdk-2023.4.1/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/plotters/PlotterModel.py` & `steam_sdk-2023.4.1/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/plotters/PlotterParametric.py` & `steam_sdk-2023.4.1/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/plotters/PlotterRoxie.py` & `steam_sdk-2023.4.1/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/plotters/PlotterSIGMA.py` & `steam_sdk-2023.4.1/steam_sdk/plotters/PlotterSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/postprocs/PostprocsMetrics.py` & `steam_sdk-2023.4.1/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/MTF_reading_functions.py` & `steam_sdk-2023.4.1/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelData.py` & `steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/ModifyModelDataconductor.py` & `steam_sdk-2023.4.1/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/clean_NaN_from_signal.py` & `steam_sdk-2023.4.1/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/compare_two_parameters.py` & `steam_sdk-2023.4.1/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/misc.py` & `steam_sdk-2023.4.1/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/tic_toc.py` & `steam_sdk-2023.4.1/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/utils/utils_PC.py` & `steam_sdk-2023.4.1/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/viewers/Viewer.py` & `steam_sdk-2023.4.1/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/viewers/ViewerMeas.py` & `steam_sdk-2023.4.1/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/viewers/ViewerSim.py` & `steam_sdk-2023.4.1/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/wrappers/java/SING/jars/steam-sing.jar` & `steam_sdk-2023.4.1/steam_sdk/wrappers/java/SING/jars/steam-sing.jar`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk/wrappers/wrapper_yaml.py` & `steam_sdk-2023.4.1/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk.egg-info/PKG-INFO` & `steam_sdk-2023.4.1/steam_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: SDK,CERN,API,STEAM
+Keywords: STEAM,CERN,SDK,API
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam_sdk-2023.4.0/steam_sdk.egg-info/SOURCES.txt` & `steam_sdk-2023.4.1/steam_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steam_sdk-2023.4.0/steam_sdk.egg-info/requires.txt` & `steam_sdk-2023.4.1/steam_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

