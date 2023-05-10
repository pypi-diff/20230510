# Comparing `tmp/vise-0.7.1.tar.gz` & `tmp/vise-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vise-0.7.1.tar", last modified: Sun Apr 23 00:27:13 2023, max compression
+gzip compressed data, was "dist/vise-0.7.2.tar", last modified: Wed May 10 02:36:57 2023, max compression
```

## Comparing `vise-0.7.1.tar` & `vise-0.7.2.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.330232 vise-0.7.1/
--rw-r--r--   0 kumagai    (501) staff       (20)      179 2020-12-23 04:48:27.000000 vise-0.7.1/MANIFEST.in
--rw-r--r--   0 kumagai    (501) staff       (20)     4389 2023-04-23 00:27:13.329938 vise-0.7.1/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     3247 2022-07-28 01:56:51.000000 vise-0.7.1/README.md
--rw-r--r--   0 kumagai    (501) staff       (20)       38 2023-04-23 00:27:13.330326 vise-0.7.1/setup.cfg
--rw-r--r--   0 kumagai    (501) staff       (20)     1460 2022-06-27 23:50:06.000000 vise-0.7.1/setup.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.130392 vise-0.7.1/vise/
--rw-r--r--   0 kumagai    (501) staff       (20)       37 2020-05-15 22:51:22.000000 vise-0.7.1/vise/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.144455 vise-0.7.1/vise/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/analyzer/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1633 2021-03-06 05:00:49.000000 vise-0.7.1/vise/analyzer/atom_grouping_type.py
--rwxr-xr-x   0 kumagai    (501) staff       (20)     7574 2022-10-21 08:31:12.000000 vise-0.7.1/vise/analyzer/band_edge_properties.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7667 2022-12-06 07:44:43.000000 vise-0.7.1/vise/analyzer/dielectric_function.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.148730 vise-0.7.1/vise/analyzer/dielectric_function_data/
--rw-r--r--   0 kumagai    (501) staff       (20)     3188 2020-11-07 08:48:51.000000 vise-0.7.1/vise/analyzer/dielectric_function_data/GaAs.csv
--rw-r--r--   0 kumagai    (501) staff       (20)     3474 2020-11-07 08:58:34.000000 vise-0.7.1/vise/analyzer/dielectric_function_data/Si.csv
--rw-r--r--   0 kumagai    (501) staff       (20)     1422 2020-11-12 08:22:54.000000 vise-0.7.1/vise/analyzer/dielectric_function_data/exp_dielectric_func.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9812 2023-03-05 02:28:14.000000 vise-0.7.1/vise/analyzer/dos_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2222 2021-05-25 08:13:08.000000 vise-0.7.1/vise/analyzer/effective_mass.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12797 2022-09-10 03:08:43.000000 vise-0.7.1/vise/analyzer/plot_band.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12057 2022-09-12 04:32:47.000000 vise-0.7.1/vise/analyzer/plot_band_dos.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6509 2022-10-12 07:02:26.000000 vise-0.7.1/vise/analyzer/plot_brillouin_zone.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7891 2022-12-06 07:45:00.000000 vise-0.7.1/vise/analyzer/plot_diele_func_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4553 2022-12-06 07:30:30.000000 vise-0.7.1/vise/analyzer/plot_dos.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.160482 vise-0.7.1/vise/analyzer/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/analyzer/vasp/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2231 2022-08-19 06:07:54.000000 vise-0.7.1/vise/analyzer/vasp/band_edge_properties.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2968 2022-12-06 07:08:20.000000 vise-0.7.1/vise/analyzer/vasp/dos_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1474 2021-08-06 10:07:19.000000 vise-0.7.1/vise/analyzer/vasp/handle_volumetric_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1866 2022-09-23 02:12:27.000000 vise-0.7.1/vise/analyzer/vasp/make_diele_func.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1242 2021-06-24 07:47:02.000000 vise-0.7.1/vise/analyzer/vasp/make_effective_mass.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3658 2022-10-04 04:01:43.000000 vise-0.7.1/vise/analyzer/vasp/make_irreps.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6229 2022-10-06 05:30:09.000000 vise-0.7.1/vise/analyzer/vasp/plot_band.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.186033 vise-0.7.1/vise/analyzer/vesta/
--rw-r--r--   0 kumagai    (501) staff       (20)       61 2021-03-12 02:41:40.000000 vise-0.7.1/vise/analyzer/vesta/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4183 2021-03-02 07:24:45.000000 vise-0.7.1/vise/analyzer/vesta/element_colors.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12453 2021-07-05 05:51:09.000000 vise-0.7.1/vise/analyzer/vesta/vesta_file.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.192979 vise-0.7.1/vise/atom_energies/
--rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 vise-0.7.1/vise/atom_energies/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)      290 2020-11-30 06:52:18.000000 vise-0.7.1/vise/atom_energies/atom_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)      515 2020-08-11 09:15:50.000000 vise-0.7.1/vise/atom_energies/atom_magnetization_hund.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1217 2021-08-04 07:35:01.000000 vise-0.7.1/vise/atom_energies/get_energy.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2267 2022-07-05 01:18:05.000000 vise-0.7.1/vise/atom_energies/make_atom_vasp_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1135 2020-11-30 02:31:47.000000 vise-0.7.1/vise/atom_energies/mp_atom_energy.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      709 2020-11-30 02:31:47.000000 vise-0.7.1/vise/atom_energies/mp_atom_mag.yaml
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.197467 vise-0.7.1/vise/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)       72 2020-05-15 22:51:22.000000 vise-0.7.1/vise/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)    14069 2023-04-22 22:01:47.000000 vise-0.7.1/vise/cli/main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    14642 2023-04-22 22:07:43.000000 vise-0.7.1/vise/cli/main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3506 2020-10-03 03:00:38.000000 vise-0.7.1/vise/cli/main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4944 2021-08-06 10:08:41.000000 vise-0.7.1/vise/cli/main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2216 2021-05-05 00:16:26.000000 vise-0.7.1/vise/cli/main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4294 2022-11-14 04:27:07.000000 vise-0.7.1/vise/defaults.py
--rw-r--r--   0 kumagai    (501) staff       (20)      134 2020-05-15 22:51:22.000000 vise-0.7.1/vise/error.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.206475 vise-0.7.1/vise/input_set/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.211344 vise-0.7.1/vise/input_set/datasets/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2594 2023-04-22 23:04:53.000000 vise-0.7.1/vise/input_set/datasets/dataset_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1642 2022-12-19 07:34:18.000000 vise-0.7.1/vise/input_set/datasets/incar_flags.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      685 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/kpar_set.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      294 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/magmom.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1516 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/potcar_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4024 2020-12-23 01:37:43.000000 vise-0.7.1/vise/input_set/datasets/potcar_set.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      623 2021-05-06 06:02:40.000000 vise-0.7.1/vise/input_set/datasets/u_parameter_set.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)      574 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/datasets/unoccupied_bands.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)     1141 2022-07-23 04:43:00.000000 vise-0.7.1/vise/input_set/fft_grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4149 2023-04-22 23:06:02.000000 vise-0.7.1/vise/input_set/incar.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12667 2022-11-30 06:56:02.000000 vise-0.7.1/vise/input_set/incar_settings_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4026 2022-11-14 04:20:42.000000 vise-0.7.1/vise/input_set/input_options.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1360 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/kpoints.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1279 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/kpoints_mode.py
--rw-r--r--   0 kumagai    (501) staff       (20)      914 2020-05-15 22:51:22.000000 vise-0.7.1/vise/input_set/potcar_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4022 2021-08-04 07:35:03.000000 vise-0.7.1/vise/input_set/prior_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8136 2023-04-22 21:47:54.000000 vise-0.7.1/vise/input_set/structure_kpoints_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3912 2022-10-06 08:28:55.000000 vise-0.7.1/vise/input_set/task.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4131 2022-11-04 09:21:10.000000 vise-0.7.1/vise/input_set/vasp_input_files.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1322 2022-10-21 08:42:57.000000 vise-0.7.1/vise/input_set/vise_log.py
--rw-r--r--   0 kumagai    (501) staff       (20)      956 2020-06-03 03:20:45.000000 vise-0.7.1/vise/input_set/xc.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.213846 vise-0.7.1/vise/tests/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.220763 vise-0.7.1/vise/tests/analyzer/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/analyzer/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1503 2020-11-30 08:10:26.000000 vise-0.7.1/vise/tests/analyzer/test_atom_grouping_type.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8181 2022-09-30 06:32:39.000000 vise-0.7.1/vise/tests/analyzer/test_band_edge_properties.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3441 2022-11-03 04:27:22.000000 vise-0.7.1/vise/tests/analyzer/test_dielectric_function.py
--rw-r--r--   0 kumagai    (501) staff       (20)    10283 2023-01-31 00:31:50.000000 vise-0.7.1/vise/tests/analyzer/test_dos_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1951 2021-05-25 08:12:05.000000 vise-0.7.1/vise/tests/analyzer/test_effective_mass.py
--rw-r--r--   0 kumagai    (501) staff       (20)    12879 2022-09-13 00:24:09.000000 vise-0.7.1/vise/tests/analyzer/test_plot_band.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1576 2022-09-12 00:48:30.000000 vise-0.7.1/vise/tests/analyzer/test_plot_band_dos.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2099 2022-10-21 06:44:45.000000 vise-0.7.1/vise/tests/analyzer/test_plot_brillouin_zone.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2639 2022-12-06 07:46:00.000000 vise-0.7.1/vise/tests/analyzer/test_plot_diele_func_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     7869 2022-12-06 07:02:33.000000 vise-0.7.1/vise/tests/analyzer/test_plot_dos.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.225056 vise-0.7.1/vise/tests/analyzer/vasp/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/analyzer/vasp/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2282 2021-03-06 04:52:09.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_band_edge_properties.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3504 2021-03-06 04:52:35.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_dos_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1607 2022-10-21 07:15:26.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_handle_volumetric_data.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1900 2022-09-23 00:52:48.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_make_diele_func.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2517 2021-06-24 07:56:18.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_make_effective_mass.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2015 2022-09-13 01:26:49.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_make_irreps.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5783 2022-10-06 05:29:21.000000 vise-0.7.1/vise/tests/analyzer/vasp/test_plot_band.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.228501 vise-0.7.1/vise/tests/cli/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/cli/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8832 2023-04-22 22:01:47.000000 vise-0.7.1/vise/tests/cli/test_main.py
--rw-r--r--   0 kumagai    (501) staff       (20)    11040 2023-04-22 22:12:44.000000 vise-0.7.1/vise/tests/cli/test_main_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1683 2022-07-29 02:57:51.000000 vise-0.7.1/vise/tests/cli/test_main_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2249 2021-04-30 01:10:17.000000 vise-0.7.1/vise/tests/cli/test_main_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2463 2021-05-04 23:31:17.000000 vise-0.7.1/vise/tests/cli/test_main_util_functions.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1785 2022-09-10 03:00:55.000000 vise-0.7.1/vise/tests/conftest.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.229881 vise-0.7.1/vise/tests/helpers/
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 vise-0.7.1/vise/tests/helpers/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     5858 2023-01-31 00:32:00.000000 vise-0.7.1/vise/tests/helpers/assertion.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4419 2022-09-30 04:31:05.000000 vise-0.7.1/vise/tests/helpers/test_assersion.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.237230 vise-0.7.1/vise/tests/input_set/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/input_set/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.239008 vise-0.7.1/vise/tests/input_set/datasets/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/input_set/datasets/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1519 2022-11-14 04:00:11.000000 vise-0.7.1/vise/tests/input_set/datasets/test_dataset_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)      780 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/input_set/datasets/test_potcar_set.py
--rw-r--r--   0 kumagai    (501) staff       (20)      232 2022-01-27 04:37:06.000000 vise-0.7.1/vise/tests/input_set/test_fft_grids.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1667 2023-04-22 23:04:07.000000 vise-0.7.1/vise/tests/input_set/test_incar.py
--rw-r--r--   0 kumagai    (501) staff       (20)     8997 2022-11-14 04:40:23.000000 vise-0.7.1/vise/tests/input_set/test_incar_settings_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3796 2022-07-26 07:16:22.000000 vise-0.7.1/vise/tests/input_set/test_input_options.py
--rw-r--r--   0 kumagai    (501) staff       (20)      533 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/input_set/test_kpoints_mode.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1555 2021-03-05 09:50:13.000000 vise-0.7.1/vise/tests/input_set/test_potcar_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2565 2022-07-01 00:59:32.000000 vise-0.7.1/vise/tests/input_set/test_prior_info.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9329 2023-03-08 02:30:32.000000 vise-0.7.1/vise/tests/input_set/test_structure_kpoints_generator.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3410 2022-10-06 08:28:37.000000 vise-0.7.1/vise/tests/input_set/test_task.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1573 2022-11-14 04:18:29.000000 vise-0.7.1/vise/tests/input_set/test_vasp_input_files.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1211 2022-10-21 08:43:44.000000 vise-0.7.1/vise/tests/input_set/test_vise_log.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1162 2021-03-02 02:37:28.000000 vise-0.7.1/vise/tests/input_set/test_xc.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4762 2022-11-06 00:50:42.000000 vise-0.7.1/vise/tests/test_defaults.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1784 2022-10-21 08:06:31.000000 vise-0.7.1/vise/tests/test_user_settings.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.290516 vise-0.7.1/vise/tests/util/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/__init__.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.292175 vise-0.7.1/vise/tests/util/phonopy/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/phonopy/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     3100 2021-08-06 10:08:41.000000 vise-0.7.1/vise/tests/util/phonopy/test_phonopy_input.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1499 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/test_bravais_lattice.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2441 2021-03-05 09:50:13.000000 vise-0.7.1/vise/tests/util/test_centering.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4437 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/test_file_transfer.py
--rw-r--r--   0 kumagai    (501) staff       (20)      217 2020-08-02 02:24:25.000000 vise-0.7.1/vise/tests/util/test_logger.py
--rw-r--r--   0 kumagai    (501) staff       (20)      511 2020-05-15 22:51:22.000000 vise-0.7.1/vise/tests/util/test_matplotlib.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1500 2022-09-28 23:59:57.000000 vise-0.7.1/vise/tests/util/test_mix_in.py
--rw-r--r--   0 kumagai    (501) staff       (20)      232 2021-04-18 02:48:05.000000 vise-0.7.1/vise/tests/util/test_string.py
--rw-r--r--   0 kumagai    (501) staff       (20)     9778 2021-07-31 08:14:24.000000 vise-0.7.1/vise/tests/util/test_structure_symmetrizer.py
--rw-r--r--   0 kumagai    (501) staff       (20)      471 2021-08-01 00:43:34.000000 vise-0.7.1/vise/tests/util/test_valence_orbitals_from_potcar.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2143 2022-11-15 04:24:17.000000 vise-0.7.1/vise/user_settings.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.308520 vise-0.7.1/vise/util/
--rw-r--r--   0 kumagai    (501) staff       (20)     3450 2021-09-15 23:40:59.000000 vise-0.7.1/vise/util/Hermann-Mauguin.yaml
--rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.1/vise/util/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     6893 2023-03-07 23:24:41.000000 vise-0.7.1/vise/util/bravais_lattice.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1786 2020-05-14 03:15:55.000000 vise-0.7.1/vise/util/centering.py
--rw-r--r--   0 kumagai    (501) staff       (20)      304 2020-11-12 05:19:29.000000 vise-0.7.1/vise/util/dash_helper.py
--rw-r--r--   0 kumagai    (501) staff       (20)      788 2021-05-30 03:06:06.000000 vise-0.7.1/vise/util/enum.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2746 2020-11-30 22:31:41.000000 vise-0.7.1/vise/util/file_transfer.py
--rw-r--r--   0 kumagai    (501) staff       (20)     1234 2021-05-01 05:11:26.000000 vise-0.7.1/vise/util/logger.py
--rw-r--r--   0 kumagai    (501) staff       (20)      802 2020-05-15 22:51:22.000000 vise-0.7.1/vise/util/matplotlib.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2752 2022-09-30 04:31:19.000000 vise-0.7.1/vise/util/mix_in.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.329227 vise-0.7.1/vise/util/phonopy/
--rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.1/vise/util/phonopy/__init__.py
--rw-r--r--   0 kumagai    (501) staff       (20)     4058 2022-09-06 01:13:47.000000 vise-0.7.1/vise/util/phonopy/phonopy_input.py
--rw-r--r--   0 kumagai    (501) staff       (20)     2043 2021-08-11 05:37:35.000000 vise-0.7.1/vise/util/plotly_util.py
--rw-r--r--   0 kumagai    (501) staff       (20)      986 2022-07-29 03:01:33.000000 vise-0.7.1/vise/util/str_related_tools.py
--rw-r--r--   0 kumagai    (501) staff       (20)      786 2021-04-20 00:50:10.000000 vise-0.7.1/vise/util/string.py
--rw-r--r--   0 kumagai    (501) staff       (20)      486 2021-03-05 09:50:13.000000 vise-0.7.1/vise/util/structure_handler.py
--rw-r--r--   0 kumagai    (501) staff       (20)    13330 2022-11-14 04:29:55.000000 vise-0.7.1/vise/util/structure_symmetrizer.py
--rw-r--r--   0 kumagai    (501) staff       (20)      229 2021-05-02 02:13:00.000000 vise-0.7.1/vise/util/typing.py
--rw-r--r--   0 kumagai    (501) staff       (20)      226 2021-07-05 05:51:09.000000 vise-0.7.1/vise/util/unit_conversion.py
--rw-r--r--   0 kumagai    (501) staff       (20)      419 2021-07-05 06:55:26.000000 vise-0.7.1/vise/util/valence_orbitals_from_potcar.py
--rw-r--r--   0 kumagai    (501) staff       (20)      117 2023-04-23 00:26:10.000000 vise-0.7.1/vise/version.py
-drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-04-23 00:27:13.132941 vise-0.7.1/vise.egg-info/
--rw-r--r--   0 kumagai    (501) staff       (20)     4389 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/PKG-INFO
--rw-r--r--   0 kumagai    (501) staff       (20)     5313 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/SOURCES.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        1 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/dependency_links.txt
--rw-r--r--   0 kumagai    (501) staff       (20)       81 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/entry_points.txt
--rw-r--r--   0 kumagai    (501) staff       (20)      163 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/requires.txt
--rw-r--r--   0 kumagai    (501) staff       (20)        5 2023-04-23 00:27:12.000000 vise-0.7.1/vise.egg-info/top_level.txt
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.932883 vise-0.7.2/
+-rw-r--r--   0 kumagai    (501) staff       (20)      179 2020-12-23 04:48:27.000000 vise-0.7.2/MANIFEST.in
+-rw-r--r--   0 kumagai    (501) staff       (20)     4389 2023-05-10 02:36:57.932572 vise-0.7.2/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     3247 2022-07-28 01:56:51.000000 vise-0.7.2/README.md
+-rw-r--r--   0 kumagai    (501) staff       (20)       38 2023-05-10 02:36:57.932983 vise-0.7.2/setup.cfg
+-rw-r--r--   0 kumagai    (501) staff       (20)     1460 2022-06-27 23:50:06.000000 vise-0.7.2/setup.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.703373 vise-0.7.2/vise/
+-rw-r--r--   0 kumagai    (501) staff       (20)       37 2020-05-15 22:51:22.000000 vise-0.7.2/vise/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.716935 vise-0.7.2/vise/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.2/vise/analyzer/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1633 2021-03-06 05:00:49.000000 vise-0.7.2/vise/analyzer/atom_grouping_type.py
+-rwxr-xr-x   0 kumagai    (501) staff       (20)     7574 2022-10-21 08:31:12.000000 vise-0.7.2/vise/analyzer/band_edge_properties.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7667 2022-12-06 07:44:43.000000 vise-0.7.2/vise/analyzer/dielectric_function.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.721701 vise-0.7.2/vise/analyzer/dielectric_function_data/
+-rw-r--r--   0 kumagai    (501) staff       (20)     3188 2020-11-07 08:48:51.000000 vise-0.7.2/vise/analyzer/dielectric_function_data/GaAs.csv
+-rw-r--r--   0 kumagai    (501) staff       (20)     3474 2020-11-07 08:58:34.000000 vise-0.7.2/vise/analyzer/dielectric_function_data/Si.csv
+-rw-r--r--   0 kumagai    (501) staff       (20)     1422 2020-11-12 08:22:54.000000 vise-0.7.2/vise/analyzer/dielectric_function_data/exp_dielectric_func.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9812 2023-03-05 02:28:14.000000 vise-0.7.2/vise/analyzer/dos_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2222 2021-05-25 08:13:08.000000 vise-0.7.2/vise/analyzer/effective_mass.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12797 2022-09-10 03:08:43.000000 vise-0.7.2/vise/analyzer/plot_band.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12057 2022-09-12 04:32:47.000000 vise-0.7.2/vise/analyzer/plot_band_dos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6509 2022-10-12 07:02:26.000000 vise-0.7.2/vise/analyzer/plot_brillouin_zone.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7891 2022-12-06 07:45:00.000000 vise-0.7.2/vise/analyzer/plot_diele_func_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4553 2022-12-06 07:30:30.000000 vise-0.7.2/vise/analyzer/plot_dos.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.731383 vise-0.7.2/vise/analyzer/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.2/vise/analyzer/vasp/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2231 2022-08-19 06:07:54.000000 vise-0.7.2/vise/analyzer/vasp/band_edge_properties.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2968 2022-12-06 07:08:20.000000 vise-0.7.2/vise/analyzer/vasp/dos_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1474 2021-08-06 10:07:19.000000 vise-0.7.2/vise/analyzer/vasp/handle_volumetric_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1866 2022-09-23 02:12:27.000000 vise-0.7.2/vise/analyzer/vasp/make_diele_func.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1242 2021-06-24 07:47:02.000000 vise-0.7.2/vise/analyzer/vasp/make_effective_mass.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3658 2022-10-04 04:01:43.000000 vise-0.7.2/vise/analyzer/vasp/make_irreps.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6229 2022-10-06 05:30:09.000000 vise-0.7.2/vise/analyzer/vasp/plot_band.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.760309 vise-0.7.2/vise/analyzer/vesta/
+-rw-r--r--   0 kumagai    (501) staff       (20)       61 2021-03-12 02:41:40.000000 vise-0.7.2/vise/analyzer/vesta/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4183 2021-03-02 07:24:45.000000 vise-0.7.2/vise/analyzer/vesta/element_colors.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12453 2021-07-05 05:51:09.000000 vise-0.7.2/vise/analyzer/vesta/vesta_file.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.790086 vise-0.7.2/vise/atom_energies/
+-rw-r--r--   0 kumagai    (501) staff       (20)       95 2020-05-18 00:09:10.000000 vise-0.7.2/vise/atom_energies/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      290 2020-11-30 06:52:18.000000 vise-0.7.2/vise/atom_energies/atom_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      515 2020-08-11 09:15:50.000000 vise-0.7.2/vise/atom_energies/atom_magnetization_hund.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1217 2021-08-04 07:35:01.000000 vise-0.7.2/vise/atom_energies/get_energy.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2267 2022-07-05 01:18:05.000000 vise-0.7.2/vise/atom_energies/make_atom_vasp_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1135 2020-11-30 02:31:47.000000 vise-0.7.2/vise/atom_energies/mp_atom_energy.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      709 2020-11-30 02:31:47.000000 vise-0.7.2/vise/atom_energies/mp_atom_mag.yaml
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.796135 vise-0.7.2/vise/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)       72 2020-05-15 22:51:22.000000 vise-0.7.2/vise/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    14069 2023-04-22 22:01:47.000000 vise-0.7.2/vise/cli/main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    14731 2023-04-23 00:38:21.000000 vise-0.7.2/vise/cli/main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3506 2020-10-03 03:00:38.000000 vise-0.7.2/vise/cli/main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4944 2021-08-06 10:08:41.000000 vise-0.7.2/vise/cli/main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2216 2021-05-05 00:16:26.000000 vise-0.7.2/vise/cli/main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4294 2022-11-14 04:27:07.000000 vise-0.7.2/vise/defaults.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      134 2020-05-15 22:51:22.000000 vise-0.7.2/vise/error.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.806389 vise-0.7.2/vise/input_set/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.811434 vise-0.7.2/vise/input_set/datasets/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/datasets/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2664 2023-04-23 00:36:04.000000 vise-0.7.2/vise/input_set/datasets/dataset_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1642 2022-12-19 07:34:18.000000 vise-0.7.2/vise/input_set/datasets/incar_flags.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      685 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/datasets/kpar_set.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      294 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/datasets/magmom.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1516 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/datasets/potcar_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4024 2020-12-23 01:37:43.000000 vise-0.7.2/vise/input_set/datasets/potcar_set.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      623 2021-05-06 06:02:40.000000 vise-0.7.2/vise/input_set/datasets/u_parameter_set.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)      574 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/datasets/unoccupied_bands.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)     1141 2022-07-23 04:43:00.000000 vise-0.7.2/vise/input_set/fft_grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4149 2023-04-22 23:06:02.000000 vise-0.7.2/vise/input_set/incar.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12667 2022-11-30 06:56:02.000000 vise-0.7.2/vise/input_set/incar_settings_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4026 2022-11-14 04:20:42.000000 vise-0.7.2/vise/input_set/input_options.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1360 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/kpoints.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1279 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/kpoints_mode.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      914 2020-05-15 22:51:22.000000 vise-0.7.2/vise/input_set/potcar_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4022 2021-08-04 07:35:03.000000 vise-0.7.2/vise/input_set/prior_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8136 2023-04-22 21:47:54.000000 vise-0.7.2/vise/input_set/structure_kpoints_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3912 2022-10-06 08:28:55.000000 vise-0.7.2/vise/input_set/task.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4131 2022-11-04 09:21:10.000000 vise-0.7.2/vise/input_set/vasp_input_files.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1322 2022-10-21 08:42:57.000000 vise-0.7.2/vise/input_set/vise_log.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      956 2020-06-03 03:20:45.000000 vise-0.7.2/vise/input_set/xc.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.815097 vise-0.7.2/vise/tests/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.821427 vise-0.7.2/vise/tests/analyzer/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/analyzer/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1503 2020-11-30 08:10:26.000000 vise-0.7.2/vise/tests/analyzer/test_atom_grouping_type.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8181 2022-09-30 06:32:39.000000 vise-0.7.2/vise/tests/analyzer/test_band_edge_properties.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3441 2022-11-03 04:27:22.000000 vise-0.7.2/vise/tests/analyzer/test_dielectric_function.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    10283 2023-01-31 00:31:50.000000 vise-0.7.2/vise/tests/analyzer/test_dos_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1951 2021-05-25 08:12:05.000000 vise-0.7.2/vise/tests/analyzer/test_effective_mass.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    12879 2022-09-13 00:24:09.000000 vise-0.7.2/vise/tests/analyzer/test_plot_band.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1576 2022-09-12 00:48:30.000000 vise-0.7.2/vise/tests/analyzer/test_plot_band_dos.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2099 2022-10-21 06:44:45.000000 vise-0.7.2/vise/tests/analyzer/test_plot_brillouin_zone.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2639 2022-12-06 07:46:00.000000 vise-0.7.2/vise/tests/analyzer/test_plot_diele_func_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     7869 2022-12-06 07:02:33.000000 vise-0.7.2/vise/tests/analyzer/test_plot_dos.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.847597 vise-0.7.2/vise/tests/analyzer/vasp/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/analyzer/vasp/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2282 2021-03-06 04:52:09.000000 vise-0.7.2/vise/tests/analyzer/vasp/test_band_edge_properties.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3504 2021-03-06 04:52:35.000000 vise-0.7.2/vise/tests/analyzer/vasp/test_dos_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1607 2022-10-21 07:15:26.000000 vise-0.7.2/vise/tests/analyzer/vasp/test_handle_volumetric_data.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1900 2022-09-23 00:52:48.000000 vise-0.7.2/vise/tests/analyzer/vasp/test_make_diele_func.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2517 2021-06-24 07:56:18.000000 vise-0.7.2/vise/tests/analyzer/vasp/test_make_effective_mass.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2015 2022-09-13 01:26:49.000000 vise-0.7.2/vise/tests/analyzer/vasp/test_make_irreps.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5783 2022-10-06 05:29:21.000000 vise-0.7.2/vise/tests/analyzer/vasp/test_plot_band.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.850742 vise-0.7.2/vise/tests/cli/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/cli/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8832 2023-04-22 22:01:47.000000 vise-0.7.2/vise/tests/cli/test_main.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    11040 2023-04-22 22:12:44.000000 vise-0.7.2/vise/tests/cli/test_main_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1683 2022-07-29 02:57:51.000000 vise-0.7.2/vise/tests/cli/test_main_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2249 2021-04-30 01:10:17.000000 vise-0.7.2/vise/tests/cli/test_main_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2463 2021-05-04 23:31:17.000000 vise-0.7.2/vise/tests/cli/test_main_util_functions.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1785 2022-09-10 03:00:55.000000 vise-0.7.2/vise/tests/conftest.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.852639 vise-0.7.2/vise/tests/helpers/
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-14 10:39:18.000000 vise-0.7.2/vise/tests/helpers/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     5858 2023-01-31 00:32:00.000000 vise-0.7.2/vise/tests/helpers/assertion.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4419 2022-09-30 04:31:05.000000 vise-0.7.2/vise/tests/helpers/test_assersion.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.861042 vise-0.7.2/vise/tests/input_set/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/input_set/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.862647 vise-0.7.2/vise/tests/input_set/datasets/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/input_set/datasets/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1519 2022-11-14 04:00:11.000000 vise-0.7.2/vise/tests/input_set/datasets/test_dataset_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      780 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/input_set/datasets/test_potcar_set.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      232 2022-01-27 04:37:06.000000 vise-0.7.2/vise/tests/input_set/test_fft_grids.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1667 2023-04-22 23:04:07.000000 vise-0.7.2/vise/tests/input_set/test_incar.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     8997 2022-11-14 04:40:23.000000 vise-0.7.2/vise/tests/input_set/test_incar_settings_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3796 2022-07-26 07:16:22.000000 vise-0.7.2/vise/tests/input_set/test_input_options.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      533 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/input_set/test_kpoints_mode.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1555 2021-03-05 09:50:13.000000 vise-0.7.2/vise/tests/input_set/test_potcar_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2565 2022-07-01 00:59:32.000000 vise-0.7.2/vise/tests/input_set/test_prior_info.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9329 2023-03-08 02:30:32.000000 vise-0.7.2/vise/tests/input_set/test_structure_kpoints_generator.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3410 2022-10-06 08:28:37.000000 vise-0.7.2/vise/tests/input_set/test_task.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1573 2022-11-14 04:18:29.000000 vise-0.7.2/vise/tests/input_set/test_vasp_input_files.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1211 2022-10-21 08:43:44.000000 vise-0.7.2/vise/tests/input_set/test_vise_log.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1162 2021-03-02 02:37:28.000000 vise-0.7.2/vise/tests/input_set/test_xc.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4762 2022-11-06 00:50:42.000000 vise-0.7.2/vise/tests/test_defaults.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1784 2022-10-21 08:06:31.000000 vise-0.7.2/vise/tests/test_user_settings.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.891091 vise-0.7.2/vise/tests/util/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/util/__init__.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.892282 vise-0.7.2/vise/tests/util/phonopy/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/util/phonopy/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     3100 2021-08-06 10:08:41.000000 vise-0.7.2/vise/tests/util/phonopy/test_phonopy_input.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1499 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/util/test_bravais_lattice.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2441 2021-03-05 09:50:13.000000 vise-0.7.2/vise/tests/util/test_centering.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4437 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/util/test_file_transfer.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      217 2020-08-02 02:24:25.000000 vise-0.7.2/vise/tests/util/test_logger.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      511 2020-05-15 22:51:22.000000 vise-0.7.2/vise/tests/util/test_matplotlib.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1500 2022-09-28 23:59:57.000000 vise-0.7.2/vise/tests/util/test_mix_in.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      232 2021-04-18 02:48:05.000000 vise-0.7.2/vise/tests/util/test_string.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     9778 2021-07-31 08:14:24.000000 vise-0.7.2/vise/tests/util/test_structure_symmetrizer.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      471 2021-08-01 00:43:34.000000 vise-0.7.2/vise/tests/util/test_valence_orbitals_from_potcar.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2143 2022-11-15 04:24:17.000000 vise-0.7.2/vise/user_settings.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.930286 vise-0.7.2/vise/util/
+-rw-r--r--   0 kumagai    (501) staff       (20)     3450 2021-09-15 23:40:59.000000 vise-0.7.2/vise/util/Hermann-Mauguin.yaml
+-rw-r--r--   0 kumagai    (501) staff       (20)        0 2020-05-15 22:51:22.000000 vise-0.7.2/vise/util/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     6893 2023-03-07 23:24:41.000000 vise-0.7.2/vise/util/bravais_lattice.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1786 2020-05-14 03:15:55.000000 vise-0.7.2/vise/util/centering.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      304 2020-11-12 05:19:29.000000 vise-0.7.2/vise/util/dash_helper.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      788 2021-05-30 03:06:06.000000 vise-0.7.2/vise/util/enum.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2746 2020-11-30 22:31:41.000000 vise-0.7.2/vise/util/file_transfer.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     1234 2021-05-01 05:11:26.000000 vise-0.7.2/vise/util/logger.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      802 2020-05-15 22:51:22.000000 vise-0.7.2/vise/util/matplotlib.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2752 2022-09-30 04:31:19.000000 vise-0.7.2/vise/util/mix_in.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.931802 vise-0.7.2/vise/util/phonopy/
+-rw-r--r--   0 kumagai    (501) staff       (20)       96 2020-05-15 22:51:22.000000 vise-0.7.2/vise/util/phonopy/__init__.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     4058 2022-09-06 01:13:47.000000 vise-0.7.2/vise/util/phonopy/phonopy_input.py
+-rw-r--r--   0 kumagai    (501) staff       (20)     2043 2021-08-11 05:37:35.000000 vise-0.7.2/vise/util/plotly_util.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      986 2022-07-29 03:01:33.000000 vise-0.7.2/vise/util/str_related_tools.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      786 2021-04-20 00:50:10.000000 vise-0.7.2/vise/util/string.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      486 2021-03-05 09:50:13.000000 vise-0.7.2/vise/util/structure_handler.py
+-rw-r--r--   0 kumagai    (501) staff       (20)    13330 2022-11-14 04:29:55.000000 vise-0.7.2/vise/util/structure_symmetrizer.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      229 2021-05-02 02:13:00.000000 vise-0.7.2/vise/util/typing.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      226 2021-07-05 05:51:09.000000 vise-0.7.2/vise/util/unit_conversion.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      419 2021-07-05 06:55:26.000000 vise-0.7.2/vise/util/valence_orbitals_from_potcar.py
+-rw-r--r--   0 kumagai    (501) staff       (20)      117 2023-05-10 02:25:33.000000 vise-0.7.2/vise/version.py
+drwxr-xr-x   0 kumagai    (501) staff       (20)        0 2023-05-10 02:36:57.707040 vise-0.7.2/vise.egg-info/
+-rw-r--r--   0 kumagai    (501) staff       (20)     4389 2023-05-10 02:36:57.000000 vise-0.7.2/vise.egg-info/PKG-INFO
+-rw-r--r--   0 kumagai    (501) staff       (20)     5313 2023-05-10 02:36:57.000000 vise-0.7.2/vise.egg-info/SOURCES.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        1 2023-05-10 02:36:57.000000 vise-0.7.2/vise.egg-info/dependency_links.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)       81 2023-05-10 02:36:57.000000 vise-0.7.2/vise.egg-info/entry_points.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)      152 2023-05-10 02:36:57.000000 vise-0.7.2/vise.egg-info/requires.txt
+-rw-r--r--   0 kumagai    (501) staff       (20)        5 2023-05-10 02:36:57.000000 vise-0.7.2/vise.egg-info/top_level.txt
```

### Comparing `vise-0.7.1/PKG-INFO` & `vise-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vise
-Version: 0.7.1
+Version: 0.7.2
 Summary: Package for handling io of vasp package in kumagai group at IMR, Tohoku university
 Home-page: https://github.com/kumagai-group/vise
 Author: Yu Kumagai
 Author-email: yukumagai@tohoku.ac.jp
 License: MIT license
 Description: ![PyPI - License](https://img.shields.io/pypi/l/vise?color=blue)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vise)
```

### Comparing `vise-0.7.1/README.md` & `vise-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/setup.py` & `vise-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/atom_grouping_type.py` & `vise-0.7.2/vise/analyzer/atom_grouping_type.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/band_edge_properties.py` & `vise-0.7.2/vise/analyzer/band_edge_properties.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/dielectric_function.py` & `vise-0.7.2/vise/analyzer/dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/dielectric_function_data/GaAs.csv` & `vise-0.7.2/vise/analyzer/dielectric_function_data/GaAs.csv`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/dielectric_function_data/Si.csv` & `vise-0.7.2/vise/analyzer/dielectric_function_data/Si.csv`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/dielectric_function_data/exp_dielectric_func.py` & `vise-0.7.2/vise/analyzer/dielectric_function_data/exp_dielectric_func.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/dos_data.py` & `vise-0.7.2/vise/analyzer/dos_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/effective_mass.py` & `vise-0.7.2/vise/analyzer/effective_mass.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/plot_band.py` & `vise-0.7.2/vise/analyzer/plot_band.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/plot_band_dos.py` & `vise-0.7.2/vise/analyzer/plot_band_dos.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/plot_brillouin_zone.py` & `vise-0.7.2/vise/analyzer/plot_brillouin_zone.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/plot_diele_func_data.py` & `vise-0.7.2/vise/analyzer/plot_diele_func_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/plot_dos.py` & `vise-0.7.2/vise/analyzer/plot_dos.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vasp/band_edge_properties.py` & `vise-0.7.2/vise/analyzer/vasp/band_edge_properties.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vasp/dos_data.py` & `vise-0.7.2/vise/analyzer/vasp/dos_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vasp/handle_volumetric_data.py` & `vise-0.7.2/vise/analyzer/vasp/handle_volumetric_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vasp/make_diele_func.py` & `vise-0.7.2/vise/analyzer/vasp/make_diele_func.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vasp/make_effective_mass.py` & `vise-0.7.2/vise/analyzer/vasp/make_effective_mass.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vasp/make_irreps.py` & `vise-0.7.2/vise/analyzer/vasp/make_irreps.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vasp/plot_band.py` & `vise-0.7.2/vise/analyzer/vasp/plot_band.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vesta/element_colors.py` & `vise-0.7.2/vise/analyzer/vesta/element_colors.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/analyzer/vesta/vesta_file.py` & `vise-0.7.2/vise/analyzer/vesta/vesta_file.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/atom_energies/atom_magnetization_hund.yaml` & `vise-0.7.2/vise/atom_energies/atom_magnetization_hund.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/atom_energies/get_energy.py` & `vise-0.7.2/vise/atom_energies/get_energy.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/atom_energies/make_atom_vasp_set.py` & `vise-0.7.2/vise/atom_energies/make_atom_vasp_set.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/atom_energies/mp_atom_energy.yaml` & `vise-0.7.2/vise/atom_energies/mp_atom_energy.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/atom_energies/mp_atom_mag.yaml` & `vise-0.7.2/vise/atom_energies/mp_atom_mag.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/cli/main.py` & `vise-0.7.2/vise/cli/main.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/cli/main_functions.py` & `vise-0.7.2/vise/cli/main_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,27 +148,28 @@
     def __init__(self, args: Namespace):
         self.args = args
         if args.prev_dir:
             self.args.prev_dir = args.prev_dir.absolute()
         if args.poscar:
             self.args.poscar = args.poscar.absolute()
 
-        try:
-            self._prior_info = PriorInfo.load_yaml()
-        except FileNotFoundError:
-            self._prior_info = PriorInfo()
-        self.task = Task.cluster_opt if self._prior_info.is_cluster \
-            else args.task
-
         for _dir in [d.absolute() for d in args.dirs]:
             if _dir.is_file():
                 logger.info(f"{_dir} is a file, so skipped.")
                 continue
 
             os.chdir(_dir)
+            logger.info(f"Creating VASP input set in {_dir}...")
+            try:
+                self._prior_info = PriorInfo.load_yaml()
+            except FileNotFoundError:
+                self._prior_info = PriorInfo()
+            self.task = Task.cluster_opt if self._prior_info.is_cluster \
+                else args.task
+
             options = CategorizedInputOptions(
                 structure=self._structure(),
                 task=self.task,
                 xc=args.xc,
                 kpt_density=args.kpt_density,
                 overridden_potcar=self._overridden_potcar(),
                 **self._option_kwargs())
```

### Comparing `vise-0.7.1/vise/cli/main_tools.py` & `vise-0.7.2/vise/cli/main_tools.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/cli/main_util.py` & `vise-0.7.2/vise/cli/main_util.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/cli/main_util_functions.py` & `vise-0.7.2/vise/cli/main_util_functions.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/defaults.py` & `vise-0.7.2/vise/defaults.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/datasets/dataset_util.py` & `vise-0.7.2/vise/input_set/datasets/dataset_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 unoccupied_bands = loadfn(Path(__file__).parent / "unoccupied_bands.yaml")
 
 # This incar_flags should be OrderedDict, but from python 3.6, dict uses
 # order-preserving semantics. Besides, it does not affect vasp result.
 incar_categories: Dict[str, Any] = \
     dict(loadfn(Path(__file__).parent / "incar_flags.yaml"))
 tag_set = set(tuple(tags) for tags in incar_categories)
-incar_categories["others"] = set(incar_params.keys()) - tag_set
+incar_categories["others"] = list(set(incar_params.keys()) - tag_set)
+all_incar_flags: List[str] = sum(incar_categories.values(), [])
 
 
 def has_f_elements(symbol_list: List[str]):
     return any([Element(el).Z > 56 for el in symbol_list])
 
 
 class LDAU:
```

### Comparing `vise-0.7.1/vise/input_set/datasets/incar_flags.yaml` & `vise-0.7.2/vise/input_set/datasets/incar_flags.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/datasets/kpar_set.yaml` & `vise-0.7.2/vise/input_set/datasets/kpar_set.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/datasets/potcar_set.py` & `vise-0.7.2/vise/input_set/datasets/potcar_set.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/datasets/potcar_set.yaml` & `vise-0.7.2/vise/input_set/datasets/potcar_set.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/datasets/u_parameter_set.yaml` & `vise-0.7.2/vise/input_set/datasets/u_parameter_set.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/datasets/unoccupied_bands.yaml` & `vise-0.7.2/vise/input_set/datasets/unoccupied_bands.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/fft_grids.py` & `vise-0.7.2/vise/input_set/fft_grids.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/incar.py` & `vise-0.7.2/vise/input_set/incar.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/incar_settings_generator.py` & `vise-0.7.2/vise/input_set/incar_settings_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/input_options.py` & `vise-0.7.2/vise/input_set/input_options.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/kpoints.py` & `vise-0.7.2/vise/input_set/kpoints.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/kpoints_mode.py` & `vise-0.7.2/vise/input_set/kpoints_mode.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/potcar_generator.py` & `vise-0.7.2/vise/input_set/potcar_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/prior_info.py` & `vise-0.7.2/vise/input_set/prior_info.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/structure_kpoints_generator.py` & `vise-0.7.2/vise/input_set/structure_kpoints_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/task.py` & `vise-0.7.2/vise/input_set/task.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/vasp_input_files.py` & `vise-0.7.2/vise/input_set/vasp_input_files.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/vise_log.py` & `vise-0.7.2/vise/input_set/vise_log.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/input_set/xc.py` & `vise-0.7.2/vise/input_set/xc.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_atom_grouping_type.py` & `vise-0.7.2/vise/tests/analyzer/test_atom_grouping_type.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_band_edge_properties.py` & `vise-0.7.2/vise/tests/analyzer/test_band_edge_properties.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_dielectric_function.py` & `vise-0.7.2/vise/tests/analyzer/test_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_dos_data.py` & `vise-0.7.2/vise/tests/analyzer/test_dos_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_effective_mass.py` & `vise-0.7.2/vise/tests/analyzer/test_effective_mass.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_plot_band.py` & `vise-0.7.2/vise/tests/analyzer/test_plot_band.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_plot_band_dos.py` & `vise-0.7.2/vise/tests/analyzer/test_plot_band_dos.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_plot_brillouin_zone.py` & `vise-0.7.2/vise/tests/analyzer/test_plot_brillouin_zone.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_plot_diele_func_data.py` & `vise-0.7.2/vise/tests/analyzer/test_plot_diele_func_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/test_plot_dos.py` & `vise-0.7.2/vise/tests/analyzer/test_plot_dos.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/vasp/test_band_edge_properties.py` & `vise-0.7.2/vise/tests/analyzer/vasp/test_band_edge_properties.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/vasp/test_dos_data.py` & `vise-0.7.2/vise/tests/analyzer/vasp/test_dos_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/vasp/test_handle_volumetric_data.py` & `vise-0.7.2/vise/tests/analyzer/vasp/test_handle_volumetric_data.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/vasp/test_make_diele_func.py` & `vise-0.7.2/vise/tests/analyzer/vasp/test_make_diele_func.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/vasp/test_make_effective_mass.py` & `vise-0.7.2/vise/tests/analyzer/vasp/test_make_effective_mass.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/vasp/test_make_irreps.py` & `vise-0.7.2/vise/tests/analyzer/vasp/test_make_irreps.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/analyzer/vasp/test_plot_band.py` & `vise-0.7.2/vise/tests/analyzer/vasp/test_plot_band.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/cli/test_main.py` & `vise-0.7.2/vise/tests/cli/test_main.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/cli/test_main_functions.py` & `vise-0.7.2/vise/tests/cli/test_main_functions.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/cli/test_main_tools.py` & `vise-0.7.2/vise/tests/cli/test_main_tools.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/cli/test_main_util.py` & `vise-0.7.2/vise/tests/cli/test_main_util.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/cli/test_main_util_functions.py` & `vise-0.7.2/vise/tests/cli/test_main_util_functions.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/conftest.py` & `vise-0.7.2/vise/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/helpers/assertion.py` & `vise-0.7.2/vise/tests/helpers/assertion.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/helpers/test_assersion.py` & `vise-0.7.2/vise/tests/helpers/test_assersion.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/datasets/test_dataset_util.py` & `vise-0.7.2/vise/tests/input_set/datasets/test_dataset_util.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/datasets/test_potcar_set.py` & `vise-0.7.2/vise/tests/input_set/datasets/test_potcar_set.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_incar.py` & `vise-0.7.2/vise/tests/input_set/test_incar.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_incar_settings_generator.py` & `vise-0.7.2/vise/tests/input_set/test_incar_settings_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_input_options.py` & `vise-0.7.2/vise/tests/input_set/test_input_options.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_kpoints_mode.py` & `vise-0.7.2/vise/tests/input_set/test_kpoints_mode.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_potcar_generator.py` & `vise-0.7.2/vise/tests/input_set/test_potcar_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_prior_info.py` & `vise-0.7.2/vise/tests/input_set/test_prior_info.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_structure_kpoints_generator.py` & `vise-0.7.2/vise/tests/input_set/test_structure_kpoints_generator.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_task.py` & `vise-0.7.2/vise/tests/input_set/test_task.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_vasp_input_files.py` & `vise-0.7.2/vise/tests/input_set/test_vasp_input_files.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_vise_log.py` & `vise-0.7.2/vise/tests/input_set/test_vise_log.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/input_set/test_xc.py` & `vise-0.7.2/vise/tests/input_set/test_xc.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/test_defaults.py` & `vise-0.7.2/vise/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/test_user_settings.py` & `vise-0.7.2/vise/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/util/phonopy/test_phonopy_input.py` & `vise-0.7.2/vise/tests/util/phonopy/test_phonopy_input.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/util/test_bravais_lattice.py` & `vise-0.7.2/vise/tests/util/test_bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/util/test_centering.py` & `vise-0.7.2/vise/tests/util/test_centering.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/util/test_file_transfer.py` & `vise-0.7.2/vise/tests/util/test_file_transfer.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/util/test_mix_in.py` & `vise-0.7.2/vise/tests/util/test_mix_in.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/tests/util/test_structure_symmetrizer.py` & `vise-0.7.2/vise/tests/util/test_structure_symmetrizer.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/user_settings.py` & `vise-0.7.2/vise/user_settings.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/Hermann-Mauguin.yaml` & `vise-0.7.2/vise/util/Hermann-Mauguin.yaml`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/bravais_lattice.py` & `vise-0.7.2/vise/util/bravais_lattice.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/centering.py` & `vise-0.7.2/vise/util/centering.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/enum.py` & `vise-0.7.2/vise/util/enum.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/file_transfer.py` & `vise-0.7.2/vise/util/file_transfer.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/logger.py` & `vise-0.7.2/vise/util/logger.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/matplotlib.py` & `vise-0.7.2/vise/util/matplotlib.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/mix_in.py` & `vise-0.7.2/vise/util/mix_in.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/phonopy/phonopy_input.py` & `vise-0.7.2/vise/util/phonopy/phonopy_input.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/plotly_util.py` & `vise-0.7.2/vise/util/plotly_util.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/str_related_tools.py` & `vise-0.7.2/vise/util/str_related_tools.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/string.py` & `vise-0.7.2/vise/util/string.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise/util/structure_symmetrizer.py` & `vise-0.7.2/vise/util/structure_symmetrizer.py`

 * *Files identical despite different names*

### Comparing `vise-0.7.1/vise.egg-info/PKG-INFO` & `vise-0.7.2/vise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vise
-Version: 0.7.1
+Version: 0.7.2
 Summary: Package for handling io of vasp package in kumagai group at IMR, Tohoku university
 Home-page: https://github.com/kumagai-group/vise
 Author: Yu Kumagai
 Author-email: yukumagai@tohoku.ac.jp
 License: MIT license
 Description: ![PyPI - License](https://img.shields.io/pypi/l/vise?color=blue)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/vise)
```

### Comparing `vise-0.7.1/vise.egg-info/SOURCES.txt` & `vise-0.7.2/vise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

