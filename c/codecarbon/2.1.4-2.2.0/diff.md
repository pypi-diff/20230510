# Comparing `tmp/codecarbon-2.1.4.tar.gz` & `tmp/codecarbon-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecarbon-2.1.4.tar", last modified: Mon Sep  5 05:31:33 2022, max compression
+gzip compressed data, was "codecarbon-2.2.0.tar", last modified: Wed May 10 21:13:19 2023, max compression
```

## Comparing `codecarbon-2.1.4.tar` & `codecarbon-2.2.0.tar`

### file list

```diff
@@ -1,99 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.257274 codecarbon-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-05 05:31:19.000000 codecarbon-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    17745 2022-09-05 05:31:33.257274 codecarbon-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17330 2022-09-05 05:31:19.000000 codecarbon-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.241274 codecarbon-2.1.4/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.245274 codecarbon-2.1.4/carbonserver/carbonserver/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.245274 codecarbon-2.1.4/carbonserver/carbonserver/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.245274 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/emissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/experiments.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/organizations.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/runs.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/teams.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/domain/users.py
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.245274 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/emissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2872 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/organizations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2320 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/runs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/teams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/routers/users.py
--rw-r--r--   0 runner    (1001) docker     (121)     9140 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.249274 codecarbon-2.1.4/carbonserver/carbonserver/database/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/database/database.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/carbonserver/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4162 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-09-05 05:31:19.000000 codecarbon-2.1.4/carbonserver/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.249274 codecarbon-2.1.4/codecarbon/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.249274 codecarbon-2.1.4/codecarbon/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.253274 codecarbon-2.1.4/codecarbon/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6268 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/co2_signal.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    13895 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (121)    11305 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/emissions.py
--rw-r--r--   0 runner    (1001) docker     (121)     7478 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1914 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/rapl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.241274 codecarbon-2.1.4/codecarbon/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.253274 codecarbon-2.1.4/codecarbon/data/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)    11411 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/data/cloud/impact.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.253274 codecarbon-2.1.4/codecarbon/data/hardware/
--rw-r--r--   0 runner    (1001) docker     (121)    49152 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/data/hardware/cpu_power.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.253274 codecarbon-2.1.4/codecarbon/data/private_infra/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.253274 codecarbon-2.1.4/codecarbon/data/private_infra/2016/
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/data/private_infra/2016/canada_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/data/private_infra/2016/usa_emissions.json
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/data/private_infra/carbon_intensity_per_source.json
--rw-r--r--   0 runner    (1001) docker     (121)    81312 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/data/private_infra/global_energy_mix.json
--rw-r--r--   0 runner    (1001) docker     (121)    36364 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/emissions_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.253274 codecarbon-2.1.4/codecarbon/external/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3243 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/external/geography.py
--rw-r--r--   0 runner    (1001) docker     (121)    11082 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/external/hardware.py
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/external/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/external/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4352 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/input.py
--rw-r--r--   0 runner    (1001) docker     (121)     6821 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.253274 codecarbon-2.1.4/codecarbon/viz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.257274 codecarbon-2.1.4/codecarbon/viz/assets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25442 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/assets/car_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)    29734 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/assets/house_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)    29874 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/assets/tv_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)    11040 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/carbonboard.py
--rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/carbonboard_on_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    28039 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/components.py
--rw-r--r--   0 runner    (1001) docker     (121)    11366 2022-09-05 05:31:19.000000 codecarbon-2.1.4/codecarbon/viz/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 05:31:33.249274 codecarbon-2.1.4/codecarbon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    17745 2022-09-05 05:31:33.000000 codecarbon-2.1.4/codecarbon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-09-05 05:31:33.000000 codecarbon-2.1.4/codecarbon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 05:31:33.000000 codecarbon-2.1.4/codecarbon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-05 05:31:33.000000 codecarbon-2.1.4/codecarbon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-05 05:31:33.000000 codecarbon-2.1.4/codecarbon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-05 05:31:33.000000 codecarbon-2.1.4/codecarbon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 05:31:33.257274 codecarbon-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-09-05 05:31:19.000000 codecarbon-2.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.224247 codecarbon-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 21:13:03.000000 codecarbon-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-10 21:13:19.224247 codecarbon-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-10 21:13:03.000000 codecarbon-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.204246 codecarbon-2.2.0/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.204246 codecarbon-2.2.0/carbonserver/carbonserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.204246 codecarbon-2.2.0/carbonserver/carbonserver/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.208246 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/domain/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.208246 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/routers/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.208246 codecarbon-2.2.0/carbonserver/carbonserver/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/carbonserver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-10 21:13:03.000000 codecarbon-2.2.0/carbonserver/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.208246 codecarbon-2.2.0/codecarbon/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.212246 codecarbon-2.2.0/codecarbon/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.216246 codecarbon-2.2.0/codecarbon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/rapl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.204246 codecarbon-2.2.0/codecarbon/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.216246 codecarbon-2.2.0/codecarbon/data/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/data/cloud/impact.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.216246 codecarbon-2.2.0/codecarbon/data/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)    49423 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/data/hardware/cpu_power.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.216246 codecarbon-2.2.0/codecarbon/data/private_infra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.216246 codecarbon-2.2.0/codecarbon/data/private_infra/2016/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/data/private_infra/2016/canada_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/data/private_infra/2016/usa_emissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/data/private_infra/carbon_intensity_per_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)    81313 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/data/private_infra/global_energy_mix.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37320 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/emissions_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.216246 codecarbon-2.2.0/codecarbon/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/external/geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/external/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/external/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/external/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.220247 codecarbon-2.2.0/codecarbon/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.220247 codecarbon-2.2.0/codecarbon/viz/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25442 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/assets/car_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/assets/house_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29874 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/assets/tv_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/carbonboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/carbonboard_on_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27905 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-10 21:13:03.000000 codecarbon-2.2.0/codecarbon/viz/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.212246 codecarbon-2.2.0/codecarbon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-10 21:13:19.000000 codecarbon-2.2.0/codecarbon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-10 21:13:19.000000 codecarbon-2.2.0/codecarbon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:13:19.000000 codecarbon-2.2.0/codecarbon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-10 21:13:19.000000 codecarbon-2.2.0/codecarbon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 21:13:19.000000 codecarbon-2.2.0/codecarbon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 21:13:19.000000 codecarbon-2.2.0/codecarbon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:13:19.224247 codecarbon-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-10 21:13:03.000000 codecarbon-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:13:19.224247 codecarbon-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_co2_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_core_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_emissions_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_emissions_tracker_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_emissions_tracker_flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_geography.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_logging_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/test_ram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-10 21:13:03.000000 codecarbon-2.2.0/tests/testutils.py
```

### Comparing `codecarbon-2.1.4/LICENSE` & `codecarbon-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/dependencies.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/dependencies.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/domain/experiments.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/domain/experiments.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/errors.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 from dataclasses import dataclass
 from enum import Enum
 
 
+class EmptyResultException(Exception):
+    """
+    The request return an empty result.
+    """
+
+    pass
+
+
 @dataclass
 class ErrorBase:
     code: str
     message: str
 
 
 class DBErrorEnum(Enum):
```

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/routers/authenticate.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/routers/authenticate.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,12 +21,11 @@
 def auth_user(
     user: UserAuthenticate,
     user_service: UserService = Depends(Provide[ServerContainer.user_service]),
 ) -> Token:
     verified_user = user_service.verify_user(user)
     if verified_user:
         return Token(access_token="a", token_type="access")
-    else:
-        raise HTTPException(
-            status_code=status.HTTP_401_UNAUTHORIZED,
-            detail="Incorrect password or email!",
-        )
+    raise HTTPException(
+        status_code=status.HTTP_401_UNAUTHORIZED,
+        detail="Incorrect password or email!",
+    )
```

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/routers/emissions.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/routers/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/routers/experiments.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/routers/experiments.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 @inject
 def read_project_experiments(
     project_id: str,
     experiment_service: ExperimentService = Depends(
         Provide[ServerContainer.experiment_service]
     ),
 ) -> List[Experiment]:
-
     return experiment_service.get_experiments_from_project(project_id)
 
 
 @router.get(
     "/experiments/{project_id}/sums/",
     tags=EXPERIMENTS_ROUTER_TAGS,
     status_code=status.HTTP_200_OK,
```

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/routers/organizations.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/routers/organizations.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/routers/projects.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/routers/projects.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/routers/runs.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/routers/runs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from datetime import datetime, timedelta
-from typing import List, Optional
+from typing import List, Optional, Union
 
 import dateutil.relativedelta
 from container import ServerContainer
 from dependency_injector.wiring import Provide, inject
 from fastapi import APIRouter, Depends
 from starlette import status
 
 from carbonserver.api.dependencies import get_token_header
-from carbonserver.api.schemas import Run, RunCreate, RunReport
+from carbonserver.api.errors import EmptyResultException
+from carbonserver.api.schemas import Empty, Run, RunCreate, RunReport
 from carbonserver.api.services.run_service import RunService
 from carbonserver.api.usecases.run.experiment_sum_by_run import (
     ExperimentSumsByRunUsecase,
 )
+from carbonserver.logger import logger
 
 RUNS_ROUTER_TAGS = ["Runs"]
 
 router = APIRouter(
     dependencies=[Depends(get_token_header)],
 )
 runs_temp_db = []
@@ -101,23 +103,27 @@
     )
 
 
 @router.get(
     "/lastrun/project/{project_id}",
     tags=RUNS_ROUTER_TAGS,
     status_code=status.HTTP_200_OK,
-    response_model=Run,
+    response_model=Union[Run, Empty],
 )
 @inject
 def read_project_last_run(
     project_id: str,
     start_date: Optional[datetime] = None,
     end_date: Optional[datetime] = None,
     run_service: RunService = Depends(Provide[ServerContainer.run_service]),
-) -> Run:
+) -> Union[Run, Empty]:
     start_date = (
         start_date
         if start_date
         else datetime.now() - dateutil.relativedelta.relativedelta(months=3)
     )
     end_date = end_date if end_date else datetime.now() + timedelta(days=1)
-    return run_service.read_project_last_run(project_id, start_date, end_date)
+    try:
+        return run_service.read_project_last_run(project_id, start_date, end_date)
+    except EmptyResultException as e:
+        logger.warning(f"read_project_last_run : {e}")
+        return Empty()
```

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/routers/teams.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/routers/teams.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/routers/users.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/routers/users.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/api/schemas.py` & `codecarbon-2.2.0/carbonserver/carbonserver/api/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 So this will help us avoiding confusion while using both.
 """
 
 from datetime import datetime
 from typing import List, Optional
 from uuid import UUID
 
-from pydantic import BaseModel, EmailStr, Field, SecretStr
+from pydantic import BaseModel, EmailStr, Extra, Field, SecretStr
+
+
+class Empty(BaseModel, extra=Extra.forbid):
+    pass
 
 
 class EmissionBase(BaseModel):
     timestamp: datetime
     run_id: UUID
     duration: int = Field(
         ..., gt=0, description="The duration must be greater than zero"
@@ -77,14 +81,15 @@
 
 
 class RunBase(BaseModel):
     timestamp: datetime
     experiment_id: UUID
     os: Optional[str]
     python_version: Optional[str]
+    codecarbon_version: Optional[str]
     cpu_count: Optional[int]
     cpu_model: Optional[str]
     gpu_count: Optional[int]
     gpu_model: Optional[str]
     longitude: Optional[float]
     latitude: Optional[float]
     region: Optional[str]
@@ -95,14 +100,15 @@
     class Config:
         schema_extra = {
             "example": {
                 "timestamp": "2021-04-04T08:43:00+02:00",
                 "experiment_id": "8edb03e1-9a28-452a-9c93-a3b6560136d7",
                 "os": "macOS-10.15.7-x86_64-i386-64bit",
                 "python_version": "3.8.0",
+                "codecarbon_version": "2.1.3",
                 "cpu_count": 12,
                 "cpu_model": "Intel(R) Core(TM) i7-8850H CPU @ 2.60GHz",
                 "gpu_count": 4,
                 "gpu_model": "NVIDIA",
                 "longitude": -7.6174,
                 "latitude": 33.5822,
                 "region": "EUROPE",
@@ -118,16 +124,18 @@
 
 
 class Run(RunBase):
     id: UUID
 
 
 class RunReport(RunBase):
+    run_id: UUID
     timestamp: datetime
-    emission: float
+    experiment_id: Optional[UUID]
+    emissions: float
     cpu_power: float
     gpu_power: float
     ram_power: float
     cpu_energy: float
     gpu_energy: float
     ram_energy: float
     energy_consumed: float
@@ -179,30 +187,29 @@
     timestamp: datetime
     name: str
     description: str
     country_name: str
     country_iso_code: str
     region: str
     on_cloud: str
-    cloud_provider: str
-    cloud_region: str
-    emission: float
+    cloud_provider: Optional[str] = None
+    cloud_region: Optional[str] = None
+    emissions: float
     cpu_power: float
     gpu_power: float
     ram_power: float
     cpu_energy: float
     gpu_energy: float
     ram_energy: float
     energy_consumed: float
     duration: int
     emissions_rate: float
     emissions_count: int
 
     class Config:
-
         schema_extra = {
             "experiment_id": "943b2aa5-9e21-41a9-8a38-562505b4b2aa",
             "timestamp": "2021-10-07T20:19:27.716693",
             "name": "Code Carbon user test",
             "description": "Code Carbon user test with default project",
             "country_name": "France",
             "country_iso_code": "FRA",
@@ -244,19 +251,19 @@
 
 
 class Project(ProjectBase):
     id: UUID
     experiments: Optional[List[Experiment]] = []
 
 
-class ProjectReport(ExperimentBase):
+class ProjectReport(ProjectBase):
     project_id: UUID
     name: str
     description: str
-    emission: float
+    emissions: float
     cpu_power: float
     gpu_power: float
     ram_power: float
     cpu_energy: float
     gpu_energy: float
     ram_energy: float
     energy_consumed: float
@@ -315,15 +322,15 @@
     teams: Optional[List[Team]]
 
 
 class OrganizationReport(OrganizationBase):
     organization_id: UUID
     name: str
     description: str
-    emission: float
+    emissions: float
     cpu_power: float
     gpu_power: float
     ram_power: float
     cpu_energy: float
     gpu_energy: float
     ram_energy: float
     energy_consumed: float
```

### Comparing `codecarbon-2.1.4/carbonserver/carbonserver/database/database.py` & `codecarbon-2.2.0/carbonserver/carbonserver/database/database.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/carbonserver/container.py` & `codecarbon-2.2.0/carbonserver/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from carbonserver.api.usecases.run.experiment_sum_by_run import (
     ExperimentSumsByRunUsecase,
 )
 from carbonserver.config import settings
 
 
 class ServerContainer(containers.DeclarativeContainer):
-
     config = providers.Configuration()
     db_url = settings.db_url
     db = providers.Singleton(
         Database,
         db_url=db_url,
     )
     emission_repository = providers.Factory(
```

### Comparing `codecarbon-2.1.4/carbonserver/main.py` & `codecarbon-2.2.0/carbonserver/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,35 +15,37 @@
     organizations,
     projects,
     runs,
     teams,
     users,
 )
 from carbonserver.database.database import engine
+from carbonserver.logger import logger
 
 
 async def db_exception_handler(request: Request, exc: DBException):
     return JSONResponse({"detail": exc.error.message}, status_code=400)
 
 
 async def generic_exception_handler(request: Request, exc: Exception):
     return JSONResponse({"detail": "Generic error"}, status_code=500)
 
 
 async def validation_exception_handler(request: Request, exc: ValidationError):
+    logger.error(f"ValidationError {exc}")
     return JSONResponse(
         {
-            "detail": "Validation error : a data is missing or in wrong format. Could be an error in our answer, not only in your request"
+            "detail": "Validation error : a data is missing or in wrong format. Could be an error in our answer, not only in your request",
+            "validation_error_message": str(exc),
         },
         status_code=400,
     )
 
 
 def create_app() -> FastAPI:
-
     container = init_container()
 
     init_db(container)
     server = init_server(container)
     server.add_exception_handler(DBException, db_exception_handler)
     server.add_exception_handler(ValidationError, validation_exception_handler)
     server.add_exception_handler(Exception, generic_exception_handler)
```

### Comparing `codecarbon-2.1.4/carbonserver/setup.py` & `codecarbon-2.2.0/carbonserver/setup.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/cli/cli_utils.py` & `codecarbon-2.2.0/codecarbon/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/cli/main.py` & `codecarbon-2.2.0/codecarbon/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import time
 
 import click
 
 from codecarbon import EmissionsTracker
 from codecarbon.cli.cli_utils import (
     get_api_endpoint,
@@ -72,15 +73,15 @@
 @click.option(
     "--api/--no-api", default=True, help="Choose to call Code Carbon API or not. (yes)"
 )
 def monitor(measure_power_secs, api_call_interval, api):
     experiment_id = get_existing_local_exp_id()
     if api and experiment_id is None:
         click.echo("ERROR: No experiment id, call 'codecarbon init' first.")
-        exit(1)
+        sys.exit(1)
     click.echo("CodeCarbon is going in an infinite loop to monitor this machine.")
     with EmissionsTracker(
         measure_power_secs=measure_power_secs,
         api_call_interval=api_call_interval,
         save_to_api=api,
     ):
         # Infinite loop
```

### Comparing `codecarbon-2.1.4/codecarbon/core/api_client.py` & `codecarbon-2.2.0/codecarbon/core/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             return None
         try:
             run = RunCreate(
                 timestamp=get_datetime_with_timezone(),
                 experiment_id=experiment_id,
                 os=self.conf.get("os"),
                 python_version=self.conf.get("python_version"),
+                codecarbon_version=self.conf.get("codecarbon_version"),
                 cpu_count=self.conf.get("cpu_count"),
                 cpu_model=self.conf.get("cpu_model"),
                 gpu_count=self.conf.get("gpu_count"),
                 gpu_model=self.conf.get("gpu_model"),
                 # Reduce precision for Privacy
                 longitude=round(self.conf.get("longitude"), 1),
                 latitude=round(self.conf.get("latitude"), 1),
@@ -135,14 +136,19 @@
             self.run_id = r.json()["id"]
             logger.info(
                 "ApiClient Successfully registered your run on the API.\n\n"
                 + f"Run ID: {self.run_id}\n"
                 + f"Experiment ID: {self.experiment_id}\n"
             )
             return self.run_id
+        except requests.exceptions.ConnectionError as e:
+            logger.error(
+                f"Failed to connect to API, please check the configuration. {e}",
+                exc_info=False,
+            )
         except Exception as e:
             logger.error(e, exc_info=True)
 
     def add_experiment(self, experiment: ExperimentCreate):
         """
         Create an experiment, used by the CLI, not the package.
         ::experiment:: The experiment to create.
```

### Comparing `codecarbon-2.1.4/codecarbon/core/cloud.py` & `codecarbon-2.2.0/codecarbon/core/cloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from typing import Any, Dict, Optional
 
 import requests
 
 from codecarbon.external.logger import logger
 
 
-def postprocess_gcp_cloud_metadata(cloud_metadata):
+def postprocess_gcp_cloud_metadata(cloud_metadata: Dict[str, Any]) -> Dict[str, Any]:
     # type: (Dict[str, Any]) -> Dict[str, Any]
 
     # Attributes contains custom metadata and also contains Kubernetes config,
     # startup script and secrets, filter it out
     if "attributes" in cloud_metadata:
         del cloud_metadata["attributes"]
 
@@ -50,15 +50,15 @@
         "url": "http://169.254.169.254/computeMetadata/v1/instance/?recursive=true&alt=json",  # noqa: E501
         "headers": {"Metadata-Flavor": "Google"},
         "postprocess_function": postprocess_gcp_cloud_metadata,
     },
 }
 
 
