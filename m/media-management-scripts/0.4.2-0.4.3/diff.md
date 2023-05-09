# Comparing `tmp/media_management_scripts-0.4.2.tar.gz` & `tmp/media_management_scripts-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/media_management_scripts-0.4.2.tar", last modified: Sun Apr 26 16:53:52 2020, max compression
+gzip compressed data, was "media_management_scripts-0.4.3.tar", last modified: Tue May  9 22:30:50 2023, max compression
```

## Comparing `media_management_scripts-0.4.2.tar` & `media_management_scripts-0.4.3.tar`

### file list

```diff
@@ -1,68 +1,82 @@
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/
--rw-r--r--   0 ray        (501) staff       (20)    12334 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/PKG-INFO
--rw-r--r--   0 ray        (501) staff       (20)     9628 2019-06-30 16:53:33.000000 media_management_scripts-0.4.2/README.md
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/bin/
--rwxr-xr-x   0 ray        (501) staff       (20)      110 2017-03-14 15:44:20.000000 media_management_scripts-0.4.2/bin/convert-dvds
--rwxr-xr-x   0 ray        (501) staff       (20)      101 2017-03-14 15:44:17.000000 media_management_scripts-0.4.2/bin/manage-media
--rw-r--r--   0 ray        (501) staff       (20)      109 2017-05-26 23:31:56.000000 media_management_scripts-0.4.2/bin/silver-tube
--rw-r--r--   0 ray        (501) staff       (20)      106 2017-06-06 16:33:45.000000 media_management_scripts-0.4.2/bin/tvdb-api
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts/
--rw-r--r--   0 ray        (501) staff       (20)       18 2020-04-26 16:37:20.000000 media_management_scripts-0.4.2/media_management_scripts/__init__.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts/commands/
--rw-r--r--   0 ray        (501) staff       (20)     4412 2020-02-15 19:24:11.000000 media_management_scripts-0.4.2/media_management_scripts/commands/__init__.py
--rw-r--r--   0 ray        (501) staff       (20)     3940 2018-03-31 17:25:16.000000 media_management_scripts-0.4.2/media_management_scripts/commands/combine_subtitles.py
--rw-r--r--   0 ray        (501) staff       (20)     4335 2020-02-18 00:31:12.000000 media_management_scripts-0.4.2/media_management_scripts/commands/common.py
--rw-r--r--   0 ray        (501) staff       (20)     2022 2018-03-16 16:08:57.000000 media_management_scripts-0.4.2/media_management_scripts/commands/compare_directories.py
--rw-r--r--   0 ray        (501) staff       (20)     1334 2018-04-29 18:26:01.000000 media_management_scripts-0.4.2/media_management_scripts/commands/concat_mp4.py
--rw-r--r--   0 ray        (501) staff       (20)     2364 2019-04-06 23:14:02.000000 media_management_scripts-0.4.2/media_management_scripts/commands/convert.py
--rw-r--r--   0 ray        (501) staff       (20)      906 2019-06-30 00:45:56.000000 media_management_scripts-0.4.2/media_management_scripts/commands/executables.py
--rw-r--r--   0 ray        (501) staff       (20)     2632 2018-07-03 22:57:34.000000 media_management_scripts-0.4.2/media_management_scripts/commands/filebot.py
--rw-r--r--   0 ray        (501) staff       (20)     4867 2017-09-01 21:57:12.000000 media_management_scripts-0.4.2/media_management_scripts/commands/find_episodes.py
--rw-r--r--   0 ray        (501) staff       (20)     6436 2018-12-30 00:48:19.000000 media_management_scripts-0.4.2/media_management_scripts/commands/itunes.py
--rw-r--r--   0 ray        (501) staff       (20)     4262 2018-12-30 00:50:03.000000 media_management_scripts-0.4.2/media_management_scripts/commands/metadata.py
--rw-r--r--   0 ray        (501) staff       (20)     4553 2018-03-07 00:34:19.000000 media_management_scripts-0.4.2/media_management_scripts/commands/metadata_compare.py
--rw-r--r--   0 ray        (501) staff       (20)     1293 2018-12-25 13:41:04.000000 media_management_scripts-0.4.2/media_management_scripts/commands/movie_rename.py
--rw-r--r--   0 ray        (501) staff       (20)     4792 2017-10-21 01:38:51.000000 media_management_scripts-0.4.2/media_management_scripts/commands/rename.py
--rw-r--r--   0 ray        (501) staff       (20)     7959 2018-07-03 23:28:20.000000 media_management_scripts-0.4.2/media_management_scripts/commands/search.py
--rw-r--r--   0 ray        (501) staff       (20)     6360 2018-12-30 00:51:02.000000 media_management_scripts-0.4.2/media_management_scripts/commands/select_streams.py
--rw-r--r--   0 ray        (501) staff       (20)     1560 2020-02-18 00:32:52.000000 media_management_scripts-0.4.2/media_management_scripts/commands/split.py
--rw-r--r--   0 ray        (501) staff       (20)     2154 2018-01-14 04:10:22.000000 media_management_scripts-0.4.2/media_management_scripts/commands/subtitles.py
--rw-r--r--   0 ray        (501) staff       (20)     1923 2020-02-18 00:28:58.000000 media_management_scripts-0.4.2/media_management_scripts/commands/thumbnail.py
--rw-r--r--   0 ray        (501) staff       (20)     4651 2018-12-30 00:56:36.000000 media_management_scripts-0.4.2/media_management_scripts/commands/tv_rename.py
--rw-r--r--   0 ray        (501) staff       (20)    12081 2018-07-28 01:42:18.000000 media_management_scripts-0.4.2/media_management_scripts/convert.py
--rw-r--r--   0 ray        (501) staff       (20)    11664 2020-04-26 16:48:51.000000 media_management_scripts-0.4.2/media_management_scripts/convert_daemon.py
--rw-r--r--   0 ray        (501) staff       (20)     1564 2018-04-03 22:24:31.000000 media_management_scripts-0.4.2/media_management_scripts/main.py
--rw-r--r--   0 ray        (501) staff       (20)     2591 2017-09-25 01:32:20.000000 media_management_scripts-0.4.2/media_management_scripts/moviedb.py
--rw-r--r--   0 ray        (501) staff       (20)     4047 2018-01-25 20:23:46.000000 media_management_scripts-0.4.2/media_management_scripts/renamer.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts/silver_tube/
--rw-r--r--   0 ray        (501) staff       (20)     1966 2018-04-29 15:31:18.000000 media_management_scripts-0.4.2/media_management_scripts/silver_tube/__init__.py
--rw-r--r--   0 ray        (501) staff       (20)     1797 2017-07-16 20:17:22.000000 media_management_scripts-0.4.2/media_management_scripts/silver_tube/delete_process.py
--rw-r--r--   0 ray        (501) staff       (20)    15053 2017-11-16 21:13:15.000000 media_management_scripts-0.4.2/media_management_scripts/silver_tube/processing.py
--rw-r--r--   0 ray        (501) staff       (20)      882 2017-05-24 16:08:17.000000 media_management_scripts-0.4.2/media_management_scripts/silver_tube/wtv.py
--rw-r--r--   0 ray        (501) staff       (20)     9229 2017-10-14 14:18:26.000000 media_management_scripts-0.4.2/media_management_scripts/silver_tube/wtv_db.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts/support/
--rw-r--r--   0 ray        (501) staff       (20)        0 2017-01-12 22:29:21.000000 media_management_scripts-0.4.2/media_management_scripts/support/__init__.py
--rw-r--r--   0 ray        (501) staff       (20)     2213 2018-02-16 10:46:22.000000 media_management_scripts-0.4.2/media_management_scripts/support/combine_all.py
--rw-r--r--   0 ray        (501) staff       (20)     2672 2018-12-16 03:53:55.000000 media_management_scripts-0.4.2/media_management_scripts/support/concat_mp4.py
--rw-r--r--   0 ray        (501) staff       (20)     3901 2018-04-29 19:06:41.000000 media_management_scripts-0.4.2/media_management_scripts/support/encoding.py
--rw-r--r--   0 ray        (501) staff       (20)     3744 2018-02-18 02:33:38.000000 media_management_scripts-0.4.2/media_management_scripts/support/episode_finder.py
--rw-r--r--   0 ray        (501) staff       (20)     7662 2019-06-30 00:50:10.000000 media_management_scripts-0.4.2/media_management_scripts/support/executables.py
--rw-r--r--   0 ray        (501) staff       (20)     2540 2018-07-03 23:26:03.000000 media_management_scripts-0.4.2/media_management_scripts/support/files.py
--rw-r--r--   0 ray        (501) staff       (20)     1383 2020-02-18 00:28:50.000000 media_management_scripts-0.4.2/media_management_scripts/support/formatting.py
--rw-r--r--   0 ray        (501) staff       (20)     5658 2017-07-28 18:19:35.000000 media_management_scripts-0.4.2/media_management_scripts/support/interlace.py
--rw-r--r--   0 ray        (501) staff       (20)    11649 2018-04-14 01:18:43.000000 media_management_scripts-0.4.2/media_management_scripts/support/metadata.py
--rw-r--r--   0 ray        (501) staff       (20)     4220 2017-12-20 12:39:48.000000 media_management_scripts-0.4.2/media_management_scripts/support/movie_rename.py
--rw-r--r--   0 ray        (501) staff       (20)     7444 2017-08-22 14:25:38.000000 media_management_scripts-0.4.2/media_management_scripts/support/search_parser.py
--rw-r--r--   0 ray        (501) staff       (20)      975 2017-10-01 01:58:34.000000 media_management_scripts-0.4.2/media_management_scripts/support/split.py
--rw-r--r--   0 ray        (501) staff       (20)     7690 2018-01-23 17:59:18.000000 media_management_scripts-0.4.2/media_management_scripts/support/ttml2srt.py
--rw-r--r--   0 ray        (501) staff       (20)     7867 2018-12-30 00:57:48.000000 media_management_scripts-0.4.2/media_management_scripts/tvdb_api.py
--rw-r--r--   0 ray        (501) staff       (20)     4988 2018-03-31 16:41:11.000000 media_management_scripts-0.4.2/media_management_scripts/utils.py
-drwxr-xr-x   0 ray        (501) staff       (20)        0 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts.egg-info/
--rw-r--r--   0 ray        (501) staff       (20)    12334 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts.egg-info/PKG-INFO
--rw-r--r--   0 ray        (501) staff       (20)     2513 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 ray        (501) staff       (20)        1 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 ray        (501) staff       (20)        1 2017-01-14 23:17:49.000000 media_management_scripts-0.4.2/media_management_scripts.egg-info/not-zip-safe
--rw-r--r--   0 ray        (501) staff       (20)      143 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts.egg-info/requires.txt
--rw-r--r--   0 ray        (501) staff       (20)       25 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/media_management_scripts.egg-info/top_level.txt
--rw-r--r--   0 ray        (501) staff       (20)       38 2020-04-26 16:53:52.000000 media_management_scripts-0.4.2/setup.cfg
--rw-r--r--   0 ray        (501) staff       (20)     1251 2019-06-30 01:01:42.000000 media_management_scripts-0.4.2/setup.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.083974 media_management_scripts-0.4.3/
+-rw-r--r--   0 ray        (501) staff       (20)    11357 2019-04-07 00:10:23.000000 media_management_scripts-0.4.3/LICENSE
+-rw-r--r--   0 ray        (501) staff       (20)    10118 2023-05-09 22:30:50.082965 media_management_scripts-0.4.3/PKG-INFO
+-rw-r--r--   0 ray        (501) staff       (20)     9813 2023-05-09 22:30:23.000000 media_management_scripts-0.4.3/README.md
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.032261 media_management_scripts-0.4.3/bin/
+-rwxr-xr-x   0 ray        (501) staff       (20)      110 2017-03-14 15:44:20.000000 media_management_scripts-0.4.3/bin/convert-dvds
+-rwxr-xr-x   0 ray        (501) staff       (20)      101 2017-03-14 15:44:17.000000 media_management_scripts-0.4.3/bin/manage-media
+-rw-r--r--   0 ray        (501) staff       (20)      109 2017-05-26 23:31:56.000000 media_management_scripts-0.4.3/bin/silver-tube
+-rw-r--r--   0 ray        (501) staff       (20)      106 2017-06-06 16:33:45.000000 media_management_scripts-0.4.3/bin/tvdb-api
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.037465 media_management_scripts-0.4.3/media_management_scripts/
+-rw-r--r--   0 ray        (501) staff       (20)       18 2023-05-09 22:28:54.000000 media_management_scripts-0.4.3/media_management_scripts/__init__.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.054669 media_management_scripts-0.4.3/media_management_scripts/commands/
+-rw-r--r--   0 ray        (501) staff       (20)     4412 2020-02-15 19:24:11.000000 media_management_scripts-0.4.3/media_management_scripts/commands/__init__.py
+-rw-r--r--   0 ray        (501) staff       (20)     3940 2018-03-31 17:25:16.000000 media_management_scripts-0.4.3/media_management_scripts/commands/combine_subtitles.py
+-rw-r--r--   0 ray        (501) staff       (20)     4587 2020-05-24 20:13:38.000000 media_management_scripts-0.4.3/media_management_scripts/commands/common.py
+-rw-r--r--   0 ray        (501) staff       (20)     2022 2018-03-16 16:08:57.000000 media_management_scripts-0.4.3/media_management_scripts/commands/compare_directories.py
+-rw-r--r--   0 ray        (501) staff       (20)     1334 2018-04-29 18:26:01.000000 media_management_scripts-0.4.3/media_management_scripts/commands/concat_mp4.py
+-rw-r--r--   0 ray        (501) staff       (20)     2589 2023-05-09 22:24:39.000000 media_management_scripts-0.4.3/media_management_scripts/commands/convert.py
+-rw-r--r--   0 ray        (501) staff       (20)      906 2019-06-30 00:45:56.000000 media_management_scripts-0.4.3/media_management_scripts/commands/executables.py
+-rw-r--r--   0 ray        (501) staff       (20)     2632 2018-07-03 22:57:34.000000 media_management_scripts-0.4.3/media_management_scripts/commands/filebot.py
+-rw-r--r--   0 ray        (501) staff       (20)     2459 2023-04-22 15:28:09.000000 media_management_scripts-0.4.3/media_management_scripts/commands/find_episodes.py
+-rw-r--r--   0 ray        (501) staff       (20)     6436 2018-12-30 00:48:19.000000 media_management_scripts-0.4.3/media_management_scripts/commands/itunes.py
+-rw-r--r--   0 ray        (501) staff       (20)     4262 2018-12-30 00:50:03.000000 media_management_scripts-0.4.3/media_management_scripts/commands/metadata.py
+-rw-r--r--   0 ray        (501) staff       (20)     4553 2018-03-07 00:34:19.000000 media_management_scripts-0.4.3/media_management_scripts/commands/metadata_compare.py
+-rw-r--r--   0 ray        (501) staff       (20)     1293 2018-12-25 13:41:04.000000 media_management_scripts-0.4.3/media_management_scripts/commands/movie_rename.py
+-rw-r--r--   0 ray        (501) staff       (20)     4792 2017-10-21 01:38:51.000000 media_management_scripts-0.4.3/media_management_scripts/commands/rename.py
+-rw-r--r--   0 ray        (501) staff       (20)     7959 2023-04-22 15:53:42.000000 media_management_scripts-0.4.3/media_management_scripts/commands/search.py
+-rw-r--r--   0 ray        (501) staff       (20)     6360 2018-12-30 00:51:02.000000 media_management_scripts-0.4.3/media_management_scripts/commands/select_streams.py
+-rw-r--r--   0 ray        (501) staff       (20)     1560 2020-02-18 00:32:52.000000 media_management_scripts-0.4.3/media_management_scripts/commands/split.py
+-rw-r--r--   0 ray        (501) staff       (20)     2154 2018-01-14 04:10:22.000000 media_management_scripts-0.4.3/media_management_scripts/commands/subtitles.py
+-rw-r--r--   0 ray        (501) staff       (20)     1923 2020-02-18 00:28:58.000000 media_management_scripts-0.4.3/media_management_scripts/commands/thumbnail.py
+-rw-r--r--   0 ray        (501) staff       (20)     4651 2018-12-30 00:56:36.000000 media_management_scripts-0.4.3/media_management_scripts/commands/tv_rename.py
+-rw-r--r--   0 ray        (501) staff       (20)    12369 2020-09-28 20:57:45.000000 media_management_scripts-0.4.3/media_management_scripts/convert.py
+-rw-r--r--   0 ray        (501) staff       (20)    11664 2020-04-26 16:48:51.000000 media_management_scripts-0.4.3/media_management_scripts/convert_daemon.py
+-rw-r--r--   0 ray        (501) staff       (20)     1564 2020-05-08 23:13:37.000000 media_management_scripts-0.4.3/media_management_scripts/main.py
+-rw-r--r--   0 ray        (501) staff       (20)     4414 2020-12-19 17:25:08.000000 media_management_scripts-0.4.3/media_management_scripts/moviedb.py
+-rw-r--r--   0 ray        (501) staff       (20)     4047 2018-01-25 20:23:46.000000 media_management_scripts-0.4.3/media_management_scripts/renamer.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.058547 media_management_scripts-0.4.3/media_management_scripts/silver_tube/
+-rw-r--r--   0 ray        (501) staff       (20)     1966 2018-04-29 15:31:18.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/__init__.py
+-rw-r--r--   0 ray        (501) staff       (20)     1797 2017-07-16 20:17:22.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/delete_process.py
+-rw-r--r--   0 ray        (501) staff       (20)    15053 2017-11-16 21:13:15.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/processing.py
+-rw-r--r--   0 ray        (501) staff       (20)      882 2017-05-24 16:08:17.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/wtv.py
+-rw-r--r--   0 ray        (501) staff       (20)     9229 2017-10-14 14:18:26.000000 media_management_scripts-0.4.3/media_management_scripts/silver_tube/wtv_db.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.069815 media_management_scripts-0.4.3/media_management_scripts/support/
+-rw-r--r--   0 ray        (501) staff       (20)        0 2017-01-12 22:29:21.000000 media_management_scripts-0.4.3/media_management_scripts/support/__init__.py
+-rw-r--r--   0 ray        (501) staff       (20)     2213 2018-02-16 10:46:22.000000 media_management_scripts-0.4.3/media_management_scripts/support/combine_all.py
+-rw-r--r--   0 ray        (501) staff       (20)     2672 2018-12-16 03:53:55.000000 media_management_scripts-0.4.3/media_management_scripts/support/concat_mp4.py
+-rw-r--r--   0 ray        (501) staff       (20)     3949 2020-09-23 22:07:37.000000 media_management_scripts-0.4.3/media_management_scripts/support/encoding.py
+-rw-r--r--   0 ray        (501) staff       (20)     4443 2023-04-22 15:48:04.000000 media_management_scripts-0.4.3/media_management_scripts/support/episode_finder.py
+-rw-r--r--   0 ray        (501) staff       (20)     7662 2019-06-30 00:50:10.000000 media_management_scripts-0.4.3/media_management_scripts/support/executables.py
+-rw-r--r--   0 ray        (501) staff       (20)     3143 2023-04-22 15:43:16.000000 media_management_scripts-0.4.3/media_management_scripts/support/files.py
+-rw-r--r--   0 ray        (501) staff       (20)     1465 2020-09-28 20:52:58.000000 media_management_scripts-0.4.3/media_management_scripts/support/formatting.py
+-rw-r--r--   0 ray        (501) staff       (20)     5658 2017-07-28 18:19:35.000000 media_management_scripts-0.4.3/media_management_scripts/support/interlace.py
+-rw-r--r--   0 ray        (501) staff       (20)    11649 2018-04-14 01:18:43.000000 media_management_scripts-0.4.3/media_management_scripts/support/metadata.py
+-rw-r--r--   0 ray        (501) staff       (20)     4220 2017-12-20 12:39:48.000000 media_management_scripts-0.4.3/media_management_scripts/support/movie_rename.py
+-rw-r--r--   0 ray        (501) staff       (20)     7444 2017-08-22 14:25:38.000000 media_management_scripts-0.4.3/media_management_scripts/support/search_parser.py
+-rw-r--r--   0 ray        (501) staff       (20)      975 2017-10-01 01:58:34.000000 media_management_scripts-0.4.3/media_management_scripts/support/split.py
+-rw-r--r--   0 ray        (501) staff       (20)     7690 2018-01-23 17:59:18.000000 media_management_scripts-0.4.3/media_management_scripts/support/ttml2srt.py
+-rw-r--r--   0 ray        (501) staff       (20)     7867 2018-12-30 00:57:48.000000 media_management_scripts-0.4.3/media_management_scripts/tvdb_api.py
+-rw-r--r--   0 ray        (501) staff       (20)     5455 2023-04-22 14:52:48.000000 media_management_scripts-0.4.3/media_management_scripts/utils.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.040260 media_management_scripts-0.4.3/media_management_scripts.egg-info/
+-rw-r--r--   0 ray        (501) staff       (20)    10118 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 ray        (501) staff       (20)     2808 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 ray        (501) staff       (20)        1 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 ray        (501) staff       (20)        1 2017-01-14 23:17:49.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/not-zip-safe
+-rw-r--r--   0 ray        (501) staff       (20)      143 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/requires.txt
+-rw-r--r--   0 ray        (501) staff       (20)       25 2023-05-09 22:30:50.000000 media_management_scripts-0.4.3/media_management_scripts.egg-info/top_level.txt
+-rw-r--r--   0 ray        (501) staff       (20)       38 2023-05-09 22:30:50.084195 media_management_scripts-0.4.3/setup.cfg
+-rw-r--r--   0 ray        (501) staff       (20)     1251 2019-06-30 01:01:42.000000 media_management_scripts-0.4.3/setup.py
+drwxr-xr-x   0 ray        (501) staff       (20)        0 2023-05-09 22:30:50.081952 media_management_scripts-0.4.3/tests/
+-rw-r--r--   0 ray        (501) staff       (20)     3638 2017-12-23 01:42:50.000000 media_management_scripts-0.4.3/tests/test_combine.py
+-rw-r--r--   0 ray        (501) staff       (20)     3345 2018-04-29 19:08:54.000000 media_management_scripts-0.4.3/tests/test_concat_mp4.py
+-rw-r--r--   0 ray        (501) staff       (20)     8456 2020-05-24 20:13:38.000000 media_management_scripts-0.4.3/tests/test_convert.py
+-rw-r--r--   0 ray        (501) staff       (20)    10091 2018-03-15 17:13:31.000000 media_management_scripts-0.4.3/tests/test_convert_dvd.py
+-rw-r--r--   0 ray        (501) staff       (20)     4051 2023-04-22 15:03:00.000000 media_management_scripts-0.4.3/tests/test_find_episodes.py
+-rw-r--r--   0 ray        (501) staff       (20)      690 2020-02-16 23:33:43.000000 media_management_scripts-0.4.3/tests/test_formatting.py
+-rw-r--r--   0 ray        (501) staff       (20)     9174 2017-10-28 16:25:41.000000 media_management_scripts-0.4.3/tests/test_metadata.py
+-rw-r--r--   0 ray        (501) staff       (20)     7095 2018-01-25 20:26:58.000000 media_management_scripts-0.4.3/tests/test_rename.py
+-rw-r--r--   0 ray        (501) staff       (20)     3930 2017-08-12 15:30:56.000000 media_management_scripts-0.4.3/tests/test_search.py
+-rw-r--r--   0 ray        (501) staff       (20)     3033 2017-08-22 14:26:44.000000 media_management_scripts-0.4.3/tests/test_search_parser.py
+-rw-r--r--   0 ray        (501) staff       (20)     7623 2020-04-25 16:09:10.000000 media_management_scripts-0.4.3/tests/test_silver_tube.py
+-rw-r--r--   0 ray        (501) staff       (20)      951 2023-04-22 15:24:11.000000 media_management_scripts-0.4.3/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `media_management_scripts-0.4.2/PKG-INFO` & `media_management_scripts-0.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,310 +1,313 @@
 Metadata-Version: 2.1
 Name: media_management_scripts
-Version: 0.4.2
+Version: 0.4.3
 Summary: Scripts for managing media
 Home-page: https://github.com/raydouglass/media_management_scripts
 Author: Ray Douglass
 Author-email: ray@raydouglass.com
 License: Apache
-Description: # Media Management Scripts
-        
-        This is a collection of command line tools for managing media files such as movies or TV shows.
-        
-        ## Installation
-        
-        Install the tools:
-        
-        `pip install media_management_scripts`
-        
-        You also need to install other programs:
-        
-        ### MacOS
-        
-        `brew install ffmpeg dialog`
-        
-        ### Ubuntu
-        
-        `apt install ffmpeg dialog`
-        
-        ### TVDB
-        
-        If you want to use TVDB for some commands, create an account on <https://www.thetvdb.com> and create API keys [here](https://www.thetvdb.com/member/api)
-        
-        Create a file `~/.config/tvdb/tvdb.ini` with contents:
-        
-        ```ini
-        [tvdb]
-        username = <your_user_name>
-        userkey = <your_user_key>
-        apikey = <your_api_key>
-        ```
-        
-        # Usage
-        
-        Pass `--help` to the subcommands for detailed help. Major features are explained in detail below.
-        
-        Most commands that rename or move files have a dry-run mode (`-n` or `--dry-run`) which will output the actions so you can verify the results.
-        
-        ## Main tools
-        __[convert](#convert)__
-        
-        __[metadata](#metadata)__
-        
-        __[rename](#rename)__
-        
-        __[search](#search)__
-        
-        __[tv-rename](#tv-rename)__
-         
-        
-        Help output
-        ```
-        usage: manage-media [-h] [-v]
-        
-        Sub commands
-            combine-subtitles   Combine a video files with subtitle file
-            combine-all         Combine a directory tree of video files with subtitle
-                                file
-            concat-mp4          Concat multiple mp4 files together
-            convert             Convert a file
-            find-episodes       Find Season/Episode/Part using file names
-            itunes              Attempts to rename iTunes episodes to the standard
-                                Plex format.
-            metadata            Show metadata for a file
-            compare             Compare metadata between files
-            compare-directory   Show metadata for a file
-            movie-rename        Renames a file based on TheMovieDB
-            rename              Renames a set of files to the specified template
-            select-streams      Extract specific streams in a video file to a new file
-            split               Split a file
-            subtitles           Convert subtitles to SRT
-            tv-rename           Renames files in a directory to sXXeYY. Can also use
-                                TVDB to name files (<show> - SxxeYY - <episode_name>)
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -v, --version         Display version
-        ```
-        
-        ## convert
-        
-        `manage-media convert <input> <output>`
-        
-        Convert a video file to different video or audio codecs. By default if no codecs are given, the file will be converted to H.264 with AAC audio.
-        
-        The source file is left intact.
-        
-        #### Examples:
-        - Convert to H.264
-            - `manage-media convert --video-codec h264 <input> <output>`
-        - Convert to HEVC/H.265:
-            - `manage-media convert --video-codec hevc <input> <output>`
-        - Convert to HEVC with AC3 audio:
-            - `manage-media convert --video-codec hevc --audio-codec ac3 <input> <output>`
-        - Convert to HEVC, but don't convert audio:
-            - `manage-media convert --vc hevc --ac copy <input> <output>`
-        - Scale to 480p
-            - `manage-media convert --scale 480`
-        - Convert to H.264 and remove interlacing (such as on mpeg2 DVDs)
-            - `manage-media convert --vc h264 --deinterlace`
-        - Convert a whole directory of files
-            - `manage-media convert --vc h264 --bulk <input dir> <output dir>`
-        
-        ## metadata
-        
-        Get a simple output of metadata for a file. Or get lots of metadata in json format
-        
-        #### Simple output
-        `manage-media metadata <input>`
-        ```
-        Battlestar Galatica (2003) - s00e01 - Battlestar Galactica The Miniseries (1).mkv
-           Directory: /Volumes/Media/TV Shows/Battlestar Galactica/Season 0/
-           Title: Battlestar Galactica: Season 1 (Disc 1)
-           Size: 6.8GB
-           Format: matroska,webm
-           Duration: 1h34m39s
-           Bitrate: 10117 Kbps
-           Video: h264 8 bit (1920x1080)
-           Audio:
-             aac (eng, 5.1)
-           Subtitles: eng, spa, fra
-           Ripped: True
-        ```
-        
-        #### Json
-        `manage-media metadata --json <input>`
-        ```json
-        {
-          "file": "/Volumes/Media/TV Shows/Battlestar Galactica/Season 0/Battlestar Galatica (2003) - s00e01 - Battlestar Galactica The Miniseries (1).mkv",
-          "title": "Battlestar Galactica: Season 1 (Disc 1)",
-          "duration": 5679.362,
-          "duration_str": "1h34m39s",
-          "size": 7354722701,
-          "size_str": "6.8GB",
-          "resolution": "HIGH_DEF",
-          "bit_rate": 10359928,
-          "bit_rate_str": "10117 Kbps",
-          "ripped": true,
-          "format": "matroska,webm",
-          "format_long_name": "Matroska / WebM",
-          "mime_type": "video/x-matroska",
-          "tags": {
-            "title": "Battlestar Galactica: Season 1 (Disc 1)",
-            "RIPPED": "true",
-            "ENCODER": "Lavf57.56.100"
-          },
-          "video_streams": [ ... ],
-          "audio_streams": [ ... ],
-          "subtitle_streams": [ ... ],
-          "other_streams": [ ... ],
-          "chapters": [ ... ],
-          "interlace": null
-        }
-        ```
-        
-        ## rename
-        
-        `manage-media rename <template> <input file>` or `manage-media rename --recursive <template> <input directory>` 
-        
-        A flexible tool to rename files
-        
-        Rename files based on a template.
-        
-        Templates can include variables or expressions by surrounding with ${...}. Functions can be called like `${upper(i)}` or `${i | upper}`.
-        
-        The following variables are available:
-          * `i`/`index` - The index of the current file being renamed
-          * `wo_ext` - The file name basename without the extension
-          * `ext` - The file extension of the current file (without '.')
-          * `filename` - The filename of the current file (basename)
-          * `re`/`regex` - A list of regex match groups (use `re[0]`, `re[1]`, etc)
-        
-        The following functions are available:
-          * `upper` - Upper cases the input
-          * `lower` - Lower cases the input
-          * `ifempty(a, b, c)` - If a is empty or null, then b, otherwise c
-          * `lpad(a, b:int)` - Left pads a to length b (defaults to 2+) with spaces
-          * `zpad(a, b:int)` - Left pads a to length b (defaults to 2+) with zeros
-        
-        `lpad`/`zpad` - By default pads to at least 2 characters. If there are 100+ files, then 3 characters, 1000+ files, then 4 characters, etc.
-        
-        Regular Expressions:
-        If a regex is included, the match groups (0=whole match, >0=match group) are available in a list 're' or 'regex'.
-        Each match group is converted to an int if possible, so a zero padded int will lose the zeros.
-        
-        Example Templates:
-        ```
-        Input: S02E04.mp4
-        Regex: S(\d+)E(\d+)
-        
-        Template: 'Season ${re[1]} Episode ${re[2]}.{ext}'
-        Result: 'Season 2 Episode 4.mp4'
-        
-        Template: 'Season ${re[1] | zpad} Episode ${zpad(re[2], 3)}.{ext}'
-        Results: 'Season 02 Episode 004.mp4'
-        ```
-        ```
-        Input: whatever.mp4
-        Regex: S(\d+)E(\d)
-        Template: 'Season ${ifempty(re[1], 'unknown', re[1])} Episode ${re[2]}.{ext}'
-        Result: 'Season unknown Episode .mp4'
-        ```
-        
-        ## search
-        
-        `manage-media search <input directory> <query>`
-        
-        Searches a directory for video files matching parameters. Note: this can take a LONG time as it has to read the metadata for each file.
-        You can speed up multiple searches in the same directory with `--db <file` which caches the metadata.
-        
-        If a video has multiple streams, comparisons mean at least one stream matches.
-        
-        Available parameters:
-        
-        Video:
-        - `v.codec` - The video codec (h264, h265, mpeg2, etc)
-        - `v.width` - The video pixel width
-        - `v.height` - The video pixel height
-        
-        Audio:
-        - `a.codec` - The audio codec (aac, ac3)
-        - `a.channels` - The number of audio channels (stereo=2, 5.1=6, etc)
-        - `a.lang` - The language of the audio track
-        
-        Subtitles:
-        - `s.codec` - The subtitle codec (srt, hdmv_pgs, mov_text, etc)
-        - `s.lang` - The language of the subtitle track
-        
-        Others:
-        - `ripped` - Whether the video is marked as ripped or not
-        - `bit_rate` - The overall average bitrate
-        - `resolution` - The resolution name (LOW_DEF, HIGH_DEF, etc)
-        
-        Metadata:
-        - `meta.xyz` - Follows the basic JSON metadata output
-        
-        Functions:
-        - `isNull(xyz)` - Returns true if the value is null
-        - `all(xyz)` - Instead of one stream matching, check all of them
-        
-        Example Queries:
-        - Find all videos that are H264
-            - `v.codec = h264`
-        - Find all videos that are H264 with stereo AAC
-            - `v.codec = h264 and a.codec = aac and a.channels = 2`
-        - Find all videos that are H265 or H264 and AAC
-            - `a.codec = aac and (v.codec = h265 or v.codec = h264)`
-            - `a.codec = aac and v.codec in [h265, h264]`
-        - Find all videos without English Subtitles
-            - `s.lang != eng`
-        - Find videos that are lower resolution than 1080
-            - `v.height < 1080`
-        - Find all videos that have ONLY AAC audio
-            - `all(a.codec) = aac`
-        
-        ## tv-rename
-        
-        Renames files in a directory to sXXeYY
-        
-        For example, if you ripped some Battlestar Galactica blurays, you might have a file structure like:
-        
-        - BSG_Season1_Disc1
-            - BSG_Season1_Disc1_t00.mkv
-            - BSG_Season1_Disc1_t01.mkv
-            - BSG_Season1_Disc1_t02.mkv
-            - BSG_Season1_Disc1_t03.mkv
-        - BSG_Season1_Disc2
-            - BSG_Season1_Disc2_t00.mkv
-            - BSG_Season1_Disc2_t01.mkv
-            - BSG_Season1_Disc2_t02.mkv
-            - BSG_Season1_Disc2_t03.mkv
-           
-        `manage-media tv-rename -s 1 -e 1 --tvdb --show "Battlestar Galactica" --output "BSG/Season 1" BSG_Season1_Disc*`
-        
-        Result
-        - BSG
-            - Season 1
-                - Battlestar Galatica (2003) - S01E01 - 33.mkv
-                - Battlestar Galatica (2003) - S01E02 - Water.mkv
-                - Battlestar Galatica (2003) - S01E03 - Bastille Day.mkv
-                - Battlestar Galatica (2003) - S01E04 - Act of Contrition.mkv
-                - Battlestar Galatica (2003) - S01E05 - You Can't Go Home Again.mkv
-                - Battlestar Galatica (2003) - S01E06 - Litmus.mkv
-                - Battlestar Galatica (2003) - S01E07 - Six Degrees of Separation.mkv
-                - Battlestar Galatica (2003) - S01E08 - Flesh and Bone.mkv
-                
-                
-        ## Configuration
-        
-        You can configuration where to find various executables by creating a file `~/.config/mms/config.ini`. By default, commands will use the executables found in your path.
-        
-        You can see which tools are being used with `manage-media `
-        
-        Config File Example
-        ```ini
-        [main]
-        ffmpeg = /path/to/ffmpeg
-        
-        ```
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Media Management Scripts
+
+This is a collection of command line tools for managing media files such as movies or TV shows.
+
+## Installation
+
+Install the tools:
+
+`pip install media_management_scripts`
+
+You also need to install other programs:
+
+### MacOS
+
+`brew install ffmpeg dialog`
+
+### Ubuntu
+
+`apt install ffmpeg dialog`
+
+### TVDB
+
+If you want to use TVDB for some commands, create an account on <https://www.thetvdb.com> and create a legacy API key [here](https://www.thetvdb.com/dashboard/account/apikey)
+
+Create a file `~/.config/tvdb/tvdb.ini` with contents:
+
+```ini
+[tvdb]
+username = <your_user_name>
+userkey = <your_user_key>
+apikey = <your_api_key>
+```
+
+# Usage
+
+Pass `--help` to the subcommands for detailed help. Major features are explained in detail below.
+
+Most commands that rename or move files have a dry-run mode (`-n` or `--dry-run`) which will output the actions so you can verify the results.
+
+## Main tools
+__[convert](#convert)__
+
+__[metadata](#metadata)__
+
+__[rename](#rename)__
+
+__[search](#search)__
+
+__[tv-rename](#tv-rename)__
+ 
+
+Help output
+```
+usage: manage-media [-h] [-v]
+
+Sub commands
+    combine-subtitles   Combine a video files with subtitle file
+    combine-all         Combine a directory tree of video files with subtitle
+                        file
+    concat-mp4          Concat multiple mp4 files together
+    convert             Convert a file
+    find-episodes       Find Season/Episode/Part using file names
+    itunes              Attempts to rename iTunes episodes to the standard
+                        Plex format.
+    metadata            Show metadata for a file
+    compare             Compare metadata between files
+    compare-directory   Show metadata for a file
+    movie-rename        Renames a file based on TheMovieDB
+    rename              Renames a set of files to the specified template
+    select-streams      Extract specific streams in a video file to a new file
+    split               Split a file
+    subtitles           Convert subtitles to SRT
+    tv-rename           Renames files in a directory to sXXeYY. Can also use
+                        TVDB to name files (<show> - SxxeYY - <episode_name>)
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         Display version
+```
+
+## convert
+
+`manage-media convert <input> <output>`
+
+Convert a video file to different video or audio codecs. By default if no codecs are given, the file will be converted to H.264 with AAC audio.
+
+The source file is left intact.
+
+#### Examples:
+- Convert to H.264
+    - `manage-media convert --video-codec h264 <input> <output>`
+- Convert to HEVC/H.265:
+    - `manage-media convert --video-codec hevc <input> <output>`
+- Convert to HEVC with AC3 audio:
+    - `manage-media convert --video-codec hevc --audio-codec ac3 <input> <output>`
+- Convert to HEVC, but don't convert audio:
+    - `manage-media convert --vc hevc --ac copy <input> <output>`
+- Scale to 480p
+    - `manage-media convert --scale 480  <input> <output>`
+- Convert to H.264 and remove interlacing (such as on mpeg2 DVDs)
+    - `manage-media convert --vc h264 --deinterlace  <input> <output>`
+- Convert a whole directory of files
+    - `manage-media convert --vc h264 --bulk <input dir> <output dir>`
+- Extract a portion of the video
+    - `manage-media convert --vc copy --ac copy --start 3m45s --end 10m00s <input> <output>`
+
+## metadata
+
+Get a simple output of metadata for a file. Or get lots of metadata in json format
+
+#### Simple output
+`manage-media metadata <input>`
+```
+Battlestar Galatica (2003) - s00e01 - Battlestar Galactica The Miniseries (1).mkv
+   Directory: /Volumes/Media/TV Shows/Battlestar Galactica/Season 0/
+   Title: Battlestar Galactica: Season 1 (Disc 1)
+   Size: 6.8GB
+   Format: matroska,webm
+   Duration: 1h34m39s
+   Bitrate: 10117 Kbps
+   Video: h264 8 bit (1920x1080)
+   Audio:
+     aac (eng, 5.1)
+   Subtitles: eng, spa, fra
+   Ripped: True
+```
+
+#### Json
+`manage-media metadata --json <input>`
+```json
+{
+  "file": "/Volumes/Media/TV Shows/Battlestar Galactica/Season 0/Battlestar Galatica (2003) - s00e01 - Battlestar Galactica The Miniseries (1).mkv",
+  "title": "Battlestar Galactica: Season 1 (Disc 1)",
+  "duration": 5679.362,
+  "duration_str": "1h34m39s",
+  "size": 7354722701,
+  "size_str": "6.8GB",
+  "resolution": "HIGH_DEF",
+  "bit_rate": 10359928,
+  "bit_rate_str": "10117 Kbps",
+  "ripped": true,
+  "format": "matroska,webm",
+  "format_long_name": "Matroska / WebM",
+  "mime_type": "video/x-matroska",
+  "tags": {
+    "title": "Battlestar Galactica: Season 1 (Disc 1)",
+    "RIPPED": "true",
+    "ENCODER": "Lavf57.56.100"
+  },
+  "video_streams": [ ... ],
+  "audio_streams": [ ... ],
+  "subtitle_streams": [ ... ],
+  "other_streams": [ ... ],
+  "chapters": [ ... ],
+  "interlace": null
+}
+```
+
+## rename
+
+`manage-media rename <template> <input file>` or `manage-media rename --recursive <template> <input directory>` 
+
+A flexible tool to rename files
+
+Rename files based on a template.
+
+Templates can include variables or expressions by surrounding with ${...}. Functions can be called like `${upper(i)}` or `${i | upper}`.
+
+The following variables are available:
+  * `i`/`index` - The index of the current file being renamed
+  * `wo_ext` - The file name basename without the extension
+  * `ext` - The file extension of the current file (without '.')
+  * `filename` - The filename of the current file (basename)
+  * `re`/`regex` - A list of regex match groups (use `re[0]`, `re[1]`, etc)
+
+The following functions are available:
+  * `upper` - Upper cases the input
+  * `lower` - Lower cases the input
+  * `ifempty(a, b, c)` - If a is empty or null, then b, otherwise c
+  * `lpad(a, b:int)` - Left pads a to length b (defaults to 2+) with spaces
+  * `zpad(a, b:int)` - Left pads a to length b (defaults to 2+) with zeros
+
+`lpad`/`zpad` - By default pads to at least 2 characters. If there are 100+ files, then 3 characters, 1000+ files, then 4 characters, etc.
+
+Regular Expressions:
+If a regex is included, the match groups (0=whole match, >0=match group) are available in a list 're' or 'regex'.
+Each match group is converted to an int if possible, so a zero padded int will lose the zeros.
+
+Example Templates:
+```
+Input: S02E04.mp4
+Regex: S(\d+)E(\d+)
+
+Template: 'Season ${re[1]} Episode ${re[2]}.{ext}'
+Result: 'Season 2 Episode 4.mp4'
+
+Template: 'Season ${re[1] | zpad} Episode ${zpad(re[2], 3)}.{ext}'
+Results: 'Season 02 Episode 004.mp4'
+```
+```
+Input: whatever.mp4
+Regex: S(\d+)E(\d)
+Template: 'Season ${ifempty(re[1], 'unknown', re[1])} Episode ${re[2]}.{ext}'
+Result: 'Season unknown Episode .mp4'
+```
+
+## search
+
+`manage-media search <input directory> <query>`
+
+Searches a directory for video files matching parameters. Note: this can take a LONG time as it has to read the metadata for each file.
+You can speed up multiple searches in the same directory with `--db <file` which caches the metadata.
+
+If a video has multiple streams, comparisons mean at least one stream matches.
+
+Available parameters:
+
+Video:
+- `v.codec` - The video codec (h264, h265, mpeg2, etc)
+- `v.width` - The video pixel width
+- `v.height` - The video pixel height
+
+Audio:
+- `a.codec` - The audio codec (aac, ac3)
+- `a.channels` - The number of audio channels (stereo=2, 5.1=6, etc)
+- `a.lang` - The language of the audio track
+
+Subtitles:
+- `s.codec` - The subtitle codec (srt, hdmv_pgs, mov_text, etc)
+- `s.lang` - The language of the subtitle track
+
+Others:
+- `ripped` - Whether the video is marked as ripped or not
+- `bit_rate` - The overall average bitrate
+- `resolution` - The resolution name (LOW_DEF, HIGH_DEF, etc)
+
+Metadata:
+- `meta.xyz` - Follows the basic JSON metadata output
+
+Functions:
+- `isNull(xyz)` - Returns true if the value is null
+- `all(xyz)` - Instead of one stream matching, check all of them
+
+Example Queries:
+- Find all videos that are H264
+    - `v.codec = h264`
+- Find all videos that are H264 with stereo AAC
+    - `v.codec = h264 and a.codec = aac and a.channels = 2`
+- Find all videos that are H265 or H264 and AAC
+    - `a.codec = aac and (v.codec = h265 or v.codec = h264)`
+    - `a.codec = aac and v.codec in [h265, h264]`
+- Find all videos without English Subtitles
+    - `s.lang != eng`
+- Find videos that are lower resolution than 1080
+    - `v.height < 1080`
+- Find all videos that have ONLY AAC audio
+    - `all(a.codec) = aac`
+
+## tv-rename
+
+Renames files in a directory to sXXeYY
+
+For example, if you ripped some Battlestar Galactica blurays, you might have a file structure like:
+
+- BSG_Season1_Disc1
+    - BSG_Season1_Disc1_t00.mkv
+    - BSG_Season1_Disc1_t01.mkv
+    - BSG_Season1_Disc1_t02.mkv
+    - BSG_Season1_Disc1_t03.mkv
+- BSG_Season1_Disc2
+    - BSG_Season1_Disc2_t00.mkv
+    - BSG_Season1_Disc2_t01.mkv
+    - BSG_Season1_Disc2_t02.mkv
+    - BSG_Season1_Disc2_t03.mkv
+   
+`manage-media tv-rename -s 1 -e 1 --tvdb --show "Battlestar Galactica" --output "BSG/Season 1" BSG_Season1_Disc*`
+
+Result
+- BSG
+    - Season 1
+        - Battlestar Galatica (2003) - S01E01 - 33.mkv
+        - Battlestar Galatica (2003) - S01E02 - Water.mkv
+        - Battlestar Galatica (2003) - S01E03 - Bastille Day.mkv
+        - Battlestar Galatica (2003) - S01E04 - Act of Contrition.mkv
+        - Battlestar Galatica (2003) - S01E05 - You Can't Go Home Again.mkv
+        - Battlestar Galatica (2003) - S01E06 - Litmus.mkv
+        - Battlestar Galatica (2003) - S01E07 - Six Degrees of Separation.mkv
+        - Battlestar Galatica (2003) - S01E08 - Flesh and Bone.mkv
+        
+        
+## Configuration
+
+You can configuration where to find various executables by creating a file `~/.config/mms/config.ini`. By default, commands will use the executables found in your path.
+
+You can see which tools are being used with `manage-media `
+
+Config File Example
+```ini
+[main]
+ffmpeg = /path/to/ffmpeg
+
+```
```

