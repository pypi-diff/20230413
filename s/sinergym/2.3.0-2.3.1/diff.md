# Comparing `tmp/sinergym-2.3.0.tar.gz` & `tmp/sinergym-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-2.3.0.tar", last modified: Mon Apr 10 18:19:39 2023, max compression
+gzip compressed data, was "sinergym-2.3.1.tar", last modified: Thu Apr 13 11:16:59 2023, max compression
```

## Comparing `sinergym-2.3.0.tar` & `sinergym-2.3.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.264739 sinergym-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-10 18:19:36.000000 sinergym-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 18:19:36.000000 sinergym-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-10 18:19:39.264739 sinergym-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-04-10 18:19:36.000000 sinergym-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 18:19:38.000000 sinergym-2.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-10 18:19:39.264739 sinergym-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-10 18:19:38.000000 sinergym-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.232739 sinergym-2.3.0/sinergym/
--rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.232739 sinergym-2.3.0/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.236739 sinergym-2.3.0/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
--rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/5ZoneAutoDXVAV.idf
--rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
--rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/buildings/ShopWithVandBattery.idf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.236739 sinergym-2.3.0/sinergym/data/variables/
--rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/5ZoneAutoDXVAV.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/variables/ShopWithVandBattery.rdd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.260739 sinergym-2.3.0/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.260739 sinergym-2.3.0/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.260739 sinergym-2.3.0/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/simulators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/simulators/eplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/simulators/eplus_alpha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.264739 sinergym-2.3.0/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39240 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)    22278 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 18:19:38.000000 sinergym-2.3.0/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:19:39.236739 sinergym-2.3.0/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-10 18:19:39.000000 sinergym-2.3.0/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.356566 sinergym-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-13 11:16:56.000000 sinergym-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 11:16:56.000000 sinergym-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-13 11:16:59.356566 sinergym-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-04-13 11:16:56.000000 sinergym-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 11:16:58.000000 sinergym-2.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-13 11:16:59.356566 sinergym-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-13 11:16:58.000000 sinergym-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.324566 sinergym-2.3.1/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.324566 sinergym-2.3.1/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.328566 sinergym-2.3.1/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/buildings/5ZoneAutoDXVAV.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/buildings/ShopWithVandBattery.idf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.332566 sinergym-2.3.1/sinergym/data/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/variables/5ZoneAutoDXVAV.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/variables/ShopWithVandBattery.rdd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.352566 sinergym-2.3.1/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.356566 sinergym-2.3.1/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.356566 sinergym-2.3.1/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/simulators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/simulators/eplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/simulators/eplus_alpha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.356566 sinergym-2.3.1/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24155 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 11:16:58.000000 sinergym-2.3.1/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:16:59.328566 sinergym-2.3.1/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17046 2023-04-13 11:16:59.000000 sinergym-2.3.1/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-13 11:16:59.000000 sinergym-2.3.1/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:16:59.000000 sinergym-2.3.1/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-13 11:16:59.000000 sinergym-2.3.1/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 11:16:59.000000 sinergym-2.3.1/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-2.3.0/LICENSE` & `sinergym-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/PKG-INFO` & `sinergym-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.3.0
+Version: 2.3.1
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.3.0 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.3.1 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.3.0/README.md` & `sinergym-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/setup.py` & `sinergym-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/__init__.py` & `sinergym-2.3.1/sinergym/__init__.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf` & `sinergym-2.3.1/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/buildings/5ZoneAutoDXVAV.idf` & `sinergym-2.3.1/sinergym/data/buildings/5ZoneAutoDXVAV.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf` & `sinergym-2.3.1/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf` & `sinergym-2.3.1/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/buildings/OfficeGridStorageSmoothing.idf` & `sinergym-2.3.1/sinergym/data/buildings/OfficeGridStorageSmoothing.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/buildings/ShopWithVandBattery.idf` & `sinergym-2.3.1/sinergym/data/buildings/ShopWithVandBattery.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd` & `sinergym-2.3.1/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/variables/5ZoneAutoDXVAV.rdd` & `sinergym-2.3.1/sinergym/data/variables/5ZoneAutoDXVAV.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd` & `sinergym-2.3.1/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd` & `sinergym-2.3.1/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/variables/OfficeGridStorageSmoothing.rdd` & `sinergym-2.3.1/sinergym/data/variables/OfficeGridStorageSmoothing.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/variables/ShopWithVandBattery.rdd` & `sinergym-2.3.1/sinergym/data/variables/ShopWithVandBattery.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-2.3.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-2.3.1/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-2.3.1/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-2.3.1/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-2.3.1/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-2.3.1/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-2.3.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-2.3.1/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-2.3.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-2.3.1/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-2.3.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-2.3.1/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-2.3.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-2.3.1/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-2.3.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-2.3.1/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-2.3.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-2.3.1/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-2.3.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-2.3.1/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-2.3.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-2.3.1/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-2.3.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-2.3.1/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-2.3.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-2.3.1/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/envs/eplus_env.py` & `sinergym-2.3.1/sinergym/envs/eplus_env.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/simulators/base.py` & `sinergym-2.3.1/sinergym/simulators/base.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/simulators/eplus.py` & `sinergym-2.3.1/sinergym/simulators/eplus.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/simulators/eplus_alpha.py` & `sinergym-2.3.1/sinergym/simulators/eplus_alpha.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/callbacks.py` & `sinergym-2.3.1/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/common.py` & `sinergym-2.3.1/sinergym/utils/common.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/config.py` & `sinergym-2.3.1/sinergym/utils/config.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/constants.py` & `sinergym-2.3.1/sinergym/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,20 @@
                 'done': [False, True],
                 'hour': [0, 23],
                 'month': [1, 12],
                 'year': [1, 2022],
                 'reward': [-3.550779087370951, -0.0086829184636919],
                 'time (seconds)': [0, 31536000],
                 'timestep': [0, 35040],