-def get_env_cloud_details(timeout=1):
+def get_env_cloud_details(timeout: int = 1) -> Optional[Any]:
     # type: (int) -> Optional[Any]
     """
     >>> get_env_cloud_details()
     {'provider': 'AWS',
      'metadata': {'accountId': '26550917306',
         'architecture': 'x86_64',
         'availabilityZone': 'us-east-1b',
@@ -85,13 +85,11 @@
             response_data = response.json()
 
             postprocess_function = params.get("postprocess_function")
             if postprocess_function is not None:
                 response_data = postprocess_function(response_data)
 
             return {"provider": provider, "metadata": response_data}
-        except Exception as e:
-            logger.debug(
-                "Not running on %s, couldn't retrieve metadata: %r", provider, e
-            )
+        except requests.exceptions.RequestException:
+            logger.debug("Not running on %s", provider)
 
     return None
```

### Comparing `codecarbon-2.1.4/codecarbon/core/co2_signal.py` & `codecarbon-2.2.0/codecarbon/core/co2_signal.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/core/config.py` & `codecarbon-2.2.0/codecarbon/core/config.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/core/cpu.py` & `codecarbon-2.2.0/codecarbon/core/cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
                     with open(rapl_file, "r") as f:
                         _ = float(f.read())
                     self._rapl_files.append(
                         RAPLFile(name=name, path=rapl_file, max_path=rapl_file_max)
                     )
                     logger.debug(f"We will read Intel RAPL files at {rapl_file}")
                 except PermissionError as e:
-                    logger.error(
+                    raise PermissionError(
                         "Unable to read Intel RAPL files for CPU power, we will use a constant for your CPU power."
                         + " Please view https://github.com/mlco2/codecarbon/issues/244"
                         + f" for workarounds : {e}"
                     )
         return
 
     def get_cpu_details(self, duration: Time, **kwargs) -> Dict:
@@ -272,16 +272,15 @@
 
     def _get_cpu_power_from_registry(self, cpu_model_raw: str) -> int:
         cpu_power_df = DataSource().get_cpu_power_data()
         cpu_matching = self._get_matching_cpu(cpu_model_raw, cpu_power_df)
         if cpu_matching:
             power = self._get_cpu_constant_power(cpu_matching, cpu_power_df)
             return power
-        else:
-            return None
+        return None
 
     @staticmethod
     def _get_cpus(cpu_df, cpu_idxs) -> list:
         return [cpu_df["Name"][idx] for idx in cpu_idxs]
 
     @staticmethod
     def _get_direct_matches(moodel: str, cpu_df: pd.DataFrame) -> list:
@@ -344,23 +343,21 @@
                 ratios_direct, max_ratio_direct, cpu_df
             )
             return cpu_matched
 
         # Check if an indirect match exists
         if max_ratio_token_set < THRESHOLD_TOKEN_SET:
             return None
-        else:
-            cpu_idxs = self._get_max_idxs(ratios_token_set, max_ratio_token_set)
-            cpu_machings = self._get_cpus(cpu_df, cpu_idxs)
-
-            if (cpu_machings and len(cpu_machings) == 1) or greedy:
-                cpu_matched = cpu_machings[0]
-                return cpu_matched
-            else:
-                return None
+        cpu_idxs = self._get_max_idxs(ratios_token_set, max_ratio_token_set)
+        cpu_machings = self._get_cpus(cpu_df, cpu_idxs)
+
+        if (cpu_machings and len(cpu_machings) == 1) or greedy:
+            cpu_matched = cpu_machings[0]
+            return cpu_matched
+        return None
 
     @staticmethod
     def _get_max_idxs(ratios: list, max_ratio: int) -> list:
         return [idx for idx, ratio in enumerate(ratios) if ratio == max_ratio]
 
     def _main(self) -> Tuple[str, int]:
         """
@@ -374,22 +371,20 @@
             power = self._get_cpu_power_from_registry(cpu_model_detected)
 
             if power:
                 logger.debug(
                     f"CPU : We detect a {cpu_model_detected} with a TDP of {power} W"
                 )
                 return cpu_model_detected, power
-            else:
-                logger.warning(
-                    f"We saw that you have a {cpu_model_detected} but we don't know it."
-                    + " Please contact us."
-                )
-                return cpu_model_detected, None
-        else:
             logger.warning(
-                "We were unable to detect your CPU using the `cpuinfo` package."
-                + " Resorting to a default power consumption of 85W."
+                f"We saw that you have a {cpu_model_detected} but we don't know it."
+                + " Please contact us."
             )
+            return cpu_model_detected, None
+        logger.warning(
+            "We were unable to detect your CPU using the `cpuinfo` package."
+            + " Resorting to a default power consumption of 85W."
+        )
         return "Unknown", None
 
     def start(self):
         pass
```

### Comparing `codecarbon-2.1.4/codecarbon/core/emissions.py` & `codecarbon-2.2.0/codecarbon/core/emissions.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/core/gpu.py` & `codecarbon-2.2.0/codecarbon/core/gpu.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/core/rapl.py` & `codecarbon-2.2.0/codecarbon/core/rapl.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/core/schemas.py` & `codecarbon-2.2.0/codecarbon/core/schemas.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 @dataclass
 class RunBase:
     timestamp: str
     experiment_id: str
     os: Optional[str]
     python_version: Optional[str]
+    codecarbon_version: Optional[str]
     cpu_count: Optional[int]
     cpu_model: Optional[str]
     gpu_count: Optional[int]
     gpu_model: Optional[str]
     longitude: Optional[float]
     latitude: Optional[float]
     region: Optional[str]