### Comparing `media_management_scripts-0.4.2/README.md` & `media_management_scripts-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ### Ubuntu
 
 `apt install ffmpeg dialog`
 
 ### TVDB
 
-If you want to use TVDB for some commands, create an account on <https://www.thetvdb.com> and create API keys [here](https://www.thetvdb.com/member/api)
+If you want to use TVDB for some commands, create an account on <https://www.thetvdb.com> and create a legacy API key [here](https://www.thetvdb.com/dashboard/account/apikey)
 
 Create a file `~/.config/tvdb/tvdb.ini` with contents:
 
 ```ini
 [tvdb]
 username = <your_user_name>
 userkey = <your_user_key>
@@ -92,19 +92,21 @@
 - Convert to HEVC/H.265:
     - `manage-media convert --video-codec hevc <input> <output>`
 - Convert to HEVC with AC3 audio:
     - `manage-media convert --video-codec hevc --audio-codec ac3 <input> <output>`
 - Convert to HEVC, but don't convert audio:
     - `manage-media convert --vc hevc --ac copy <input> <output>`
 - Scale to 480p
-    - `manage-media convert --scale 480`
+    - `manage-media convert --scale 480  <input> <output>`
 - Convert to H.264 and remove interlacing (such as on mpeg2 DVDs)
-    - `manage-media convert --vc h264 --deinterlace`
+    - `manage-media convert --vc h264 --deinterlace  <input> <output>`
 - Convert a whole directory of files
     - `manage-media convert --vc h264 --bulk <input dir> <output dir>`
+- Extract a portion of the video
+    - `manage-media convert --vc copy --ac copy --start 3m45s --end 10m00s <input> <output>`
 
 ## metadata
 
 Get a simple output of metadata for a file. Or get lots of metadata in json format
 
 #### Simple output
 `manage-media metadata <input>`
@@ -293,8 +295,8 @@
 You can see which tools are being used with `manage-media `
 
 Config File Example
 ```ini
 [main]
 ffmpeg = /path/to/ffmpeg
 
