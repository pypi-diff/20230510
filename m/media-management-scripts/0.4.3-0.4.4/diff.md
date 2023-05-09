# Comparing `tmp/media_management_scripts-0.4.3.tar.gz` & `tmp/media_management_scripts-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media_management_scripts-0.4.3.tar", last modified: Tue May  9 22:30:50 2023, max compression
+gzip compressed data, was "media_management_scripts-0.4.4.tar", last modified: Tue May  9 22:44:44 2023, max compression
```

## Comparing `media_management_scripts-0.4.3.tar` & `media_management_scripts-0.4.4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.083974 media_management_scripts-0.4.3/
--rw-r--r--   0 ray        (501) staff       (20)    11357 2019-04-07 00:10:23.000000 media_management_scripts-0.4.3/LICENSE
--rw-r--r--   0 ray        (501) staff       (20)    10118 2023-05-09 22:30:50.082965 media_management_scripts-0.4.3/PKG-INFO
--rw-r--r--   0 ray        (501) staff       (20)     9813 2023-05-09 22:30:23.000000 media_management_scripts-0.4.3/README.md
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.032261 media_management_scripts-0.4.3/bin/
--rwxr-xr-x   0 ray        (501) staff       (20)      110 2017-03-14 15:44:20.000000 media_management_scripts-0.4.3/bin/convert-dvds
--rwxr-xr-x   0 ray        (501) staff       (20)      101 2017-03-14 15:44:17.000000 media_management_scripts-0.4.3/bin/manage-media
--rw-r--r--   0 ray        (501) staff       (20)      109 2017-05-26 23:31:56.000000 media_management_scripts-0.4.3/bin/silver-tube
--rw-r--r--   0 ray        (501) staff       (20)      106 2017-06-06 16:33:45.000000 media_management_scripts-0.4.3/bin/tvdb-api
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.037465 media_management_scripts-0.4.3/media_management_scripts/
--rw-r--r--   0 ray        (501) staff       (20)       18 2023-05-09 22:28:54.000000 media_management_scripts-0.4.3/media_management_scripts/__init__.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.054669 media_management_scripts-0.4.3/media_management_scripts/commands/
--rw-r--r--   0 ray        (501) staff       (20)     4412 2020-02-15 19:24:11.000000 media_management_scripts-0.4.3/media_management_scripts/commands/__init__.py
--rw-r--r--   0 ray        (501) staff       (20)     3940 2018-03-31 17:25:16.000000 media_management_scripts-0.4.3/media_management_scripts/commands/combine_subtitles.py
--rw-r--r--   0 ray        (501) staff       (20)     4587 2020-05-24 20:13:38.000000 media_management_scripts-0.4.3/media_management_scripts/commands/common.py
--rw-r--r--   0 ray        (501) staff       (20)     2022 2018-03-16 16:08:57.000000 media_management_scripts-0.4.3/media_management_scripts/commands/compare_directories.py
--rw-r--r--   0 ray        (501) staff       (20)     1334 2018-04-29 18:26:01.000000 media_management_scripts-0.4.3/media_management_scripts/commands/concat_mp4.py
--rw-r--r--   0 ray        (501) staff       (20)     2589 2023-05-09 22:24:39.000000 media_management_scripts-0.4.3/media_management_scripts/commands/convert.py
--rw-r--r--   0 ray        (501) staff       (20)      906 2019-06-30 00:45:56.000000 media_management_scripts-0.4.3/media_management_scripts/commands/executables.py
--rw-r--r--   0 ray        (501) staff       (20)     2632 2018-07-03 22:57:34.000000 media_management_scripts-0.4.3/media_management_scripts/commands/filebot.py
--rw-r--r--   0 ray        (501) staff       (20)     2459 2023-04-22 15:28:09.000000 media_management_scripts-0.4.3/media_management_scripts/commands/find_episodes.py
--rw-r--r--   0 ray        (501) staff       (20)     6436 2018-12-30 00:48:19.000000 media_management_scripts-0.4.3/media_management_scripts/commands/itunes.py
--rw-r--r--   0 ray        (501) staff       (20)     4262 2018-12-30 00:50:03.000000 media_management_scripts-0.4.3/media_management_scripts/commands/metadata.py
--rw-r--r--   0 ray        (501) staff       (20)     4553 2018-03-07 00:34:19.000000 media_management_scripts-0.4.3/media_management_scripts/commands/metadata_compare.py
--rw-r--r--   0 ray        (501) staff       (20)     1293 2018-12-25 13:41:04.000000 media_management_scripts-0.4.3/media_management_scripts/commands/movie_rename.py
--rw-r--r--   0 ray        (501) staff       (20)     4792 2017-10-21 01:38:51.000000 media_management_scripts-0.4.3/media_management_scripts/commands/rename.py
--rw-r--r--   0 ray        (501) staff       (20)     7959 2023-04-22 15:53:42.000000 media_management_scripts-0.4.3/media_management_scripts/commands/search.py
--rw-r--r--   0 ray        (501) staff       (20)     6360 2018-12-30 00:51:02.000000 media_management_scripts-0.4.3/media_management_scripts/commands/select_streams.py
--rw-r--r--   0 ray        (501) staff       (20)     1560 2020-02-18 00:32:52.000000 media_management_scripts-0.4.3/media_management_scripts/commands/split.py
--rw-r--r--   0 ray        (501) staff       (20)     2154 2018-01-14 04:10:22.000000 media_management_scripts-0.4.3/media_management_scripts/commands/subtitles.py
--rw-r--r--   0 ray        (501) staff       (20)     1923 2020-02-18 00:28:58.000000 media_management_scripts-0.4.3/media_management_scripts/commands/thumbnail.py
--rw-r--r--   0 ray        (501) staff       (20)     4651 2018-12-30 00:56:36.000000 media_management_scripts-0.4.3/media_management_scripts/commands/tv_rename.py
--rw-r--r--   0 ray        (501) staff       (20)    12369 2020-09-28 20:57:45.000000 media_management_scripts-0.4.3/media_management_scripts/convert.py
--rw-r--r--   0 ray        (501) staff       (20)    11664 2020-04-26 16:48:51.000000 media_management_scripts-0.4.3/media_management_scripts/convert_daemon.py
--rw-r--r--   0 ray        (501) staff       (20)     1564 2020-05-08 23:13:37.000000 media_management_scripts-0.4.3/media_management_scripts/main.py
--rw-r--r--   0 ray        (501) staff       (20)     4414 2020-12-19 17:25:08.000000 media_management_scripts-0.4.3/media_management_scripts/moviedb.py
--rw-r--r--   0 ray        (501) staff       (20)     4047 2018-01-25 20:23:46.000000 media_management_scripts-0.4.3/media_management_scripts/renamer.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.058547 media_management_scripts-0.4.3/media_management_scripts/silver_tube/
--rw-r--r--   0 ray        (501) staff       (20)     1966 2018-04-29 15:31:18.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/__init__.py
--rw-r--r--   0 ray        (501) staff       (20)     1797 2017-07-16 20:17:22.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/delete_process.py
--rw-r--r--   0 ray        (501) staff       (20)    15053 2017-11-16 21:13:15.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/processing.py
--rw-r--r--   0 ray        (501) staff       (20)      882 2017-05-24 16:08:17.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/wtv.py
--rw-r--r--   0 ray        (501) staff       (20)     9229 2017-10-14 14:18:26.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/wtv_db.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.069815 media_management_scripts-0.4.3/media_management_scripts/support/
--rw-r--r--   0 ray        (501) staff       (20)        0 2017-01-12 22:29:21.000000 media_management_scripts-0.4.3/media_management_scripts/support/__init__.py
--rw-r--r--   0 ray        (501) staff       (20)     2213 2018-02-16 10:46:22.000000 media_management_scripts-0.4.3/media_management_scripts/support/combine_all.py
--rw-r--r--   0 ray        (501) staff       (20)     2672 2018-12-16 03:53:55.000000 media_management_scripts-0.4.3/media_management_scripts/support/concat_mp4.py
--rw-r--r--   0 ray        (501) staff       (20)     3949 2020-09-23 22:07:37.000000 media_management_scripts-0.4.3/media_management_scripts/support/encoding.py
--rw-r--r--   0 ray        (501) staff       (20)     4443 2023-04-22 15:48:04.000000 media_management_scripts-0.4.3/media_management_scripts/support/episode_finder.py
--rw-r--r--   0 ray        (501) staff       (20)     7662 2019-06-30 00:50:10.000000 media_management_scripts-0.4.3/media_management_scripts/support/executables.py
--rw-r--r--   0 ray        (501) staff       (20)     3143 2023-04-22 15:43:16.000000 media_management_scripts-0.4.3/media_management_scripts/support/files.py
--rw-r--r--   0 ray        (501) staff       (20)     1465 2020-09-28 20:52:58.000000 media_management_scripts-0.4.3/media_management_scripts/support/formatting.py
--rw-r--r--   0 ray        (501) staff       (20)     5658 2017-07-28 18:19:35.000000 media_management_scripts-0.4.3/media_management_scripts/support/interlace.py
--rw-r--r--   0 ray        (501) staff       (20)    11649 2018-04-14 01:18:43.000000 media_management_scripts-0.4.3/media_management_scripts/support/metadata.py
--rw-r--r--   0 ray        (501) staff       (20)     4220 2017-12-20 12:39:48.000000 media_management_scripts-0.4.3/media_management_scripts/support/movie_rename.py
--rw-r--r--   0 ray        (501) staff       (20)     7444 2017-08-22 14:25:38.000000 media_management_scripts-0.4.3/media_management_scripts/support/search_parser.py
--rw-r--r--   0 ray        (501) staff       (20)      975 2017-10-01 01:58:34.000000 media_management_scripts-0.4.3/media_management_scripts/support/split.py
--rw-r--r--   0 ray        (501) staff       (20)     7690 2018-01-23 17:59:18.000000 media_management_scripts-0.4.3/media_management_scripts/support/ttml2srt.py
--rw-r--r--   0 ray        (501) staff       (20)     7867 2018-12-30 00:57:48.000000 media_management_scripts-0.4.3/media_management_scripts/tvdb_api.py
--rw-r--r--   0 ray        (501) staff       (20)     5455 2023-04-22 14:52:48.000000 media_management_scripts-0.4.3/media_management_scripts/utils.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.040260 media_management_scripts-0.4.3/media_management_scripts.egg-info/
--rw-r--r--   0 ray        (501) staff       (20)    10118 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/PKG-INFO
--rw-r--r--   0 ray        (501) staff       (20)     2808 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 ray        (501) staff       (20)        1 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 ray        (501) staff       (20)        1 2017-01-14 23:17:49.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/not-zip-safe
--rw-r--r--   0 ray        (501) staff       (20)      143 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/requires.txt
--rw-r--r--   0 ray        (501) staff       (20)       25 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/top_level.txt
--rw-r--r--   0 ray        (501) staff       (20)       38 2023-05-09 22:30:50.084195 media_management_scripts-0.4.3/setup.cfg
--rw-r--r--   0 ray        (501) staff       (20)     1251 2019-06-30 01:01:42.000000 media_management_scripts-0.4.3/setup.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.081952 media_management_scripts-0.4.3/tests/
--rw-r--r--   0 ray        (501) staff       (20)     3638 2017-12-23 01:42:50.000000 media_management_scripts-0.4.3/tests/test_combine.py
--rw-r--r--   0 ray        (501) staff       (20)     3345 2018-04-29 19:08:54.000000 media_management_scripts-0.4.3/tests/test_concat_mp4.py
--rw-r--r--   0 ray        (501) staff       (20)     8456 2020-05-24 20:13:38.000000 media_management_scripts-0.4.3/tests/test_convert.py
--rw-r--r--   0 ray        (501) staff       (20)    10091 2018-03-15 17:13:31.000000 media_management_scripts-0.4.3/tests/test_convert_dvd.py
--rw-r--r--   0 ray        (501) staff       (20)     4051 2023-04-22 15:03:00.000000 media_management_scripts-0.4.3/tests/test_find_episodes.py
--rw-r--r--   0 ray        (501) staff       (20)      690 2020-02-16 23:33:43.000000 media_management_scripts-0.4.3/tests/test_formatting.py
--rw-r--r--   0 ray        (501) staff       (20)     9174 2017-10-28 16:25:41.000000 media_management_scripts-0.4.3/tests/test_metadata.py
--rw-r--r--   0 ray        (501) staff       (20)     7095 2018-01-25 20:26:58.000000 media_management_scripts-0.4.3/tests/test_rename.py
--rw-r--r--   0 ray        (501) staff       (20)     3930 2017-08-12 15:30:56.000000 media_management_scripts-0.4.3/tests/test_search.py
--rw-r--r--   0 ray        (501) staff       (20)     3033 2017-08-22 14:26:44.000000 media_management_scripts-0.4.3/tests/test_search_parser.py
--rw-r--r--   0 ray        (501) staff       (20)     7623 2020-04-25 16:09:10.000000 media_management_scripts-0.4.3/tests/test_silver_tube.py
--rw-r--r--   0 ray        (501) staff       (20)      951 2023-04-22 15:24:11.000000 media_management_scripts-0.4.3/tests/test_utils.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:44:44.402514 media_management_scripts-0.4.4/
+-rw-r--r--   0 ray        (501) staff       (20)    11357 2019-04-07 00:10:23.000000 media_management_scripts-0.4.4/LICENSE
+-rw-r--r--   0 ray        (501) staff       (20)    10118 2023-05-09 22:44:44.401661 media_management_scripts-0.4.4/PKG-INFO
+-rw-r--r--   0 ray        (501) staff       (20)     9813 2023-05-09 22:30:23.000000 media_management_scripts-0.4.4/README.md
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:44:44.364584 media_management_scripts-0.4.4/bin/
+-rwxr-xr-x   0 ray        (501) staff       (20)      110 2017-03-14 15:44:20.000000 media_management_scripts-0.4.4/bin/convert-dvds
+-rwxr-xr-x   0 ray        (501) staff       (20)      101 2017-03-14 15:44:17.000000 media_management_scripts-0.4.4/bin/manage-media
+-rw-r--r--   0 ray        (501) staff       (20)      109 2017-05-26 23:31:56.000000 media_management_scripts-0.4.4/bin/silver-tube
+-rw-r--r--   0 ray        (501) staff       (20)      106 2017-06-06 16:33:45.000000 media_management_scripts-0.4.4/bin/tvdb-api
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:44:44.367846 media_management_scripts-0.4.4/media_management_scripts/
+-rw-r--r--   0 ray        (501) staff       (20)       18 2023-05-09 22:43:44.000000 media_management_scripts-0.4.4/media_management_scripts/__init__.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:44:44.384202 media_management_scripts-0.4.4/media_management_scripts/commands/
+-rw-r--r--   0 ray        (501) staff       (20)     4412 2020-02-15 19:24:11.000000 media_management_scripts-0.4.4/media_management_scripts/commands/__init__.py
+-rw-r--r--   0 ray        (501) staff       (20)     3940 2018-03-31 17:25:16.000000 media_management_scripts-0.4.4/media_management_scripts/commands/combine_subtitles.py
+-rw-r--r--   0 ray        (501) staff       (20)     4587 2020-05-24 20:13:38.000000 media_management_scripts-0.4.4/media_management_scripts/commands/common.py
+-rw-r--r--   0 ray        (501) staff       (20)     2022 2018-03-16 16:08:57.000000 media_management_scripts-0.4.4/media_management_scripts/commands/compare_directories.py
+-rw-r--r--   0 ray        (501) staff       (20)     1334 2018-04-29 18:26:01.000000 media_management_scripts-0.4.4/media_management_scripts/commands/concat_mp4.py
+-rw-r--r--   0 ray        (501) staff       (20)     2875 2023-05-09 22:43:14.000000 media_management_scripts-0.4.4/media_management_scripts/commands/convert.py
+-rw-r--r--   0 ray        (501) staff       (20)      906 2019-06-30 00:45:56.000000 media_management_scripts-0.4.4/media_management_scripts/commands/executables.py
+-rw-r--r--   0 ray        (501) staff       (20)     2632 2018-07-03 22:57:34.000000 media_management_scripts-0.4.4/media_management_scripts/commands/filebot.py
+-rw-r--r--   0 ray        (501) staff       (20)     2459 2023-04-22 15:28:09.000000 media_management_scripts-0.4.4/media_management_scripts/commands/find_episodes.py
+-rw-r--r--   0 ray        (501) staff       (20)     6436 2018-12-30 00:48:19.000000 media_management_scripts-0.4.4/media_management_scripts/commands/itunes.py
+-rw-r--r--   0 ray        (501) staff       (20)     4262 2018-12-30 00:50:03.000000 media_management_scripts-0.4.4/media_management_scripts/commands/metadata.py
+-rw-r--r--   0 ray        (501) staff       (20)     4553 2018-03-07 00:34:19.000000 media_management_scripts-0.4.4/media_management_scripts/commands/metadata_compare.py
+-rw-r--r--   0 ray        (501) staff       (20)     1293 2018-12-25 13:41:04.000000 media_management_scripts-0.4.4/media_management_scripts/commands/movie_rename.py
+-rw-r--r--   0 ray        (501) staff       (20)     4792 2017-10-21 01:38:51.000000 media_management_scripts-0.4.4/media_management_scripts/commands/rename.py
+-rw-r--r--   0 ray        (501) staff       (20)     7959 2023-04-22 15:53:42.000000 media_management_scripts-0.4.4/media_management_scripts/commands/search.py
+-rw-r--r--   0 ray        (501) staff       (20)     6360 2018-12-30 00:51:02.000000 media_management_scripts-0.4.4/media_management_scripts/commands/select_streams.py
+-rw-r--r--   0 ray        (501) staff       (20)     1560 2020-02-18 00:32:52.000000 media_management_scripts-0.4.4/media_management_scripts/commands/split.py
+-rw-r--r--   0 ray        (501) staff       (20)     2154 2018-01-14 04:10:22.000000 media_management_scripts-0.4.4/media_management_scripts/commands/subtitles.py
+-rw-r--r--   0 ray        (501) staff       (20)     1923 2020-02-18 00:28:58.000000 media_management_scripts-0.4.4/media_management_scripts/commands/thumbnail.py
+-rw-r--r--   0 ray        (501) staff       (20)     4651 2018-12-30 00:56:36.000000 media_management_scripts-0.4.4/media_management_scripts/commands/tv_rename.py
+-rw-r--r--   0 ray        (501) staff       (20)    12369 2020-09-28 20:57:45.000000 media_management_scripts-0.4.4/media_management_scripts/convert.py
+-rw-r--r--   0 ray        (501) staff       (20)    11664 2020-04-26 16:48:51.000000 media_management_scripts-0.4.4/media_management_scripts/convert_daemon.py
+-rw-r--r--   0 ray        (501) staff       (20)     1564 2020-05-08 23:13:37.000000 media_management_scripts-0.4.4/media_management_scripts/main.py
+-rw-r--r--   0 ray        (501) staff       (20)     4414 2020-12-19 17:25:08.000000 media_management_scripts-0.4.4/media_management_scripts/moviedb.py
+-rw-r--r--   0 ray        (501) staff       (20)     4047 2018-01-25 20:23:46.000000 media_management_scripts-0.4.4/media_management_scripts/renamer.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:44:44.387369 media_management_scripts-0.4.4/media_management_scripts/silver_tube/
+-rw-r--r--   0 ray        (501) staff       (20)     1966 2018-04-29 15:31:18.000000 media_management_scripts-0.4.4/media_management_scripts/silver_tube/__init__.py
+-rw-r--r--   0 ray        (501) staff       (20)     1797 2017-07-16 20:17:22.000000 media_management_scripts-0.4.4/media_management_scripts/silver_tube/delete_process.py
+-rw-r--r--   0 ray        (501) staff       (20)    15053 2017-11-16 21:13:15.000000 media_management_scripts-0.4.4/media_management_scripts/silver_tube/processing.py
+-rw-r--r--   0 ray        (501) staff       (20)      882 2017-05-24 16:08:17.000000 media_management_scripts-0.4.4/media_management_scripts/silver_tube/wtv.py
+-rw-r--r--   0 ray        (501) staff       (20)     9229 2017-10-14 14:18:26.000000 media_management_scripts-0.4.4/media_management_scripts/silver_tube/wtv_db.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:44:44.394487 media_management_scripts-0.4.4/media_management_scripts/support/
+-rw-r--r--   0 ray        (501) staff       (20)        0 2017-01-12 22:29:21.000000 media_management_scripts-0.4.4/media_management_scripts/support/__init__.py
+-rw-r--r--   0 ray        (501) staff       (20)     2213 2018-02-16 10:46:22.000000 media_management_scripts-0.4.4/media_management_scripts/support/combine_all.py
+-rw-r--r--   0 ray        (501) staff       (20)     2672 2018-12-16 03:53:55.000000 media_management_scripts-0.4.4/media_management_scripts/support/concat_mp4.py
+-rw-r--r--   0 ray        (501) staff       (20)     3949 2020-09-23 22:07:37.000000 media_management_scripts-0.4.4/media_management_scripts/support/encoding.py
+-rw-r--r--   0 ray        (501) staff       (20)     4443 2023-04-22 15:48:04.000000 media_management_scripts-0.4.4/media_management_scripts/support/episode_finder.py
+-rw-r--r--   0 ray        (501) staff       (20)     7662 2019-06-30 00:50:10.000000 media_management_scripts-0.4.4/media_management_scripts/support/executables.py
+-rw-r--r--   0 ray        (501) staff       (20)     3147 2023-05-09 22:34:29.000000 media_management_scripts-0.4.4/media_management_scripts/support/files.py
+-rw-r--r--   0 ray        (501) staff       (20)     1465 2020-09-28 20:52:58.000000 media_management_scripts-0.4.4/media_management_scripts/support/formatting.py
+-rw-r--r--   0 ray        (501) staff       (20)     5658 2017-07-28 18:19:35.000000 media_management_scripts-0.4.4/media_management_scripts/support/interlace.py
+-rw-r--r--   0 ray        (501) staff       (20)    11649 2018-04-14 01:18:43.000000 media_management_scripts-0.4.4/media_management_scripts/support/metadata.py
+-rw-r--r--   0 ray        (501) staff       (20)     4220 2017-12-20 12:39:48.000000 media_management_scripts-0.4.4/media_management_scripts/support/movie_rename.py
+-rw-r--r--   0 ray        (501) staff       (20)     7444 2017-08-22 14:25:38.000000 media_management_scripts-0.4.4/media_management_scripts/support/search_parser.py
+-rw-r--r--   0 ray        (501) staff       (20)      975 2017-10-01 01:58:34.000000 media_management_scripts-0.4.4/media_management_scripts/support/split.py
+-rw-r--r--   0 ray        (501) staff       (20)     7690 2018-01-23 17:59:18.000000 media_management_scripts-0.4.4/media_management_scripts/support/ttml2srt.py
+-rw-r--r--   0 ray        (501) staff       (20)     7867 2018-12-30 00:57:48.000000 media_management_scripts-0.4.4/media_management_scripts/tvdb_api.py
+-rw-r--r--   0 ray        (501) staff       (20)     5455 2023-04-22 14:52:48.000000 media_management_scripts-0.4.4/media_management_scripts/utils.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:44:44.371990 media_management_scripts-0.4.4/media_management_scripts.egg-info/
+-rw-r--r--   0 ray        (501) staff       (20)    10118 2023-05-09 22:44:44.000000 media_management_scripts-0.4.4/media_management_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 ray        (501) staff       (20)     2808 2023-05-09 22:44:44.000000 media_management_scripts-0.4.4/media_management_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 ray        (501) staff       (20)        1 2023-05-09 22:44:44.000000 media_management_scripts-0.4.4/media_management_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 ray        (501) staff       (20)        1 2017-01-14 23:17:49.000000 media_management_scripts-0.4.4/media_management_scripts.egg-info/not-zip-safe
+-rw-r--r--   0 ray        (501) staff       (20)      143 2023-05-09 22:44:44.000000 media_management_scripts-0.4.4/media_management_scripts.egg-info/requires.txt
+-rw-r--r--   0 ray        (501) staff       (20)       25 2023-05-09 22:44:44.000000 media_management_scripts-0.4.4/media_management_scripts.egg-info/top_level.txt
+-rw-r--r--   0 ray        (501) staff       (20)       38 2023-05-09 22:44:44.402678 media_management_scripts-0.4.4/setup.cfg
+-rw-r--r--   0 ray        (501) staff       (20)     1251 2019-06-30 01:01:42.000000 media_management_scripts-0.4.4/setup.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:44:44.400863 media_management_scripts-0.4.4/tests/
+-rw-r--r--   0 ray        (501) staff       (20)     3638 2017-12-23 01:42:50.000000 media_management_scripts-0.4.4/tests/test_combine.py
+-rw-r--r--   0 ray        (501) staff       (20)     3345 2018-04-29 19:08:54.000000 media_management_scripts-0.4.4/tests/test_concat_mp4.py
+-rw-r--r--   0 ray        (501) staff       (20)     8456 2020-05-24 20:13:38.000000 media_management_scripts-0.4.4/tests/test_convert.py
+-rw-r--r--   0 ray        (501) staff       (20)    10091 2018-03-15 17:13:31.000000 media_management_scripts-0.4.4/tests/test_convert_dvd.py
+-rw-r--r--   0 ray        (501) staff       (20)     4051 2023-04-22 15:03:00.000000 media_management_scripts-0.4.4/tests/test_find_episodes.py
+-rw-r--r--   0 ray        (501) staff       (20)      690 2020-02-16 23:33:43.000000 media_management_scripts-0.4.4/tests/test_formatting.py
+-rw-r--r--   0 ray        (501) staff       (20)     9174 2017-10-28 16:25:41.000000 media_management_scripts-0.4.4/tests/test_metadata.py
+-rw-r--r--   0 ray        (501) staff       (20)     7095 2018-01-25 20:26:58.000000 media_management_scripts-0.4.4/tests/test_rename.py
+-rw-r--r--   0 ray        (501) staff       (20)     3930 2017-08-12 15:30:56.000000 media_management_scripts-0.4.4/tests/test_search.py
+-rw-r--r--   0 ray        (501) staff       (20)     3033 2017-08-22 14:26:44.000000 media_management_scripts-0.4.4/tests/test_search_parser.py
+-rw-r--r--   0 ray        (501) staff       (20)     7623 2020-04-25 16:09:10.000000 media_management_scripts-0.4.4/tests/test_silver_tube.py
+-rw-r--r--   0 ray        (501) staff       (20)      951 2023-04-22 15:24:11.000000 media_management_scripts-0.4.4/tests/test_utils.py
```

### Comparing `media_management_scripts-0.4.3/LICENSE` & `media_management_scripts-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/PKG-INFO` & `media_management_scripts-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media_management_scripts
-Version: 0.4.3
+Version: 0.4.4
 Summary: Scripts for managing media
 Home-page: https://github.com/raydouglass/media_management_scripts
 Author: Ray Douglass
 Author-email: ray@raydouglass.com
 License: Apache
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `media_management_scripts-0.4.3/README.md` & `media_management_scripts-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/__init__.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/combine_subtitles.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/combine_subtitles.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/common.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/common.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/compare_directories.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/compare_directories.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/concat_mp4.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/concat_mp4.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/convert.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,28 +34,32 @@
 
         convert_parser = subparser.add_parser('convert', help='Convert a file',
                                               parents=[parent_parser, input_parser, convert_parent_parser, output_parser],
                                               formatter_class=argparse.RawTextHelpFormatter,
                                               description=desc)
         convert_parser.add_argument('--bulk', help='Enables bulk conversion mode', action='store_const', const=True,
                                     default=False)
+        convert_parser.add_argument('--bulk-ext', help='Use a difference extension for the output files', default=None)
 
     def subexecute(self, ns):
         import os
         from media_management_scripts.convert import convert_config_from_ns
         input_to_cmd = ns['input']
         output = ns['output']
         overwrite = ns['overwrite']
         bulk = ns['bulk']
+        bulk_ext = ns['bulk_ext']
         config = convert_config_from_ns(ns)
 
         if os.path.isdir(input_to_cmd):
             if bulk:
                 os.makedirs(output, exist_ok=True)
                 files = list(get_input_output(input_to_cmd, output, filter=movie_files_filter))
+                if bulk_ext:
+                    files = list(map(lambda i: (i[0], os.path.splitext(i[1])[0]+'.'+bulk_ext), files))
                 self._bulk(files, lambda i, o: _bulk_convert(i, o, config, overwrite), ['Input', 'Output'])
             else:
                 print('Cowardly refusing to convert a direction without --bulk flag')
         elif not overwrite and os.path.exists(output):
             print('Cowardly refusing to overwrite existing file: {}'.format(output))
         else:
             convert_with_config(input_to_cmd, output, config, print_output=True, overwrite=overwrite)
```

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/executables.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/executables.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/filebot.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/filebot.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/find_episodes.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/find_episodes.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/itunes.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/itunes.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/metadata.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/metadata_compare.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/metadata_compare.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/movie_rename.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/movie_rename.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/rename.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/rename.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/search.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/search.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/select_streams.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/select_streams.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/split.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/split.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/subtitles.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/subtitles.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/thumbnail.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/thumbnail.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/commands/tv_rename.py` & `media_management_scripts-0.4.4/media_management_scripts/commands/tv_rename.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/convert.py` & `media_management_scripts-0.4.4/media_management_scripts/convert.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/convert_daemon.py` & `media_management_scripts-0.4.4/media_management_scripts/convert_daemon.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/main.py` & `media_management_scripts-0.4.4/media_management_scripts/main.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/moviedb.py` & `media_management_scripts-0.4.4/media_management_scripts/moviedb.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/renamer.py` & `media_management_scripts-0.4.4/media_management_scripts/renamer.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/silver_tube/__init__.py` & `media_management_scripts-0.4.4/media_management_scripts/silver_tube/__init__.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/silver_tube/delete_process.py` & `media_management_scripts-0.4.4/media_management_scripts/silver_tube/delete_process.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/silver_tube/processing.py` & `media_management_scripts-0.4.4/media_management_scripts/silver_tube/processing.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/silver_tube/wtv.py` & `media_management_scripts-0.4.4/media_management_scripts/silver_tube/wtv.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/silver_tube/wtv_db.py` & `media_management_scripts-0.4.4/media_management_scripts/silver_tube/wtv_db.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/combine_all.py` & `media_management_scripts-0.4.4/media_management_scripts/support/combine_all.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/concat_mp4.py` & `media_management_scripts-0.4.4/media_management_scripts/support/concat_mp4.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/encoding.py` & `media_management_scripts-0.4.4/media_management_scripts/support/encoding.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/episode_finder.py` & `media_management_scripts-0.4.4/media_management_scripts/support/episode_finder.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/executables.py` & `media_management_scripts-0.4.4/media_management_scripts/support/executables.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/files.py` & `media_management_scripts-0.4.4/media_management_scripts/support/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         else:
             yield input_dir
 
 
 def get_input_output(input_dir: str,
                      output_dir: str,
                      work_dir: str = None,
-                     filter: Callable[[str], bool] = mp4_mkv_filter) -> Iterator[Tuple[str, ...]]:
+                     filter: Callable[[str], bool] = movie_files_filter) -> Iterator[Tuple[str, ...]]:
     """
     Mimic the file structure from input_dir into output_dir (and optionally work_dir).
 
     The input files are filtered
     """
     for file in sorted(list_files(input_dir, filter)):
         input_file = os.path.join(input_dir, file)
