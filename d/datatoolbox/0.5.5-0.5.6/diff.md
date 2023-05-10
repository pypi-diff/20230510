# Comparing `tmp/datatoolbox-0.5.5.tar.gz` & `tmp/datatoolbox-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatoolbox-0.5.5.tar", last modified: Tue May  9 08:11:42 2023, max compression
+gzip compressed data, was "datatoolbox-0.5.6.tar", last modified: Wed May 10 09:20:56 2023, max compression
```

## Comparing `datatoolbox-0.5.5.tar` & `datatoolbox-0.5.6.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/
--rwxrwx---   0 root         (0) vboxsf     (999)      159 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/.gitignore
--rwxrwx---   0 root         (0) vboxsf     (999)      950 2022-10-19 13:17:33.000000 datatoolbox-0.5.5/.gitlab-ci.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      703 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/.travis.yml
--rwxrwx---   0 root         (0) vboxsf     (999)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/LICENSE
--rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)      771 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/README.md
--rwxrwx---   0 root         (0) vboxsf     (999)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/appveyor.yml
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/ci/
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/ci/appveyor/
--rwxrwx---   0 root         (0) vboxsf     (999)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/ci/appveyor/install.ps1
--rwxrwx---   0 root         (0) vboxsf     (999)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/ci/appveyor/run_with_env.cmd
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/
--rwxrwx---   0 root         (0) vboxsf     (999)     4362 2023-05-04 12:41:44.000000 datatoolbox-0.5.5/datatoolbox/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)    15385 2023-03-30 07:48:47.000000 datatoolbox-0.5.5/datatoolbox/admin.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6655 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/config.py
--rwxrwx---   0 root         (0) vboxsf     (999)    18640 2022-12-01 09:27:15.000000 datatoolbox-0.5.5/datatoolbox/converters.py
--rwxrwx---   0 root         (0) vboxsf     (999)    11733 2022-12-19 11:17:33.000000 datatoolbox-0.5.5/datatoolbox/core.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/data/
--rwxrwx---   0 root         (0) vboxsf     (999)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/data/GHG_alternative_naming.pkl
--rwxrwx---   0 root         (0) vboxsf     (999)    13482 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/data/GHG_properties_2019_CA.csv
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/
--rwxrwx---   0 root         (0) vboxsf     (999)      286 2023-05-04 13:24:49.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/inventory.csv
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/
--rwxrwx---   0 root         (0) vboxsf     (999)    10757 2023-05-04 13:24:48.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     8466 2023-05-04 13:24:48.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
--rwxrwx---   0 root         (0) vboxsf     (999)      999 2023-05-04 13:24:48.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
--rwxrwx---   0 root         (0) vboxsf     (999)      161 2023-05-04 13:24:49.000000 datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/sources.csv
--rwxrwx---   0 root         (0) vboxsf     (999)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/data/all.csv
--rwxrwx---   0 root         (0) vboxsf     (999)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/data/compatible1_5_unfiltered.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.5.5/datatoolbox/data/continent.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.5.5/datatoolbox/data/country_codes.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/datatoolbox/data/datashelf_contents.csv
--rwxrwx---   0 root         (0) vboxsf     (999)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.5.5/datatoolbox/data/external_mappings.py
--rwxrwx---   0 root         (0) vboxsf     (999)      178 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/data/personal_template.py
--rwxrwx---   0 root         (0) vboxsf     (999)      999 2019-08-14 10:00:22.000000 datatoolbox-0.5.5/datatoolbox/data/regions.csv
--rwxrwx---   0 root         (0) vboxsf     (999)   237054 2023-04-28 11:35:43.000000 datatoolbox-0.5.5/datatoolbox/data_readers.py
--rwxrwx---   0 root         (0) vboxsf     (999)    68067 2023-05-04 07:37:43.000000 datatoolbox-0.5.5/datatoolbox/data_structures.py
--rwxrwx---   0 root         (0) vboxsf     (999)    63785 2023-05-09 07:33:41.000000 datatoolbox-0.5.5/datatoolbox/database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/greenhouse_gas_database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/init_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)    21652 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/interfaces.py
--rwxrwx---   0 root         (0) vboxsf     (999)    10991 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/io_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/mapping.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.5.5/datatoolbox/naming_convention.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/patches.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2175 2022-11-16 12:15:23.000000 datatoolbox-0.5.5/datatoolbox/pint_definitions.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.5/datatoolbox/relations.py
--rwxrwx---   0 root         (0) vboxsf     (999)    26527 2023-04-05 07:52:48.000000 datatoolbox-0.5.5/datatoolbox/sets.py
--rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.5/datatoolbox/storage.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/templates.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/tools/
--rwxrwx---   0 root         (0) vboxsf     (999)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.5.5/datatoolbox/tools/CRF_extract_CA_2021.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.5.5/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.5.5/datatoolbox/tools/IEA_B2DS_4.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.5.5/datatoolbox/tools/WEO_2019_test.SCEN
--rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/__init__.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.5.5/datatoolbox/tools/conversion_to_v0.3.py
--rwxrwx---   0 root         (0) vboxsf     (999)    42729 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/excel.py
--rwxrwx---   0 root         (0) vboxsf     (999)      370 2022-11-17 09:58:39.000000 datatoolbox-0.5.5/datatoolbox/tools/export_all.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/for_datatables.py
--rwxrwx---   0 root         (0) vboxsf     (999)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/html.py
--rwxrwx---   0 root         (0) vboxsf     (999)      182 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/install_support.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/kaya_idendentiy_decomposition.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/magicc6.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/matplotlib.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/pandas.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/py_magicc_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7869 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/pyam.py
--rwxrwx---   0 root         (0) vboxsf     (999)      965 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/renaming_DB.py
--rwxrwx---   0 root         (0) vboxsf     (999)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.5.5/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
--rwxrwx---   0 root         (0) vboxsf     (999)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.5.5/datatoolbox/tools/run_magicc6.m
--rwxrwx---   0 root         (0) vboxsf     (999)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.5.5/datatoolbox/tools/statistics.py
--rwxrwx---   0 root         (0) vboxsf     (999)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.5.5/datatoolbox/tools/test.docx
--rwxrwx---   0 root         (0) vboxsf     (999)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/tools/word.py
--rwxrwx---   0 root         (0) vboxsf     (999)     9617 2023-03-30 13:29:22.000000 datatoolbox-0.5.5/datatoolbox/tools/xarray.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox/tutorials/
--rwxrwx---   0 root         (0) vboxsf     (999)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/datatoolbox/tutorials/00_search_find_and_access_data.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/tutorials/01_emission_comparison.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/datatoolbox/tutorials/02_unit_conversion.py
--rwxrwx---   0 root         (0) vboxsf     (999)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.5.5/datatoolbox/tutorials/03_intermediate_example.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/datatoolbox/tutorials/04_sources.py
--rwxrwx---   0 root         (0) vboxsf     (999)      382 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/datatoolbox/tutorials/05_plot_source_content.py
--rwxrwx---   0 root         (0) vboxsf     (999)      734 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/datatoolbox/tutorials/06_xarray_examples.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.5.5/datatoolbox/tutorials/07_renewable_share_compuation.py
--rwxrwx---   0 root         (0) vboxsf     (999)      793 2021-05-11 12:59:38.000000 datatoolbox-0.5.5/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
--rwxrwx---   0 root         (0) vboxsf     (999)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/datatoolbox/tutorials/introduction_v1.ipynb
--rwxrwx---   0 root         (0) vboxsf     (999)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.5.5/datatoolbox/tutorials/jump_start.py
--rwxrwx---   0 root         (0) vboxsf     (999)      300 2022-11-21 13:35:45.000000 datatoolbox-0.5.5/datatoolbox/units.py
--rwxrwx---   0 root         (0) vboxsf     (999)    43915 2022-11-22 09:50:19.000000 datatoolbox-0.5.5/datatoolbox/util.py
--rwxrwx---   0 root         (0) vboxsf     (999)      176 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox/version.py
--rwxrwx---   0 root         (0) vboxsf     (999)      746 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/datatoolbox/workflows.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)     3714 2023-05-09 08:11:41.000000 datatoolbox-0.5.5/datatoolbox.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        1 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (999)      149 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       12 2023-05-09 08:11:40.000000 datatoolbox-0.5.5/datatoolbox.egg-info/top_level.txt
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/doc/
--rwxrwx---   0 root         (0) vboxsf     (999)     7755 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/doc/Makefile
--rwxrwx---   0 root         (0) vboxsf     (999)     9684 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/conf.py
--rwxrwx---   0 root         (0) vboxsf     (999)       79 2021-01-05 10:54:01.000000 datatoolbox-0.5.5/doc/core.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      149 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/data_structures.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      122 2021-01-11 16:19:59.000000 datatoolbox-0.5.5/doc/database.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       91 2021-01-11 16:18:53.000000 datatoolbox-0.5.5/doc/database_database.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      130 2021-01-11 16:21:50.000000 datatoolbox-0.5.5/doc/database_gitrepomanager.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       93 2021-01-11 16:03:03.000000 datatoolbox-0.5.5/doc/excel.rst
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/doc/figures/
--rwxrwx---   0 root         (0) vboxsf     (999)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.5.5/doc/figures/ID_meta_data.svg
--rwxrwx---   0 root         (0) vboxsf     (999)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.5.5/doc/figures/config_input.png
--rwxrwx---   0 root         (0) vboxsf     (999)     7157 2021-05-17 15:04:37.000000 datatoolbox-0.5.5/doc/first_steps.md
--rwxrwx---   0 root         (0) vboxsf     (999)      100 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/foo.rst_template
--rwxrwx---   0 root         (0) vboxsf     (999)       77 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/help.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      463 2021-01-11 16:06:28.000000 datatoolbox-0.5.5/doc/index.rst
--rwxrwx---   0 root         (0) vboxsf     (999)     1754 2021-05-21 08:03:28.000000 datatoolbox-0.5.5/doc/installation.md
--rwxrwx---   0 root         (0) vboxsf     (999)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/doc/license.rst
--rwxrwx---   0 root         (0) vboxsf     (999)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/doc/make.bat
--rwxrwx---   0 root         (0) vboxsf     (999)      103 2021-01-11 16:09:22.000000 datatoolbox-0.5.5/doc/matplotlib.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:10:43.000000 datatoolbox-0.5.5/doc/pandas.rst
--rwxrwx---   0 root         (0) vboxsf     (999)      133 2021-01-11 16:20:57.000000 datatoolbox-0.5.5/doc/tools.rst
--rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:09:13.000000 datatoolbox-0.5.5/doc/xarray.rst
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/documentation/
--rwxrwx---   0 root         (0) vboxsf     (999)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.5.5/documentation/Datatoolbox - First steps.md
--rwxrwx---   0 root         (0) vboxsf     (999)      381 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/environment.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      418 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/make_proj.sh
--rwxrwx---   0 root         (0) vboxsf     (999)      558 2021-01-12 15:45:18.000000 datatoolbox-0.5.5/readthedocs.yml
--rwxrwx---   0 root         (0) vboxsf     (999)      215 2022-10-19 13:17:33.000000 datatoolbox-0.5.5/requirements.txt
--rwxrwx---   0 root         (0) vboxsf     (999)       38 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (999)     1839 2023-05-03 11:16:28.000000 datatoolbox-0.5.5/setup.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-09 08:11:42.000000 datatoolbox-0.5.5/tests/
--rwxrwx---   0 root         (0) vboxsf     (999)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.5.5/tests/test_calculations.py
--rwxrwx---   0 root         (0) vboxsf     (999)      696 2022-11-18 16:16:07.000000 datatoolbox-0.5.5/tests/test_converters.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2836 2022-11-21 11:08:31.000000 datatoolbox-0.5.5/tests/test_database.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.5.5/tests/test_dataset.py
--rwxrwx---   0 root         (0) vboxsf     (999)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/tests/test_datatable.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.5.5/tests/test_io.py
--rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-22 09:54:34.000000 datatoolbox-0.5.5/tests/test_linked_functions.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.5.5/tests/test_pyam.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/tests/test_tableset.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/tests/test_tools.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1227 2022-11-21 13:23:54.000000 datatoolbox-0.5.5/tests/test_units.py
--rwxrwx---   0 root         (0) vboxsf     (999)      870 2020-10-14 14:04:19.000000 datatoolbox-0.5.5/tests/test_utilities.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.5.5/tests/test_xarray.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.5.5/tests/util_for_testing.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/
+-rwxrwx---   0 root         (0) vboxsf     (999)      159 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/.gitignore
+-rwxrwx---   0 root         (0) vboxsf     (999)      950 2022-10-19 13:17:33.000000 datatoolbox-0.5.6/.gitlab-ci.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      703 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/.travis.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)     1073 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/LICENSE
+-rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)      771 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/README.md
+-rwxrwx---   0 root         (0) vboxsf     (999)     1225 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/appveyor.yml
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/ci/
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/ci/appveyor/
+-rwxrwx---   0 root         (0) vboxsf     (999)     3111 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/ci/appveyor/install.ps1
+-rwxrwx---   0 root         (0) vboxsf     (999)     1842 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/ci/appveyor/run_with_env.cmd
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/
+-rwxrwx---   0 root         (0) vboxsf     (999)     4362 2023-05-04 12:41:44.000000 datatoolbox-0.5.6/datatoolbox/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    15385 2023-03-30 07:48:47.000000 datatoolbox-0.5.6/datatoolbox/admin.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6655 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/config.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    18640 2022-12-01 09:27:15.000000 datatoolbox-0.5.6/datatoolbox/converters.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    11733 2022-12-19 11:17:33.000000 datatoolbox-0.5.6/datatoolbox/core.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/data/
+-rwxrwx---   0 root         (0) vboxsf     (999)    15781 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/data/GHG_alternative_naming.pkl
+-rwxrwx---   0 root         (0) vboxsf     (999)    13482 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/data/GHG_properties_2019_CA.csv
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/
+-rwxrwx---   0 root         (0) vboxsf     (999)      286 2023-05-09 08:12:07.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/inventory.csv
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/
+-rwxrwx---   0 root         (0) vboxsf     (999)    10757 2023-05-09 08:12:04.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     8466 2023-05-09 08:12:04.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)      999 2023-05-09 08:12:04.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)      161 2023-05-09 08:12:07.000000 datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/sources.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)    22865 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/data/all.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)    14615 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/data/compatible1_5_unfiltered.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)    10757 2020-04-20 12:32:09.000000 datatoolbox-0.5.6/datatoolbox/data/continent.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     8466 2021-09-15 15:48:16.000000 datatoolbox-0.5.6/datatoolbox/data/country_codes.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     1711 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/datatoolbox/data/datashelf_contents.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)     2923 2021-12-16 12:32:58.000000 datatoolbox-0.5.6/datatoolbox/data/external_mappings.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      178 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/data/personal_template.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      999 2019-08-14 10:00:22.000000 datatoolbox-0.5.6/datatoolbox/data/regions.csv
+-rwxrwx---   0 root         (0) vboxsf     (999)   237054 2023-04-28 11:35:43.000000 datatoolbox-0.5.6/datatoolbox/data_readers.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    68067 2023-05-04 07:37:43.000000 datatoolbox-0.5.6/datatoolbox/data_structures.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    64211 2023-05-10 08:59:02.000000 datatoolbox-0.5.6/datatoolbox/database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     6730 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/greenhouse_gas_database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3542 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/init_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    21652 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/interfaces.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    10991 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/io_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    41818 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/mapping.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2854 2022-12-01 09:27:15.000000 datatoolbox-0.5.6/datatoolbox/naming_convention.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3305 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/patches.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2175 2022-11-16 12:15:23.000000 datatoolbox-0.5.6/datatoolbox/pint_definitions.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.6/datatoolbox/relations.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    26527 2023-04-05 07:52:48.000000 datatoolbox-0.5.6/datatoolbox/sets.py
+-rwxrwx---   0 root         (0) vboxsf     (999)        0 2020-06-08 07:09:19.000000 datatoolbox-0.5.6/datatoolbox/storage.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1632 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/templates.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox/tools/
+-rwxrwx---   0 root         (0) vboxsf     (999)    16351 2021-04-19 11:31:45.000000 datatoolbox-0.5.6/datatoolbox/tools/CRF_extract_CA_2021.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)    28022 2021-02-02 15:17:26.000000 datatoolbox-0.5.6/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)    17445 2021-02-02 12:48:44.000000 datatoolbox-0.5.6/datatoolbox/tools/IEA_B2DS_4.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)    17375 2019-12-20 11:46:57.000000 datatoolbox-0.5.6/datatoolbox/tools/WEO_2019_test.SCEN
+-rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/__init__.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4320 2022-11-17 09:58:39.000000 datatoolbox-0.5.6/datatoolbox/tools/conversion_to_v0.3.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    42729 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/excel.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      370 2022-11-17 09:58:39.000000 datatoolbox-0.5.6/datatoolbox/tools/export_all.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4441 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/for_datatables.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     8132 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/html.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      182 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/install_support.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7188 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/kaya_idendentiy_decomposition.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     4283 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/magicc6.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5931 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/matplotlib.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3797 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/pandas.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5533 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/py_magicc_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7869 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/pyam.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      965 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/renaming_DB.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    84992 2019-08-14 10:26:08.000000 datatoolbox-0.5.6/datatoolbox/tools/run_MAGICC_startup_simple.xlsx
+-rwxrwx---   0 root         (0) vboxsf     (999)     1830 2021-02-02 14:03:36.000000 datatoolbox-0.5.6/datatoolbox/tools/run_magicc6.m
+-rwxrwx---   0 root         (0) vboxsf     (999)     1044 2022-11-17 09:58:40.000000 datatoolbox-0.5.6/datatoolbox/tools/statistics.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    61174 2021-06-03 14:06:07.000000 datatoolbox-0.5.6/datatoolbox/tools/test.docx
+-rwxrwx---   0 root         (0) vboxsf     (999)     8625 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/tools/word.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     9617 2023-03-30 13:29:22.000000 datatoolbox-0.5.6/datatoolbox/tools/xarray.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/datatoolbox/tutorials/
+-rwxrwx---   0 root         (0) vboxsf     (999)     2996 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/datatoolbox/tutorials/00_search_find_and_access_data.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1019 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/tutorials/01_emission_comparison.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2096 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/datatoolbox/tutorials/02_unit_conversion.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     5685 2020-10-14 14:04:18.000000 datatoolbox-0.5.6/datatoolbox/tutorials/03_intermediate_example.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1416 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/datatoolbox/tutorials/04_sources.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      382 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/datatoolbox/tutorials/05_plot_source_content.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      734 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/datatoolbox/tutorials/06_xarray_examples.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1142 2021-05-11 13:19:29.000000 datatoolbox-0.5.6/datatoolbox/tutorials/07_renewable_share_compuation.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      793 2021-05-11 12:59:38.000000 datatoolbox-0.5.6/datatoolbox/tutorials/08_low_carbon_fuel_computation.py
+-rwxrwx---   0 root         (0) vboxsf     (999)   137631 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/datatoolbox/tutorials/introduction_v1.ipynb
+-rwxrwx---   0 root         (0) vboxsf     (999)     4631 2022-03-22 14:54:50.000000 datatoolbox-0.5.6/datatoolbox/tutorials/jump_start.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      300 2022-11-21 13:35:45.000000 datatoolbox-0.5.6/datatoolbox/units.py
+-rwxrwx---   0 root         (0) vboxsf     (999)    43915 2022-11-22 09:50:19.000000 datatoolbox-0.5.6/datatoolbox/util.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      176 2023-05-10 09:20:54.000000 datatoolbox-0.5.6/datatoolbox/version.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      746 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/datatoolbox/workflows.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/
+-rwxrwx---   0 root         (0) vboxsf     (999)     1037 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/PKG-INFO
+-rwxrwx---   0 root         (0) vboxsf     (999)     3714 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/SOURCES.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)        1 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/dependency_links.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)      149 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/requires.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       12 2023-05-10 09:20:55.000000 datatoolbox-0.5.6/datatoolbox.egg-info/top_level.txt
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/doc/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7755 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/doc/Makefile
+-rwxrwx---   0 root         (0) vboxsf     (999)     9684 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/conf.py
+-rwxrwx---   0 root         (0) vboxsf     (999)       79 2021-01-05 10:54:01.000000 datatoolbox-0.5.6/doc/core.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      149 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/data_structures.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      122 2021-01-11 16:19:59.000000 datatoolbox-0.5.6/doc/database.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       91 2021-01-11 16:18:53.000000 datatoolbox-0.5.6/doc/database_database.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      130 2021-01-11 16:21:50.000000 datatoolbox-0.5.6/doc/database_gitrepomanager.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       93 2021-01-11 16:03:03.000000 datatoolbox-0.5.6/doc/excel.rst
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/doc/figures/
+-rwxrwx---   0 root         (0) vboxsf     (999)    21579 2020-11-09 13:08:35.000000 datatoolbox-0.5.6/doc/figures/ID_meta_data.svg
+-rwxrwx---   0 root         (0) vboxsf     (999)    67463 2021-05-17 15:08:58.000000 datatoolbox-0.5.6/doc/figures/config_input.png
+-rwxrwx---   0 root         (0) vboxsf     (999)     7157 2021-05-17 15:04:37.000000 datatoolbox-0.5.6/doc/first_steps.md
+-rwxrwx---   0 root         (0) vboxsf     (999)      100 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/foo.rst_template
+-rwxrwx---   0 root         (0) vboxsf     (999)       77 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/help.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      463 2021-01-11 16:06:28.000000 datatoolbox-0.5.6/doc/index.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)     1754 2021-05-21 08:03:28.000000 datatoolbox-0.5.6/doc/installation.md
+-rwxrwx---   0 root         (0) vboxsf     (999)     1080 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/doc/license.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)     7353 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/doc/make.bat
+-rwxrwx---   0 root         (0) vboxsf     (999)      103 2021-01-11 16:09:22.000000 datatoolbox-0.5.6/doc/matplotlib.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:10:43.000000 datatoolbox-0.5.6/doc/pandas.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)      133 2021-01-11 16:20:57.000000 datatoolbox-0.5.6/doc/tools.rst
+-rwxrwx---   0 root         (0) vboxsf     (999)       95 2021-01-11 16:09:13.000000 datatoolbox-0.5.6/doc/xarray.rst
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/documentation/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7761 2020-12-22 15:09:15.000000 datatoolbox-0.5.6/documentation/Datatoolbox - First steps.md
+-rwxrwx---   0 root         (0) vboxsf     (999)      381 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/environment.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      418 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/make_proj.sh
+-rwxrwx---   0 root         (0) vboxsf     (999)      558 2021-01-12 15:45:18.000000 datatoolbox-0.5.6/readthedocs.yml
+-rwxrwx---   0 root         (0) vboxsf     (999)      215 2022-10-19 13:17:33.000000 datatoolbox-0.5.6/requirements.txt
+-rwxrwx---   0 root         (0) vboxsf     (999)       38 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/setup.cfg
+-rwxrwx---   0 root         (0) vboxsf     (999)     1839 2023-05-03 11:16:28.000000 datatoolbox-0.5.6/setup.py
+drwxrwx---   0 root         (0) vboxsf     (999)        0 2023-05-10 09:20:56.000000 datatoolbox-0.5.6/tests/
+-rwxrwx---   0 root         (0) vboxsf     (999)     7292 2022-12-19 11:29:58.000000 datatoolbox-0.5.6/tests/test_calculations.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      696 2022-11-18 16:16:07.000000 datatoolbox-0.5.6/tests/test_converters.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2836 2022-11-21 11:08:31.000000 datatoolbox-0.5.6/tests/test_database.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1640 2023-03-30 13:32:13.000000 datatoolbox-0.5.6/tests/test_dataset.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     7741 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/tests/test_datatable.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1063 2022-11-16 11:59:46.000000 datatoolbox-0.5.6/tests/test_io.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      390 2022-11-22 09:54:34.000000 datatoolbox-0.5.6/tests/test_linked_functions.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1563 2023-05-04 07:49:24.000000 datatoolbox-0.5.6/tests/test_pyam.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     3570 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/tests/test_tableset.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2610 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/tests/test_tools.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     1227 2022-11-21 13:23:54.000000 datatoolbox-0.5.6/tests/test_units.py
+-rwxrwx---   0 root         (0) vboxsf     (999)      870 2020-10-14 14:04:19.000000 datatoolbox-0.5.6/tests/test_utilities.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2437 2022-10-19 13:17:33.000000 datatoolbox-0.5.6/tests/test_xarray.py
+-rwxrwx---   0 root         (0) vboxsf     (999)     2959 2022-05-25 07:15:53.000000 datatoolbox-0.5.6/tests/util_for_testing.py
```

### Comparing `datatoolbox-0.5.5/.gitlab-ci.yml` & `datatoolbox-0.5.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/.travis.yml` & `datatoolbox-0.5.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/LICENSE` & `datatoolbox-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/PKG-INFO` & `datatoolbox-0.5.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.5.5
+Version: 0.5.6
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.5.5/README.md` & `datatoolbox-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/appveyor.yml` & `datatoolbox-0.5.6/appveyor.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/ci/appveyor/install.ps1` & `datatoolbox-0.5.6/ci/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/ci/appveyor/run_with_env.cmd` & `datatoolbox-0.5.6/ci/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/__init__.py` & `datatoolbox-0.5.6/datatoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/admin.py` & `datatoolbox-0.5.6/datatoolbox/admin.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/config.py` & `datatoolbox-0.5.6/datatoolbox/config.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/converters.py` & `datatoolbox-0.5.6/datatoolbox/converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/core.py` & `datatoolbox-0.5.6/datatoolbox/core.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/GHG_alternative_naming.pkl` & `datatoolbox-0.5.6/datatoolbox/data/GHG_alternative_naming.pkl`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/GHG_properties_2019_CA.csv` & `datatoolbox-0.5.6/datatoolbox/data/GHG_properties_2019_CA.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv` & `datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv` & `datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv` & `datatoolbox-0.5.6/datatoolbox/data/SANDBOX_datashelf/mappings/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/all.csv` & `datatoolbox-0.5.6/datatoolbox/data/all.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/compatible1_5_unfiltered.xlsx` & `datatoolbox-0.5.6/datatoolbox/data/compatible1_5_unfiltered.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/continent.csv` & `datatoolbox-0.5.6/datatoolbox/data/continent.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/country_codes.csv` & `datatoolbox-0.5.6/datatoolbox/data/country_codes.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/datashelf_contents.csv` & `datatoolbox-0.5.6/datatoolbox/data/datashelf_contents.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/external_mappings.py` & `datatoolbox-0.5.6/datatoolbox/data/external_mappings.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data/regions.csv` & `datatoolbox-0.5.6/datatoolbox/data/regions.csv`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data_readers.py` & `datatoolbox-0.5.6/datatoolbox/data_readers.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/data_structures.py` & `datatoolbox-0.5.6/datatoolbox/data_structures.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/database.py` & `datatoolbox-0.5.6/datatoolbox/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1329,14 +1329,21 @@
         repo = self.repositories[sourceID]
         if sourceID not in self.validatedRepos:
             self._validateRepository(sourceID)
         return repo
 
     #%% Private methods
     
