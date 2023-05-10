# Comparing `tmp/mwrpy-0.1.5.tar.gz` & `tmp/mwrpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mwrpy-0.1.5.tar", last modified: Mon May  8 14:28:45 2023, max compression
+gzip compressed data, was "mwrpy-0.1.6.tar", last modified: Wed May 10 12:19:06 2023, max compression
```

## Comparing `mwrpy-0.1.5.tar` & `mwrpy-0.1.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.173237 mwrpy-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 14:28:33.000000 mwrpy-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 14:28:33.000000 mwrpy-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-08 14:28:45.173237 mwrpy-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-08 14:28:33.000000 mwrpy-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.161236 mwrpy-0.1.5/mwrpy/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/atmos.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.165236 mwrpy-0.1.5/mwrpy/level1/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level1/lev1_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level1/met_quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level1/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    48094 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level1/rpg_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level1/write_lev1_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.165236 mwrpy-0.1.5/mwrpy/level2/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level2/get_ret_coeff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level2/lev2_meta_nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level2/lwp_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/level2/write_lev2_nc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.165236 mwrpy-0.1.5/mwrpy/plots/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51855 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/plots/generate_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/plots/plot_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/plots/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/process_mwrpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/rpg_mwr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.165236 mwrpy-0.1.5/mwrpy/site_config/
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/hatpro.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.169237 mwrpy-0.1.5/mwrpy/site_config/hyytiala/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.169237 mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/hyytiala/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.161236 mwrpy-0.1.5/mwrpy/site_config/juelich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.173237 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
--rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 14:28:33.000000 mwrpy-0.1.5/mwrpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:28:45.165236 mwrpy-0.1.5/mwrpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-08 14:28:44.000000 mwrpy-0.1.5/mwrpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-08 14:28:45.000000 mwrpy-0.1.5/mwrpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:28:44.000000 mwrpy-0.1.5/mwrpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 14:28:44.000000 mwrpy-0.1.5/mwrpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 14:28:44.000000 mwrpy-0.1.5/mwrpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:28:45.173237 mwrpy-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-08 14:28:33.000000 mwrpy-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.218681 mwrpy-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 12:18:50.000000 mwrpy-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 12:18:50.000000 mwrpy-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-10 12:19:06.218681 mwrpy-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-10 12:18:50.000000 mwrpy-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/atmos.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1939 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/level1/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/lev1_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/met_quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48094 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/rpg_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level1/write_lev1_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/level2/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/get_ret_coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/lev2_meta_nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/lwp_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/level2/write_lev2_nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51855 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/plots/generate_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/plots/plot_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/plots/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/process_mwrpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/rpg_mwr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/site_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hatpro.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/site_config/hyytiala/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)    33953 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    73995 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    80385 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)    39550 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/hyytiala/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.210681 mwrpy-0.1.6/mwrpy/site_config/juelich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.218681 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 12:18:50.000000 mwrpy-0.1.6/mwrpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:06.214681 mwrpy-0.1.6/mwrpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-05-10 12:19:05.000000 mwrpy-0.1.6/mwrpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-10 12:19:06.000000 mwrpy-0.1.6/mwrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:19:05.000000 mwrpy-0.1.6/mwrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 12:19:05.000000 mwrpy-0.1.6/mwrpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 12:19:05.000000 mwrpy-0.1.6/mwrpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:19:06.218681 mwrpy-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 12:18:50.000000 mwrpy-0.1.6/setup.py
```

### Comparing `mwrpy-0.1.5/LICENSE` & `mwrpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/PKG-INFO` & `mwrpy-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Home-page: https://github.com/actris-cloudnet/mwrpy
 Author: University of Cologne
 Author-email: actris-ccres-mwr@uni-koeln.de
 License: UNKNOWN
 Description: # MWRpy