-                'total_power_no_units': [-3.259557259261767, -0.0173658369273838]}
+                'total_power_no_units': [-3.259557259261767, -0.0173658369273838],
+                # Added previous variables:
+                'Zone Thermostat Cooling Setpoint Temperature(SPACE1-1)_previous': [21.0, 30.0],
+                'Zone Thermostat Heating Setpoint Temperature(SPACE1-1)_previous': [15.0,
+                                                                                    22.49999046325684],
+                'Zone Air Temperature(SPACE1-1)_previous': [15.22565264653451, 30.00826655379267]}
 
 
 RANGES_DATACENTER = {
     'East-ClgSetP-RL': [21.0, 30.0],
     'East-HtgSetP-RL': [15.0, 22.499973],
     'Facility Total HVAC Electricity Demand Rate(Whole Building)': [1763.7415,
                                                                     76803.016],
```

### Comparing `sinergym-2.3.0/sinergym/utils/controllers.py` & `sinergym-2.3.1/sinergym/utils/controllers.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/env_checker.py` & `sinergym-2.3.1/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/evaluation.py` & `sinergym-2.3.1/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/gcloud.py` & `sinergym-2.3.1/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/logger.py` & `sinergym-2.3.1/sinergym/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/rewards.py` & `sinergym-2.3.1/sinergym/utils/rewards.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym/utils/wrappers.py` & `sinergym-2.3.1/sinergym/utils/wrappers.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,57 +45,77 @@
         return obs, reward_vector, terminated, truncated, info
 
 
 class NormalizeObservation(gym.ObservationWrapper):
 
     def __init__(self,
                  env: Any,
-                 ranges: Dict[str, Sequence[Any]]):
+                 ranges: Dict[str, Sequence[Any]],
+                 variables: Optional[List[str]] = None):
         """Observations normalized to range [0, 1].
 
         Args:
             env (Any): Original Sinergym environment.
             ranges (Dict[str, Sequence[Any]]): Observation variables ranges to apply normalization (rely on environment).
+            variables (Optional[List[str]]): List of variables you want to normalize. If it is None, all environment variables are included.
         """
         super(NormalizeObservation, self).__init__(env)
         self.unwrapped_observation = None
         self.ranges = ranges
