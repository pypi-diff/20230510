# Comparing `tmp/esi_syncopy-2023.3.tar.gz` & `tmp/esi_syncopy-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi_syncopy-2023.3.tar", max compression
+gzip compressed data, was "esi_syncopy-2023.5.tar", max compression
```

## Comparing `esi_syncopy-2023.3.tar` & `esi_syncopy-2023.5.tar`

### file list

```diff
@@ -1,125 +1,128 @@
--rw-r--r--   0        0        0     1597 2023-04-05 11:26:16.656767 esi_syncopy-2023.3/LICENSE
--rw-r--r--   0        0        0     3566 2023-04-05 11:26:16.656767 esi_syncopy-2023.3/README.rst
--rw-r--r--   0        0        0     1365 2023-04-06 08:45:16.506910 esi_syncopy-2023.3/pyproject.toml
--rw-r--r--   0        0        0     6850 2023-04-05 23:03:37.371806 esi_syncopy-2023.3/syncopy/__init__.py
--rw-r--r--   0        0        0    17907 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/connectivity/AV_compRoutines.py
--rw-r--r--   0        0        0    22230 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/connectivity/ST_compRoutines.py
--rw-r--r--   0        0        0      252 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/connectivity/__init__.py
--rw-r--r--   0        0        0    28388 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/connectivity/connectivity_analysis.py
--rw-r--r--   0        0        0     6277 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/connectivity/csd.py
--rw-r--r--   0        0        0     2537 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/connectivity/granger.py
--rw-r--r--   0        0        0     7250 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/connectivity/wilson_sf.py
--rw-r--r--   0        0        0      859 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/datatype/__init__.py
--rw-r--r--   0        0        0    59351 2023-04-05 23:03:37.371806 esi_syncopy-2023.3/syncopy/datatype/base_data.py
--rw-r--r--   0        0        0    30728 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/datatype/continuous_data.py
--rw-r--r--   0        0        0    28178 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/datatype/discrete_data.py
--rw-r--r--   0        0        0    21790 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/datatype/methods/arithmetic.py
--rw-r--r--   0        0        0     2331 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/datatype/methods/copy.py
--rw-r--r--   0        0        0    14482 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/datatype/methods/definetrial.py
--rw-r--r--   0        0        0     8708 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/datatype/methods/redefinetrial.py
--rw-r--r--   0        0        0    20139 2023-04-05 23:03:37.371806 esi_syncopy-2023.3/syncopy/datatype/methods/selectdata.py
--rw-r--r--   0        0        0     7450 2023-04-05 11:26:16.676768 esi_syncopy-2023.3/syncopy/datatype/methods/show.py
--rw-r--r--   0        0        0    41610 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/datatype/selector.py
--rw-r--r--   0        0        0     3342 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/datatype/util.py
--rw-r--r--   0        0        0      591 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/io/__init__.py
--rw-r--r--   0        0        0    18316 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/io/load_ft.py
--rw-r--r--   0        0        0    11592 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/io/load_nwb.py
--rw-r--r--   0        0        0    13581 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/io/load_spy_container.py
--rw-r--r--   0        0        0    39102 2023-04-05 23:03:37.371806 esi_syncopy-2023.3/syncopy/io/load_tdt.py
--rw-r--r--   0        0        0    12147 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/io/save_spy_container.py
--rw-r--r--   0        0        0     8532 2023-04-06 08:45:16.506910 esi_syncopy-2023.3/syncopy/io/utils.py
--rw-r--r--   0        0        0      258 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/plotting/__init__.py
--rw-r--r--   0        0        0     5589 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/plotting/_helpers.py
--rw-r--r--   0        0        0     5239 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/plotting/_plotting.py
--rw-r--r--   0        0        0     2039 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/plotting/config.py
--rw-r--r--   0        0        0     5347 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/plotting/helpers.py
--rw-r--r--   0        0        0     9335 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/plotting/mp_plotting.py
--rw-r--r--   0        0        0    11023 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/plotting/sp_plotting.py
--rw-r--r--   0        0        0     2244 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/plotting/spy_plotting.py
--rw-r--r--   0        0        0      248 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/preproc/__init__.py
--rw-r--r--   0        0        0    29554 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/preproc/compRoutines.py
--rw-r--r--   0        0        0     6953 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/preproc/firws.py
--rw-r--r--   0        0        0    14478 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/preproc/preprocessing.py
--rw-r--r--   0        0        0     8623 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/preproc/resampledata.py
--rw-r--r--   0        0        0     3944 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/preproc/resampling.py
--rw-r--r--   0        0        0      647 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/__init__.py
--rw-r--r--   0        0        0    51088 2023-04-05 23:03:37.371806 esi_syncopy-2023.3/syncopy/shared/computational_routine.py
--rw-r--r--   0        0        0     1826 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/const_def.py
--rw-r--r--   0        0        0     1674 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/dask_helpers.py
--rw-r--r--   0        0        0    16260 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/errors.py
--rw-r--r--   0        0        0      739 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/filetypes.py
--rw-r--r--   0        0        0    14519 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/input_processors.py
--rw-r--r--   0        0        0    38857 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/kwarg_decorators.py
--rw-r--r--   0        0        0     5905 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/latency.py
--rw-r--r--   0        0        0     8819 2023-04-06 08:45:16.506910 esi_syncopy-2023.3/syncopy/shared/log.py
--rw-r--r--   0        0        0    13913 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/metadata.py
--rw-r--r--   0        0        0    30214 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/parsers.py
--rw-r--r--   0        0        0     1742 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/queries.py
--rw-r--r--   0        0        0    12045 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/shared/tools.py
--rw-r--r--   0        0        0      829 2023-04-05 13:30:10.091089 esi_syncopy-2023.3/syncopy/specest/README.md
--rw-r--r--   0        0        0      254 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/__init__.py
--rw-r--r--   0        0        0     1078 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/_norm_spec.py
--rw-r--r--   0        0        0    44187 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/compRoutines.py
--rw-r--r--   0        0        0     9165 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/fooofspy.py
--rw-r--r--   0        0        0    45570 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/freqanalysis.py
--rw-r--r--   0        0        0     4694 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/mtmconvol.py
--rw-r--r--   0        0        0     4446 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/mtmfft.py
--rw-r--r--   0        0        0     5550 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/stft.py
--rw-r--r--   0        0        0    13340 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/superlet.py
--rw-r--r--   0        0        0     3655 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/wavelet.py
--rw-r--r--   0        0        0      129 2023-04-05 11:26:16.680768 esi_syncopy-2023.3/syncopy/specest/wavelets/__init__.py
--rw-r--r--   0        0        0    19699 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/specest/wavelets/transform.py
--rw-r--r--   0        0        0    10511 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/specest/wavelets/wavelets.py
--rw-r--r--   0        0        0      443 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/statistics/__init__.py
--rw-r--r--   0        0        0    12921 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/statistics/compRoutines.py
--rw-r--r--   0        0        0     6788 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/statistics/jackknifing.py
--rw-r--r--   0        0        0     7166 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/statistics/psth.py
--rw-r--r--   0        0        0     8734 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/statistics/spike_psth.py
--rw-r--r--   0        0        0    17812 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/statistics/summary_stats.py
--rw-r--r--   0        0        0     9407 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/statistics/timelockanalysis.py
--rw-r--r--   0        0        0      958 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/README.md
--rw-r--r--   0        0        0        0 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/backend/__init__.py
--rwxr-xr-x   0        0        0     1796 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/backend/run_tests.sh
--rw-r--r--   0        0        0     9750 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/backend/test_conn.py
--rw-r--r--   0        0        0     9950 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/backend/test_fooofspy.py
--rw-r--r--   0        0        0     4377 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/backend/test_resampling.py
--rw-r--r--   0        0        0    14593 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/backend/test_timefreq.py
--rw-r--r--   0        0        0     2708 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/conftest.py
--rw-r--r--   0        0        0     3975 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/helpers.py
--rw-r--r--   0        0        0     2037 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/local_spy.py
--rw-r--r--   0        0        0    11500 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/misc.py
--rwxr-xr-x   0        0        0      195 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/no_slurm.sh
--rw-r--r--   0        0        0      646 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/run_tests.cmd
--rwxr-xr-x   0        0        0     2530 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/run_tests.sh
--rw-r--r--   0        0        0    14267 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/synth_data.py
--rw-r--r--   0        0        0    13196 2023-04-05 23:03:37.371806 esi_syncopy-2023.3/syncopy/tests/test_attach_dataset.py
--rw-r--r--   0        0        0    17727 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_basedata.py
--rw-r--r--   0        0        0     5637 2023-04-05 23:03:37.371806 esi_syncopy-2023.3/syncopy/tests/test_cfg.py
--rw-r--r--   0        0        0    23769 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_computationalroutine.py
--rw-r--r--   0        0        0    35539 2023-04-05 23:03:37.371806 esi_syncopy-2023.3/syncopy/tests/test_connectivity.py
--rw-r--r--   0        0        0    34902 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_continuousdata.py
--rw-r--r--   0        0        0      958 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_datatype_util.py
--rw-r--r--   0        0        0     9276 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_decorators.py
--rw-r--r--   0        0        0    25596 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_discretedata.py
--rw-r--r--   0        0        0     2959 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_info.py
--rw-r--r--   0        0        0     5131 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_logging.py
--rw-r--r--   0        0        0    21863 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_metadata.py
--rw-r--r--   0        0        0     3611 2023-04-06 08:45:16.506910 esi_syncopy-2023.3/syncopy/tests/test_packagesetup.py
--rwxr-xr-x   0        0        0    13207 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_parsers.py
--rw-r--r--   0        0        0    14282 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_plotting.py
--rw-r--r--   0        0        0    20034 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_preproc.py
--rw-r--r--   0        0        0    10961 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_redefinetrial.py
--rw-r--r--   0        0        0     8983 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_resampledata.py
--rw-r--r--   0        0        0    21742 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_selectdata.py
--rw-r--r--   0        0        0    67192 2023-04-05 11:26:16.684768 esi_syncopy-2023.3/syncopy/tests/test_specest.py
--rw-r--r--   0        0        0     9735 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_specest_fooof.py
--rw-r--r--   0        0        0    13851 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_spike_psth.py
--rw-r--r--   0        0        0    25769 2023-04-05 11:26:16.688768 esi_syncopy-2023.3/syncopy/tests/test_spyio.py
--rw-r--r--   0        0        0     3737 2023-04-05 11:26:16.688768 esi_syncopy-2023.3/syncopy/tests/test_spytools.py
--rw-r--r--   0        0        0    23373 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_statistics.py
--rw-r--r--   0        0        0     4692 2023-04-05 11:26:16.688768 esi_syncopy-2023.3/syncopy/tests/test_synth_data.py
--rw-r--r--   0        0        0     9213 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_timelockanalysis.py
--rw-r--r--   0        0        0     5112 2023-04-05 11:26:16.688768 esi_syncopy-2023.3/syncopy/tests/test_tools.py
--rw-r--r--   0        0        0    16832 2023-04-05 23:03:37.375806 esi_syncopy-2023.3/syncopy/tests/test_welch.py
--rw-r--r--   0        0        0     4805 1970-01-01 00:00:00.000000 esi_syncopy-2023.3/PKG-INFO
+-rw-r--r--   0        0        0     1597 2023-04-05 11:26:16.656767 esi_syncopy-2023.5/LICENSE
+-rw-r--r--   0        0        0     4297 2023-05-09 09:07:32.200585 esi_syncopy-2023.5/README.rst
+-rw-r--r--   0        0        0     1401 2023-05-09 09:07:32.204584 esi_syncopy-2023.5/pyproject.toml
+-rw-r--r--   0        0        0     6875 2023-05-09 09:07:32.204584 esi_syncopy-2023.5/syncopy/__init__.py
+-rw-r--r--   0        0        0    17907 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/connectivity/AV_compRoutines.py
+-rw-r--r--   0        0        0    22230 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/connectivity/ST_compRoutines.py
+-rw-r--r--   0        0        0      252 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/connectivity/__init__.py
+-rw-r--r--   0        0        0    28157 2023-05-09 09:07:32.204584 esi_syncopy-2023.5/syncopy/connectivity/connectivity_analysis.py
+-rw-r--r--   0        0        0     6277 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/connectivity/csd.py
+-rw-r--r--   0        0        0     2537 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/connectivity/granger.py
+-rw-r--r--   0        0        0     7250 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/connectivity/wilson_sf.py
+-rw-r--r--   0        0        0      859 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/datatype/__init__.py
+-rw-r--r--   0        0        0    59490 2023-05-09 09:07:32.204584 esi_syncopy-2023.5/syncopy/datatype/base_data.py
+-rw-r--r--   0        0        0    29559 2023-05-09 09:07:32.204584 esi_syncopy-2023.5/syncopy/datatype/continuous_data.py
+-rw-r--r--   0        0        0    26600 2023-05-09 09:07:32.204584 esi_syncopy-2023.5/syncopy/datatype/discrete_data.py
+-rw-r--r--   0        0        0    21746 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/datatype/methods/arithmetic.py
+-rw-r--r--   0        0        0     2331 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/datatype/methods/copy.py
+-rw-r--r--   0        0        0    14320 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/datatype/methods/definetrial.py
+-rw-r--r--   0        0        0     8708 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/datatype/methods/redefinetrial.py
+-rw-r--r--   0        0        0    20133 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/datatype/methods/selectdata.py
+-rw-r--r--   0        0        0     7450 2023-04-05 11:26:16.676768 esi_syncopy-2023.5/syncopy/datatype/methods/show.py
+-rw-r--r--   0        0        0    42546 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/datatype/selector.py
+-rw-r--r--   0        0        0     5015 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/datatype/util.py
+-rw-r--r--   0        0        0      591 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/io/__init__.py
+-rw-r--r--   0        0        0    18316 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/io/load_ft.py
+-rw-r--r--   0        0        0    11592 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/io/load_nwb.py
+-rw-r--r--   0        0        0    13581 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/io/load_spy_container.py
+-rw-r--r--   0        0        0    39102 2023-04-05 23:03:37.371806 esi_syncopy-2023.5/syncopy/io/load_tdt.py
+-rw-r--r--   0        0        0    12487 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/io/save_spy_container.py
+-rw-r--r--   0        0        0     8532 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/io/utils.py
+-rw-r--r--   0        0        0      258 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/plotting/__init__.py
+-rw-r--r--   0        0        0     5598 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/plotting/_helpers.py
+-rw-r--r--   0        0        0     5239 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/plotting/_plotting.py
+-rw-r--r--   0        0        0     2039 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/plotting/config.py
+-rw-r--r--   0        0        0     5346 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/plotting/helpers.py
+-rw-r--r--   0        0        0     9335 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/plotting/mp_plotting.py
+-rw-r--r--   0        0        0    11023 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/plotting/sp_plotting.py
+-rw-r--r--   0        0        0     2244 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/plotting/spy_plotting.py
+-rw-r--r--   0        0        0      248 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/preproc/__init__.py
+-rw-r--r--   0        0        0    30638 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/preproc/compRoutines.py
+-rw-r--r--   0        0        0     7086 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/preproc/firws.py
+-rw-r--r--   0        0        0    14915 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/preproc/preprocessing.py
+-rw-r--r--   0        0        0     8363 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/preproc/resampledata.py
+-rw-r--r--   0        0        0     3944 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/preproc/resampling.py
+-rw-r--r--   0        0        0      647 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/__init__.py
+-rw-r--r--   0        0        0    51088 2023-04-05 23:03:37.371806 esi_syncopy-2023.5/syncopy/shared/computational_routine.py
+-rw-r--r--   0        0        0     1826 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/const_def.py
+-rw-r--r--   0        0        0     1674 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/dask_helpers.py
+-rw-r--r--   0        0        0    16260 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/errors.py
+-rw-r--r--   0        0        0      739 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/filetypes.py
+-rw-r--r--   0        0        0    14519 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/input_processors.py
+-rw-r--r--   0        0        0    38882 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/shared/kwarg_decorators.py
+-rw-r--r--   0        0        0     5905 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/latency.py
+-rw-r--r--   0        0        0     9274 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/shared/log.py
+-rw-r--r--   0        0        0    13913 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/metadata.py
+-rw-r--r--   0        0        0    30214 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/parsers.py
+-rw-r--r--   0        0        0     1742 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/queries.py
+-rw-r--r--   0        0        0    12045 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/shared/tools.py
+-rw-r--r--   0        0        0      829 2023-04-05 13:30:10.091089 esi_syncopy-2023.5/syncopy/specest/README.md
+-rw-r--r--   0        0        0      254 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/__init__.py
+-rw-r--r--   0        0        0     1078 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/_norm_spec.py
+-rw-r--r--   0        0        0    44187 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/compRoutines.py
+-rw-r--r--   0        0        0     9165 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/fooofspy.py
+-rw-r--r--   0        0        0    45570 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/freqanalysis.py
+-rw-r--r--   0        0        0     4694 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/mtmconvol.py
+-rw-r--r--   0        0        0     4446 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/mtmfft.py
+-rw-r--r--   0        0        0     5550 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/stft.py
+-rw-r--r--   0        0        0    13340 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/superlet.py
+-rw-r--r--   0        0        0     3655 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/wavelet.py
+-rw-r--r--   0        0        0      129 2023-04-05 11:26:16.680768 esi_syncopy-2023.5/syncopy/specest/wavelets/__init__.py
+-rw-r--r--   0        0        0    19699 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/specest/wavelets/transform.py
+-rw-r--r--   0        0        0    10511 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/specest/wavelets/wavelets.py
+-rw-r--r--   0        0        0      443 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/statistics/__init__.py
+-rw-r--r--   0        0        0    12921 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/statistics/compRoutines.py
+-rw-r--r--   0        0        0     6788 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/statistics/jackknifing.py
+-rw-r--r--   0        0        0     7166 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/statistics/psth.py
+-rw-r--r--   0        0        0     8734 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/statistics/spike_psth.py
+-rw-r--r--   0        0        0    17812 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/statistics/summary_stats.py
+-rw-r--r--   0        0        0     9407 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/statistics/timelockanalysis.py
+-rw-r--r--   0        0        0      147 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/synthdata/__init__.py
+-rw-r--r--   0        0        0     9539 2023-05-10 08:48:46.210434 esi_syncopy-2023.5/syncopy/synthdata/analog.py
+-rw-r--r--   0        0        0     3688 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/synthdata/spikes.py
+-rw-r--r--   0        0        0     3844 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/synthdata/utils.py
+-rw-r--r--   0        0        0      958 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/README.md
+-rw-r--r--   0        0        0        0 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/backend/__init__.py
+-rwxr-xr-x   0        0        0     1796 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/backend/run_tests.sh
+-rw-r--r--   0        0        0     9769 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/tests/backend/test_conn.py
+-rw-r--r--   0        0        0     9943 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/tests/backend/test_fooofspy.py
+-rw-r--r--   0        0        0     4377 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/backend/test_resampling.py
+-rw-r--r--   0        0        0    14593 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/backend/test_timefreq.py
+-rw-r--r--   0        0        0     2708 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/conftest.py
+-rw-r--r--   0        0        0     3975 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/helpers.py
+-rw-r--r--   0        0        0     1810 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/tests/local_spy.py
+-rw-r--r--   0        0        0    11500 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/misc.py
+-rwxr-xr-x   0        0        0      195 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/no_slurm.sh
+-rw-r--r--   0        0        0      646 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/run_tests.cmd
+-rwxr-xr-x   0        0        0     2530 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/run_tests.sh
+-rw-r--r--   0        0        0    13196 2023-04-05 23:03:37.371806 esi_syncopy-2023.5/syncopy/tests/test_attach_dataset.py
+-rw-r--r--   0        0        0    17727 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/test_basedata.py
+-rw-r--r--   0        0        0     5625 2023-05-09 11:00:13.325129 esi_syncopy-2023.5/syncopy/tests/test_cfg.py
+-rw-r--r--   0        0        0    23813 2023-05-09 09:07:32.208585 esi_syncopy-2023.5/syncopy/tests/test_computationalroutine.py
+-rw-r--r--   0        0        0    35654 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/tests/test_connectivity.py
+-rw-r--r--   0        0        0    35030 2023-05-09 09:07:32.212585 esi_syncopy-2023.5/syncopy/tests/test_continuousdata.py
+-rw-r--r--   0        0        0      958 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/test_datatype_util.py
+-rw-r--r--   0        0        0     9059 2023-05-09 09:07:32.212585 esi_syncopy-2023.5/syncopy/tests/test_decorators.py
+-rw-r--r--   0        0        0    25596 2023-04-05 23:03:37.375806 esi_syncopy-2023.5/syncopy/tests/test_discretedata.py
+-rw-r--r--   0        0        0     2959 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/test_info.py
+-rw-r--r--   0        0        0     5131 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/test_logging.py
+-rw-r--r--   0        0        0    21856 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/tests/test_metadata.py
+-rw-r--r--   0        0        0     3611 2023-05-09 09:07:32.212585 esi_syncopy-2023.5/syncopy/tests/test_packagesetup.py
+-rwxr-xr-x   0        0        0    13207 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/test_parsers.py
+-rw-r--r--   0        0        0    14243 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/tests/test_plotting.py
+-rw-r--r--   0        0        0    23494 2023-05-09 11:00:13.325129 esi_syncopy-2023.5/syncopy/tests/test_preproc.py
+-rw-r--r--   0        0        0    10965 2023-05-09 09:07:32.212585 esi_syncopy-2023.5/syncopy/tests/test_redefinetrial.py
+-rw-r--r--   0        0        0     8973 2023-05-09 11:00:13.325129 esi_syncopy-2023.5/syncopy/tests/test_resampledata.py
+-rw-r--r--   0        0        0    22068 2023-05-09 09:07:32.212585 esi_syncopy-2023.5/syncopy/tests/test_selectdata.py
+-rw-r--r--   0        0        0    67192 2023-04-05 11:26:16.684768 esi_syncopy-2023.5/syncopy/tests/test_specest.py
+-rw-r--r--   0        0        0     9735 2023-04-05 23:03:37.375806 esi_syncopy-2023.5/syncopy/tests/test_specest_fooof.py
+-rw-r--r--   0        0        0    13844 2023-05-09 09:07:32.212585 esi_syncopy-2023.5/syncopy/tests/test_spike_psth.py
+-rw-r--r--   0        0        0    25769 2023-04-05 11:26:16.688768 esi_syncopy-2023.5/syncopy/tests/test_spyio.py
+-rw-r--r--   0        0        0     3737 2023-04-05 11:26:16.688768 esi_syncopy-2023.5/syncopy/tests/test_spytools.py
+-rw-r--r--   0        0        0    23406 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/tests/test_statistics.py
+-rw-r--r--   0        0        0     5826 2023-05-09 17:45:16.934978 esi_syncopy-2023.5/syncopy/tests/test_synthdata.py
+-rw-r--r--   0        0        0     9202 2023-05-09 11:00:13.325129 esi_syncopy-2023.5/syncopy/tests/test_timelockanalysis.py
+-rw-r--r--   0        0        0     5112 2023-04-05 11:26:16.688768 esi_syncopy-2023.5/syncopy/tests/test_tools.py
+-rw-r--r--   0        0        0    16810 2023-05-09 09:07:32.212585 esi_syncopy-2023.5/syncopy/tests/test_welch.py
+-rw-r--r--   0        0        0     5536 1970-01-01 00:00:00.000000 esi_syncopy-2023.5/PKG-INFO
```

### Comparing `esi_syncopy-2023.3/LICENSE` & `esi_syncopy-2023.5/LICENSE`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/README.rst` & `esi_syncopy-2023.5/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -66,14 +66,28 @@
 Getting Started
 ===============
 Please visit our `online documentation <http://syncopy.org>`_.
 
 Developer Installation
 -----------------------
 