```

### Comparing `codecarbon-2.1.4/codecarbon/core/units.py` & `codecarbon-2.2.0/codecarbon/core/units.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/core/util.py` & `codecarbon-2.2.0/codecarbon/core/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
             exceptions if len(exceptions) != 1 else exceptions[0], exc_info=True
         )
         logger.warning("stopping.")
         pass
 
 
 def resolve_path(path: Union[str, Path]) -> Path:
-
     """
     Fully resolve a path:
     resolve env vars ($HOME etc.) -> expand user (~) -> make absolute
 
     Args:
         path (Union[str, Path]): Path to a file or repository to resolve as
             string or pathlib.Path
@@ -68,16 +67,15 @@
 
 
 def detect_cpu_model() -> str:
     cpu_info = cpuinfo.get_cpu_info()
     if cpu_info:
         cpu_model_detected = cpu_info.get("brand_raw", "")
         return cpu_model_detected
-    else:
-        return None
+    return None
 
 
 def count_cpus() -> int:
     if os.environ.get("SLURM_JOB_ID") is None:
         return psutil.cpu_count()
 
     try:
```

### Comparing `codecarbon-2.1.4/codecarbon/data/cloud/impact.csv` & `codecarbon-2.2.0/codecarbon/data/cloud/impact.csv`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/data/hardware/cpu_power.csv` & `codecarbon-2.2.0/codecarbon/data/hardware/cpu_power.csv`

 * *Files 1% similar despite different names*

```diff
@@ -838,14 +838,19 @@
 AMD Ryzen Threadripper 3970X,280
 AMD Ryzen Threadripper 3980X,280
 AMD Ryzen Threadripper 3990X,280
 AMD Ryzen Threadripper PRO 3945WX,280
 AMD Ryzen Threadripper PRO 3955WX,280
 AMD Ryzen Threadripper PRO 3975WX,280
 AMD Ryzen Threadripper PRO 3995WX,280
+AMD Ryzen Threadripper PRO 5945WX,280
+AMD Ryzen Threadripper PRO 5955WX,280
+AMD Ryzen Threadripper PRO 5965WX,280
+AMD Ryzen Threadripper PRO 5975WX,280
+AMD Ryzen Threadripper PRO 5995WX,280
 AMD Sempron 130,45
 AMD Sempron 140,45
 AMD Sempron 145,45
 AMD Sempron 150,45
 AMD Sempron 180,45
 AMD Sempron 2200+,62
 AMD Sempron 2200+,62
@@ -2043,14 +2048,16 @@
 Intel Xeon E7-8870 v3,140
 Intel Xeon E7-8880 v3,150
 Intel Xeon E7-8880L v3,115
 Intel Xeon E7-8890 v3,165
 Intel Xeon E7-8891 v3,165
 Intel Xeon E7-8893 v3,140
 Intel Xeon Gold 6154,200
+Intel Xeon Gold 6144,150
+Intel Xeon Gold 6230N,125
 Intel Xeon L5506,60
 Intel Xeon L5508,38
 Intel Xeon L5518,60
 Intel Xeon L5520,60
 Intel Xeon L5530,60
 Intel Xeon L5609,40
 Intel Xeon L5618,40
@@ -2095,14 +2102,15 @@
 Intel Xeon Phi 7250F,230
 Intel Xeon Phi 7285,250
 Intel Xeon Phi 7290,245
 Intel Xeon Phi 7290F,260
 Intel Xeon Phi 7295,320
 Intel Xeon Phi SE10P,300
 Intel Xeon Phi SE10X,300
+Intel Xeon Platinum 8171M,165
 Intel Xeon Platinum 8180,205
 Intel Xeon Platinum 8180M,205
 Intel Xeon Platinum 8253,125
 Intel Xeon Platinum 8256,105
 Intel Xeon Platinum 8259CL,210
 Intel Xeon Platinum 8260,165
 Intel Xeon Platinum 8260M,165
```

### Comparing `codecarbon-2.1.4/codecarbon/data/private_infra/2016/canada_energy_mix.json` & `codecarbon-2.2.0/codecarbon/data/private_infra/2016/canada_energy_mix.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/data/private_infra/2016/usa_emissions.json` & `codecarbon-2.2.0/codecarbon/data/private_infra/2016/usa_emissions.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/data/private_infra/carbon_intensity_per_source.json` & `codecarbon-2.2.0/codecarbon/data/private_infra/carbon_intensity_per_source.json`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/data/private_infra/global_energy_mix.json` & `codecarbon-2.2.0/codecarbon/data/private_infra/global_energy_mix.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -5076,7 +5076,8 @@
 00013d30: 736f 6c61 725f 5457 6822 3a20 302e 3031  solar_TWh": 0.01
 00013d40: 342c 0a20 2020 2020 2020 2022 746f 7461  4,.        "tota
 00013d50: 6c5f 5457 6822 3a20 382e 3934 3630 3139  l_TWh": 8.946019
 00013d60: 3939 3939 3939 3939 392c 0a20 2020 2020  999999999,.     
 00013d70: 2020 2022 7769 6e64 5f54 5768 223a 2030     "wind_TWh": 0
 00013d80: 2e30 2c0a 2020 2020 2020 2020 2279 6561  .0,.        "yea
 00013d90: 7222 3a20 3230 3138 0a20 2020 207d 0a7d  r": 2018.    }.}
+00013da0: 0a                                       .
```

### Comparing `codecarbon-2.1.4/codecarbon/emissions_tracker.py` & `codecarbon-2.2.0/codecarbon/emissions_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import uuid
 from abc import ABC, abstractmethod
 from collections import Counter
 from datetime import datetime
 from functools import wraps
 from typing import Callable, List, Optional, Union
 
+from codecarbon._version import __version__
 from codecarbon.core import cpu, gpu
 from codecarbon.core.config import get_hierarchical_config, parse_gpu_ids
 from codecarbon.core.emissions import Emissions
 from codecarbon.core.units import Energy, Power, Time
 from codecarbon.core.util import count_cpus, suppress
 from codecarbon.external.geography import CloudMetadata, GeoMetadata
 from codecarbon.external.hardware import CPU, GPU, RAM
@@ -51,15 +52,15 @@
 _sentinel = object()
 
 
 class BaseEmissionsTracker(ABC):
     """
     Primary abstraction with Emissions Tracking functionality.
     Has two abstract methods, `_get_geo_metadata` and `_get_cloud_metadata`
-    that are implemented by two concrete classes `OfflineCarbonTracker`
+    that are implemented by two concrete classes: `OfflineCarbonTracker`
     and `CarbonTracker.`
     """
 
     def _set_from_conf(
         self, var, name, default=None, return_type=None, prevent_setter=False
     ):
         """
@@ -98,24 +99,23 @@
         """
         # Check the hierarchical configuration has been read parsed and set.
         assert hasattr(self, "_external_conf")
         assert isinstance(self._external_conf, dict)
 
         # Store final values in _conf
         if not hasattr(self, "_conf"):
-            self._conf = {}
+            self._conf = {"codecarbon_version": __version__}
 
         value = _sentinel
 
         # a value for the keyword argument `name` is provided in the constructor:
         # use it
         if var is not _sentinel:
             value = var
         else:
-
             # no value provided in the constructor for `name`: check in the conf
             # (using the provided default value)
             value = self._external_conf.get(name, default)
 
             # parse to `return_type` if needed
             if return_type is not None:
                 if return_type is bool:
@@ -149,57 +149,59 @@
         emissions_endpoint: Optional[str] = _sentinel,
         experiment_id: Optional[str] = _sentinel,
         co2_signal_api_token: Optional[str] = _sentinel,
         tracking_mode: Optional[str] = _sentinel,
         log_level: Optional[Union[int, str]] = _sentinel,
         on_csv_write: Optional[str] = _sentinel,
         logger_preamble: Optional[str] = _sentinel,
+        default_cpu_power: Optional[int] = _sentinel,
     ):
         """
         :param project_name: Project name for current experiment run, default name
-                             as "codecarbon"
+                             is "codecarbon".
         :param measure_power_secs: Interval (in seconds) to measure hardware power
-                                   usage, defaults to 15
+                                   usage, defaults to 15.
         :param api_call_interval: Occurrence to wait before calling API :
                             -1 : only call api on flush() and at the end.
                             1 : at every measure
                             2 : every 2 measure, etc...
         :param api_endpoint: Optional URL of Code Carbon API endpoint for sending
-                             emissions data
-        :param api_key: API key for Code Carbon API, mandatory to use it !
+                             emissions data.
+        :param api_key: API key for Code Carbon API (mandatory!).
         :param output_dir: Directory path to which the experiment details are logged,
