# Comparing `tmp/hftbacktest-1.5.4.tar.gz` & `tmp/hftbacktest-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hftbacktest-1.5.4.tar", last modified: Sun Apr 30 14:11:12 2023, max compression
+gzip compressed data, was "hftbacktest-1.5.5.tar", last modified: Wed May 10 15:04:42 2023, max compression
```

## Comparing `hftbacktest-1.5.4.tar` & `hftbacktest-1.5.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/LICENSE
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6815 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5706 2023-04-30 12:46:55.000000 hftbacktest-1.5.4/README.rst
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.329382 hftbacktest-1.5.4/hftbacktest/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11501 2023-04-30 14:07:40.000000 hftbacktest-1.5.4/hftbacktest/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/assettype.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14547 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.329382 hftbacktest-1.5.4/hftbacktest/data/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/data/__init__.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/data/utils/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/data/utils/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11484 2023-04-28 13:21:33.000000 hftbacktest-1.5.4/hftbacktest/data/utils/binancefutures.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.5.4/hftbacktest/data/utils/snapshot.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.5.4/hftbacktest/data/utils/tardis.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.5.4/hftbacktest/data/validation.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/experimental/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14453 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/backtest.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/experimental/live/
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/__init__.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/binancefutures.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/custom_strategy.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/ordermanager.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/live/settings.py
--rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6821 2023-04-29 10:30:43.000000 hftbacktest-1.5.4/hftbacktest/experimental/multiassetinit.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/marketdepth.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/models/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/models/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-04-29 14:47:02.000000 hftbacktest-1.5.4/hftbacktest/models/latencies.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/models/queue.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4143 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/order.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.330382 hftbacktest-1.5.4/hftbacktest/proc/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/__init__.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5866 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/local.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14794 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/nopartialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    22145 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/partialfillexchange.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5903 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/proc/proc.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/reader.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13631 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/stat.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/state.py
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/hftbacktest/typing.py
-drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-30 14:11:12.329382 hftbacktest-1.5.4/hftbacktest.egg-info/
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6815 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/PKG-INFO
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1252 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/SOURCES.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/dependency_links.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.5.4/hftbacktest.egg-info/not-zip-safe
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/requires.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-04-30 14:11:12.000000 hftbacktest-1.5.4/hftbacktest.egg-info/top_level.txt
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-04-30 14:11:12.331382 hftbacktest-1.5.4/setup.cfg
--rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.5.4/setup.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1079 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/LICENSE
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5696 2023-05-10 14:57:57.000000 hftbacktest-1.5.5/README.rst
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11501 2023-05-10 14:57:27.000000 hftbacktest-1.5.5/hftbacktest/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1011 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/assettype.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14547 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/data/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1592 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/data/__init__.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/data/utils/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       44 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/data/utils/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11484 2023-04-28 13:21:33.000000 hftbacktest-1.5.5/hftbacktest/data/utils/binancefutures.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2160 2023-04-30 14:00:09.000000 hftbacktest-1.5.5/hftbacktest/data/utils/snapshot.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6901 2023-04-28 13:18:47.000000 hftbacktest-1.5.5/hftbacktest/data/utils/tardis.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    11553 2023-04-28 12:19:24.000000 hftbacktest-1.5.5/hftbacktest/data/validation.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/experimental/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    14453 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/backtest.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest/experimental/live/
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/__init__.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)    19630 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/binancefutures.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)      333 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/custom_strategy.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     7792 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/ordermanager.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     3578 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/live/settings.py
+-rwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)     6821 2023-04-29 10:30:43.000000 hftbacktest-1.5.5/hftbacktest/experimental/multiassetinit.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6194 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/marketdepth.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/hftbacktest/models/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/models/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    10010 2023-04-29 14:47:02.000000 hftbacktest-1.5.5/hftbacktest/models/latencies.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3305 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/models/queue.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     4139 2023-05-10 12:56:12.000000 hftbacktest-1.5.5/hftbacktest/order.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/hftbacktest/proc/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        0 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/proc/__init__.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5866 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/proc/local.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    14794 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/proc/nopartialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    22145 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/proc/partialfillexchange.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     5899 2023-05-10 12:56:12.000000 hftbacktest-1.5.5/hftbacktest/proc/proc.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     3252 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/reader.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)    13687 2023-05-10 13:22:50.000000 hftbacktest-1.5.5/hftbacktest/stat.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     2149 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/state.py
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)      876 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/hftbacktest/typing.py
+drwxr-xr-x   0 nkaz001   (1000) nkaz001   (1000)        0 2023-05-10 15:04:42.471240 hftbacktest-1.5.5/hftbacktest.egg-info/
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     6805 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/PKG-INFO
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1252 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/SOURCES.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/dependency_links.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)        1 2023-04-28 14:15:39.000000 hftbacktest-1.5.5/hftbacktest.egg-info/not-zip-safe
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       48 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/requires.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       12 2023-05-10 15:04:42.000000 hftbacktest-1.5.5/hftbacktest.egg-info/top_level.txt
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)     1249 2023-05-10 15:04:42.472240 hftbacktest-1.5.5/setup.cfg
+-rw-r--r--   0 nkaz001   (1000) nkaz001   (1000)       61 2023-04-27 05:42:48.000000 hftbacktest-1.5.5/setup.py
```

### Comparing `hftbacktest-1.5.4/LICENSE` & `hftbacktest-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/PKG-INFO` & `hftbacktest-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.4
+Version: 1.5.5
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -43,15 +43,15 @@
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
 * Backtest accounting for both feed and order latency, using provided models or your own custom model.
 * Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
 
 Documentation
 =============
 