-```
+```
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/__init__.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/combine_subtitles.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/combine_subtitles.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/common.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
                                    help="Attempt to detect interlacing and remove it")
 convert_parent_parser.add_argument('--deinterlace-threshold', type=float, default=.5)
 convert_parent_parser.add_argument('--add-ripped-metadata', action='store_const', const=True, default=False,
                                    help='Adds a metadata item to the output indicating this is a ripped video',
                                    dest='include_meta')
 convert_parent_parser.add_argument('--scale', choices=[r.height for r in Resolution], type=int, default=None,
                                    help='Set the maximum height scale')
+convert_parent_parser.add_argument('--start', '-s', type=DurationType(), help='Start time of the input in 00h00m00.00s format')
+convert_parent_parser.add_argument('--end', '-e', type=DurationType(), help='End time of the input in 00h00m00.00s format')
 
 start_end_parser = argparse.ArgumentParser(add_help=False)
 start_end_parser.add_argument('--start', '-s', type=DurationType(), help='Start time of the input in 00h00m00.00s format')
 start_end_parser.add_argument('--end', '-e', type=DurationType(), help='End time of the input in 00h00m00.00s format')
 
 
 class VideoCodecAction(argparse.Action):
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/compare_directories.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/compare_directories.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/concat_mp4.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/concat_mp4.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/convert.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/convert.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from . import SubCommand
 from .common import *
 import argparse