-To get the latest development version, please clone our GitHub repository:
+To get the latest development version, please clone our GitHub repository and change to the `dev` branch. We highly recommend to install into a new conda virtual environment, so that this development version does not interfere with your existing installation.
 
 .. code-block:: bash
 
    git clone https://github.com/esi-neuroscience/syncopy.git
    cd syncopy/
+   conda env create --name syncopy-dev --file syncopy.yml
+   conda activate syncopy-dev
    pip install -e .
+
+
+We recommend to verify your development installation by running the unit tests. You can skip the parallel tests to save some time, the tests should run in about 5 minutes then:
+
+
+.. code-block:: bash
+
+   python -m pytest -k "not parallel"
+
+
+You now have a verified developer installation of Syncopy. Please refert to our `contributing guide <https://github.com/esi-neuroscience/syncopy/blob/master/CONTRIBUTING.md>`_ if you want to contribute to Syncopy.
+
```

### Comparing `esi_syncopy-2023.3/pyproject.toml` & `esi_syncopy-2023.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "esi-syncopy"
 packages = [
     {include = "syncopy"}
 ]
-version = "2023.03"
+version = "2023.05"
 license = "BSD-3-Clause"
 readme="README.rst"
 homepage="https://syncopy.org"
 repository="https://github.com/esi-neuroscience/syncopy"
 include = [
     "LICENSE",
 ]
@@ -32,18 +32,19 @@
 natsort = "^8.1.0"
 psutil = ">=5.9"
 fooof = ">=1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 pytest = "^7.0"
-ipython = "^8.0"
+ipython = ">=8.10"
 pytest-cov = "^3.0.0"
-sphinx-book-theme = "^0.3.3"
+sphinx-book-theme = ">=1.0.1"
 sphinx-automodapi = "^0.14.1"
+pydata-sphinx-theme = ">=0.13.3"
 numpydoc = "^1.4.0"
 ipdb = "^0.13.9"
 memory-profiler = "^0.60.0"
 flake8 = "^3.9"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `esi_syncopy-2023.3/syncopy/__init__.py` & `esi_syncopy-2023.5/syncopy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 from .io import *
 from .datatype import *
 from .specest import *
 from .connectivity import *
 from .statistics import *
 from .plotting import *
 from .preproc import *
+from .synthdata import *
 
 from .datatype.util import setup_storage, get_dir_size
 storage_tmpdir_size_gb, storage_tmpdir_numfiles = setup_storage()  # Creates the storage dir if needed and computes size and number of files in there if any.
 spydir_size_gb, spydir_numfiles = get_dir_size(__spydir__, out="GB")
 
 from .shared.log import setup_logging
 __logdir__ = None  # Gets set in setup_logging() call below.
```

### Comparing `esi_syncopy-2023.3/syncopy/connectivity/AV_compRoutines.py` & `esi_syncopy-2023.5/syncopy/connectivity/AV_compRoutines.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/connectivity/ST_compRoutines.py` & `esi_syncopy-2023.5/syncopy/connectivity/ST_compRoutines.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/connectivity/connectivity_analysis.py` & `esi_syncopy-2023.5/syncopy/connectivity/connectivity_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,18 +268,14 @@
         SPYWarning(msg)
 
     # if a subset selection is present
     # get sampleinfo and check for equidistancy
     if data.selection is not None:
         sinfo = data.selection.trialdefinition[:, :2]
         # user picked discrete set of time points
-        if isinstance(data.selection.time[0], list):
-            lgl = "equidistant time points"
-            actual = "non-equidistant set of time points"
-            raise SPYValueError(legal=lgl, varname="select", actual=actual)
     else:
         sinfo = data.sampleinfo
     lenTrials = np.diff(sinfo).squeeze()
 
     # check padding
 
     if method == "corr" and pad != 'maxperlen':
```

### Comparing `esi_syncopy-2023.3/syncopy/connectivity/csd.py` & `esi_syncopy-2023.5/syncopy/connectivity/csd.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/connectivity/granger.py` & `esi_syncopy-2023.5/syncopy/connectivity/granger.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/connectivity/wilson_sf.py` & `esi_syncopy-2023.5/syncopy/connectivity/wilson_sf.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/datatype/__init__.py` & `esi_syncopy-2023.5/syncopy/datatype/__init__.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/datatype/base_data.py` & `esi_syncopy-2023.5/syncopy/datatype/base_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -987,19 +987,17 @@
             self._selector = None
         else:
             self._selector = Selector(self, select)
 
     @property
     def trialdefinition(self):
         """nTrials x >=3 :class:`numpy.ndarray` of [start, end, offset, trialinfo[:]]"""
-        return np.array(self._trialdefinition)
-
-    @trialdefinition.setter
-    def trialdefinition(self, trl):
-        _definetrial(self, trialdefinition=trl)
+        if self._trialdefinition is not None:
+            # to avoid hanging references
+            return self._trialdefinition.copy()
 
     @property
     def sampleinfo(self):
         """nTrials x 2 :class:`numpy.ndarray` of [start, end] sample indices"""
         if self._trialdefinition is not None:
             return self._trialdefinition[:, :2]
         else:
@@ -1008,14 +1006,20 @@
     @sampleinfo.setter
     def sampleinfo(self, sinfo):
         raise SPYError(
             "Cannot set sampleinfo. Use `BaseData.trialdefinition` instead."
         )
 
     @property
+    def trial_ids(self):
+        """Index list of trials"""
+        if self._trialdefinition is not None:
+            return self._trial_ids
+
+    @property
     def trialintervals(self):
         """nTrials x 2 :class:`numpy.ndarray` of [start, end] times in seconds """
         if self._trialdefinition is not None and self._samplerate is not None:
             # trial lengths in samples
             start_end = self.sampleinfo - self.sampleinfo[:, 0][:, None]
             start_end[:, 1] -= 1  # account for last time point
            # add offset and convert to seconds
@@ -1030,19 +1034,19 @@
         if self._trialdefinition is not None:
             return self._trialdefinition[:, 2]
         else:
             return None
 
     @property
     def trials(self):
-        """list-like array of trials"""
+        """list-like iterable of trials"""
 
         if self.sampleinfo is not None:
             trial_ids = list(range(self.sampleinfo.shape[0]))
-            # this is cheap as it just initializes a list-like object
+            # this is cheap as it just initializes an indexable generator
             # with no real data and/or computation!
             return TrialIndexer(self, trial_ids)
         else:
             return None
 
     @property
     def trialinfo(self):
```

### Comparing `esi_syncopy-2023.3/syncopy/datatype/continuous_data.py` & `esi_syncopy-2023.5/syncopy/datatype/continuous_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 import numpy as np
 from abc import ABC
 from collections.abc import Iterator
 
 # Local imports
 from .base_data import BaseData, FauxTrial, _definetrial
 from .methods.definetrial import definetrial
+from .base_data import BaseData
 from syncopy.shared.parsers import scalar_parser, array_parser
-from syncopy.shared.errors import SPYValueError, SPYWarning
+from syncopy.shared.errors import SPYValueError, log
 from syncopy.shared.tools import best_match
 from syncopy.plotting import sp_plotting, mp_plotting
+from .util import TimeIndexer
+
 
 
 __all__ = ["AnalogData", "SpectralData", "CrossSpectralData", "TimeLockData"]
 
 
 class ContinuousData(BaseData, ABC):
     """Abstract class for uniformly sampled data
@@ -81,15 +84,15 @@
         hdstr = "Syncopy {clname:s} object with fields\n\n"
         ppstr = hdstr.format(clname=self.__class__.__name__)
         maxKeyLength = max([len(k) for k in ppattrs])
         printString = "{0:>" + str(maxKeyLength + 5) + "} : {1:}\n"
         for attr in ppattrs:
             value = getattr(self, attr)
             if hasattr(value, 'shape') and attr == "data" and self.sampleinfo is not None:
-                tlen = np.unique([sinfo[1] - sinfo[0] for sinfo in self.sampleinfo])
+                tlen = np.unique(np.diff(self.sampleinfo))
                 if tlen.size == 1:
                     trlstr = "of length {} ".format(str(tlen[0]))
                 else:
                     trlstr = ""
                 dsize = np.prod(self.data.shape)*self.data.dtype.itemsize/1024**2
                 dunit = "MB"
                 if dsize > 1000:
@@ -148,45 +151,62 @@
             self._channel = None
             return
 
         if self.data is None:
             raise SPYValueError("Syncopy: Cannot assign `channels` without data. " +
                   "Please assign data first")
 
-        try:
-            array_parser(channel, varname="channel", ntype="str",
-                         dims=(self.data.shape[self.dimord.index("channel")],))
-        except Exception as exc:
-            raise exc
+        array_parser(channel, varname="channel", ntype="str",
+                     dims=(self.data.shape[self.dimord.index("channel")],))
 
         self._channel = np.array(channel)
 
     @property
     def samplerate(self):
         """float: sampling rate of uniformly sampled data in Hz"""
         return self._samplerate
 
     @samplerate.setter
     def samplerate(self, sr):
         if sr is None:
             self._samplerate = None
             return
 
-        try:
-            scalar_parser(sr, varname="samplerate", lims=[np.finfo('float').eps, np.inf])
-        except Exception as exc:
-            raise exc
+        scalar_parser(sr, varname="samplerate", lims=[np.finfo('float').eps, np.inf])
         self._samplerate = float(sr)
+        # we need a new TimeIndexer
+        if self.trialdefinition is not None:
+            self._time = TimeIndexer(self.trialdefinition,
+                                     self.samplerate,
+                                     list(self._trial_ids))
+
+    @BaseData.trialdefinition.setter
+    def trialdefinition(self, trldef):
+
+        # all-to-all trialdefinition
+        if trldef is None:
+            self._trialdefinition = np.array([[0, self.data.shape[self.dimord.index("time")], 0]])
+            self._trial_ids = [0]
+        else:
+            scount = self.data.shape[self.dimord.index("time")]
+            array_parser(trldef, varname="trialdefinition", dims=2)
+            array_parser(trldef[:, :2], varname="sampleinfo", hasnan=False,
+                         hasinf=False, ntype="int_like", lims=[0, scount])
+
+            self._trialdefinition = trldef.copy()
+            self._trial_ids = np.arange(self.sampleinfo.shape[0])
+            self._time = TimeIndexer(self.trialdefinition,
+                                     self.samplerate,
+                                     list(self._trial_ids))
 
     @property
     def time(self):
-        """list(float): trigger-relative time axes of each trial """
+        """indexable iterable of the time arrays"""
         if self.samplerate is not None and self.sampleinfo is not None:
-            return [(np.arange(0, stop - start) + self._t0[tk]) / self.samplerate \
-                    for tk, (start, stop) in enumerate(self.sampleinfo)]
+            return self._time
 
     # Helper function that grabs a single trial
     def _get_trial(self, trialno):
         idx = [slice(None)] * len(self.dimord)
         idx[self._stackingDim] = slice(int(self.sampleinfo[trialno, 0]), int(self.sampleinfo[trialno, 1]))
         return self._data[tuple(idx)]
 
@@ -229,26 +249,26 @@
         shp[self._stackingDim] = stop - start
         idx[self._stackingDim] = slice(start, stop)
 
         # process existing data selections
         if self.selection is not None:
 
             # time-selection is most delicate due to trial-offset
-            tsel = self.selection.time[self.selection.trial_ids.index(trialno)]
+            tsel = self.selection.time[trialno]
             if isinstance(tsel, slice):
                 if tsel.start is not None:
                     tstart = tsel.start
                 else:
                     tstart = 0
                 if tsel.stop is not None:
                     tstop = tsel.stop
                 else:
                     tstop = stop - start
 
-                # account for trial offsets an compute slicing index + shape
+                # account for trial offsets and compute slicing index + shape
                 start = start + tstart
                 stop = start + (tstop - tstart)
                 idx[self._stackingDim] = slice(start, stop)
                 shp[self._stackingDim] = stop - start
 
             else:
                 idx[self._stackingDim] = [tp + start for tp in tsel]
@@ -279,87 +299,33 @@
                     elif isinstance(sel, list):
                         shp[dimIdx] = len(sel)
                     else:
                         shp[dimIdx] = 1
 
         return FauxTrial(shp, tuple(idx), self.data.dtype, self.dimord)
 
-    # Helper function that extracts timing-related indices
-    def _get_time(self, trials, toi=None, toilim=None):
-        """
-        Get relative by-trial indices of time-selections
-        `toi` is legacy.. `toilim ` is used by selections via `latency`
-
-        Parameters
-        ----------
-        trials : list
-            List of trial-indices to perform selection on
-        toi : None or list
-            Time-points to be selected (in seconds) on a by-trial scale.
-        toilim : None or list
-            Time-window to be selected (in seconds) on a by-trial scale
-
-        Returns
-        -------
-        timing : list of lists
-            List of by-trial sample-indices corresponding to provided
-            time-selection. If both `toi` and `toilim` are `None`, `timing`
-            is a list of universal (i.e., ``slice(None)``) selectors.
-
-        Notes
-        -----
-        This class method is intended to be solely used by
-        :class:`syncopy.datatype.selector.Selector` objects and thus has purely
-        auxiliary character. Therefore, all input sanitization and error checking
-        is left to :class:`syncopy.datatype.selector.Selector` and not
-        performed here.
-
-        See also
-        --------
-        syncopy.datatype.selector.Selector : Syncopy data selectors
-        """
-        timing = []
-        if toilim is not None:
-            for trlno in trials:
-                _, selTime = best_match(self.time[trlno], toilim, span=True)
-                selTime = selTime.tolist()
-                if len(selTime) > 1:
-                    timing.append(slice(selTime[0], selTime[-1] + 1, 1))
-                else:
-                    timing.append(selTime)
-
-        elif toi is not None:
-            for trlno in trials:
-                _, selTime = best_match(self.time[trlno], toi)
-                selTime = selTime.tolist()
-                if len(selTime) > 1:
-                    timeSteps = np.diff(selTime)
-                    if timeSteps.min() == timeSteps.max() == 1:
-                        selTime = slice(selTime[0], selTime[-1] + 1, 1)
-                timing.append(selTime)
-
-        else:
-            timing = [slice(None)] * len(trials)
-
-        return timing
-
     # Make instantiation persistent in all subclasses
     def __init__(self, data=None, channel=None, samplerate=None, **kwargs):
 
         self._channel = None
         self._samplerate = None
         self._data = None
+        self._time = None
 
         self.samplerate = samplerate     # use setter for error-checking
 
         # Call initializer
         super().__init__(data=data, **kwargs)
 
-        # might be set from concatenation
-        if self.channel is None:
+        # catches channel propagation
+        # from concatenation of syncopy data objects
+        if self._channel is None:
+            self.channel = channel
+        # overwrites channels from concatenation if desired
+        elif channel is not None:
             self.channel = channel
 
         if self.data is not None:
 
             # In case of manual data allocation (reading routine would leave a
             # mark in `cfg`), fill in missing info
             if self.sampleinfo is None:
@@ -814,16 +780,16 @@
         simple structure:
                               [[0, nSamples, offset],
                               [nSamples, 2 * nSamples, offset],
                               [2 * nSamples, 3 * nSamples, offset],
                               ...]
         """
 
