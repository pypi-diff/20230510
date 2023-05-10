# Comparing `tmp/exchange_calendars-4.2.6.tar.gz` & `tmp/exchange_calendars-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars-4.2.6.tar", last modified: Sun Apr  9 08:25:16 2023, max compression
+gzip compressed data, was "exchange_calendars-4.2.7.tar", last modified: Wed May 10 02:13:46 2023, max compression
```

## Comparing `exchange_calendars-4.2.6.tar` & `exchange_calendars-4.2.7.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.742903 exchange_calendars-4.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-04-09 08:25:16.742903 exchange_calendars-4.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.678897 exchange_calendars-4.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/changes_archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.678897 exchange_calendars-4.2.6/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    91635 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/calendar_methods.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37097 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/calendar_properties.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/minutes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/sessions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   149635 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/docs/tutorials/trading_index.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.678897 exchange_calendars-4.2.6/etc/
--rw-r--r--   0 runner    (1001) docker     (123)   141885 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/NYSE-Historical-Closings.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/check_holidays.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/ecal
--rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/factory_bounds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50169 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/lunisolar
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/make_exchange_calendar_test_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements_lunisolar.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements_minpandas.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/requirements_update_xkrx_holidays.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/etc/update_xkrx_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.690898 exchange_calendars-4.2.6/exchange_calendars/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/always_open.py
--rw-r--r--   0 runner    (1001) docker     (123)    24837 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/calendar_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/calendar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/common_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/ecal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   108025 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_aixk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_asex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_bvmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_cmes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_iepa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xasx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbkk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xcbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xcse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xdub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xfra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xhel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xhkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xjse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkls.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkrx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xnys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xnze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xosl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xpar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xpra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xsgo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xshg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xsto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xswx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtae.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xwar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xwbo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/lunisolar_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.690898 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/korean_holiday.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/offsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/precomputed_exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/tase_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/us_futures_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/us_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.690898 exchange_calendars-4.2.6/exchange_calendars/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/weekday_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/xbkk_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/xkls_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/xkrx_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/exchange_calendars/xtks_holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.690898 exchange_calendars-4.2.6/exchange_calendars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 08:25:16.000000 exchange_calendars-4.2.6/exchange_calendars.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-09 08:25:16.742903 exchange_calendars-4.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.702899 exchange_calendars-4.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:25:16.742903 exchange_calendars-4.2.6/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/24-5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/24-7.csv
--rw-r--r--   0 runner    (1001) docker     (123)   110144 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/aixk.csv
--rw-r--r--   0 runner    (1001) docker     (123)   496439 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/asex.csv
--rw-r--r--   0 runner    (1001) docker     (123)   537779 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/bvmf.csv
--rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/cmes.csv
--rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/iepa.csv
--rw-r--r--   0 runner    (1001) docker     (123)   114134 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)   492279 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xams.csv
--rw-r--r--   0 runner    (1001) docker     (123)   560074 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xasx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   494164 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbkk.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486819 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbog.csv
--rw-r--r--   0 runner    (1001) docker     (123)   418309 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbom.csv
--rw-r--r--   0 runner    (1001) docker     (123)   492344 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbru.csv
--rw-r--r--   0 runner    (1001) docker     (123)   530954 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499559 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbud.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498389 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xbue.csv
--rw-r--r--   0 runner    (1001) docker     (123)   547139 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xcbf.csv
--rw-r--r--   0 runner    (1001) docker     (123)   484804 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xcse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   507099 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xdub.csv
--rw-r--r--   0 runner    (1001) docker     (123)   552404 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xetr.csv
--rw-r--r--   0 runner    (1001) docker     (123)   551104 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xfra.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486559 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xhel.csv
--rw-r--r--   0 runner    (1001) docker     (123)   868914 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xhkg.csv
--rw-r--r--   0 runner    (1001) docker     (123)   145764 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xice.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500014 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xidx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   502614 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xist.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499819 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xjse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   504889 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xkar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   499299 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xkls.csv
--rw-r--r--   0 runner    (1001) docker     (123)   793869 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xkrx.csv
--rw-r--r--   0 runner    (1001) docker     (123)   501444 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xlim.csv
--rw-r--r--   0 runner    (1001) docker     (123)   488119 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xlis.csv
--rw-r--r--   0 runner    (1001) docker     (123)   553509 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xlon.csv
--rw-r--r--   0 runner    (1001) docker     (123)   541224 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xmad.csv
--rw-r--r--   0 runner    (1001) docker     (123)   503979 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xmex.csv
--rw-r--r--   0 runner    (1001) docker     (123)   490784 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xmil.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xmos.csv
--rw-r--r--   0 runner    (1001) docker     (123)   541094 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xnys.csv
--rw-r--r--   0 runner    (1001) docker     (123)   550909 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xnze.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486299 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xosl.csv
--rw-r--r--   0 runner    (1001) docker     (123)   493059 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xpar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   504694 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xphs.csv
--rw-r--r--   0 runner    (1001) docker     (123)   501184 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xpra.csv
--rw-r--r--   0 runner    (1001) docker     (123)   618964 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xses.csv
--rw-r--r--   0 runner    (1001) docker     (123)   498714 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xsgo.csv
--rw-r--r--   0 runner    (1001) docker     (123)   855469 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xshg.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xsto.csv
--rw-r--r--   0 runner    (1001) docker     (123)   485129 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xswx.csv
--rw-r--r--   0 runner    (1001) docker     (123)    79204 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xtae.csv
--rw-r--r--   0 runner    (1001) docker     (123)   548374 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xtai.csv
--rw-r--r--   0 runner    (1001) docker     (123)   617749 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xtks.csv
--rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xtse.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500989 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xwar.csv
--rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/resources/xwbo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_aixk_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_always_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_asex_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_bvmf_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_calendar_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_calendar_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_cmes_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)   162253 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_iepa_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_weekday_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xams_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xasx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbkk_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbog_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbom_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbru_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbud_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xbue_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xcbf_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xcse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xdub_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xetr_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xfra_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xhel_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xhkg_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xice_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xidx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xist_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xjse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xkar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xkls_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xkrx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xlim_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xlis_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xlon_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xmad_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xmex_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xmil_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xmos_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xnys_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xnze_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xosl_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xpar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xphs_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xpra_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xses_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xsgo_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xshg_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xsto_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xswx_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xtae_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xtai_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xtks_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xtse_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xwar_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-09 08:25:04.000000 exchange_calendars-4.2.6/tests/test_xwbo_calendar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.096064 exchange_calendars-4.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-05-10 02:13:46.096064 exchange_calendars-4.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24250 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:45.988055 exchange_calendars-4.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/changes_archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:45.992056 exchange_calendars-4.2.7/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    91635 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/calendar_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37097 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/calendar_properties.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/minutes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/sessions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   149635 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/docs/tutorials/trading_index.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:45.996056 exchange_calendars-4.2.7/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)   141885 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/NYSE-Historical-Closings.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/check_holidays.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3854 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/ecal
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/factory_bounds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50169 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/lunisolar
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/make_exchange_calendar_test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements_lunisolar.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements_minpandas.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/requirements_update_xkrx_holidays.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/etc/update_xkrx_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.028059 exchange_calendars-4.2.7/exchange_calendars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/always_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24837 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/calendar_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20100 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/calendar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/common_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/ecal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108025 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_aixk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_asex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_bvmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_cmes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_iepa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xasx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbkk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xcbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xcse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xdub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xfra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xhel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xhkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xjse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xnys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xnze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xosl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xpar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xpra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xsgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xshg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xsto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xswx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xwar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xwbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/lunisolar_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.032059 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/korean_holiday.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/offsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/precomputed_exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/tase_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/us_futures_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/us_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.032059 exchange_calendars-4.2.7/exchange_calendars/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/weekday_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/xbkk_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12755 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/xkls_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34830 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/xkrx_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/exchange_calendars/xtks_holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.032059 exchange_calendars-4.2.7/exchange_calendars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38414 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 02:13:45.000000 exchange_calendars-4.2.7/exchange_calendars.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 02:13:46.096064 exchange_calendars-4.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.044060 exchange_calendars-4.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:13:46.096064 exchange_calendars-4.2.7/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/24-5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/24-7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   110144 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/aixk.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   496439 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/asex.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   537779 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/bvmf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/cmes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   461924 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/iepa.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   114134 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   492279 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xams.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   560074 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xasx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   494164 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbkk.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486819 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbog.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   418309 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbom.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   492344 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbru.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   530954 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499559 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbud.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498389 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xbue.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   547139 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xcbf.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   484804 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xcse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   507099 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xdub.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   552404 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xetr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   551104 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xfra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486559 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xhel.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   868914 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xhkg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   145764 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500014 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xidx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502614 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499819 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xjse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   504889 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xkar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   499299 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xkls.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   793869 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xkrx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   501444 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xlim.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   488119 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xlis.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   553509 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xlon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   541224 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xmad.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   503979 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xmex.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   490784 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xmil.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500079 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xmos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   541094 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xnys.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   550909 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xnze.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486299 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xosl.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   493059 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xpar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   504694 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xphs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   501184 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xpra.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   618964 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xses.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   498714 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xsgo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   855469 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xshg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xsto.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   485129 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xswx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    79204 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xtae.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   548374 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xtai.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   617749 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xtks.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   486494 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xtse.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   500989 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xwar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   555134 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/resources/xwbo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_aixk_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_always_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_asex_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_bvmf_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_calendar_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69070 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_calendar_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_cmes_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162253 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_iepa_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_weekday_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xams_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xasx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbkk_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbog_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbom_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbru_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbud_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xbue_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xcbf_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xcse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xdub_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xetr_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xfra_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xhel_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xhkg_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xice_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xidx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xist_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xjse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xkar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xkls_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xkrx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xlim_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xlis_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xlon_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xmad_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xmex_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xmil_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xmos_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xnys_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xnze_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xosl_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xpar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xphs_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xpra_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xses_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8517 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xsgo_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xshg_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xsto_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xswx_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xtae_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xtai_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xtks_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xtse_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xwar_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-10 02:13:30.000000 exchange_calendars-4.2.7/tests/test_xwbo_calendar.py
```

### Comparing `exchange_calendars-4.2.6/.gitignore` & `exchange_calendars-4.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/LICENSE` & `exchange_calendars-4.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/PKG-INFO` & `exchange_calendars-4.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange_calendars
-Version: 4.2.6
+Version: 4.2.7
 Summary: Calendars for securities exchanges
 Author: Gerry Manoim
 Author-email: gerrymanoim@gmail.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `exchange_calendars-4.2.6/README.md` & `exchange_calendars-4.2.7/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/docs/changes_archive.md` & `exchange_calendars-4.2.7/docs/changes_archive.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/docs/tutorials/calendar_methods.ipynb` & `exchange_calendars-4.2.7/docs/tutorials/calendar_methods.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/docs/tutorials/calendar_properties.ipynb` & `exchange_calendars-4.2.7/docs/tutorials/calendar_properties.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/docs/tutorials/minutes.ipynb` & `exchange_calendars-4.2.7/docs/tutorials/minutes.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/docs/tutorials/sessions.ipynb` & `exchange_calendars-4.2.7/docs/tutorials/sessions.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/docs/tutorials/trading_index.ipynb` & `exchange_calendars-4.2.7/docs/tutorials/trading_index.ipynb`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/NYSE-Historical-Closings.pdf` & `exchange_calendars-4.2.7/etc/NYSE-Historical-Closings.pdf`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/bench.py` & `exchange_calendars-4.2.7/etc/bench.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/check_holidays.py` & `exchange_calendars-4.2.7/etc/check_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/ecal` & `exchange_calendars-4.2.7/etc/ecal`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/factory_bounds.py` & `exchange_calendars-4.2.7/etc/factory_bounds.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/lunisolar` & `exchange_calendars-4.2.7/etc/lunisolar`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/make_exchange_calendar_test_csv.py` & `exchange_calendars-4.2.7/etc/make_exchange_calendar_test_csv.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/requirements.txt` & `exchange_calendars-4.2.7/etc/requirements.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/requirements_dev.txt` & `exchange_calendars-4.2.7/etc/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/requirements_minpandas.txt` & `exchange_calendars-4.2.7/etc/requirements_minpandas.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/etc/update_xkrx_holidays.py` & `exchange_calendars-4.2.7/etc/update_xkrx_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/__init__.py` & `exchange_calendars-4.2.7/exchange_calendars/__init__.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/calendar_helpers.py` & `exchange_calendars-4.2.7/exchange_calendars/calendar_helpers.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/calendar_utils.py` & `exchange_calendars-4.2.7/exchange_calendars/calendar_utils.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/common_holidays.py` & `exchange_calendars-4.2.7/exchange_calendars/common_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/ecal.py` & `exchange_calendars-4.2.7/exchange_calendars/ecal.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     start = "{year}-{month}".format(year=year, month=month)
     if month == 12:
         end = "{year}-{month}".format(year=year + 1, month=1)
     else:
         end = "{year}-{month}".format(year=year, month=month + 1)
 
-    days = pd.date_range(start, end, closed="left")
+    days = pd.date_range(start, end, inclusive="left")
 
     title = months[month - 1]
     if print_year:
         title += " {year}".format(year=year)
 
     print("{title:^28}".format(title=title).rstrip(), file=out)
     print(" Su  Mo  Tu  We  Th  Fr  Sa", file=out)
```

### Comparing `exchange_calendars-4.2.6/exchange_calendars/errors.py` & `exchange_calendars-4.2.7/exchange_calendars/errors.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_aixk.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_aixk.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_asex.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_asex.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_bvmf.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_bvmf.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_cmes.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_cmes.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_iepa.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_iepa.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xams.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xams.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xasx.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xasx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbkk.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbkk.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbog.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbog.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbom.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbom.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbru.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbru.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbse.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbud.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbud.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xbue.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xbue.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xcbf.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xcbf.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xcse.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xcse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xdub.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xdub.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xetr.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xetr.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xfra.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xfra.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xhel.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xhel.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xhkg.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xhkg.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xice.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xice.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xidx.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xidx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xist.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xist.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xjse.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xjse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkar.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkls.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkls.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xkrx.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xkrx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlim.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlim.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlis.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlis.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xlon.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xlon.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmad.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmad.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmex.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmex.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmil.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmil.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xmos.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xmos.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xnys.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xnys.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xnze.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xnze.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xosl.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xosl.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xpar.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xpar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xphs.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xphs.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xpra.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xpra.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xses.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xses.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xsgo.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xsgo.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xshg.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xshg.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xsto.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xsto.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xswx.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xswx.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtae.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtae.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtai.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtai.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtks.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtks.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xtse.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xtse.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xwar.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xwar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/exchange_calendar_xwbo.py` & `exchange_calendars-4.2.7/exchange_calendars/exchange_calendar_xwbo.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .exchange_calendar import HolidayCalendar, ExchangeCalendar
 
 NewYearsDay = new_years_day()
 
 Epiphany = epiphany(end_date="2019")
 
 AscensionDay = ascension_day(end_date="2019")
-WhitMonday = whit_monday()
+WhitMonday = whit_monday(end_date="2023")
 CorpusChristi = corpus_christi(end_date="2019")
 
 LabourDay = european_labour_day()
 
 AssumptionDay = assumption_day(end_date="2019")
 
 NationalHoliday = Holiday("National Holiday", month=10, day=26)
```

### Comparing `exchange_calendars-4.2.6/exchange_calendars/lunisolar_holidays.py` & `exchange_calendars-4.2.7/exchange_calendars/lunisolar_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/holiday.py` & `exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/korean_holiday.py` & `exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/korean_holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/pandas_extensions/offsets.py` & `exchange_calendars-4.2.7/exchange_calendars/pandas_extensions/offsets.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/precomputed_exchange_calendar.py` & `exchange_calendars-4.2.7/exchange_calendars/precomputed_exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/tase_holidays.py` & `exchange_calendars-4.2.7/exchange_calendars/tase_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/us_futures_calendar.py` & `exchange_calendars-4.2.7/exchange_calendars/us_futures_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/us_holidays.py` & `exchange_calendars-4.2.7/exchange_calendars/us_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/utils/pandas_utils.py` & `exchange_calendars-4.2.7/exchange_calendars/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/xbkk_holidays.py` & `exchange_calendars-4.2.7/exchange_calendars/xbkk_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/xkls_holidays.py` & `exchange_calendars-4.2.7/exchange_calendars/xkls_holidays.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         "2016-12-11",
         "2017-12-01",
         "2018-11-20",
         "2019-11-09",
         "2020-10-29",
         "2021-10-19",
         "2022-10-09",