-See `full document here <https://hftbacktest.readthedocs.io/en/latest/>`_.
+See `full document here <https://hftbacktest.readthedocs.io/>`_.
 
 Getting started
 ===============
 
 Installation
 ------------
```

### Comparing `hftbacktest-1.5.4/README.rst` & `hftbacktest-1.5.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
 * Backtest accounting for both feed and order latency, using provided models or your own custom model.
 * Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
 
 Documentation
 =============
 
-See `full document here <https://hftbacktest.readthedocs.io/en/latest/>`_.
+See `full document here <https://hftbacktest.readthedocs.io/>`_.
 
 Getting started
 ===============
 
 Installation
 ------------
```

### Comparing `hftbacktest-1.5.4/hftbacktest/__init__.py` & `hftbacktest-1.5.5/hftbacktest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     'validate_data',
     'correct_local_timestamp',
     'correct_exch_timestamp',
     'correct_exch_timestamp_adjust',
     'correct'
 )
 
-__version__ = '1.5.4'
+__version__ = '1.5.5'
 
 
 # JIT'ed latency models
 ConstantLatency = jitclass()(ConstantLatency_)
 FeedLatency = jitclass()(FeedLatency_)
 ForwardFeedLatency = jitclass()(ForwardFeedLatency_)
 BackwardFeedLatency = jitclass()(BackwardFeedLatency_)
```

### Comparing `hftbacktest-1.5.4/hftbacktest/assettype.py` & `hftbacktest-1.5.5/hftbacktest/assettype.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/backtest.py` & `hftbacktest-1.5.5/hftbacktest/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/data/__init__.py` & `hftbacktest-1.5.5/hftbacktest/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/data/utils/binancefutures.py` & `hftbacktest-1.5.5/hftbacktest/data/utils/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/data/utils/snapshot.py` & `hftbacktest-1.5.5/hftbacktest/data/utils/snapshot.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/data/utils/tardis.py` & `hftbacktest-1.5.5/hftbacktest/data/utils/tardis.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/data/validation.py` & `hftbacktest-1.5.5/hftbacktest/data/validation.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/experimental/backtest.py` & `hftbacktest-1.5.5/hftbacktest/experimental/backtest.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/experimental/live/binancefutures.py` & `hftbacktest-1.5.5/hftbacktest/experimental/live/binancefutures.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/experimental/live/ordermanager.py` & `hftbacktest-1.5.5/hftbacktest/experimental/live/ordermanager.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/experimental/live/settings.py` & `hftbacktest-1.5.5/hftbacktest/experimental/live/settings.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/experimental/multiassetinit.py` & `hftbacktest-1.5.5/hftbacktest/experimental/multiassetinit.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/marketdepth.py` & `hftbacktest-1.5.5/hftbacktest/marketdepth.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/models/latencies.py` & `hftbacktest-1.5.5/hftbacktest/models/latencies.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/models/queue.py` & `hftbacktest-1.5.5/hftbacktest/models/queue.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/order.py` & `hftbacktest-1.5.5/hftbacktest/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
     def __getitem__(self, key):
         return self.order_list[key]
 
     def __len__(self):
         return len(self.order_list)
 