-        # first harness all parsers here
-        _definetrial(self, trialdefinition=trldef)
+        # we need parent setter for basic validation
+        ContinuousData.trialdefinition.fset(self, trldef)
 
         # now check for additional conditions
 
         # FIXME: not clear, is timelocked data to be expected
         # to have same offsets?!
         # if not np.unique(trldef[:, 2]).size == 1:
         #     lgl = "equal offsets for timelocked data"
@@ -833,15 +799,14 @@
         # diff-diff should give 0 -> same number of samples for each trial
         if not np.all(np.diff(trldef, axis=0, n=2) == 0):
             lgl = "all trials of same length for timelocked data"
             act = "unequal sized trials defined"
             raise SPYValueError(lgl, varname="trialdefinition", actual=act)
 
     # TODO - overload `time` property, as there is only one by definition!
-
     # implement plotting
     def singlepanelplot(self, shifted=True, **show_kwargs):
 
         figax = sp_plotting.plot_AnalogData(self, shifted, **show_kwargs)
         return figax
 
     def multipanelplot(self, **show_kwargs):
```

### Comparing `esi_syncopy-2023.3/syncopy/datatype/discrete_data.py` & `esi_syncopy-2023.5/syncopy/datatype/discrete_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,19 +136,43 @@
 
         try:
             scalar_parser(sr, varname="samplerate", lims=[1, np.inf])
         except Exception as exc:
             raise exc
         self._samplerate = sr
 
+    @BaseData.trialdefinition.setter
+    def trialdefinition(self, trldef):
+
+        if trldef is None:
+            sidx = self.dimord.index("sample")
+            self._trialdefinition = np.array([[np.nanmin(self.data[:, sidx]),
+                                               np.nanmax(self.data[:, sidx]), 0]])
+        else:
+            array_parser(trldef, varname="trialdefinition", dims=2)
+            array_parser(trldef[:, :2], varname="sampleinfo", hasnan=False,
+                         hasinf=False, ntype="int_like", lims=[0, np.inf])
+
+            self._trialdefinition = trldef.copy()
+
+            # Compute trial-IDs by matching data samples with provided trial-bounds
+            samples = self.data[:, self.dimord.index("sample")]
+            idx = np.searchsorted(samples, self.sampleinfo.ravel())
+            idx = idx.reshape(self.sampleinfo.shape)
+
+            self._trialslice = [slice(st,end) for st,end in idx]
+            self.trialid = np.full((samples.shape), -1, dtype=int)
+            for itrl, itrl_slice in enumerate(self._trialslice):
+                self.trialid[itrl_slice] = itrl
+
     @property
     def time(self):
         """list(float): trigger-relative time of each event """
         if self.samplerate is not None and self.sampleinfo is not None:
-            return [(trl[:,self.dimord.index("sample")] - self.sampleinfo[tk,0] + self._t0[tk]) / self.samplerate \
+            return [(trl[:,self.dimord.index("sample")] - self.sampleinfo[tk,0] + self.trialdefinition[tk, 2]) / self.samplerate \
                     for tk, trl in enumerate(self.trials)]
 
     @property
     def trialid(self):
         """:class:`numpy.ndarray` of trial id associated with the sample"""
         return self._trialid
 
@@ -173,15 +197,15 @@
             raise exc
         self._trialid = np.array(trlid, dtype=int)
 
     @property
     def trialtime(self):
         """list(:class:`numpy.ndarray`): trigger-relative sample times in s"""
         if self.samplerate is not None and self.sampleinfo is not None:
-            sample0 = self.sampleinfo[:, 0] - self._t0[:]
+            sample0 = self.sampleinfo[:, 0] - self._t0
             sample0 = np.append(sample0, np.nan)[self.trialid]
             return (self.data[:, self.dimord.index("sample")] - sample0) / self.samplerate
 
     # Helper function that grabs a single trial
     def _get_trial(self, trialno):
         return self._data[self._trialslice[trialno], :]
 
@@ -223,82 +247,14 @@
         else:
             idx[0] = trialIdx.tolist()
 
         shp = [len(idx[0]), nCol]
 
         return FauxTrial(shp, tuple(idx), self.data.dtype, self.dimord)
 
-    # Helper function that extracts by-trial timing-related indices
-    def _get_time(self, trials, toi=None, toilim=None):
-        """
-        Get relative by-trial indices of time-selections.
-
-        Parameters
-        ----------
-        trials : list
-            List of trial-indices to perform selection on.
-        toi : None or list
-            Time-points to be selected (in seconds) on a by-trial scale.
-        toilim : None or list
-            Time-window to be selected (in seconds) on a by-trial scale.
-
-        Returns
-        -------
-        timing : list of lists
-            List of by-trial sample-indices corresponding to provided
-            time-selection. If both `toi` and `toilim` are `None`, `timing`
-            is a list of universal (i.e., ``slice(None)``) selectors.
-
-        Notes
-        -----
-        This class method is intended to be solely used by
-        :class:`syncopy.datatype.selector.Selector` objects and thus has purely
-        auxiliary character. Therefore, all input sanitization and error checking
-        is left to :class:`syncopy.datatype.selector.Selector` and not
-        performed here.
-
-        See also
-        --------
-        syncopy.datatype.selector.Selector : Syncopy data selectors
-        """
-        timing = []
-        if toilim is not None:
-            allTrials = self.trialtime
-            for trlno in trials:
-                trlTime = allTrials[self._trialslice[trlno]]
-                _, selTime = best_match(trlTime, toilim, span=True)
-                selTime = selTime.tolist()
-                if len(selTime) > 1 and np.diff(trlTime).min() > 0:
-                    timing.append(slice(selTime[0], selTime[-1] + 1, 1))
-                else:
-                    timing.append(selTime)
-
-        elif toi is not None:
-            allTrials = self.trialtime
-            for trlno in trials:
-                trlTime = allTrials[self._trialslice[trlno]]
-                _, arrayIdx = best_match(trlTime, toi)
-                # squash duplicate values then readd
-                _, xdi = np.unique(trlTime[arrayIdx], return_index=True)
-                arrayIdx = arrayIdx[xdi] # we assume sorted data
-                selTime = []
-                for t in arrayIdx:
-                    selTime += np.where(trlTime[t] == trlTime)[0].tolist()
-                # convert to slice if possible
-                if len(selTime) > 1:
-                    timeSteps = np.diff(selTime)
-                    if timeSteps.min() == timeSteps.max() == 1:
-                        selTime = slice(selTime[0], selTime[-1] + 1, 1)
-                timing.append(selTime)
-
-        else:
-            timing = [slice(None)] * len(trials)
-
-        return timing
-
     def __init__(self, data=None, samplerate=None, trialid=None, **kwargs):
 
         # set as instance attribute to allow (un-)registering of additional datasets
         self._hdfFileDatasetProperties = BaseData._hdfFileDatasetProperties + ("data",)
 
         # Assign (default) values
         self._trialid = None
```

### Comparing `esi_syncopy-2023.3/syncopy/datatype/methods/arithmetic.py` & `esi_syncopy-2023.5/syncopy/datatype/methods/arithmetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 # Builtin/3rd party package imports
 import numpy as np
 import h5py
 
 # Local imports
 from syncopy import __acme__
-from .selectdata import _get_selection_size
 from syncopy.shared.parsers import data_parser
 from syncopy.shared.errors import SPYValueError, SPYTypeError, SPYWarning, SPYInfo
 from syncopy.shared.computational_routine import ComputationalRoutine
 from syncopy.shared.kwarg_decorators import process_io, detect_parallel_client
 
 if __acme__:
     import dask.distributed as dd
```

### Comparing `esi_syncopy-2023.3/syncopy/datatype/methods/copy.py` & `esi_syncopy-2023.5/syncopy/datatype/methods/copy.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/datatype/methods/definetrial.py` & `esi_syncopy-2023.5/syncopy/datatype/methods/definetrial.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Builtin/3rd party package imports
 import sys
 import numpy as np
 
 # Local imports
 from syncopy.shared.parsers import data_parser, array_parser, scalar_parser
 from syncopy.shared.errors import SPYTypeError, SPYValueError
+from ...datatype.util import TimeIndexer
 
 __all__ = ["definetrial"]
 
 
 def definetrial(obj, trialdefinition=None, pre=None, post=None, start=None,
                 trigger=None, stop=None, clip_edges=False):
     """(Re-)define trials of a Syncopy data object
@@ -70,44 +71,35 @@
 
     >>> # define whole recording as single trial
     >>> definetrial(obj, trialdefinition=None)
 
     """
 
     # Start by vetting input object
-    try:
-        data_parser(obj, varname="obj")
-    except Exception as exc:
-        raise exc
+    data_parser(obj, varname="obj")
     if obj.data is None:
         lgl = "non-empty Syncopy data object"
         act = "empty Syncopy data object"
         raise SPYValueError(legal=lgl, varname="obj", actual=act)
 
     # Check array/object holding trial specifications
     if trialdefinition is not None:
         if trialdefinition.__class__.__name__ == "EventData":
-            try:
-                data_parser(trialdefinition, varname="trialdefinition",
-                            writable=None, empty=False)
-            except Exception as exc:
-                raise exc
+            data_parser(trialdefinition, varname="trialdefinition",
+                        writable=None, empty=False)
             evt = True
         else:
             array_parser(trialdefinition, varname="trialdefinition", dims=2)
 
             if any(["ContinuousData" in str(base) for base in obj.__class__.__mro__]):
                 scount = obj.data.shape[obj.dimord.index("time")]
             else:
                 scount = np.inf
-            try:
-                array_parser(trialdefinition[:, :2], varname="sampleinfo", dims=(None, 2), hasnan=False,
+            array_parser(trialdefinition[:, :2], varname="sampleinfo", dims=(None, 2), hasnan=False,
                          hasinf=False, ntype="int_like", lims=[0, scount])
-            except Exception as exc:
-                raise exc
 
             trl = np.array(trialdefinition, dtype="float")
             ref = obj
             tgt = obj
             evt = False
     else:
         # Construct object-class-specific `trl` arrays treating data-set as single trial
@@ -321,15 +313,16 @@
     # all data genres
     if trl.shape[1] < 3:
         raise SPYValueError("array of shape (no. of trials, 3+)",
                             varname="trialdefinition",
                             actual="shape = {shp:s}".format(shp=str(trl.shape)))
 
     # Finally: assign `sampleinfo`, `t0` and `trialinfo` (and potentially `trialid`)
-    tgt._trialdefinition = trl
+    # use target class setter
+    tgt.trialdefinition = trl
 
     # In the discrete case, we have some additinal work to do
     if any(["DiscreteData" in str(base) for base in tgt.__class__.__mro__]):
 
         # Compute trial-IDs by matching data samples with provided trial-bounds
         samples = tgt.data[:, tgt.dimord.index("sample")]
         idx = np.searchsorted(samples, tgt.sampleinfo.ravel())
```

### Comparing `esi_syncopy-2023.3/syncopy/datatype/methods/redefinetrial.py` & `esi_syncopy-2023.5/syncopy/datatype/methods/redefinetrial.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/datatype/methods/selectdata.py` & `esi_syncopy-2023.5/syncopy/datatype/methods/selectdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import h5py
 
 # Local imports
 import syncopy as spy
 from syncopy.shared.tools import get_frontend_cfg, get_defaults
 from syncopy.shared.parsers import data_parser
-from syncopy.shared.errors import SPYValueError, SPYTypeError, SPYInfo, SPYWarning
+from syncopy.shared.errors import SPYValueError, SPYTypeError, SPYInfo, log
 from syncopy.shared.kwarg_decorators import unwrap_cfg, process_io, detect_parallel_client
 from syncopy.shared.computational_routine import ComputationalRoutine
 from syncopy.shared.latency import get_analysis_window, create_trial_selection
 
 __all__ = ["selectdata"]
 
 
@@ -317,14 +317,15 @@
     # first do a selection without latency as a possible subselection
     # of trials needs to be applied before the latency digesting functions
     # can be called (if the user by himself throws out non-fitting trials)
     selectDict.pop('latency')
 
     # Pass provided selections on to `Selector` class which performs error checking
     # this is an in-place selection!
+
     data.selection = selectDict
 
     # -- sort out trials if latency is set --
 
     if latency is not None:
         if not isinstance(latency, str) or latency != 'all':
             # sanity check done here, converts str arguments
```

### Comparing `esi_syncopy-2023.3/syncopy/datatype/methods/show.py` & `esi_syncopy-2023.5/syncopy/datatype/methods/show.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/datatype/selector.py` & `esi_syncopy-2023.5/syncopy/datatype/selector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Builtin/3rd party package imports
 from functools import reduce
 import numpy as np
+from numbers import Number
 
 # syncopy imports
 from syncopy.shared.parsers import array_parser, data_parser
 from syncopy.shared.errors import SPYTypeError, SPYValueError, SPYError
+from syncopy.shared.tools import best_match
 
 # local imports
 from .util import TrialIndexer
 
 
 class Selector:
     """
@@ -90,21 +92,15 @@
     size. To not overflow memory and slow down computations, neither `toi`
     nor `toilim` is checked for consistency with respect to `data.time`, i.e.,
     the code does not verify that min/max of `toi`/`toilim` are within the
     bounds of `data.time` for each selected trial.
 
     For objects that have a `time` property, a suitable new `trialdefinition`
     array (accessible via the identically named `Selector` class property)
-    is automatically constructed based on the provided selection. For unsorted
-    time-selections with or without repetitions, the `timepoints` property
-    encodes the timing of the selected (discrete) points. To permit this
-    functionality, the input object's samplerate is stored in the identically
-    named hidden attribute `_samplerate`. In addition, the hidden `_timeShuffle`
-    attribute is a binary flag encoding whether selected time-points are
-    unordered and/or contain repetitions (`Selector._timeShuffle = True`).
+    is automatically constructed based on the provided selection. 
 
     By default, each selection property tries to convert a user-provided
     selection to a contiguous slice-indexer so that simple NumPy array
     indexing can be used for best performance. However, after setting all
     selection indices appropriate for the input object, a consistency
     check is performed by :meth:`_make_consistent` to ensure that the
     calculated indices can actually be jointly used on a multi-dimensional
@@ -414,33 +410,25 @@
                         lgl = (
                             "`select: latency` selection with `latency[0]` < `latency[1]`"
                         )
                         act = "selection range from {} to {}".format(
                             timeSpec[0], timeSpec[1]
                         )
                         raise SPYValueError(legal=lgl, varname=vname, actual=act)
-            timing = data._get_time(self.trial_ids, toi=None, toilim=select.get("latency"))
-
-            # ---------------------------------------------------------------------------
-            # this is legacy, might be needed later if ppl really want to "time shuffle"
-            # to destroy any correlations and produce white noise from their data..
-            # .. which is questionable
-
-            # Determine, whether time-selection is unordered/contains repetitions
-            # and set `self._timeShuffle` accordingly
-            if timeSpec is not None:  # saves time for `timeSpec = None` "selections"
-                for tsel in timing:
-                    if isinstance(tsel, list) and len(tsel) > 1:
-                        if np.diff(tsel).min() <= 0:
-                            self._timeShuffle = True
-                            break
-            # ---------------------------------------------------------------------------
 
             # Assign timing selection and copy over samplerate from source object
-            self._time = timing
+            if any(["DiscreteData" in str(base) for base in data.__class__.__mro__]):
+                # special case DiscreteData: here we need an assignable property
+                # for `_make_consistent` so we unpack the Indexer right away
+                self._time = list(SelectionTimeIndexer(data, toilim=select.get("latency"),
+                                                       idx_list=self.trial_ids))
+
+            else:
+                self._time = SelectionTimeIndexer(data, toilim=select.get("latency"),
+                                                  idx_list=self.trial_ids)
             self._samplerate = data.samplerate
 
         else:
             return
 
     @property
     def trialdefinition(self):
@@ -451,45 +439,39 @@
     def trialdefinition(self, data):
 
         # Get original `trialdefinition` array for reference
         trl = data.trialdefinition
 
         # `DiscreteData`: simply copy relevant sample-count -> trial assignments,
         # for other classes build new trialdefinition array using `t0`-offsets
+
         if self._dataClass in ["SpikeData", "EventData"]:
             trlDef = trl[self.trial_ids, :]
         else:
             trlDef = np.zeros((len(self.trial_ids), trl.shape[1]))
             counter = 0
             for tk, trlno in enumerate(self.trial_ids):
-                tsel = self.time[tk]
+                tsel = self.time[trlno]
                 if isinstance(tsel, slice):
                     start, stop, step = tsel.start, tsel.stop, tsel.step
                     if start is None:
                         start = 0
                     if stop is None:
-                        trlTime = data._get_time([trlno], toilim=[-np.inf, np.inf])[0]
-                        if isinstance(trlTime, list):
-                            stop = np.max(trlTime)
-                            # Avoid creating empty arrays for "static" `SpectralData` objects
-                            if stop == start == 0:
-                                stop += 1
-                        else:
-                            stop = trlTime.stop
+                        stop = trl[trlno, 1] - trl[trlno, 0]
                     if step is None:
                         step = 1
                     nSamples = (stop - start) / step
-                    endSample = stop + data._t0[trlno]
+                    endSample = stop + data._trialdefinition[trlno, 2]
                     t0 = int(endSample - nSamples)
                 else:
                     nSamples = len(tsel)
                     if nSamples == 0:
                         t0 = 0
                     else:
-                        t0 = data._t0[trlno]
+                        t0 = data._trialdefinition[trlno, 2]
                 trlDef[tk, :3] = [counter, counter + nSamples, t0]
                 trlDef[tk, 3:] = trl[trlno, 3:]
                 counter += nSamples
         self._trialdefinition = trlDef
 
     @property
     def sampleinfo(self):
@@ -513,27 +495,14 @@
             # add offset and convert to seconds
             start_end = (start_end + self.trialdefinition[:, 2][:, None]) / self._samplerate
             return start_end
         else:
             return None
 
     @property
-    def timepoints(self):
-        """len(self.trial_ids) list of lists encoding actual (not sample indices!)
-        timing information of unordered `toi` selections"""
-        if self._timeShuffle:
-            return [
-                [
-                    (tvec[tp] + self.trialdefinition[tk, 2]) / self._samplerate
-                    for tp in range(len(tvec))
-                ]
-                for tk, tvec in enumerate(self.time)
-            ]
-
-    @property
     def freq(self):
         """List or slice encoding frequency-selection"""
         return self._freq
 
     @freq.setter
     def freq(self, dataselect):
 
@@ -862,14 +831,15 @@
                 wantedChannels = data.channel_idx[self.channel]
                 chanPerTrial = []
 
             for tk, trialno in enumerate(self.trial_ids):
                 trialArr = np.arange(data._trialslice[trialno].stop - data._trialslice[trialno].start)
                 byTrialSelections = []
                 for selection in actualSelections:
+                    # discrete data selections are still indexed by relative trial indices..
                     byTrialSelections.append(trialArr[getattr(self, selection)[tk]])
 
                 # (try to) preserve unordered selections by processing them first
                 areShuffled = [(np.diff(sel) <= 0).any() for sel in byTrialSelections]
                 combiOrder = np.argsort(areShuffled)[::-1]
                 combinedSelect = byTrialSelections[combiOrder[0]]
                 for combIdx in combiOrder:
@@ -953,15 +923,15 @@
         ppattrs.sort()
 
         # Construct dict of pretty-printable property info
         ppdict = {}
         for attr in ppattrs:
             val = getattr(self, attr)
             if val is not None and attr in self._byTrialProps:
-                val = val[0]
+                val = next(iter(val))
             if isinstance(val, slice):
                 if val.start is val.stop is None:
                     ppdict[attr] = "all {}{}, ".format(
                         attr, "s" if not attr.endswith("s") else ""
                     )
                 elif val.start is None or val.stop is None:
                     ppdict[attr] = "{}-range, ".format(attr)
@@ -982,7 +952,80 @@
 
         # Construct string for printing
         msg = "Syncopy {} selector with ".format(self._dataClass)
         for pout in ppdict.values():
             msg += pout
 
         return msg[:-2]
+
+
+class SelectionTimeIndexer:
+
+    def __init__(self, data_object, toilim, idx_list):
+        """
+        Class to obtain an indexable iterable of time slices
+        from an instantiated Syncopy data class `data_object` with an
+        active time/latency selection given by `toilim`.
+        Relies on the `time` property of the respective
+        `data_object`.
+        Proper parsing of `toilim` is required beforehand.
+
+        Parameters
+        ----------
+        data_object : Syncopy data class, e.g. AnalogData
+
+        idx_list : list
+            List of valid trial indices
+        """
+
+        self.data_object = data_object
+        self.toilim = toilim
+
+        self.idx_set = set(idx_list)
+        self._len = len(idx_list)
+
+        if any(["DiscreteData" in str(base) for base in self.__class__.__mro__]):
+            self.is_discrete = True
+            self.trialtime = data_object.trialtime
+        else:
+            self.is_discrete = False
+            self.trialtime = None
+
+    def construct_time_slice(self, trialno):
+
+        # trivial all time points selection
+        if self.toilim is None:
+            return slice(None)
+
+        # continuous data
+        elif not self.is_discrete:
+            _, selTime = best_match(self.data_object.time[trialno], self.toilim, span=True)
+            return np.s_[selTime[0]:selTime[-1] + 1:1]
+        # discrete data
+        else:
+            trlTime = self.trialtime[self.data_object._trialslice[trialno]]
+            _, selTime = best_match(trlTime, self.toilim, span=True)
+            return np.s_[selTime[0]:selTime[-1] + 1:1]
+
+    def __getitem__(self, trialno):
+        # single trial access via index operator []
+        if not isinstance(trialno, Number):
+            raise SPYTypeError(trialno, "trial index", "single number to index a single trial")
+        if trialno not in self.idx_set:
+            lgl = "index of existing trials"
+            raise SPYValueError(lgl, "trial index", trialno)
+        return self.construct_time_slice(trialno)
+
+    def __iter__(self):
+        # this generator gets freshly created and exhausted
+        # for each new iteration, with only 1 time array being in memory
+        # at any given time
+        yield from (self[i] for i in self.idx_set)
+
+    def __len__(self):
+        return self._len
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        return "{} element iterable".format(self._len)
```

### Comparing `esi_syncopy-2023.3/syncopy/datatype/util.py` & `esi_syncopy-2023.5/syncopy/datatype/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Helpers and tools for Syncopy data classes
 """
 
 import os
 from numbers import Number
+import numpy as np
 
 # Syncopy imports
 from syncopy import __storage__, __storagelimit__, __sessionid__
 from syncopy.shared.errors import SPYTypeError, SPYValueError
 
 __all__ = ['TrialIndexer']
 
@@ -26,31 +27,83 @@
         data_object : Syncopy data class, e.g. AnalogData
 
         idx_list : list
             List of valid trial indices for `_get_trial`
         """
 
         self.data_object = data_object
-        self.idx_list = idx_list
+        self.idx_set = set(idx_list)
         self._len = len(idx_list)
 
     def __getitem__(self, trialno):
         # single trial access via index operator []
         if not isinstance(trialno, Number):
             raise SPYTypeError(trialno, "trial index", "single number to index a single trial")
-        if trialno not in self.idx_list:
+        if trialno not in self.idx_set:
             lgl = "index of existing trials"
             raise SPYValueError(lgl, "trial index", trialno)
         return self.data_object._get_trial(trialno)
 
     def __iter__(self):
         # this generator gets freshly created and exhausted
         # for each new iteration, with only 1 trial being in memory
         # at any given time
-        yield from (self[i] for i in self.idx_list)
+        yield from (self[i] for i in self.idx_set)
+
+    def __len__(self):
+        return self._len
+
+    def __repr__(self):
+        return self.__str__()
+
+    def __str__(self):
+        return "{} element iterable".format(self._len)
+
+
+class TimeIndexer:
+
+    def __init__(self, trialdefinition, samplerate, idx_list):
+        """
+        Class to obtain an indexable time array iterable from
+        an instantiated Syncopy data class `data_object`.
+        Relies on the `trialdefinition` of the respective
+        `data_object`.
+
+        Parameters
+        ----------
+        data_object : Syncopy data class, e.g. AnalogData
+
+        idx_list : list
+            List of valid trial indices
+        """
+
+        self.trialdefinition = trialdefinition
+        self.samplerate = samplerate
+        self.idx_set = set(idx_list)
+        self._len = len(idx_list)
+
+    def construct_time_array(self, trialno):
+
+        start, stop, offset = self.trialdefinition[trialno, :3]
+        return (np.arange(0, stop - start) + offset) / self.samplerate
+
+    def __getitem__(self, trialno):
+        # single trial access via index operator []
+        if not isinstance(trialno, Number):
+            raise SPYTypeError(trialno, "trial index", "single number to index a single trial")
+        if trialno not in self.idx_set:
+            lgl = "index of existing trials"
+            raise SPYValueError(lgl, "trial index", trialno)
+        return self.construct_time_array(trialno)
+
+    def __iter__(self):
+        # this generator gets freshly created and exhausted
+        # for each new iteration, with only 1 time array being in memory
+        # at any given time
+        yield from (self[i] for i in self.idx_set)
 
     def __len__(self):
         return self._len
 
     def __repr__(self):
         return self.__str__()
 
@@ -102,10 +155,7 @@
             err = (
                 "Syncopy core: cannot create temporary storage directory {}. "
                 + "Original error message below\n{}"
             )
             raise IOError(err.format(storage_dir, str(exc)))
 
     return get_dir_size(storage_dir, out="GB")
-
-
-
```

### Comparing `esi_syncopy-2023.3/syncopy/io/__init__.py` & `esi_syncopy-2023.5/syncopy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/io/load_ft.py` & `esi_syncopy-2023.5/syncopy/io/load_ft.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/io/load_nwb.py` & `esi_syncopy-2023.5/syncopy/io/load_nwb.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/io/load_spy_container.py` & `esi_syncopy-2023.5/syncopy/io/load_spy_container.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/io/load_tdt.py` & `esi_syncopy-2023.5/syncopy/io/load_tdt.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/io/save_spy_container.py` & `esi_syncopy-2023.5/syncopy/io/save_spy_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Save Syncopy data objects to disk
 #
 
 # Builtin/3rd party package imports
 import os
 import json
 import h5py
+import shutil
 import numpy as np
 from collections import OrderedDict
 import syncopy as spy
 
 # Local imports
 from syncopy.shared.filetypes import FILE_EXT
 from syncopy.shared.parsers import filename_parser, data_parser
@@ -253,34 +254,36 @@
                     filename.format(ext=FILE_EXT["info"])))
                 SPYWarning(msg.format(key, info_fle))
                 h5f.attrs[key] = [outDict[key][0], "...", outDict[key][-1]]
 
     # Save the dataset names that should be loaded later into the JSON.
     outDict['_hdfFileDatasetProperties'] = list(out._hdfFileDatasetProperties)
 
-
     # Re-assign filename after saving (and remove source in case it came from `__storage__`)
     if not replace:
         h5f.close()
+        # points to source file path
         if __storage__ in out.filename:
+            is_virtual = out.data.is_virtual
             out.data.file.close()
             try:
                 os.unlink(out.filename)
+                if is_virtual:
+                    virtual_dir_path = os.path.splitext(out.filename)[0]
+                    shutil.rmtree(virtual_dir_path)
             except PermissionError as ex:
-                print(f"Could not delete file '{out.filename}': {str(ex)}.")
+                spy.log(f"Could not delete file '{out.filename}': {str(ex)}.", level='IMPORTANT')
         out.data = dataFile
 
     # Compute checksum and finally write JSON (automatically overwrites existing)
     outDict["file_checksum"] = hash_file(dataFile)
 
     with open(infoFile, 'w') as out_json:
         json.dump(outDict, out_json, indent=4)
-
-    return
-
+    spy.log(f"Wrote container to {os.path.dirname(out.filename)}", level='INFO')
 
 def _dict_converter(dct, firstrun=True):
     """
     Convert all dict values having NumPy dtypes to corresponding builtin types
 
     Also works w/ nested dict of dicts and is cycle-save, i.e., it can
     handle self-referencing dictionaires. For instance, consider a nested dict
```

### Comparing `esi_syncopy-2023.3/syncopy/io/utils.py` & `esi_syncopy-2023.5/syncopy/io/utils.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/plotting/_helpers.py` & `esi_syncopy-2023.5/syncopy/plotting/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         The keywords provided to the `selectdata` method
     """
 
     # apply the selection
     dataobject.selectdata(inplace=True, **show_kwargs)
 
     # still have to index the only and single trial
-    idx = dataobject.selection.time[0]
+    idx = next(iter(dataobject.selection.time))
 
     # index selection, again the single trial
     time = dataobject.time[trl][idx]
 
     return time
```

### Comparing `esi_syncopy-2023.3/syncopy/plotting/_plotting.py` & `esi_syncopy-2023.5/syncopy/plotting/_plotting.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/plotting/config.py` & `esi_syncopy-2023.5/syncopy/plotting/config.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/plotting/helpers.py` & `esi_syncopy-2023.5/syncopy/plotting/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Helpers  to generate correct data, labels etc. for the plots
 # from Syncopy dataypes
 #
 
 # Builtin/3rd party package imports
 import numpy as np
 from copy import deepcopy
-import re
 import functools
 
 
 def revert_selection(plotter):
 
     """
     To extract 'meta-information' like time and freq axis
@@ -80,15 +79,15 @@
         The keywords provided to the `selectdata` method
     """
 
     # apply the selection
     dataobject.selectdata(inplace=True, **show_kwargs)
 
     # still have to index the only and single trial
-    idx = dataobject.selection.time[0]
+    idx = next(iter(dataobject.selection.time))
 
     # index selection, again the single trial
     time = dataobject.time[trl][idx]
 
     return time
```

### Comparing `esi_syncopy-2023.3/syncopy/plotting/mp_plotting.py` & `esi_syncopy-2023.5/syncopy/plotting/mp_plotting.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/plotting/sp_plotting.py` & `esi_syncopy-2023.5/syncopy/plotting/sp_plotting.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/plotting/spy_plotting.py` & `esi_syncopy-2023.5/syncopy/plotting/spy_plotting.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/preproc/compRoutines.py` & `esi_syncopy-2023.5/syncopy/preproc/compRoutines.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,30 +112,38 @@
     # max order is signal length
     if order is None:
         order = dat.shape[0]
 
     # construct the filter
     fkernel = design_wsinc(window, order, freq / samplerate, filter_type)
 
+    # switch to time-domain convolutions if NaNs present
+    if np.any(np.isnan(dat)):
+        method = 'direct'
+    else:
+        method = 'fft'
+    # to pass info to user
+    metadata = {'has_nan': np.array(method == 'direct')}
+
     # filtering by convolution
     if direction == 'onepass':
-        filtered = apply_fir(dat, fkernel)
+        filtered = apply_fir(dat, fkernel, method)
 
     # for symmetric filters actual
     # filter direction does NOT matter
     elif direction == 'twopass':
-        filtered = apply_fir(dat, fkernel)
-        filtered = apply_fir(filtered, fkernel)
+        filtered = apply_fir(dat, fkernel, method)
+        filtered = apply_fir(filtered, fkernel, method)
 
     elif direction == 'onepass-minphase':
         # 0-phase transform
         fkernel = minphaserceps(fkernel)
-        filtered = apply_fir(dat, fkernel)
+        filtered = apply_fir(dat, fkernel, method)
 
-    return filtered
+    return filtered, metadata
 
 
 class SincFiltering(ComputationalRoutine):
 
     """
     Compute class that performs filtering with windowed sinc filters
     of :class:`~syncopy.AnalogData` objects
@@ -234,31 +242,35 @@
         dat = dat
 
     # filtering does not change the shape
     outShape = dat.shape
     if noCompute:
         return outShape, np.float32
 
+    # we can't do anything here, but at least
+    # collect this information to pass back to user
+    metadata = {'has_nan': np.array(np.any(np.isnan(dat)))}
+
     # detrend
     if polyremoval == 0:
         dat = sci.detrend(dat, type='constant', axis=0, overwrite_data=True)
     elif polyremoval == 1:
         dat = sci.detrend(dat, type='linear', axis=0, overwrite_data=True)
 
     # design the butterworth filter with "second-order-sections" output
     sos = sci.butter(order, freq, filter_type, fs=samplerate, output='sos')
 
     # do the filtering
     if direction == 'twopass':
         filtered = sci.sosfiltfilt(sos, dat, axis=0)
-        return filtered
+        return filtered, metadata
 
     elif direction == 'onepass':
         filtered = sci.sosfilt(sos, dat, axis=0)
-        return filtered
+        return filtered, metadata
 
 
 class ButFiltering(ComputationalRoutine):
 
     """
     Compute class that performs filtering with butterworth filters
     of :class:`~syncopy.AnalogData` objects
@@ -697,23 +709,35 @@
     outShape = dat.shape
     if noCompute:
         return outShape, np.float32
 
     logger = logging.getLogger("syncopy_" + platform.node())
     logger.debug(f"Detrending data chunk with shape {dat.shape} with polyremoval={polyremoval}.")
 
-    # detrend
+    # we can't do anything here, but at least
+    # collect this information to pass back to user
+    has_nan = np.array(np.any(np.isnan(dat)))
+    metadata = {'has_nan': has_nan}
+
+    # demeaning, this 'works' with NaNs (all nan come back)
     if polyremoval == 0:
         dat = sci.detrend(dat, type='constant', axis=0, overwrite_data=True)
-    elif polyremoval == 1:
+    elif polyremoval == 1 and not has_nan:
         dat = sci.detrend(dat, type='linear', axis=0, overwrite_data=True)
+    # here we have to nan-all the offending channels ourselves
+    elif polyremoval == 1 and has_nan:
+        nan_col_sum = np.sum(np.isnan(dat), axis=0)
+        nan_cols = np.where(nan_col_sum)[0]
+        ok_cols = np.where(nan_col_sum == 0)[0]
+        dat[:, nan_cols] = np.nan
+        dat[:, ok_cols] = sci.detrend(dat[:, ok_cols], type='linear', axis=0, overwrite_data=True)
 
     # renaming
     detrended = dat
-    return detrended
+    return detrended, metadata
 
 
 class Detrending(ComputationalRoutine):
 
     """
     Compute class that performs constant or linear detrending
     of :class:`~syncopy.AnalogData` objects
```

### Comparing `esi_syncopy-2023.3/syncopy/preproc/firws.py` & `esi_syncopy-2023.5/syncopy/preproc/firws.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,44 +3,47 @@
 # Routines for designing and applying
 # FIR windowed sinc filters
 #
 
 # Builtin/3rd party package imports
 import numpy as np
 import scipy.signal.windows as sci_win
-from scipy.signal import fftconvolve
+from scipy.signal import convolve
 
 
-def apply_fir(data, fkernel):
+def apply_fir(data, fkernel, method='fft'):
 
     """
     Convolution of the input `data` with a FIR filter.
     The filter's impulse response is given by `fkernel`.
 
     Parameters
     ----------
     data  : (N, K) :class:`numpy.ndarray`
         Uniformly sampled multi-channel time-series data
         The 1st dimension is interpreted as the time axis,
         columns represent individual channels.
     fkernel : (N,) :class:`numpy.ndarray`
         The time domain representation of the FIR filter
+    method : ('direct', 'fft')
+        Direct convolution in the time-domain or fft based
+        convolution
 
     Returns
     -------
     filtered : (N, K) :class:`~numpy.ndarray`
         The filtered signals
 
     """
 
     slices = [None for _ in data.shape]
     slices[0] = slice(None)
     slices = tuple(slices)
 
-    filtered = fftconvolve(data, fkernel[slices], mode="same")
+    filtered = convolve(data, fkernel[slices], mode="same", method=method)
     return filtered
 
 
 def design_wsinc(window, order, f_c, filter_type="lp"):
 
     """
     Construct the windowed sinc filter kernel in the time domain
```

### Comparing `esi_syncopy-2023.3/syncopy/preproc/preprocessing.py` & `esi_syncopy-2023.5/syncopy/preproc/preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # Builtin/3rd party package imports
 import numpy as np
 
 # Syncopy imports
 from syncopy import AnalogData
 from syncopy.shared.parsers import data_parser, scalar_parser, array_parser
 from syncopy.shared.tools import get_defaults, get_frontend_cfg
-from syncopy.shared.errors import SPYValueError, SPYInfo
+from syncopy.shared.errors import SPYValueError, SPYInfo, SPYWarning
+from syncopy.shared.metadata import metadata_from_hdf5_file
 from syncopy.shared.kwarg_decorators import (
     unwrap_cfg,
     unwrap_select,
     detect_parallel_client,
 )
 from syncopy.shared.input_processors import (
     check_effective_parameters,
@@ -190,19 +191,14 @@
 
     # -- get trial info
 
     # if a subset selection is present
     # get sampleinfo and check for equidistancy
     if data.selection is not None:
         sinfo = data.selection.trialdefinition[:, :2]
-        # user picked discrete set of time points
-        if isinstance(data.selection.time[0], list):
-            lgl = "equidistant time points (toi) or time slice (toilim)"
-            actual = "non-equidistant set of time points"
-            raise SPYValueError(legal=lgl, varname="select", actual=actual)
     else:
         sinfo = data.sampleinfo
     lenTrials = np.diff(sinfo).squeeze()
 
     # check for equidistant sampling as needed for filtering
     # FIXME: could be too slow, see #259
     # if not all([np.allclose(np.diff(time), 1 / data.samplerate) for time in data.time]):
@@ -344,14 +340,15 @@
         )
 
         # not really a `filterMethod` though..
         filterMethod = Detrending(polyremoval=polyremoval, timeAxis=timeAxis)
     # only zscoring
     else:
         filterMethod = None
+
     # -------------------------------------------
     # Call the chosen filter ComputationalRoutine
     # -------------------------------------------
 
     # unlikely but possible: post-processing without filtering
     if filterMethod is None:
         filtered = data
@@ -364,14 +361,29 @@
             chan_per_worker=kwargs.get("chan_per_worker"),
             keeptrials=True,
         )
         filterMethod.compute(
             data, filtered, parallel=kwargs.get("parallel"), log_dict=log_dict
         )
 
+        # give warnings if NaNs were present
+        nan_trials = []
+        for key, value in metadata_from_hdf5_file(filtered.filename).items():
+            if 'has_nan' in key and value:
+                # try to also record the trial numbers
+                trl_num = key.split('__')[-1].split('_')[0]
+                nan_trials.append(int(trl_num))
+
+        if len(nan_trials) != 0:
+            msg = "Data contains NaNs! See `.info['nan_trials']` for the offending trials"
+            if filter_class == 'but':
+                msg += "\n\t\t try using a 'onepass' FIR filter of low order.."
+            SPYWarning(msg)
+        filtered.info['nan_trials'] = nan_trials
+
     # -- check for post-processing flags --
 
     if rectify:
         log_dict["rectify"] = rectify
         rectified = AnalogData(dimord=data.dimord)
         rectCR = Rectify()
         rectCR.initialize(
```

### Comparing `esi_syncopy-2023.3/syncopy/preproc/resampledata.py` & `esi_syncopy-2023.5/syncopy/preproc/resampledata.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,18 +109,14 @@
     timeAxis = data.dimord.index("time")
 
     # if a subset selection is present
     # get sampleinfo and check for equidistancy
     if data.selection is not None:
         sinfo = data.selection.trialdefinition[:, :2]
         # user picked discrete set of time points
-        if isinstance(data.selection.time[0], list):
-            lgl = "equidistant time points (toi) or time slice (toilim)"
-            actual = "non-equidistant set of time points"
-            raise SPYValueError(legal=lgl, varname="select", actual=actual)
     else:
         sinfo = data.sampleinfo
     lenTrials = np.diff(sinfo).squeeze()
 
     # Get everything of interest in local namespace
     defaults = get_defaults(resampledata)
     lcls = locals()
```

### Comparing `esi_syncopy-2023.3/syncopy/preproc/resampling.py` & `esi_syncopy-2023.5/syncopy/preproc/resampling.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/__init__.py` & `esi_syncopy-2023.5/syncopy/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/computational_routine.py` & `esi_syncopy-2023.5/syncopy/shared/computational_routine.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/const_def.py` & `esi_syncopy-2023.5/syncopy/shared/const_def.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/dask_helpers.py` & `esi_syncopy-2023.5/syncopy/shared/dask_helpers.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/errors.py` & `esi_syncopy-2023.5/syncopy/shared/errors.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/filetypes.py` & `esi_syncopy-2023.5/syncopy/shared/filetypes.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/input_processors.py` & `esi_syncopy-2023.5/syncopy/shared/input_processors.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/kwarg_decorators.py` & `esi_syncopy-2023.5/syncopy/shared/kwarg_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,20 +247,21 @@
                     lgl = "only one Syncopy data object"
                     raise SPYValueError(lgl, varname='data')
                 if isinstance(arg, spy.datatype.base_data.BaseData):
                     data = arg
                 else:
                     posargs.append(arg)
 
-        # if there was no Syncopy data found at this point, we have to give up
+        # if there was no Syncopy data found at this point,
+        # we call the wrapped function without it
         if data is None:
-            raise SPYError("Found no Syncopy data object as input")
-
-        # Call function with unfolded `data` + modified positional/keyword args
-        return func(data, *posargs, **cfg)
+            return func(*posargs, **cfg)
+        else:
+            # Call function with unfolded `data` + modified positional/keyword args
+            return func(data, *posargs, **cfg)
 
     # Append two-liner to docstring header mentioning the use of `cfg`
     introEntry = \
     "    \n" +\
     "    The parameters listed below can be provided as is or a via a `cfg`\n" +\
     "    configuration 'structure', see Notes for details. \n"
     wrapper_cfg.__doc__ = _append_docstring(wrapper_cfg,
```

### Comparing `esi_syncopy-2023.3/syncopy/shared/latency.py` & `esi_syncopy-2023.5/syncopy/shared/latency.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/log.py` & `esi_syncopy-2023.5/syncopy/shared/log.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import sys
 import logging
 import socket
 import syncopy
 import warnings
 import datetime
 import platform
-import getpass
 
 
 loggername = "syncopy"  # Since this is a library, we should not use the root logger (see Python logging docs).
 loglevels = ['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']
 
 
 def setup_logging(spydir=None, session=""):
@@ -61,14 +60,20 @@
 
     # Interactive formatter: no hostname and session info (less clutter on terminal).
     fmt_interactive = logging.Formatter('%(asctime)s - %(levelname)s: %(message)s', datefmt_interactive)
     # Log file formatter: with hostname and session info.
     fmt_with_hostname = logging.Formatter('%(asctime)s - %(levelname)s - %(hostname)s - %(session)s: %(message)s',
                                           datefmt_file)
 
+    # Allow users to set env variable SPYLOGMSECS to have millisecond precision in logs. Useful for performance profiling.
+    if os.environ.get("SPYLOGMSECS"):
+        fmt_interactive = logging.Formatter('%(asctime)s.%(msecs)03d - %(levelname)s: %(message)s', datefmt_interactive)
+        fmt_with_hostname = logging.Formatter('%(asctime)s.%(msecs)03d - %(levelname)s - %(hostname)s - %(session)s: %(message)s',
+                                          datefmt_file)
+
     sh = logging.StreamHandler(sys.stdout)
     sh.setFormatter(fmt_interactive)
     spy_logger.addHandler(sh)
 
     logfile = os.path.join(syncopy.__logdir__, f'syncopy.log')
     fh = logging.FileHandler(logfile)  # The default mode is 'append'.
     fh.addFilter(HostnameFilter())
```

### Comparing `esi_syncopy-2023.3/syncopy/shared/metadata.py` & `esi_syncopy-2023.5/syncopy/shared/metadata.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/parsers.py` & `esi_syncopy-2023.5/syncopy/shared/parsers.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/queries.py` & `esi_syncopy-2023.5/syncopy/shared/queries.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/shared/tools.py` & `esi_syncopy-2023.5/syncopy/shared/tools.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/README.md` & `esi_syncopy-2023.5/syncopy/specest/README.md`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/_norm_spec.py` & `esi_syncopy-2023.5/syncopy/specest/_norm_spec.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/compRoutines.py` & `esi_syncopy-2023.5/syncopy/specest/compRoutines.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/fooofspy.py` & `esi_syncopy-2023.5/syncopy/specest/fooofspy.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/freqanalysis.py` & `esi_syncopy-2023.5/syncopy/specest/freqanalysis.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/mtmconvol.py` & `esi_syncopy-2023.5/syncopy/specest/mtmconvol.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/mtmfft.py` & `esi_syncopy-2023.5/syncopy/specest/mtmfft.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/stft.py` & `esi_syncopy-2023.5/syncopy/specest/stft.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/superlet.py` & `esi_syncopy-2023.5/syncopy/specest/superlet.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/wavelet.py` & `esi_syncopy-2023.5/syncopy/specest/wavelet.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/wavelets/transform.py` & `esi_syncopy-2023.5/syncopy/specest/wavelets/transform.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/specest/wavelets/wavelets.py` & `esi_syncopy-2023.5/syncopy/specest/wavelets/wavelets.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/statistics/compRoutines.py` & `esi_syncopy-2023.5/syncopy/statistics/compRoutines.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/statistics/jackknifing.py` & `esi_syncopy-2023.5/syncopy/statistics/jackknifing.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/statistics/psth.py` & `esi_syncopy-2023.5/syncopy/statistics/psth.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/statistics/spike_psth.py` & `esi_syncopy-2023.5/syncopy/statistics/spike_psth.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/statistics/summary_stats.py` & `esi_syncopy-2023.5/syncopy/statistics/summary_stats.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/statistics/timelockanalysis.py` & `esi_syncopy-2023.5/syncopy/statistics/timelockanalysis.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/README.md` & `esi_syncopy-2023.5/syncopy/tests/README.md`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/backend/run_tests.sh` & `esi_syncopy-2023.5/syncopy/tests/backend/run_tests.sh`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/backend/test_conn.py` & `esi_syncopy-2023.5/syncopy/tests/backend/test_conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # syncopy.connectivity backend method tests
 #
 import numpy as np
 import matplotlib.pyplot as ppl
 
-from syncopy.tests import synth_data
+from syncopy import synthdata
 from syncopy.connectivity import csd
 from syncopy.connectivity import ST_compRoutines as stCR
 from syncopy.connectivity.wilson_sf import (
     wilson_sf,
     regularize_csd,
     max_rel_err
 )
@@ -187,15 +187,15 @@
     fs = 200
     nChannels = 2
     nSamples = 1000
     nTrials = 150
     CSDav = np.zeros((nSamples // 2 + 1, nChannels, nChannels), dtype=np.complex64)
     for _ in range(nTrials):
 
-        sol = synth_data.AR2_network(nSamples=nSamples, seed=None)
+        sol = synthdata.ar2_network(nSamples=nSamples, seed=None, nTrials=None)
         # --- get the (single trial) CSD ---
 
         CSD, freqs = csd.csd(sol, fs,
                              norm=False)
 
         CSDav += CSD
 
@@ -272,15 +272,15 @@
     nSamples = 1500
     nTrials = 100
 
     CSDav = np.zeros((nSamples // 2 + 1, 2, 2), dtype=np.complex64)
     for _ in range(nTrials):
 
         # -- simulate 2 AR(2) processes with 2->1 coupling --
-        sol = synth_data.AR2_network(nSamples=nSamples)
+        sol = synthdata.ar2_network(nSamples=nSamples, nTrials=None)
 
         # --- get CSD ---
         bw = 2
         NW = bw * nSamples / (2 * fs)
         Kmax = int(2 * NW - 1)  # optimal number of tapers
         CSD, freqs = csd.csd(sol, fs,
                              taper='dpss',
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/backend/test_fooofspy.py` & `esi_syncopy-2023.5/syncopy/tests/backend/test_fooofspy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 import numpy as np
 import pytest
 
 
 from syncopy.specest.fooofspy import fooofspy
 from syncopy.tests.backend.test_resampling import trl_av_power
-from syncopy.tests import synth_data as sd
+from syncopy import synthdata as sd
 from fooof.sim.gen import gen_power_spectrum
 
 import matplotlib.pyplot as plt
 
 
 def _power_spectrum(freq_range=[3, 40],
                     freq_res=0.5):
@@ -34,15 +34,15 @@
     """
     Create AR(1) background + ratio * (harmonic + phase diffusion)
     and take the mtmfft with 1Hz spectral smoothing
     """
     fs = 400
     nSamples = 1000
     # single channel and alpha2 = 0 <-> single AR(1)
-    signals = [sd.AR2_network(AdjMat=np.zeros(1),
+    signals = [sd.ar2_network(AdjMat=np.zeros(1),
                               alphas=[0.8, 0],
                               nSamples=nSamples) + ratio * sd.phase_diffusion(freq=hfreq,
                                                                               fs=fs, eps=0.1,
                                                                               nChannels=1)
                for i in range(nTrials)]
 
     power, freqs = trl_av_power(signals, nSamples, fs, tapsmofrq=1)
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/backend/test_resampling.py` & `esi_syncopy-2023.5/syncopy/tests/backend/test_resampling.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/backend/test_timefreq.py` & `esi_syncopy-2023.5/syncopy/tests/backend/test_timefreq.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/conftest.py` & `esi_syncopy-2023.5/syncopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/helpers.py` & `esi_syncopy-2023.5/syncopy/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/local_spy.py` & `esi_syncopy-2023.5/syncopy/tests/local_spy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,44 @@
 # -*- coding: utf-8 -*-
 #
 # Simple script for testing Syncopy w/o pip-installing it
 #
 
 # Builtin/3rd party package imports
 import numpy as np
-
-# Add SynCoPy package to Python search path
 import os
 import sys
-spy_path = os.path.abspath(".." + os.sep + "..")
-if spy_path not in sys.path:
-    sys.path.insert(0, spy_path)
 
 # Import package
 import syncopy as spy
 
-# Import artificial data generator
-from syncopy.tests.misc import generate_artificial_data
-from syncopy.tests import synth_data
-
+# Import artificial data generators
+from syncopy import synthdata
 
 # Prepare code to be executed using, e.g., iPython's `%run` magic command
 if __name__ == "__main__":
 
     nTrials = 20
 
     nSamples = 1000
     fs = 500
 
     trls = []
     AdjMat = np.zeros((2, 2))
     # coupling from 0 to 1
     AdjMat[0, 1] = .15
     alphas = [.55, -.8]
-    adata = synth_data.AR2_network(nTrials, samplerate=fs,
-                                   AdjMat=AdjMat,
+    adata = synthdata.ar2_network(nTrials, samplerate=fs,
+                                  AdjMat=AdjMat,
+                                  nSamples=nSamples,
+                                  alphas=alphas)
+    adata += synthdata.ar2_network(nTrials, AdjMat=np.zeros((2, 2)),
+                                   samplerate=fs,
                                    nSamples=nSamples,
-                                   alphas=alphas)
-    adata += synth_data.AR2_network(nTrials, AdjMat=np.zeros((2, 2)),
-                                    samplerate=fs,
-                                    nSamples=nSamples,
-                                    alphas=[0.9, 0])
+                                   alphas=[0.9, 0])
 
     spec = spy.freqanalysis(adata, tapsmofrq=2, keeptrials=False)
     foi = np.linspace(40, 160, 25)
     coh = spy.connectivityanalysis(adata, method='coh', tapsmofrq=5)
 
     # show new plotting
     # adata.singlepanelplot(trials=12, toilim=[0, 0.35])
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/misc.py` & `esi_syncopy-2023.5/syncopy/tests/misc.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/run_tests.cmd` & `esi_syncopy-2023.5/syncopy/tests/run_tests.cmd`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/run_tests.sh` & `esi_syncopy-2023.5/syncopy/tests/run_tests.sh`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_attach_dataset.py` & `esi_syncopy-2023.5/syncopy/tests/test_attach_dataset.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_basedata.py` & `esi_syncopy-2023.5/syncopy/tests/test_basedata.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_cfg.py` & `esi_syncopy-2023.5/syncopy/tests/test_cfg.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import tempfile
 import os
 import dask.distributed as dd
 
 # Local imports
 import syncopy as spy
 
-import syncopy.tests.synth_data as synth_data
+from syncopy import synthdata
 from syncopy.shared.tools import StructDict
 
 
 availableFrontend_cfgs = {'freqanalysis': {'method': 'mtmconvol', 't_ftimwin': 0.1, 'foi': np.arange(1,60)},
                           'preprocessing': {'freq': 10, 'filter_class': 'firws', 'filter_type': 'hp'},
                           'resampledata': {'resamplefs': 125, 'lpfreq': 60},
                           'connectivityanalysis': {'method': 'coh', 'tapsmofrq': 5},
@@ -31,18 +31,18 @@
     nChannels = 3
     nTrials = 10
     fs = 200
     fNy = fs / 2
 
     # -- use flat white noise as test data --
 
-    adata = synth_data.white_noise(nTrials,
-                                   nSamples=nSamples,
-                                   nChannels=nChannels,
-                                   samplerate=fs)
+    adata = synthdata.white_noise(nTrials=nTrials,
+                                  nSamples=nSamples,
+                                  nChannels=nChannels,
+                                  samplerate=fs)
 
     # for toi tests, -1s offset
     time_span = [-.9, -.6]
     flow, fhigh = 0.3 * fNy, 0.4 * fNy
 
     def test_single_frontends(self):
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_computationalroutine.py` & `esi_syncopy-2023.5/syncopy/tests/test_computationalroutine.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,29 +126,28 @@
                           "channel": range(0, int(nChannels / 2)),
                           "latency": [-0.5, 0.6]}]
 
     # Error tolerances and respective quality metrics (depend on data selection!)
     tols = [1e-6, 1e-6, 1e-2]
     metrix = [np.max, np.max, np.mean]
 
-
     def test_sequential_equidistant(self):
         for sk, select in enumerate(self.sigdataSelections):
             sel = Selector(self.sigdata, select)
             out = filter_manager(self.sigdata, self.b, self.a, select=select)
 
             # check correct signal filtering (especially wrt data-selection)
             if select is None:
                 reference = self.orig
             else:
                 ref = []
                 for tk, trlno in enumerate(sel.trial_ids):
-                    ref.append(self.origdata.trials[trlno][sel.time[tk], sel.channel])
+                    ref.append(self.origdata.trials[trlno][sel.time[trlno], sel.channel])
                     # check for correct time selection
-                    assert np.array_equal(out.time[tk], self.sigdata.time[trlno][sel.time[tk]])
+                    assert np.array_equal(out.time[tk], self.sigdata.time[trlno][sel.time[trlno]])
                 reference = np.vstack(ref)
             assert self.metrix[sk](np.abs(out.data - reference)) < self.tols[sk]
             assert np.array_equal(out.channel, self.sigdata.channel[sel.channel])
 
             # ensure pre-selection is equivalent to in-place selection
             if select is None:
                 selected = self.sigdata.selectdata()
@@ -163,15 +162,15 @@
 
             # check correct signal filtering (especially wrt data-selection)
             if select is None:
                 reference = self.orig[:self.t.size, :]
             else:
                 ref = np.zeros(out.trials[0].shape)
                 for tk, trlno in enumerate(sel.trial_ids):
-                    ref += self.origdata.trials[trlno][sel.time[tk], sel.channel]
+                    ref += self.origdata.trials[trlno][sel.time[trlno], sel.channel]
                     # check for correct time selection (accounting for trial-averaging)
                     assert np.array_equal(out.time[0], self.sigdata.time[0][sel.time[0]])
                 reference = ref / len(sel.trial_ids)
             assert self.metrix[sk](np.abs(out.data - reference)) < self.tols[sk]
             assert np.array_equal(out.channel, self.sigdata.channel[sel.channel])
 
             # ensure pre-selection is equivalent to in-place selection
@@ -195,19 +194,19 @@
             for select in self.artdataSelections:
                 sel = Selector(nonequidata, select)
                 out = filter_manager(nonequidata, self.b, self.a, select=select)
 
                 # compare expected w/actual shape of computed data
                 reference = 0
                 for tk, trlno in enumerate(sel.trial_ids):
-                    reference += nonequidata.trials[trlno][sel.time[tk]].shape[0]
+                    reference += nonequidata.trials[trlno][sel.time[trlno]].shape[0]
                     # check for correct time selection
                     # FIXME: remove `if` below as soon as `time` prop for lists is fixed
                     if not isinstance(sel.time[0], list):
-                        assert np.array_equal(out.time[tk], nonequidata.time[trlno][sel.time[tk]])
+                        assert np.array_equal(out.time[tk], nonequidata.time[trlno][sel.time[trlno]])
 
                 assert out.data.shape[0] == reference
                 assert np.array_equal(out.channel, nonequidata.channel[sel.channel])
 
                 # ensure pre-selection is equivalent to in-place selection
                 if select is None:
                     selected = nonequidata.selectdata()
@@ -254,16 +253,16 @@
                 print(f"test_computationalroutine: loading done")
                 assert out.filename == dummy.filename, f"save: expected out.filename '{out.filename}' == dummy.filename '{dummy.filename}'."
                 if select is None:
                     reference = self.orig
                 else:
                     ref = []
                     for tk, trlno in enumerate(sel.trial_ids):
-                        ref.append(self.origdata.trials[trlno][sel.time[tk], sel.channel])
-                        assert np.array_equal(dummy.time[tk], self.sigdata.time[trlno][sel.time[tk]])
+                        ref.append(self.origdata.trials[trlno][sel.time[trlno], sel.channel])
+                        assert np.array_equal(dummy.time[tk], self.sigdata.time[trlno][sel.time[trlno]])
                     reference = np.vstack(ref)
                 assert self.metrix[sk](np.abs(dummy.data - reference)) < self.tols[sk]
                 assert np.array_equal(dummy.channel, self.sigdata.channel[sel.channel])
                 time.sleep(0.01)
                 del out
 
                 # ensure out_sel is written/read correctly
@@ -292,17 +291,17 @@
 
                     # check correct signal filtering (especially wrt data-selection)
                     if select is None:
                         reference = self.orig
                     else:
                         ref = []
                         for tk, trlno in enumerate(sel.trial_ids):
-                            ref.append(self.origdata.trials[trlno][sel.time[tk], sel.channel])
+                            ref.append(self.origdata.trials[trlno][sel.time[trlno], sel.channel])
                             # check for correct time selection
-                            assert np.array_equal(out.time[tk], self.sigdata.time[trlno][sel.time[tk]])
+                            assert np.array_equal(out.time[tk], self.sigdata.time[trlno][sel.time[trlno]])
                         reference = np.vstack(ref)
                     assert self.metrix[sk](np.abs(out.data - reference)) < self.tols[sk]
                     assert np.array_equal(out.channel, self.sigdata.channel[sel.channel])
 
                     # ensure correct no. HDF5 files were generated for virtual data-set
                     if parallel_store:
                         nfiles = len(glob(os.path.join(os.path.splitext(out.filename)[0], "*.h5")))
@@ -330,16 +329,16 @@
                                          keeptrials=False)
 
                     # check correct signal filtering (especially wrt data-selection)
                     if select is None:
                         reference = self.orig[:self.t.size, :]
                     else:
                         ref = np.zeros(out.trials[0].shape)
-                        for tk, trlno in enumerate(sel.trial_ids):
-                            ref += self.origdata.trials[trlno][sel.time[tk], sel.channel]
+                        for trlno, trlno in enumerate(sel.trial_ids):
+                            ref += self.origdata.trials[trlno][sel.time[trlno], sel.channel]
                             # check for correct time selection (accounting for trial-averaging)
                             assert np.array_equal(out.time[0], self.sigdata.time[0][sel.time[0]])
                         reference = ref / len(sel.trial_ids)
                     assert self.metrix[sk](np.abs(out.data - reference)) < self.tols[sk]
                     assert np.array_equal(out.channel, self.sigdata.channel[sel.channel])
                     assert out.data.is_virtual == False
 
@@ -372,19 +371,19 @@
                         out = filter_manager(nonequidata, self.b, self.a, select=select,
                                              chan_per_worker=chan_per_worker, parallel=True,
                                              parallel_store=parallel_store)
 
                         # compare expected w/actual shape of computed data
                         reference = 0
                         for tk, trlno in enumerate(sel.trial_ids):
-                            reference += nonequidata.trials[trlno][sel.time[tk]].shape[0]
+                            reference += nonequidata.trials[trlno][sel.time[trlno]].shape[0]
                             # check for correct time selection
                             # FIXME: remove `if` below as soon as `time` prop for lists is fixed
                             if not isinstance(sel.time[0], list):
-                                assert np.array_equal(out.time[tk], nonequidata.time[trlno][sel.time[tk]])
+                                assert np.array_equal(out.time[tk], nonequidata.time[trlno][sel.time[trlno]])
                         assert out.data.shape[0] == reference
                         assert np.array_equal(out.channel, nonequidata.channel[sel.channel])
                         assert out.data.is_virtual == parallel_store
 
                         if parallel_store:
                             nfiles = len(glob(os.path.join(os.path.splitext(out.filename)[0], "*.h5")))
                             if chan_per_worker is None:
@@ -447,16 +446,16 @@
                     assert out.filename == dummy.filename
                     assert not out.data.is_virtual
                     if select is None:
                         reference = self.orig
                     else:
                         ref = []
                         for tk, trlno in enumerate(sel.trial_ids):
-                            ref.append(self.origdata.trials[trlno][sel.time[tk], sel.channel])
-                            assert np.array_equal(dummy.time[tk], self.sigdata.time[trlno][sel.time[tk]])
+                            ref.append(self.origdata.trials[trlno][sel.time[trlno], sel.channel])
+                            assert np.array_equal(dummy.time[tk], self.sigdata.time[trlno][sel.time[trlno]])
                         reference = np.vstack(ref)
                     assert self.metrix[sk](np.abs(dummy.data - reference)) < self.tols[sk]
                     assert np.array_equal(dummy.channel, self.sigdata.channel[sel.channel])
                     # del dummy, out
 
                     # ensure out_sel is written/read correctly
                     fname2 = os.path.join(tdir, "dummy2")
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_connectivity.py` & `esi_syncopy-2023.5/syncopy/tests/test_connectivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Local imports
 
 import syncopy as spy
 from syncopy import AnalogData, SpectralData
 from syncopy.connectivity.connectivity_analysis import connectivity_outputs
 from syncopy import connectivityanalysis as cafunc
-import syncopy.tests.synth_data as synth_data
+from syncopy import synthdata
 import syncopy.tests.helpers as helpers
 from syncopy.shared.errors import SPYValueError
 from syncopy.shared.tools import get_defaults
 
 # Decorator to decide whether or not to run memory-intensive tests
 availMem = psutil.virtual_memory().total
 minRAM = 5
@@ -103,19 +103,19 @@
 
     # channel indices of coupling
     # a number other than 0 at AdjMat(i,j)
     # means coupling from i->j
     cpl_idx = np.where(AdjMat)
     nocpl_idx = np.where(AdjMat == 0)
 
-    data = synth_data.AR2_network(nTrials,
-                                  AdjMat=AdjMat,
-                                  nSamples=nSamples,
-                                  samplerate=fs,
-                                  seed=42)
+    data = synthdata.ar2_network(AdjMat=AdjMat,
+                                 nSamples=nSamples,
+                                 samplerate=fs,
+                                 nTrials=nTrials,
+                                 seed=42)
 
     time_span = [-1, nSamples / fs - 1]   # -1s offset
 
     cfg = spy.StructDict()
     cfg.tapsmofrq = 1
     cfg.foi = None
     spec = spy.freqanalysis(data, cfg, output='fourier', keeptapers=True, demean_taper=True)
@@ -275,29 +275,29 @@
     nTrials = 100
     fs = 1000
 
     # -- two harmonics with individual phase diffusion --
 
     f1, f2 = 20, 40
     # a lot of phase diffusion (1% per step) in the 20Hz band
-    s1 = synth_data.phase_diffusion(nTrials, freq=f1,
-                                    eps=.03,
-                                    nChannels=nChannels,
-                                    nSamples=nSamples,
-                                    seed=helpers.test_seed)
+    s1 = synthdata.phase_diffusion(nTrials=nTrials, freq=f1,
+                                   eps=.03,
+                                   nChannels=nChannels,
+                                   nSamples=nSamples,
+                                   seed=helpers.test_seed)
 
     # little diffusion in the 40Hz band
-    s2 = synth_data.phase_diffusion(nTrials, freq=f2,
-                                    eps=.001,
-                                    nChannels=nChannels,
-                                    nSamples=nSamples,
-                                    seed=helpers.test_seed)
+    s2 = synthdata.phase_diffusion(nTrials=nTrials, freq=f2,
+                                   eps=.001,
+                                   nChannels=nChannels,
+                                   nSamples=nSamples,
+                                   seed=helpers.test_seed)
 
-    wn = synth_data.white_noise(nTrials, nChannels=nChannels, nSamples=nSamples,
-                                seed=helpers.test_seed)
+    wn = synthdata.white_noise(nTrials=nTrials, nChannels=nChannels, nSamples=nSamples,
+                               seed=helpers.test_seed)
 
     # superposition
     data = s1 + s2 + wn
     data.samplerate = fs
     time_span = [-1, nSamples / fs - 1]   # -1s offset
 
     # spectral analysis
@@ -519,28 +519,28 @@
     fs = 1000
     Method = 'csd'
 
     # -- two harmonics with individual phase diffusion --
 
     f1, f2 = 20, 40
     # a lot of phase diffusion (1% per step) in the 20Hz band
-    s1 = synth_data.phase_diffusion(nTrials, freq=f1,
-                                    eps=.01,
-                                    nChannels=nChannels,
-                                    nSamples=nSamples,
-                                    seed=42)
+    s1 = synthdata.phase_diffusion(nTrials=nTrials, freq=f1,
+                                   eps=.01,
+                                   nChannels=nChannels,
+                                   nSamples=nSamples,
+                                   seed=42)
 
     # little diffusion in the 40Hz band
-    s2 = synth_data.phase_diffusion(nTrials, freq=f2,
-                                    eps=.001,
-                                    nChannels=nChannels,
-                                    nSamples=nSamples,
-                                    seed=42)
+    s2 = synthdata.phase_diffusion(nTrials=nTrials, freq=f2,
+                                   eps=.001,
+                                   nChannels=nChannels,
+                                   nSamples=nSamples,
+                                   seed=42)
 
-    wn = synth_data.white_noise(nTrials, nChannels=nChannels, nSamples=nSamples)
+    wn = synthdata.white_noise(nTrials=nTrials, nChannels=nChannels, nSamples=nSamples)
 
     # superposition
     data = s1 + s2 + wn
     data.samplerate = fs
     time_span = [-1, nSamples / fs - 1]   # -1s offset
 
     # spectral analysis
@@ -587,27 +587,29 @@
     # -- a single harmonic with phase shifts between channels
 
     f1 = 10   # period is 0.1s
     trls = []
     for _ in range(nTrials):
 
         # no phase diffusion
-        p1 = synth_data.phase_diffusion(freq=f1,
-                                        eps=0,
-                                        nChannels=nChannels,
-                                        nSamples=nSamples,
-                                        seed=42,
-                                        return_phase=True)
+        p1 = synthdata.phase_diffusion(freq=f1,
+                                       eps=0,
+                                       nChannels=nChannels,
+                                       nSamples=nSamples,
+                                       seed=42,
+                                       return_phase=True,
+                                       nTrials=None)
         # same frequency but more diffusion
-        p2 = synth_data.phase_diffusion(freq=f1,
-                                        eps=0.1,
-                                        nChannels=1,
-                                        nSamples=nSamples,
-                                        seed=42,
-                                        return_phase=True)
+        p2 = synthdata.phase_diffusion(freq=f1,
+                                       eps=0.1,
+                                       nChannels=1,
+                                       nSamples=nSamples,
+                                       seed=42,
+                                       return_phase=True,
+                                       nTrials=None)
 
         # set 2nd channel to higher phase diffusion
         p1[:, 1] = p2[:, 0]
         # add a pi/2 phase shift for the even channels
         p1[:, 2::2] += np.pi / 2
 
         trls.append(np.cos(p1))
@@ -737,21 +739,21 @@
     nTrials = 20
     fs = 1000
 
     # -- one harmonic with individual phase diffusion --
 
     f1 = 20
     # phase diffusion (1% per step) in the 20Hz band
-    s1 = synth_data.phase_diffusion(nTrials, freq=f1,
-                                    eps=.01,
-                                    nChannels=nChannels,
-                                    nSamples=nSamples,
-                                    seed=helpers.test_seed)
-    wn = synth_data.white_noise(nTrials, nChannels=nChannels, nSamples=nSamples,
-                                seed=helpers.test_seed)
+    s1 = synthdata.phase_diffusion(nTrials=nTrials, freq=f1,
+                                   eps=.01,
+                                   nChannels=nChannels,
+                                   nSamples=nSamples,
+                                   seed=helpers.test_seed)
+    wn = synthdata.white_noise(nTrials=nTrials, nChannels=nChannels, nSamples=nSamples,
+                               seed=helpers.test_seed)
 
     # superposition
     data = s1 + wn
     data.samplerate = fs
     time_span = [-1, nSamples / fs - 1]   # -1s offset
 
     # spectral analysis
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_continuousdata.py` & `esi_syncopy-2023.5/syncopy/tests/test_continuousdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,20 +192,22 @@
         for attr in ["channel", "data", "sampleinfo", "trialinfo"]:
             assert getattr(dummy, attr) is None
         with pytest.raises(SPYTypeError):
             AnalogData({})
 
         # -- test with single array--
 
-        dummy = AnalogData(data=self.data)
+        chan_labels = [str(i) for i in range(self.nc)]
+        dummy = AnalogData(data=self.data, channel=chan_labels)
         assert dummy.dimord == AnalogData._defaultDimord
         assert dummy.channel.size == self.nc
         assert (dummy.sampleinfo == [0, self.ns]).min()
         assert dummy.trialinfo.shape == (1, 0)
         assert np.array_equal(dummy.data, self.data)
+        assert np.all(dummy.channel == chan_labels)
 
         # wrong shape for data-type
         with pytest.raises(SPYValueError):
             AnalogData(np.ones((3,)))
 
         # -- test with list of arrays
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_datatype_util.py` & `esi_syncopy-2023.5/syncopy/tests/test_datatype_util.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_decorators.py` & `esi_syncopy-2023.5/syncopy/tests/test_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,20 +161,14 @@
         assert "`data` must be Syncopy data object!" in str(exc.value)
 
         # cfg is not dict/StructDict
         with pytest.raises(SPYTypeError)as exc:
             group_objects(cfg="invalid")
         assert "Wrong type of `cfg`: expected dictionary-like" in str(exc.value)
 
-        # input is just a numpy array
-        data = np.arange(2)
-        with pytest.raises(SPYError) as exc:
-            group_objects(data)
-        assert "Found no Syncopy data object as input" in str(exc.value)
-
 
     def test_varargin(self):
         """
         This was originally meant to test multiple Syncopy objects
         as 'data' input at once, this functionality was deprecated and got
         removed. What remains are the `groupbychan` cfg and select tests.
         """
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_discretedata.py` & `esi_syncopy-2023.5/syncopy/tests/test_discretedata.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_info.py` & `esi_syncopy-2023.5/syncopy/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_logging.py` & `esi_syncopy-2023.5/syncopy/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_metadata.py` & `esi_syncopy-2023.5/syncopy/tests/test_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import os
 import dask.distributed as dd
 
 # Local imports
 from syncopy import freqanalysis
 from syncopy.datatype.methods.copy import copy
 from syncopy.shared.tools import get_defaults
-from syncopy.tests.synth_data import AR2_network, phase_diffusion
+from syncopy.synthdata import ar2_network, phase_diffusion
 from syncopy.shared.metadata import encode_unique_md_label, decode_unique_md_label, parse_cF_returns, _parse_backend_metadata, _merge_md_list, metadata_from_hdf5_file, metadata_nest, metadata_unnest
 from syncopy.shared.errors import SPYValueError, SPYTypeError, SPYWarning
 import syncopy as spy
 
 
 def _get_fooof_signal(nTrials=100, nChannels = 1, nSamples = 1000, seed=None):
     """
@@ -29,15 +29,15 @@
 
     Note: One must perform trial averaging during the FFT to get realistic
     data out of it (and reduce noise). Then work with the averaged data.
 
     Returns AnalogData instance.
     """
     samplerate = 1000
-    ar1_part = AR2_network(AdjMat=np.zeros(nChannels), nSamples=nSamples, alphas=[0.9, 0], nTrials=nTrials, seed=seed)
+    ar1_part = ar2_network(AdjMat=np.zeros(nChannels), nSamples=nSamples, alphas=[0.9, 0], nTrials=nTrials, seed=seed)
     pd1 = phase_diffusion(freq=30., eps=.1, samplerate=samplerate, nChannels=nChannels, nSamples=nSamples, nTrials=nTrials, seed=seed)
     pd2 = phase_diffusion(freq=50., eps=.1, samplerate=samplerate, nChannels=nChannels, nSamples=nSamples, nTrials=nTrials, seed=seed)
     signal = ar1_part + .8 * pd1 + 0.6 * pd2
     return signal
 
 
 class TestMetadataHelpers():
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_packagesetup.py` & `esi_syncopy-2023.5/syncopy/tests/test_packagesetup.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_parsers.py` & `esi_syncopy-2023.5/syncopy/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_plotting.py` & `esi_syncopy-2023.5/syncopy/tests/test_plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 import pytest
 import itertools
 import numpy as np
 import matplotlib.pyplot as ppl
 
 # Local imports
 import syncopy as spy
-import syncopy.tests.synth_data as synth_data
+from syncopy import synthdata
 import syncopy.tests.helpers as helpers
 from syncopy.shared.errors import SPYValueError
 
 
 class TestAnalogPlotting():
 
     nTrials = 10
     nChannels = 9
     nSamples = 300
-    adata = synth_data.AR2_network(nTrials=nTrials,
-                                   AdjMat=np.zeros(nChannels),
-                                   nSamples=nSamples,
-                                   seed=helpers.test_seed)
-
-    adata += 0.3 * synth_data.linear_trend(nTrials=nTrials,
-                                           y_max=nSamples / 20,
-                                           nSamples=nSamples,
-                                           nChannels=nChannels)
+    adata = synthdata.ar2_network(nTrials=nTrials,
+                                  AdjMat=np.zeros(nChannels),
+                                  nSamples=nSamples,
+                                  seed=helpers.test_seed)
+
+    adata += 0.3 * synthdata.linear_trend(nTrials=nTrials,
+                                          y_max=nSamples / 20,
+                                          nSamples=nSamples,
+                                          nChannels=nChannels)
 
 
     # add an offset
     adata = adata + 5
 
     # all trials are equal
     toi_min, toi_max = adata.time[0][0], adata.time[0][-1]
@@ -133,23 +133,23 @@
 
 class TestSpectralPlotting():
 
     nTrials = 10
     nChannels = 4
     nSamples = 300
     AdjMat = np.zeros((nChannels, nChannels))
-    adata = synth_data.AR2_network(nTrials=nTrials,
-                                   AdjMat=AdjMat,
-                                   nSamples=nSamples)
+    adata = synthdata.ar2_network(nTrials=nTrials,
+                                  AdjMat=AdjMat,
+                                  nSamples=nSamples)
 
     # add AR(1) 'background'
-    adata = adata + 1.2 * synth_data.AR2_network(nTrials=nTrials,
-                                                 AdjMat=AdjMat,
-                                                 nSamples=nSamples,
-                                                 alphas=[0.8, 0])
+    adata = adata + 1.2 * synthdata.ar2_network(nTrials=nTrials,
+                                                AdjMat=AdjMat,
+                                                nSamples=nSamples,
+                                                alphas=[0.8, 0])
 
     # some interesting range
     frequency = [1, 400]
 
     # all trials are equal
     toi_min, toi_max = adata.time[0][0], adata.time[0][-1]
 
@@ -259,24 +259,24 @@
 
     nTrials = 40
     nChannels = 4
     nSamples = 400
 
     AdjMat = np.zeros((nChannels, nChannels))
     AdjMat[2, 3] = 0.2   # coupling
-    adata = synth_data.AR2_network(nTrials=nTrials,
-                                   AdjMat=AdjMat,
-                                   nSamples=nSamples)
+    adata = synthdata.ar2_network(nTrials=nTrials,
+                                  AdjMat=AdjMat,
+                                  nSamples=nSamples)
 
     # add 'background'
-    adata = adata + .6 * synth_data.AR2_network(nTrials=nTrials,
-                                                AdjMat=np.zeros((nChannels,
-                                                                 nChannels)),
-                                                nSamples=nSamples,
-                                                alphas=[0.8, 0])
+    adata = adata + .6 * synthdata.ar2_network(nTrials=nTrials,
+                                               AdjMat=np.zeros((nChannels,
+                                                                nChannels)),
+                                               nSamples=nSamples,
+                                               alphas=[0.8, 0])
 
     # some interesting range
     frequency = [1, 400]
 
     # all trials are equal
     toi_min, toi_max = adata.time[0][0], adata.time[0][-1]
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_preproc.py` & `esi_syncopy-2023.5/syncopy/tests/test_preproc.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Local imports
 import dask.distributed as dd
 
 from syncopy import preprocessing as ppfunc
 from syncopy import AnalogData, freqanalysis
 import syncopy.preproc as preproc  # submodule
 import syncopy.tests.helpers as helpers
-from syncopy.tests import synth_data as sd
+from syncopy import synthdata as sd
 
 from syncopy.shared.errors import SPYValueError
 from syncopy.shared.tools import get_defaults, best_match
 
 # Decorator to decide whether or not to run memory-intensive tests
 availMem = psutil.virtual_memory().total
 minRAM = 5
@@ -239,14 +239,37 @@
                 assert np.all(np.imag(htrafo.trials[0]) == 0)
 
         # test wrong hilbert parameter
         with pytest.raises(SPYValueError) as err:
             call(hilbert='absnot')
         assert "one of {'" in str(err)
 
+    def test_but_NaN(self):
+
+        nSamples = 20
+        nTrials = 5
+        nChannels = 3
+
+        # create test data with NaNs in 2 trials
+        arr = [(i + 1) * np.ones((nSamples, nChannels)) for i in range(nTrials)]
+        # add NaNs in 2nd and last trial
+        arr[1][5, 1] = np.nan
+        arr[-1][10:15, 2] = np.nan
+        adata = AnalogData(data=arr, samplerate=50)
+        res = ppfunc(adata,
+                     freq=20,
+                     filter_class='but')
+
+        # IIR filters can't work around NaNs
+        assert np.sum(np.isnan(res.trials[0])) == 0
+        assert np.sum(np.isnan(res.trials[1])) == nSamples
+        assert np.sum(np.isnan(res.trials[4])) == nSamples
+        # check that metadata got propagated
+        assert res.info['nan_trials'] == [1, 4]
+
 
 class TestFIRWS:
 
     nSamples = 1000
     nChannels = 4
     nTrials = 50
     fs = 200
@@ -445,23 +468,58 @@
                 assert np.all(np.imag(htrafo.trials[0]) == 0)
 
         # test wrong hilbert parameter
         with pytest.raises(SPYValueError) as err:
             call(hilbert='absnot')
         assert "one of {'" in str(err)
 
+    def test_firws_NaN(self):
+
+        nSamples = 20
+        nTrials = 5
+        nChannels = 3
+        order = 6  # length of the fir filter
+
+        # create test data with NaNs in 2 trials
+        arr = [(i + 1) * np.ones((nSamples, nChannels)) for i in range(nTrials)]
+        # add NaNs in 2nd and last trial
+        arr[1][5, 1] = np.nan
+        arr[-1][10:15, 2] = np.nan  # "NaN island"
+        adata = AnalogData(data=arr, samplerate=50)
+        res = ppfunc(adata,
+                     freq=20,
+                     filter_class='firws',
+                     order=order,
+                     direction='onepass')
+
+        # no NaNs in 1st trial
+        assert np.sum(np.isnan(res.trials[0])) == 0
+        # we "want" only NaNs in the result, where the filter
+        # support covers/touches the NaN sample(s) in the input
+        # for an isolated NaN this happens exactly for order (filter length) samples
+        assert np.sum(np.isnan(res.trials[1])) == 1 + order
+        # for an island of NaNs, the NaN region
+        # grows in total also by the filter order
+        number_NaN = np.sum(np.isnan(adata.trials[4]))
+        assert np.sum(np.isnan(res.trials[4])) == number_NaN + order
+        # final sanity check
+        assert np.sum(np.isnan(res.trials[4])) < nSamples
+
+        # finally check that the metadata got propagated
+        assert res.info['nan_trials'] == [1, 4]
+
 
 class TestDetrending:
 
     """ Test standalone detrending """
 
     nTrials = 2
     nSamples = 5000
-    AData = sd.linear_trend(nTrials, nSamples=nSamples, y_max=10)
-    AData += sd.white_noise(nTrials, nSamples=nSamples) + 5  # add constant
+    AData = sd.linear_trend(nTrials=2, nSamples=nSamples, y_max=10)
+    AData += sd.white_noise(nTrials=2, nSamples=nSamples) + 5  # add constant
 
     def test_demeaning(self):
 
         res = ppfunc(self.AData, filter_class=None, polyremoval=0)
 
         orig_c0 = self.AData.show(trials=1, channel=0)
         res_c0 = res.show(trials=1, channel=0)
@@ -502,22 +560,59 @@
                      if (inspect.ismethod(getattr(self, attr)) and 'parallel' not in attr)]
 
         for test_name in all_tests:
             test_method = getattr(self, test_name)
             test_method()
         client.close()
 
+    def test_detr_NaN(self):
+
+        nSamples = 20
+        nTrials = 5
+        nChannels = 3
+
+        # create test data with NaNs in 2 trials
+        arr = [(i + 1) * np.ones((nSamples, nChannels)) for i in range(nTrials)]
+        # add NaNs in 2nd and last trial
+        arr[1][5, 1] = np.nan
+        arr[-1][10:15, 2] = np.nan
+        adata = AnalogData(data=arr, samplerate=50)
+
+        # -- demeaning --
+        res = ppfunc(adata,
+                     filter_class=None,
+                     polyremoval=0)
+
+        # detrending can't work around NaNs
+        assert np.sum(np.isnan(res.trials[0])) == 0
+        assert np.sum(np.isnan(res.trials[1])) == nSamples
+        assert np.sum(np.isnan(res.trials[4])) == nSamples
+        # check that metadata got propagated
+        assert res.info['nan_trials'] == [1, 4]
+
+        # -- linear detrending --
+        res = ppfunc(adata,
+                     filter_class=None,
+                     polyremoval=1)
+
+        # detrending can't work around NaNs
+        assert np.sum(np.isnan(res.trials[0])) == 0
+        assert np.sum(np.isnan(res.trials[1])) == nSamples
+        assert np.sum(np.isnan(res.trials[4])) == nSamples
+        # check that metadata got propagated
+        assert res.info['nan_trials'] == [1, 4]
+
 
 class TestStandardize:
 
     """ Test standalone and general zscore """
 
     nTrials = 2
     nSamples = 5000
-    AData = 100 * sd.white_noise(nTrials, nSamples=nSamples) + 5  # add constant
+    AData = 100 * sd.white_noise(nTrials=nTrials, nSamples=nSamples) + 5  # add constant
 
     def test_standardize(self):
 
         res = ppfunc(self.AData, filter_class=None, zscore=True)
 
         orig_c0 = self.AData.show(trials=1, channel=0)
         res_c0 = res.show(trials=1, channel=0)
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_redefinetrial.py` & `esi_syncopy-2023.5/syncopy/tests/test_redefinetrial.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     # longer trial 6 (with overlap)
     trldef[5] = [48, 65, -10]
     irreg_data.trialdefinition = trldef
 
     # check trial lengths in seconds
     assert np.all(np.diff(reg_data.trialintervals) == 0.9)
     assert not np.all(np.diff(irreg_data.trialintervals) == 0.9)
-    # one short trial
+    # # one short trial
     assert np.sum(np.diff(irreg_data.trialintervals) < 0.9) == 1
-    # one long trial
+    # # one long trial
     assert np.sum(np.diff(irreg_data.trialintervals) > 0.9) == 1
 
     def test_user_input(self):
         """ check non compatible arguments are catched """
 
         # offset and trialdef
         with pytest.raises(SPYError, match='Incompatible input arguments'):
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_resampledata.py` & `esi_syncopy-2023.5/syncopy/tests/test_resampledata.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import matplotlib.pyplot as ppl
 
 # Local imports
 import dask.distributed as dd
 
 from syncopy import resampledata, freqanalysis
-import syncopy.tests.synth_data as synth_data
+from syncopy import synthdata
 import syncopy.tests.helpers as helpers
 from syncopy.shared.errors import SPYValueError
 from syncopy.shared.tools import get_defaults
 
 # availableFilterTypes = ('lp', 'hp', 'bp', 'bs')
 
 
@@ -26,19 +26,19 @@
     nSamples = 991
     nChannels = 4
     nTrials = 100
     fs = 200
     fNy = fs / 2
 
     # -- use flat white noise as test data --
-    adata = synth_data.white_noise(nTrials,
-                                   nChannels=nChannels,
-                                   nSamples=nSamples,
-                                   samplerate=fs,
-                                   seed=42)
+    adata = synthdata.white_noise(nTrials=nTrials,
+                                  nChannels=nChannels,
+                                  nSamples=nSamples,
+                                  samplerate=fs,
+                                  seed=42)
 
     # original spectrum
     spec = freqanalysis(adata, tapsmofrq=1, keeptrials=False)
     # mean of the flat spectrum
     pow_orig = spec.show(channel=0)[5:].mean()
 
     # for toi tests, -1s offset
@@ -166,19 +166,19 @@
     nSamples = 1000
     nChannels = 4
     nTrials = 100
     fs = 200
     fNy = fs / 2
 
     # -- use flat white noise as test data --
-    adata = synth_data.white_noise(nTrials,
-                                   nChannels=nChannels,
-                                   nSamples=nSamples,
-                                   samplerate=fs,
-                                   seed=42)
+    adata = synthdata.white_noise(nTrials=nTrials,
+                                  nChannels=nChannels,
+                                  nSamples=nSamples,
+                                  samplerate=fs,
+                                  seed=42)
 
     # original spectrum
     spec = freqanalysis(adata, tapsmofrq=1, keeptrials=False)
     # mean of the flat spectrum
     pow_orig = spec.show(channel=0).mean()
 
     # for toi tests, -1s offset
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_selectdata.py` & `esi_syncopy-2023.5/syncopy/tests/test_selectdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         for selection in valid_selections:
             # instantiate Selector and check attributes
             sel_kwargs, solution = selection
             selector_object = Selector(self.adata, sel_kwargs)
             for sel_kw in sel_kwargs.keys():
                 attr_name = map_sel_attr[sel_kw]
-                assert getattr(selector_object, attr_name) == solution[sel_kw]
+                assert list(getattr(selector_object, attr_name)) == solution[sel_kw]
 
     def test_ad_invalid(self):
 
         # each selection test is a 3-tuple: (selection kwargs, Error, error message sub-string)
         invalid_selections = [
             ({'channel': ["channel33", "channel01"]},
              SPYValueError, "existing names or indices"),
@@ -223,26 +223,30 @@
                 {'frequency': 'all',
                  'taper': 'taper2',
                  'latency': [1.2, 1.7],
                  'trials': np.arange(1, 3)},
                 # the 'solutions'
                 {'frequency': slice(None),
                  'taper': [1],
-                 'latency': [[1], [1]],
+                 'latency': [slice(1, 2, 1), slice(1, 2, 1)],
                  'trials': [1, 2]},
             )
         ]
 
         for selection in valid_selections:
             # instantiate Selector and check attributes
             sel_kwargs, solution = selection
             selector_object = Selector(self.sdata, sel_kwargs)
             for sel_kw in sel_kwargs.keys():
                 attr_name = map_sel_attr[sel_kw]
-                assert getattr(selector_object, attr_name) == solution[sel_kw]
+                res = getattr(selector_object, attr_name)
+                if sel_kw == 'latency':
+                    assert list(res) == solution[sel_kw]
+                else:
+                    assert res == solution[sel_kw]
 
     def test_spectral_invalid(self):
 
         # each selection test is a 3-tuple: (selection kwargs, Error, error message sub-string)
         invalid_selections = [
             ({'frequency': '40Hz'}, SPYValueError, "'all' or `None` or float or list/array"),
             ({'frequency': 4}, SPYValueError, "all array elements to be bounded"),
@@ -330,15 +334,19 @@
 
         for selection in valid_selections:
             # instantiate Selector and check attributes
             sel_kwargs, solution = selection
             selector_object = Selector(self.csd_data, sel_kwargs)
             for sel_kw in sel_kwargs.keys():
                 attr_name = map_sel_attr[sel_kw]
-                assert getattr(selector_object, attr_name) == solution[sel_kw]
+                res = getattr(selector_object, attr_name)
+                if sel_kw == 'latency':
+                    assert list(res) == solution[sel_kw]
+                else:
+                    assert res == solution[sel_kw]
 
     def test_csd_invalid(self):
 
         # each selection test is a 3-tuple: (selection kwargs, Error, error message sub-string)
         invalid_selections = [
             (
                 {'channel_i': [0, 2]}, NotImplementedError,
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_specest.py` & `esi_syncopy-2023.5/syncopy/tests/test_specest.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_specest_fooof.py` & `esi_syncopy-2023.5/syncopy/tests/test_specest_fooof.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_spike_psth.py` & `esi_syncopy-2023.5/syncopy/tests/test_spike_psth.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import pytest
 import dask.distributed as dd
 
 # syncopy imports
 import syncopy as spy
 from syncopy.shared.errors import SPYValueError
-from syncopy.tests import synth_data as sd
+from syncopy import synthdata as sd
 from syncopy.statistics.spike_psth import available_outputs
 
 
 def get_spike_data(nTrials = 10, seed=None):
     return sd.poisson_noise(nTrials,
                             nUnits=3,
                             nChannels=2,
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_spyio.py` & `esi_syncopy-2023.5/syncopy/tests/test_spyio.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_spytools.py` & `esi_syncopy-2023.5/syncopy/tests/test_spytools.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_statistics.py` & `esi_syncopy-2023.5/syncopy/tests/test_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import scipy.stats as st
 
 # Local imports
 import syncopy as spy
 from syncopy.datatype import AnalogData, SpectralData, CrossSpectralData
 from syncopy.shared.errors import SPYValueError, SPYTypeError
 from syncopy.tests import helpers
-from syncopy.tests import synth_data as sd
+from syncopy import synthdata as sd
 from syncopy.statistics import jackknifing as jk
 from syncopy.connectivity.AV_compRoutines import NormalizeCrossSpectra
 
 
 class TestSumStatistics:
 
     # initialize rng instance
@@ -223,22 +223,22 @@
         self.test_selections()
         # should have no effect here
         self.test_trial_statistics()
         client.close()
 
     def test_itc(self, do_plot=True):
 
-        adata = sd.white_noise(100,
+        adata = sd.white_noise(nTrials=100,
                                nSamples=1000,
                                nChannels=2,
                                samplerate=500,
                                seed=42)
 
         # add simple 60Hz armonic
-        adata += sd.harmonic(100,
+        adata += sd.harmonic(nTrials=100,
                              freq=60,
                              nSamples=1000,
                              nChannels=2,
                              samplerate=500)
 
         trials = []
         # add frequency drift along trials
@@ -361,15 +361,15 @@
     def test_jk_csd(self, **kwargs):
         """
         Jackknife cross-spectral densities, here again the trivial average/variance
         yields the same results.
         """
         nTrials = 10
         nSamples = 500
-        adata = 10 * sd.white_noise(nTrials, nSamples=nSamples, seed=helpers.test_seed)
+        adata = 10 * sd.white_noise(nTrials=nTrials, nSamples=nSamples, seed=helpers.test_seed)
         # to test for property propagation
         adata.channel = [f'chV_{i}' for i in range(1, 3)]
 
         # -- still trivial CSDs --
 
         # single trial cross spectra (not densities!)
         cross_spectra = spy.connectivityanalysis(adata,
@@ -410,15 +410,15 @@
         stationary bivariate Gaussian processes, Sandia monograph by Amos and Koopmans(1963)"
         """
 
         nTrials = 50
         nSamples = 1000
         # sufficient to check this entry
         show_kwargs = {'channel_i': 0, 'channel_j': 1}
-        adata = sd.white_noise(nTrials, nSamples=nSamples, seed=helpers.test_seed)
+        adata = sd.white_noise(nTrials=nTrials, nSamples=nSamples, seed=helpers.test_seed)
 
         # confidence for 100 trials from
         # above mentioned publication for squared coherence
         ci95 = {30: 0.98, 50: 0.06, 100: 0.03}
 
         # important to match between
         # replicates and direct estimate!
@@ -537,15 +537,15 @@
 
     def test_jk_granger(self):
 
         AdjMat = np.zeros((2,2))
         # weak coupling 1 -> 0
         AdjMat[1, 0] = 0.025
         nTrials = 35
-        adata = sd.AR2_network(nTrials, AdjMat=AdjMat, seed=42)
+        adata = sd.ar2_network(nTrials=nTrials, AdjMat=AdjMat, seed=42)
         # true causality is at 200Hz
         flims = [190, 210]
 
         # direct estimate
         res = spy.connectivityanalysis(adata, method='granger',
                                        jackknife=True,
                                        tapsmofrq=5)
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_synth_data.py` & `esi_syncopy-2023.5/syncopy/tests/test_synthdata.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,80 +3,129 @@
 # Ensure synthetic data generator functions used in tests work as expected.
 #
 
 # Builtin/3rd party package imports
 import numpy as np
 import pytest
 
-from syncopy.tests.synth_data import white_noise, AR2_network
+from syncopy import AnalogData
+from syncopy.shared.tools import StructDict
+from syncopy.synthdata import collect_trials
+from syncopy.synthdata import white_noise, ar2_network
 from syncopy.shared.errors import SPYValueError
-import syncopy as spy
+
+
+def test_trial_collection():
+    """
+    tests the decorator to construct
+    multi-trial AnalogData from single trial functions
+    """
+
+    # a trivial single trial (np.ndarray) producing function
+    @collect_trials
+    def ones(nChannels, nSamples):
+        return np.ones((nSamples, nChannels))
+
+    cfg = StructDict()
+    cfg.nTrials = 10
+    cfg.samplerate = 12
+    cfg.nChannels = 3
+    cfg.nSamples = 10
+
+    adata = ones(cfg)
+
+    assert isinstance(adata, AnalogData)
+    assert len(adata.trials) == cfg.nTrials
+    assert len(adata.channel) == cfg.nChannels
+    assert len(adata.time[0]) == cfg.nSamples
+    assert adata.samplerate == cfg.samplerate
+
+    # with nTrials=None, the decorator gets bypassed
+    # and returns the single trial array
+    cfg['nTrials'] = None
+    arr = ones(cfg)
+    assert isinstance(arr, np.ndarray)
+    assert arr.shape == (cfg.nSamples, cfg.nChannels)
+
 
 class TestSynthData:
 
-    nTrials=100
+    nTrials = 100
     nChannels = 1
     nSamples = 1000
     samplerate = 1000
 
     def test_white_noise_without_seed(self):
         """Without seed set, the data should not be identical.
            Note: This does not use collect trials.
         """
-        wn1 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, seed=None)
-        wn2 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, seed=None)
+        cfg = StructDict()
+        cfg.nSamples = self.nSamples
+        cfg.nChannels = self.nChannels
+        cfg.nTrials = None
+        # that is the default
+        # cfg.seed = None
+
+        wn1 = white_noise(cfg)
+        wn2 = white_noise(cfg)
         assert isinstance(wn1, np.ndarray)
         assert isinstance(wn2, np.ndarray)
 
         assert not np.allclose(wn1, wn2)
 
     def test_white_noise_with_seed(self):
         """With seed set, the data should be identical.
            Note: This does not use @collect_trials.
         """