-from media_management_scripts.support.files import get_input_output
+import os
+from media_management_scripts.support.files import get_input_output, movie_files_filter
 from media_management_scripts.convert import convert_with_config
 
 
-def _bulk_convert(i, o, config):
+def _bulk_convert(i, o, config, overwrite):
     print('Starting {}'.format(i))
-    convert_with_config(i, o, config, print_output=False)
+    os.makedirs(os.path.dirname(o), exist_ok=True)
+    convert_with_config(i, o, config, print_output=True, overwrite=overwrite)
 
 
 class ConvertCommand(SubCommand):
     @property
     def name(self):
         return 'convert'
 
@@ -38,24 +40,25 @@
                                     default=False)
 
     def subexecute(self, ns):
         import os
         from media_management_scripts.convert import convert_config_from_ns
         input_to_cmd = ns['input']
         output = ns['output']
+        overwrite = ns['overwrite']
         bulk = ns['bulk']
         config = convert_config_from_ns(ns)
 
         if os.path.isdir(input_to_cmd):
             if bulk:
                 os.makedirs(output, exist_ok=True)
-                files = list(get_input_output(input_to_cmd, output))
-                self._bulk(files, lambda i, o: _bulk_convert(i, o, config), ['Input', 'Output'])
+                files = list(get_input_output(input_to_cmd, output, filter=movie_files_filter))
+                self._bulk(files, lambda i, o: _bulk_convert(i, o, config, overwrite), ['Input', 'Output'])
             else:
                 print('Cowardly refusing to convert a direction without --bulk flag')
