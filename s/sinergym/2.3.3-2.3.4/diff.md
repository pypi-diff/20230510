# Comparing `tmp/sinergym-2.3.3.tar.gz` & `tmp/sinergym-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-2.3.3.tar", last modified: Thu Apr 27 10:29:21 2023, max compression
+gzip compressed data, was "sinergym-2.3.4.tar", last modified: Wed May 10 07:17:54 2023, max compression
```

## Comparing `sinergym-2.3.3.tar` & `sinergym-2.3.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.579013 sinergym-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 10:29:18.000000 sinergym-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-27 10:29:18.000000 sinergym-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-27 10:29:21.579013 sinergym-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-04-27 10:29:18.000000 sinergym-2.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-27 10:29:20.000000 sinergym-2.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 10:29:21.579013 sinergym-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-27 10:29:20.000000 sinergym-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.551013 sinergym-2.3.3/sinergym/
--rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.551013 sinergym-2.3.3/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.555013 sinergym-2.3.3/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
--rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/5ZoneAutoDXVAV.idf
--rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
--rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
--rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/buildings/ShopWithVandBattery.idf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.555013 sinergym-2.3.3/sinergym/data/variables/
--rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/5ZoneAutoDXVAV.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
--rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/variables/ShopWithVandBattery.rdd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.575013 sinergym-2.3.3/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.575013 sinergym-2.3.3/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.575013 sinergym-2.3.3/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/simulators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/simulators/eplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/simulators/eplus_alpha.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.579013 sinergym-2.3.3/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 10:29:20.000000 sinergym-2.3.3/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:29:21.551013 sinergym-2.3.3/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 10:29:21.000000 sinergym-2.3.3/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.781370 sinergym-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 07:17:52.000000 sinergym-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 07:17:52.000000 sinergym-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-10 07:17:54.781370 sinergym-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-10 07:17:52.000000 sinergym-2.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 07:17:53.000000 sinergym-2.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-10 07:17:54.781370 sinergym-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-10 07:17:53.000000 sinergym-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.745370 sinergym-2.3.4/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (123)    94684 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.745370 sinergym-2.3.4/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.749370 sinergym-2.3.4/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)   168677 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   140099 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/5ZoneAutoDXVAV.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   586238 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   373188 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   475269 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/OfficeGridStorageSmoothing.idf
+-rw-r--r--   0 runner    (1001) docker     (123)   265862 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/buildings/ShopWithVandBattery.idf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.753370 sinergym-2.3.4/sinergym/data/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)    35474 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    32612 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/5ZoneAutoDXVAV.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    39868 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    36451 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42336 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/OfficeGridStorageSmoothing.rdd
+-rw-r--r--   0 runner    (1001) docker     (123)    42494 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/variables/ShopWithVandBattery.rdd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.777371 sinergym-2.3.4/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (123)    28629 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1565086 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28503 2023-05-10 07:17:53.000000 sinergym-2.3.4/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1550279 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28704 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1621761 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28716 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1553382 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28801 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558629 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28740 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1558423 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1601571 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29016 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1637298 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1629153 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1639985 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29614 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1613784 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29529 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1624547 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (123)    29243 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1625209 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.777371 sinergym-2.3.4/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.777371 sinergym-2.3.4/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/simulators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/simulators/eplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/simulators/eplus_alpha.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.781370 sinergym-2.3.4/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24235 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:17:54.749370 sinergym-2.3.4/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12180 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 07:17:54.000000 sinergym-2.3.4/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-2.3.3/LICENSE` & `sinergym-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/PKG-INFO` & `sinergym-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.3.3
+Version: 2.3.4
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
-Metadata-Version: 2.1 Name: sinergym Version: 2.3.3 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.3.4 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.3.3/README.md` & `sinergym-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/setup.py` & `sinergym-2.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/__init__.py` & `sinergym-2.3.4/sinergym/__init__.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf` & `sinergym-2.3.4/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/buildings/5ZoneAutoDXVAV.idf` & `sinergym-2.3.4/sinergym/data/buildings/5ZoneAutoDXVAV.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf` & `sinergym-2.3.4/sinergym/data/buildings/ASHRAE9012016_OfficeMedium_Denver.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf` & `sinergym-2.3.4/sinergym/data/buildings/ASHRAE9012016_Warehouse_Denver.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/buildings/OfficeGridStorageSmoothing.idf` & `sinergym-2.3.4/sinergym/data/buildings/OfficeGridStorageSmoothing.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/buildings/ShopWithVandBattery.idf` & `sinergym-2.3.4/sinergym/data/buildings/ShopWithVandBattery.idf`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd` & `sinergym-2.3.4/sinergym/data/variables/2ZoneDataCenterHVAC_wEconomizer.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/variables/5ZoneAutoDXVAV.rdd` & `sinergym-2.3.4/sinergym/data/variables/5ZoneAutoDXVAV.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd` & `sinergym-2.3.4/sinergym/data/variables/ASHRAE9012016_OfficeMedium_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd` & `sinergym-2.3.4/sinergym/data/variables/ASHRAE9012016_Warehouse_Denver.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/variables/OfficeGridStorageSmoothing.rdd` & `sinergym-2.3.4/sinergym/data/variables/OfficeGridStorageSmoothing.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/variables/ShopWithVandBattery.rdd` & `sinergym-2.3.4/sinergym/data/variables/ShopWithVandBattery.rdd`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-2.3.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-2.3.4/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-2.3.4/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-2.3.4/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-2.3.4/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-2.3.4/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-2.3.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-2.3.4/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-2.3.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-2.3.4/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-2.3.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-2.3.4/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-2.3.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-2.3.4/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-2.3.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-2.3.4/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-2.3.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-2.3.4/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-2.3.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-2.3.4/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-2.3.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-2.3.4/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-2.3.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-2.3.4/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-2.3.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-2.3.4/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/envs/eplus_env.py` & `sinergym-2.3.4/sinergym/envs/eplus_env.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/simulators/base.py` & `sinergym-2.3.4/sinergym/simulators/base.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/simulators/eplus.py` & `sinergym-2.3.4/sinergym/simulators/eplus.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,15 +488,15 @@
             self._conn.close()
             self._conn = None
             # Process the output
             # Sleep the thread so EnergyPlus has time to do the post processing
             time.sleep(1)
 
             # Kill subprocess
