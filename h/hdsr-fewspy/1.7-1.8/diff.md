# Comparing `tmp/hdsr_fewspy-1.7.tar.gz` & `tmp/hdsr_fewspy-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.7.tar", last modified: Wed May  3 12:26:15 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.8.tar", last modified: Wed May 10 11:47:10 2023, max compression
```

## Comparing `hdsr_fewspy-1.7.tar` & `hdsr_fewspy-1.8.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.7/LICENSE.txt
--rw-rw-rw-   0        0        0    23177 2023-05-03 12:26:16.000000 hdsr_fewspy-1.7/PKG-INFO
--rw-rw-rw-   0        0        0    22301 2023-05-03 12:24:46.000000 hdsr_fewspy-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/
--rw-rw-rw-   0        0        0      462 2023-05-03 11:03:03.000000 hdsr_fewspy-1.7/hdsr_fewspy/__init__.py
--rw-rw-rw-   0        0        0    14458 2023-05-03 11:28:19.000000 hdsr_fewspy-1.7/hdsr_fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/
--rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7535 2023-05-02 15:42:12.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2950 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2578 2023-04-26 14:48:57.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2917 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     9475 2023-05-02 15:54:18.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     6091 2023-05-02 15:54:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2895 2023-05-02 15:54:31.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/github.py
--rw-rw-rw-   0        0        0      521 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     6246 2023-05-02 18:32:13.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.7/hdsr_fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     5955 2023-05-02 10:29:19.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6875 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/utils.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0     4570 2023-05-02 16:27:51.000000 hdsr_fewspy-1.7/hdsr_fewspy/date_frequency.py
--rw-rw-rw-   0        0        0      681 2023-05-02 10:03:04.000000 hdsr_fewspy-1.7/hdsr_fewspy/exceptions.py
--rw-rw-rw-   0        0        0     4363 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/permissions.py
--rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.7/hdsr_fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3557 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1837 2023-05-02 18:38:33.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_qualifiers.py
--rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     7743 2023-05-03 11:53:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-03 12:26:15.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    23177 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 12:26:14.000000 hdsr_fewspy-1.7/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.7/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-05-03 12:26:16.000000 hdsr_fewspy-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-03 12:18:21.000000 hdsr_fewspy-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    23553 2023-05-10 11:47:11.000000 hdsr_fewspy-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    22677 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      462 2023-05-03 11:03:03.000000 hdsr_fewspy-1.8/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    14235 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7535 2023-05-02 15:42:12.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2963 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2592 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2931 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     9493 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     6091 2023-05-02 15:54:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2915 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      470 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6259 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     5986 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6900 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4573 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      612 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     2806 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.8/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     3798 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1837 2023-05-02 18:38:33.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0     1842 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_custom_secrets.py
+-rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_qualifiers.py
+-rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     7743 2023-05-03 11:53:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    23553 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1994 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-05-10 11:47:11.000000 hdsr_fewspy-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/setup.py
```

### Comparing `hdsr_fewspy-1.7/LICENSE.txt` & `hdsr_fewspy-1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/PKG-INFO` & `hdsr_fewspy-1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr_fewspy
-Version: 1.7
+Version: 1.8
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.7.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.8.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -58,53 +58,64 @@
 get_time_series_single        | 4, 5, 6            | Returns 1 dataframe or a list >=1 xml/json responses     
 get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
 get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response)
 
 ### Usage
 
 ###### Preparation
-1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
+1. Only once needed: ensure you have a github account with a GITHUB_PERSONAL_ACCESS_TOKEN. Read topic 
+   'GITHUB_PERSONAL_ACCESS_TOKEN' below.
+2. You can create a hdsr_fewspy API in two ways (the first way dominates the second): 
+   a. or with API arguments 'github_email' and/or token 'github_personal_access_token'
+   b. or put these arguments in a .env file and use API argument 'secrets_env_path' (defaults to 'G:/secrets.env')
+      The .env file must have these 2 rows:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
-HDSR_FEWSPY_EMAIL=<your_hdsr_email>
-HDSR_FEWSPY_TOKEN=<contact renier.kramer.hdsr.nl to get HDSR_FEWSPY_TOKEN>
+GITHUB_EMAIL=<your_github_email>
 ```
 2. Only once per project: install hdsr_fewspy dependency:
 ```
 pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