-        elif os.path.exists(output):
+        elif not overwrite and os.path.exists(output):
             print('Cowardly refusing to overwrite existing file: {}'.format(output))
         else:
-            convert_with_config(input_to_cmd, output, config, print_output=True)
+            convert_with_config(input_to_cmd, output, config, print_output=True, overwrite=overwrite)
 
 
 SubCommand.register(ConvertCommand)
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/executables.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/executables.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/filebot.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/filebot.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/find_episodes.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/tv_rename.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,113 @@
 from . import SubCommand
 from .common import *
 
+from media_management_scripts.tvdb_api import TVDB, get_season_episode
 
-class FindEpisodesCommand(SubCommand):
+from os.path import isfile, join, basename, dirname
+
+
+def pad(i):
+    if i < 10:
+        return '0' + str(i)
+    else:
+        return str(i)
+
+
+class TvRenameCommand(SubCommand):
     @property
     def name(self):
-        return 'find-episodes'
+        return 'tv-rename'
 
     def build_argparse(self, subparser):
-        find_episode_parser = subparser.add_parser(self.name, help='Find Season/Episode/Part using file names',
-                                                   parents=[parent_parser, input_parser])
-
-        find_episode_parser.add_argument('--strip-youtube-dl', default=True, type=bool)
-        find_episode_parser.add_argument('--concat-files', action='store_const', const=True, default=False)
-        find_episode_parser.add_argument('--output', '-o', default='./', dest='output')
-        find_episode_parser.add_argument('--seasons', action='store_const', const=True, default=False,
-                                         help='If renaming, moves files into season directories')
-        find_episode_parser.add_argument('--ignore-parts', action='store_const', const=True, default=False)
-        find_episode_parser.add_argument('--use-101-pattern', '--101', action='store_const', const=True, default=False,
-                                         help='Use a \d\d\d pattern')
-
-        group = find_episode_parser.add_mutually_exclusive_group()
-        group.add_argument('--rename', action='store_const', const=True, default=False,
-                           help='Renames the files using the season & episode if found')
-        group.add_argument('--copy', action='store_const', const=True, default=False,
-                           help='Copies the file with new name to output directory')
+        tv_rename_parser = subparser.add_parser('tv-rename',
+                                                help='Renames files in a directory to sXXeYY. Can also use TVDB to name files (<show> - SxxeYY - <episode_name>)',
+                                                parents=[parent_parser])
+        tv_rename_parser.add_argument('-s', '--season', default=1, help='The season to use', type=int)
+        tv_rename_parser.add_argument('-e', '--episode', default=1, help='The episode to start with', type=int)
+        tv_rename_parser.add_argument('--tvdb', default=False, action='store_const', const=True,
+                                      help='Use TVDB to rename episodes')
+        tv_rename_parser.add_argument('--show', default=None, help='The name of the show', type=str)
+        tv_rename_parser.add_argument('--output', default=None, help='The output directory to move & rename to',
+                                      type=str)
+        tv_rename_parser.add_argument('input', nargs='*',
+                                      help='The directories to search for files. These will be processed in order.')
 
     def subexecute(self, ns):
-        import os
-        from media_management_scripts.support.episode_finder import find_episodes
-        from media_management_scripts.utils import season_episode_name
-        from media_management_scripts.support.concat_mp4 import concat_mp4
-        from texttable import Texttable
-
-        concat = {}
-        input = ns['input']
-        do_new_name = ns.get('rename', False) or ns.get('copy', False)
-        out_dir = ns['output']
-        ignore_parts = ns['ignore_parts']
-        season_folders = ns.get('seasons', False)
-
-        table = []
-        # for ep in sorted(find_episodes(input, ns['strip_youtube_dl']), key=lambda x: (x.season, x.episode, x.part)):
-        results = list(find_episodes(input, ns['strip_youtube_dl'], ns.get('use_101_pattern')))
-        for ep in sorted(results):
-            # for ep in find_episodes(input, ns['strip_youtube_dl']):
-            if ep.part and ep.season and ep.episode and not ignore_parts:
-                key = (ep.season, ep.episode)
-                eps = concat.get(key, [])
-                eps.append(ep)
-                concat[key] = eps
-            elif do_new_name and ep.season and ep.episode:
-                path = ep.path
-                filename = os.path.basename(path)
-                name, ext = os.path.splitext(filename)
-
-                new_name = season_episode_name(ep.season, int(ep.episode), ext)
-                if season_folders:
-                    season_f = os.path.join(out_dir, 'Season {}'.format(ep.season))
-                else:
-                    season_f = out_dir
-                out_file = os.path.join(season_f, new_name)
-                table.append((ep.path, ep.season_episode, out_file))
-            elif ep.season and ep.episode:
-                table.append((ep.path, ep.season_episode, None))
+        input_to_cmd = ns['input']
+        season = ns.get('season', 1)
+        episode = ns.get('episode', 1)
+        show = ns.get('show', None)
+        output = ns.get('output', None)
+        use_tvb = ns['tvdb']
+        if use_tvb and show is None:
+            import sys
+            print('You must specify a show name if using TVDB')
+            sys.exit(1)
+
+        if use_tvb:
+            from media_management_scripts.tvdb_api import from_config
+            tvdb = from_config()
+        else:
+            tvdb = None
+
+        results = self.run(input_to_cmd, season, episode, show, output, tvdb)
+        if results:
+            self._bulk_move(results, column_descriptions=['Source', 'Destination'])
+
+    def _remove_special_characters(self, s):
+        # https://stackoverflow.com/a/31976060
+        return s.translate({ord(c): None for c in '/<>:\'"\\|?*'})
+
+    def run(self, input_dirs, season=1, episode=1, show=None, output=None, tvdb=None):
+        from os import listdir, path
+
+        files = []
+        for input_dir in input_dirs:
+            new_files = sorted(
+                [join(input_dir, f) for f in listdir(input_dir) if
+                 isfile(join(input_dir, f)) and not f.startswith('.')])
+            files.extend(new_files)
+        if tvdb:
+            shows = [(str(i), name) for i, name in tvdb.search_series(show)]
+            if len(shows) == 0:
+                print('Not search results for show \'{}\' found.'.format(show))
+                return
+            if len(shows) > 1:
+                from dialog import Dialog
+                d = Dialog(autowidgetsize=True)
+                code, tag = d.menu('Choices:', choices=shows, title='Pick a show')
+                if code != d.OK:
+                    return
+                show = next(x[1] for x in shows if x[0] == tag)
+                series_id = int(tag)
             else:
-                table.append((ep.path, None, None))
-        columns = ('Original', 'Episode', 'New Path')
-        if ns.get('rename', False):
-            self._bulk_move(table, column_descriptions=columns, src_index=0, dest_index=2, print_table=True)
-        elif ns.get('copy', False):
-            self._bulk_copy(table, column_descriptions=columns, src_index=0, dest_index=2, print_table=True)
+                series_id = int(shows[0][0])
+            episodes = tvdb.get_episodes(series_id)
+            episode_map = {get_season_episode(ep): ep for ep in episodes}
         else:
-            self._bulk_print(table, column_descriptions=columns, src_index=0, dest_index=2)
-        for key in concat:
-            concats = sorted(concat[key])
-            print('s{}e{}'.format(key[0], key[1]))
-            for item in concats:
-                print('   {} pt{}'.format(item.name, item.part))
-            if ns['concat_files']:
-                to_concat = [item.path for item in concats]
-                if len(to_concat) > 1:
-                    if season_folders:
-                        season_f = os.path.join(out_dir, 'Season {}'.format(key[0]))
-                    else:
-                        season_f = out_dir
-                    if not os.path.exists(season_f):
-                        os.makedirs(season_f)
-                    output_file = os.path.join(season_f, season_episode_name(key[0], key[1], '.mp4'))
-                    print('Concating files: {} -> {}'.format(to_concat, output_file))
-                    concat_mp4(output_file, to_concat)
+            episode_map = {}
+        results = []
+        for file in files:
+            ext = path.splitext(file)[1]
+            ep = episode_map.get((season, episode), None)
+            ep_name = ep.get('episodeName', None) if ep else None
+            if show is not None and ep is not None and ep_name is not None:
+                new_name = '{} - S{}E{} - {}{}'.format(show, pad(season), pad(episode), ep_name, ext)
+            elif show is not None:
+                new_name = '{} - S{}E{}{}'.format(show, pad(season), pad(episode), ext)
+            else:
+                new_name = 'S{}E{}{}'.format(pad(season), pad(episode), ext)
+
+            new_name = self._remove_special_characters(new_name)
+
+            if output:
+                new_name = join(output, 'Season {}'.format(pad(season)), new_name)
+            else:
+                dir = dirname(file)
+                new_name = join(dir, new_name)
+            results.append((file, new_name))
+            episode += 1
+        return results
 
 
-SubCommand.register(FindEpisodesCommand)
+SubCommand.register(TvRenameCommand)
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/itunes.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/itunes.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/metadata.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/metadata_compare.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/metadata_compare.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/movie_rename.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/movie_rename.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/rename.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/rename.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/search.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,10 +179,10 @@
                     'ripped': metadata.ripped,
                     'bit_rate': metadata.bit_rate,
                     'resolution': metadata.resolution._name_,
                     'meta': metadata.to_dict()
 
                 }
                 if query.exec(context) is True:
-                    yield file, metadata, True
+                    yield path, metadata, True
             except Exception:
-                yield file, None, False
+                yield path, None, False
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/select_streams.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/select_streams.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/split.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/split.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/subtitles.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/subtitles.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/thumbnail.py` & `media_management_scripts-0.4.3/media_management_scripts/commands/thumbnail.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/commands/tv_rename.py` & `media_management_scripts-0.4.3/media_management_scripts/support/episode_finder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,123 @@
-from . import SubCommand
-from .common import *
-
-from media_management_scripts.tvdb_api import TVDB, get_season_episode
-
-from os.path import isfile, join, basename, dirname
-
-
-def pad(i):
-    if i < 10:
-        return '0' + str(i)
-    else:
-        return str(i)
+import os
+import re
+from typing import Tuple, Iterator, Iterable
+import functools
+
+from media_management_scripts.utils import compare, season_episode_name, to_int
+from media_management_scripts.support.files import  list_files, movie_and_subtitle_files_filter
+
+patterns = [(re.compile('[Ss](\d+),?\s*[Ee](\d+)'), 1, 2),
+            (re.compile('(\d+)x(\d+)'), 1, 2),
+            (re.compile('[Ss]eries\s*(\d+).*[Ee]pisode\s*(\d+)'), 1, 2),
+            (re.compile('[Ss]eason\s*(\d+).*[Ee]pisode\s*(\d+)'), 1, 2),
+            (re.compile('[Ss]eason\s*(\d+).*[Ee]pisode.?\s*(\d+)'), 1, 2)]
+pattern_101 = re.compile('(\d)(\d\d)')
+
+part_patterns = [re.compile('[Pp]art\s*(\d+)'), re.compile('pt\s*(\d+)')]
+
+
+@functools.total_ordering
+class EpisodePart():
+    def __init__(self, name, path, season, episode, part):
+        self.name = name
+        self.path = path
+        self.season=season
+        self.episode=episode
+        self.part = part
+
+    def __str__(self):
+        if self.season is None or self.episode is None:
+            return '{}: No match'.format(self.name)
+        if self.part is not None:
+            return '{}: S{:02d}E{:02d} pt{}'.format(self.name, self.season, self.episode, self.part)
+        else:
+            return '{}: S{:02d}E{:02d}'.format(self.name, self.season, self.episode)
 
+    def __repr__(self):
+        return self.__str__()
 
-class TvRenameCommand(SubCommand):
     @property