-        seed = 42
-        wn1 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, seed=seed)
-        wn2 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, seed=seed)
+        cfg = StructDict()
+        cfg.nSamples = self.nSamples
+        cfg.nChannels = self.nChannels
+        cfg.nTrials = None
+        cfg.seed = 42
+
+        wn1 = white_noise(cfg)
+        wn2 = white_noise(cfg)
+
         assert isinstance(wn1, np.ndarray)
         assert isinstance(wn2, np.ndarray)
 
         assert np.allclose(wn1, wn2)
 
     def test_collect_trials_wn_seed_array(self):
         """Uses @collect_trials."""
         # Trials must differ within an object if seed_per_trial is left at default (true):
         seed = 42
         wn1 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, nTrials=self.nTrials, seed=seed)
-        assert isinstance(wn1, spy.AnalogData)
+        assert isinstance(wn1, AnalogData)
         assert not np.allclose(wn1.show(trials=0), wn1.show(trials=1))
 
         # However, using the same seed for a new instance must lead to identical trials between instances:
         wn2 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, nTrials=self.nTrials, seed=seed)
         assert np.allclose(wn1.show(trials=0), wn2.show(trials=0))
         assert np.allclose(wn1.show(trials=1), wn2.show(trials=1))
 
     def test_collect_trials_wn_seed_scalar(self):
         """Uses @collect_trials."""
         # Trials must be identical within an object if seed_per_trial is False (and a seed is used).
         seed = 42
         wn1 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, nTrials=self.nTrials, seed=seed, seed_per_trial=False)