-                           defaults to current directory
-        :param output_file: Name of output CSV file, defaults to `emissions.csv`
+                           defaults to current directory.
+        :param output_file: Name of the output CSV file, defaults to `emissions.csv`.
         :param save_to_file: Indicates if the emission artifacts should be logged to a
-                             file, defaults to True
-        :param save_to_api: Indicates if the emission artifacts should be send to the
-                            CodeCarbon API, defaults to False
+                             file, defaults to True.
+        :param save_to_api: Indicates if the emission artifacts should be sent to the
+                            CodeCarbon API, defaults to False.
         :param save_to_logger: Indicates if the emission artifacts should be written
-                            to a dedicated logger, defaults to False
+                            to a dedicated logger, defaults to False.
         :param logging_logger: LoggerOutput object encapsulating a logging.logger
-                            or a Google Cloud logger
-        :param gpu_ids: User-specified known gpu ids to track, defaults to None
+                            or a Google Cloud logger.
+        :param gpu_ids: User-specified known gpu ids to track, defaults to None.
         :param emissions_endpoint: Optional URL of http endpoint for sending emissions
-                                   data
-        :param experiment_id: Id of the experiment
+                                   data.
+        :param experiment_id: Id of the experiment.
         :param co2_signal_api_token: API token for co2signal.com (requires sign-up for
                                      free beta)
         :param tracking_mode: One of "process" or "machine" in order to measure the
-                              power consumptions due to the entire machine or try and
+                              power consumption due to the entire machine or to try and
                               isolate the tracked processe's in isolation.
-                              Defaults to "machine"
+                              Defaults to "machine".
         :param log_level: Global codecarbon log level. Accepts one of:
                             {"debug", "info", "warning", "error", "critical"}.
                           Defaults to "info".
         :param on_csv_write: "append" or "update". Whether to always append a new line
                              to the csv when writing or to update the existing `run_id`
                              row (useful when calling`tracker.flush()` manually).
-                             Accepts one of "append" or "update".
-        :param logger_preamble: String to systematically include in the logger's.
+                             Accepts one of "append" or "update". Default is "append".
+        :param logger_preamble: String to systematically include in the logger.
                                 messages. Defaults to "".
+        :param default_cpu_power: cpu power to be used as default if the cpu is not known
         """
 
         # logger.info("base tracker init")
         self._external_conf = get_hierarchical_config()
 
         self._set_from_conf(api_call_interval, "api_call_interval", 8, int)
         self._set_from_conf(api_endpoint, "api_endpoint", "https://api.codecarbon.io")
@@ -214,14 +216,15 @@
         self._set_from_conf(save_to_api, "save_to_api", False, bool)
         self._set_from_conf(save_to_file, "save_to_file", True, bool)
         self._set_from_conf(save_to_logger, "save_to_logger", False, bool)
         self._set_from_conf(logging_logger, "logging_logger")
         self._set_from_conf(tracking_mode, "tracking_mode", "machine")
         self._set_from_conf(on_csv_write, "on_csv_write", "append")
         self._set_from_conf(logger_preamble, "logger_preamble", "")
+        self._set_from_conf(default_cpu_power, "default_cpu_power")
 
         assert self._tracking_mode in ["machine", "process"]
         set_logger_level(self._log_level)
         set_logger_format(self._logger_preamble)
 
         self._start_time: Optional[float] = None
         self._last_measured_time: float = time.time()
@@ -279,14 +282,19 @@
         else:
             logger.warning(
                 "No CPU tracking mode found. Falling back on CPU constant mode."
             )
             tdp = cpu.TDP()
             power = tdp.tdp
             model = tdp.model
+            if (power is None) and self._default_cpu_power:
+                # We haven't been able to calculate CPU power but user has input a default one. We use it
+                user_input_power = self._default_cpu_power
+                logger.debug(f"Using user input TDP: {user_input_power} W")
+                power = user_input_power
             logger.info(f"CPU Model on constant consumption mode: {model}")
             self._conf["cpu_model"] = model
             if tdp:
                 hardware = CPU.from_utils(self._output_dir, "constant", model, power)
                 self._hardware.append(hardware)
             else:
                 logger.warning(
@@ -297,14 +305,15 @@
                 self._hardware.append(hardware)
 
         self._conf["hardware"] = list(map(lambda x: x.description(), self._hardware))
 
         logger.info(">>> Tracker's metadata:")
         logger.info(f"  Platform system: {self._conf.get('os')}")
         logger.info(f"  Python version: {self._conf.get('python_version')}")
+        logger.info(f"  CodeCarbon version: {self._conf.get('codecarbon_version')}")
         logger.info(f"  Available RAM : {self._conf.get('ram_total_size'):.3f} GB")
         logger.info(f"  CPU count: {self._conf.get('cpu_count')}")
         logger.info(f"  CPU model: {self._conf.get('cpu_model')}")
         logger.info(f"  GPU count: {self._conf.get('gpu_count')}")
         logger.info(f"  GPU model: {self._conf.get('gpu_model')}")
 
         # Run `self._measure_power` every `measure_power_secs` seconds in a
@@ -380,20 +389,20 @@
             hardware.start()
 
         self._scheduler.start()
 
     @suppress(Exception)
     def flush(self) -> Optional[float]:
         """
-        Write emission to disk or call the API depending on the configuration
+        Write the emissions to disk or call the API depending on the configuration,
         but keep running the experiment.
         :return: CO2 emissions in kgs
         """
         if self._start_time is None:
-            logger.error("Need to first start the tracker")
+            logger.error("You first need to start the tracker.")
             return None
 
         # Run to calculate the power used from last
         # scheduled measurement to shutdown
         self._measure_power_and_energy()
 
         emissions_data = self._prepare_emissions_data()
@@ -407,23 +416,25 @@
     @suppress(Exception)
     def stop(self) -> Optional[float]:
         """
         Stops tracking the experiment
         :return: CO2 emissions in kgs
         """
         if self._start_time is None:
-            logger.error("Need to first start the tracker")
+            logger.error("You first need to start the tracker.")
             return None
 
         if self._scheduler:
             self._scheduler.stop()
-
-        # Run to calculate the power used from last
-        # scheduled measurement to shutdown
-        self._measure_power_and_energy()
+            self._scheduler = None
+            # Run to calculate the power used from last
+            # scheduled measurement to shutdown
+            self._measure_power_and_energy()
+        else:
+            logger.warning("Tracker already stopped !")
 
         emissions_data = self._prepare_emissions_data()
 
         for persistence in self.persistence_objs:
             if isinstance(persistence, CodeCarbonAPIOutput):
                 emissions_data = self._prepare_emissions_data(delta=True)
 
@@ -431,15 +442,15 @@
 
         self.final_emissions_data = emissions_data
         self.final_emissions = emissions_data.emissions
         return emissions_data.emissions
 
     def _prepare_emissions_data(self, delta=False) -> EmissionsData:
         """