-            os.killpg(self._eplus_process.pid, signal.SIGTERM)
+            self._eplus_process.kill()
             self._episode_existed = False
 
     def _run_eplus_outputProcessing(self) -> None:  # pragma: no cover
         # If simulator has not been running with reset at least one time this
         # method is null.
         if hasattr(self, '_eplus_working_dir'):
             eplus_outputProcessing_process = subprocess.Popen(
```

### Comparing `sinergym-2.3.3/sinergym/simulators/eplus_alpha.py` & `sinergym-2.3.4/sinergym/simulators/eplus_alpha.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/callbacks.py` & `sinergym-2.3.4/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/common.py` & `sinergym-2.3.4/sinergym/utils/common.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/config.py` & `sinergym-2.3.4/sinergym/utils/config.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/constants.py` & `sinergym-2.3.4/sinergym/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/controllers.py` & `sinergym-2.3.4/sinergym/utils/controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             env (Any): Simulation environment
         """
 
         self.env = env
 
         self.variables = env.variables
 
-        self.setpoints_summer = (26, 29.0)
+        self.setpoints_summer = (23, 26.0)
         self.setpoints_winter = (20.0, 23.5)
 
     def act(self, observation: List[Any]) -> Sequence[Any]:
         """Select action based on indoor temperature.
 
         Args:
             observation (List[Any]): Perceived observation.
```

### Comparing `sinergym-2.3.3/sinergym/utils/env_checker.py` & `sinergym-2.3.4/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/evaluation.py` & `sinergym-2.3.4/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/gcloud.py` & `sinergym-2.3.4/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/logger.py` & `sinergym-2.3.4/sinergym/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/rewards.py` & `sinergym-2.3.4/sinergym/utils/rewards.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym/utils/wrappers.py` & `sinergym-2.3.4/sinergym/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym.egg-info/PKG-INFO` & `sinergym-2.3.4/sinergym.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 2.3.3
+Version: 2.3.4
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
-Metadata-Version: 2.1 Name: sinergym Version: 2.3.3 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 2.3.4 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
```

### Comparing `sinergym-2.3.3/sinergym.egg-info/SOURCES.txt` & `sinergym-2.3.4/sinergym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinergym-2.3.3/sinergym.egg-info/requires.txt` & `sinergym-2.3.4/sinergym.egg-info/requires.txt`

 * *Files identical despite different names*