-    def name(self):
-        return 'tv-rename'
-
-    def build_argparse(self, subparser):
-        tv_rename_parser = subparser.add_parser('tv-rename',
-                                                help='Renames files in a directory to sXXeYY. Can also use TVDB to name files (<show> - SxxeYY - <episode_name>)',
-                                                parents=[parent_parser])
-        tv_rename_parser.add_argument('-s', '--season', default=1, help='The season to use', type=int)
-        tv_rename_parser.add_argument('-e', '--episode', default=1, help='The episode to start with', type=int)
-        tv_rename_parser.add_argument('--tvdb', default=False, action='store_const', const=True,
-                                      help='Use TVDB to rename episodes')
-        tv_rename_parser.add_argument('--show', default=None, help='The name of the show', type=str)
-        tv_rename_parser.add_argument('--output', default=None, help='The output directory to move & rename to',
-                                      type=str)
-        tv_rename_parser.add_argument('input', nargs='*',
-                                      help='The directories to search for files. These will be processed in order.')
-
-    def subexecute(self, ns):
-        input_to_cmd = ns['input']
-        season = ns.get('season', 1)
-        episode = ns.get('episode', 1)
-        show = ns.get('show', None)
-        output = ns.get('output', None)
-        use_tvb = ns['tvdb']
-        if use_tvb and show is None:
-            import sys
-            print('You must specify a show name if using TVDB')
-            sys.exit(1)
-
-        if use_tvb:
-            from media_management_scripts.tvdb_api import from_config
-            tvdb = from_config()
+    def season_episode(self):
+        if self.part is not None:
+            return 'S{:02d}E{:02d} pt{}'.format(self.season, self.episode, self.part)
         else:
-            tvdb = None
+            return 'S{:02d}E{:02d}'.format(self.season, self.episode)
 
-        results = self.run(input_to_cmd, season, episode, show, output, tvdb)
-        if results:
-            self._bulk_move(results, column_descriptions=['Source', 'Destination'])
-
-    def _remove_special_characters(self, s):
-        # https://stackoverflow.com/a/31976060
-        return s.translate({ord(c): None for c in '/<>:\'"\\|?*'})
-
-    def run(self, input_dirs, season=1, episode=1, show=None, output=None, tvdb=None):
-        from os import listdir, path
-
-        files = []
-        for input_dir in input_dirs:
-            new_files = sorted(
-                [join(input_dir, f) for f in listdir(input_dir) if
-                 isfile(join(input_dir, f)) and not f.startswith('.')])
-            files.extend(new_files)
-        if tvdb:
-            shows = [(str(i), name) for i, name in tvdb.search_series(show)]
-            if len(shows) == 0:
-                print('Not search results for show \'{}\' found.'.format(show))
-                return
-            if len(shows) > 1:
-                from dialog import Dialog
-                d = Dialog(autowidgetsize=True)
-                code, tag = d.menu('Choices:', choices=shows, title='Pick a show')
-                if code != d.OK:
-                    return
-                show = next(x[1] for x in shows if x[0] == tag)
-                series_id = int(tag)
+    def __eq__(self, other):
+        if issubclass(type(other), EpisodePart):
+            return self.name == other.name and self.season == other.season \
+                   and self.episode == other.episode and self.part == other.part
+        return False
+
+    def __gt__(self, other):
+        if not issubclass(type(other), EpisodePart):
+            raise Exception()
+        cmp = compare(self.season, other.season)
+        if cmp == 0:
+            cmp = compare(self.episode, other.episode)
+        if cmp == 0:
+            cmp = compare(self.part, other.part)
+        if cmp == 0:
+            cmp = compare(self.name, other.name)
+        if cmp <= 0:
+            return True
+        return False
+
+
+def extract(name, use101=False) -> Tuple[int, int, int]:
+    season = None
+    ep = None
+    part = None
+    for pattern, season_group, episode_group in patterns:
+        m = pattern.search(name)
+        if m:
+            season = m.group(season_group)
+            ep = m.group(episode_group)
+            break
+    if season is None and ep is None and use101:
+        m = pattern_101.search(name)
+        if m:
+            season = m.group(1)
+            ep = m.group(2)
+    for pattern in part_patterns:
+        m = pattern.search(name)
+        if m:
+            part = m.group(1)
+            break
+    return to_int(season), to_int(ep), to_int(part)
+
+
+def find_episodes(dir, use101=False) -> Iterator[EpisodePart]:
+    for path in list_files(dir, movie_and_subtitle_files_filter):
+        name = os.path.basename(path)
+        name, _ = os.path.splitext(name)
+        season, ep, part = extract(name, use101)
+        path = os.path.join(dir, path)
+        yield EpisodePart(name, path, season, ep, part)
+
+def calculate_new_filenames(episodes: Iterable[EpisodePart], output_dir, use_season_folders, show_name):
+    for ep in episodes:
+        if ep.season and ep.episode:
+            path = ep.path
+            filename = os.path.basename(path)
+            name, ext = os.path.splitext(filename)
+
+            new_name = season_episode_name(ep.season, int(ep.episode), ep.name, ext)
+            if show_name:
+                new_name = "{} - {}".format(show_name, new_name)
+            if use_season_folders:
+                season_f = 'Season {:02d}'.format(ep.season)
             else:
-                series_id = int(shows[0][0])
-            episodes = tvdb.get_episodes(series_id)
-            episode_map = {get_season_episode(ep): ep for ep in episodes}
-        else:
-            episode_map = {}
-        results = []
-        for file in files:
-            ext = path.splitext(file)[1]
-            ep = episode_map.get((season, episode), None)
-            ep_name = ep.get('episodeName', None) if ep else None
-            if show is not None and ep is not None and ep_name is not None:
-                new_name = '{} - S{}E{} - {}{}'.format(show, pad(season), pad(episode), ep_name, ext)
-            elif show is not None:
-                new_name = '{} - S{}E{}{}'.format(show, pad(season), pad(episode), ext)
-            else:
-                new_name = 'S{}E{}{}'.format(pad(season), pad(episode), ext)
-
-            new_name = self._remove_special_characters(new_name)
+                season_f = None
 
-            if output:
-                new_name = join(output, 'Season {}'.format(pad(season)), new_name)
+            if show_name and season_f:
+                out_file = os.path.join(output_dir, show_name, season_f, new_name)
+            elif show_name:
+                out_file = os.path.join(output_dir, show_name, new_name)
+            elif season_f:
+                out_file = os.path.join(output_dir, season_f, new_name)
             else:
-                dir = dirname(file)
-                new_name = join(dir, new_name)
-            results.append((file, new_name))
-            episode += 1
-        return results
-
-
-SubCommand.register(TvRenameCommand)
+                out_file = os.path.join(output_dir, new_name)
+            yield ep.path, ep.season_episode, out_file
+        else:
+            yield ep.path, None, None
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/convert.py` & `media_management_scripts-0.4.3/media_management_scripts/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,23 @@
         return -2
     if use_nice and nice_exe:
         args = [nice_exe, ffmpeg()]
     else:
         args = [ffmpeg()]
     if overwrite:
         args.append('-y')
+    if config.start:
+        args.extend(['-ss', str(config.start)])
+    if config.end:
+        if config.end > 0:
+            args.extend(['-to', str(config.end)])
+        else:
+            new_end = metadata.estimated_duration+config.end
+            args.extend(['-to', str(new_end)])
+
     args.extend(['-i', input])
 
     if config.scale:
         args.extend(['-vf', 'scale=-1:{}'.format(config.scale)])
 
     args.extend(['-c:v', config.video_codec])
     crf = config.crf
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/convert_daemon.py` & `media_management_scripts-0.4.3/media_management_scripts/convert_daemon.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/main.py` & `media_management_scripts-0.4.3/media_management_scripts/main.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/renamer.py` & `media_management_scripts-0.4.3/media_management_scripts/renamer.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/silver_tube/__init__.py` & `media_management_scripts-0.4.3/media_management_scripts/silver_tube/__init__.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/silver_tube/delete_process.py` & `media_management_scripts-0.4.3/media_management_scripts/silver_tube/delete_process.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/silver_tube/processing.py` & `media_management_scripts-0.4.3/media_management_scripts/silver_tube/processing.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/silver_tube/wtv.py` & `media_management_scripts-0.4.3/media_management_scripts/silver_tube/wtv.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/silver_tube/wtv_db.py` & `media_management_scripts-0.4.3/media_management_scripts/silver_tube/wtv_db.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/combine_all.py` & `media_management_scripts-0.4.3/media_management_scripts/support/combine_all.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/concat_mp4.py` & `media_management_scripts-0.4.3/media_management_scripts/support/concat_mp4.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/encoding.py` & `media_management_scripts-0.4.3/media_management_scripts/support/encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         return Resolution.ULTRA_HIGH_DEF
 
 
 class VideoCodec(Enum):
     H264 = ('libx264', ['h264'])
     H265 = ('libx265', ['hevc', 'h265'])
     MPEG2 = ('mpeg2video', ['mpeg2video','mpeg2'])
+    COPY = ('copy', ['copy'])
 
     @property
     def ffmpeg_encoder_name(self):
         return self.value[0]
 
     @property
     def ffmpeg_codec_name(self):
@@ -96,14 +97,15 @@
         return to_comp == self.ffmpeg_encoder_name or to_comp in self.codec_names
 
 
 class AudioCodec(Enum):
     AAC = 'aac'
     AC3 = 'ac3'
     DTS = 'dts'
+    COPY = 'copy'
 
     @property
     def extension(self):
         return self.value
 
     @property
     def ffmpeg_codec_name(self):
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/executables.py` & `media_management_scripts-0.4.3/media_management_scripts/support/executables.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/files.py` & `media_management_scripts-0.4.3/media_management_scripts/support/files.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 import os
 
-from typing import Callable, Tuple, Iterator
+from typing import Callable, Tuple, Iterator, Iterable
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
 def mp4_mkv_filter(f: str) -> bool:
     return f.endswith('.mkv') or f.endswith('.mp4')
 
 
 def all_files_filter(f: str) -> bool:
     return True
 
 
-def movie_files_filter(file):
+def movie_files_filter(file) -> bool:
     return os.path.isfile(file) and \