-3. Run imports and instantiate a hdsr_fewspy API: 
+3. Example simple:
 ```
 from datetime import datetime
 import hdsr_fewspy
-from hdsr_fewspy import Api, PiSettings, OutputChoices, github_pi_setting_defaults, TimeZoneChoices
 
-# option 1 Instantiate API using default settings:
-api = hdsr_fewspy.Api()  
+api = hdsr_fewspy.Api()
+```
+4. Example sophisticated:
+```
+# Optionally, you can specify several API arguments:
+# github_email: str, 
+# github_personal_access_token: str
+# secrets_env_path: str or pathlib.Path
+# pi_settings: hdsr_fewspy.PiSettings 
+# output_directory_root: str or pathlib.path
+
+# For example in case of pi_settings, you can use predefined settings ('standalone', 'production', etc):
+sa_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
+api = hdsr_fewspy.Api(pi_settings=sa_pi_settings)
 
-# option 2 Instantiate API using custom settings:
+# Or create your own pi_settings:
 custom_settings = hdsr_fewspy.PiSettings(
    settings_name="does not matter blabla",            
    document_version=1.25",
    ssl_verify=True,
    domain="localhost",
    port="8080",
    service="FewsWebServices",
    filter_id="INTERNAL-API",
    module_instance_ids="WerkFilter",
    time_zone=hdsr_fewspy.TimeZoneChoices.eu_amsterdam,  # = 1.0 (only affects get_time_series dataframe and csv)
 )
 api = hdsr_fewspy.Api(pi_settings=custom_settings)
-# or use a default custom setting:
-sa_default_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
-api = hdsr_fewspy.Api(pi_settings=sa_default_pi_settings)
-
-# option 3: Instantiate API with download directory
-# If you want to download responses to file, then you need to specify an output_directory_root. The files will be 
-downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<here_your_files_will_be_downloaded>
+
+# In case you want to download responses to file, then you need to specify an output_directory_root 
+# The files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<files_will_be_downloaded_here>
 api = hdsr_fewspy.Api(output_directory_root=<path_to_a_dir>)
 ```
 
 ###### Examples 9 different API calls (using api option 3 from above)
 1. get_parameters
 ```
 df = api.get_parameters(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
@@ -322,21 +333,21 @@
 
 ### Releases
 [Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 3rd 2023)
+### Test Coverage (May 10th 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                              10      0   100%
-hdsr_fewspy\api.py                                                  107     16    85%
+hdsr_fewspy\api.py                                                  110     16    85%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
@@ -344,30 +355,30 @@
 hdsr_fewspy\api_calls\time_series\base.py                           109      9    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
-hdsr_fewspy\constants\paths.py                                       11      0   100%
+hdsr_fewspy\constants\paths.py                                       10      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 78      7    91%
 hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
-hdsr_fewspy\exceptions.py                                            16      0   100%
-hdsr_fewspy\permissions.py                                           67      5    93%
+hdsr_fewspy\exceptions.py                                            14      0   100%
+hdsr_fewspy\permissions.py                                           47      1    98%
 hdsr_fewspy\retry_session.py                                         68     12    82%
-hdsr_fewspy\secrets.py                                               64     20    69%
+hdsr_fewspy\secrets.py                                               71     19    73%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1526    193    87%
+TOTAL                                                              1513    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.7/README.md` & `hdsr_fewspy-1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,53 +36,64 @@
 get_time_series_single        | 4, 5, 6            | Returns 1 dataframe or a list >=1 xml/json responses     
 get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
 get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response)
 
 ### Usage
 
 ###### Preparation
-1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
+1. Only once needed: ensure you have a github account with a GITHUB_PERSONAL_ACCESS_TOKEN. Read topic 
+   'GITHUB_PERSONAL_ACCESS_TOKEN' below.
+2. You can create a hdsr_fewspy API in two ways (the first way dominates the second): 
+   a. or with API arguments 'github_email' and/or token 'github_personal_access_token'
+   b. or put these arguments in a .env file and use API argument 'secrets_env_path' (defaults to 'G:/secrets.env')
+      The .env file must have these 2 rows:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
-HDSR_FEWSPY_EMAIL=<your_hdsr_email>
-HDSR_FEWSPY_TOKEN=<contact renier.kramer.hdsr.nl to get HDSR_FEWSPY_TOKEN>
+GITHUB_EMAIL=<your_github_email>
 ```
 2. Only once per project: install hdsr_fewspy dependency:
 ```
 pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
-3. Run imports and instantiate a hdsr_fewspy API: 
+3. Example simple:
 ```
 from datetime import datetime
 import hdsr_fewspy
-from hdsr_fewspy import Api, PiSettings, OutputChoices, github_pi_setting_defaults, TimeZoneChoices
 
-# option 1 Instantiate API using default settings:
-api = hdsr_fewspy.Api()  
+api = hdsr_fewspy.Api()
+```
+4. Example sophisticated:
+```
+# Optionally, you can specify several API arguments:
+# github_email: str, 
+# github_personal_access_token: str
+# secrets_env_path: str or pathlib.Path
+# pi_settings: hdsr_fewspy.PiSettings 
+# output_directory_root: str or pathlib.path
+
+# For example in case of pi_settings, you can use predefined settings ('standalone', 'production', etc):
+sa_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
+api = hdsr_fewspy.Api(pi_settings=sa_pi_settings)
 