-    def __delitem__(self, key):
+    def delitem(self, key):
         order, _ = self.order_list[key]
         del self.order_list[key]
         self.orders[order.order_id] -= 1
         if self.orders[order.order_id] <= 0:
             del self.orders[order.order_id]
 
     def __contains__(self, key):
```

### Comparing `hftbacktest-1.5.4/hftbacktest/proc/local.py` & `hftbacktest-1.5.5/hftbacktest/proc/local.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/proc/nopartialfillexchange.py` & `hftbacktest-1.5.5/hftbacktest/proc/nopartialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/proc/partialfillexchange.py` & `hftbacktest-1.5.5/hftbacktest/proc/partialfillexchange.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/proc/proc.py` & `hftbacktest-1.5.5/hftbacktest/proc/proc.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             # Process the order part.
             next_timestamp = 0
             next_frontmost_timestamp = 0
             i = 0
             while i < self.orders_from.__len__():
                 order, recv_timestamp = self.orders_from[i]
                 if self.orders_from.frontmost_timestamp == recv_timestamp:
-                    self.orders_from.__delitem__(i)
+                    self.orders_from.delitem(i)
 
                     next_timestamp = self._process_recv_order(
                         order,
                         recv_timestamp,
                         wait_resp,
                         next_timestamp
                     )
```

### Comparing `hftbacktest-1.5.4/hftbacktest/reader.py` & `hftbacktest-1.5.5/hftbacktest/reader.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/stat.py` & `hftbacktest-1.5.5/hftbacktest/stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,21 +336,22 @@
 
         mid = pd.Series(self.mid, index=dt_index)
 
         if capital is not None:
             ((mid / mid[0] - 1).resample(resample).last() * 100).plot(ax=axs[0], style='grey', alpha=0.5)
             (rs_equity / capital * 100).plot(ax=axs[0])
             (rs_equity_wo_fee / capital * 100).plot(ax=axs[0])
+            axs[0].set_ylabel('Cumulative Returns (%)')
         else:
             mid.resample(resample).last().plot(ax=axs[0], style='grey', alpha=0.5)
             (rs_equity * 100).plot(ax=axs[0])
             (rs_equity_wo_fee * 100).plot(ax=axs[0])
+            axs[0].set_ylabel('Cumulative Returns')
 
         # axs[0].set_title('Equity')
-        axs[0].set_ylabel('Cumulative Returns (%)')
         axs[0].grid()
         axs[0].legend(['Trading asset', 'Strategy incl. fee', 'Strategy excl. fee'])
 
         # todo: this can mislead a user due to aggregation.
         position = pd.Series(self.position, index=dt_index).resample(resample).last()
         position.plot(ax=axs[1])
         # ax3 = ax2.twinx()
```

### Comparing `hftbacktest-1.5.4/hftbacktest/state.py` & `hftbacktest-1.5.5/hftbacktest/state.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest/typing.py` & `hftbacktest-1.5.5/hftbacktest/typing.py`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/hftbacktest.egg-info/PKG-INFO` & `hftbacktest-1.5.5/hftbacktest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hftbacktest
-Version: 1.5.4
+Version: 1.5.5
 Summary: High-frequency trading and market making backtesting tool
 Home-page: https://github.com/nkaz001/hftbacktest
 Author: nkaz001
 Author-email: nkaz001@protonmail.com
 License: MIT
 Project-URL: Docs, https://hftbacktest.readthedocs.io/en/latest/
 Project-URL: GitHub: issues, https://github.com/nkaz001/hftbacktest/issues
@@ -43,15 +43,15 @@
 * Full order book reconstruction based on L2 feeds(Market-By-Price).
 * Backtest accounting for both feed and order latency, using provided models or your own custom model.
 * Order fill simulation that takes into account the order queue position, using provided models or your own custom model.
 
 Documentation
 =============
 
-See `full document here <https://hftbacktest.readthedocs.io/en/latest/>`_.
+See `full document here <https://hftbacktest.readthedocs.io/>`_.
 
 Getting started
 ===============
 
 Installation
 ------------
```

### Comparing `hftbacktest-1.5.4/hftbacktest.egg-info/SOURCES.txt` & `hftbacktest-1.5.5/hftbacktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hftbacktest-1.5.4/setup.cfg` & `hftbacktest-1.5.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 [options]
 python_requires = >=3.8
 packages = find:
 zip_safe = False
 include_package_data = True
 install_requires = 
-	numba ~= 0.56
-	numpy < 1.24, >= 1.18
+	numba ~= 0.57
+	numpy < 1.25, >= 1.21
 	pandas
 	matplotlib
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

