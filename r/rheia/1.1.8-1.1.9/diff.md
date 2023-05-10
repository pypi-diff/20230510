# Comparing `tmp/rheia-1.1.8.tar.gz` & `tmp/rheia-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Diede\OneDrive - UCL\Academia\rheia_framework\pip_build\dist\.tmp-zgkw09fl\rheia-1.1.8.tar", last modified: Fri Feb 17 14:52:07 2023, max compression
+gzip compressed data, was "C:\Users\Diede\OneDrive - UCL\Academia\rheia_framework\pip_build\dist\.tmp-sferaic4\rheia-1.1.9.tar", last modified: Wed May 10 15:21:27 2023, max compression
```

## Comparing `rheia-1.1.8.tar` & `rheia-1.1.9.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.440896 rheia-1.1.8/
--rw-rw-rw-   0        0        0     1095 2021-03-17 10:06:00.000000 rheia-1.1.8/LICENSE
--rw-rw-rw-   0        0        0       16 2021-01-06 11:48:13.000000 rheia-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      565 2023-02-17 14:52:07.440896 rheia-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1008 2021-07-15 07:42:37.000000 rheia-1.1.8/README.md
--rw-rw-rw-   0        0        0      108 2021-03-17 10:15:07.000000 rheia-1.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-17 14:52:07.440896 rheia-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-02-17 14:51:34.000000 rheia-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.158724 rheia-1.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.174036 rheia-1.1.8/src/rheia/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.189680 rheia-1.1.8/src/rheia/CASES/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.158724 rheia-1.1.8/src/rheia/CASES/DATA/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.189680 rheia-1.1.8/src/rheia/CASES/DATA/climate/
--rw-rw-rw-   0        0        0    71681 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/DATA/climate/climate_Brussels.CSV
--rw-rw-rw-   0        0        0    71577 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/DATA/climate/climate_Madrid.CSV
--rw-rw-rw-   0        0        0    72055 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/DATA/climate/climate_Paris.CSV
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.189680 rheia-1.1.8/src/rheia/CASES/DATA/demand/
--rw-rw-rw-   0        0        0   112890 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/DATA/demand/load_Brussels_dwelling.csv
--rw-rw-rw-   0        0        0   113023 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/DATA/demand/load_Madrid_dwelling.csv
--rw-rw-rw-   0        0        0   112964 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/DATA/demand/load_Paris_dwelling.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.205307 rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/__init__.py
--rw-rw-rw-   0        0        0    29012 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/case.txt
--rw-rw-rw-   0        0        0     1096 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/case_description.py
--rw-rw-rw-   0        0        0       89 2022-09-29 11:47:02.000000 rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/design_space.csv
--rw-rw-rw-   0        0        0     4870 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/run_energyplan.py
--rw-rw-rw-   0        0        0      154 2022-09-29 11:47:24.000000 rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/stochastic_space.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.205307 rheia-1.1.8/src/rheia/CASES/FOUR_BAR_TRUSS/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/FOUR_BAR_TRUSS/__init__.py
--rw-rw-rw-   0        0        0     1111 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/FOUR_BAR_TRUSS/case_description.py
--rw-rw-rw-   0        0        0      145 2022-09-29 11:46:13.000000 rheia-1.1.8/src/rheia/CASES/FOUR_BAR_TRUSS/design_space.csv
--rw-rw-rw-   0        0        0      970 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/FOUR_BAR_TRUSS/four_bar_truss.py
--rw-rw-rw-   0        0        0      129 2022-09-29 11:31:59.000000 rheia-1.1.8/src/rheia/CASES/FOUR_BAR_TRUSS/stochastic_space.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.236949 rheia-1.1.8/src/rheia/CASES/H2_FUEL/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.236949 rheia-1.1.8/src/rheia/CASES/H2_FUEL/__pycache__/
--rw-rw-rw-   0        0        0      165 2022-09-29 13:24:41.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0     1938 2022-09-29 13:24:41.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/__pycache__/case_description.cpython-38.pyc
--rw-rw-rw-   0        0        0    15321 2022-09-29 13:24:41.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/__pycache__/h2_fuel.cpython-38.pyc
--rw-rw-rw-   0        0        0     2115 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/case_description.py
--rw-rw-rw-   0        0        0      280 2022-09-29 11:54:50.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:51:33.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_0.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:51:51.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_1.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:55:40.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_10.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:55:20.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_11.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:55:06.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_12.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:54:32.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_13.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:54:18.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_14.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:54:03.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_15.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:53:47.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_16.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:50:33.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_17.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:50:07.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_18.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:50:57.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_19.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:52:07.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_2.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:52:23.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_3.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:52:40.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_4.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:52:57.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_5.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:53:12.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_6.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:53:29.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_7.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:49:39.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_8.csv
--rw-rw-rw-   0        0        0      292 2022-09-29 11:56:01.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_9.csv
--rw-rw-rw-   0        0        0      282 2022-09-29 11:51:17.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/design_space_tutorial_uq.csv
--rw-rw-rw-   0        0        0    19598 2022-09-29 13:05:42.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/h2_fuel.py
--rw-rw-rw-   0        0        0      389 2022-09-29 11:56:36.000000 rheia-1.1.8/src/rheia/CASES/H2_FUEL/stochastic_space.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.252585 rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/__init__.py
--rw-rw-rw-   0        0        0     2473 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/case_description.py
--rw-rw-rw-   0        0        0     1029 2022-09-29 11:58:09.000000 rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/design_space.csv
--rw-rw-rw-   0        0        0    40333 2022-09-29 13:05:37.000000 rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/h2_mobility.py
--rw-rw-rw-   0        0        0      822 2022-09-29 11:58:03.000000 rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/stochastic_space.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.268210 rheia-1.1.8/src/rheia/CASES/H2_POWER/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/H2_POWER/__init__.py
--rw-rw-rw-   0        0        0     2530 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/H2_POWER/case_description.py
--rw-rw-rw-   0        0        0      572 2022-09-29 11:57:36.000000 rheia-1.1.8/src/rheia/CASES/H2_POWER/design_space.csv
--rw-rw-rw-   0        0        0    35668 2022-09-29 13:05:33.000000 rheia-1.1.8/src/rheia/CASES/H2_POWER/h2_power.py
--rw-rw-rw-   0        0        0      800 2022-09-29 11:57:53.000000 rheia-1.1.8/src/rheia/CASES/H2_POWER/stochastic_space.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.268210 rheia-1.1.8/src/rheia/CASES/NO_MODEL/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/NO_MODEL/__init__.py
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/NO_MODEL/case_description.py
--rw-rw-rw-   0        0        0       25 2022-09-29 11:58:40.000000 rheia-1.1.8/src/rheia/CASES/NO_MODEL/design_space.csv
--rw-rw-rw-   0        0        0       50 2022-09-29 11:58:51.000000 rheia-1.1.8/src/rheia/CASES/NO_MODEL/stochastic_space.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.268210 rheia-1.1.8/src/rheia/CASES/REF/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/REF/__init__.py
--rw-rw-rw-   0        0        0     1271 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/REF/case_description.py
--rw-rw-rw-   0        0        0       26 2022-09-29 11:59:25.000000 rheia-1.1.8/src/rheia/CASES/REF/design_space.csv
--rw-rw-rw-   0        0        0       51 2022-09-29 11:59:16.000000 rheia-1.1.8/src/rheia/CASES/REF/stochastic_space.csv
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/CASES/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.283833 rheia-1.1.8/src/rheia/CASES/__pycache__/
--rw-rw-rw-   0        0        0      157 2022-09-29 13:35:01.000000 rheia-1.1.8/src/rheia/CASES/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0    15662 2022-09-29 13:35:01.000000 rheia-1.1.8/src/rheia/CASES/__pycache__/determine_stoch_des_space.cpython-38.pyc
--rw-rw-rw-   0        0        0    22514 2022-09-29 11:46:22.000000 rheia-1.1.8/src/rheia/CASES/determine_stoch_des_space.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.283833 rheia-1.1.8/src/rheia/OPT/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.165507 rheia-1.1.8/src/rheia/OPT/INPUTS/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.165507 rheia-1.1.8/src/rheia/OPT/INPUTS/H2_FUEL/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.283833 rheia-1.1.8/src/rheia/OPT/INPUTS/H2_FUEL/2D/
--rw-rw-rw-   0        0        0      480 2022-09-29 13:16:16.000000 rheia-1.1.8/src/rheia/OPT/INPUTS/H2_FUEL/2D/DOE_n20
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/OPT/__init__.py
--rw-rw-rw-   0        0        0    26704 2023-02-17 14:49:53.000000 rheia-1.1.8/src/rheia/OPT/genetic_algorithms.py
--rw-rw-rw-   0        0        0    10034 2023-02-17 14:50:13.000000 rheia-1.1.8/src/rheia/OPT/optimization.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.299458 rheia-1.1.8/src/rheia/POST_PROCESS/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/POST_PROCESS/__init__.py
--rw-rw-rw-   0        0        0    15406 2022-09-29 10:49:07.000000 rheia-1.1.8/src/rheia/POST_PROCESS/post_process.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.174036 rheia-1.1.8/src/rheia/RESULTS/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.165507 rheia-1.1.8/src/rheia/RESULTS/ENERGYPLAN/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.165507 rheia-1.1.8/src/rheia/RESULTS/ENERGYPLAN/UQ/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.299458 rheia-1.1.8/src/rheia/RESULTS/ENERGYPLAN/UQ/run_1/
--rw-rw-rw-   0        0        0       55 2022-09-29 13:35:00.000000 rheia-1.1.8/src/rheia/RESULTS/ENERGYPLAN/UQ/run_1/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.165507 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.165507 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.299458 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/
--rw-rw-rw-   0        0        0     2014 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/STATUS.txt
--rw-rw-rw-   0        0        0    54885 2022-09-29 13:00:20.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/fitness.csv
--rw-rw-rw-   0        0        0      444 2022-09-29 13:24:56.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/fitness_final_sorted.csv
--rw-rw-rw-   0        0        0    54185 2022-09-29 13:00:37.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/population.csv
--rw-rw-rw-   0        0        0      440 2022-09-29 13:24:56.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/population_final_sorted.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.165507 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.299458 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/
--rw-rw-rw-   0        0        0      720 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/STATUS.txt
--rw-rw-rw-   0        0        0    18078 2022-09-29 13:02:01.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/fitness.csv
--rw-rw-rw-   0        0        0      400 2022-09-29 13:22:55.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/fitness_final_sorted.csv
--rw-rw-rw-   0        0        0    16070 2022-09-29 13:01:52.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/population.csv
--rw-rw-rw-   0        0        0      440 2022-09-29 13:22:55.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/population_final_sorted.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.174036 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.299458 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/
--rw-rw-rw-   0        0        0     3898 2022-09-29 13:19:11.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/data_cdf_lcoh.csv
--rw-rw-rw-   0        0        0     3933 2022-09-29 13:19:11.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/data_pdf_lcoh.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:19:09.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/full_pce_order_2_lcoh.txt
--rw-rw-rw-   0        0        0      682 2022-09-29 13:19:09.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/full_pce_order_2_lcoh_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25375 2022-09-29 12:58:48.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.315082 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      686 2022-09-29 13:21:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:13.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      683 2022-09-29 13:22:13.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25369 2022-09-29 12:58:37.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.315082 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      694 2022-09-29 13:21:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:13.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      688 2022-09-29 13:22:13.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25556 2022-09-29 12:58:26.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.324088 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:18.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      691 2022-09-29 13:22:18.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25547 2022-09-29 12:56:38.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.331101 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:18.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      688 2022-09-29 13:22:18.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25645 2022-09-29 12:56:26.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.331101 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      688 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:19.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      683 2022-09-29 13:22:19.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25598 2022-09-29 12:56:15.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.331101 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      686 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:19.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      682 2022-09-29 13:22:19.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25561 2022-09-29 12:56:02.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.346736 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      692 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:19.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      686 2022-09-29 13:22:19.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25370 2022-09-29 12:55:50.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.346736 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:20.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      688 2022-09-29 13:22:20.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25394 2022-09-29 12:55:38.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.346736 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:20.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      679 2022-09-29 13:22:20.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25373 2022-09-29 12:55:26.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.346736 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:21.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      685 2022-09-29 13:22:21.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25716 2022-09-29 12:55:14.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.362364 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:24.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      690 2022-09-29 13:21:24.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:21.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      695 2022-09-29 13:22:21.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25555 2022-09-29 12:54:51.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.362364 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:24.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      696 2022-09-29 13:21:24.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      685 2022-09-29 13:22:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25738 2022-09-29 12:54:38.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.362364 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      690 2022-09-29 13:21:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:14.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      689 2022-09-29 13:22:14.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25723 2022-09-29 12:58:14.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.377987 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      694 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:14.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      691 2022-09-29 13:22:14.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25668 2022-09-29 12:58:01.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.377987 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      690 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:15.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      687 2022-09-29 13:22:15.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25738 2022-09-29 12:57:44.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.377987 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      682 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:15.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      685 2022-09-29 13:22:15.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25371 2022-09-29 12:57:32.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.393614 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      692 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:16.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      687 2022-09-29 13:22:16.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25549 2022-09-29 12:57:22.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.393614 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      688 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:16.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      688 2022-09-29 13:22:16.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25677 2022-09-29 12:57:12.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.393614 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:17.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      686 2022-09-29 13:22:17.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25562 2022-09-29 12:57:00.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.409237 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/
--rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_1_LCOH.txt
--rw-rw-rw-   0        0        0      692 2022-09-29 13:21:23.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_1_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0      216 2022-09-29 13:22:17.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_2_LCOH.txt
--rw-rw-rw-   0        0        0      693 2022-09-29 13:22:17.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_2_LCOH_Sobol_indices.csv
--rw-rw-rw-   0        0        0    25544 2022-09-29 12:56:49.000000 rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/samples.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.174036 rheia-1.1.8/src/rheia/RESULTS/H2_POWER/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.174036 rheia-1.1.8/src/rheia/RESULTS/H2_POWER/ROB/
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.409237 rheia-1.1.8/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/
--rw-rw-rw-   0        0        0     2952 2022-09-29 14:10:11.000000 rheia-1.1.8/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/STATUS.txt
--rw-rw-rw-   0        0        0    78870 2022-09-29 14:16:15.000000 rheia-1.1.8/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/fitness.csv
--rw-rw-rw-   0        0        0   152385 2022-09-29 14:16:00.000000 rheia-1.1.8/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/population.csv
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.425262 rheia-1.1.8/src/rheia/TESTS/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/TESTS/__init__.py
--rw-rw-rw-   0        0        0     5158 2022-09-29 13:08:34.000000 rheia-1.1.8/src/rheia/TESTS/test_det_stoch_des_space.py
--rw-rw-rw-   0        0        0    10499 2022-09-29 13:06:47.000000 rheia-1.1.8/src/rheia/TESTS/test_genetic_algorithms.py
--rw-rw-rw-   0        0        0     4274 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/TESTS/test_models.py
--rw-rw-rw-   0        0        0     3537 2022-09-29 13:03:24.000000 rheia-1.1.8/src/rheia/TESTS/test_optimization.py
--rw-rw-rw-   0        0        0    12192 2022-09-29 12:01:53.000000 rheia-1.1.8/src/rheia/TESTS/test_pce.py
--rw-rw-rw-   0        0        0     2543 2022-09-29 14:04:24.000000 rheia-1.1.8/src/rheia/TESTS/test_post_process.py
--rw-rw-rw-   0        0        0     1509 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/TESTS/test_uncertainty_quantification.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.440896 rheia-1.1.8/src/rheia/UQ/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/UQ/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.440896 rheia-1.1.8/src/rheia/UQ/__pycache__/
--rw-rw-rw-   0        0        0      154 2022-09-29 13:35:01.000000 rheia-1.1.8/src/rheia/UQ/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0    22498 2022-09-29 13:35:01.000000 rheia-1.1.8/src/rheia/UQ/__pycache__/pce.cpython-38.pyc
--rw-rw-rw-   0        0        0     5280 2022-09-29 13:35:01.000000 rheia-1.1.8/src/rheia/UQ/__pycache__/uncertainty_quantification.cpython-38.pyc
--rw-rw-rw-   0        0        0    34093 2022-11-14 15:51:29.000000 rheia-1.1.8/src/rheia/UQ/pce.py
--rw-rw-rw-   0        0        0     7576 2022-11-11 14:21:11.000000 rheia-1.1.8/src/rheia/UQ/uncertainty_quantification.py
--rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.8/src/rheia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 14:52:07.174036 rheia-1.1.8/src/rheia.egg-info/
--rw-rw-rw-   0        0        0      565 2023-02-17 14:52:07.000000 rheia-1.1.8/src/rheia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13101 2023-02-17 14:52:07.000000 rheia-1.1.8/src/rheia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 14:52:07.000000 rheia-1.1.8/src/rheia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-17 14:52:06.000000 rheia-1.1.8/src/rheia.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      131 2023-02-17 14:52:07.000000 rheia-1.1.8/src/rheia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-17 14:52:07.000000 rheia-1.1.8/src/rheia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.149235 rheia-1.1.9/
+-rw-rw-rw-   0        0        0     1095 2021-03-17 10:06:00.000000 rheia-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       16 2021-01-06 11:48:13.000000 rheia-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      565 2023-05-10 15:21:27.148235 rheia-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1008 2021-07-15 07:42:37.000000 rheia-1.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-17 10:15:07.000000 rheia-1.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 15:21:27.149235 rheia-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-05-10 15:20:56.000000 rheia-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.921568 rheia-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.942994 rheia-1.1.9/src/rheia/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.953754 rheia-1.1.9/src/rheia/CASES/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.921568 rheia-1.1.9/src/rheia/CASES/DATA/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.953754 rheia-1.1.9/src/rheia/CASES/DATA/climate/
+-rw-rw-rw-   0        0        0    71681 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/DATA/climate/climate_Brussels.CSV
+-rw-rw-rw-   0        0        0    71577 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/DATA/climate/climate_Madrid.CSV
+-rw-rw-rw-   0        0        0    72055 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/DATA/climate/climate_Paris.CSV
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.953754 rheia-1.1.9/src/rheia/CASES/DATA/demand/
+-rw-rw-rw-   0        0        0   112890 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/DATA/demand/load_Brussels_dwelling.csv
+-rw-rw-rw-   0        0        0   113023 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/DATA/demand/load_Madrid_dwelling.csv
+-rw-rw-rw-   0        0        0   112964 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/DATA/demand/load_Paris_dwelling.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.953754 rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/__init__.py
+-rw-rw-rw-   0        0        0    29012 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/case.txt
+-rw-rw-rw-   0        0        0     1096 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/case_description.py
+-rw-rw-rw-   0        0        0       89 2022-09-29 11:47:02.000000 rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/design_space.csv
+-rw-rw-rw-   0        0        0     4870 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/run_energyplan.py
+-rw-rw-rw-   0        0        0      154 2022-09-29 11:47:24.000000 rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/stochastic_space.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.973490 rheia-1.1.9/src/rheia/CASES/FOUR_BAR_TRUSS/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/FOUR_BAR_TRUSS/__init__.py
+-rw-rw-rw-   0        0        0     1111 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/FOUR_BAR_TRUSS/case_description.py
+-rw-rw-rw-   0        0        0      145 2022-09-29 11:46:13.000000 rheia-1.1.9/src/rheia/CASES/FOUR_BAR_TRUSS/design_space.csv
+-rw-rw-rw-   0        0        0      970 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/FOUR_BAR_TRUSS/four_bar_truss.py
+-rw-rw-rw-   0        0        0      129 2022-09-29 11:31:59.000000 rheia-1.1.9/src/rheia/CASES/FOUR_BAR_TRUSS/stochastic_space.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.989478 rheia-1.1.9/src/rheia/CASES/H2_FUEL/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.989478 rheia-1.1.9/src/rheia/CASES/H2_FUEL/__pycache__/
+-rw-rw-rw-   0        0        0      165 2022-09-29 13:24:41.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0     1938 2022-09-29 13:24:41.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/__pycache__/case_description.cpython-38.pyc
+-rw-rw-rw-   0        0        0    15321 2022-09-29 13:24:41.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/__pycache__/h2_fuel.cpython-38.pyc
+-rw-rw-rw-   0        0        0     2115 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/case_description.py
+-rw-rw-rw-   0        0        0      280 2022-09-29 11:54:50.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:51:33.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_0.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:51:51.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_1.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:55:40.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_10.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:55:20.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_11.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:55:06.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_12.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:54:32.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_13.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:54:18.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_14.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:54:03.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_15.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:53:47.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_16.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:50:33.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_17.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:50:07.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_18.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:50:57.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_19.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:52:07.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_2.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:52:23.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_3.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:52:40.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_4.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:52:57.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_5.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:53:12.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_6.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:53:29.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_7.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:49:39.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_8.csv
+-rw-rw-rw-   0        0        0      292 2022-09-29 11:56:01.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_9.csv
+-rw-rw-rw-   0        0        0      282 2022-09-29 11:51:17.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/design_space_tutorial_uq.csv
+-rw-rw-rw-   0        0        0    19598 2022-09-29 13:05:42.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/h2_fuel.py
+-rw-rw-rw-   0        0        0      389 2022-09-29 11:56:36.000000 rheia-1.1.9/src/rheia/CASES/H2_FUEL/stochastic_space.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.008858 rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/__init__.py
+-rw-rw-rw-   0        0        0     2473 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/case_description.py
+-rw-rw-rw-   0        0        0     1029 2022-09-29 11:58:09.000000 rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/design_space.csv
+-rw-rw-rw-   0        0        0    40333 2022-09-29 13:05:37.000000 rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/h2_mobility.py
+-rw-rw-rw-   0        0        0      822 2022-09-29 11:58:03.000000 rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/stochastic_space.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.010837 rheia-1.1.9/src/rheia/CASES/H2_POWER/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/H2_POWER/__init__.py
+-rw-rw-rw-   0        0        0     2530 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/H2_POWER/case_description.py
+-rw-rw-rw-   0        0        0      572 2022-09-29 11:57:36.000000 rheia-1.1.9/src/rheia/CASES/H2_POWER/design_space.csv
+-rw-rw-rw-   0        0        0    35668 2022-09-29 13:05:33.000000 rheia-1.1.9/src/rheia/CASES/H2_POWER/h2_power.py
+-rw-rw-rw-   0        0        0      800 2022-09-29 11:57:53.000000 rheia-1.1.9/src/rheia/CASES/H2_POWER/stochastic_space.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.010837 rheia-1.1.9/src/rheia/CASES/NO_MODEL/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/NO_MODEL/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/NO_MODEL/case_description.py
+-rw-rw-rw-   0        0        0       25 2022-09-29 11:58:40.000000 rheia-1.1.9/src/rheia/CASES/NO_MODEL/design_space.csv
+-rw-rw-rw-   0        0        0       50 2022-09-29 11:58:51.000000 rheia-1.1.9/src/rheia/CASES/NO_MODEL/stochastic_space.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.022510 rheia-1.1.9/src/rheia/CASES/REF/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/REF/__init__.py
+-rw-rw-rw-   0        0        0     1271 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/REF/case_description.py
+-rw-rw-rw-   0        0        0       26 2022-09-29 11:59:25.000000 rheia-1.1.9/src/rheia/CASES/REF/design_space.csv
+-rw-rw-rw-   0        0        0       51 2022-09-29 11:59:16.000000 rheia-1.1.9/src/rheia/CASES/REF/stochastic_space.csv
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/CASES/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.026520 rheia-1.1.9/src/rheia/CASES/__pycache__/
+-rw-rw-rw-   0        0        0      157 2022-09-29 13:35:01.000000 rheia-1.1.9/src/rheia/CASES/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    15662 2022-09-29 13:35:01.000000 rheia-1.1.9/src/rheia/CASES/__pycache__/determine_stoch_des_space.cpython-38.pyc
+-rw-rw-rw-   0        0        0    22514 2022-09-29 11:46:22.000000 rheia-1.1.9/src/rheia/CASES/determine_stoch_des_space.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.028923 rheia-1.1.9/src/rheia/OPT/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.921568 rheia-1.1.9/src/rheia/OPT/INPUTS/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.921568 rheia-1.1.9/src/rheia/OPT/INPUTS/H2_FUEL/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.028923 rheia-1.1.9/src/rheia/OPT/INPUTS/H2_FUEL/2D/
+-rw-rw-rw-   0        0        0      480 2022-09-29 13:16:16.000000 rheia-1.1.9/src/rheia/OPT/INPUTS/H2_FUEL/2D/DOE_n20
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/OPT/__init__.py
+-rw-rw-rw-   0        0        0    26634 2023-05-10 15:10:55.000000 rheia-1.1.9/src/rheia/OPT/genetic_algorithms.py
+-rw-rw-rw-   0        0        0    10034 2023-02-17 14:50:13.000000 rheia-1.1.9/src/rheia/OPT/optimization.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.028923 rheia-1.1.9/src/rheia/POST_PROCESS/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/POST_PROCESS/__init__.py
+-rw-rw-rw-   0        0        0    15406 2022-09-29 10:49:07.000000 rheia-1.1.9/src/rheia/POST_PROCESS/post_process.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.942994 rheia-1.1.9/src/rheia/RESULTS/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.921568 rheia-1.1.9/src/rheia/RESULTS/ENERGYPLAN/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.921568 rheia-1.1.9/src/rheia/RESULTS/ENERGYPLAN/UQ/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.036169 rheia-1.1.9/src/rheia/RESULTS/ENERGYPLAN/UQ/run_1/
+-rw-rw-rw-   0        0        0       55 2022-09-29 13:35:00.000000 rheia-1.1.9/src/rheia/RESULTS/ENERGYPLAN/UQ/run_1/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.936203 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.921568 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.039184 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/
+-rw-rw-rw-   0        0        0     2014 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/STATUS.txt
+-rw-rw-rw-   0        0        0    54885 2022-09-29 13:00:20.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/fitness.csv
+-rw-rw-rw-   0        0        0      444 2022-09-29 13:24:56.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/fitness_final_sorted.csv
+-rw-rw-rw-   0        0        0    54185 2022-09-29 13:00:37.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/population.csv
+-rw-rw-rw-   0        0        0      440 2022-09-29 13:24:56.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/population_final_sorted.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.936203 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.043182 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/
+-rw-rw-rw-   0        0        0      720 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/STATUS.txt
+-rw-rw-rw-   0        0        0    18078 2022-09-29 13:02:01.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/fitness.csv
+-rw-rw-rw-   0        0        0      400 2022-09-29 13:22:55.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/fitness_final_sorted.csv
+-rw-rw-rw-   0        0        0    16070 2022-09-29 13:01:52.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/population.csv
+-rw-rw-rw-   0        0        0      440 2022-09-29 13:22:55.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/population_final_sorted.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.942994 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.046174 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/
+-rw-rw-rw-   0        0        0     3898 2022-09-29 13:19:11.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/data_cdf_lcoh.csv
+-rw-rw-rw-   0        0        0     3933 2022-09-29 13:19:11.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/data_pdf_lcoh.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:19:09.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/full_pce_order_2_lcoh.txt
+-rw-rw-rw-   0        0        0      682 2022-09-29 13:19:09.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/full_pce_order_2_lcoh_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25375 2022-09-29 12:58:48.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.049182 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      686 2022-09-29 13:21:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:13.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      683 2022-09-29 13:22:13.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25369 2022-09-29 12:58:37.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.053176 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      694 2022-09-29 13:21:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:13.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      688 2022-09-29 13:22:13.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25556 2022-09-29 12:58:26.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.054387 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:18.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      691 2022-09-29 13:22:18.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25547 2022-09-29 12:56:38.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.054387 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:18.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      688 2022-09-29 13:22:18.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25645 2022-09-29 12:56:26.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.054387 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      688 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:19.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      683 2022-09-29 13:22:19.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25598 2022-09-29 12:56:15.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.054387 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      686 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:19.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      682 2022-09-29 13:22:19.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25561 2022-09-29 12:56:02.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.070013 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      692 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:19.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      686 2022-09-29 13:22:19.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25370 2022-09-29 12:55:50.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.070013 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:20.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      688 2022-09-29 13:22:20.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25394 2022-09-29 12:55:38.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.070013 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:20.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      679 2022-09-29 13:22:20.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25373 2022-09-29 12:55:26.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.070013 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:21.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      685 2022-09-29 13:22:21.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25716 2022-09-29 12:55:14.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.070013 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:24.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      690 2022-09-29 13:21:24.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:21.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      695 2022-09-29 13:22:21.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25555 2022-09-29 12:54:51.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.085637 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:24.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      696 2022-09-29 13:21:24.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      685 2022-09-29 13:22:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25738 2022-09-29 12:54:38.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.089642 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      690 2022-09-29 13:21:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:14.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      689 2022-09-29 13:22:14.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25723 2022-09-29 12:58:14.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.089642 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      694 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:14.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      691 2022-09-29 13:22:14.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25668 2022-09-29 12:58:01.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.089642 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      690 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:15.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      687 2022-09-29 13:22:15.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25738 2022-09-29 12:57:44.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.103837 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      682 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:15.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      685 2022-09-29 13:22:15.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25371 2022-09-29 12:57:32.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.106834 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      692 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:16.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      687 2022-09-29 13:22:16.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25549 2022-09-29 12:57:22.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.110003 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      688 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:16.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      688 2022-09-29 13:22:16.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25677 2022-09-29 12:57:12.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.110003 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      684 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:17.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      686 2022-09-29 13:22:17.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25562 2022-09-29 12:57:00.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.110003 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_1_LCOH.txt
+-rw-rw-rw-   0        0        0      692 2022-09-29 13:21:23.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_1_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0      216 2022-09-29 13:22:17.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_2_LCOH.txt
+-rw-rw-rw-   0        0        0      693 2022-09-29 13:22:17.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_2_LCOH_Sobol_indices.csv
+-rw-rw-rw-   0        0        0    25544 2022-09-29 12:56:49.000000 rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/samples.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.942994 rheia-1.1.9/src/rheia/RESULTS/H2_POWER/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.942994 rheia-1.1.9/src/rheia/RESULTS/H2_POWER/ROB/
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.120509 rheia-1.1.9/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/
+-rw-rw-rw-   0        0        0     2952 2022-09-29 14:10:11.000000 rheia-1.1.9/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/STATUS.txt
+-rw-rw-rw-   0        0        0    78870 2022-09-29 14:16:15.000000 rheia-1.1.9/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/fitness.csv
+-rw-rw-rw-   0        0        0   152385 2022-09-29 14:16:00.000000 rheia-1.1.9/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/population.csv
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.137229 rheia-1.1.9/src/rheia/TESTS/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/TESTS/__init__.py
+-rw-rw-rw-   0        0        0     5158 2022-09-29 13:08:34.000000 rheia-1.1.9/src/rheia/TESTS/test_det_stoch_des_space.py
+-rw-rw-rw-   0        0        0    10499 2022-09-29 13:06:47.000000 rheia-1.1.9/src/rheia/TESTS/test_genetic_algorithms.py
+-rw-rw-rw-   0        0        0     4274 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/TESTS/test_models.py
+-rw-rw-rw-   0        0        0     3537 2022-09-29 13:03:24.000000 rheia-1.1.9/src/rheia/TESTS/test_optimization.py
+-rw-rw-rw-   0        0        0    12192 2022-09-29 12:01:53.000000 rheia-1.1.9/src/rheia/TESTS/test_pce.py
+-rw-rw-rw-   0        0        0     2543 2022-09-29 14:04:24.000000 rheia-1.1.9/src/rheia/TESTS/test_post_process.py
+-rw-rw-rw-   0        0        0     1509 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/TESTS/test_uncertainty_quantification.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.142235 rheia-1.1.9/src/rheia/UQ/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/UQ/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:27.147226 rheia-1.1.9/src/rheia/UQ/__pycache__/
+-rw-rw-rw-   0        0        0      154 2022-09-29 13:35:01.000000 rheia-1.1.9/src/rheia/UQ/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0    22498 2022-09-29 13:35:01.000000 rheia-1.1.9/src/rheia/UQ/__pycache__/pce.cpython-38.pyc
+-rw-rw-rw-   0        0        0     5280 2022-09-29 13:35:01.000000 rheia-1.1.9/src/rheia/UQ/__pycache__/uncertainty_quantification.cpython-38.pyc
+-rw-rw-rw-   0        0        0    34093 2022-11-14 15:51:29.000000 rheia-1.1.9/src/rheia/UQ/pce.py
+-rw-rw-rw-   0        0        0     7576 2022-11-11 14:21:11.000000 rheia-1.1.9/src/rheia/UQ/uncertainty_quantification.py
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:41:49.000000 rheia-1.1.9/src/rheia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:21:26.942994 rheia-1.1.9/src/rheia.egg-info/
+-rw-rw-rw-   0        0        0      565 2023-05-10 15:21:26.000000 rheia-1.1.9/src/rheia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13101 2023-05-10 15:21:26.000000 rheia-1.1.9/src/rheia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 15:21:26.000000 rheia-1.1.9/src/rheia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 15:21:26.000000 rheia-1.1.9/src/rheia.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      131 2023-05-10 15:21:26.000000 rheia-1.1.9/src/rheia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 15:21:26.000000 rheia-1.1.9/src/rheia.egg-info/top_level.txt
```

### Comparing `rheia-1.1.8/LICENSE` & `rheia-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/PKG-INFO` & `rheia-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rheia
-Version: 1.1.8
+Version: 1.1.9
 Summary: Robust design optimization of renewable Hydrogen and dErIved energy cArrier systems
 Home-page: https://github.com/rheia-framework/RHEIA
 Author: Diederik Coppitters, Panagiotis Tsirikoglou, Ward De Paepe, Konstantinos Kyprianidis, Anestis Kalfas, Francesco Contino
 Author-email: rheia.framework@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `rheia-1.1.8/README.md` & `rheia-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/setup.py` & `rheia-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='rheia',
-      version='1.1.8',
+      version='1.1.9',
       description='Robust design optimization of renewable Hydrogen and dErIved energy cArrier systems',
       url='https://github.com/rheia-framework/RHEIA',
       author='Diederik Coppitters, Panagiotis Tsirikoglou, Ward De Paepe, Konstantinos Kyprianidis, Anestis Kalfas, Francesco Contino',
       author_email='rheia.framework@gmail.com',
       package_dir={"": "src"},
       packages= setuptools.find_packages(where="src"),
       classifiers=[
                 "Programming Language :: Python :: 3",
                 "License :: OSI Approved :: MIT License",
                 "Operating System :: OS Independent",
       ],       
       install_requires=[
       'pyDOE>=0.3.8',
-      'deap==1.3.1',
+      'deap>=1.3.1',
       'numpy>=1.24.1',
       'scipy>=1.10.0',
       'sobolsequence>=0.2.1',
       'pandas>=1.5.3',
       'matplotlib>=3.2.2',
       'pvlib>=0.9.4',
       'h5py>=3.8.0'
       ],
-      python_requires = ">=3.6",
+      python_requires = ">=3.8",
       include_package_data=True,
       zip_safe=False)
```