+        ranges_keys = list(self.ranges.keys())
+        self.normalization_variables = deepcopy(
+            self.env.variables['observation'])
+
+        # Normalized variables must be in ranges dict, if not the variable will
+        # not be normalized.
+        if variables is None:
+            self.normalized_variables = [
+                var for var in self.normalization_variables if var in ranges_keys]
+        else:
+            self.normalized_variables = [
+                var for var in variables if var in ranges_keys]
+
+        for variable in self.normalized_variables:
+            # Check variables exist
+            assert variable in self.normalization_variables, 'NormalizeObservation: {} does not exist in environment.'.format(
+                variable)
 
     def observation(self, obs: np.ndarray) -> np.ndarray:
         """Applies normalization to observation.
 
         Args:
             obs (np.ndarray): Original observation.
 
         Returns:
             np.ndarray: Normalized observation.
         """
         # Save original obs in class attribute
         self.unwrapped_observation = obs.copy()
 
-        # NOTE: If you want to record day, month and hour, you should add that
-        # variables as keys
-        for i, variable in enumerate(self.env.variables['observation']):
+        for variable in self.normalized_variables:
+            # Calculate variable index for obs
+            variable_index = self.normalization_variables.index(variable)
             # normalization (handle DivisionbyZero Error)
             if (self.ranges[variable][1] -
                     self.ranges[variable][0] == 0):
-                obs[i] = max(
+                obs[variable_index] = max(
                     self.ranges[variable][0], min(
-                        obs[i], self.ranges[variable][1]))
+                        obs[variable_index], self.ranges[variable][1]))
             else:
-                obs[i] = (obs[i] - self.ranges[variable][0]) / \
-                    (self.ranges[variable][1] - self.ranges[variable][0])
+                obs[variable_index] = (
+                    obs[variable_index] - self.ranges[variable][0]) / (
+                    self.ranges[variable][1] - self.ranges[variable][0])
 
             # If value is out
-            if np.isnan(obs[i]):
-                obs[i] = 0
-            elif obs[i] > 1:
-                obs[i] = 1
-            elif obs[i] < 0:
-                obs[i] = 0
+            if np.isnan(obs[variable_index]):
+                obs[variable_index] = 0
+            elif obs[variable_index] > 1:
+                obs[variable_index] = 1
+            elif obs[variable_index] < 0:
+                obs[variable_index] = 0
         # Return obs values in the SAME ORDER than obs argument.
         return np.array(obs)
 
     def get_unwrapped_obs(self) -> Optional[np.ndarray]:
         """Get last environment observation without normalization.
 
         Returns:
@@ -182,15 +202,15 @@
         Args:
             env (Any): Original Gym environment.
             logger_class (CSVLogger): CSV Logger class to use to log all information.
             monitor_header: Header for monitor.csv in each episode. Default is None (default format).
             progress_header: Header for progress.csv in whole simulation. Default is None (default format).
             flag (bool, optional): State of logger (activate or deactivate). Defaults to True.
         """
-        gym.Wrapper.__init__(self, env)
+        super(LoggerWrapper, self).__init__(env)
         # Headers for csv logger
         monitor_header_list = monitor_header if monitor_header is not None else ['timestep'] + env.variables['observation'] + env.variables['action'] + [
             'time (seconds)', 'reward', 'power_penalty', 'comfort_penalty', 'abs_comfort', 'terminated']
         self.monitor_header = ''
         for element_header in monitor_header_list:
             self.monitor_header += element_header + ','
         self.monitor_header = self.monitor_header[:-1]
@@ -335,41 +355,48 @@
 class DatetimeWrapper(gym.ObservationWrapper):
     """Wrapper to substitute day value by is_weekend flag, and hour and month by sin and cos values.
        Observation space is updated automatically."""
 
     def __init__(self,
                  env: Any):
         super(DatetimeWrapper, self).__init__(env)
+        # Save observation variables before wrapper
+        self.original_datetime_observation_variables = deepcopy(
+            self.variables['observation'])
         # Update new shape
         new_shape = env.observation_space.shape[0] + 2
         self.observation_space = gym.spaces.Box(
             low=-5e6, high=5e6, shape=(new_shape,), dtype=np.float32)
         # Update observation variables
         day_index = self.variables['observation'].index('day')
         self.variables['observation'][day_index] = 'is_weekend'
         hour_index = self.variables['observation'].index('hour')
         self.variables['observation'][hour_index] = 'hour_cos'
         self.variables['observation'].insert(hour_index + 1, 'hour_sin')
         month_index = self.variables['observation'].index('month')
         self.variables['observation'][month_index] = 'month_cos'
         self.variables['observation'].insert(month_index + 1, 'month_sin')