-        :delta: True to return only the delta comsumption since last call
+        :delta: If 'True', return only the delta comsumption since the last call.
         """
         cloud: CloudMetadata = self._get_cloud_metadata()
         duration: Time = Time.from_seconds(time.time() - self._start_time)
 
         if cloud.is_on_private_infra:
             emissions = self._emissions.get_private_infra_emissions(
                 self._total_energy, self._geo
@@ -459,16 +470,16 @@
             cloud_provider = cloud.provider
             cloud_region = cloud.region
         total_emissions = EmissionsData(
             timestamp=datetime.now().strftime("%Y-%m-%dT%H:%M:%S"),
             project_name=self._project_name,
             run_id=str(self.run_id),
             duration=duration.seconds,
-            emissions=emissions,
-            emissions_rate=emissions * 1000 / duration.seconds,  # g/s
+            emissions=emissions,  # kg
+            emissions_rate=emissions / duration.seconds,  # kg/s
             cpu_power=self._cpu_power.W,
             gpu_power=self._gpu_power.W,
             ram_power=self._ram_power.W,
             cpu_energy=self._total_cpu_energy.kWh,
             gpu_energy=self._total_gpu_energy.kWh,
             ram_energy=self._total_ram_energy.kWh,
             energy_consumed=self._total_energy.kWh,
@@ -476,14 +487,15 @@
             country_iso_code=country_iso_code,
             region=region,
             on_cloud=on_cloud,
             cloud_provider=cloud_provider,
             cloud_region=cloud_region,
             os=self._conf.get("os"),
             python_version=self._conf.get("python_version"),
+            codecarbon_version=self._conf.get("codecarbon_version"),
             gpu_count=self._conf.get("gpu_count"),
             gpu_model=self._conf.get("gpu_model"),
             cpu_count=self._conf.get("cpu_count"),
             cpu_model=self._conf.get("cpu_model"),
             longitude=self._conf.get("longitude"),
             latitude=self._conf.get("latitude"),
             ram_total_size=self._conf.get("ram_total_size"),
@@ -543,22 +555,22 @@
             )
             self._total_energy += energy
             if isinstance(hardware, CPU):
                 self._total_cpu_energy += energy
                 self._cpu_power = power
                 logger.info(
                     f"Energy consumed for all CPUs : {self._total_cpu_energy.kWh:.6f} kWh"
-                    + f". All CPUs Power : {self._cpu_power.W} W"
+                    + f". Total CPU Power : {self._cpu_power.W} W"
                 )
             elif isinstance(hardware, GPU):
                 self._total_gpu_energy += energy
                 self._gpu_power = power
                 logger.info(
                     f"Energy consumed for all GPUs : {self._total_gpu_energy.kWh:.6f} kWh"
-                    + f". All GPUs Power : {self._gpu_power.W} W"
+                    + f". Total GPU Power : {self._gpu_power.W} W"
                 )
             elif isinstance(hardware, RAM):
                 self._total_ram_energy += energy
                 self._ram_power = power
                 logger.info(
                     f"Energy consumed for RAM : {self._total_ram_energy.kWh:.6f} kWh"
                     + f". RAM Power : {self._ram_power.W} W"
@@ -567,24 +579,24 @@
                 logger.error(f"Unknown hardware type: {hardware} ({type(hardware)})")
             h_time = time.time() - h_time
             logger.debug(
                 f"{hardware.__class__.__name__} : {hardware.total_power().W:,.2f} "
                 + f"W during {last_duration:,.2f} s [measurement time: {h_time:,.4f}]"
             )
         logger.info(
-            f"{self._total_energy.kWh:.6f} kWh of electricity used since the begining."
+            f"{self._total_energy.kWh:.6f} kWh of electricity used since the beginning."
         )
         self._last_measured_time = time.time()
         self._measure_occurrence += 1
         if self._cc_api__out is not None and self._api_call_interval != -1:
             if self._measure_occurrence >= self._api_call_interval:
                 emissions = self._prepare_emissions_data(delta=True)
                 logger.info(
-                    f"{emissions.emissions_rate:.6f} g.CO2eq/s mean an estimation of "
-                    + f"{emissions.emissions_rate*3600*24*365/1000:,} kg.CO2eq/year"
+                    f"{emissions.emissions_rate * 1000:.6f} g.CO2eq/s mean an estimation of "
+                    + f"{emissions.emissions_rate*3600*24*365:,} kg.CO2eq/year"
                 )
                 self._cc_api__out.out(emissions)
                 self._measure_occurrence = 0
         logger.debug(f"last_duration={last_duration}\n------------------------")
 
     def __enter__(self):
         self.start()
@@ -610,15 +622,15 @@
         cloud_region: Optional[str] = _sentinel,
         country_2letter_iso_code: Optional[str] = _sentinel,
         **kwargs,
     ):
         """
         :param country_iso_code: 3 letter ISO Code of the country where the
                                  experiment is being run
-        :param region: The provincial region, for example, California in the US.
+        :param region: The province or region (e.g. California in the US).
                        Currently, this only affects calculations for the United States
                        and Canada
         :param cloud_provider: The cloud provider specified for estimating emissions
                                intensity, defaults to None.
                                See https://github.com/mlco2/codecarbon/
                                         blob/master/codecarbon/data/cloud/impact.csv
                                for a list of cloud providers
@@ -698,15 +710,15 @@
             )
         return self._cloud
 
 
 class EmissionsTracker(BaseEmissionsTracker):
     """
     An online emissions tracker that auto infers geographical location,
-    using `geojs` API
+    using the `geojs` API
     """
 
     def _get_geo_metadata(self) -> GeoMetadata:
         return GeoMetadata.from_geo_js(self._data_source.geo_js_url)
 
     def _get_cloud_metadata(self) -> CloudMetadata:
         if self._cloud is None:
@@ -738,43 +750,43 @@
     co2_signal_api_token: Optional[str] = _sentinel,
     log_level: Optional[Union[int, str]] = _sentinel,
 ):
     """
     Decorator that supports both `EmissionsTracker` and `OfflineEmissionsTracker`
     :param fn: Function to be decorated
     :param project_name: Project name for current experiment run,
-                         default name as "codecarbon"
+                         default name is "codecarbon".
     :param measure_power_secs: Interval (in seconds) to measure hardware power usage,
-                               defaults to 15
+                               defaults to 15.
     :api_call_interval: Number of measure to make before calling the Code Carbon API.
     :param output_dir: Directory path to which the experiment details are logged,
-                       defaults to current directory
+                       defaults to current directory.
     :param output_file: Name of output CSV file, defaults to `emissions.csv`
     :param save_to_file: Indicates if the emission artifacts should be logged to a file,
-                         defaults to True
+                         defaults to True.
     :param save_to_api: Indicates if the emission artifacts should be send to the
-                        CodeCarbon API, defaults to False
+                        CodeCarbon API, defaults to False.
     :param save_to_logger: Indicates if the emission artifacts should be written
-                        to a dedicated logger, defaults to False
+                        to a dedicated logger, defaults to False.
     :param logging_logger: LoggerOutput object encapsulating a logging.logger
-                        or a Google Cloud logger
-    :param offline: Indicates if the tracker should be run in offline mode
+                        or a Google Cloud logger.
+    :param offline: Indicates if the tracker should be run in offline mode.
     :param country_iso_code: 3 letter ISO Code of the country where the experiment is
                              being run, required if `offline=True`
-    :param region: The provincial region, for example, California in the US.
-                   Currently, this only affects calculations for the United States
+    :param region: The provice or region (e.g. California in the US).
+                   Currently, this only affects calculations for the United States.
     :param cloud_provider: The cloud provider specified for estimating emissions
                            intensity, defaults to None.
                            See https://github.com/mlco2/codecarbon/
                                             blob/master/codecarbon/data/cloud/impact.csv
-                           for a list of cloud providers
+                           for a list of cloud providers.
     :param cloud_region: The region of the cloud data center, defaults to None.
                          See https://github.com/mlco2/codecarbon/
                                             blob/master/codecarbon/data/cloud/impact.csv
-                         for a list of cloud regions
+                         for a list of cloud regions.
     :param gpu_ids: User-specified known gpu ids to track, defaults to None
     :param log_level: Global codecarbon log level. Accepts one of:
                         {"debug", "info", "warning", "error", "critical"}.
                       Defaults to "info".
 
     :return: The decorated function
     """
@@ -825,15 +837,15 @@
                 )
             tracker.start()
             try:
                 fn_result = fn(*args, **kwargs)
             finally:
                 logger.info(
                     "\nGraceful stopping: collecting and writing information.\n"
-                    + "Please Allow for a few seconds..."
+                    + "Please wait a few seconds..."
                 )
                 tracker.stop()
                 logger.info("Done!\n")
             return fn_result
 
         return wrapped_fn
```

### Comparing `codecarbon-2.1.4/codecarbon/external/geography.py` & `codecarbon-2.2.0/codecarbon/external/geography.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from codecarbon.core.cloud import get_env_cloud_details
 from codecarbon.external.logger import logger
 
 
 @dataclass
 class CloudMetadata:
-
     provider: Optional[str]
     region: Optional[str]
 
     @property
     def is_on_private_infra(self) -> bool:
         return self.provider is None and self.region is None
 
@@ -77,21 +76,27 @@
             self.region,
         )
 
     @classmethod
     def from_geo_js(cls, url: str) -> "GeoMetadata":
         try:
             response: Dict = requests.get(url, timeout=0.5).json()
-        except requests.exceptions.Timeout:
+        except Exception as e:
             # If there is a timeout, we default to Canada