### Comparing `rheia-1.1.8/src/rheia/CASES/DATA/climate/climate_Brussels.CSV` & `rheia-1.1.9/src/rheia/CASES/DATA/climate/climate_Brussels.CSV`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/DATA/climate/climate_Madrid.CSV` & `rheia-1.1.9/src/rheia/CASES/DATA/climate/climate_Madrid.CSV`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/DATA/climate/climate_Paris.CSV` & `rheia-1.1.9/src/rheia/CASES/DATA/climate/climate_Paris.CSV`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/DATA/demand/load_Brussels_dwelling.csv` & `rheia-1.1.9/src/rheia/CASES/DATA/demand/load_Brussels_dwelling.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/DATA/demand/load_Madrid_dwelling.csv` & `rheia-1.1.9/src/rheia/CASES/DATA/demand/load_Madrid_dwelling.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/DATA/demand/load_Paris_dwelling.csv` & `rheia-1.1.9/src/rheia/CASES/DATA/demand/load_Paris_dwelling.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/case.txt` & `rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/case.txt`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/case_description.py` & `rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/case_description.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/ENERGYPLAN/run_energyplan.py` & `rheia-1.1.9/src/rheia/CASES/ENERGYPLAN/run_energyplan.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/FOUR_BAR_TRUSS/case_description.py` & `rheia-1.1.9/src/rheia/CASES/FOUR_BAR_TRUSS/case_description.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/FOUR_BAR_TRUSS/four_bar_truss.py` & `rheia-1.1.9/src/rheia/CASES/FOUR_BAR_TRUSS/four_bar_truss.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_FUEL/__pycache__/case_description.cpython-38.pyc` & `rheia-1.1.9/src/rheia/CASES/H2_FUEL/__pycache__/case_description.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_FUEL/__pycache__/h2_fuel.cpython-38.pyc` & `rheia-1.1.9/src/rheia/CASES/H2_FUEL/__pycache__/h2_fuel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_FUEL/case_description.py` & `rheia-1.1.9/src/rheia/CASES/H2_FUEL/case_description.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_FUEL/h2_fuel.py` & `rheia-1.1.9/src/rheia/CASES/H2_FUEL/h2_fuel.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/case_description.py` & `rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/case_description.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/design_space.csv` & `rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/design_space.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/h2_mobility.py` & `rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/h2_mobility.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_MOBILITY/stochastic_space.csv` & `rheia-1.1.9/src/rheia/CASES/H2_MOBILITY/stochastic_space.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_POWER/case_description.py` & `rheia-1.1.9/src/rheia/CASES/H2_POWER/case_description.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_POWER/design_space.csv` & `rheia-1.1.9/src/rheia/CASES/H2_POWER/design_space.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_POWER/h2_power.py` & `rheia-1.1.9/src/rheia/CASES/H2_POWER/h2_power.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/H2_POWER/stochastic_space.csv` & `rheia-1.1.9/src/rheia/CASES/H2_POWER/stochastic_space.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/REF/case_description.py` & `rheia-1.1.9/src/rheia/CASES/REF/case_description.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/__pycache__/determine_stoch_des_space.cpython-38.pyc` & `rheia-1.1.9/src/rheia/CASES/__pycache__/determine_stoch_des_space.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/CASES/determine_stoch_des_space.py` & `rheia-1.1.9/src/rheia/CASES/determine_stoch_des_space.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/OPT/genetic_algorithms.py` & `rheia-1.1.9/src/rheia/OPT/genetic_algorithms.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,20 +143,20 @@
         file_dir = os.path.join(self.opt_res_dir, filename)
                 
         dummy = ['-']
 
         df = pd.DataFrame(nests, columns=None)
         
         with open(file_dir, 'a') as f:
-             df.to_csv(f, header=False, index=False, line_terminator='\n')
+             df.to_csv(f, header=False, index=False, lineterminator='\n')
 
         df2 = pd.DataFrame(dummy, columns=None)
 
         with open(file_dir, 'a') as f:
-             df2.to_csv(f, header=False, index=False, line_terminator='\n')
+             df2.to_csv(f, header=False, index=False, lineterminator='\n')
         
         '''
         with open(file_dir, 'a') as file:
 
             for n_in in nests:
 
                 for item in n_in:
@@ -235,23 +235,22 @@
                 my_data = uq.Data(self.run_dict, self.space_obj)
 
                 # acquire information on stochastic parameters
                 my_data.read_stoch_parameters(
                     var_values=sample[-len(self.space_obj.var_dict):])
 
                 # array for the number of quantities of interest considered
-                self.objective_position = np.zeros(
-                    len(self.run_dict['objective names']))
+                self.objective_position = []
                 for index, obj in enumerate(
                         self.run_dict['objective of interest']):
 
                     # for each quantity of interest, determine its position
                     # in the list
-                    self.objective_position[index] = self.run_dict[
-                        'objective names'].index(obj)
+                    self.objective_position.append(self.run_dict[
+                        'objective names'].index(obj))
 
                 # generate a random experiment for the quantity of interest
                 self.my_experiment = uq.RandomExperiment(
                     my_data, self.objective_position)
 
                 # create uniform/gaussian distributions and corresponding
                 # orthogonal polynomials
```

### Comparing `rheia-1.1.8/src/rheia/OPT/optimization.py` & `rheia-1.1.9/src/rheia/OPT/optimization.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/POST_PROCESS/post_process.py` & `rheia-1.1.9/src/rheia/POST_PROCESS/post_process.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/STATUS.txt` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/STATUS.txt`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/fitness.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/fitness.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/population.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/DET/run_tutorial/population.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/STATUS.txt` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/STATUS.txt`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/fitness.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/fitness.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/population.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/ROB/run_tutorial/population.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/data_cdf_lcoh.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/data_cdf_lcoh.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/data_pdf_lcoh.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/data_pdf_lcoh.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/full_pce_order_2_lcoh_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/full_pce_order_2_lcoh_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/opt_design_tutorial/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_0/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_1/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_10/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_11/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_12/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_13/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_14/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_15/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_16/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_17/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_18/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_19/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_2/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_3/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_4/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_5/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_6/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_7/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_8/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_1_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_1_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_2_LCOH_Sobol_indices.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/full_pce_order_2_LCOH_Sobol_indices.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/samples.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_FUEL/UQ/sample_tutorial_9/samples.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/STATUS.txt` & `rheia-1.1.9/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/STATUS.txt`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/fitness.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/fitness.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/population.csv` & `rheia-1.1.9/src/rheia/RESULTS/H2_POWER/ROB/run_tutorial/population.csv`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/TESTS/test_det_stoch_des_space.py` & `rheia-1.1.9/src/rheia/TESTS/test_det_stoch_des_space.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/TESTS/test_genetic_algorithms.py` & `rheia-1.1.9/src/rheia/TESTS/test_genetic_algorithms.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/TESTS/test_models.py` & `rheia-1.1.9/src/rheia/TESTS/test_models.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/TESTS/test_optimization.py` & `rheia-1.1.9/src/rheia/TESTS/test_optimization.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/TESTS/test_pce.py` & `rheia-1.1.9/src/rheia/TESTS/test_pce.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/TESTS/test_post_process.py` & `rheia-1.1.9/src/rheia/TESTS/test_post_process.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/TESTS/test_uncertainty_quantification.py` & `rheia-1.1.9/src/rheia/TESTS/test_uncertainty_quantification.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/UQ/__pycache__/pce.cpython-38.pyc` & `rheia-1.1.9/src/rheia/UQ/__pycache__/pce.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/UQ/__pycache__/uncertainty_quantification.cpython-38.pyc` & `rheia-1.1.9/src/rheia/UQ/__pycache__/uncertainty_quantification.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/UQ/pce.py` & `rheia-1.1.9/src/rheia/UQ/pce.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia/UQ/uncertainty_quantification.py` & `rheia-1.1.9/src/rheia/UQ/uncertainty_quantification.py`

 * *Files identical despite different names*

### Comparing `rheia-1.1.8/src/rheia.egg-info/PKG-INFO` & `rheia-1.1.9/src/rheia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rheia
-Version: 1.1.8
+Version: 1.1.9
 Summary: Robust design optimization of renewable Hydrogen and dErIved energy cArrier systems
 Home-page: https://github.com/rheia-framework/RHEIA
 Author: Diederik Coppitters, Panagiotis Tsirikoglou, Ward De Paepe, Konstantinos Kyprianidis, Anestis Kalfas, Francesco Contino
 Author-email: rheia.framework@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `rheia-1.1.8/src/rheia.egg-info/SOURCES.txt` & `rheia-1.1.9/src/rheia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