-# option 2 Instantiate API using custom settings:
+# Or create your own pi_settings:
 custom_settings = hdsr_fewspy.PiSettings(
    settings_name="does not matter blabla",            
    document_version=1.25",
    ssl_verify=True,
    domain="localhost",
    port="8080",
    service="FewsWebServices",
    filter_id="INTERNAL-API",
    module_instance_ids="WerkFilter",
    time_zone=hdsr_fewspy.TimeZoneChoices.eu_amsterdam,  # = 1.0 (only affects get_time_series dataframe and csv)
 )
 api = hdsr_fewspy.Api(pi_settings=custom_settings)
-# or use a default custom setting:
-sa_default_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
-api = hdsr_fewspy.Api(pi_settings=sa_default_pi_settings)
-
-# option 3: Instantiate API with download directory
-# If you want to download responses to file, then you need to specify an output_directory_root. The files will be 
-downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<here_your_files_will_be_downloaded>
+
+# In case you want to download responses to file, then you need to specify an output_directory_root 
+# The files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<files_will_be_downloaded_here>
 api = hdsr_fewspy.Api(output_directory_root=<path_to_a_dir>)
 ```
 
 ###### Examples 9 different API calls (using api option 3 from above)
 1. get_parameters
 ```
 df = api.get_parameters(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
@@ -300,21 +311,21 @@
 
 ### Releases
 [Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 3rd 2023)
+### Test Coverage (May 10th 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                              10      0   100%
-hdsr_fewspy\api.py                                                  107     16    85%
+hdsr_fewspy\api.py                                                  110     16    85%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
@@ -322,30 +333,30 @@
 hdsr_fewspy\api_calls\time_series\base.py                           109      9    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
-hdsr_fewspy\constants\paths.py                                       11      0   100%
+hdsr_fewspy\constants\paths.py                                       10      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 78      7    91%
 hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
-hdsr_fewspy\exceptions.py                                            16      0   100%
-hdsr_fewspy\permissions.py                                           67      5    93%
+hdsr_fewspy\exceptions.py                                            14      0   100%
+hdsr_fewspy\permissions.py                                           47      1    98%
 hdsr_fewspy\retry_session.py                                         68     12    82%
-hdsr_fewspy\secrets.py                                               64     20    69%
+hdsr_fewspy\secrets.py                                               71     19    73%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1526    193    87%
+TOTAL                                                              1513    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from datetime import datetime
 from hdsr_fewspy import api_calls
 from hdsr_fewspy import exceptions
 from hdsr_fewspy.constants.choices import OutputChoices
 from hdsr_fewspy.constants.choices import TimeZoneChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
+from hdsr_fewspy.constants.paths import SECRETS_ENV_PATH
 from hdsr_fewspy.constants.pi_settings import github_pi_setting_defaults
 from hdsr_fewspy.constants.pi_settings import PiSettings
 from hdsr_fewspy.constants.request_settings import get_default_request_settings
 from hdsr_fewspy.constants.request_settings import RequestSettings
 from hdsr_fewspy.permissions import Permissions
 from hdsr_fewspy.retry_session import RetryBackoffSession
+from hdsr_fewspy.secrets import Secrets
 from pathlib import Path
 from typing import List
 from typing import Optional
 from typing import Union
 
 import geopandas as gpd
 import logging
@@ -33,18 +35,26 @@
 
     The methods corresponding with the FEWS PI-REST requests. For more info on how to work with the FEWS REST Web
     Service, visit the Deltares website: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service.
     """
 
     def __init__(
         self,
+        github_email: str = None,
+        github_personal_access_token: str = None,
+        secrets_env_path: Union[str, Path] = SECRETS_ENV_PATH,
         pi_settings: PiSettings = None,
         output_directory_root: Union[str, Path] = None,
     ):
-        self.permissions = Permissions()
+        self.secrets = Secrets(
+            github_email=github_email,
+            github_personal_access_token=github_personal_access_token,
+            secrets_env_path=secrets_env_path,
+        )
+        self.permissions = Permissions(secrets=self.secrets)
         self.output_dir = self.__get_output_dir(output_directory_root=output_directory_root)
         self.pi_settings = self.__validate_pi_settings(pi_settings=pi_settings)
         self.request_settings: RequestSettings = get_default_request_settings()
         self.retry_backoff_session = RetryBackoffSession(
             _request_settings=self.request_settings,
             pi_settings=self.pi_settings,
             output_dir=self.output_dir,
@@ -288,54 +298,30 @@
             output_choice=output_choice,
             retry_backoff_session=self.retry_backoff_session,
         )
         all_file_paths = api_call.run()
         return all_file_paths
 
 
-# DONE: Use BackoffRetry strategy
-
-# DONE: add rate_limiting to requests (freq and size)
-
 # TODO: don't use strings as urls...
 
-# Done: authenticate by GET request a hdsr-mid repo (yet to build) that holds email_token items per user
-
-# DONE: test other get requests than get_timeseries
-
-# DONE: improve documentation
-
-# DONE: enable users to override Api.pi_settings
-
-# DONE: conversion client - server timezone
-
-# DONE: fix moduleInstanceIds and filterId
-
-# DONE: wat als iemand alleen maar statistieken wil van tijdseries?
-
-# DONE: besides allowed_request_args use a required_request_args (get_locations zonder filter duurt tering lang!!)
-
-# DONE: create pypi package
-
 # TODO: Ciska wel interesse wel in:
 #  --------------------------------
 #  get_samples (grote request)
 #  - Deltares is hier begin 2024 klaar. Nu geeft FEWS EFICS piwebservice na 2 of 5 minuten een timeout
 #  get_timeseries (grote request)
 #  - altijd start + end
 #  - altijd omitEmptyTimeSeries op True anders geeft ie minimaal weken aan tijdseries terug
 #  - vaak filter_id
 #  - soms parameter_id, location_id, moduleinstance_id
 #  - heel soms qualifier_id
 #  get_parameters (middlegrote request = 400 parameters)
 #  get_locations (kleine request = 300 locaties)
 
-# TODO: Ciska geen interesse in:
-#  --------------------------------
-#  get_qualifiers
+# TODO: Ciska geen interesse in: get_qualifiers
 
 # TODO: check of properties goed meekomen in get_timeseries in PI_JSON (in PI_XML gaat het goed) -> Ciska:" bij
 #  EFICS werkt niet helemaal lekker. bij get_samples gaat het helemaal fout"
 
 # TODO: van potentieel grote naar kleine request belasting: get_samples, get_timeseries,
 #  get_qualifiers (25 groepen * 100k regels per groep), get_parameters (4000), get_locations (300)
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/__init__.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/base.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         response = self.retry_backoff_session.get(
             url=self.url, params=self.filtered_fews_parameters, verify=self.pi_settings.ssl_verify
         )
 
         if self.output_choice in {OutputChoices.json_response_in_memory, OutputChoices.xml_response_in_memory}:
             return response
 
-        assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error"
+        assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error GetLocations"
         # parse the response to dataframe
         if response.status_code == 200:
 
             # convert to gdf and snake_case
             df = pd.json_normalize(data=response.json()["locations"])
             df.columns = [camel_to_snake_case(i) for i in df.columns]
             df.set_index("location_id", inplace=True)
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def run(self) -> Union[ResponseType, pd.DataFrame]:
         response = self.retry_backoff_session.get(
             url=self.url, params=self.filtered_fews_parameters, verify=self.pi_settings.ssl_verify
         )
         if self.output_choice in {OutputChoices.json_response_in_memory, OutputChoices.xml_response_in_memory}:
             return response
 
-        assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error"
+        assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error GetParameters"
         # parse the response to dataframe
         df = pd.DataFrame(columns=COLUMNS)
         if response.status_code == 200:
             if "timeSeriesParameters" in response.json().keys():
                 df = pd.DataFrame(response.json()["timeSeriesParameters"])
                 df.columns = [camel_to_snake_case(i) for i in df.columns]
                 df["uses_datum"] = df["uses_datum"] == "true"
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_qualifiers.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_qualifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def run(self) -> Union[ResponseType, pd.DataFrame]:
         response = self.retry_backoff_session.get(
             url=self.url, params=self.filtered_fews_parameters, verify=self.pi_settings.ssl_verify
         )
         if self.output_choice == OutputChoices.xml_response_in_memory:
             return response
 
-        assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error"
+        assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error GetQualifiers"
         # parse the response to dataframe
         if response.status_code == 200:
             tree = ElementTree.fromstring(response.content)
             qualifiers_tree = [i for i in tree.iter(tag=f"{NS}qualifier")]
             qualifiers_tuple = (self._element_to_tuple(i) for i in qualifiers_tree)
             df = pd.DataFrame(qualifiers_tuple, columns=COLUMNS)
         else:
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_samples.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_samples.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         request_params["showStatistics"] = True
         response = self.retry_backoff_session.get(
             url=self.url, params=request_params, verify=self.pi_settings.ssl_verify
         )
         return response
 
     def _get_nr_timestamps(self, request_params: Dict) -> int:
-        assert "moduleInstanceIds" in request_params, "code error"
+        assert "moduleInstanceIds" in request_params, "code error GetTimeSeriesBase"
         response = self._get_statistics(request_params=request_params)
         msg = f"status_code={response.status_code}, err={response.text}, request_params={request_params}"
         if not response.ok:
             return self.__get_nr_timestamps_invalid_response(response=response, msg=msg)
         if self.pi_settings.document_format == PiRestDocumentFormatChoices.json:
             timeseries = response.json().get("timeSeries", None)
             if not timeseries:
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,13 +52,13 @@
             date_range_freq=date_range_freq,
             request_params=self.initial_fews_parameters,
         )
 
         if self.output_choice in {OutputChoices.json_response_in_memory, OutputChoices.xml_response_in_memory}:
             return responses
 
-        assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error"
+        assert self.output_choice == OutputChoices.pandas_dataframe_in_memory, "code error GetTimeSeriesSingle"
         # parse the response to dataframe
         df = response_jsons_to_one_df(
             responses=responses, drop_missing_values=self.drop_missing_values, flag_threshold=self.flag_threshold
         )
         return df
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py` & `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/constants/choices.py` & `hdsr_fewspy-1.8/hdsr_fewspy/constants/choices.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.8/hdsr_fewspy/constants/pi_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     def _read_github(self, settings_name: str) -> pd.Series:
         logger.info(f"get_on_the_fly_pi_settings for setttings_name '{settings_name}'")
         df_slice = self.df_github_settings[self.df_github_settings["settings_name"] == settings_name]
         if df_slice.empty:
             available_setting_names = self.df_github_settings["settings_name"].tolist()
             msg = f"pi settings_name '{settings_name}' is not in available setting_names '{available_setting_names}'"
             raise AssertionError(msg)
-        assert len(df_slice) == 1, "code error"
+        assert len(df_slice) == 1, "code error _read_github"
         pd_series = df_slice.iloc[0]
         return pd_series
 
     def get_pi_settings(self, settings_name: str) -> PiSettings:
         pd_series = self._read_github(settings_name=settings_name)
         pi_settings = PiSettings(
             settings_name=pd_series["settings_name"],
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/constants/request_settings.py` & `hdsr_fewspy-1.8/hdsr_fewspy/constants/request_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/converters/download.py` & `hdsr_fewspy-1.8/hdsr_fewspy/converters/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 class XmlDownloadDir(DownloadBase):
     def run(self, responses: List[ResponseType], file_name_values: List[str], **kwargs) -> List[Path]:
         """Create for every response a separate .xml file.
         All responses are for a unique location_parameter_qualifier combi in get_time_series_multi."""
         file_name_base = self._get_base_file_name(request_class=self.request_class, file_name_values=file_name_values)
         file_paths_created = []
         for index, response in enumerate(responses):
-            assert response.status_code == 200, "code error"
+            assert response.status_code == 200, "code error XmlDownloadDir"
             file_path = self.output_dir / f"{file_name_base}_{index}.xml"
             logger.info(f"writing response to new file {file_path}")
             self._ensure_output_dir_exists(file_path=file_path)
             with open(file=file_path.as_posix(), mode="w", encoding="utf-8") as xml_file:
                 xml_file.write(response.text)
             file_paths_created.append(file_path)
         return file_paths_created
@@ -83,15 +83,15 @@
 class JsonDownloadDir(DownloadBase):
     def run(self, responses: List[ResponseType], file_name_values: List[str], **kwargs) -> List[Path]:
         """Create for every response a separate .json file.
         All responses are for a unique location_parameter_qualifier combi in get_time_series_multi."""
         file_name_base = self._get_base_file_name(request_class=self.request_class, file_name_values=file_name_values)
         file_paths_created = []
         for index, response in enumerate(responses):
-            assert response.status_code == 200, "code error"
+            assert response.status_code == 200, "code error JsonDownloadDir"
             file_path = self.output_dir / f"{file_name_base}_{index}.json"
             logger.info(f"writing response to new file {file_path}")
             self._ensure_output_dir_exists(file_path=file_path)
             with open(file=file_path.as_posix(), mode="w", encoding="utf-8") as json_file:
                 # indent=None results in half the file size compared to indent=4
                 json.dump(obj=response.json(), fp=json_file, ensure_ascii=False, indent=None)
             file_paths_created.append(file_path)
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.8/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,10 +194,10 @@
             pi_time_series=data, drop_missing_values=drop_missing_values, flag_threshold=flag_threshold
         )
         for time_series in time_series_set.time_series:
             _df = time_series.events
             _df["location_id"] = time_series_set.location_ids[0]
             _df["parameter_id"] = time_series_set.parameter_ids[0]
             if not df.empty:
-                assert sorted(_df.columns) == sorted(df.columns), "code error"
+                assert sorted(_df.columns) == sorted(df.columns), "code error response_jsons_to_one_df"
             df = pd.concat(objs=[df, _df], axis=0)
     return df
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/converters/manager.py` & `hdsr_fewspy-1.8/hdsr_fewspy/converters/manager.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/converters/utils.py` & `hdsr_fewspy-1.8/hdsr_fewspy/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.8/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/date_frequency.py` & `hdsr_fewspy-1.8/hdsr_fewspy/date_frequency.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,27 +65,27 @@
         enddate_request: pd.Timestamp,
     ) -> pd.Timedelta:
         """Optional increase or decrease the time-window of a request depending on nr_timestamps found."""
         if nr_timestamps > request_settings.max_request_nr_timestamps:
             date_range_freq = 0.7 * date_range_freq
         elif nr_timestamps < request_settings.min_request_nr_timestamps:
             if date_range_freq > request_settings.max_request_period:
-                logger.info(
+                logger.debug(
                     f"date_range_freq={date_range_freq} exceeds max_request_period="
                     f"(={request_settings.max_request_period}). Continue with date_range_freq={date_range_freq}"
                 )
                 return date_range_freq
             period_required = enddate_request - startdate_request
             if date_range_freq > period_required:
-                logger.info(
+                logger.debug(
                     f"date_range_freq={date_range_freq} exceeds period available (={period_required}). Continue with "
                     f"date_range_freq={date_range_freq}"
                 )
                 return date_range_freq
 
             try:
                 date_range_freq = 1.3 * date_range_freq
             except (OverflowError, pd.errors.OutOfBoundsDatetime) as err:
-                logger.info(
+                logger.debug(
                     f"could not increase date_range_freq (err={err}). Continue with date_range_freq={date_range_freq}"
                 )
         return date_range_freq
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/exceptions.py` & `hdsr_fewspy-1.8/hdsr_fewspy/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,14 @@
     pass
 
 
 class UserNotFoundInHdsrFewspyAuthError(Exception):
     pass
 
 
-class UserInvalidTokenHdsrFewspyAuthError(Exception):
-    pass
-
-
 class NoPermissionInHdsrFewspyAuthError(Exception):
     pass
 
 
 class PiSettingsError(Exception):
     pass
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/permissions.py` & `hdsr_fewspy-1.8/hdsr_fewspy/permissions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,25 @@
 from hdsr_fewspy.constants import github
 from hdsr_fewspy.exceptions import NoPermissionInHdsrFewspyAuthError
-from hdsr_fewspy.exceptions import UserInvalidTokenHdsrFewspyAuthError
 from hdsr_fewspy.exceptions import UserNotFoundInHdsrFewspyAuthError
 from hdsr_fewspy.secrets import Secrets
 from hdsr_pygithub import GithubFileDownloader
-from typing import Dict
 from typing import List
 
 import logging
 import pandas as pd
-import validators
 
 
 logger = logging.getLogger(__name__)
 
 
 class Permissions:
-    def __init__(self):
-        self.secrets = Secrets()
-        logger.info(
-            "using hdsr_fewspy_email and hdsr_fewspy_token from os environmental variables (loaded from G:/secrets.env)"
-        )
-        self.hdsr_fewspy_email = self.validate_email(email=self.secrets.hdsr_fewspy_email)
-        self.hdsr_fewspy_token = self.secrets.hdsr_fewspy_token.strip()
+    def __init__(self, secrets: Secrets):
+        self.secrets = secrets
         self._permission_row = None
-        self.ensure_any_permissions()
-
-    @classmethod
-    def validate_email(cls, email: str) -> str:
-        logger.info("validatng email")
-        assert isinstance(email, str) and email
-        if not validators.email(value=email) == True:  # noqa
-            raise AssertionError(f"email '{email}' is invalid")
-        return email.strip()
-
-    def ensure_any_permissions(self) -> None:
-        if self.permissions_row.empty:
-            raise NoPermissionInHdsrFewspyAuthError(f"user {self.hdsr_fewspy_email} has no permissions at all")
 
     @property
     def permissions_row(self) -> pd.Series:
         if self._permission_row is not None:
             return self._permission_row
         logger.info("determine permissions")
         github_downloader = GithubFileDownloader(
@@ -53,32 +32,25 @@
         df = pd.read_csv(filepath_or_buffer=github_downloader.get_download_url(), sep=";")
 
         # strip all values
         df_obj = df.select_dtypes(["object"])
         df[df_obj.columns] = df_obj.apply(lambda x: x.str.strip())
 
         # get row with matching email
-        permissions_row = df[df["email"] == self.hdsr_fewspy_email]
-        assert len(permissions_row) == 1, "code error"
+        permissions_row = df[df["email"] == self.secrets.github_email]
+        nr_rows = len(permissions_row)
+        if nr_rows != 1:
+            msg = f"github_email {self.secrets.github_email} is registered {nr_rows} times in hdsr_fewspy_auth"
+            raise UserNotFoundInHdsrFewspyAuthError(msg)
         permissions_row = permissions_row.loc[0]
 
-        # check user exists
+        # check github_email exists
         if permissions_row.empty:
-            raise UserNotFoundInHdsrFewspyAuthError(
-                f"email {self.hdsr_fewspy_email} not in permission file. Please contact maintainer of this package"
-            )
-
-        # check user has valid token
-        if permissions_row["hdsr_fewspy_token"] != self.hdsr_fewspy_token:
-            raise UserInvalidTokenHdsrFewspyAuthError(
-                "email found in permission file, but token does not match. Please contact maintainer of this package"
-            )
+            raise NoPermissionInHdsrFewspyAuthError(f"github_email {self.secrets.github_email} has no permissions")
 
-        # hide token
-        permissions_row["hdsr_fewspy_token"] = "..."
         self._permission_row = permissions_row
         return self._permission_row
 
     @staticmethod
     def split_string_in_list(value: str) -> List[str]:
         return [x for x in value.split(",") if x]
 
@@ -93,16 +65,7 @@
     @property
     def allowed_module_instance_id(self) -> List[str]:
         return self.split_string_in_list(value=self.permissions_row["allowed_module_instance_id"])
 
     @property
     def allowed_filter_id(self) -> List[str]:
         return self.split_string_in_list(value=self.permissions_row["allowed_filter_id"])
-
-    @property
-    def all_fields(self) -> Dict:
-        return {
-            "allowed_domain": self.allowed_domain,
-            "allowed_service": self.allowed_service,
-            "allowed_module_instance_id": self.allowed_module_instance_id,
-            "allowed_filter_id": self.allowed_filter_id,
-        }
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/retry_session.py` & `hdsr_fewspy-1.8/hdsr_fewspy/retry_session.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/fixtures.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_qualifiers.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy.egg-info/PKG-INFO` & `hdsr_fewspy-1.8/hdsr_fewspy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr-fewspy
-Version: 1.7
+Version: 1.8
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.7.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.8.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -58,53 +58,64 @@
 get_time_series_single        | 4, 5, 6            | Returns 1 dataframe or a list >=1 xml/json responses     
 get_time_series_multi         | 1, 2, 3            | Returns a list with downloaded files (1 .csv or >=1 .xml/.json per unique location_parameter_qualifier)
 get_time_series_statistics    | 4, 5               | Returns 1 object (xml/json response)
 
 ### Usage
 
 ###### Preparation
-1. Only once needed: ensure you have a file G:/secrets.env. This file must contain at least these 3 lines:
+1. Only once needed: ensure you have a github account with a GITHUB_PERSONAL_ACCESS_TOKEN. Read topic 
+   'GITHUB_PERSONAL_ACCESS_TOKEN' below.
+2. You can create a hdsr_fewspy API in two ways (the first way dominates the second): 
+   a. or with API arguments 'github_email' and/or token 'github_personal_access_token'
+   b. or put these arguments in a .env file and use API argument 'secrets_env_path' (defaults to 'G:/secrets.env')
+      The .env file must have these 2 rows:
 ```
 GITHUB_PERSONAL_ACCESS_TOKEN=<see topic 'GITHUB_PERSONAL_ACCESS_TOKEN' below>
-HDSR_FEWSPY_EMAIL=<your_hdsr_email>
-HDSR_FEWSPY_TOKEN=<contact renier.kramer.hdsr.nl to get HDSR_FEWSPY_TOKEN>
+GITHUB_EMAIL=<your_github_email>
 ```
 2. Only once per project: install hdsr_fewspy dependency:
 ```
 pip install hdsr-fewspy (or 'conda install hdsr-fewspy -channel hdsr-mid')
 ```
-3. Run imports and instantiate a hdsr_fewspy API: 
+3. Example simple:
 ```
 from datetime import datetime
 import hdsr_fewspy
-from hdsr_fewspy import Api, PiSettings, OutputChoices, github_pi_setting_defaults, TimeZoneChoices
 
-# option 1 Instantiate API using default settings:
-api = hdsr_fewspy.Api()  
+api = hdsr_fewspy.Api()
+```
+4. Example sophisticated:
+```
+# Optionally, you can specify several API arguments:
+# github_email: str, 
+# github_personal_access_token: str
+# secrets_env_path: str or pathlib.Path
+# pi_settings: hdsr_fewspy.PiSettings 
+# output_directory_root: str or pathlib.path
+
+# For example in case of pi_settings, you can use predefined settings ('standalone', 'production', etc):
+sa_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
+api = hdsr_fewspy.Api(pi_settings=sa_pi_settings)
 
-# option 2 Instantiate API using custom settings:
+# Or create your own pi_settings:
 custom_settings = hdsr_fewspy.PiSettings(
    settings_name="does not matter blabla",            
    document_version=1.25",
    ssl_verify=True,
    domain="localhost",
    port="8080",
    service="FewsWebServices",
    filter_id="INTERNAL-API",
    module_instance_ids="WerkFilter",
    time_zone=hdsr_fewspy.TimeZoneChoices.eu_amsterdam,  # = 1.0 (only affects get_time_series dataframe and csv)
 )
 api = hdsr_fewspy.Api(pi_settings=custom_settings)
-# or use a default custom setting:
-sa_default_pi_settings = hdsr_fewspy.github_pi_setting_defaults.get_pi_settings(settings_name="standalone")
-api = hdsr_fewspy.Api(pi_settings=sa_default_pi_settings)
-
-# option 3: Instantiate API with download directory
-# If you want to download responses to file, then you need to specify an output_directory_root. The files will be 
-downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<here_your_files_will_be_downloaded>
+
+# In case you want to download responses to file, then you need to specify an output_directory_root 
+# The files will be downloaded in a subdir: output_directory_root/hdsr_fewspy_<datetime>/<files_will_be_downloaded_here>
 api = hdsr_fewspy.Api(output_directory_root=<path_to_a_dir>)
 ```
 
 ###### Examples 9 different API calls (using api option 3 from above)
 1. get_parameters
 ```
 df = api.get_parameters(output_choice=hdsr_fewspy.OutputChoices.pandas_dataframe_in_memory)
@@ -322,21 +333,21 @@
 
 ### Releases
 [Release history][releases]
 
 ### Contributions
 All contributions, bug reports, documentation improvements, enhancements and ideas are welcome on the [issues page].
 
-### Test Coverage (May 3rd 2023)
+### Test Coverage (May 10th 2023)
 ```
 ---------- coverage: platform win32, python 3.7.12-final-0 -----------
 Name                                                              Stmts   Miss  Cover
 -------------------------------------------------------------------------------------
 hdsr_fewspy\__init__.py                                              10      0   100%
-hdsr_fewspy\api.py                                                  107     16    85%
+hdsr_fewspy\api.py                                                  110     16    85%
 hdsr_fewspy\api_calls\__init__.py                                    18      0   100%
 hdsr_fewspy\api_calls\base.py                                       100     12    88%
 hdsr_fewspy\api_calls\get_filters.py                                 25      0   100%
 hdsr_fewspy\api_calls\get_locations.py                               44      2    95%
 hdsr_fewspy\api_calls\get_parameters.py                              40      1    98%
 hdsr_fewspy\api_calls\get_qualifiers.py                              50     16    68%
 hdsr_fewspy\api_calls\get_samples.py                                 24      8    67%
@@ -344,30 +355,30 @@
 hdsr_fewspy\api_calls\time_series\base.py                           109      9    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_multi.py           73      6    92%
 hdsr_fewspy\api_calls\time_series\get_time_series_single.py          35      2    94%
 hdsr_fewspy\api_calls\time_series\get_time_series_statistics.py      23      2    91%
 hdsr_fewspy\constants\choices.py                                     89      3    97%
 hdsr_fewspy\constants\custom_types.py                                 2      0   100%
 hdsr_fewspy\constants\github.py                                       8      0   100%
-hdsr_fewspy\constants\paths.py                                       11      0   100%
+hdsr_fewspy\constants\paths.py                                       10      0   100%
 hdsr_fewspy\constants\pi_settings.py                                 78      7    91%
 hdsr_fewspy\constants\request_settings.py                            12      0   100%
 hdsr_fewspy\converters\download.py                                   82      4    95%
 hdsr_fewspy\converters\json_to_df_timeseries.py                     112      8    93%
 hdsr_fewspy\converters\manager.py                                    27      0   100%
 hdsr_fewspy\converters\utils.py                                      45     17    62%
 hdsr_fewspy\converters\xml_to_python_obj.py                         105     27    74%
 hdsr_fewspy\date_frequency.py                                        46      5    89%
-hdsr_fewspy\exceptions.py                                            16      0   100%
-hdsr_fewspy\permissions.py                                           67      5    93%
+hdsr_fewspy\exceptions.py                                            14      0   100%
+hdsr_fewspy\permissions.py                                           47      1    98%
 hdsr_fewspy\retry_session.py                                         68     12    82%
-hdsr_fewspy\secrets.py                                               64     20    69%
+hdsr_fewspy\secrets.py                                               71     19    73%
 setup.py                                                             10     10     0%
 -------------------------------------------------------------------------------------
-TOTAL                                                              1526    193    87%
+TOTAL                                                              1513    188    88%
 ```
 
 ### Conda general tips
 #### Build conda environment (on Windows) from any directory using environment.yml:
 Note1: prefix is not set in the environment.yml as then conda does not handle it very well
 Note2: env_directory can be anywhere, it does not have to be in your code project
 ```
```

### Comparing `hdsr_fewspy-1.7/hdsr_fewspy.egg-info/SOURCES.txt` & `hdsr_fewspy-1.8/hdsr_fewspy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 hdsr_fewspy/converters/json_to_df_timeseries.py
 hdsr_fewspy/converters/manager.py
 hdsr_fewspy/converters/utils.py
 hdsr_fewspy/converters/xml_to_python_obj.py
 hdsr_fewspy/tests/__init__.py
 hdsr_fewspy/tests/fixtures.py
 hdsr_fewspy/tests/fixtures_requests.py
+hdsr_fewspy/tests/test_custom_secrets.py
 hdsr_fewspy/tests/test_sa_get_filters.py
 hdsr_fewspy/tests/test_sa_get_locations.py
 hdsr_fewspy/tests/test_sa_get_parameters.py
 hdsr_fewspy/tests/test_sa_get_qualifiers.py
 hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
 hdsr_fewspy/tests/test_sa_get_timeseries_single.py
 hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
```

### Comparing `hdsr_fewspy-1.7/pyproject.toml` & `hdsr_fewspy-1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.7/setup.py` & `hdsr_fewspy-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.7"
+version = "1.8"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
```