-        assert isinstance(wn1, spy.AnalogData)
+        assert isinstance(wn1, AnalogData)
         assert np.allclose(wn1.show(trials=0), wn1.show(trials=1))
 
         # And also, using the same scalar seed again should lead to an identical object.
         wn2 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, nTrials=self.nTrials, seed=seed, seed_per_trial=False)
         assert np.allclose(wn1.show(trials=0), wn2.show(trials=0))
         assert np.allclose(wn1.show(trials=1), wn2.show(trials=1))
 
     def test_collect_trials_wn_no_seed(self):
         """Uses @collect_trials."""
         # Trials must differ within an object if seed is None:
         seed = None
         wn1 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, nTrials=self.nTrials, seed=seed)
-        assert isinstance(wn1, spy.AnalogData)
+        assert isinstance(wn1, AnalogData)
         assert not np.allclose(wn1.show(trials=0), wn1.show(trials=1))
 
         # And instances must also differ:
         wn2 = white_noise(nSamples=self.nSamples, nChannels=self.nChannels, nTrials=self.nTrials, seed=seed)
         assert not np.allclose(wn1.show(trials=0), wn2.show(trials=0))
         assert not np.allclose(wn1.show(trials=1), wn2.show(trials=1))
 
@@ -84,28 +133,28 @@
     #### Tests for AR2_network
 
     def test_ar2_without_seed(self):
         """Without seed set, the data should not be identical.
            Note: This does not use collect trials.
         """
         num_channels = 2