-        "2023-09-27",
+        "2023-09-28",
         "2024-09-15",
         "2025-09-04",
         "2026-08-25",
         "2027-08-14",
         "2028-08-03",
         "2029-07-24",
         "2030-07-13",
@@ -247,15 +247,15 @@
         "2016-07-06",
         "2017-06-25",
         "2018-06-15",
         "2019-06-05",
         "2020-05-24",
         "2021-05-13",
         "2022-05-03",
-        "2023-04-21",
+        "2023-04-22",
         "2024-04-10",
         "2025-03-30",
         "2026-03-20",
         "2027-03-09",
         "2028-02-26",
         "2029-02-14",
         "2030-02-04",
@@ -324,15 +324,15 @@
         "2016-09-12",
         "2017-09-01",
         "2018-08-22",
         "2019-08-11",
         "2020-07-31",
         "2021-07-20",
         "2022-07-10",
-        "2023-06-28",
+        "2023-06-29",
         "2024-06-16",
         "2025-06-06",
         "2026-05-27",
         "2027-05-16",
         "2028-05-05",
         "2029-04-24",
         "2030-04-13",
@@ -376,15 +376,15 @@
         "2015-11-10",
         "2017-10-18",
         "2018-11-06",
         "2019-10-28",
         "2020-11-14",
         "2021-11-04",
         "2022-10-24",