+    def _ssh_agent_running(self):
+        import subprocess
+
+        proc = subprocess.Popen(["ssh-add -l"], stdout=subprocess.PIPE, shell=True)
+        (out, err) = proc.communicate()
+        return not out.startswith(b'The agent has no identities')
+
     def _get_difference_to_remote(self):
         
         new_items = self.remote_sources.index.difference(
             self.sources.index
         )
         compare_df = self.sources.copy()
         compare_df['remote_tag'] = self.remote_sources['tag']
@@ -1532,17 +1539,20 @@
             # check for remote data
             try:
                 if foreground:
                     print("Looking for new online sources...", end='')
                     self._pull_remote_sources()
                     print("Done!")    
                 else:
-                    print("Looking for new online sources in the backgound")
-                    thread = Thread(target=self._pull_remote_sources)
-                    thread.start()
+                    if self._ssh_agent_running():
+                        print("Looking for new online sources in the backgound")
+                        thread = Thread(target=self._pull_remote_sources)
+                        thread.start()
+                    else:
+                        print('SSH agent not running, not checking for remote data.')
                 # 
                 # print("Done!")
             except:
                 print("Could not check online data repository")
                 import traceback
 
                 traceback.print_exc()
```

### Comparing `datatoolbox-0.5.5/datatoolbox/greenhouse_gas_database.py` & `datatoolbox-0.5.6/datatoolbox/greenhouse_gas_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/init_tools.py` & `datatoolbox-0.5.6/datatoolbox/init_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/interfaces.py` & `datatoolbox-0.5.6/datatoolbox/interfaces.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/io_tools.py` & `datatoolbox-0.5.6/datatoolbox/io_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/mapping.py` & `datatoolbox-0.5.6/datatoolbox/mapping.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/naming_convention.py` & `datatoolbox-0.5.6/datatoolbox/naming_convention.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/patches.py` & `datatoolbox-0.5.6/datatoolbox/patches.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/pint_definitions.txt` & `datatoolbox-0.5.6/datatoolbox/pint_definitions.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/sets.py` & `datatoolbox-0.5.6/datatoolbox/sets.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/templates.py` & `datatoolbox-0.5.6/datatoolbox/templates.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/CRF_extract_CA_2021.xlsx` & `datatoolbox-0.5.6/datatoolbox/tools/CRF_extract_CA_2021.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN` & `datatoolbox-0.5.6/datatoolbox/tools/EQW_SPLIT_EFF0460_CATEFFEXT_210120.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/IEA_B2DS_4.SCEN` & `datatoolbox-0.5.6/datatoolbox/tools/IEA_B2DS_4.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/WEO_2019_test.SCEN` & `datatoolbox-0.5.6/datatoolbox/tools/WEO_2019_test.SCEN`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/conversion_to_v0.3.py` & `datatoolbox-0.5.6/datatoolbox/tools/conversion_to_v0.3.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/excel.py` & `datatoolbox-0.5.6/datatoolbox/tools/excel.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/for_datatables.py` & `datatoolbox-0.5.6/datatoolbox/tools/for_datatables.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/html.py` & `datatoolbox-0.5.6/datatoolbox/tools/html.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/kaya_idendentiy_decomposition.py` & `datatoolbox-0.5.6/datatoolbox/tools/kaya_idendentiy_decomposition.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/magicc6.py` & `datatoolbox-0.5.6/datatoolbox/tools/magicc6.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/matplotlib.py` & `datatoolbox-0.5.6/datatoolbox/tools/matplotlib.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/pandas.py` & `datatoolbox-0.5.6/datatoolbox/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/py_magicc_tools.py` & `datatoolbox-0.5.6/datatoolbox/tools/py_magicc_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/pyam.py` & `datatoolbox-0.5.6/datatoolbox/tools/pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/renaming_DB.py` & `datatoolbox-0.5.6/datatoolbox/tools/renaming_DB.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/run_MAGICC_startup_simple.xlsx` & `datatoolbox-0.5.6/datatoolbox/tools/run_MAGICC_startup_simple.xlsx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/run_magicc6.m` & `datatoolbox-0.5.6/datatoolbox/tools/run_magicc6.m`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/statistics.py` & `datatoolbox-0.5.6/datatoolbox/tools/statistics.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/test.docx` & `datatoolbox-0.5.6/datatoolbox/tools/test.docx`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/word.py` & `datatoolbox-0.5.6/datatoolbox/tools/word.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tools/xarray.py` & `datatoolbox-0.5.6/datatoolbox/tools/xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/00_search_find_and_access_data.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/00_search_find_and_access_data.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/01_emission_comparison.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/01_emission_comparison.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/02_unit_conversion.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/02_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/03_intermediate_example.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/03_intermediate_example.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/04_sources.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/04_sources.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/06_xarray_examples.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/06_xarray_examples.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/07_renewable_share_compuation.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/07_renewable_share_compuation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/08_low_carbon_fuel_computation.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/08_low_carbon_fuel_computation.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/introduction_v1.ipynb` & `datatoolbox-0.5.6/datatoolbox/tutorials/introduction_v1.ipynb`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/tutorials/jump_start.py` & `datatoolbox-0.5.6/datatoolbox/tutorials/jump_start.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/util.py` & `datatoolbox-0.5.6/datatoolbox/util.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox/workflows.py` & `datatoolbox-0.5.6/datatoolbox/workflows.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/datatoolbox.egg-info/PKG-INFO` & `datatoolbox-0.5.6/datatoolbox.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatoolbox
-Version: 0.5.5
+Version: 0.5.6
 Summary: The Python Data Toolbox
 Home-page: https://gitlab.com/climateanalytics/datatoolbox
 Author: Andreas Geiges
 Author-email: a.geiges@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `datatoolbox-0.5.5/datatoolbox.egg-info/SOURCES.txt` & `datatoolbox-0.5.6/datatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/doc/Makefile` & `datatoolbox-0.5.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/doc/conf.py` & `datatoolbox-0.5.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/doc/figures/ID_meta_data.svg` & `datatoolbox-0.5.6/doc/figures/ID_meta_data.svg`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/doc/figures/config_input.png` & `datatoolbox-0.5.6/doc/figures/config_input.png`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/doc/first_steps.md` & `datatoolbox-0.5.6/doc/first_steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/doc/installation.md` & `datatoolbox-0.5.6/doc/installation.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/doc/license.rst` & `datatoolbox-0.5.6/doc/license.rst`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/doc/make.bat` & `datatoolbox-0.5.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/documentation/Datatoolbox - First steps.md` & `datatoolbox-0.5.6/documentation/Datatoolbox - First steps.md`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/readthedocs.yml` & `datatoolbox-0.5.6/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/setup.py` & `datatoolbox-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_calculations.py` & `datatoolbox-0.5.6/tests/test_calculations.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_converters.py` & `datatoolbox-0.5.6/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_database.py` & `datatoolbox-0.5.6/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_dataset.py` & `datatoolbox-0.5.6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_datatable.py` & `datatoolbox-0.5.6/tests/test_datatable.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_io.py` & `datatoolbox-0.5.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_pyam.py` & `datatoolbox-0.5.6/tests/test_pyam.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_tableset.py` & `datatoolbox-0.5.6/tests/test_tableset.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_tools.py` & `datatoolbox-0.5.6/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_units.py` & `datatoolbox-0.5.6/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_utilities.py` & `datatoolbox-0.5.6/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/test_xarray.py` & `datatoolbox-0.5.6/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `datatoolbox-0.5.5/tests/util_for_testing.py` & `datatoolbox-0.5.6/tests/util_for_testing.py`

 * *Files identical despite different names*