```

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/formatting.py` & `media_management_scripts-0.4.4/media_management_scripts/support/formatting.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/interlace.py` & `media_management_scripts-0.4.4/media_management_scripts/support/interlace.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/metadata.py` & `media_management_scripts-0.4.4/media_management_scripts/support/metadata.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/movie_rename.py` & `media_management_scripts-0.4.4/media_management_scripts/support/movie_rename.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/search_parser.py` & `media_management_scripts-0.4.4/media_management_scripts/support/search_parser.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/split.py` & `media_management_scripts-0.4.4/media_management_scripts/support/split.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/support/ttml2srt.py` & `media_management_scripts-0.4.4/media_management_scripts/support/ttml2srt.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/tvdb_api.py` & `media_management_scripts-0.4.4/media_management_scripts/tvdb_api.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts/utils.py` & `media_management_scripts-0.4.4/media_management_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/media_management_scripts.egg-info/PKG-INFO` & `media_management_scripts-0.4.4/media_management_scripts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: media-management-scripts
-Version: 0.4.3
+Version: 0.4.4
 Summary: Scripts for managing media
 Home-page: https://github.com/raydouglass/media_management_scripts
 Author: Ray Douglass
 Author-email: ray@raydouglass.com
 License: Apache
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `media_management_scripts-0.4.3/media_management_scripts.egg-info/SOURCES.txt` & `media_management_scripts-0.4.4/media_management_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/setup.py` & `media_management_scripts-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_combine.py` & `media_management_scripts-0.4.4/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_concat_mp4.py` & `media_management_scripts-0.4.4/tests/test_concat_mp4.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_convert.py` & `media_management_scripts-0.4.4/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_convert_dvd.py` & `media_management_scripts-0.4.4/tests/test_convert_dvd.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_find_episodes.py` & `media_management_scripts-0.4.4/tests/test_find_episodes.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_formatting.py` & `media_management_scripts-0.4.4/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_metadata.py` & `media_management_scripts-0.4.4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_rename.py` & `media_management_scripts-0.4.4/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_search.py` & `media_management_scripts-0.4.4/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_search_parser.py` & `media_management_scripts-0.4.4/tests/test_search_parser.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_silver_tube.py` & `media_management_scripts-0.4.4/tests/test_silver_tube.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.3/tests/test_utils.py` & `media_management_scripts-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