-        "2023-11-12",
+        "2023-11-13",
         "2024-10-31",
     ]
 )
 
 # Malaysia's observances of Thaipusam (Tamil Calendar)
 thaipusam = pd.to_datetime(
     [
@@ -434,14 +434,15 @@
     ]
 )
 
 misc_adhoc = pd.to_datetime(
     [
         "2024-06-03",  # Yang di-Pertuan Agong's Birthday
         "2023-06-05",  # Yang di-Pertuan Agong's Birthday
+        "2023-04-21",  # Special Public Holiday's announced by Anwar
         "2022-06-06",  # Yang di-Pertuan Agong's Birthday
         "2021-06-07",  # Yang di-Pertuan Agong's Birthday
         "2020-06-08",  # Yang di-Pertuan Agong's Birthday
         "2019-09-09",  # Yang di-Pertuan Agong's Birthday
         "2019-07-30",  # Installation of Yang di-Pertuan Agong
         "2018-09-10",  # Yang di-Pertuan Agong's Birthday
         "2018-05-11",  # Special Holiday (probably post election holiday?)
```

### Comparing `exchange_calendars-4.2.6/exchange_calendars/xkrx_holidays.py` & `exchange_calendars-4.2.7/exchange_calendars/xkrx_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars/xtks_holidays.py` & `exchange_calendars-4.2.7/exchange_calendars/xtks_holidays.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/exchange_calendars.egg-info/PKG-INFO` & `exchange_calendars-4.2.7/exchange_calendars.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange-calendars
-Version: 4.2.6
+Version: 4.2.7
 Summary: Calendars for securities exchanges
 Author: Gerry Manoim
 Author-email: gerrymanoim@gmail.com
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `exchange_calendars-4.2.6/exchange_calendars.egg-info/SOURCES.txt` & `exchange_calendars-4.2.7/exchange_calendars.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/pyproject.toml` & `exchange_calendars-4.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/setup.cfg` & `exchange_calendars-4.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/24-5.csv` & `exchange_calendars-4.2.7/tests/resources/24-5.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/24-7.csv` & `exchange_calendars-4.2.7/tests/resources/24-7.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/aixk.csv` & `exchange_calendars-4.2.7/tests/resources/aixk.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/asex.csv` & `exchange_calendars-4.2.7/tests/resources/asex.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/bvmf.csv` & `exchange_calendars-4.2.7/tests/resources/bvmf.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/cmes.csv` & `exchange_calendars-4.2.7/tests/resources/cmes.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/iepa.csv` & `exchange_calendars-4.2.7/tests/resources/iepa.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/test.csv` & `exchange_calendars-4.2.7/tests/resources/test.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xams.csv` & `exchange_calendars-4.2.7/tests/resources/xams.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xasx.csv` & `exchange_calendars-4.2.7/tests/resources/xasx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xbkk.csv` & `exchange_calendars-4.2.7/tests/resources/xbkk.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xbog.csv` & `exchange_calendars-4.2.7/tests/resources/xbog.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xbom.csv` & `exchange_calendars-4.2.7/tests/resources/xbom.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xbru.csv` & `exchange_calendars-4.2.7/tests/resources/xbru.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xbse.csv` & `exchange_calendars-4.2.7/tests/resources/xbse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xbud.csv` & `exchange_calendars-4.2.7/tests/resources/xbud.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xbue.csv` & `exchange_calendars-4.2.7/tests/resources/xbue.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xcbf.csv` & `exchange_calendars-4.2.7/tests/resources/xcbf.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xcse.csv` & `exchange_calendars-4.2.7/tests/resources/xcse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xdub.csv` & `exchange_calendars-4.2.7/tests/resources/xdub.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xetr.csv` & `exchange_calendars-4.2.7/tests/resources/xetr.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xfra.csv` & `exchange_calendars-4.2.7/tests/resources/xfra.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xhel.csv` & `exchange_calendars-4.2.7/tests/resources/xhel.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xhkg.csv` & `exchange_calendars-4.2.7/tests/resources/xhkg.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xice.csv` & `exchange_calendars-4.2.7/tests/resources/xice.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xidx.csv` & `exchange_calendars-4.2.7/tests/resources/xidx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xist.csv` & `exchange_calendars-4.2.7/tests/resources/xist.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xjse.csv` & `exchange_calendars-4.2.7/tests/resources/xjse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xkar.csv` & `exchange_calendars-4.2.7/tests/resources/xkar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xkls.csv` & `exchange_calendars-4.2.7/tests/resources/xkls.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xkrx.csv` & `exchange_calendars-4.2.7/tests/resources/xkrx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xlim.csv` & `exchange_calendars-4.2.7/tests/resources/xlim.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xlis.csv` & `exchange_calendars-4.2.7/tests/resources/xlis.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xlon.csv` & `exchange_calendars-4.2.7/tests/resources/xlon.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xmad.csv` & `exchange_calendars-4.2.7/tests/resources/xmad.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xmex.csv` & `exchange_calendars-4.2.7/tests/resources/xmex.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xmil.csv` & `exchange_calendars-4.2.7/tests/resources/xmil.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xmos.csv` & `exchange_calendars-4.2.7/tests/resources/xmos.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xnys.csv` & `exchange_calendars-4.2.7/tests/resources/xnys.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xnze.csv` & `exchange_calendars-4.2.7/tests/resources/xnze.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xosl.csv` & `exchange_calendars-4.2.7/tests/resources/xosl.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xpar.csv` & `exchange_calendars-4.2.7/tests/resources/xpar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xphs.csv` & `exchange_calendars-4.2.7/tests/resources/xphs.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xpra.csv` & `exchange_calendars-4.2.7/tests/resources/xpra.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xses.csv` & `exchange_calendars-4.2.7/tests/resources/xses.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xsgo.csv` & `exchange_calendars-4.2.7/tests/resources/xsgo.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xshg.csv` & `exchange_calendars-4.2.7/tests/resources/xshg.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xsto.csv` & `exchange_calendars-4.2.7/tests/resources/xsto.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xswx.csv` & `exchange_calendars-4.2.7/tests/resources/xswx.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xtae.csv` & `exchange_calendars-4.2.7/tests/resources/xtae.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xtai.csv` & `exchange_calendars-4.2.7/tests/resources/xtai.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xtks.csv` & `exchange_calendars-4.2.7/tests/resources/xtks.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xtse.csv` & `exchange_calendars-4.2.7/tests/resources/xtse.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xwar.csv` & `exchange_calendars-4.2.7/tests/resources/xwar.csv`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/resources/xwbo.csv` & `exchange_calendars-4.2.7/tests/resources/xwbo.csv`

 * *Files 2% similar despite different names*

```diff
@@ -7688,7 +7688,854 @@
 2020-12-21T00:00:00Z,2020-12-21T08:00:00Z,2020-12-21T16:30:00Z,,
 2020-12-22T00:00:00Z,2020-12-22T08:00:00Z,2020-12-22T16:30:00Z,,
 2020-12-23T00:00:00Z,2020-12-23T08:00:00Z,2020-12-23T16:30:00Z,,
 2020-12-28T00:00:00Z,2020-12-28T08:00:00Z,2020-12-28T16:30:00Z,,
 2020-12-29T00:00:00Z,2020-12-29T08:00:00Z,2020-12-29T16:30:00Z,,
 2020-12-30T00:00:00Z,2020-12-30T08:00:00Z,2020-12-30T13:15:00Z,,
 2021-01-04T00:00:00Z,2021-01-04T08:00:00Z,2021-01-04T16:30:00Z,,
+2021-01-05T00:00:00Z,2021-01-05T08:00:00Z,2021-01-05T16:30:00Z,,
+2021-01-06T00:00:00Z,2021-01-06T08:00:00Z,2021-01-06T16:30:00Z,,
+2021-01-07T00:00:00Z,2021-01-07T08:00:00Z,2021-01-07T16:30:00Z,,
+2021-01-08T00:00:00Z,2021-01-08T08:00:00Z,2021-01-08T16:30:00Z,,
+2021-01-11T00:00:00Z,2021-01-11T08:00:00Z,2021-01-11T16:30:00Z,,
+2021-01-12T00:00:00Z,2021-01-12T08:00:00Z,2021-01-12T16:30:00Z,,
+2021-01-13T00:00:00Z,2021-01-13T08:00:00Z,2021-01-13T16:30:00Z,,
+2021-01-14T00:00:00Z,2021-01-14T08:00:00Z,2021-01-14T16:30:00Z,,
+2021-01-15T00:00:00Z,2021-01-15T08:00:00Z,2021-01-15T16:30:00Z,,
+2021-01-18T00:00:00Z,2021-01-18T08:00:00Z,2021-01-18T16:30:00Z,,
+2021-01-19T00:00:00Z,2021-01-19T08:00:00Z,2021-01-19T16:30:00Z,,
+2021-01-20T00:00:00Z,2021-01-20T08:00:00Z,2021-01-20T16:30:00Z,,
+2021-01-21T00:00:00Z,2021-01-21T08:00:00Z,2021-01-21T16:30:00Z,,
+2021-01-22T00:00:00Z,2021-01-22T08:00:00Z,2021-01-22T16:30:00Z,,
+2021-01-25T00:00:00Z,2021-01-25T08:00:00Z,2021-01-25T16:30:00Z,,
+2021-01-26T00:00:00Z,2021-01-26T08:00:00Z,2021-01-26T16:30:00Z,,
+2021-01-27T00:00:00Z,2021-01-27T08:00:00Z,2021-01-27T16:30:00Z,,
+2021-01-28T00:00:00Z,2021-01-28T08:00:00Z,2021-01-28T16:30:00Z,,
+2021-01-29T00:00:00Z,2021-01-29T08:00:00Z,2021-01-29T16:30:00Z,,
+2021-02-01T00:00:00Z,2021-02-01T08:00:00Z,2021-02-01T16:30:00Z,,
+2021-02-02T00:00:00Z,2021-02-02T08:00:00Z,2021-02-02T16:30:00Z,,
+2021-02-03T00:00:00Z,2021-02-03T08:00:00Z,2021-02-03T16:30:00Z,,
+2021-02-04T00:00:00Z,2021-02-04T08:00:00Z,2021-02-04T16:30:00Z,,
+2021-02-05T00:00:00Z,2021-02-05T08:00:00Z,2021-02-05T16:30:00Z,,
+2021-02-08T00:00:00Z,2021-02-08T08:00:00Z,2021-02-08T16:30:00Z,,
+2021-02-09T00:00:00Z,2021-02-09T08:00:00Z,2021-02-09T16:30:00Z,,
+2021-02-10T00:00:00Z,2021-02-10T08:00:00Z,2021-02-10T16:30:00Z,,
+2021-02-11T00:00:00Z,2021-02-11T08:00:00Z,2021-02-11T16:30:00Z,,
+2021-02-12T00:00:00Z,2021-02-12T08:00:00Z,2021-02-12T16:30:00Z,,
+2021-02-15T00:00:00Z,2021-02-15T08:00:00Z,2021-02-15T16:30:00Z,,
+2021-02-16T00:00:00Z,2021-02-16T08:00:00Z,2021-02-16T16:30:00Z,,
+2021-02-17T00:00:00Z,2021-02-17T08:00:00Z,2021-02-17T16:30:00Z,,
+2021-02-18T00:00:00Z,2021-02-18T08:00:00Z,2021-02-18T16:30:00Z,,
+2021-02-19T00:00:00Z,2021-02-19T08:00:00Z,2021-02-19T16:30:00Z,,
+2021-02-22T00:00:00Z,2021-02-22T08:00:00Z,2021-02-22T16:30:00Z,,
+2021-02-23T00:00:00Z,2021-02-23T08:00:00Z,2021-02-23T16:30:00Z,,
+2021-02-24T00:00:00Z,2021-02-24T08:00:00Z,2021-02-24T16:30:00Z,,
+2021-02-25T00:00:00Z,2021-02-25T08:00:00Z,2021-02-25T16:30:00Z,,
+2021-02-26T00:00:00Z,2021-02-26T08:00:00Z,2021-02-26T16:30:00Z,,
+2021-03-01T00:00:00Z,2021-03-01T08:00:00Z,2021-03-01T16:30:00Z,,
+2021-03-02T00:00:00Z,2021-03-02T08:00:00Z,2021-03-02T16:30:00Z,,
+2021-03-03T00:00:00Z,2021-03-03T08:00:00Z,2021-03-03T16:30:00Z,,
+2021-03-04T00:00:00Z,2021-03-04T08:00:00Z,2021-03-04T16:30:00Z,,
+2021-03-05T00:00:00Z,2021-03-05T08:00:00Z,2021-03-05T16:30:00Z,,
+2021-03-08T00:00:00Z,2021-03-08T08:00:00Z,2021-03-08T16:30:00Z,,
+2021-03-09T00:00:00Z,2021-03-09T08:00:00Z,2021-03-09T16:30:00Z,,
+2021-03-10T00:00:00Z,2021-03-10T08:00:00Z,2021-03-10T16:30:00Z,,
+2021-03-11T00:00:00Z,2021-03-11T08:00:00Z,2021-03-11T16:30:00Z,,
+2021-03-12T00:00:00Z,2021-03-12T08:00:00Z,2021-03-12T16:30:00Z,,
+2021-03-15T00:00:00Z,2021-03-15T08:00:00Z,2021-03-15T16:30:00Z,,
+2021-03-16T00:00:00Z,2021-03-16T08:00:00Z,2021-03-16T16:30:00Z,,
+2021-03-17T00:00:00Z,2021-03-17T08:00:00Z,2021-03-17T16:30:00Z,,
+2021-03-18T00:00:00Z,2021-03-18T08:00:00Z,2021-03-18T16:30:00Z,,
+2021-03-19T00:00:00Z,2021-03-19T08:00:00Z,2021-03-19T16:30:00Z,,
+2021-03-22T00:00:00Z,2021-03-22T08:00:00Z,2021-03-22T16:30:00Z,,
+2021-03-23T00:00:00Z,2021-03-23T08:00:00Z,2021-03-23T16:30:00Z,,
+2021-03-24T00:00:00Z,2021-03-24T08:00:00Z,2021-03-24T16:30:00Z,,
+2021-03-25T00:00:00Z,2021-03-25T08:00:00Z,2021-03-25T16:30:00Z,,
+2021-03-26T00:00:00Z,2021-03-26T08:00:00Z,2021-03-26T16:30:00Z,,
+2021-03-29T00:00:00Z,2021-03-29T07:00:00Z,2021-03-29T15:30:00Z,,
+2021-03-30T00:00:00Z,2021-03-30T07:00:00Z,2021-03-30T15:30:00Z,,
+2021-03-31T00:00:00Z,2021-03-31T07:00:00Z,2021-03-31T15:30:00Z,,
+2021-04-01T00:00:00Z,2021-04-01T07:00:00Z,2021-04-01T15:30:00Z,,
+2021-04-06T00:00:00Z,2021-04-06T07:00:00Z,2021-04-06T15:30:00Z,,
+2021-04-07T00:00:00Z,2021-04-07T07:00:00Z,2021-04-07T15:30:00Z,,
+2021-04-08T00:00:00Z,2021-04-08T07:00:00Z,2021-04-08T15:30:00Z,,
+2021-04-09T00:00:00Z,2021-04-09T07:00:00Z,2021-04-09T15:30:00Z,,
+2021-04-12T00:00:00Z,2021-04-12T07:00:00Z,2021-04-12T15:30:00Z,,
+2021-04-13T00:00:00Z,2021-04-13T07:00:00Z,2021-04-13T15:30:00Z,,
+2021-04-14T00:00:00Z,2021-04-14T07:00:00Z,2021-04-14T15:30:00Z,,
+2021-04-15T00:00:00Z,2021-04-15T07:00:00Z,2021-04-15T15:30:00Z,,
+2021-04-16T00:00:00Z,2021-04-16T07:00:00Z,2021-04-16T15:30:00Z,,
+2021-04-19T00:00:00Z,2021-04-19T07:00:00Z,2021-04-19T15:30:00Z,,
+2021-04-20T00:00:00Z,2021-04-20T07:00:00Z,2021-04-20T15:30:00Z,,
+2021-04-21T00:00:00Z,2021-04-21T07:00:00Z,2021-04-21T15:30:00Z,,
+2021-04-22T00:00:00Z,2021-04-22T07:00:00Z,2021-04-22T15:30:00Z,,
+2021-04-23T00:00:00Z,2021-04-23T07:00:00Z,2021-04-23T15:30:00Z,,
+2021-04-26T00:00:00Z,2021-04-26T07:00:00Z,2021-04-26T15:30:00Z,,
+2021-04-27T00:00:00Z,2021-04-27T07:00:00Z,2021-04-27T15:30:00Z,,
+2021-04-28T00:00:00Z,2021-04-28T07:00:00Z,2021-04-28T15:30:00Z,,
+2021-04-29T00:00:00Z,2021-04-29T07:00:00Z,2021-04-29T15:30:00Z,,
+2021-04-30T00:00:00Z,2021-04-30T07:00:00Z,2021-04-30T15:30:00Z,,
+2021-05-03T00:00:00Z,2021-05-03T07:00:00Z,2021-05-03T15:30:00Z,,
+2021-05-04T00:00:00Z,2021-05-04T07:00:00Z,2021-05-04T15:30:00Z,,
+2021-05-05T00:00:00Z,2021-05-05T07:00:00Z,2021-05-05T15:30:00Z,,
+2021-05-06T00:00:00Z,2021-05-06T07:00:00Z,2021-05-06T15:30:00Z,,
+2021-05-07T00:00:00Z,2021-05-07T07:00:00Z,2021-05-07T15:30:00Z,,
+2021-05-10T00:00:00Z,2021-05-10T07:00:00Z,2021-05-10T15:30:00Z,,
+2021-05-11T00:00:00Z,2021-05-11T07:00:00Z,2021-05-11T15:30:00Z,,
+2021-05-12T00:00:00Z,2021-05-12T07:00:00Z,2021-05-12T15:30:00Z,,
+2021-05-13T00:00:00Z,2021-05-13T07:00:00Z,2021-05-13T15:30:00Z,,
+2021-05-14T00:00:00Z,2021-05-14T07:00:00Z,2021-05-14T15:30:00Z,,
+2021-05-17T00:00:00Z,2021-05-17T07:00:00Z,2021-05-17T15:30:00Z,,
+2021-05-18T00:00:00Z,2021-05-18T07:00:00Z,2021-05-18T15:30:00Z,,
+2021-05-19T00:00:00Z,2021-05-19T07:00:00Z,2021-05-19T15:30:00Z,,
+2021-05-20T00:00:00Z,2021-05-20T07:00:00Z,2021-05-20T15:30:00Z,,
+2021-05-21T00:00:00Z,2021-05-21T07:00:00Z,2021-05-21T15:30:00Z,,
+2021-05-25T00:00:00Z,2021-05-25T07:00:00Z,2021-05-25T15:30:00Z,,
+2021-05-26T00:00:00Z,2021-05-26T07:00:00Z,2021-05-26T15:30:00Z,,
+2021-05-27T00:00:00Z,2021-05-27T07:00:00Z,2021-05-27T15:30:00Z,,
+2021-05-28T00:00:00Z,2021-05-28T07:00:00Z,2021-05-28T15:30:00Z,,
+2021-05-31T00:00:00Z,2021-05-31T07:00:00Z,2021-05-31T15:30:00Z,,
+2021-06-01T00:00:00Z,2021-06-01T07:00:00Z,2021-06-01T15:30:00Z,,
+2021-06-02T00:00:00Z,2021-06-02T07:00:00Z,2021-06-02T15:30:00Z,,
+2021-06-03T00:00:00Z,2021-06-03T07:00:00Z,2021-06-03T15:30:00Z,,
+2021-06-04T00:00:00Z,2021-06-04T07:00:00Z,2021-06-04T15:30:00Z,,
+2021-06-07T00:00:00Z,2021-06-07T07:00:00Z,2021-06-07T15:30:00Z,,
+2021-06-08T00:00:00Z,2021-06-08T07:00:00Z,2021-06-08T15:30:00Z,,
+2021-06-09T00:00:00Z,2021-06-09T07:00:00Z,2021-06-09T15:30:00Z,,
+2021-06-10T00:00:00Z,2021-06-10T07:00:00Z,2021-06-10T15:30:00Z,,
+2021-06-11T00:00:00Z,2021-06-11T07:00:00Z,2021-06-11T15:30:00Z,,
+2021-06-14T00:00:00Z,2021-06-14T07:00:00Z,2021-06-14T15:30:00Z,,
+2021-06-15T00:00:00Z,2021-06-15T07:00:00Z,2021-06-15T15:30:00Z,,
+2021-06-16T00:00:00Z,2021-06-16T07:00:00Z,2021-06-16T15:30:00Z,,
+2021-06-17T00:00:00Z,2021-06-17T07:00:00Z,2021-06-17T15:30:00Z,,
+2021-06-18T00:00:00Z,2021-06-18T07:00:00Z,2021-06-18T15:30:00Z,,
+2021-06-21T00:00:00Z,2021-06-21T07:00:00Z,2021-06-21T15:30:00Z,,
+2021-06-22T00:00:00Z,2021-06-22T07:00:00Z,2021-06-22T15:30:00Z,,
+2021-06-23T00:00:00Z,2021-06-23T07:00:00Z,2021-06-23T15:30:00Z,,
+2021-06-24T00:00:00Z,2021-06-24T07:00:00Z,2021-06-24T15:30:00Z,,
+2021-06-25T00:00:00Z,2021-06-25T07:00:00Z,2021-06-25T15:30:00Z,,
+2021-06-28T00:00:00Z,2021-06-28T07:00:00Z,2021-06-28T15:30:00Z,,
+2021-06-29T00:00:00Z,2021-06-29T07:00:00Z,2021-06-29T15:30:00Z,,
+2021-06-30T00:00:00Z,2021-06-30T07:00:00Z,2021-06-30T15:30:00Z,,
+2021-07-01T00:00:00Z,2021-07-01T07:00:00Z,2021-07-01T15:30:00Z,,
+2021-07-02T00:00:00Z,2021-07-02T07:00:00Z,2021-07-02T15:30:00Z,,
+2021-07-05T00:00:00Z,2021-07-05T07:00:00Z,2021-07-05T15:30:00Z,,
+2021-07-06T00:00:00Z,2021-07-06T07:00:00Z,2021-07-06T15:30:00Z,,
+2021-07-07T00:00:00Z,2021-07-07T07:00:00Z,2021-07-07T15:30:00Z,,
+2021-07-08T00:00:00Z,2021-07-08T07:00:00Z,2021-07-08T15:30:00Z,,
+2021-07-09T00:00:00Z,2021-07-09T07:00:00Z,2021-07-09T15:30:00Z,,
+2021-07-12T00:00:00Z,2021-07-12T07:00:00Z,2021-07-12T15:30:00Z,,
+2021-07-13T00:00:00Z,2021-07-13T07:00:00Z,2021-07-13T15:30:00Z,,
+2021-07-14T00:00:00Z,2021-07-14T07:00:00Z,2021-07-14T15:30:00Z,,
+2021-07-15T00:00:00Z,2021-07-15T07:00:00Z,2021-07-15T15:30:00Z,,
+2021-07-16T00:00:00Z,2021-07-16T07:00:00Z,2021-07-16T15:30:00Z,,
+2021-07-19T00:00:00Z,2021-07-19T07:00:00Z,2021-07-19T15:30:00Z,,
+2021-07-20T00:00:00Z,2021-07-20T07:00:00Z,2021-07-20T15:30:00Z,,
+2021-07-21T00:00:00Z,2021-07-21T07:00:00Z,2021-07-21T15:30:00Z,,
+2021-07-22T00:00:00Z,2021-07-22T07:00:00Z,2021-07-22T15:30:00Z,,
+2021-07-23T00:00:00Z,2021-07-23T07:00:00Z,2021-07-23T15:30:00Z,,
+2021-07-26T00:00:00Z,2021-07-26T07:00:00Z,2021-07-26T15:30:00Z,,
+2021-07-27T00:00:00Z,2021-07-27T07:00:00Z,2021-07-27T15:30:00Z,,
+2021-07-28T00:00:00Z,2021-07-28T07:00:00Z,2021-07-28T15:30:00Z,,
+2021-07-29T00:00:00Z,2021-07-29T07:00:00Z,2021-07-29T15:30:00Z,,
+2021-07-30T00:00:00Z,2021-07-30T07:00:00Z,2021-07-30T15:30:00Z,,
+2021-08-02T00:00:00Z,2021-08-02T07:00:00Z,2021-08-02T15:30:00Z,,
+2021-08-03T00:00:00Z,2021-08-03T07:00:00Z,2021-08-03T15:30:00Z,,
+2021-08-04T00:00:00Z,2021-08-04T07:00:00Z,2021-08-04T15:30:00Z,,
+2021-08-05T00:00:00Z,2021-08-05T07:00:00Z,2021-08-05T15:30:00Z,,
+2021-08-06T00:00:00Z,2021-08-06T07:00:00Z,2021-08-06T15:30:00Z,,
+2021-08-09T00:00:00Z,2021-08-09T07:00:00Z,2021-08-09T15:30:00Z,,
+2021-08-10T00:00:00Z,2021-08-10T07:00:00Z,2021-08-10T15:30:00Z,,
+2021-08-11T00:00:00Z,2021-08-11T07:00:00Z,2021-08-11T15:30:00Z,,
+2021-08-12T00:00:00Z,2021-08-12T07:00:00Z,2021-08-12T15:30:00Z,,
+2021-08-13T00:00:00Z,2021-08-13T07:00:00Z,2021-08-13T15:30:00Z,,
+2021-08-16T00:00:00Z,2021-08-16T07:00:00Z,2021-08-16T15:30:00Z,,
+2021-08-17T00:00:00Z,2021-08-17T07:00:00Z,2021-08-17T15:30:00Z,,
+2021-08-18T00:00:00Z,2021-08-18T07:00:00Z,2021-08-18T15:30:00Z,,
+2021-08-19T00:00:00Z,2021-08-19T07:00:00Z,2021-08-19T15:30:00Z,,
+2021-08-20T00:00:00Z,2021-08-20T07:00:00Z,2021-08-20T15:30:00Z,,
+2021-08-23T00:00:00Z,2021-08-23T07:00:00Z,2021-08-23T15:30:00Z,,
+2021-08-24T00:00:00Z,2021-08-24T07:00:00Z,2021-08-24T15:30:00Z,,
+2021-08-25T00:00:00Z,2021-08-25T07:00:00Z,2021-08-25T15:30:00Z,,
+2021-08-26T00:00:00Z,2021-08-26T07:00:00Z,2021-08-26T15:30:00Z,,
+2021-08-27T00:00:00Z,2021-08-27T07:00:00Z,2021-08-27T15:30:00Z,,
+2021-08-30T00:00:00Z,2021-08-30T07:00:00Z,2021-08-30T15:30:00Z,,
+2021-08-31T00:00:00Z,2021-08-31T07:00:00Z,2021-08-31T15:30:00Z,,
+2021-09-01T00:00:00Z,2021-09-01T07:00:00Z,2021-09-01T15:30:00Z,,
+2021-09-02T00:00:00Z,2021-09-02T07:00:00Z,2021-09-02T15:30:00Z,,
+2021-09-03T00:00:00Z,2021-09-03T07:00:00Z,2021-09-03T15:30:00Z,,
+2021-09-06T00:00:00Z,2021-09-06T07:00:00Z,2021-09-06T15:30:00Z,,
+2021-09-07T00:00:00Z,2021-09-07T07:00:00Z,2021-09-07T15:30:00Z,,
+2021-09-08T00:00:00Z,2021-09-08T07:00:00Z,2021-09-08T15:30:00Z,,
+2021-09-09T00:00:00Z,2021-09-09T07:00:00Z,2021-09-09T15:30:00Z,,
+2021-09-10T00:00:00Z,2021-09-10T07:00:00Z,2021-09-10T15:30:00Z,,
+2021-09-13T00:00:00Z,2021-09-13T07:00:00Z,2021-09-13T15:30:00Z,,
+2021-09-14T00:00:00Z,2021-09-14T07:00:00Z,2021-09-14T15:30:00Z,,
+2021-09-15T00:00:00Z,2021-09-15T07:00:00Z,2021-09-15T15:30:00Z,,
+2021-09-16T00:00:00Z,2021-09-16T07:00:00Z,2021-09-16T15:30:00Z,,
+2021-09-17T00:00:00Z,2021-09-17T07:00:00Z,2021-09-17T15:30:00Z,,
+2021-09-20T00:00:00Z,2021-09-20T07:00:00Z,2021-09-20T15:30:00Z,,
+2021-09-21T00:00:00Z,2021-09-21T07:00:00Z,2021-09-21T15:30:00Z,,
+2021-09-22T00:00:00Z,2021-09-22T07:00:00Z,2021-09-22T15:30:00Z,,
+2021-09-23T00:00:00Z,2021-09-23T07:00:00Z,2021-09-23T15:30:00Z,,
+2021-09-24T00:00:00Z,2021-09-24T07:00:00Z,2021-09-24T15:30:00Z,,
+2021-09-27T00:00:00Z,2021-09-27T07:00:00Z,2021-09-27T15:30:00Z,,
+2021-09-28T00:00:00Z,2021-09-28T07:00:00Z,2021-09-28T15:30:00Z,,
+2021-09-29T00:00:00Z,2021-09-29T07:00:00Z,2021-09-29T15:30:00Z,,
+2021-09-30T00:00:00Z,2021-09-30T07:00:00Z,2021-09-30T15:30:00Z,,
+2021-10-01T00:00:00Z,2021-10-01T07:00:00Z,2021-10-01T15:30:00Z,,
+2021-10-04T00:00:00Z,2021-10-04T07:00:00Z,2021-10-04T15:30:00Z,,
+2021-10-05T00:00:00Z,2021-10-05T07:00:00Z,2021-10-05T15:30:00Z,,
+2021-10-06T00:00:00Z,2021-10-06T07:00:00Z,2021-10-06T15:30:00Z,,
+2021-10-07T00:00:00Z,2021-10-07T07:00:00Z,2021-10-07T15:30:00Z,,
+2021-10-08T00:00:00Z,2021-10-08T07:00:00Z,2021-10-08T15:30:00Z,,
+2021-10-11T00:00:00Z,2021-10-11T07:00:00Z,2021-10-11T15:30:00Z,,
+2021-10-12T00:00:00Z,2021-10-12T07:00:00Z,2021-10-12T15:30:00Z,,
+2021-10-13T00:00:00Z,2021-10-13T07:00:00Z,2021-10-13T15:30:00Z,,
+2021-10-14T00:00:00Z,2021-10-14T07:00:00Z,2021-10-14T15:30:00Z,,
+2021-10-15T00:00:00Z,2021-10-15T07:00:00Z,2021-10-15T15:30:00Z,,
+2021-10-18T00:00:00Z,2021-10-18T07:00:00Z,2021-10-18T15:30:00Z,,
+2021-10-19T00:00:00Z,2021-10-19T07:00:00Z,2021-10-19T15:30:00Z,,
+2021-10-20T00:00:00Z,2021-10-20T07:00:00Z,2021-10-20T15:30:00Z,,
+2021-10-21T00:00:00Z,2021-10-21T07:00:00Z,2021-10-21T15:30:00Z,,
+2021-10-22T00:00:00Z,2021-10-22T07:00:00Z,2021-10-22T15:30:00Z,,
+2021-10-25T00:00:00Z,2021-10-25T07:00:00Z,2021-10-25T15:30:00Z,,
+2021-10-27T00:00:00Z,2021-10-27T07:00:00Z,2021-10-27T15:30:00Z,,
+2021-10-28T00:00:00Z,2021-10-28T07:00:00Z,2021-10-28T15:30:00Z,,
+2021-10-29T00:00:00Z,2021-10-29T07:00:00Z,2021-10-29T15:30:00Z,,
+2021-11-01T00:00:00Z,2021-11-01T08:00:00Z,2021-11-01T16:30:00Z,,
+2021-11-02T00:00:00Z,2021-11-02T08:00:00Z,2021-11-02T16:30:00Z,,
+2021-11-03T00:00:00Z,2021-11-03T08:00:00Z,2021-11-03T16:30:00Z,,
+2021-11-04T00:00:00Z,2021-11-04T08:00:00Z,2021-11-04T16:30:00Z,,
+2021-11-05T00:00:00Z,2021-11-05T08:00:00Z,2021-11-05T16:30:00Z,,
+2021-11-08T00:00:00Z,2021-11-08T08:00:00Z,2021-11-08T16:30:00Z,,
+2021-11-09T00:00:00Z,2021-11-09T08:00:00Z,2021-11-09T16:30:00Z,,
+2021-11-10T00:00:00Z,2021-11-10T08:00:00Z,2021-11-10T16:30:00Z,,
+2021-11-11T00:00:00Z,2021-11-11T08:00:00Z,2021-11-11T16:30:00Z,,
+2021-11-12T00:00:00Z,2021-11-12T08:00:00Z,2021-11-12T16:30:00Z,,
+2021-11-15T00:00:00Z,2021-11-15T08:00:00Z,2021-11-15T16:30:00Z,,
+2021-11-16T00:00:00Z,2021-11-16T08:00:00Z,2021-11-16T16:30:00Z,,
+2021-11-17T00:00:00Z,2021-11-17T08:00:00Z,2021-11-17T16:30:00Z,,
+2021-11-18T00:00:00Z,2021-11-18T08:00:00Z,2021-11-18T16:30:00Z,,
+2021-11-19T00:00:00Z,2021-11-19T08:00:00Z,2021-11-19T16:30:00Z,,
+2021-11-22T00:00:00Z,2021-11-22T08:00:00Z,2021-11-22T16:30:00Z,,
+2021-11-23T00:00:00Z,2021-11-23T08:00:00Z,2021-11-23T16:30:00Z,,
+2021-11-24T00:00:00Z,2021-11-24T08:00:00Z,2021-11-24T16:30:00Z,,
+2021-11-25T00:00:00Z,2021-11-25T08:00:00Z,2021-11-25T16:30:00Z,,
+2021-11-26T00:00:00Z,2021-11-26T08:00:00Z,2021-11-26T16:30:00Z,,
+2021-11-29T00:00:00Z,2021-11-29T08:00:00Z,2021-11-29T16:30:00Z,,
+2021-11-30T00:00:00Z,2021-11-30T08:00:00Z,2021-11-30T16:30:00Z,,
+2021-12-01T00:00:00Z,2021-12-01T08:00:00Z,2021-12-01T16:30:00Z,,
+2021-12-02T00:00:00Z,2021-12-02T08:00:00Z,2021-12-02T16:30:00Z,,
+2021-12-03T00:00:00Z,2021-12-03T08:00:00Z,2021-12-03T16:30:00Z,,
+2021-12-06T00:00:00Z,2021-12-06T08:00:00Z,2021-12-06T16:30:00Z,,
+2021-12-07T00:00:00Z,2021-12-07T08:00:00Z,2021-12-07T16:30:00Z,,
+2021-12-08T00:00:00Z,2021-12-08T08:00:00Z,2021-12-08T16:30:00Z,,
+2021-12-09T00:00:00Z,2021-12-09T08:00:00Z,2021-12-09T16:30:00Z,,
+2021-12-10T00:00:00Z,2021-12-10T08:00:00Z,2021-12-10T16:30:00Z,,
+2021-12-13T00:00:00Z,2021-12-13T08:00:00Z,2021-12-13T16:30:00Z,,
+2021-12-14T00:00:00Z,2021-12-14T08:00:00Z,2021-12-14T16:30:00Z,,
+2021-12-15T00:00:00Z,2021-12-15T08:00:00Z,2021-12-15T16:30:00Z,,
+2021-12-16T00:00:00Z,2021-12-16T08:00:00Z,2021-12-16T16:30:00Z,,
+2021-12-17T00:00:00Z,2021-12-17T08:00:00Z,2021-12-17T16:30:00Z,,
+2021-12-20T00:00:00Z,2021-12-20T08:00:00Z,2021-12-20T16:30:00Z,,
+2021-12-21T00:00:00Z,2021-12-21T08:00:00Z,2021-12-21T16:30:00Z,,
+2021-12-22T00:00:00Z,2021-12-22T08:00:00Z,2021-12-22T16:30:00Z,,
+2021-12-23T00:00:00Z,2021-12-23T08:00:00Z,2021-12-23T16:30:00Z,,
+2021-12-27T00:00:00Z,2021-12-27T08:00:00Z,2021-12-27T16:30:00Z,,
+2021-12-28T00:00:00Z,2021-12-28T08:00:00Z,2021-12-28T16:30:00Z,,
+2021-12-29T00:00:00Z,2021-12-29T08:00:00Z,2021-12-29T16:30:00Z,,
+2021-12-30T00:00:00Z,2021-12-30T08:00:00Z,2021-12-30T13:15:00Z,,
+2022-01-03T00:00:00Z,2022-01-03T08:00:00Z,2022-01-03T16:30:00Z,,
+2022-01-04T00:00:00Z,2022-01-04T08:00:00Z,2022-01-04T16:30:00Z,,
+2022-01-05T00:00:00Z,2022-01-05T08:00:00Z,2022-01-05T16:30:00Z,,
+2022-01-06T00:00:00Z,2022-01-06T08:00:00Z,2022-01-06T16:30:00Z,,
+2022-01-07T00:00:00Z,2022-01-07T08:00:00Z,2022-01-07T16:30:00Z,,
+2022-01-10T00:00:00Z,2022-01-10T08:00:00Z,2022-01-10T16:30:00Z,,
+2022-01-11T00:00:00Z,2022-01-11T08:00:00Z,2022-01-11T16:30:00Z,,
+2022-01-12T00:00:00Z,2022-01-12T08:00:00Z,2022-01-12T16:30:00Z,,
+2022-01-13T00:00:00Z,2022-01-13T08:00:00Z,2022-01-13T16:30:00Z,,
+2022-01-14T00:00:00Z,2022-01-14T08:00:00Z,2022-01-14T16:30:00Z,,
+2022-01-17T00:00:00Z,2022-01-17T08:00:00Z,2022-01-17T16:30:00Z,,
+2022-01-18T00:00:00Z,2022-01-18T08:00:00Z,2022-01-18T16:30:00Z,,
+2022-01-19T00:00:00Z,2022-01-19T08:00:00Z,2022-01-19T16:30:00Z,,
+2022-01-20T00:00:00Z,2022-01-20T08:00:00Z,2022-01-20T16:30:00Z,,
+2022-01-21T00:00:00Z,2022-01-21T08:00:00Z,2022-01-21T16:30:00Z,,
+2022-01-24T00:00:00Z,2022-01-24T08:00:00Z,2022-01-24T16:30:00Z,,
+2022-01-25T00:00:00Z,2022-01-25T08:00:00Z,2022-01-25T16:30:00Z,,
+2022-01-26T00:00:00Z,2022-01-26T08:00:00Z,2022-01-26T16:30:00Z,,
+2022-01-27T00:00:00Z,2022-01-27T08:00:00Z,2022-01-27T16:30:00Z,,
+2022-01-28T00:00:00Z,2022-01-28T08:00:00Z,2022-01-28T16:30:00Z,,
+2022-01-31T00:00:00Z,2022-01-31T08:00:00Z,2022-01-31T16:30:00Z,,
+2022-02-01T00:00:00Z,2022-02-01T08:00:00Z,2022-02-01T16:30:00Z,,
+2022-02-02T00:00:00Z,2022-02-02T08:00:00Z,2022-02-02T16:30:00Z,,
+2022-02-03T00:00:00Z,2022-02-03T08:00:00Z,2022-02-03T16:30:00Z,,
+2022-02-04T00:00:00Z,2022-02-04T08:00:00Z,2022-02-04T16:30:00Z,,
+2022-02-07T00:00:00Z,2022-02-07T08:00:00Z,2022-02-07T16:30:00Z,,
+2022-02-08T00:00:00Z,2022-02-08T08:00:00Z,2022-02-08T16:30:00Z,,
+2022-02-09T00:00:00Z,2022-02-09T08:00:00Z,2022-02-09T16:30:00Z,,
+2022-02-10T00:00:00Z,2022-02-10T08:00:00Z,2022-02-10T16:30:00Z,,
+2022-02-11T00:00:00Z,2022-02-11T08:00:00Z,2022-02-11T16:30:00Z,,
+2022-02-14T00:00:00Z,2022-02-14T08:00:00Z,2022-02-14T16:30:00Z,,
+2022-02-15T00:00:00Z,2022-02-15T08:00:00Z,2022-02-15T16:30:00Z,,
+2022-02-16T00:00:00Z,2022-02-16T08:00:00Z,2022-02-16T16:30:00Z,,
+2022-02-17T00:00:00Z,2022-02-17T08:00:00Z,2022-02-17T16:30:00Z,,
+2022-02-18T00:00:00Z,2022-02-18T08:00:00Z,2022-02-18T16:30:00Z,,
+2022-02-21T00:00:00Z,2022-02-21T08:00:00Z,2022-02-21T16:30:00Z,,
+2022-02-22T00:00:00Z,2022-02-22T08:00:00Z,2022-02-22T16:30:00Z,,
+2022-02-23T00:00:00Z,2022-02-23T08:00:00Z,2022-02-23T16:30:00Z,,
+2022-02-24T00:00:00Z,2022-02-24T08:00:00Z,2022-02-24T16:30:00Z,,
+2022-02-25T00:00:00Z,2022-02-25T08:00:00Z,2022-02-25T16:30:00Z,,
+2022-02-28T00:00:00Z,2022-02-28T08:00:00Z,2022-02-28T16:30:00Z,,
+2022-03-01T00:00:00Z,2022-03-01T08:00:00Z,2022-03-01T16:30:00Z,,
+2022-03-02T00:00:00Z,2022-03-02T08:00:00Z,2022-03-02T16:30:00Z,,
+2022-03-03T00:00:00Z,2022-03-03T08:00:00Z,2022-03-03T16:30:00Z,,
+2022-03-04T00:00:00Z,2022-03-04T08:00:00Z,2022-03-04T16:30:00Z,,
+2022-03-07T00:00:00Z,2022-03-07T08:00:00Z,2022-03-07T16:30:00Z,,
+2022-03-08T00:00:00Z,2022-03-08T08:00:00Z,2022-03-08T16:30:00Z,,
+2022-03-09T00:00:00Z,2022-03-09T08:00:00Z,2022-03-09T16:30:00Z,,
+2022-03-10T00:00:00Z,2022-03-10T08:00:00Z,2022-03-10T16:30:00Z,,
+2022-03-11T00:00:00Z,2022-03-11T08:00:00Z,2022-03-11T16:30:00Z,,
+2022-03-14T00:00:00Z,2022-03-14T08:00:00Z,2022-03-14T16:30:00Z,,
+2022-03-15T00:00:00Z,2022-03-15T08:00:00Z,2022-03-15T16:30:00Z,,
+2022-03-16T00:00:00Z,2022-03-16T08:00:00Z,2022-03-16T16:30:00Z,,
+2022-03-17T00:00:00Z,2022-03-17T08:00:00Z,2022-03-17T16:30:00Z,,
+2022-03-18T00:00:00Z,2022-03-18T08:00:00Z,2022-03-18T16:30:00Z,,
+2022-03-21T00:00:00Z,2022-03-21T08:00:00Z,2022-03-21T16:30:00Z,,
+2022-03-22T00:00:00Z,2022-03-22T08:00:00Z,2022-03-22T16:30:00Z,,
+2022-03-23T00:00:00Z,2022-03-23T08:00:00Z,2022-03-23T16:30:00Z,,
+2022-03-24T00:00:00Z,2022-03-24T08:00:00Z,2022-03-24T16:30:00Z,,
+2022-03-25T00:00:00Z,2022-03-25T08:00:00Z,2022-03-25T16:30:00Z,,
+2022-03-28T00:00:00Z,2022-03-28T07:00:00Z,2022-03-28T15:30:00Z,,
+2022-03-29T00:00:00Z,2022-03-29T07:00:00Z,2022-03-29T15:30:00Z,,
+2022-03-30T00:00:00Z,2022-03-30T07:00:00Z,2022-03-30T15:30:00Z,,
+2022-03-31T00:00:00Z,2022-03-31T07:00:00Z,2022-03-31T15:30:00Z,,
+2022-04-01T00:00:00Z,2022-04-01T07:00:00Z,2022-04-01T15:30:00Z,,
+2022-04-04T00:00:00Z,2022-04-04T07:00:00Z,2022-04-04T15:30:00Z,,
+2022-04-05T00:00:00Z,2022-04-05T07:00:00Z,2022-04-05T15:30:00Z,,
+2022-04-06T00:00:00Z,2022-04-06T07:00:00Z,2022-04-06T15:30:00Z,,
+2022-04-07T00:00:00Z,2022-04-07T07:00:00Z,2022-04-07T15:30:00Z,,
+2022-04-08T00:00:00Z,2022-04-08T07:00:00Z,2022-04-08T15:30:00Z,,
+2022-04-11T00:00:00Z,2022-04-11T07:00:00Z,2022-04-11T15:30:00Z,,
+2022-04-12T00:00:00Z,2022-04-12T07:00:00Z,2022-04-12T15:30:00Z,,
+2022-04-13T00:00:00Z,2022-04-13T07:00:00Z,2022-04-13T15:30:00Z,,
+2022-04-14T00:00:00Z,2022-04-14T07:00:00Z,2022-04-14T15:30:00Z,,
+2022-04-19T00:00:00Z,2022-04-19T07:00:00Z,2022-04-19T15:30:00Z,,
+2022-04-20T00:00:00Z,2022-04-20T07:00:00Z,2022-04-20T15:30:00Z,,
+2022-04-21T00:00:00Z,2022-04-21T07:00:00Z,2022-04-21T15:30:00Z,,
+2022-04-22T00:00:00Z,2022-04-22T07:00:00Z,2022-04-22T15:30:00Z,,
+2022-04-25T00:00:00Z,2022-04-25T07:00:00Z,2022-04-25T15:30:00Z,,
+2022-04-26T00:00:00Z,2022-04-26T07:00:00Z,2022-04-26T15:30:00Z,,
+2022-04-27T00:00:00Z,2022-04-27T07:00:00Z,2022-04-27T15:30:00Z,,
+2022-04-28T00:00:00Z,2022-04-28T07:00:00Z,2022-04-28T15:30:00Z,,
+2022-04-29T00:00:00Z,2022-04-29T07:00:00Z,2022-04-29T15:30:00Z,,
+2022-05-02T00:00:00Z,2022-05-02T07:00:00Z,2022-05-02T15:30:00Z,,
+2022-05-03T00:00:00Z,2022-05-03T07:00:00Z,2022-05-03T15:30:00Z,,
+2022-05-04T00:00:00Z,2022-05-04T07:00:00Z,2022-05-04T15:30:00Z,,
+2022-05-05T00:00:00Z,2022-05-05T07:00:00Z,2022-05-05T15:30:00Z,,
+2022-05-06T00:00:00Z,2022-05-06T07:00:00Z,2022-05-06T15:30:00Z,,
+2022-05-09T00:00:00Z,2022-05-09T07:00:00Z,2022-05-09T15:30:00Z,,
+2022-05-10T00:00:00Z,2022-05-10T07:00:00Z,2022-05-10T15:30:00Z,,
+2022-05-11T00:00:00Z,2022-05-11T07:00:00Z,2022-05-11T15:30:00Z,,
+2022-05-12T00:00:00Z,2022-05-12T07:00:00Z,2022-05-12T15:30:00Z,,
+2022-05-13T00:00:00Z,2022-05-13T07:00:00Z,2022-05-13T15:30:00Z,,
+2022-05-16T00:00:00Z,2022-05-16T07:00:00Z,2022-05-16T15:30:00Z,,
+2022-05-17T00:00:00Z,2022-05-17T07:00:00Z,2022-05-17T15:30:00Z,,
+2022-05-18T00:00:00Z,2022-05-18T07:00:00Z,2022-05-18T15:30:00Z,,
+2022-05-19T00:00:00Z,2022-05-19T07:00:00Z,2022-05-19T15:30:00Z,,
+2022-05-20T00:00:00Z,2022-05-20T07:00:00Z,2022-05-20T15:30:00Z,,
+2022-05-23T00:00:00Z,2022-05-23T07:00:00Z,2022-05-23T15:30:00Z,,
+2022-05-24T00:00:00Z,2022-05-24T07:00:00Z,2022-05-24T15:30:00Z,,
+2022-05-25T00:00:00Z,2022-05-25T07:00:00Z,2022-05-25T15:30:00Z,,
+2022-05-26T00:00:00Z,2022-05-26T07:00:00Z,2022-05-26T15:30:00Z,,
+2022-05-27T00:00:00Z,2022-05-27T07:00:00Z,2022-05-27T15:30:00Z,,
+2022-05-30T00:00:00Z,2022-05-30T07:00:00Z,2022-05-30T15:30:00Z,,
+2022-05-31T00:00:00Z,2022-05-31T07:00:00Z,2022-05-31T15:30:00Z,,
+2022-06-01T00:00:00Z,2022-06-01T07:00:00Z,2022-06-01T15:30:00Z,,
+2022-06-02T00:00:00Z,2022-06-02T07:00:00Z,2022-06-02T15:30:00Z,,
+2022-06-03T00:00:00Z,2022-06-03T07:00:00Z,2022-06-03T15:30:00Z,,
+2022-06-07T00:00:00Z,2022-06-07T07:00:00Z,2022-06-07T15:30:00Z,,
+2022-06-08T00:00:00Z,2022-06-08T07:00:00Z,2022-06-08T15:30:00Z,,
+2022-06-09T00:00:00Z,2022-06-09T07:00:00Z,2022-06-09T15:30:00Z,,
+2022-06-10T00:00:00Z,2022-06-10T07:00:00Z,2022-06-10T15:30:00Z,,
+2022-06-13T00:00:00Z,2022-06-13T07:00:00Z,2022-06-13T15:30:00Z,,
+2022-06-14T00:00:00Z,2022-06-14T07:00:00Z,2022-06-14T15:30:00Z,,
+2022-06-15T00:00:00Z,2022-06-15T07:00:00Z,2022-06-15T15:30:00Z,,
+2022-06-16T00:00:00Z,2022-06-16T07:00:00Z,2022-06-16T15:30:00Z,,
+2022-06-17T00:00:00Z,2022-06-17T07:00:00Z,2022-06-17T15:30:00Z,,
+2022-06-20T00:00:00Z,2022-06-20T07:00:00Z,2022-06-20T15:30:00Z,,
+2022-06-21T00:00:00Z,2022-06-21T07:00:00Z,2022-06-21T15:30:00Z,,
+2022-06-22T00:00:00Z,2022-06-22T07:00:00Z,2022-06-22T15:30:00Z,,
+2022-06-23T00:00:00Z,2022-06-23T07:00:00Z,2022-06-23T15:30:00Z,,
+2022-06-24T00:00:00Z,2022-06-24T07:00:00Z,2022-06-24T15:30:00Z,,
+2022-06-27T00:00:00Z,2022-06-27T07:00:00Z,2022-06-27T15:30:00Z,,
+2022-06-28T00:00:00Z,2022-06-28T07:00:00Z,2022-06-28T15:30:00Z,,
+2022-06-29T00:00:00Z,2022-06-29T07:00:00Z,2022-06-29T15:30:00Z,,
+2022-06-30T00:00:00Z,2022-06-30T07:00:00Z,2022-06-30T15:30:00Z,,
+2022-07-01T00:00:00Z,2022-07-01T07:00:00Z,2022-07-01T15:30:00Z,,
+2022-07-04T00:00:00Z,2022-07-04T07:00:00Z,2022-07-04T15:30:00Z,,
+2022-07-05T00:00:00Z,2022-07-05T07:00:00Z,2022-07-05T15:30:00Z,,
+2022-07-06T00:00:00Z,2022-07-06T07:00:00Z,2022-07-06T15:30:00Z,,
+2022-07-07T00:00:00Z,2022-07-07T07:00:00Z,2022-07-07T15:30:00Z,,
+2022-07-08T00:00:00Z,2022-07-08T07:00:00Z,2022-07-08T15:30:00Z,,
+2022-07-11T00:00:00Z,2022-07-11T07:00:00Z,2022-07-11T15:30:00Z,,
+2022-07-12T00:00:00Z,2022-07-12T07:00:00Z,2022-07-12T15:30:00Z,,
+2022-07-13T00:00:00Z,2022-07-13T07:00:00Z,2022-07-13T15:30:00Z,,
+2022-07-14T00:00:00Z,2022-07-14T07:00:00Z,2022-07-14T15:30:00Z,,
+2022-07-15T00:00:00Z,2022-07-15T07:00:00Z,2022-07-15T15:30:00Z,,
+2022-07-18T00:00:00Z,2022-07-18T07:00:00Z,2022-07-18T15:30:00Z,,
+2022-07-19T00:00:00Z,2022-07-19T07:00:00Z,2022-07-19T15:30:00Z,,
+2022-07-20T00:00:00Z,2022-07-20T07:00:00Z,2022-07-20T15:30:00Z,,
+2022-07-21T00:00:00Z,2022-07-21T07:00:00Z,2022-07-21T15:30:00Z,,
+2022-07-22T00:00:00Z,2022-07-22T07:00:00Z,2022-07-22T15:30:00Z,,
+2022-07-25T00:00:00Z,2022-07-25T07:00:00Z,2022-07-25T15:30:00Z,,
+2022-07-26T00:00:00Z,2022-07-26T07:00:00Z,2022-07-26T15:30:00Z,,
+2022-07-27T00:00:00Z,2022-07-27T07:00:00Z,2022-07-27T15:30:00Z,,
+2022-07-28T00:00:00Z,2022-07-28T07:00:00Z,2022-07-28T15:30:00Z,,
+2022-07-29T00:00:00Z,2022-07-29T07:00:00Z,2022-07-29T15:30:00Z,,
+2022-08-01T00:00:00Z,2022-08-01T07:00:00Z,2022-08-01T15:30:00Z,,
+2022-08-02T00:00:00Z,2022-08-02T07:00:00Z,2022-08-02T15:30:00Z,,
+2022-08-03T00:00:00Z,2022-08-03T07:00:00Z,2022-08-03T15:30:00Z,,
+2022-08-04T00:00:00Z,2022-08-04T07:00:00Z,2022-08-04T15:30:00Z,,
+2022-08-05T00:00:00Z,2022-08-05T07:00:00Z,2022-08-05T15:30:00Z,,
+2022-08-08T00:00:00Z,2022-08-08T07:00:00Z,2022-08-08T15:30:00Z,,
+2022-08-09T00:00:00Z,2022-08-09T07:00:00Z,2022-08-09T15:30:00Z,,
+2022-08-10T00:00:00Z,2022-08-10T07:00:00Z,2022-08-10T15:30:00Z,,
+2022-08-11T00:00:00Z,2022-08-11T07:00:00Z,2022-08-11T15:30:00Z,,
+2022-08-12T00:00:00Z,2022-08-12T07:00:00Z,2022-08-12T15:30:00Z,,
+2022-08-15T00:00:00Z,2022-08-15T07:00:00Z,2022-08-15T15:30:00Z,,
+2022-08-16T00:00:00Z,2022-08-16T07:00:00Z,2022-08-16T15:30:00Z,,
+2022-08-17T00:00:00Z,2022-08-17T07:00:00Z,2022-08-17T15:30:00Z,,
+2022-08-18T00:00:00Z,2022-08-18T07:00:00Z,2022-08-18T15:30:00Z,,
+2022-08-19T00:00:00Z,2022-08-19T07:00:00Z,2022-08-19T15:30:00Z,,
+2022-08-22T00:00:00Z,2022-08-22T07:00:00Z,2022-08-22T15:30:00Z,,
+2022-08-23T00:00:00Z,2022-08-23T07:00:00Z,2022-08-23T15:30:00Z,,
+2022-08-24T00:00:00Z,2022-08-24T07:00:00Z,2022-08-24T15:30:00Z,,
+2022-08-25T00:00:00Z,2022-08-25T07:00:00Z,2022-08-25T15:30:00Z,,
+2022-08-26T00:00:00Z,2022-08-26T07:00:00Z,2022-08-26T15:30:00Z,,
+2022-08-29T00:00:00Z,2022-08-29T07:00:00Z,2022-08-29T15:30:00Z,,
+2022-08-30T00:00:00Z,2022-08-30T07:00:00Z,2022-08-30T15:30:00Z,,
+2022-08-31T00:00:00Z,2022-08-31T07:00:00Z,2022-08-31T15:30:00Z,,
+2022-09-01T00:00:00Z,2022-09-01T07:00:00Z,2022-09-01T15:30:00Z,,
+2022-09-02T00:00:00Z,2022-09-02T07:00:00Z,2022-09-02T15:30:00Z,,
+2022-09-05T00:00:00Z,2022-09-05T07:00:00Z,2022-09-05T15:30:00Z,,
+2022-09-06T00:00:00Z,2022-09-06T07:00:00Z,2022-09-06T15:30:00Z,,
+2022-09-07T00:00:00Z,2022-09-07T07:00:00Z,2022-09-07T15:30:00Z,,
+2022-09-08T00:00:00Z,2022-09-08T07:00:00Z,2022-09-08T15:30:00Z,,
+2022-09-09T00:00:00Z,2022-09-09T07:00:00Z,2022-09-09T15:30:00Z,,
+2022-09-12T00:00:00Z,2022-09-12T07:00:00Z,2022-09-12T15:30:00Z,,
+2022-09-13T00:00:00Z,2022-09-13T07:00:00Z,2022-09-13T15:30:00Z,,
+2022-09-14T00:00:00Z,2022-09-14T07:00:00Z,2022-09-14T15:30:00Z,,
+2022-09-15T00:00:00Z,2022-09-15T07:00:00Z,2022-09-15T15:30:00Z,,
+2022-09-16T00:00:00Z,2022-09-16T07:00:00Z,2022-09-16T15:30:00Z,,
+2022-09-19T00:00:00Z,2022-09-19T07:00:00Z,2022-09-19T15:30:00Z,,
+2022-09-20T00:00:00Z,2022-09-20T07:00:00Z,2022-09-20T15:30:00Z,,
+2022-09-21T00:00:00Z,2022-09-21T07:00:00Z,2022-09-21T15:30:00Z,,
+2022-09-22T00:00:00Z,2022-09-22T07:00:00Z,2022-09-22T15:30:00Z,,
+2022-09-23T00:00:00Z,2022-09-23T07:00:00Z,2022-09-23T15:30:00Z,,
+2022-09-26T00:00:00Z,2022-09-26T07:00:00Z,2022-09-26T15:30:00Z,,
+2022-09-27T00:00:00Z,2022-09-27T07:00:00Z,2022-09-27T15:30:00Z,,
+2022-09-28T00:00:00Z,2022-09-28T07:00:00Z,2022-09-28T15:30:00Z,,
+2022-09-29T00:00:00Z,2022-09-29T07:00:00Z,2022-09-29T15:30:00Z,,
+2022-09-30T00:00:00Z,2022-09-30T07:00:00Z,2022-09-30T15:30:00Z,,
+2022-10-03T00:00:00Z,2022-10-03T07:00:00Z,2022-10-03T15:30:00Z,,
+2022-10-04T00:00:00Z,2022-10-04T07:00:00Z,2022-10-04T15:30:00Z,,
+2022-10-05T00:00:00Z,2022-10-05T07:00:00Z,2022-10-05T15:30:00Z,,
+2022-10-06T00:00:00Z,2022-10-06T07:00:00Z,2022-10-06T15:30:00Z,,
+2022-10-07T00:00:00Z,2022-10-07T07:00:00Z,2022-10-07T15:30:00Z,,
+2022-10-10T00:00:00Z,2022-10-10T07:00:00Z,2022-10-10T15:30:00Z,,
+2022-10-11T00:00:00Z,2022-10-11T07:00:00Z,2022-10-11T15:30:00Z,,
+2022-10-12T00:00:00Z,2022-10-12T07:00:00Z,2022-10-12T15:30:00Z,,
+2022-10-13T00:00:00Z,2022-10-13T07:00:00Z,2022-10-13T15:30:00Z,,
+2022-10-14T00:00:00Z,2022-10-14T07:00:00Z,2022-10-14T15:30:00Z,,
+2022-10-17T00:00:00Z,2022-10-17T07:00:00Z,2022-10-17T15:30:00Z,,
+2022-10-18T00:00:00Z,2022-10-18T07:00:00Z,2022-10-18T15:30:00Z,,
+2022-10-19T00:00:00Z,2022-10-19T07:00:00Z,2022-10-19T15:30:00Z,,
+2022-10-20T00:00:00Z,2022-10-20T07:00:00Z,2022-10-20T15:30:00Z,,
+2022-10-21T00:00:00Z,2022-10-21T07:00:00Z,2022-10-21T15:30:00Z,,
+2022-10-24T00:00:00Z,2022-10-24T07:00:00Z,2022-10-24T15:30:00Z,,
+2022-10-25T00:00:00Z,2022-10-25T07:00:00Z,2022-10-25T15:30:00Z,,
+2022-10-27T00:00:00Z,2022-10-27T07:00:00Z,2022-10-27T15:30:00Z,,
+2022-10-28T00:00:00Z,2022-10-28T07:00:00Z,2022-10-28T15:30:00Z,,
+2022-10-31T00:00:00Z,2022-10-31T08:00:00Z,2022-10-31T16:30:00Z,,
+2022-11-01T00:00:00Z,2022-11-01T08:00:00Z,2022-11-01T16:30:00Z,,
+2022-11-02T00:00:00Z,2022-11-02T08:00:00Z,2022-11-02T16:30:00Z,,
+2022-11-03T00:00:00Z,2022-11-03T08:00:00Z,2022-11-03T16:30:00Z,,
+2022-11-04T00:00:00Z,2022-11-04T08:00:00Z,2022-11-04T16:30:00Z,,
+2022-11-07T00:00:00Z,2022-11-07T08:00:00Z,2022-11-07T16:30:00Z,,
+2022-11-08T00:00:00Z,2022-11-08T08:00:00Z,2022-11-08T16:30:00Z,,
+2022-11-09T00:00:00Z,2022-11-09T08:00:00Z,2022-11-09T16:30:00Z,,
+2022-11-10T00:00:00Z,2022-11-10T08:00:00Z,2022-11-10T16:30:00Z,,
+2022-11-11T00:00:00Z,2022-11-11T08:00:00Z,2022-11-11T16:30:00Z,,
+2022-11-14T00:00:00Z,2022-11-14T08:00:00Z,2022-11-14T16:30:00Z,,
+2022-11-15T00:00:00Z,2022-11-15T08:00:00Z,2022-11-15T16:30:00Z,,
+2022-11-16T00:00:00Z,2022-11-16T08:00:00Z,2022-11-16T16:30:00Z,,
+2022-11-17T00:00:00Z,2022-11-17T08:00:00Z,2022-11-17T16:30:00Z,,
+2022-11-18T00:00:00Z,2022-11-18T08:00:00Z,2022-11-18T16:30:00Z,,
+2022-11-21T00:00:00Z,2022-11-21T08:00:00Z,2022-11-21T16:30:00Z,,
+2022-11-22T00:00:00Z,2022-11-22T08:00:00Z,2022-11-22T16:30:00Z,,
+2022-11-23T00:00:00Z,2022-11-23T08:00:00Z,2022-11-23T16:30:00Z,,
+2022-11-24T00:00:00Z,2022-11-24T08:00:00Z,2022-11-24T16:30:00Z,,
+2022-11-25T00:00:00Z,2022-11-25T08:00:00Z,2022-11-25T16:30:00Z,,
+2022-11-28T00:00:00Z,2022-11-28T08:00:00Z,2022-11-28T16:30:00Z,,
+2022-11-29T00:00:00Z,2022-11-29T08:00:00Z,2022-11-29T16:30:00Z,,
+2022-11-30T00:00:00Z,2022-11-30T08:00:00Z,2022-11-30T16:30:00Z,,
+2022-12-01T00:00:00Z,2022-12-01T08:00:00Z,2022-12-01T16:30:00Z,,
+2022-12-02T00:00:00Z,2022-12-02T08:00:00Z,2022-12-02T16:30:00Z,,
+2022-12-05T00:00:00Z,2022-12-05T08:00:00Z,2022-12-05T16:30:00Z,,
+2022-12-06T00:00:00Z,2022-12-06T08:00:00Z,2022-12-06T16:30:00Z,,
+2022-12-07T00:00:00Z,2022-12-07T08:00:00Z,2022-12-07T16:30:00Z,,
+2022-12-08T00:00:00Z,2022-12-08T08:00:00Z,2022-12-08T16:30:00Z,,
+2022-12-09T00:00:00Z,2022-12-09T08:00:00Z,2022-12-09T16:30:00Z,,
+2022-12-12T00:00:00Z,2022-12-12T08:00:00Z,2022-12-12T16:30:00Z,,
+2022-12-13T00:00:00Z,2022-12-13T08:00:00Z,2022-12-13T16:30:00Z,,
+2022-12-14T00:00:00Z,2022-12-14T08:00:00Z,2022-12-14T16:30:00Z,,
+2022-12-15T00:00:00Z,2022-12-15T08:00:00Z,2022-12-15T16:30:00Z,,
+2022-12-16T00:00:00Z,2022-12-16T08:00:00Z,2022-12-16T16:30:00Z,,
+2022-12-19T00:00:00Z,2022-12-19T08:00:00Z,2022-12-19T16:30:00Z,,
+2022-12-20T00:00:00Z,2022-12-20T08:00:00Z,2022-12-20T16:30:00Z,,
+2022-12-21T00:00:00Z,2022-12-21T08:00:00Z,2022-12-21T16:30:00Z,,
+2022-12-22T00:00:00Z,2022-12-22T08:00:00Z,2022-12-22T16:30:00Z,,
+2022-12-23T00:00:00Z,2022-12-23T08:00:00Z,2022-12-23T16:30:00Z,,
+2022-12-27T00:00:00Z,2022-12-27T08:00:00Z,2022-12-27T16:30:00Z,,
+2022-12-28T00:00:00Z,2022-12-28T08:00:00Z,2022-12-28T16:30:00Z,,
+2022-12-29T00:00:00Z,2022-12-29T08:00:00Z,2022-12-29T16:30:00Z,,
+2022-12-30T00:00:00Z,2022-12-30T08:00:00Z,2022-12-30T13:15:00Z,,
+2023-01-02T00:00:00Z,2023-01-02T08:00:00Z,2023-01-02T16:30:00Z,,
+2023-01-03T00:00:00Z,2023-01-03T08:00:00Z,2023-01-03T16:30:00Z,,
+2023-01-04T00:00:00Z,2023-01-04T08:00:00Z,2023-01-04T16:30:00Z,,
+2023-01-05T00:00:00Z,2023-01-05T08:00:00Z,2023-01-05T16:30:00Z,,
+2023-01-06T00:00:00Z,2023-01-06T08:00:00Z,2023-01-06T16:30:00Z,,
+2023-01-09T00:00:00Z,2023-01-09T08:00:00Z,2023-01-09T16:30:00Z,,
+2023-01-10T00:00:00Z,2023-01-10T08:00:00Z,2023-01-10T16:30:00Z,,
+2023-01-11T00:00:00Z,2023-01-11T08:00:00Z,2023-01-11T16:30:00Z,,
+2023-01-12T00:00:00Z,2023-01-12T08:00:00Z,2023-01-12T16:30:00Z,,
+2023-01-13T00:00:00Z,2023-01-13T08:00:00Z,2023-01-13T16:30:00Z,,
+2023-01-16T00:00:00Z,2023-01-16T08:00:00Z,2023-01-16T16:30:00Z,,
+2023-01-17T00:00:00Z,2023-01-17T08:00:00Z,2023-01-17T16:30:00Z,,
+2023-01-18T00:00:00Z,2023-01-18T08:00:00Z,2023-01-18T16:30:00Z,,
+2023-01-19T00:00:00Z,2023-01-19T08:00:00Z,2023-01-19T16:30:00Z,,
+2023-01-20T00:00:00Z,2023-01-20T08:00:00Z,2023-01-20T16:30:00Z,,
+2023-01-23T00:00:00Z,2023-01-23T08:00:00Z,2023-01-23T16:30:00Z,,
+2023-01-24T00:00:00Z,2023-01-24T08:00:00Z,2023-01-24T16:30:00Z,,
+2023-01-25T00:00:00Z,2023-01-25T08:00:00Z,2023-01-25T16:30:00Z,,
+2023-01-26T00:00:00Z,2023-01-26T08:00:00Z,2023-01-26T16:30:00Z,,
+2023-01-27T00:00:00Z,2023-01-27T08:00:00Z,2023-01-27T16:30:00Z,,
+2023-01-30T00:00:00Z,2023-01-30T08:00:00Z,2023-01-30T16:30:00Z,,
+2023-01-31T00:00:00Z,2023-01-31T08:00:00Z,2023-01-31T16:30:00Z,,
+2023-02-01T00:00:00Z,2023-02-01T08:00:00Z,2023-02-01T16:30:00Z,,
+2023-02-02T00:00:00Z,2023-02-02T08:00:00Z,2023-02-02T16:30:00Z,,
+2023-02-03T00:00:00Z,2023-02-03T08:00:00Z,2023-02-03T16:30:00Z,,
+2023-02-06T00:00:00Z,2023-02-06T08:00:00Z,2023-02-06T16:30:00Z,,
+2023-02-07T00:00:00Z,2023-02-07T08:00:00Z,2023-02-07T16:30:00Z,,
+2023-02-08T00:00:00Z,2023-02-08T08:00:00Z,2023-02-08T16:30:00Z,,
+2023-02-09T00:00:00Z,2023-02-09T08:00:00Z,2023-02-09T16:30:00Z,,
+2023-02-10T00:00:00Z,2023-02-10T08:00:00Z,2023-02-10T16:30:00Z,,
+2023-02-13T00:00:00Z,2023-02-13T08:00:00Z,2023-02-13T16:30:00Z,,
+2023-02-14T00:00:00Z,2023-02-14T08:00:00Z,2023-02-14T16:30:00Z,,
+2023-02-15T00:00:00Z,2023-02-15T08:00:00Z,2023-02-15T16:30:00Z,,
+2023-02-16T00:00:00Z,2023-02-16T08:00:00Z,2023-02-16T16:30:00Z,,
+2023-02-17T00:00:00Z,2023-02-17T08:00:00Z,2023-02-17T16:30:00Z,,
+2023-02-20T00:00:00Z,2023-02-20T08:00:00Z,2023-02-20T16:30:00Z,,
+2023-02-21T00:00:00Z,2023-02-21T08:00:00Z,2023-02-21T16:30:00Z,,
+2023-02-22T00:00:00Z,2023-02-22T08:00:00Z,2023-02-22T16:30:00Z,,
+2023-02-23T00:00:00Z,2023-02-23T08:00:00Z,2023-02-23T16:30:00Z,,
+2023-02-24T00:00:00Z,2023-02-24T08:00:00Z,2023-02-24T16:30:00Z,,
+2023-02-27T00:00:00Z,2023-02-27T08:00:00Z,2023-02-27T16:30:00Z,,
+2023-02-28T00:00:00Z,2023-02-28T08:00:00Z,2023-02-28T16:30:00Z,,
+2023-03-01T00:00:00Z,2023-03-01T08:00:00Z,2023-03-01T16:30:00Z,,
+2023-03-02T00:00:00Z,2023-03-02T08:00:00Z,2023-03-02T16:30:00Z,,
+2023-03-03T00:00:00Z,2023-03-03T08:00:00Z,2023-03-03T16:30:00Z,,
+2023-03-06T00:00:00Z,2023-03-06T08:00:00Z,2023-03-06T16:30:00Z,,
+2023-03-07T00:00:00Z,2023-03-07T08:00:00Z,2023-03-07T16:30:00Z,,
+2023-03-08T00:00:00Z,2023-03-08T08:00:00Z,2023-03-08T16:30:00Z,,
+2023-03-09T00:00:00Z,2023-03-09T08:00:00Z,2023-03-09T16:30:00Z,,
+2023-03-10T00:00:00Z,2023-03-10T08:00:00Z,2023-03-10T16:30:00Z,,
+2023-03-13T00:00:00Z,2023-03-13T08:00:00Z,2023-03-13T16:30:00Z,,
+2023-03-14T00:00:00Z,2023-03-14T08:00:00Z,2023-03-14T16:30:00Z,,
+2023-03-15T00:00:00Z,2023-03-15T08:00:00Z,2023-03-15T16:30:00Z,,
+2023-03-16T00:00:00Z,2023-03-16T08:00:00Z,2023-03-16T16:30:00Z,,
+2023-03-17T00:00:00Z,2023-03-17T08:00:00Z,2023-03-17T16:30:00Z,,
+2023-03-20T00:00:00Z,2023-03-20T08:00:00Z,2023-03-20T16:30:00Z,,
+2023-03-21T00:00:00Z,2023-03-21T08:00:00Z,2023-03-21T16:30:00Z,,
+2023-03-22T00:00:00Z,2023-03-22T08:00:00Z,2023-03-22T16:30:00Z,,
+2023-03-23T00:00:00Z,2023-03-23T08:00:00Z,2023-03-23T16:30:00Z,,
+2023-03-24T00:00:00Z,2023-03-24T08:00:00Z,2023-03-24T16:30:00Z,,
+2023-03-27T00:00:00Z,2023-03-27T07:00:00Z,2023-03-27T15:30:00Z,,
+2023-03-28T00:00:00Z,2023-03-28T07:00:00Z,2023-03-28T15:30:00Z,,
+2023-03-29T00:00:00Z,2023-03-29T07:00:00Z,2023-03-29T15:30:00Z,,
+2023-03-30T00:00:00Z,2023-03-30T07:00:00Z,2023-03-30T15:30:00Z,,
+2023-03-31T00:00:00Z,2023-03-31T07:00:00Z,2023-03-31T15:30:00Z,,
+2023-04-03T00:00:00Z,2023-04-03T07:00:00Z,2023-04-03T15:30:00Z,,
+2023-04-04T00:00:00Z,2023-04-04T07:00:00Z,2023-04-04T15:30:00Z,,
+2023-04-05T00:00:00Z,2023-04-05T07:00:00Z,2023-04-05T15:30:00Z,,
+2023-04-06T00:00:00Z,2023-04-06T07:00:00Z,2023-04-06T15:30:00Z,,
+2023-04-11T00:00:00Z,2023-04-11T07:00:00Z,2023-04-11T15:30:00Z,,
+2023-04-12T00:00:00Z,2023-04-12T07:00:00Z,2023-04-12T15:30:00Z,,
+2023-04-13T00:00:00Z,2023-04-13T07:00:00Z,2023-04-13T15:30:00Z,,
+2023-04-14T00:00:00Z,2023-04-14T07:00:00Z,2023-04-14T15:30:00Z,,
+2023-04-17T00:00:00Z,2023-04-17T07:00:00Z,2023-04-17T15:30:00Z,,
+2023-04-18T00:00:00Z,2023-04-18T07:00:00Z,2023-04-18T15:30:00Z,,
+2023-04-19T00:00:00Z,2023-04-19T07:00:00Z,2023-04-19T15:30:00Z,,
+2023-04-20T00:00:00Z,2023-04-20T07:00:00Z,2023-04-20T15:30:00Z,,
+2023-04-21T00:00:00Z,2023-04-21T07:00:00Z,2023-04-21T15:30:00Z,,
+2023-04-24T00:00:00Z,2023-04-24T07:00:00Z,2023-04-24T15:30:00Z,,
+2023-04-25T00:00:00Z,2023-04-25T07:00:00Z,2023-04-25T15:30:00Z,,
+2023-04-26T00:00:00Z,2023-04-26T07:00:00Z,2023-04-26T15:30:00Z,,
+2023-04-27T00:00:00Z,2023-04-27T07:00:00Z,2023-04-27T15:30:00Z,,
+2023-04-28T00:00:00Z,2023-04-28T07:00:00Z,2023-04-28T15:30:00Z,,
+2023-05-02T00:00:00Z,2023-05-02T07:00:00Z,2023-05-02T15:30:00Z,,
+2023-05-03T00:00:00Z,2023-05-03T07:00:00Z,2023-05-03T15:30:00Z,,
+2023-05-04T00:00:00Z,2023-05-04T07:00:00Z,2023-05-04T15:30:00Z,,
+2023-05-05T00:00:00Z,2023-05-05T07:00:00Z,2023-05-05T15:30:00Z,,
+2023-05-08T00:00:00Z,2023-05-08T07:00:00Z,2023-05-08T15:30:00Z,,
+2023-05-09T00:00:00Z,2023-05-09T07:00:00Z,2023-05-09T15:30:00Z,,
+2023-05-10T00:00:00Z,2023-05-10T07:00:00Z,2023-05-10T15:30:00Z,,
+2023-05-11T00:00:00Z,2023-05-11T07:00:00Z,2023-05-11T15:30:00Z,,
+2023-05-12T00:00:00Z,2023-05-12T07:00:00Z,2023-05-12T15:30:00Z,,
+2023-05-15T00:00:00Z,2023-05-15T07:00:00Z,2023-05-15T15:30:00Z,,
+2023-05-16T00:00:00Z,2023-05-16T07:00:00Z,2023-05-16T15:30:00Z,,
+2023-05-17T00:00:00Z,2023-05-17T07:00:00Z,2023-05-17T15:30:00Z,,
+2023-05-18T00:00:00Z,2023-05-18T07:00:00Z,2023-05-18T15:30:00Z,,
+2023-05-19T00:00:00Z,2023-05-19T07:00:00Z,2023-05-19T15:30:00Z,,
+2023-05-22T00:00:00Z,2023-05-22T07:00:00Z,2023-05-22T15:30:00Z,,
+2023-05-23T00:00:00Z,2023-05-23T07:00:00Z,2023-05-23T15:30:00Z,,
+2023-05-24T00:00:00Z,2023-05-24T07:00:00Z,2023-05-24T15:30:00Z,,
+2023-05-25T00:00:00Z,2023-05-25T07:00:00Z,2023-05-25T15:30:00Z,,
+2023-05-26T00:00:00Z,2023-05-26T07:00:00Z,2023-05-26T15:30:00Z,,
+2023-05-29T00:00:00Z,2023-05-29T07:00:00Z,2023-05-29T15:30:00Z,,
+2023-05-30T00:00:00Z,2023-05-30T07:00:00Z,2023-05-30T15:30:00Z,,
+2023-05-31T00:00:00Z,2023-05-31T07:00:00Z,2023-05-31T15:30:00Z,,
+2023-06-01T00:00:00Z,2023-06-01T07:00:00Z,2023-06-01T15:30:00Z,,
+2023-06-02T00:00:00Z,2023-06-02T07:00:00Z,2023-06-02T15:30:00Z,,
+2023-06-05T00:00:00Z,2023-06-05T07:00:00Z,2023-06-05T15:30:00Z,,
+2023-06-06T00:00:00Z,2023-06-06T07:00:00Z,2023-06-06T15:30:00Z,,
+2023-06-07T00:00:00Z,2023-06-07T07:00:00Z,2023-06-07T15:30:00Z,,
+2023-06-08T00:00:00Z,2023-06-08T07:00:00Z,2023-06-08T15:30:00Z,,
+2023-06-09T00:00:00Z,2023-06-09T07:00:00Z,2023-06-09T15:30:00Z,,
+2023-06-12T00:00:00Z,2023-06-12T07:00:00Z,2023-06-12T15:30:00Z,,
+2023-06-13T00:00:00Z,2023-06-13T07:00:00Z,2023-06-13T15:30:00Z,,
+2023-06-14T00:00:00Z,2023-06-14T07:00:00Z,2023-06-14T15:30:00Z,,
+2023-06-15T00:00:00Z,2023-06-15T07:00:00Z,2023-06-15T15:30:00Z,,
+2023-06-16T00:00:00Z,2023-06-16T07:00:00Z,2023-06-16T15:30:00Z,,
+2023-06-19T00:00:00Z,2023-06-19T07:00:00Z,2023-06-19T15:30:00Z,,
+2023-06-20T00:00:00Z,2023-06-20T07:00:00Z,2023-06-20T15:30:00Z,,
+2023-06-21T00:00:00Z,2023-06-21T07:00:00Z,2023-06-21T15:30:00Z,,
+2023-06-22T00:00:00Z,2023-06-22T07:00:00Z,2023-06-22T15:30:00Z,,
+2023-06-23T00:00:00Z,2023-06-23T07:00:00Z,2023-06-23T15:30:00Z,,
+2023-06-26T00:00:00Z,2023-06-26T07:00:00Z,2023-06-26T15:30:00Z,,
+2023-06-27T00:00:00Z,2023-06-27T07:00:00Z,2023-06-27T15:30:00Z,,
+2023-06-28T00:00:00Z,2023-06-28T07:00:00Z,2023-06-28T15:30:00Z,,
+2023-06-29T00:00:00Z,2023-06-29T07:00:00Z,2023-06-29T15:30:00Z,,
+2023-06-30T00:00:00Z,2023-06-30T07:00:00Z,2023-06-30T15:30:00Z,,
+2023-07-03T00:00:00Z,2023-07-03T07:00:00Z,2023-07-03T15:30:00Z,,
+2023-07-04T00:00:00Z,2023-07-04T07:00:00Z,2023-07-04T15:30:00Z,,
+2023-07-05T00:00:00Z,2023-07-05T07:00:00Z,2023-07-05T15:30:00Z,,
+2023-07-06T00:00:00Z,2023-07-06T07:00:00Z,2023-07-06T15:30:00Z,,
+2023-07-07T00:00:00Z,2023-07-07T07:00:00Z,2023-07-07T15:30:00Z,,
+2023-07-10T00:00:00Z,2023-07-10T07:00:00Z,2023-07-10T15:30:00Z,,
+2023-07-11T00:00:00Z,2023-07-11T07:00:00Z,2023-07-11T15:30:00Z,,
+2023-07-12T00:00:00Z,2023-07-12T07:00:00Z,2023-07-12T15:30:00Z,,
+2023-07-13T00:00:00Z,2023-07-13T07:00:00Z,2023-07-13T15:30:00Z,,
+2023-07-14T00:00:00Z,2023-07-14T07:00:00Z,2023-07-14T15:30:00Z,,
+2023-07-17T00:00:00Z,2023-07-17T07:00:00Z,2023-07-17T15:30:00Z,,
+2023-07-18T00:00:00Z,2023-07-18T07:00:00Z,2023-07-18T15:30:00Z,,
+2023-07-19T00:00:00Z,2023-07-19T07:00:00Z,2023-07-19T15:30:00Z,,
+2023-07-20T00:00:00Z,2023-07-20T07:00:00Z,2023-07-20T15:30:00Z,,
+2023-07-21T00:00:00Z,2023-07-21T07:00:00Z,2023-07-21T15:30:00Z,,
+2023-07-24T00:00:00Z,2023-07-24T07:00:00Z,2023-07-24T15:30:00Z,,
+2023-07-25T00:00:00Z,2023-07-25T07:00:00Z,2023-07-25T15:30:00Z,,
+2023-07-26T00:00:00Z,2023-07-26T07:00:00Z,2023-07-26T15:30:00Z,,
+2023-07-27T00:00:00Z,2023-07-27T07:00:00Z,2023-07-27T15:30:00Z,,
+2023-07-28T00:00:00Z,2023-07-28T07:00:00Z,2023-07-28T15:30:00Z,,
+2023-07-31T00:00:00Z,2023-07-31T07:00:00Z,2023-07-31T15:30:00Z,,
+2023-08-01T00:00:00Z,2023-08-01T07:00:00Z,2023-08-01T15:30:00Z,,
+2023-08-02T00:00:00Z,2023-08-02T07:00:00Z,2023-08-02T15:30:00Z,,
+2023-08-03T00:00:00Z,2023-08-03T07:00:00Z,2023-08-03T15:30:00Z,,
+2023-08-04T00:00:00Z,2023-08-04T07:00:00Z,2023-08-04T15:30:00Z,,
+2023-08-07T00:00:00Z,2023-08-07T07:00:00Z,2023-08-07T15:30:00Z,,
+2023-08-08T00:00:00Z,2023-08-08T07:00:00Z,2023-08-08T15:30:00Z,,
+2023-08-09T00:00:00Z,2023-08-09T07:00:00Z,2023-08-09T15:30:00Z,,
+2023-08-10T00:00:00Z,2023-08-10T07:00:00Z,2023-08-10T15:30:00Z,,
+2023-08-11T00:00:00Z,2023-08-11T07:00:00Z,2023-08-11T15:30:00Z,,
+2023-08-14T00:00:00Z,2023-08-14T07:00:00Z,2023-08-14T15:30:00Z,,
+2023-08-15T00:00:00Z,2023-08-15T07:00:00Z,2023-08-15T15:30:00Z,,
+2023-08-16T00:00:00Z,2023-08-16T07:00:00Z,2023-08-16T15:30:00Z,,
+2023-08-17T00:00:00Z,2023-08-17T07:00:00Z,2023-08-17T15:30:00Z,,
+2023-08-18T00:00:00Z,2023-08-18T07:00:00Z,2023-08-18T15:30:00Z,,
+2023-08-21T00:00:00Z,2023-08-21T07:00:00Z,2023-08-21T15:30:00Z,,
+2023-08-22T00:00:00Z,2023-08-22T07:00:00Z,2023-08-22T15:30:00Z,,
+2023-08-23T00:00:00Z,2023-08-23T07:00:00Z,2023-08-23T15:30:00Z,,
+2023-08-24T00:00:00Z,2023-08-24T07:00:00Z,2023-08-24T15:30:00Z,,
+2023-08-25T00:00:00Z,2023-08-25T07:00:00Z,2023-08-25T15:30:00Z,,
+2023-08-28T00:00:00Z,2023-08-28T07:00:00Z,2023-08-28T15:30:00Z,,
+2023-08-29T00:00:00Z,2023-08-29T07:00:00Z,2023-08-29T15:30:00Z,,
+2023-08-30T00:00:00Z,2023-08-30T07:00:00Z,2023-08-30T15:30:00Z,,
+2023-08-31T00:00:00Z,2023-08-31T07:00:00Z,2023-08-31T15:30:00Z,,
+2023-09-01T00:00:00Z,2023-09-01T07:00:00Z,2023-09-01T15:30:00Z,,
+2023-09-04T00:00:00Z,2023-09-04T07:00:00Z,2023-09-04T15:30:00Z,,
+2023-09-05T00:00:00Z,2023-09-05T07:00:00Z,2023-09-05T15:30:00Z,,
+2023-09-06T00:00:00Z,2023-09-06T07:00:00Z,2023-09-06T15:30:00Z,,
+2023-09-07T00:00:00Z,2023-09-07T07:00:00Z,2023-09-07T15:30:00Z,,
+2023-09-08T00:00:00Z,2023-09-08T07:00:00Z,2023-09-08T15:30:00Z,,
+2023-09-11T00:00:00Z,2023-09-11T07:00:00Z,2023-09-11T15:30:00Z,,
+2023-09-12T00:00:00Z,2023-09-12T07:00:00Z,2023-09-12T15:30:00Z,,
+2023-09-13T00:00:00Z,2023-09-13T07:00:00Z,2023-09-13T15:30:00Z,,
+2023-09-14T00:00:00Z,2023-09-14T07:00:00Z,2023-09-14T15:30:00Z,,
+2023-09-15T00:00:00Z,2023-09-15T07:00:00Z,2023-09-15T15:30:00Z,,
+2023-09-18T00:00:00Z,2023-09-18T07:00:00Z,2023-09-18T15:30:00Z,,
+2023-09-19T00:00:00Z,2023-09-19T07:00:00Z,2023-09-19T15:30:00Z,,
+2023-09-20T00:00:00Z,2023-09-20T07:00:00Z,2023-09-20T15:30:00Z,,
+2023-09-21T00:00:00Z,2023-09-21T07:00:00Z,2023-09-21T15:30:00Z,,
+2023-09-22T00:00:00Z,2023-09-22T07:00:00Z,2023-09-22T15:30:00Z,,
+2023-09-25T00:00:00Z,2023-09-25T07:00:00Z,2023-09-25T15:30:00Z,,
+2023-09-26T00:00:00Z,2023-09-26T07:00:00Z,2023-09-26T15:30:00Z,,
+2023-09-27T00:00:00Z,2023-09-27T07:00:00Z,2023-09-27T15:30:00Z,,
+2023-09-28T00:00:00Z,2023-09-28T07:00:00Z,2023-09-28T15:30:00Z,,
+2023-09-29T00:00:00Z,2023-09-29T07:00:00Z,2023-09-29T15:30:00Z,,
+2023-10-02T00:00:00Z,2023-10-02T07:00:00Z,2023-10-02T15:30:00Z,,
+2023-10-03T00:00:00Z,2023-10-03T07:00:00Z,2023-10-03T15:30:00Z,,
+2023-10-04T00:00:00Z,2023-10-04T07:00:00Z,2023-10-04T15:30:00Z,,
+2023-10-05T00:00:00Z,2023-10-05T07:00:00Z,2023-10-05T15:30:00Z,,
+2023-10-06T00:00:00Z,2023-10-06T07:00:00Z,2023-10-06T15:30:00Z,,
+2023-10-09T00:00:00Z,2023-10-09T07:00:00Z,2023-10-09T15:30:00Z,,
+2023-10-10T00:00:00Z,2023-10-10T07:00:00Z,2023-10-10T15:30:00Z,,
+2023-10-11T00:00:00Z,2023-10-11T07:00:00Z,2023-10-11T15:30:00Z,,
+2023-10-12T00:00:00Z,2023-10-12T07:00:00Z,2023-10-12T15:30:00Z,,
+2023-10-13T00:00:00Z,2023-10-13T07:00:00Z,2023-10-13T15:30:00Z,,
+2023-10-16T00:00:00Z,2023-10-16T07:00:00Z,2023-10-16T15:30:00Z,,
+2023-10-17T00:00:00Z,2023-10-17T07:00:00Z,2023-10-17T15:30:00Z,,
+2023-10-18T00:00:00Z,2023-10-18T07:00:00Z,2023-10-18T15:30:00Z,,
+2023-10-19T00:00:00Z,2023-10-19T07:00:00Z,2023-10-19T15:30:00Z,,
+2023-10-20T00:00:00Z,2023-10-20T07:00:00Z,2023-10-20T15:30:00Z,,
+2023-10-23T00:00:00Z,2023-10-23T07:00:00Z,2023-10-23T15:30:00Z,,
+2023-10-24T00:00:00Z,2023-10-24T07:00:00Z,2023-10-24T15:30:00Z,,
+2023-10-25T00:00:00Z,2023-10-25T07:00:00Z,2023-10-25T15:30:00Z,,
+2023-10-27T00:00:00Z,2023-10-27T07:00:00Z,2023-10-27T15:30:00Z,,
+2023-10-30T00:00:00Z,2023-10-30T08:00:00Z,2023-10-30T16:30:00Z,,
+2023-10-31T00:00:00Z,2023-10-31T08:00:00Z,2023-10-31T16:30:00Z,,
+2023-11-01T00:00:00Z,2023-11-01T08:00:00Z,2023-11-01T16:30:00Z,,
+2023-11-02T00:00:00Z,2023-11-02T08:00:00Z,2023-11-02T16:30:00Z,,
+2023-11-03T00:00:00Z,2023-11-03T08:00:00Z,2023-11-03T16:30:00Z,,
+2023-11-06T00:00:00Z,2023-11-06T08:00:00Z,2023-11-06T16:30:00Z,,
+2023-11-07T00:00:00Z,2023-11-07T08:00:00Z,2023-11-07T16:30:00Z,,
+2023-11-08T00:00:00Z,2023-11-08T08:00:00Z,2023-11-08T16:30:00Z,,
+2023-11-09T00:00:00Z,2023-11-09T08:00:00Z,2023-11-09T16:30:00Z,,
+2023-11-10T00:00:00Z,2023-11-10T08:00:00Z,2023-11-10T16:30:00Z,,
+2023-11-13T00:00:00Z,2023-11-13T08:00:00Z,2023-11-13T16:30:00Z,,
+2023-11-14T00:00:00Z,2023-11-14T08:00:00Z,2023-11-14T16:30:00Z,,
+2023-11-15T00:00:00Z,2023-11-15T08:00:00Z,2023-11-15T16:30:00Z,,
+2023-11-16T00:00:00Z,2023-11-16T08:00:00Z,2023-11-16T16:30:00Z,,
+2023-11-17T00:00:00Z,2023-11-17T08:00:00Z,2023-11-17T16:30:00Z,,
+2023-11-20T00:00:00Z,2023-11-20T08:00:00Z,2023-11-20T16:30:00Z,,
+2023-11-21T00:00:00Z,2023-11-21T08:00:00Z,2023-11-21T16:30:00Z,,
+2023-11-22T00:00:00Z,2023-11-22T08:00:00Z,2023-11-22T16:30:00Z,,
+2023-11-23T00:00:00Z,2023-11-23T08:00:00Z,2023-11-23T16:30:00Z,,
+2023-11-24T00:00:00Z,2023-11-24T08:00:00Z,2023-11-24T16:30:00Z,,
+2023-11-27T00:00:00Z,2023-11-27T08:00:00Z,2023-11-27T16:30:00Z,,
+2023-11-28T00:00:00Z,2023-11-28T08:00:00Z,2023-11-28T16:30:00Z,,
+2023-11-29T00:00:00Z,2023-11-29T08:00:00Z,2023-11-29T16:30:00Z,,
+2023-11-30T00:00:00Z,2023-11-30T08:00:00Z,2023-11-30T16:30:00Z,,
+2023-12-01T00:00:00Z,2023-12-01T08:00:00Z,2023-12-01T16:30:00Z,,
+2023-12-04T00:00:00Z,2023-12-04T08:00:00Z,2023-12-04T16:30:00Z,,
+2023-12-05T00:00:00Z,2023-12-05T08:00:00Z,2023-12-05T16:30:00Z,,
+2023-12-06T00:00:00Z,2023-12-06T08:00:00Z,2023-12-06T16:30:00Z,,
+2023-12-07T00:00:00Z,2023-12-07T08:00:00Z,2023-12-07T16:30:00Z,,
+2023-12-08T00:00:00Z,2023-12-08T08:00:00Z,2023-12-08T16:30:00Z,,
+2023-12-11T00:00:00Z,2023-12-11T08:00:00Z,2023-12-11T16:30:00Z,,
+2023-12-12T00:00:00Z,2023-12-12T08:00:00Z,2023-12-12T16:30:00Z,,
+2023-12-13T00:00:00Z,2023-12-13T08:00:00Z,2023-12-13T16:30:00Z,,
+2023-12-14T00:00:00Z,2023-12-14T08:00:00Z,2023-12-14T16:30:00Z,,
+2023-12-15T00:00:00Z,2023-12-15T08:00:00Z,2023-12-15T16:30:00Z,,
+2023-12-18T00:00:00Z,2023-12-18T08:00:00Z,2023-12-18T16:30:00Z,,
+2023-12-19T00:00:00Z,2023-12-19T08:00:00Z,2023-12-19T16:30:00Z,,
+2023-12-20T00:00:00Z,2023-12-20T08:00:00Z,2023-12-20T16:30:00Z,,
+2023-12-21T00:00:00Z,2023-12-21T08:00:00Z,2023-12-21T16:30:00Z,,
+2023-12-22T00:00:00Z,2023-12-22T08:00:00Z,2023-12-22T16:30:00Z,,
+2023-12-27T00:00:00Z,2023-12-27T08:00:00Z,2023-12-27T16:30:00Z,,
+2023-12-28T00:00:00Z,2023-12-28T08:00:00Z,2023-12-28T16:30:00Z,,
+2023-12-29T00:00:00Z,2023-12-29T08:00:00Z,2023-12-29T13:15:00Z,,
+2024-01-02T00:00:00Z,2024-01-02T08:00:00Z,2024-01-02T16:30:00Z,,
+2024-01-03T00:00:00Z,2024-01-03T08:00:00Z,2024-01-03T16:30:00Z,,
+2024-01-04T00:00:00Z,2024-01-04T08:00:00Z,2024-01-04T16:30:00Z,,
+2024-01-05T00:00:00Z,2024-01-05T08:00:00Z,2024-01-05T16:30:00Z,,
+2024-01-08T00:00:00Z,2024-01-08T08:00:00Z,2024-01-08T16:30:00Z,,
+2024-01-09T00:00:00Z,2024-01-09T08:00:00Z,2024-01-09T16:30:00Z,,
+2024-01-10T00:00:00Z,2024-01-10T08:00:00Z,2024-01-10T16:30:00Z,,
+2024-01-11T00:00:00Z,2024-01-11T08:00:00Z,2024-01-11T16:30:00Z,,
+2024-01-12T00:00:00Z,2024-01-12T08:00:00Z,2024-01-12T16:30:00Z,,
+2024-01-15T00:00:00Z,2024-01-15T08:00:00Z,2024-01-15T16:30:00Z,,
+2024-01-16T00:00:00Z,2024-01-16T08:00:00Z,2024-01-16T16:30:00Z,,
+2024-01-17T00:00:00Z,2024-01-17T08:00:00Z,2024-01-17T16:30:00Z,,
+2024-01-18T00:00:00Z,2024-01-18T08:00:00Z,2024-01-18T16:30:00Z,,
+2024-01-19T00:00:00Z,2024-01-19T08:00:00Z,2024-01-19T16:30:00Z,,
+2024-01-22T00:00:00Z,2024-01-22T08:00:00Z,2024-01-22T16:30:00Z,,
+2024-01-23T00:00:00Z,2024-01-23T08:00:00Z,2024-01-23T16:30:00Z,,
+2024-01-24T00:00:00Z,2024-01-24T08:00:00Z,2024-01-24T16:30:00Z,,
+2024-01-25T00:00:00Z,2024-01-25T08:00:00Z,2024-01-25T16:30:00Z,,
+2024-01-26T00:00:00Z,2024-01-26T08:00:00Z,2024-01-26T16:30:00Z,,
+2024-01-29T00:00:00Z,2024-01-29T08:00:00Z,2024-01-29T16:30:00Z,,
+2024-01-30T00:00:00Z,2024-01-30T08:00:00Z,2024-01-30T16:30:00Z,,
+2024-01-31T00:00:00Z,2024-01-31T08:00:00Z,2024-01-31T16:30:00Z,,
+2024-02-01T00:00:00Z,2024-02-01T08:00:00Z,2024-02-01T16:30:00Z,,
+2024-02-02T00:00:00Z,2024-02-02T08:00:00Z,2024-02-02T16:30:00Z,,
+2024-02-05T00:00:00Z,2024-02-05T08:00:00Z,2024-02-05T16:30:00Z,,
+2024-02-06T00:00:00Z,2024-02-06T08:00:00Z,2024-02-06T16:30:00Z,,
+2024-02-07T00:00:00Z,2024-02-07T08:00:00Z,2024-02-07T16:30:00Z,,
+2024-02-08T00:00:00Z,2024-02-08T08:00:00Z,2024-02-08T16:30:00Z,,
+2024-02-09T00:00:00Z,2024-02-09T08:00:00Z,2024-02-09T16:30:00Z,,
+2024-02-12T00:00:00Z,2024-02-12T08:00:00Z,2024-02-12T16:30:00Z,,
+2024-02-13T00:00:00Z,2024-02-13T08:00:00Z,2024-02-13T16:30:00Z,,
+2024-02-14T00:00:00Z,2024-02-14T08:00:00Z,2024-02-14T16:30:00Z,,
+2024-02-15T00:00:00Z,2024-02-15T08:00:00Z,2024-02-15T16:30:00Z,,
+2024-02-16T00:00:00Z,2024-02-16T08:00:00Z,2024-02-16T16:30:00Z,,
+2024-02-19T00:00:00Z,2024-02-19T08:00:00Z,2024-02-19T16:30:00Z,,
+2024-02-20T00:00:00Z,2024-02-20T08:00:00Z,2024-02-20T16:30:00Z,,
+2024-02-21T00:00:00Z,2024-02-21T08:00:00Z,2024-02-21T16:30:00Z,,
+2024-02-22T00:00:00Z,2024-02-22T08:00:00Z,2024-02-22T16:30:00Z,,
+2024-02-23T00:00:00Z,2024-02-23T08:00:00Z,2024-02-23T16:30:00Z,,
+2024-02-26T00:00:00Z,2024-02-26T08:00:00Z,2024-02-26T16:30:00Z,,
+2024-02-27T00:00:00Z,2024-02-27T08:00:00Z,2024-02-27T16:30:00Z,,
+2024-02-28T00:00:00Z,2024-02-28T08:00:00Z,2024-02-28T16:30:00Z,,
+2024-02-29T00:00:00Z,2024-02-29T08:00:00Z,2024-02-29T16:30:00Z,,
+2024-03-01T00:00:00Z,2024-03-01T08:00:00Z,2024-03-01T16:30:00Z,,
+2024-03-04T00:00:00Z,2024-03-04T08:00:00Z,2024-03-04T16:30:00Z,,
+2024-03-05T00:00:00Z,2024-03-05T08:00:00Z,2024-03-05T16:30:00Z,,
+2024-03-06T00:00:00Z,2024-03-06T08:00:00Z,2024-03-06T16:30:00Z,,
+2024-03-07T00:00:00Z,2024-03-07T08:00:00Z,2024-03-07T16:30:00Z,,
+2024-03-08T00:00:00Z,2024-03-08T08:00:00Z,2024-03-08T16:30:00Z,,
+2024-03-11T00:00:00Z,2024-03-11T08:00:00Z,2024-03-11T16:30:00Z,,
+2024-03-12T00:00:00Z,2024-03-12T08:00:00Z,2024-03-12T16:30:00Z,,
+2024-03-13T00:00:00Z,2024-03-13T08:00:00Z,2024-03-13T16:30:00Z,,
+2024-03-14T00:00:00Z,2024-03-14T08:00:00Z,2024-03-14T16:30:00Z,,
+2024-03-15T00:00:00Z,2024-03-15T08:00:00Z,2024-03-15T16:30:00Z,,
+2024-03-18T00:00:00Z,2024-03-18T08:00:00Z,2024-03-18T16:30:00Z,,
+2024-03-19T00:00:00Z,2024-03-19T08:00:00Z,2024-03-19T16:30:00Z,,
+2024-03-20T00:00:00Z,2024-03-20T08:00:00Z,2024-03-20T16:30:00Z,,
+2024-03-21T00:00:00Z,2024-03-21T08:00:00Z,2024-03-21T16:30:00Z,,
+2024-03-22T00:00:00Z,2024-03-22T08:00:00Z,2024-03-22T16:30:00Z,,
+2024-03-25T00:00:00Z,2024-03-25T08:00:00Z,2024-03-25T16:30:00Z,,
+2024-03-26T00:00:00Z,2024-03-26T08:00:00Z,2024-03-26T16:30:00Z,,
+2024-03-27T00:00:00Z,2024-03-27T08:00:00Z,2024-03-27T16:30:00Z,,
+2024-03-28T00:00:00Z,2024-03-28T08:00:00Z,2024-03-28T16:30:00Z,,
+2024-04-02T00:00:00Z,2024-04-02T07:00:00Z,2024-04-02T15:30:00Z,,
+2024-04-03T00:00:00Z,2024-04-03T07:00:00Z,2024-04-03T15:30:00Z,,
+2024-04-04T00:00:00Z,2024-04-04T07:00:00Z,2024-04-04T15:30:00Z,,
+2024-04-05T00:00:00Z,2024-04-05T07:00:00Z,2024-04-05T15:30:00Z,,
+2024-04-08T00:00:00Z,2024-04-08T07:00:00Z,2024-04-08T15:30:00Z,,
+2024-04-09T00:00:00Z,2024-04-09T07:00:00Z,2024-04-09T15:30:00Z,,
+2024-04-10T00:00:00Z,2024-04-10T07:00:00Z,2024-04-10T15:30:00Z,,
+2024-04-11T00:00:00Z,2024-04-11T07:00:00Z,2024-04-11T15:30:00Z,,
+2024-04-12T00:00:00Z,2024-04-12T07:00:00Z,2024-04-12T15:30:00Z,,
+2024-04-15T00:00:00Z,2024-04-15T07:00:00Z,2024-04-15T15:30:00Z,,
+2024-04-16T00:00:00Z,2024-04-16T07:00:00Z,2024-04-16T15:30:00Z,,
+2024-04-17T00:00:00Z,2024-04-17T07:00:00Z,2024-04-17T15:30:00Z,,
+2024-04-18T00:00:00Z,2024-04-18T07:00:00Z,2024-04-18T15:30:00Z,,
+2024-04-19T00:00:00Z,2024-04-19T07:00:00Z,2024-04-19T15:30:00Z,,
+2024-04-22T00:00:00Z,2024-04-22T07:00:00Z,2024-04-22T15:30:00Z,,
+2024-04-23T00:00:00Z,2024-04-23T07:00:00Z,2024-04-23T15:30:00Z,,
+2024-04-24T00:00:00Z,2024-04-24T07:00:00Z,2024-04-24T15:30:00Z,,
+2024-04-25T00:00:00Z,2024-04-25T07:00:00Z,2024-04-25T15:30:00Z,,
+2024-04-26T00:00:00Z,2024-04-26T07:00:00Z,2024-04-26T15:30:00Z,,
+2024-04-29T00:00:00Z,2024-04-29T07:00:00Z,2024-04-29T15:30:00Z,,
+2024-04-30T00:00:00Z,2024-04-30T07:00:00Z,2024-04-30T15:30:00Z,,
+2024-05-02T00:00:00Z,2024-05-02T07:00:00Z,2024-05-02T15:30:00Z,,
```

### Comparing `exchange_calendars-4.2.6/tests/test_aixk_calendar.py` & `exchange_calendars-4.2.7/tests/test_aixk_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_always_open.py` & `exchange_calendars-4.2.7/tests/test_always_open.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_asex_calendar.py` & `exchange_calendars-4.2.7/tests/test_asex_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_bvmf_calendar.py` & `exchange_calendars-4.2.7/tests/test_bvmf_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_calendar_dispatcher.py` & `exchange_calendars-4.2.7/tests/test_calendar_dispatcher.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_calendar_helpers.py` & `exchange_calendars-4.2.7/tests/test_calendar_helpers.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_cmes_calendar.py` & `exchange_calendars-4.2.7/tests/test_cmes_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_exchange_calendar.py` & `exchange_calendars-4.2.7/tests/test_exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_iepa_calendar.py` & `exchange_calendars-4.2.7/tests/test_iepa_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_weekday_calendar.py` & `exchange_calendars-4.2.7/tests/test_weekday_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xams_calendar.py` & `exchange_calendars-4.2.7/tests/test_xams_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xasx_calendar.py` & `exchange_calendars-4.2.7/tests/test_xasx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xbkk_calendar.py` & `exchange_calendars-4.2.7/tests/test_xbkk_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xbog_calendar.py` & `exchange_calendars-4.2.7/tests/test_xbog_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xbom_calendar.py` & `exchange_calendars-4.2.7/tests/test_xbom_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xbru_calendar.py` & `exchange_calendars-4.2.7/tests/test_xbru_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xbse_calendar.py` & `exchange_calendars-4.2.7/tests/test_xbse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xbud_calendar.py` & `exchange_calendars-4.2.7/tests/test_xbud_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xbue_calendar.py` & `exchange_calendars-4.2.7/tests/test_xbue_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xcbf_calendar.py` & `exchange_calendars-4.2.7/tests/test_xcbf_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xcse_calendar.py` & `exchange_calendars-4.2.7/tests/test_xcse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xdub_calendar.py` & `exchange_calendars-4.2.7/tests/test_xdub_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xetr_calendar.py` & `exchange_calendars-4.2.7/tests/test_xetr_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xfra_calendar.py` & `exchange_calendars-4.2.7/tests/test_xfra_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xhel_calendar.py` & `exchange_calendars-4.2.7/tests/test_xhel_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xhkg_calendar.py` & `exchange_calendars-4.2.7/tests/test_xhkg_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xice_calendar.py` & `exchange_calendars-4.2.7/tests/test_xice_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xidx_calendar.py` & `exchange_calendars-4.2.7/tests/test_xidx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xist_calendar.py` & `exchange_calendars-4.2.7/tests/test_xist_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xjse_calendar.py` & `exchange_calendars-4.2.7/tests/test_xjse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xkar_calendar.py` & `exchange_calendars-4.2.7/tests/test_xkar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xkls_calendar.py` & `exchange_calendars-4.2.7/tests/test_xkls_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xkrx_calendar.py` & `exchange_calendars-4.2.7/tests/test_xkrx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xlim_calendar.py` & `exchange_calendars-4.2.7/tests/test_xlim_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xlis_calendar.py` & `exchange_calendars-4.2.7/tests/test_xlis_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xlon_calendar.py` & `exchange_calendars-4.2.7/tests/test_xlon_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xmad_calendar.py` & `exchange_calendars-4.2.7/tests/test_xmad_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xmex_calendar.py` & `exchange_calendars-4.2.7/tests/test_xmex_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xmil_calendar.py` & `exchange_calendars-4.2.7/tests/test_xmil_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xmos_calendar.py` & `exchange_calendars-4.2.7/tests/test_xmos_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xnys_calendar.py` & `exchange_calendars-4.2.7/tests/test_xnys_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xnze_calendar.py` & `exchange_calendars-4.2.7/tests/test_xnze_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xosl_calendar.py` & `exchange_calendars-4.2.7/tests/test_xosl_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xpar_calendar.py` & `exchange_calendars-4.2.7/tests/test_xpar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xphs_calendar.py` & `exchange_calendars-4.2.7/tests/test_xphs_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xpra_calendar.py` & `exchange_calendars-4.2.7/tests/test_xpra_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xses_calendar.py` & `exchange_calendars-4.2.7/tests/test_xses_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xsgo_calendar.py` & `exchange_calendars-4.2.7/tests/test_xsgo_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xshg_calendar.py` & `exchange_calendars-4.2.7/tests/test_xshg_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xsto_calendar.py` & `exchange_calendars-4.2.7/tests/test_xsto_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xswx_calendar.py` & `exchange_calendars-4.2.7/tests/test_xswx_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xtae_calendar.py` & `exchange_calendars-4.2.7/tests/test_xtae_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xtai_calendar.py` & `exchange_calendars-4.2.7/tests/test_xtai_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xtks_calendar.py` & `exchange_calendars-4.2.7/tests/test_xtks_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xtse_calendar.py` & `exchange_calendars-4.2.7/tests/test_xtse_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xwar_calendar.py` & `exchange_calendars-4.2.7/tests/test_xwar_calendar.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars-4.2.6/tests/test_xwbo_calendar.py` & `exchange_calendars-4.2.7/tests/test_xwbo_calendar.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,16 @@
             "2011-12-23",
             "2011-12-27",
             #
             # New Year's Eve not made up since 2016. Ensure day on which previously
             # made up (prior Friday) is not a holiday.
             "2016-12-30",
             "2017-12-29",
+            # Whit Monday was a trading day in 2023
+            "2023-05-29",
         ]
 
     @pytest.fixture
     def early_closes_sample(self):
         yield [
             # Last trading day preceeding New Year's Eve
             "2017-12-29",
```