-            logger.info(
-                "Unable to access geographical location. \
-                Using 'Canada' as the default value"
+            logger.warning(
+                f"Unable to access geographical location. Using 'Canada' as the default value - Exception : {e}"
+            )
+            return cls(
+                country_iso_code="CAN",
+                country_name="Canada",
+                region="Quebec",
+                latitude=46.8,
+                longitude=-71.2,
+                country_2letter_iso_code="CA",
             )
-            return cls(country_iso_code="CAN", country_name="Canada")
         return cls(
             country_iso_code=response["country_code3"].upper(),
             country_name=response["country"],
             region=response.get("region", "").lower(),
             latitude=float(response.get("latitude")),
             longitude=float(response.get("longitude")),
             country_2letter_iso_code=response.get("country_code"),
```

### Comparing `codecarbon-2.1.4/codecarbon/external/hardware.py` & `codecarbon-2.2.0/codecarbon/external/hardware.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,34 +112,32 @@
         if self._mode == "intel_power_gadget":
             self._intel_interface = IntelPowerGadget(self._output_dir)
         elif self._mode == "intel_rapl":
             self._intel_interface = IntelRAPL(rapl_dir=rapl_dir)
 
     def __repr__(self) -> str:
         if self._mode != "constant":
-            return "CPU({})".format(
-                " ".join(map(str.capitalize, self._mode.split("_")))
-            )
+            return f"CPU({' '.join(map(str.capitalize, self._mode.split('_')))})"
 
-        s = "CPU({} > {}W".format(self._model, self._tdp)
+        s = f"CPU({self._model} > {self._tdp}W"
 
         if self._is_generic_tdp:
             s += " [generic]"
 
         return s + ")"
 
     def _get_power_from_cpus(self) -> Power:
         """
         Get CPU power
         :return: power in kW
         """
         if self._mode == "constant":
             power = self._tdp * CONSUMPTION_PERCENTAGE_CONSTANT
             return Power.from_watts(power)
-        elif self._mode == "intel_rapl":
+        if self._mode == "intel_rapl":
             # Don't call get_cpu_details to avoid computing energy twice and loosing data.
             all_cpu_details: Dict = self._intel_interface.get_static_cpu_details()
         else:
             all_cpu_details: Dict = self._intel_interface.get_cpu_details()
 
         power = 0
         for metric, value in all_cpu_details.items():
@@ -190,15 +188,14 @@
     def from_utils(
         cls,
         output_dir: str,
         mode: str,
         model: Optional[str] = None,
         tdp: Optional[int] = None,
     ) -> "CPU":
-
         if model is None:
             model = detect_cpu_model()
             if model is None:
                 logger.warning("Could not read CPU model.")
 
         if tdp is None:
             tdp = POWER_CONSTANT
@@ -207,15 +204,14 @@
             return cpu
 
         return cls(output_dir=output_dir, mode=mode, model=model, tdp=tdp)
 
 
 @dataclass
 class RAM(BaseHardware):
-
     # 3 watts of power for every 8GB of DDR3 or DDR4 memory
     # https://www.crucial.com/support/articles-faq-memory/how-much-power-does-memory-use
     power_per_GB = 3 / 8  # W/GB
 
     def __init__(
         self,
         pid: int = psutil.Process().pid,
```

### Comparing `codecarbon-2.1.4/codecarbon/external/logger.py` & `codecarbon-2.2.0/codecarbon/external/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     if logger.hasHandlers():
         logger.handlers.clear()
 
     logger.addHandler(handler)
 
 
 def set_logger_level(level: Optional[str] = None):
-
     if level is None:
         lower_envs = {k.lower(): v for k, v in os.environ.items()}
         level = lower_envs.get("codecarbon_log_level", "INFO")
 
     logger = logging.getLogger("codecarbon")
 
     if isinstance(level, int):
```

### Comparing `codecarbon-2.1.4/codecarbon/external/scheduler.py` & `codecarbon-2.2.0/codecarbon/external/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from threading import Lock, Timer
 
 
-class PeriodicScheduler(object):
+class PeriodicScheduler:
     """
     A periodic task running in threading.Timers
     From https://stackoverflow.com/a/18906292/14541668
     """
 
     def __init__(self, interval, function, *args, **kwargs):
         """
```

### Comparing `codecarbon-2.1.4/codecarbon/input.py` & `codecarbon-2.2.0/codecarbon/input.py`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/output.py` & `codecarbon-2.2.0/codecarbon/output.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     country_name: str
     country_iso_code: str
     region: str
     cloud_provider: str
     cloud_region: str
     os: str
     python_version: str
+    codecarbon_version: str
     cpu_count: float
     cpu_model: str
     gpu_count: float
     gpu_model: str
     longitude: float
     latitude: float
     ram_total_size: float
@@ -66,17 +67,17 @@
         self.duration = delta_duration
         delta_emissions = self.emissions - previous_emission.emissions
         self.emissions = delta_emissions
         self.cpu_energy -= previous_emission.cpu_energy
         self.gpu_energy -= previous_emission.gpu_energy
         self.ram_energy -= previous_emission.ram_energy
         self.energy_consumed -= previous_emission.energy_consumed
-        # delta_emissions in kg.CO2 => * 1000 to convert in g
         if delta_duration > 0:
-            self.emissions_rate = delta_emissions * 1000 / delta_duration
+            # emissions_rate in g/s : delta_emissions in kg.CO2 / delta_duration in s
+            self.emissions_rate = delta_emissions / delta_duration
         else:
             self.emissions_rate = 0
 
 
 class BaseOutput(ABC):
     """
     An abstract class that requires children to inherit a single method,
```

### Comparing `codecarbon-2.1.4/codecarbon/viz/assets/car_icon.png` & `codecarbon-2.2.0/codecarbon/viz/assets/car_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/viz/assets/house_icon.png` & `codecarbon-2.2.0/codecarbon/viz/assets/house_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/viz/assets/tv_icon.png` & `codecarbon-2.2.0/codecarbon/viz/assets/tv_icon.png`

 * *Files identical despite different names*

### Comparing `codecarbon-2.1.4/codecarbon/viz/carbonboard.py` & `codecarbon-2.2.0/codecarbon/viz/carbonboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,16 +168,15 @@
         [Input(component_id="hidden_project_summary", component_property="data")],
     )
     def update_show_regional_comparison(hidden_project_summary: dcc.Store):
         country_iso_code = hidden_project_summary["country_iso_code"]
         # add country codes here to render for different countries
         if country_iso_code.upper() in ["USA", "CAN"]:
             return {"display": "block"}
-        else:
-            return {"display": "none"}
+        return {"display": "none"}
 
     @app.callback(
         [
             Output(component_id="country_name", component_property="children"),
             Output(
                 component_id="regional_emissions_comparison_choropleth",
                 component_property="figure",
@@ -227,16 +226,15 @@
         ),
         [Input(component_id="hidden_project_summary", component_property="data")],
     )
     def update_on_cloud(hidden_project_summary: dcc.Store):
         on_cloud = hidden_project_summary["on_cloud"]
         if on_cloud == "Y":
             return {"display": "block"}
-        else:
-            return {"display": "none"}
+        return {"display": "none"}
 
     @app.callback(
         [
             Output(component_id="cloud_provider_name", component_property="children"),
             Output(
                 component_id="cloud_emissions_barchart", component_property="figure"
             ),
```

### Comparing `codecarbon-2.1.4/codecarbon/viz/carbonboard_on_api.py` & `codecarbon-2.2.0/codecarbon/viz/carbonboard_on_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,16 +169,15 @@
         [Input(component_id="hidden_project_summary", component_property="data")],
     )
     def update_show_regional_comparison(hidden_project_summary: dcc.Store):
         country_iso_code = hidden_project_summary["country_iso_code"]
         # add country codes here to render for different countries
         if country_iso_code.upper() in ["USA", "CAN"]:
             return {"display": "block"}
-        else:
-            return {"display": "none"}
+        return {"display": "none"}
 
     @app.callback(
         [
             Output(component_id="country_name", component_property="children"),
             Output(
                 component_id="regional_emissions_comparison_choropleth",
                 component_property="figure",
@@ -228,16 +227,15 @@
         ),
         [Input(component_id="hidden_project_summary", component_property="data")],
     )
     def update_on_cloud(hidden_project_summary: dcc.Store):
         on_cloud = hidden_project_summary["on_cloud"]
         if on_cloud == "Y":
             return {"display": "block"}
-        else:
-            return {"display": "none"}
+        return {"display": "none"}
 
     @app.callback(
         [
             Output(component_id="cloud_provider_name", component_property="children"),
             Output(
                 component_id="cloud_emissions_barchart", component_property="figure"
             ),
```

### Comparing `codecarbon-2.1.4/codecarbon/viz/components.py` & `codecarbon-2.2.0/codecarbon/viz/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,45 +360,44 @@
                     f"Already running on {cloud_provider_name}'s least emissions region ",
                     html.Strong(
                         f"{cloud_emissions_project_region.region}",
                         style={"fontWeight": "normal", "color": "green"},
                     ),
                 ]
             )
-        else:
-            return (
-                html.H4(
-                    [
-                        "Had this been run in ",
-                        html.Strong(
-                            f"{cloud_emissions_minimum_region.region}",
-                            style={"fontWeight": "normal", "color": "green"},
-                        ),
-                        " region, ",
-                    ]
-                ),
-                html.H4(
-                    [
-                        "then the emitted carbon would have been ",
-                        html.Strong(
-                            f"{'{:.1f}'.format(cloud_emissions_minimum_region.emissions)} kg",
-                            style={"fontWeight": "normal", "color": "green"},
-                        ),
-                    ]
-                ),
-                html.H4(
-                    [
-                        "Reducing the current  emissions by ",
-                        html.Strong(
-                            f"{'{:.1f}'.format(cloud_emissions_project_region.emissions - cloud_emissions_minimum_region.emissions)} kg",
-                            style={"fontWeight": "normal", "color": "green"},
-                        ),
-                    ]
-                ),
-            )
+        return (
+            html.H4(
+                [
+                    "Had this been run in ",
+                    html.Strong(
+                        f"{cloud_emissions_minimum_region.region}",
+                        style={"fontWeight": "normal", "color": "green"},
+                    ),
+                    " region, ",
+                ]
+            ),
+            html.H4(
+                [
+                    "then the emitted carbon would have been ",
+                    html.Strong(
+                        f"{'{:.1f}'.format(cloud_emissions_minimum_region.emissions)} kg",
+                        style={"fontWeight": "normal", "color": "green"},
+                    ),
+                ]
+            ),
+            html.H4(
+                [
+                    "Reducing the current  emissions by ",
+                    html.Strong(
+                        f"{'{:.1f}'.format(cloud_emissions_project_region.emissions - cloud_emissions_minimum_region.emissions)} kg",
+                        style={"fontWeight": "normal", "color": "green"},
+                    ),
+                ]
+            ),
+        )
 
     @staticmethod
     def get_emissions_tab():
         return dcc.Tab(
             label="Emissions Equivalent",
             value="emissions_tab",
             id="global_emissions",
```

### Comparing `codecarbon-2.1.4/codecarbon/viz/data.py` & `codecarbon-2.2.0/codecarbon/viz/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,52 +58,52 @@
         1 CO2, CH4, and N2O/0.988 CO2
         = 4.09 x 10-4 metric tons CO2E/mile
         = 0.409 kg CO2E/mile
         Source: EPA
         :param project_carbon_equivalent: total project emissions in kg CO2E
         :return: number of miles driven by avg car
         """
-        return "{:.0f}".format(project_carbon_equivalent / 0.409)
+        return f"{project_carbon_equivalent / 0.409:.0f}"
 
     def get_tv_time(self, project_carbon_equivalent: float):
         """
         Gives the amount of time
         a 32-inch LCD flat screen TV will emit
         an equivalent amount of carbon
         Ratio is 0.097 kg CO2 / 1 hour tv
         :param project_carbon_equivalent: total project emissions in kg CO2E
         :return: equivalent TV time
         """
         time_in_minutes = project_carbon_equivalent * (1 / 0.097) * 60
-        formated_value = "{:.0f} minutes".format(time_in_minutes)
+        formated_value = f"{time_in_minutes:.0f} minutes"
         if time_in_minutes >= 60:
             time_in_hours = time_in_minutes / 60
-            formated_value = "{:.0f} hours".format(time_in_hours)
+            formated_value = f"{time_in_hours:.0f} hours"
             if time_in_hours >= 24:
                 time_in_days = time_in_hours / 24
-                formated_value = "{:.0f} days".format(time_in_days)
+                formated_value = f"{time_in_days:.0f} days"
         return formated_value
 
     def get_household_fraction(self, project_carbon_equivalent: float):
         """
         Total CO2 emissions for energy use per home: 5.734 metric tons CO2 for electricity
         + 2.06 metric tons CO2 for natural gas + 0.26 metric tons CO2 for liquid petroleum gas
          + 0.30 metric tons CO2 for fuel oil  = 8.35 metric tons CO2 per home per year / 52 weeks
          = 160.58 kg CO2/week on average
         Source: EPA
         :param project_carbon_equivalent: total project emissions in kg CO2E
         :return: % of weekly emissions re: an average American household
         """
-        return "{:.2f}".format((project_carbon_equivalent / 160.58) * 100)
+        return f"{project_carbon_equivalent / 160.58 * 100:.2f}"
 
     def get_global_emissions_choropleth_data(
         self, net_energy_consumed: float
     ) -> List[Dict]:
         def formatted_energy_percentage(energy_type: float, total: float) -> float:
-            return float("{:.1f}".format((energy_type / total) * 100))
+            return float(f"{energy_type / total * 100:.1f}")
 
         global_energy_mix = self._data_source.get_global_energy_mix_data()
         choropleth_data = []
         for country_iso_code in global_energy_mix.keys():
             country_name = global_energy_mix[country_iso_code]["country_name"]
 
             if country_iso_code not in ["_define", "ATA"]:
@@ -147,34 +147,34 @@
                     }
                 )
         return choropleth_data
 
     def get_regional_emissions_choropleth_data(
         self, net_energy_consumed: float, country_iso_code: str
     ) -> List[Dict]:
-
         # add country codes here to render for different countries
         if country_iso_code.upper() not in ["USA", "CAN"]:
             return [{"region_code": "", "region_name": "", "emissions": ""}]
 
         try:
             region_emissions = self._data_source.get_country_emissions_data(
                 country_iso_code.lower()
             )
-        except DataSourceException:  # This country has regional data at the energy mix level, not the emissions level
+        except (
+            DataSourceException
+        ):  # This country has regional data at the energy mix level, not the emissions level
             country_energy_mix = self._data_source.get_country_energy_mix_data(
                 country_iso_code.lower()
             )
             region_emissions = {
                 region: {"regionCode": region}
                 for region, energy_mix in country_energy_mix.items()
             }
         choropleth_data = []
         for region_name in region_emissions.keys():
-
             region_code = region_emissions[region_name]["regionCode"]
             if region_name not in ["_unit"]:
                 from codecarbon.core.units import Energy
 
                 energy_consumed = Energy.from_energy(kWh=net_energy_consumed)
 
                 from codecarbon.external.geography import GeoMetadata
@@ -233,18 +233,15 @@
 
     @staticmethod
     def get_data_from_api(host):
         transformed_projects = []
         project_list = Data.list_projects(host)
         for project in project_list:
             project_sum_by_experiments_url = (
-                host
-                + "/experiments/{project_id}/detailed_sums".format(
-                    project_id=project["id"]
-                )
+                host + f"/experiments/{project['id']}/detailed_sums"
             )
             project_name = project["name"]
             sums = requests.get(project_sum_by_experiments_url).json()
             for experiment in sums:
                 experiment["project_name"] = project_name
                 # experiment["emission_rate"] = 0
                 # if experiment["emissions_count"] > 0:
@@ -257,15 +254,15 @@
 
     @staticmethod
     def list_projects(host):
         projects = []
         teams_url = host + "/teams"
         teams = requests.get(teams_url).json()
         for team in teams:
-            projets_url = host + "/projects/team/{team_id}".format(team_id=team["id"])
+            projets_url = host + f"/projects/team/{team['id']}"
             team_projects = requests.get(projets_url).json()
             if team_projects:
                 projects.append(
                     list(
                         map(
                             lambda x: {"id": x["id"], "name": x["name"]},
                             iter(team_projects),
```

### Comparing `codecarbon-2.1.4/setup.py` & `codecarbon-2.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,34 @@
 ]
 
 TEST_DEPENDENCIES = ["mock", "pytest", "responses", "tox", "numpy", "requests-mock"]
 
 
 setuptools.setup(
     name="codecarbon",
-    version="2.1.4",
+    version="2.2.0",
     author="Mila, DataForGood, BCG GAMMA, Comet.ml, Haverford College",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    license_files=("LICENSE",),
     packages=setuptools.find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests"]
     ),
     install_requires=DEPENDENCIES,
     tests_require=TEST_DEPENDENCIES,
-    extras_require={"viz": ["dash", "dash_bootstrap_components < 1.0.0", "fire"]},
+    extras_require={
+        "viz": ["dash", "dash_bootstrap_components < 1.0.0", "fire"],
+        "dashboard": ["dash>=2.2.0", "plotly>=5.6.0", "dash_bootstrap_components"],
+    },
     classifiers=[
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "License :: OSI Approved :: MIT License",
     ],
     package_data={
         "codecarbon": [
             "data/cloud/impact.csv",
             "data/hardware/cpu_power.csv",
             "data/private_infra/2016/usa_emissions.json",
             "data/private_infra/2016/canada_energy_mix.json",
```