```

### Comparing `mwrpy-0.1.5/README.md` & `mwrpy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/atmos.py` & `mwrpy-0.1.6/mwrpy/atmos.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/cli.py` & `mwrpy-0.1.6/mwrpy/cli.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/level1/lev1_meta_nc.py` & `mwrpy-0.1.6/mwrpy/level1/lev1_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/level1/met_quality_control.py` & `mwrpy-0.1.6/mwrpy/level1/met_quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/level1/quality_control.py` & `mwrpy-0.1.6/mwrpy/level1/quality_control.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/level1/rpg_bin.py` & `mwrpy-0.1.6/mwrpy/level1/rpg_bin.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/level1/write_lev1_nc.py` & `mwrpy-0.1.6/mwrpy/level1/write_lev1_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/level2/get_ret_coeff.py` & `mwrpy-0.1.6/mwrpy/level2/get_ret_coeff.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/level2/lev2_meta_nc.py` & `mwrpy-0.1.6/mwrpy/level2/lev2_meta_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/level2/lwp_offset.py` & `mwrpy-0.1.6/mwrpy/level2/lwp_offset.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,31 +15,26 @@
     lev1: dict, lwp_org: np.ndarray, index: np.ndarray
 ) -> np.ndarray:
     """This function corrects Lwp offset using the
     2min standard deviation of the 31.4 GHz channel and IR temperature
 
     Args:
         lev1: Level 1 data.
-        lwp: Lwp array.
+        lwp_org: Lwp array.
         index: Index to use.
-        site: site: Name of site.
-
-    Examples:
-        >>> from level2.lwp_offset import correct_lwp_offset
-        >>> correct_lwp_offset(lev1, lwp, index, 'site_name')
     """
 
     if "elevation_angle" in lev1:
         elevation_angle = lev1["elevation_angle"][:]
     else:
         elevation_angle = 90 - lev1["zenith_angle"][:]
 
     lwcl_i, _ = find_lwcl_free(lev1, index)
     lwp = np.copy(lwp_org)
-    lwp[(lwcl_i != 0) | (lwp > 0.04) | (elevation_angle[index] < 89.0)] = np.nan
+    lwp[(lwcl_i != 1) | (lwp > 0.04) | (elevation_angle[index] < 89.0)] = np.nan
     time = lev1["time"][index]
     if max(time) > 25:
         lwp_df = pd.DataFrame({"Lwp": lwp}, index=pd.to_datetime(time, unit="s"))
     else:
         lwp_df = pd.DataFrame({"Lwp": lwp}, index=pd.to_datetime(time, unit="h"))
     lwp_std = lwp_df.rolling("2min", center=True, min_periods=10).std()
     lwp_max = lwp_std.rolling("20min", center=True, min_periods=100).max()
```

### Comparing `mwrpy-0.1.5/mwrpy/level2/write_lev2_nc.py` & `mwrpy-0.1.6/mwrpy/level2/write_lev2_nc.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/plots/generate_plots.py` & `mwrpy-0.1.6/mwrpy/plots/generate_plots.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/plots/plot_meta.py` & `mwrpy-0.1.6/mwrpy/plots/plot_meta.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/plots/plot_utils.py` & `mwrpy-0.1.6/mwrpy/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/process_mwrpy.py` & `mwrpy-0.1.6/mwrpy/process_mwrpy.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/rpg_mwr.py` & `mwrpy-0.1.6/mwrpy/rpg_mwr.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/hatpro.yaml` & `mwrpy-0.1.6/mwrpy/site_config/hatpro.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/HPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/IWV_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/LWP_NN_MA_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/TPB_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret` & `mwrpy-0.1.6/mwrpy/site_config/hyytiala/coefficients/TPT_NN_FI_Hyytiala_v110_v00110_n01.00.ret`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/hyytiala/config.yaml` & `mwrpy-0.1.6/mwrpy/site_config/hyytiala/config.yaml`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/hpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/iwv_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/lwp_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_01.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_02.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_03.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_04.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_05.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_06.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_07.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_08.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_09.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_10.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_11.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_12.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tbx_deb_rt00_90_13.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tpb_deb_rt00.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc` & `mwrpy-0.1.6/mwrpy/site_config/juelich/coefficients/tpt_deb_rt00_90.nc`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy/utils.py` & `mwrpy-0.1.6/mwrpy/utils.py`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/mwrpy.egg-info/PKG-INFO` & `mwrpy-0.1.6/mwrpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwrpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for Microwave Radiometer processing in ACTRIS
 Home-page: https://github.com/actris-cloudnet/mwrpy
 Author: University of Cologne
 Author-email: actris-ccres-mwr@uni-koeln.de
 License: UNKNOWN
 Description: # MWRpy
```

### Comparing `mwrpy-0.1.5/mwrpy.egg-info/SOURCES.txt` & `mwrpy-0.1.6/mwrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mwrpy-0.1.5/setup.py` & `mwrpy-0.1.6/setup.py`

 * *Files identical despite different names*