-        arn1 = AR2_network(nSamples=self.nSamples, seed=None)  # 2 channels, via default adj matrix
-        arn2 = AR2_network(nSamples=self.nSamples, seed=None)
+        arn1 = ar2_network(nSamples=self.nSamples, seed=None, nTrials=None)  # 2 channels, via default adj matrix
+        arn2 = ar2_network(nSamples=self.nSamples, seed=None, nTrials=None)
         assert isinstance(arn1, np.ndarray)
         assert isinstance(arn2, np.ndarray)
         assert arn1.shape == (self.nSamples, num_channels)
         assert arn2.shape == (self.nSamples, num_channels)
 
         assert not np.allclose(arn1, arn2)
 
     def test_ar2_with_seed(self):
         """With seed set, the data should be identical.
            Note: This does not use collect trials.
         """
         seed = 42
-        arn1 = AR2_network(nSamples=self.nSamples, seed=seed, seed_per_trial=False)
-        arn2 = AR2_network(nSamples=self.nSamples, seed=seed, seed_per_trial=False)
+        arn1 = ar2_network(nSamples=self.nSamples, seed=seed, seed_per_trial=False, nTrials=None)
+        arn2 = ar2_network(nSamples=self.nSamples, seed=seed, seed_per_trial=False, nTrials=None)
 
         assert np.allclose(arn1, arn2)
 
 if __name__ == '__main__':
     T1 = TestSynthData()
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_timelockanalysis.py` & `esi_syncopy-2023.5/syncopy/tests/test_timelockanalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 import pytest
 import dask.distributed as dd
 import h5py
 
 # syncopy imports
 import syncopy as spy
 from syncopy.shared.errors import SPYValueError, SPYTypeError