-           (file.endswith('.mkv') or \
-            file.endswith('.mp4') or \
+           (mp4_mkv_filter(file) or \
             file.endswith('.avi') or \
             file.endswith('.m4v') or \
             file.endswith('.webm') or \
             get_mime(file).startswith('video/'))
 
+def subtitle_files_filter(file) -> bool:
+    return file.endswith('.srt') or \
+        file.endswith('.ass') or \
+        file.endswith('.ttml') or \
+        file.endswith('.vtt') or \
+        file.endswith('.xml') or \
+        file.endswith('.dfxp')
+
+def multi_files_filter(filters: Iterable[Callable[[str], bool]]) -> Callable[[str], bool]:
+    def new_filter(file):
+        for f in filters:
+            if f(file):
+                return True
+        return False
+
+    return new_filter
+
+def movie_and_subtitle_files_filter(file) -> bool:
+    return multi_files_filter([movie_files_filter, subtitle_files_filter])(file)
 
 def get_mime(file):
     import magic
     return magic.from_file(file, mime=True)
 
 
 def check_exists(output: str, log=True):
@@ -68,15 +86,15 @@
 
 
 def get_input_output(input_dir: str,
                      output_dir: str,
                      work_dir: str = None,
                      filter: Callable[[str], bool] = mp4_mkv_filter) -> Iterator[Tuple[str, ...]]:
     """
-    Mimic the file structure from input_dir into output_dir (and optionally work_dir.
+    Mimic the file structure from input_dir into output_dir (and optionally work_dir).
 
     The input files are filtered
     """
     for file in sorted(list_files(input_dir, filter)):
         input_file = os.path.join(input_dir, file)
         output_file = os.path.join(output_dir, file)
         if work_dir:
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/formatting.py` & `media_management_scripts-0.4.3/media_management_scripts/support/formatting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-DURATION_PATTERN = re.compile(r'(((\d+(\.\d+)?)h)?(\d+(\.\d+)?)m)?(\d+(\.\d+)?)s')
+DURATION_PATTERN = re.compile(r'-?(((\d+(\.\d+)?)h)?(\d+(\.\d+)?)m)?(\d+(\.\d+)?)s')
 
 def sizeof_fmt(num, suffix='B'):
     for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
         if abs(num) < 1024.0:
             return "%3.1f%s%s" % (num, unit, suffix)
         num /= 1024.0
     return "%.1f%s%s" % (num, 'Yi', suffix)
@@ -27,15 +27,18 @@
     m = DURATION_PATTERN.match(dur_str)
     if m:
         hours = m.group(3)
         minutes = m.group(5)
         seconds = m.group(7)
         hours = float(hours) * 60 * 60 if hours else 0
         minutes = float(minutes) * 60 if minutes else 0
-        return hours + minutes + float(seconds)
+        total = hours + minutes + float(seconds)
+        if dur_str.startswith('-'):
+            total*=-1
+        return total
     else:
         raise Exception('Invalid duration format: ' + dur_str)
 
 
 def bitrate_to_str(bitrate: float):
     if bitrate is None:
         return None
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/interlace.py` & `media_management_scripts-0.4.3/media_management_scripts/support/interlace.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/metadata.py` & `media_management_scripts-0.4.3/media_management_scripts/support/metadata.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/movie_rename.py` & `media_management_scripts-0.4.3/media_management_scripts/support/movie_rename.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/search_parser.py` & `media_management_scripts-0.4.3/media_management_scripts/support/search_parser.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/split.py` & `media_management_scripts-0.4.3/media_management_scripts/support/split.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/support/ttml2srt.py` & `media_management_scripts-0.4.3/media_management_scripts/support/ttml2srt.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/tvdb_api.py` & `media_management_scripts-0.4.3/media_management_scripts/tvdb_api.py`

 * *Files identical despite different names*

### Comparing `media_management_scripts-0.4.2/media_management_scripts/utils.py` & `media_management_scripts-0.4.3/media_management_scripts/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from media_management_scripts.support.encoding import DEFAULT_CRF, DEFAULT_PRESET, Resolution, VideoCodec, AudioCodec
 from media_management_scripts.support.metadata import MetadataExtractor, Metadata
 from typing import Iterable, NamedTuple
 from configparser import ConfigParser
 from media_management_scripts.support.executables import ffprobe
 
+def to_int(maybe_int) -> int:
+    if maybe_int is None:
+        return None
+    try:
+        return int(maybe_int)
+    except ValueError:
+        return None
+
 def compare_gt(this, other):
     if this is not None and other is not None:
         return int(this > other)
     elif this is not None:
         return -1
     else:
         return 1
@@ -33,21 +41,27 @@
     return MetadataExtractor({'ffprobe_exe': ffprobe()}, db_file=db_file)
 
 
 def extract_metadata(input: str, detect_interlace=False, db_file=None) -> Metadata:
     return create_metadata_extractor(db_file=db_file).extract(input, detect_interlace)
 
 
-def season_episode_name(season, episode, ext=None):
+def season_episode_name(season, episode, episode_name=None, ext=None):
     if ext:
         if not ext.startswith('.'):
             ext = '.' + ext
-        return 's{}e{:02d}{}'.format(season, int(episode), ext)
+        if episode_name:
+            return 'S{:02d}E{:02d} - {}{}'.format(int(season), int(episode), episode_name, ext)
+        else:
+            return 'S{:02d}E{:02d}{}'.format(int(season), int(episode), ext)
     else:
-        return 's{}e{:02d}'.format(season, int(episode))
+        if episode_name:
+            return 'S{:02d}E{:02d} - {}'.format(int(season), int(episode), episode_name)
+        else:
+            return 'S{:02d}E{:02d}'.format(int(season), int(episode))
 
 
 def fuzzy_equals(a: str, b: str, ignore_chars: Iterable[str] = [], ratio: float = .85) -> bool:
     from difflib import SequenceMatcher
     ifignore = (lambda x: x in ignore_chars) if ignore_chars else None
     return SequenceMatcher(ifignore, a, b).ratio() >= ratio
```

### Comparing `media_management_scripts-0.4.2/media_management_scripts.egg-info/PKG-INFO` & `media_management_scripts-0.4.3/media_management_scripts.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,310 +1,313 @@
 Metadata-Version: 2.1
 Name: media-management-scripts
-Version: 0.4.2
+Version: 0.4.3
 Summary: Scripts for managing media
 Home-page: https://github.com/raydouglass/media_management_scripts
 Author: Ray Douglass
 Author-email: ray@raydouglass.com
 License: Apache
-Description: # Media Management Scripts
-        
-        This is a collection of command line tools for managing media files such as movies or TV shows.
-        
-        ## Installation
-        
-        Install the tools:
-        
-        `pip install media_management_scripts`
-        
-        You also need to install other programs:
-        
-        ### MacOS
-        
-        `brew install ffmpeg dialog`
-        
-        ### Ubuntu
-        
-        `apt install ffmpeg dialog`
-        
-        ### TVDB
-        
-        If you want to use TVDB for some commands, create an account on <https://www.thetvdb.com> and create API keys [here](https://www.thetvdb.com/member/api)
-        
-        Create a file `~/.config/tvdb/tvdb.ini` with contents:
-        
-        ```ini
-        [tvdb]
-        username = <your_user_name>
-        userkey = <your_user_key>
-        apikey = <your_api_key>
-        ```
-        
-        # Usage
-        
-        Pass `--help` to the subcommands for detailed help. Major features are explained in detail below.
-        
-        Most commands that rename or move files have a dry-run mode (`-n` or `--dry-run`) which will output the actions so you can verify the results.
-        
-        ## Main tools
-        __[convert](#convert)__
-        
-        __[metadata](#metadata)__
-        
-        __[rename](#rename)__
-        
-        __[search](#search)__
-        
-        __[tv-rename](#tv-rename)__
-         
-        
-        Help output
-        ```
-        usage: manage-media [-h] [-v]
-        
-        Sub commands
-            combine-subtitles   Combine a video files with subtitle file
-            combine-all         Combine a directory tree of video files with subtitle
-                                file
-            concat-mp4          Concat multiple mp4 files together
-            convert             Convert a file
-            find-episodes       Find Season/Episode/Part using file names
-            itunes              Attempts to rename iTunes episodes to the standard
-                                Plex format.
-            metadata            Show metadata for a file
-            compare             Compare metadata between files
-            compare-directory   Show metadata for a file
-            movie-rename        Renames a file based on TheMovieDB
-            rename              Renames a set of files to the specified template
-            select-streams      Extract specific streams in a video file to a new file
-            split               Split a file
-            subtitles           Convert subtitles to SRT
-            tv-rename           Renames files in a directory to sXXeYY. Can also use
-                                TVDB to name files (<show> - SxxeYY - <episode_name>)
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -v, --version         Display version
-        ```
-        
-        ## convert
-        
-        `manage-media convert <input> <output>`
-        
-        Convert a video file to different video or audio codecs. By default if no codecs are given, the file will be converted to H.264 with AAC audio.
-        
-        The source file is left intact.
-        
-        #### Examples:
-        - Convert to H.264
-            - `manage-media convert --video-codec h264 <input> <output>`
-        - Convert to HEVC/H.265:
-            - `manage-media convert --video-codec hevc <input> <output>`
-        - Convert to HEVC with AC3 audio:
-            - `manage-media convert --video-codec hevc --audio-codec ac3 <input> <output>`
-        - Convert to HEVC, but don't convert audio:
-            - `manage-media convert --vc hevc --ac copy <input> <output>`
-        - Scale to 480p
-            - `manage-media convert --scale 480`
-        - Convert to H.264 and remove interlacing (such as on mpeg2 DVDs)
-            - `manage-media convert --vc h264 --deinterlace`
-        - Convert a whole directory of files
-            - `manage-media convert --vc h264 --bulk <input dir> <output dir>`
-        
-        ## metadata
-        
-        Get a simple output of metadata for a file. Or get lots of metadata in json format
-        
-        #### Simple output
-        `manage-media metadata <input>`
-        ```
-        Battlestar Galatica (2003) - s00e01 - Battlestar Galactica The Miniseries (1).mkv
-           Directory: /Volumes/Media/TV Shows/Battlestar Galactica/Season 0/
-           Title: Battlestar Galactica: Season 1 (Disc 1)
-           Size: 6.8GB
-           Format: matroska,webm
-           Duration: 1h34m39s
-           Bitrate: 10117 Kbps
-           Video: h264 8 bit (1920x1080)
-           Audio:
-             aac (eng, 5.1)
-           Subtitles: eng, spa, fra
-           Ripped: True
-        ```
-        
-        #### Json
-        `manage-media metadata --json <input>`
-        ```json
-        {
-          "file": "/Volumes/Media/TV Shows/Battlestar Galactica/Season 0/Battlestar Galatica (2003) - s00e01 - Battlestar Galactica The Miniseries (1).mkv",
-          "title": "Battlestar Galactica: Season 1 (Disc 1)",
-          "duration": 5679.362,
-          "duration_str": "1h34m39s",
-          "size": 7354722701,
-          "size_str": "6.8GB",
-          "resolution": "HIGH_DEF",
-          "bit_rate": 10359928,
-          "bit_rate_str": "10117 Kbps",
-          "ripped": true,
-          "format": "matroska,webm",
-          "format_long_name": "Matroska / WebM",
-          "mime_type": "video/x-matroska",
-          "tags": {
-            "title": "Battlestar Galactica: Season 1 (Disc 1)",
-            "RIPPED": "true",
-            "ENCODER": "Lavf57.56.100"
-          },
-          "video_streams": [ ... ],
-          "audio_streams": [ ... ],
-          "subtitle_streams": [ ... ],
-          "other_streams": [ ... ],
-          "chapters": [ ... ],
-          "interlace": null
-        }
-        ```
-        
-        ## rename
-        
-        `manage-media rename <template> <input file>` or `manage-media rename --recursive <template> <input directory>` 
-        
-        A flexible tool to rename files
-        
-        Rename files based on a template.
-        
-        Templates can include variables or expressions by surrounding with ${...}. Functions can be called like `${upper(i)}` or `${i | upper}`.
-        
-        The following variables are available:
-          * `i`/`index` - The index of the current file being renamed
-          * `wo_ext` - The file name basename without the extension
-          * `ext` - The file extension of the current file (without '.')
-          * `filename` - The filename of the current file (basename)
-          * `re`/`regex` - A list of regex match groups (use `re[0]`, `re[1]`, etc)
-        
-        The following functions are available:
-          * `upper` - Upper cases the input
-          * `lower` - Lower cases the input
-          * `ifempty(a, b, c)` - If a is empty or null, then b, otherwise c
-          * `lpad(a, b:int)` - Left pads a to length b (defaults to 2+) with spaces
-          * `zpad(a, b:int)` - Left pads a to length b (defaults to 2+) with zeros
-        
-        `lpad`/`zpad` - By default pads to at least 2 characters. If there are 100+ files, then 3 characters, 1000+ files, then 4 characters, etc.
-        
-        Regular Expressions:
-        If a regex is included, the match groups (0=whole match, >0=match group) are available in a list 're' or 'regex'.
-        Each match group is converted to an int if possible, so a zero padded int will lose the zeros.
-        
-        Example Templates:
-        ```
-        Input: S02E04.mp4
-        Regex: S(\d+)E(\d+)
-        
-        Template: 'Season ${re[1]} Episode ${re[2]}.{ext}'
-        Result: 'Season 2 Episode 4.mp4'
-        
-        Template: 'Season ${re[1] | zpad} Episode ${zpad(re[2], 3)}.{ext}'
-        Results: 'Season 02 Episode 004.mp4'
-        ```
-        ```
-        Input: whatever.mp4
-        Regex: S(\d+)E(\d)
-        Template: 'Season ${ifempty(re[1], 'unknown', re[1])} Episode ${re[2]}.{ext}'
-        Result: 'Season unknown Episode .mp4'
-        ```
-        
-        ## search
-        
-        `manage-media search <input directory> <query>`
-        
-        Searches a directory for video files matching parameters. Note: this can take a LONG time as it has to read the metadata for each file.
-        You can speed up multiple searches in the same directory with `--db <file` which caches the metadata.
-        
-        If a video has multiple streams, comparisons mean at least one stream matches.
-        
-        Available parameters:
-        
-        Video:
-        - `v.codec` - The video codec (h264, h265, mpeg2, etc)
-        - `v.width` - The video pixel width
-        - `v.height` - The video pixel height
-        
-        Audio:
-        - `a.codec` - The audio codec (aac, ac3)
-        - `a.channels` - The number of audio channels (stereo=2, 5.1=6, etc)
-        - `a.lang` - The language of the audio track
-        
-        Subtitles:
-        - `s.codec` - The subtitle codec (srt, hdmv_pgs, mov_text, etc)
-        - `s.lang` - The language of the subtitle track
-        
-        Others:
-        - `ripped` - Whether the video is marked as ripped or not
-        - `bit_rate` - The overall average bitrate
-        - `resolution` - The resolution name (LOW_DEF, HIGH_DEF, etc)
-        
-        Metadata:
-        - `meta.xyz` - Follows the basic JSON metadata output
-        
-        Functions:
-        - `isNull(xyz)` - Returns true if the value is null
-        - `all(xyz)` - Instead of one stream matching, check all of them
-        
-        Example Queries:
-        - Find all videos that are H264
-            - `v.codec = h264`
-        - Find all videos that are H264 with stereo AAC
-            - `v.codec = h264 and a.codec = aac and a.channels = 2`
-        - Find all videos that are H265 or H264 and AAC
-            - `a.codec = aac and (v.codec = h265 or v.codec = h264)`
-            - `a.codec = aac and v.codec in [h265, h264]`
-        - Find all videos without English Subtitles
-            - `s.lang != eng`
-        - Find videos that are lower resolution than 1080
-            - `v.height < 1080`
-        - Find all videos that have ONLY AAC audio
-            - `all(a.codec) = aac`
-        
-        ## tv-rename
-        
-        Renames files in a directory to sXXeYY
-        
-        For example, if you ripped some Battlestar Galactica blurays, you might have a file structure like:
-        
-        - BSG_Season1_Disc1
-            - BSG_Season1_Disc1_t00.mkv
-            - BSG_Season1_Disc1_t01.mkv
-            - BSG_Season1_Disc1_t02.mkv
-            - BSG_Season1_Disc1_t03.mkv
-        - BSG_Season1_Disc2
-            - BSG_Season1_Disc2_t00.mkv
-            - BSG_Season1_Disc2_t01.mkv
-            - BSG_Season1_Disc2_t02.mkv
-            - BSG_Season1_Disc2_t03.mkv
-           
-        `manage-media tv-rename -s 1 -e 1 --tvdb --show "Battlestar Galactica" --output "BSG/Season 1" BSG_Season1_Disc*`
-        
-        Result
-        - BSG
-            - Season 1
-                - Battlestar Galatica (2003) - S01E01 - 33.mkv
-                - Battlestar Galatica (2003) - S01E02 - Water.mkv
-                - Battlestar Galatica (2003) - S01E03 - Bastille Day.mkv
-                - Battlestar Galatica (2003) - S01E04 - Act of Contrition.mkv
-                - Battlestar Galatica (2003) - S01E05 - You Can't Go Home Again.mkv
-                - Battlestar Galatica (2003) - S01E06 - Litmus.mkv
-                - Battlestar Galatica (2003) - S01E07 - Six Degrees of Separation.mkv
-                - Battlestar Galatica (2003) - S01E08 - Flesh and Bone.mkv
-                
-                
-        ## Configuration
-        
-        You can configuration where to find various executables by creating a file `~/.config/mms/config.ini`. By default, commands will use the executables found in your path.
-        
-        You can see which tools are being used with `manage-media `
-        
-        Config File Example
-        ```ini
-        [main]
-        ffmpeg = /path/to/ffmpeg
-        
-        ```
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Media Management Scripts
+
+This is a collection of command line tools for managing media files such as movies or TV shows.
+
+## Installation
+
+Install the tools:
+
+`pip install media_management_scripts`
+
+You also need to install other programs:
+
+### MacOS
+
+`brew install ffmpeg dialog`
+
+### Ubuntu
+
+`apt install ffmpeg dialog`
+
+### TVDB
+
+If you want to use TVDB for some commands, create an account on <https://www.thetvdb.com> and create a legacy API key [here](https://www.thetvdb.com/dashboard/account/apikey)
+
+Create a file `~/.config/tvdb/tvdb.ini` with contents:
+
+```ini
+[tvdb]
+username = <your_user_name>
+userkey = <your_user_key>
+apikey = <your_api_key>
+```
+
+# Usage
+
+Pass `--help` to the subcommands for detailed help. Major features are explained in detail below.
+
+Most commands that rename or move files have a dry-run mode (`-n` or `--dry-run`) which will output the actions so you can verify the results.
+
+## Main tools
+__[convert](#convert)__
+
+__[metadata](#metadata)__
+
+__[rename](#rename)__
+
+__[search](#search)__
+
+__[tv-rename](#tv-rename)__
+ 
+
+Help output
+```
+usage: manage-media [-h] [-v]
+
+Sub commands
+    combine-subtitles   Combine a video files with subtitle file
+    combine-all         Combine a directory tree of video files with subtitle
+                        file
+    concat-mp4          Concat multiple mp4 files together
+    convert             Convert a file
+    find-episodes       Find Season/Episode/Part using file names
+    itunes              Attempts to rename iTunes episodes to the standard
+                        Plex format.
+    metadata            Show metadata for a file
+    compare             Compare metadata between files
+    compare-directory   Show metadata for a file
+    movie-rename        Renames a file based on TheMovieDB
+    rename              Renames a set of files to the specified template
+    select-streams      Extract specific streams in a video file to a new file
+    split               Split a file
+    subtitles           Convert subtitles to SRT
+    tv-rename           Renames files in a directory to sXXeYY. Can also use
+                        TVDB to name files (<show> - SxxeYY - <episode_name>)
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v, --version         Display version
+```
+
+## convert
+
+`manage-media convert <input> <output>`
+
+Convert a video file to different video or audio codecs. By default if no codecs are given, the file will be converted to H.264 with AAC audio.
+
+The source file is left intact.
+
+#### Examples:
+- Convert to H.264
+    - `manage-media convert --video-codec h264 <input> <output>`
+- Convert to HEVC/H.265:
+    - `manage-media convert --video-codec hevc <input> <output>`
+- Convert to HEVC with AC3 audio:
+    - `manage-media convert --video-codec hevc --audio-codec ac3 <input> <output>`
+- Convert to HEVC, but don't convert audio:
+    - `manage-media convert --vc hevc --ac copy <input> <output>`
+- Scale to 480p
+    - `manage-media convert --scale 480  <input> <output>`
+- Convert to H.264 and remove interlacing (such as on mpeg2 DVDs)
+    - `manage-media convert --vc h264 --deinterlace  <input> <output>`
+- Convert a whole directory of files
+    - `manage-media convert --vc h264 --bulk <input dir> <output dir>`
+- Extract a portion of the video
+    - `manage-media convert --vc copy --ac copy --start 3m45s --end 10m00s <input> <output>`
+
+## metadata
+
+Get a simple output of metadata for a file. Or get lots of metadata in json format
+
+#### Simple output
+`manage-media metadata <input>`
+```
+Battlestar Galatica (2003) - s00e01 - Battlestar Galactica The Miniseries (1).mkv
+   Directory: /Volumes/Media/TV Shows/Battlestar Galactica/Season 0/
+   Title: Battlestar Galactica: Season 1 (Disc 1)
+   Size: 6.8GB
+   Format: matroska,webm
+   Duration: 1h34m39s
+   Bitrate: 10117 Kbps
+   Video: h264 8 bit (1920x1080)
+   Audio:
+     aac (eng, 5.1)
+   Subtitles: eng, spa, fra
+   Ripped: True
+```
+
+#### Json
+`manage-media metadata --json <input>`
+```json
+{
+  "file": "/Volumes/Media/TV Shows/Battlestar Galactica/Season 0/Battlestar Galatica (2003) - s00e01 - Battlestar Galactica The Miniseries (1).mkv",
+  "title": "Battlestar Galactica: Season 1 (Disc 1)",
+  "duration": 5679.362,
+  "duration_str": "1h34m39s",
+  "size": 7354722701,
+  "size_str": "6.8GB",
+  "resolution": "HIGH_DEF",
+  "bit_rate": 10359928,
+  "bit_rate_str": "10117 Kbps",
+  "ripped": true,
+  "format": "matroska,webm",
+  "format_long_name": "Matroska / WebM",
+  "mime_type": "video/x-matroska",
+  "tags": {
+    "title": "Battlestar Galactica: Season 1 (Disc 1)",
+    "RIPPED": "true",
+    "ENCODER": "Lavf57.56.100"
+  },
+  "video_streams": [ ... ],
+  "audio_streams": [ ... ],
+  "subtitle_streams": [ ... ],
+  "other_streams": [ ... ],
+  "chapters": [ ... ],
+  "interlace": null
+}
+```
+
+## rename
+
+`manage-media rename <template> <input file>` or `manage-media rename --recursive <template> <input directory>` 
+
+A flexible tool to rename files
+
+Rename files based on a template.
+
+Templates can include variables or expressions by surrounding with ${...}. Functions can be called like `${upper(i)}` or `${i | upper}`.
+
+The following variables are available:
+  * `i`/`index` - The index of the current file being renamed
+  * `wo_ext` - The file name basename without the extension
+  * `ext` - The file extension of the current file (without '.')
+  * `filename` - The filename of the current file (basename)
+  * `re`/`regex` - A list of regex match groups (use `re[0]`, `re[1]`, etc)
+
+The following functions are available:
+  * `upper` - Upper cases the input
+  * `lower` - Lower cases the input
+  * `ifempty(a, b, c)` - If a is empty or null, then b, otherwise c
+  * `lpad(a, b:int)` - Left pads a to length b (defaults to 2+) with spaces
+  * `zpad(a, b:int)` - Left pads a to length b (defaults to 2+) with zeros
+
+`lpad`/`zpad` - By default pads to at least 2 characters. If there are 100+ files, then 3 characters, 1000+ files, then 4 characters, etc.
+
+Regular Expressions:
+If a regex is included, the match groups (0=whole match, >0=match group) are available in a list 're' or 'regex'.
+Each match group is converted to an int if possible, so a zero padded int will lose the zeros.
+
+Example Templates:
+```
+Input: S02E04.mp4
+Regex: S(\d+)E(\d+)
+
+Template: 'Season ${re[1]} Episode ${re[2]}.{ext}'
+Result: 'Season 2 Episode 4.mp4'
+
+Template: 'Season ${re[1] | zpad} Episode ${zpad(re[2], 3)}.{ext}'
+Results: 'Season 02 Episode 004.mp4'
+```
+```
+Input: whatever.mp4
+Regex: S(\d+)E(\d)
+Template: 'Season ${ifempty(re[1], 'unknown', re[1])} Episode ${re[2]}.{ext}'
+Result: 'Season unknown Episode .mp4'
+```
+
+## search
+
+`manage-media search <input directory> <query>`
+
+Searches a directory for video files matching parameters. Note: this can take a LONG time as it has to read the metadata for each file.
+You can speed up multiple searches in the same directory with `--db <file` which caches the metadata.
+
+If a video has multiple streams, comparisons mean at least one stream matches.
+
+Available parameters:
+
+Video:
+- `v.codec` - The video codec (h264, h265, mpeg2, etc)
+- `v.width` - The video pixel width
+- `v.height` - The video pixel height
+
+Audio:
+- `a.codec` - The audio codec (aac, ac3)
+- `a.channels` - The number of audio channels (stereo=2, 5.1=6, etc)
+- `a.lang` - The language of the audio track
+
+Subtitles:
+- `s.codec` - The subtitle codec (srt, hdmv_pgs, mov_text, etc)
+- `s.lang` - The language of the subtitle track
+
+Others:
+- `ripped` - Whether the video is marked as ripped or not
+- `bit_rate` - The overall average bitrate
+- `resolution` - The resolution name (LOW_DEF, HIGH_DEF, etc)
+
+Metadata:
+- `meta.xyz` - Follows the basic JSON metadata output
+
+Functions:
+- `isNull(xyz)` - Returns true if the value is null
+- `all(xyz)` - Instead of one stream matching, check all of them
+
+Example Queries:
+- Find all videos that are H264
+    - `v.codec = h264`
+- Find all videos that are H264 with stereo AAC
+    - `v.codec = h264 and a.codec = aac and a.channels = 2`
+- Find all videos that are H265 or H264 and AAC
+    - `a.codec = aac and (v.codec = h265 or v.codec = h264)`
+    - `a.codec = aac and v.codec in [h265, h264]`
+- Find all videos without English Subtitles
+    - `s.lang != eng`
+- Find videos that are lower resolution than 1080
+    - `v.height < 1080`
+- Find all videos that have ONLY AAC audio
+    - `all(a.codec) = aac`
+
+## tv-rename
+
+Renames files in a directory to sXXeYY
+
+For example, if you ripped some Battlestar Galactica blurays, you might have a file structure like:
+
+- BSG_Season1_Disc1
+    - BSG_Season1_Disc1_t00.mkv
+    - BSG_Season1_Disc1_t01.mkv
+    - BSG_Season1_Disc1_t02.mkv
+    - BSG_Season1_Disc1_t03.mkv
+- BSG_Season1_Disc2
+    - BSG_Season1_Disc2_t00.mkv
+    - BSG_Season1_Disc2_t01.mkv
+    - BSG_Season1_Disc2_t02.mkv
+    - BSG_Season1_Disc2_t03.mkv
+   
+`manage-media tv-rename -s 1 -e 1 --tvdb --show "Battlestar Galactica" --output "BSG/Season 1" BSG_Season1_Disc*`
+
+Result
+- BSG
+    - Season 1
+        - Battlestar Galatica (2003) - S01E01 - 33.mkv
+        - Battlestar Galatica (2003) - S01E02 - Water.mkv
+        - Battlestar Galatica (2003) - S01E03 - Bastille Day.mkv
+        - Battlestar Galatica (2003) - S01E04 - Act of Contrition.mkv
+        - Battlestar Galatica (2003) - S01E05 - You Can't Go Home Again.mkv
+        - Battlestar Galatica (2003) - S01E06 - Litmus.mkv
+        - Battlestar Galatica (2003) - S01E07 - Six Degrees of Separation.mkv
+        - Battlestar Galatica (2003) - S01E08 - Flesh and Bone.mkv
+        
+        
+## Configuration
+
+You can configuration where to find various executables by creating a file `~/.config/mms/config.ini`. By default, commands will use the executables found in your path.
+
+You can see which tools are being used with `manage-media `
+
+Config File Example
+```ini
+[main]
+ffmpeg = /path/to/ffmpeg
+
+```
```

### Comparing `media_management_scripts-0.4.2/setup.py` & `media_management_scripts-0.4.3/setup.py`

 * *Files identical despite different names*