+        # Save observation variables after wrapper
+        self.datetime_observation_variables = deepcopy(
+            self.variables['observation'])
 
     def observation(self, obs: np.ndarray) -> np.ndarray:
         """Applies calculation in is_weekend flag, and sen and cos in hour and month
 
         Args:
             obs (np.ndarray): Original observation.
 
         Returns:
             np.ndarray: Transformed observation.
         """
-        obs_dict = dict(zip(self.original_obs, obs))
+        # Get obs_dict with observation variables from unwrapped env
+        obs_dict = dict(zip(self.original_datetime_observation_variables, obs))
         # New obs dict with same values than obs_dict but with new fields with
         # None
-        new_obs = dict.fromkeys(self.variables['observation'])
+        new_obs = dict.fromkeys(self.datetime_observation_variables)
         for key, value in obs_dict.items():
             if key in new_obs.keys():
                 new_obs[key] = value
         dt = datetime(
             int(obs_dict['year']),
             int(obs_dict['month']),
             int(obs_dict['day']),
@@ -390,44 +417,49 @@
 
     def __init__(self,
                  env: Any,
                  previous_variables: List[str]):
         super(PreviousObservationWrapper, self).__init__(env)
         # Check and apply previous variables to observation space and variables
         # names
-        self.original_variable_index = []
+        self.previous_variables = previous_variables
+        self.original_previous_observation_variables = deepcopy(
+            self.variables['observation'])
         for obs_var in previous_variables:
             assert obs_var in self.variables['observation'], '{} variable is not defined in observation space, revise the name.'.format(
                 obs_var)
-            self.original_variable_index.append(
-                self.variables['observation'].index(obs_var))
             self.variables['observation'].append(obs_var + '_previous')
         # Update new shape
         new_shape = env.observation_space.shape[0] + len(previous_variables)
         self.observation_space = gym.spaces.Box(
             low=-5e6, high=5e6, shape=(new_shape,), dtype=np.float32)
 
+        self.previous_observation_variables = deepcopy(
+            self.variables['observation'])
+
         # previous observation initialization
         self.previous_observation = np.zeros(
             shape=len(previous_variables), dtype=np.float32)
 
     def observation(self, obs: np.ndarray) -> np.ndarray:
         """Add previous observation to the current one
 
         Args:
             obs (np.ndarray): Original observation.
 
         Returns:
             np.ndarray: observation with
         """
-
+        # Concatenate current obs with previous observation variables
         new_obs = np.concatenate((obs, self.previous_observation))
-        # Aquí tengo que seleccionar las variables que se correponden con lo
-        # que son
-        self.previous_observation = obs[self.original_variable_index]
+        # Update previous observation to current observation
+        self.previous_observation = []
+        for variable in self.previous_variables:
+            index = self.previous_observation_variables.index(variable)
+            self.previous_observation.append(obs[index])
 
         return new_obs
 
 
 class DiscreteIncrementalWrapper(gym.ActionWrapper):
     """A wrapper for an incremental setpoint discrete action space environment.
     WARNING: A environment with only temperature setpoints control must be used
@@ -503,21 +535,21 @@
         """Takes the discrete action and transforms it to setpoints tuple."""
         action_ = self.action_mapping[action]
         # Update current setpoints values with incremental action
         self.current_setpoints = [
             sum(i) for i in zip(
                 self.current_setpoints,
                 action_)]
-
-        setpoints = np.clip(
+        # clip setpoints returned
+        self.current_setpoints = np.clip(
             np.array(self.current_setpoints),
             self.min_values,
             self.max_values
         )
-        return list(setpoints)
+        return list(self.current_setpoints)
 
     # ---------------------- Specific environment wrappers ---------------------#
 
 
 class OfficeGridStorageSmoothingActionConstraintsWrapper(
         gym.ActionWrapper):  # pragma: no cover
     def __init__(self, env):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sinergym-2.3.0/sinergym.egg-info/PKG-INFO` & `sinergym-2.3.1/sinergym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.3.0
+Version: 2.3.1
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 2.3.0 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.3.1 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.3.0/sinergym.egg-info/SOURCES.txt` & `sinergym-2.3.1/sinergym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.0/sinergym.egg-info/requires.txt` & `sinergym-2.3.1/sinergym.egg-info/requires.txt`

 * *Files identical despite different names*