-from syncopy.tests import synth_data
+from syncopy import synthdata
 
 
 class TestTimelockanalysis:
 
     nTrials = 10
     nChannels = 3
     nSamples = 500
     fs = 200
 
     # create simple white noise
     # "real" data gets created for semantic test
-    adata = synth_data.white_noise(nTrials, samplerate=fs,
-                                   nSamples=nSamples,
-                                   nChannels=nChannels,
-                                   seed=42)
+    adata = synthdata.white_noise(nTrials=nTrials, samplerate=fs,
+                                  nSamples=nSamples,
+                                  nChannels=nChannels,
+                                  seed=42)
 
     # change trial sizes, original interval is [-1, 1.495] seconds
     trldef = adata.trialdefinition
     trldef[1] = [500, 700, -200]  # [-1, -0.005] seconds
     trldef[2] = [680, 960, -20]  # [-0.1, 1.295] seconds
     trldef[3] = [1000, 1200, -100]  # [-0.5, 0.495] seconds
     adata.trialdefinition = trldef
@@ -40,22 +40,22 @@
     overlap = (np.min(adata.trialintervals[:, 1]) -\
         np.max(adata.trialintervals[:, 0])) * fs + 1
 
     def test_timelockanalysis(self):
 
         # create bigger dataset for statistics only here
         # moderate phase diffusion, same initial phase/value!
-        adata = synth_data.phase_diffusion(nTrials=300,
-                                           rand_ini=False,
-                                           samplerate=self.fs,
-                                           nSamples=self.nSamples,
-                                           nChannels=self.nChannels,
-                                           freq=40,
-                                           eps=0.01,
-                                           seed=42)
+        adata = synthdata.phase_diffusion(nTrials=300,
+                                          rand_ini=False,
+                                          samplerate=self.fs,
+                                          nSamples=self.nSamples,
+                                          nChannels=self.nChannels,
+                                          freq=40,
+                                          eps=0.01,
+                                          seed=42)
 
         # change trial sizes, original interval is [-1, 1.495] seconds
         trldef = adata.trialdefinition
         trldef[1] = [500, 700, -200]  # [-1, -0.005] seconds
         trldef[2] = [680, 960, -20]  # [-0.1, 1.295] seconds
         trldef[3] = [1000, 1200, -100]  # [-0.5, 0.495] seconds
         adata.trialdefinition = trldef
```

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_tools.py` & `esi_syncopy-2023.5/syncopy/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `esi_syncopy-2023.3/syncopy/tests/test_welch.py` & `esi_syncopy-2023.5/syncopy/tests/test_welch.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 import numpy as np
 import inspect
 import dask.distributed as dd
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from syncopy.shared.errors import SPYValueError
 from syncopy.shared.const_def import spectralConversions
-import syncopy.tests.synth_data as synth_data
+from syncopy import synthdata
 from syncopy.tests.helpers import teardown, test_seed
 
 
 class TestWelch():
     """
     Test the frontend (user API) for running Welch's method for estimation of power spectra.
     """
 
     # White noise
-    adata = synth_data.white_noise(nTrials=2, nChannels=3, nSamples=20000, samplerate=1000,
-                                   seed=test_seed)
+    adata = synthdata.white_noise(nTrials=2, nChannels=3, nSamples=20000, samplerate=1000,
+                                  seed=test_seed)
     do_plot = True
 
     def setup_class(cls):
         plt.close('all')    # Close plots that are still open.
 
     @staticmethod
     def get_welch_cfg():
@@ -126,15 +126,15 @@
         cfg_with_overlap.toi = 0.8
         cfg_with_overlap.t_ftimwin = 1.2
         cfg_with_overlap.foilim = foilim
         cfg_with_overlap.output = "abs"
 
         nSamples = 30000
         samplerate = 1000
-        wn = synth_data.white_noise(nTrials=1, nChannels=3, nSamples=nSamples, samplerate=samplerate)
+        wn = synthdata.white_noise(nTrials=1, nChannels=3, nSamples=nSamples, samplerate=samplerate)
 
         spec_short_windows = spy.freqanalysis(cfg_no_overlap, wn)
         spec_long_windows = spy.freqanalysis(cfg_with_overlap, wn)
 
         # Check number of windows, we want something similar/comparable.
         assert spec_short_windows.dimord.index('time') == spec_long_windows.dimord.index('time')
         ti = spec_short_windows.dimord.index('time')
@@ -170,16 +170,16 @@
         (Variance can be computed along trials.)
 
         Compare a long signal without overlap versus a short signal with overlap, that result in the
         same window count. We expect to see higher variance for the shorter signal.
 
         Potential nice-to-have for later: investigate sweet spot for the overlap parameter as a function of signal length.
         """
-        wn_long = synth_data.white_noise(nTrials=20, nChannels=1, nSamples=10000, samplerate=1000, seed=42)  # 10 seconds of signal
-        wn_short = synth_data.white_noise(nTrials=20, nChannels=1, nSamples=1000, samplerate=1000, seed=42)  # 1  second of signal
+        wn_long = synthdata.white_noise(nTrials=20, nChannels=1, nSamples=10000, samplerate=1000, seed=42)  # 10 seconds of signal
+        wn_short = synthdata.white_noise(nTrials=20, nChannels=1, nSamples=1000, samplerate=1000, seed=42)  # 1  second of signal
 
         foilim = [5, 200]  # Shared between cases.
 
         cfg_long_no_overlap = TestWelch.get_welch_cfg()  # Results in 100 windows of length 100.
         cfg_long_no_overlap.toi = 0.0         # overlap [0, 1[
         cfg_long_no_overlap.t_ftimwin = 0.1   # window length in sec
         cfg_long_no_overlap.foilim = foilim
@@ -231,15 +231,15 @@
         variances = np.zeros((sig_lengths.size, overlaps.size), dtype=float)  # Filled in loop below.
 
         foilim = [5, 200]  # Shared between cases.
         f_timwin = 0.2
 
         for sigl_idx, sig_len in enumerate(sig_lengths):
             for overl_idx, overlap in enumerate(overlaps):
-                wn = synth_data.white_noise(nTrials=20, nChannels=1, nSamples=sig_len, samplerate=1000, seed=test_seed)
+                wn = synthdata.white_noise(nTrials=20, nChannels=1, nSamples=sig_len, samplerate=1000, seed=test_seed)
 
                 cfg = TestWelch.get_welch_cfg()  # Results in 100 windows of length 100.
                 cfg.toi = overlap
                 cfg.t_ftimwin = f_timwin
                 cfg.foilim = foilim
 
                 spec = spy.freqanalysis(cfg, wn)
```

### Comparing `esi_syncopy-2023.3/PKG-INFO` & `esi_syncopy-2023.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-syncopy
-Version: 2023.3
+Version: 2023.5
 Summary: A toolkit for user-friendly large-scale electrophysiology data analysis. Syncopy is compatible with the Matlab toolbox FieldTrip.
 Home-page: https://syncopy.org
 License: BSD-3-Clause
 Author: Stefan Fürtinger
 Author-email: sfuerti@esi-frankfurt.de
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -98,15 +98,29 @@
 Getting Started
 ===============
 Please visit our `online documentation <http://syncopy.org>`_.
 
 Developer Installation
 -----------------------
 
-To get the latest development version, please clone our GitHub repository:
+To get the latest development version, please clone our GitHub repository and change to the `dev` branch. We highly recommend to install into a new conda virtual environment, so that this development version does not interfere with your existing installation.
 
 .. code-block:: bash
 
    git clone https://github.com/esi-neuroscience/syncopy.git
    cd syncopy/
+   conda env create --name syncopy-dev --file syncopy.yml
+   conda activate syncopy-dev
    pip install -e .
 
+
+We recommend to verify your development installation by running the unit tests. You can skip the parallel tests to save some time, the tests should run in about 5 minutes then:
+
+
+.. code-block:: bash
+
+   python -m pytest -k "not parallel"
+
+
+You now have a verified developer installation of Syncopy. Please refert to our `contributing guide <https://github.com/esi-neuroscience/syncopy/blob/master/CONTRIBUTING.md>`_ if you want to contribute to Syncopy.
+
+
```

