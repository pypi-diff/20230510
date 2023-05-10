# Comparing `tmp/H5Gizmos-0.1.8.tar.gz` & `tmp/H5Gizmos-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/awatters/repos/H5Gizmos/dist/tmp5pclsp07/H5Gizmos-0.1.8.tar", last modified: Wed Nov  2 13:36:53 2022, max compression
+gzip compressed data, was "H5Gizmos-0.1.9.tar", last modified: Wed Mar  1 16:28:32 2023, max compression
```

## Comparing `H5Gizmos-0.1.8.tar` & `H5Gizmos-0.1.9.tar`

### file list

```diff
@@ -1,84 +1,89 @@
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/
--rw-r--r--   0 awatters  (1035)     1035     2452 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/PKG-INFO
--rw-r--r--   0 awatters  (1035)     1035     1323 2021-08-30 14:48:21.000000 H5Gizmos-0.1.8/LICENSE
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos.egg-info/
--rw-r--r--   0 awatters  (1035)     1035     2452 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos.egg-info/PKG-INFO
--rw-r--r--   0 awatters  (1035)     1035     2519 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos.egg-info/SOURCES.txt
--rw-r--r--   0 awatters  (1035)     1035      250 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos.egg-info/entry_points.txt
--rw-r--r--   0 awatters  (1035)     1035       61 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos.egg-info/requires.txt
--rw-r--r--   0 awatters  (1035)     1035        9 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos.egg-info/top_level.txt
--rw-r--r--   0 awatters  (1035)     1035        1 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos.egg-info/dependency_links.txt
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/bin/
--rw-r--r--   0 awatters  (1035)     1035      525 2022-09-27 14:00:12.000000 H5Gizmos-0.1.8/bin/json_gizmo
--rwxr-xr-x   0 awatters  (1035)     1035      924 2022-01-14 13:41:57.000000 H5Gizmos-0.1.8/bin/gif_gizmo
--rw-r--r--   0 awatters  (1035)     1035      583 2022-09-20 14:52:47.000000 H5Gizmos-0.1.8/bin/gz_examine
--rwxr-xr-x   0 awatters  (1035)     1035      920 2022-01-14 13:43:34.000000 H5Gizmos-0.1.8/bin/snap_gizmo
--rw-r--r--   0 awatters  (1035)     1035      388 2022-06-02 14:15:56.000000 H5Gizmos-0.1.8/bin/gizmo_script
--rw-r--r--   0 awatters  (1035)     1035      317 2022-06-10 12:13:13.000000 H5Gizmos-0.1.8/bin/gizmo_link
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/python/
--rw-r--r--   0 awatters  (1035)     1035    33287 2022-11-02 13:14:00.000000 H5Gizmos-0.1.8/H5Gizmos/python/gizmo_server.py
--rw-r--r--   0 awatters  (1035)     1035    48725 2022-06-02 18:21:32.000000 H5Gizmos-0.1.8/H5Gizmos/python/H5Gizmos.py
--rw-r--r--   0 awatters  (1035)     1035    19060 2022-06-13 15:31:56.000000 H5Gizmos-0.1.8/H5Gizmos/python/gizmo_link.py
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/python/test/
--rw-r--r--   0 awatters  (1035)     1035    26562 2022-01-14 15:26:26.000000 H5Gizmos-0.1.8/H5Gizmos/python/test/test_H5Gizmos.py
--rw-r--r--   0 awatters  (1035)     1035        0 2021-10-06 14:23:57.000000 H5Gizmos-0.1.8/H5Gizmos/python/test/__init__.py
--rw-r--r--   0 awatters  (1035)     1035      560 2021-10-07 14:23:01.000000 H5Gizmos-0.1.8/H5Gizmos/python/test/test_hex_codec.py
--rw-r--r--   0 awatters  (1035)     1035     2120 2021-11-19 14:35:54.000000 H5Gizmos-0.1.8/H5Gizmos/python/test/test_gz_resources.py
--rw-r--r--   0 awatters  (1035)     1035    23437 2022-11-02 13:19:29.000000 H5Gizmos-0.1.8/H5Gizmos/python/test/test_gizmo_server.py
--rw-r--r--   0 awatters  (1035)     1035     4938 2022-05-26 16:02:09.000000 H5Gizmos-0.1.8/H5Gizmos/python/gz_get_blob.py
--rw-r--r--   0 awatters  (1035)     1035     7324 2022-06-17 18:15:47.000000 H5Gizmos-0.1.8/H5Gizmos/python/qd_file_browser.py
--rw-r--r--   0 awatters  (1035)     1035        0 2021-10-04 17:58:00.000000 H5Gizmos-0.1.8/H5Gizmos/python/__init__.py
--rw-r--r--   0 awatters  (1035)     1035     8133 2022-05-19 17:10:22.000000 H5Gizmos-0.1.8/H5Gizmos/python/gz_resources.py
--rw-r--r--   0 awatters  (1035)     1035    18265 2022-05-02 19:27:41.000000 H5Gizmos-0.1.8/H5Gizmos/python/gz_screencap.py
--rw-r--r--   0 awatters  (1035)     1035     2662 2022-06-08 18:56:02.000000 H5Gizmos-0.1.8/H5Gizmos/python/gz_tools.py
--rw-r--r--   0 awatters  (1035)     1035     8910 2022-10-05 12:37:17.000000 H5Gizmos-0.1.8/H5Gizmos/python/examine.py
--rw-r--r--   0 awatters  (1035)     1035     2656 2022-11-02 13:11:48.000000 H5Gizmos-0.1.8/H5Gizmos/python/ping_test.py
--rw-r--r--   0 awatters  (1035)     1035     4057 2022-06-13 15:33:14.000000 H5Gizmos-0.1.8/H5Gizmos/python/gizmo_script_support.py
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/python/scripts/
--rwxr-xr-x   0 awatters  (1035)     1035     3008 2022-06-02 15:36:36.000000 H5Gizmos-0.1.8/H5Gizmos/python/scripts/lorenz.py
--rw-r--r--   0 awatters  (1035)     1035       92 2022-06-02 14:19:40.000000 H5Gizmos-0.1.8/H5Gizmos/python/scripts/__init__.py
--rw-r--r--   0 awatters  (1035)     1035      555 2022-06-10 14:16:27.000000 H5Gizmos-0.1.8/H5Gizmos/python/scripts/hello_env.py
--rw-r--r--   0 awatters  (1035)     1035     2434 2022-06-21 14:02:41.000000 H5Gizmos-0.1.8/H5Gizmos/python/scripts/show_binary.py
--rw-r--r--   0 awatters  (1035)     1035    49478 2022-09-14 15:46:55.000000 H5Gizmos-0.1.8/H5Gizmos/python/gz_jQuery.py
--rw-r--r--   0 awatters  (1035)     1035      361 2021-10-05 19:49:53.000000 H5Gizmos-0.1.8/H5Gizmos/python/hex_codec.py
--rw-r--r--   0 awatters  (1035)     1035    19156 2022-06-07 18:18:42.000000 H5Gizmos-0.1.8/H5Gizmos/python/gz_components.py
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/js/
--rw-r--r--   0 awatters  (1035)     1035    39602 2022-06-16 14:28:31.000000 H5Gizmos-0.1.8/H5Gizmos/js/H5Gizmos.js
--rw-r--r--   0 awatters  (1035)     1035     9906 2022-04-01 13:01:31.000000 H5Gizmos-0.1.8/H5Gizmos/js/screen_capture_canvas.js
--rw-r--r--   0 awatters  (1035)     1035      810 2022-06-08 18:56:45.000000 H5Gizmos-0.1.8/H5Gizmos/__init__.py
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/static/
--rw-r--r--   0 awatters  (1035)     1035    21870 2021-12-09 16:49:21.000000 H5Gizmos-0.1.8/H5Gizmos/static/icon.png
--rw-r--r--   0 awatters  (1035)     1035      538 2022-01-25 20:23:42.000000 H5Gizmos-0.1.8/H5Gizmos/static/JQuery_overrides.css
--rw-r--r--   0 awatters  (1035)     1035     1158 2022-06-13 15:47:32.000000 H5Gizmos-0.1.8/H5Gizmos/static/gizmo_link_start.html
--rw-r--r--   0 awatters  (1035)     1035       75 2022-01-17 01:02:03.000000 H5Gizmos-0.1.8/H5Gizmos/static/gizmo_style.css
--rw-r--r--   0 awatters  (1035)     1035     4899 2022-06-13 19:43:17.000000 H5Gizmos-0.1.8/H5Gizmos/static/gizmo_link_support.js
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/
--rw-r--r--   0 awatters  (1035)     1035   253669 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.min.js
--rw-r--r--   0 awatters  (1035)     1035    32588 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/index.html
--rw-r--r--   0 awatters  (1035)     1035    32076 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.min.css
--rw-r--r--   0 awatters  (1035)     1035    13849 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.theme.min.css
--rw-r--r--   0 awatters  (1035)     1035    18671 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.theme.css
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/
--rw-r--r--   0 awatters  (1035)     1035     7013 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777777_256x240.png
--rw-r--r--   0 awatters  (1035)     1035     4632 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 awatters  (1035)     1035     4676 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777620_256x240.png
--rw-r--r--   0 awatters  (1035)     1035     6313 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 awatters  (1035)     1035     7074 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_555555_256x240.png
--rw-r--r--   0 awatters  (1035)     1035     7006 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_444444_256x240.png
--rw-r--r--   0 awatters  (1035)     1035    37326 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.css
--rw-r--r--   0 awatters  (1035)     1035    86709 2021-10-28 13:07:36.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery.min.js
--rw-r--r--   0 awatters  (1035)     1035     1847 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/package.json
--rw-r--r--   0 awatters  (1035)     1035    15548 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.structure.min.css
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/external/
-drwxr-xr-x   0 awatters  (1035)     1035        0 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/external/jquery/
--rw-r--r--   0 awatters  (1035)     1035   293430 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/external/jquery/jquery.js
--rw-r--r--   0 awatters  (1035)     1035    18705 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.structure.css
--rw-r--r--   0 awatters  (1035)     1035     1817 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/LICENSE.txt
--rw-r--r--   0 awatters  (1035)     1035    12660 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/AUTHORS.txt
--rw-r--r--   0 awatters  (1035)     1035   520714 2021-10-28 12:45:01.000000 H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.js
--rw-r--r--   0 awatters  (1035)     1035     1592 2022-06-07 17:30:46.000000 H5Gizmos-0.1.8/H5Gizmos/static/logo.svg
--rw-r--r--   0 awatters  (1035)     1035       37 2021-12-09 15:57:32.000000 H5Gizmos-0.1.8/MANIFEST.in
--rw-r--r--   0 awatters  (1035)     1035     2045 2022-06-21 13:40:55.000000 H5Gizmos-0.1.8/README.md
--rw-r--r--   0 awatters  (1035)     1035     1622 2022-11-02 13:34:37.000000 H5Gizmos-0.1.8/setup.py
--rw-r--r--   0 awatters  (1035)     1035       38 2022-11-02 13:36:53.000000 H5Gizmos-0.1.8/setup.cfg
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.211215 H5Gizmos-0.1.9/
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.185012 H5Gizmos-0.1.9/H5Gizmos/
+-rw-r--r--   0 awatters   (503) staff       (20)      810 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/__init__.py
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.186895 H5Gizmos-0.1.9/H5Gizmos/js/
+-rw-r--r--   0 awatters   (503) staff       (20)    41097 2023-02-03 18:52:52.000000 H5Gizmos-0.1.9/H5Gizmos/js/H5Gizmos.js
+-rw-r--r--   0 awatters   (503) staff       (20)     9960 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/js/screen_capture_canvas.js
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.191887 H5Gizmos-0.1.9/H5Gizmos/python/
+-rw-r--r--   0 awatters   (503) staff       (20)    48706 2023-01-23 20:33:00.000000 H5Gizmos-0.1.9/H5Gizmos/python/H5Gizmos.py
+-rw-r--r--   0 awatters   (503) staff       (20)        0 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/__init__.py
+-rw-r--r--   0 awatters   (503) staff       (20)     8910 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/examine.py
+-rw-r--r--   0 awatters   (503) staff       (20)     6357 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/file_selector.py
+-rw-r--r--   0 awatters   (503) staff       (20)     2993 2023-01-18 19:36:54.000000 H5Gizmos-0.1.9/H5Gizmos/python/gizmo_launch_url.py
+-rw-r--r--   0 awatters   (503) staff       (20)    19060 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/gizmo_link.py
+-rw-r--r--   0 awatters   (503) staff       (20)     4057 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/gizmo_script_support.py
+-rw-r--r--   0 awatters   (503) staff       (20)    38614 2023-03-01 14:19:40.000000 H5Gizmos-0.1.9/H5Gizmos/python/gizmo_server.py
+-rw-r--r--   0 awatters   (503) staff       (20)    21037 2023-02-03 18:51:01.000000 H5Gizmos-0.1.9/H5Gizmos/python/gz_components.py
+-rw-r--r--   0 awatters   (503) staff       (20)     4938 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/gz_get_blob.py
+-rw-r--r--   0 awatters   (503) staff       (20)    53587 2023-01-18 19:37:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/gz_jQuery.py
+-rw-r--r--   0 awatters   (503) staff       (20)     1074 2023-01-23 20:33:00.000000 H5Gizmos-0.1.9/H5Gizmos/python/gz_plotly.py
+-rw-r--r--   0 awatters   (503) staff       (20)     8160 2023-01-23 20:33:00.000000 H5Gizmos-0.1.9/H5Gizmos/python/gz_resources.py
+-rw-r--r--   0 awatters   (503) staff       (20)    18265 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/gz_screencap.py
+-rw-r--r--   0 awatters   (503) staff       (20)     2662 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/gz_tools.py
+-rw-r--r--   0 awatters   (503) staff       (20)      361 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/hex_codec.py
+-rw-r--r--   0 awatters   (503) staff       (20)     2656 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/ping_test.py
+-rw-r--r--   0 awatters   (503) staff       (20)     7324 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/qd_file_browser.py
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.192632 H5Gizmos-0.1.9/H5Gizmos/python/scripts/
+-rw-r--r--   0 awatters   (503) staff       (20)       92 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/scripts/__init__.py
+-rw-r--r--   0 awatters   (503) staff       (20)      555 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/scripts/hello_env.py
+-rwxr-xr-x   0 awatters   (503) staff       (20)     3008 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/scripts/lorenz.py
+-rw-r--r--   0 awatters   (503) staff       (20)     2559 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/scripts/show_binary.py
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.193859 H5Gizmos-0.1.9/H5Gizmos/python/test/
+-rw-r--r--   0 awatters   (503) staff       (20)        0 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/test/__init__.py
+-rw-r--r--   0 awatters   (503) staff       (20)    26562 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/test/test_H5Gizmos.py
+-rw-r--r--   0 awatters   (503) staff       (20)    23437 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/test/test_gizmo_server.py
+-rw-r--r--   0 awatters   (503) staff       (20)     2120 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/test/test_gz_resources.py
+-rw-r--r--   0 awatters   (503) staff       (20)      560 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/python/test/test_hex_codec.py
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.195361 H5Gizmos-0.1.9/H5Gizmos/static/
+-rw-r--r--   0 awatters   (503) staff       (20)      538 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/JQuery_overrides.css
+-rw-r--r--   0 awatters   (503) staff       (20)     1158 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/gizmo_link_start.html
+-rw-r--r--   0 awatters   (503) staff       (20)     4899 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/gizmo_link_support.js
+-rw-r--r--   0 awatters   (503) staff       (20)       75 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/gizmo_style.css
+-rw-r--r--   0 awatters   (503) staff       (20)    21870 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/icon.png
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.200458 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/
+-rw-r--r--   0 awatters   (503) staff       (20)    12660 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/AUTHORS.txt
+-rw-r--r--   0 awatters   (503) staff       (20)     1817 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/LICENSE.txt
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.183650 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/external/
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.200691 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/external/jquery/
+-rw-r--r--   0 awatters   (503) staff       (20)   293430 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/external/jquery/jquery.js
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.202514 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/
+-rw-r--r--   0 awatters   (503) staff       (20)     7006 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 awatters   (503) staff       (20)     7074 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 awatters   (503) staff       (20)     4676 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 awatters   (503) staff       (20)     7013 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 awatters   (503) staff       (20)     4632 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 awatters   (503) staff       (20)     6313 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 awatters   (503) staff       (20)    32588 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/index.html
+-rw-r--r--   0 awatters   (503) staff       (20)    37326 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.css
+-rw-r--r--   0 awatters   (503) staff       (20)   520714 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.js
+-rw-r--r--   0 awatters   (503) staff       (20)    32076 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.min.css
+-rw-r--r--   0 awatters   (503) staff       (20)   253669 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.min.js
+-rw-r--r--   0 awatters   (503) staff       (20)    18705 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.structure.css
+-rw-r--r--   0 awatters   (503) staff       (20)    15548 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.structure.min.css
+-rw-r--r--   0 awatters   (503) staff       (20)    18671 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.theme.css
+-rw-r--r--   0 awatters   (503) staff       (20)    13849 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.theme.min.css
+-rw-r--r--   0 awatters   (503) staff       (20)    86709 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery.min.js
+-rw-r--r--   0 awatters   (503) staff       (20)     1847 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/package.json
+-rw-r--r--   0 awatters   (503) staff       (20)     1592 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/H5Gizmos/static/logo.svg
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.202762 H5Gizmos-0.1.9/H5Gizmos/static/plotly.1.58.5/
+-rw-r--r--   0 awatters   (503) staff       (20)  7540484 2023-01-23 20:33:00.000000 H5Gizmos-0.1.9/H5Gizmos/static/plotly.1.58.5/plotly-latest.js
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.186113 H5Gizmos-0.1.9/H5Gizmos.egg-info/
+-rw-r--r--   0 awatters   (503) staff       (20)     3251 2023-03-01 16:28:32.000000 H5Gizmos-0.1.9/H5Gizmos.egg-info/PKG-INFO
+-rw-r--r--   0 awatters   (503) staff       (20)     2664 2023-03-01 16:28:32.000000 H5Gizmos-0.1.9/H5Gizmos.egg-info/SOURCES.txt
+-rw-r--r--   0 awatters   (503) staff       (20)        1 2023-03-01 16:28:32.000000 H5Gizmos-0.1.9/H5Gizmos.egg-info/dependency_links.txt
+-rw-r--r--   0 awatters   (503) staff       (20)      249 2023-03-01 16:28:32.000000 H5Gizmos-0.1.9/H5Gizmos.egg-info/entry_points.txt
+-rw-r--r--   0 awatters   (503) staff       (20)       61 2023-03-01 16:28:32.000000 H5Gizmos-0.1.9/H5Gizmos.egg-info/requires.txt
+-rw-r--r--   0 awatters   (503) staff       (20)        9 2023-03-01 16:28:32.000000 H5Gizmos-0.1.9/H5Gizmos.egg-info/top_level.txt
+-rw-r--r--   0 awatters   (503) staff       (20)     1323 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/LICENSE
+-rw-r--r--   0 awatters   (503) staff       (20)       37 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/MANIFEST.in
+-rw-r--r--   0 awatters   (503) staff       (20)     3251 2023-03-01 16:28:32.210996 H5Gizmos-0.1.9/PKG-INFO
+-rw-r--r--   0 awatters   (503) staff       (20)     2881 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/README.md
+drwxr-xr-x   0 awatters   (503) staff       (20)        0 2023-03-01 16:28:32.210700 H5Gizmos-0.1.9/bin/
+-rwxr-xr-x   0 awatters   (503) staff       (20)      924 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/bin/gif_gizmo
+-rw-r--r--   0 awatters   (503) staff       (20)      317 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/bin/gizmo_link
+-rw-r--r--   0 awatters   (503) staff       (20)      388 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/bin/gizmo_script
+-rw-r--r--   0 awatters   (503) staff       (20)      583 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/bin/gz_examine
+-rw-r--r--   0 awatters   (503) staff       (20)      525 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/bin/json_gizmo
+-rwxr-xr-x   0 awatters   (503) staff       (20)      920 2023-01-11 16:39:58.000000 H5Gizmos-0.1.9/bin/snap_gizmo
+-rw-r--r--   0 awatters   (503) staff       (20)       38 2023-03-01 16:28:32.211267 H5Gizmos-0.1.9/setup.cfg
+-rw-r--r--   0 awatters   (503) staff       (20)     1622 2023-03-01 16:23:40.000000 H5Gizmos-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `H5Gizmos-0.1.8/PKG-INFO` & `H5Gizmos-0.1.9/H5Gizmos.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: H5Gizmos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for building interactive graphical interfaces for applications using browser technology and HTML5
 Home-page: https://github.com/AaronWatters/H5Gizmos
 Author: Aaron Watters
 Author-email: awatters@flatironinstitute.org
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://github.com/AaronWatters/H5Gizmos/raw/main/doc/lorenz.gif" width="50%">
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AaronWatters/H5Gizmos/HEAD)
 
 # H5Gizmos
 
+A computer dashboard is a graphical user interface that provides real-time feedback about the state of a system or process. It is typically used in scientific and engineering applications where it is important to monitor the status of complex systems.
+
+The computer dashboard was first developed at Lawrence Livermore National Laboratory in the early 1990s. It was designed to provide immediate feedback about the performance of supercomputers, which were then used for simulations of nuclear weapons tests. The original dashboard included several hundred individual gauges that displayed various aspects of system performance.
+
+Today, computer dashboards are used in a wide variety of applications, from monitoring web servers and databases to tracking the progress of scientific experiments. They have also been adapted for use in business settings, where they can provide information about sales figures, customer satisfaction levels, and other key metrics.
+
 H5Gizmos provides
-tools for building interactive graphical interfaces for applications using browser technology and HTML5. 
+tools for building dashboards and other
+interactive graphical interfaces for applications using browser technology and HTML5. 
 
 A Gizmo "child" interface displays in a standard web browser such as Chrome and communicates
 with a "parent" Python process using a web socket and other HTTP protocols.  H5Gizmos can load and
 use arbitrary Javascript resources to provide sophisticated interactive graphical interfaces.
 
-The H5Gizmo mechanism is designed to facilitate the development of "dashboards" and special purpose
-tools for scientific and technical workflows.
-
 The animation below shows a gizmo script displaying a matplotlib plot running from the VS code editor.
 The gizmo user interface appears as a new HTML frame in the browser instance below the editor.
 
 <img src="https://github.com/AaronWatters/H5Gizmos/raw/main/doc/curves.gif" width="50%">
 
 <a href="https://github.com/AaronWatters/H5Gizmos/blob/main/doc/curves.gif">[Link to image]</a>
 
@@ -62,9 +64,7 @@
 To install an experimental version of H5Gizmos, first clone or download
 the H5Gizmos Github repository and then install in developer mode as follows:
 
 ```bash
  cd H5Gizmos
  pip install -e .
 ```
-
-
```

#### html2text {}

```diff
@@ -1,27 +1,38 @@
-Metadata-Version: 2.1 Name: H5Gizmos Version: 0.1.8 Summary: Tools for building
+Metadata-Version: 2.1 Name: H5Gizmos Version: 0.1.9 Summary: Tools for building
 interactive graphical interfaces for applications using browser technology and
 HTML5 Home-page: https://github.com/AaronWatters/H5Gizmos Author: Aaron Watters
-Author-email: awatters@flatironinstitute.org License: UNKNOWN Platform: UNKNOWN
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE [https://github.com/AaronWatters/H5Gizmos/raw/main/doc/lorenz.gif] [!
-[Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
-AaronWatters/H5Gizmos/HEAD) # H5Gizmos H5Gizmos provides tools for building
-interactive graphical interfaces for applications using browser technology and
-HTML5. A Gizmo "child" interface displays in a standard web browser such as
-Chrome and communicates with a "parent" Python process using a web socket and
-other HTTP protocols. H5Gizmos can load and use arbitrary Javascript resources
-to provide sophisticated interactive graphical interfaces. The H5Gizmo
-mechanism is designed to facilitate the development of "dashboards" and special
-purpose tools for scientific and technical workflows. The animation below shows
-a gizmo script displaying a matplotlib plot running from the VS code editor.
-The gizmo user interface appears as a new HTML frame in the browser instance
-below the editor. [https://github.com/AaronWatters/H5Gizmos/raw/main/doc/
-curves.gif] [Link_to_image] Please see the_"hello_curves"_tutorial for a
-detailed discussion of this gizmo. # Documentation The documentation for
-H5Gizmos starts at doc/README.md. The H5Gizmos documentation is provided using
-Github markdown for simplicity. If you wish to view the documentation locally
-from a clone of the repository, please use https://github.com/joeyespo/grip or
-a similar github emulator. # Installation ```bash pip install H5Gizmos ``` #
-Development (or experimental) install To install an experimental version of
-H5Gizmos, first clone or download the H5Gizmos Github repository and then
-install in developer mode as follows: ```bash cd H5Gizmos pip install -e . ```
+Author-email: awatters@flatironinstitute.org Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE [https://
+github.com/AaronWatters/H5Gizmos/raw/main/doc/lorenz.gif] [![Binder](https://
+mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AaronWatters/H5Gizmos/
+HEAD) # H5Gizmos A computer dashboard is a graphical user interface that
+provides real-time feedback about the state of a system or process. It is
+typically used in scientific and engineering applications where it is important
+to monitor the status of complex systems. The computer dashboard was first
+developed at Lawrence Livermore National Laboratory in the early 1990s. It was
+designed to provide immediate feedback about the performance of supercomputers,
+which were then used for simulations of nuclear weapons tests. The original
+dashboard included several hundred individual gauges that displayed various
+aspects of system performance. Today, computer dashboards are used in a wide
+variety of applications, from monitoring web servers and databases to tracking
+the progress of scientific experiments. They have also been adapted for use in
+business settings, where they can provide information about sales figures,
+customer satisfaction levels, and other key metrics. H5Gizmos provides tools
+for building dashboards and other interactive graphical interfaces for
+applications using browser technology and HTML5. A Gizmo "child" interface
+displays in a standard web browser such as Chrome and communicates with a
+"parent" Python process using a web socket and other HTTP protocols. H5Gizmos
+can load and use arbitrary Javascript resources to provide sophisticated
+interactive graphical interfaces. The animation below shows a gizmo script
+displaying a matplotlib plot running from the VS code editor. The gizmo user
+interface appears as a new HTML frame in the browser instance below the editor.
+[https://github.com/AaronWatters/H5Gizmos/raw/main/doc/curves.gif] [Link_to
+image] Please see the_"hello_curves"_tutorial for a detailed discussion of this
+gizmo. # Documentation The documentation for H5Gizmos starts at doc/README.md.
+The H5Gizmos documentation is provided using Github markdown for simplicity. If
+you wish to view the documentation locally from a clone of the repository,
+please use https://github.com/joeyespo/grip or a similar github emulator. #
+Installation ```bash pip install H5Gizmos ``` # Development (or experimental)
+install To install an experimental version of H5Gizmos, first clone or download
+the H5Gizmos Github repository and then install in developer mode as follows:
+```bash cd H5Gizmos pip install -e . ```
```

### Comparing `H5Gizmos-0.1.8/LICENSE` & `H5Gizmos-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos.egg-info/PKG-INFO` & `H5Gizmos-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: H5Gizmos
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for building interactive graphical interfaces for applications using browser technology and HTML5
 Home-page: https://github.com/AaronWatters/H5Gizmos
 Author: Aaron Watters
 Author-email: awatters@flatironinstitute.org
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://github.com/AaronWatters/H5Gizmos/raw/main/doc/lorenz.gif" width="50%">
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AaronWatters/H5Gizmos/HEAD)
 
 # H5Gizmos
 
+A computer dashboard is a graphical user interface that provides real-time feedback about the state of a system or process. It is typically used in scientific and engineering applications where it is important to monitor the status of complex systems.
+
+The computer dashboard was first developed at Lawrence Livermore National Laboratory in the early 1990s. It was designed to provide immediate feedback about the performance of supercomputers, which were then used for simulations of nuclear weapons tests. The original dashboard included several hundred individual gauges that displayed various aspects of system performance.
+
+Today, computer dashboards are used in a wide variety of applications, from monitoring web servers and databases to tracking the progress of scientific experiments. They have also been adapted for use in business settings, where they can provide information about sales figures, customer satisfaction levels, and other key metrics.
+
 H5Gizmos provides
-tools for building interactive graphical interfaces for applications using browser technology and HTML5. 
+tools for building dashboards and other
+interactive graphical interfaces for applications using browser technology and HTML5. 
 
 A Gizmo "child" interface displays in a standard web browser such as Chrome and communicates
 with a "parent" Python process using a web socket and other HTTP protocols.  H5Gizmos can load and
 use arbitrary Javascript resources to provide sophisticated interactive graphical interfaces.
 
-The H5Gizmo mechanism is designed to facilitate the development of "dashboards" and special purpose
-tools for scientific and technical workflows.
-
 The animation below shows a gizmo script displaying a matplotlib plot running from the VS code editor.
 The gizmo user interface appears as a new HTML frame in the browser instance below the editor.
 
 <img src="https://github.com/AaronWatters/H5Gizmos/raw/main/doc/curves.gif" width="50%">
 
 <a href="https://github.com/AaronWatters/H5Gizmos/blob/main/doc/curves.gif">[Link to image]</a>
 
@@ -62,9 +64,7 @@
 To install an experimental version of H5Gizmos, first clone or download
 the H5Gizmos Github repository and then install in developer mode as follows:
 
 ```bash
  cd H5Gizmos
  pip install -e .
 ```
-
-
```

#### html2text {}

```diff
@@ -1,27 +1,38 @@
-Metadata-Version: 2.1 Name: H5Gizmos Version: 0.1.8 Summary: Tools for building
+Metadata-Version: 2.1 Name: H5Gizmos Version: 0.1.9 Summary: Tools for building
 interactive graphical interfaces for applications using browser technology and
 HTML5 Home-page: https://github.com/AaronWatters/H5Gizmos Author: Aaron Watters
-Author-email: awatters@flatironinstitute.org License: UNKNOWN Platform: UNKNOWN
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE [https://github.com/AaronWatters/H5Gizmos/raw/main/doc/lorenz.gif] [!
-[Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
-AaronWatters/H5Gizmos/HEAD) # H5Gizmos H5Gizmos provides tools for building
-interactive graphical interfaces for applications using browser technology and
-HTML5. A Gizmo "child" interface displays in a standard web browser such as
-Chrome and communicates with a "parent" Python process using a web socket and
-other HTTP protocols. H5Gizmos can load and use arbitrary Javascript resources
-to provide sophisticated interactive graphical interfaces. The H5Gizmo
-mechanism is designed to facilitate the development of "dashboards" and special
-purpose tools for scientific and technical workflows. The animation below shows
-a gizmo script displaying a matplotlib plot running from the VS code editor.
-The gizmo user interface appears as a new HTML frame in the browser instance
-below the editor. [https://github.com/AaronWatters/H5Gizmos/raw/main/doc/
-curves.gif] [Link_to_image] Please see the_"hello_curves"_tutorial for a
-detailed discussion of this gizmo. # Documentation The documentation for
-H5Gizmos starts at doc/README.md. The H5Gizmos documentation is provided using
-Github markdown for simplicity. If you wish to view the documentation locally
-from a clone of the repository, please use https://github.com/joeyespo/grip or
-a similar github emulator. # Installation ```bash pip install H5Gizmos ``` #
-Development (or experimental) install To install an experimental version of
-H5Gizmos, first clone or download the H5Gizmos Github repository and then
-install in developer mode as follows: ```bash cd H5Gizmos pip install -e . ```
+Author-email: awatters@flatironinstitute.org Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE [https://
+github.com/AaronWatters/H5Gizmos/raw/main/doc/lorenz.gif] [![Binder](https://
+mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AaronWatters/H5Gizmos/
+HEAD) # H5Gizmos A computer dashboard is a graphical user interface that
+provides real-time feedback about the state of a system or process. It is
+typically used in scientific and engineering applications where it is important
+to monitor the status of complex systems. The computer dashboard was first
+developed at Lawrence Livermore National Laboratory in the early 1990s. It was
+designed to provide immediate feedback about the performance of supercomputers,
+which were then used for simulations of nuclear weapons tests. The original
+dashboard included several hundred individual gauges that displayed various
+aspects of system performance. Today, computer dashboards are used in a wide
+variety of applications, from monitoring web servers and databases to tracking
+the progress of scientific experiments. They have also been adapted for use in
+business settings, where they can provide information about sales figures,
+customer satisfaction levels, and other key metrics. H5Gizmos provides tools
+for building dashboards and other interactive graphical interfaces for
+applications using browser technology and HTML5. A Gizmo "child" interface
+displays in a standard web browser such as Chrome and communicates with a
+"parent" Python process using a web socket and other HTTP protocols. H5Gizmos
+can load and use arbitrary Javascript resources to provide sophisticated
+interactive graphical interfaces. The animation below shows a gizmo script
+displaying a matplotlib plot running from the VS code editor. The gizmo user
+interface appears as a new HTML frame in the browser instance below the editor.
+[https://github.com/AaronWatters/H5Gizmos/raw/main/doc/curves.gif] [Link_to
+image] Please see the_"hello_curves"_tutorial for a detailed discussion of this
+gizmo. # Documentation The documentation for H5Gizmos starts at doc/README.md.
+The H5Gizmos documentation is provided using Github markdown for simplicity. If
+you wish to view the documentation locally from a clone of the repository,
+please use https://github.com/joeyespo/grip or a similar github emulator. #
+Installation ```bash pip install H5Gizmos ``` # Development (or experimental)
+install To install an experimental version of H5Gizmos, first clone or download
+the H5Gizmos Github repository and then install in developer mode as follows:
+```bash cd H5Gizmos pip install -e . ```
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos.egg-info/SOURCES.txt` & `H5Gizmos-0.1.9/H5Gizmos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 H5Gizmos.egg-info/requires.txt
 H5Gizmos.egg-info/top_level.txt
 H5Gizmos/js/H5Gizmos.js
 H5Gizmos/js/screen_capture_canvas.js
 H5Gizmos/python/H5Gizmos.py
 H5Gizmos/python/__init__.py
 H5Gizmos/python/examine.py
+H5Gizmos/python/file_selector.py
+H5Gizmos/python/gizmo_launch_url.py
 H5Gizmos/python/gizmo_link.py
 H5Gizmos/python/gizmo_script_support.py
 H5Gizmos/python/gizmo_server.py
 H5Gizmos/python/gz_components.py
 H5Gizmos/python/gz_get_blob.py
 H5Gizmos/python/gz_jQuery.py
+H5Gizmos/python/gz_plotly.py
 H5Gizmos/python/gz_resources.py
 H5Gizmos/python/gz_screencap.py
 H5Gizmos/python/gz_tools.py
 H5Gizmos/python/hex_codec.py
 H5Gizmos/python/ping_test.py
 H5Gizmos/python/qd_file_browser.py
 H5Gizmos/python/scripts/__init__.py
@@ -57,13 +60,14 @@
 H5Gizmos/static/jquery-ui-1.12.1/external/jquery/jquery.js
 H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_444444_256x240.png
 H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_555555_256x240.png
 H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777620_256x240.png
 H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777777_256x240.png
 H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_cc0000_256x240.png
 H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_ffffff_256x240.png
+H5Gizmos/static/plotly.1.58.5/plotly-latest.js
 bin/gif_gizmo
 bin/gizmo_link
 bin/gizmo_script
 bin/gz_examine
 bin/json_gizmo
 bin/snap_gizmo
```

### Comparing `H5Gizmos-0.1.8/bin/json_gizmo` & `H5Gizmos-0.1.9/bin/json_gizmo`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/bin/gif_gizmo` & `H5Gizmos-0.1.9/bin/gif_gizmo`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/bin/gz_examine` & `H5Gizmos-0.1.9/bin/gz_examine`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/bin/snap_gizmo` & `H5Gizmos-0.1.9/bin/snap_gizmo`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gizmo_server.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gizmo_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 
 from . import H5Gizmos
 #from . import gz_resources
 
 from aiohttp import web
-#import aiohttp
+import aiohttp
 import asyncio
 #import weakref
 import mimetypes
 import os
 import sys
 import contextlib
 import socket
 #import traceback
 import sys
-from . import ping_test
+#from . import ping_test
+import time
 
 # Max size for posts -- really big
 DEFAULT_MAX_SIZE = 1000 * 1000 * 1000 * 1000 * 100
 
 # Packet chunk size limit for both GET and web socket
 DEFAULT_PACKET_SIZE = 1000 * 1000 * 10
 
 PROCESS_SHARED_GIZMO_SERVER = None
 
 # Environment variable used to construct proxied urls.
 PREFIX_ENV_VAR = "GIZMO_LINK_PREFIX"
 
+# Environment variable indicating which port to use.
+USE_PORT_ENV_VAR = "GIZMO_USE_PORT"
+
 # set/unset to enable/disable auto detection of prefix
 DETECT_PREFIX_ENV_VAR = True
 
 def get_or_create_event_loop():
     try:
         # xxxx this is deprecated in python 3.10 -- need a workaround that gets an unstarted event loop(?) or something
         loop = asyncio.get_event_loop()
@@ -90,14 +94,15 @@
         print ("System exit:")
 
 async def get_gizmo(from_server=None, verbose=False, log_messages=False, title="Gizmo"):
     """
     Get a gizmo (the official way).  Set up a server iff needed.
     """
     from_server = _check_server(from_server, verbose=verbose)
+    await from_server.check_server_name_is_reachable()
     return from_server.gizmo(log_messages=log_messages, title=title)
 
 def _check_server(server=None, verbose=False):
     "Make sure the gizmo server is set up."
     global PROCESS_SHARED_GIZMO_SERVER
     out = None  # xxxx
     err = None
@@ -115,14 +120,15 @@
         if DETECT_PREFIX_ENV_VAR:
             prefix = os.environ.get(PREFIX_ENV_VAR)
             if prefix is not None:
                 # xxxx could sanity check the prefix?
                 if verbose:
                     print("setting server prefix", [PREFIX_ENV_VAR, prefix])
                 set_url_prefix(prefix, server=server)
+        #server.check_server_name_is_reachable() -- but need to await...
     return server
 
 def set_url_prefix(proxy_prefix, server=None):
     """
     Specify the proxy prefix the server should use.
 
     This overrides localhost URLs and relative links.
@@ -150,50 +156,82 @@
 
 def get_local_ip(port=None):
     hostname = socket.gethostname()
     try:
         local_ip = socket.gethostbyname(hostname)
     except Exception:
         local_ip = socket.gethostbyname("localhost")
+    """
     try:
         if not ping_test.pingable(local_ip):
             return "localhost"
     except Exception:
         return "localhost"
     if port is not None:
         # check that we can send a message on the port
         test = ping_test.loop_test(local_ip, port)
         if not test:
             return "localhost"
+            """
     return local_ip
 
 
 def choose_port0(limit=1000):
     "old version"
     for i in range(limit):
         port = DEFAULT_PORT + i
         if not is_port_in_use(port):
             #print ("CHOSE PORT", port)
             return port
     raise ValueError("Could not find open port: " + repr(
         (DEFAULT_PORT, DEFAULT_PORT+limit)))
 
 
-def choose_port():
+def choose_port1():
     """
     Copied from repo2docker...
     Hacky method to get a free random port on local host
     """
     import socket
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     s.bind(("", 0))
     port = s.getsockname()[1]
     s.close()
     return port
 
+def choose_port(verbose=True):
+    """
+    Try to use port indicated by USE_PORT_ENV_VAR, or fall back to any free port.
+    """
+    port = None
+    port_str = os.environ.get(USE_PORT_ENV_VAR)
+    #("DEBUG:", USE_PORT_ENV_VAR, repr(port_str))
+    if port_str is not None:
+        try:
+            port_int = int(port_str)
+        except Exception as e:
+            if verbose:
+                print("Invalid port int ", USE_PORT_ENV_VAR, "value", repr(port_str))
+        else:
+            if is_port_in_use(port_int):
+                if verbose:
+                    print("Port int ", USE_PORT_ENV_VAR, "value", repr(port_str), "is not available.")
+            else:
+                port = port_int
+        if verbose and port is None:
+            print("Failed to use", USE_PORT_ENV_VAR, "value", repr(port_str), "falling back to random port.")
+        else:
+            port = port_int
+    if port is not None:
+        #("DEBUG: using specified port", port)
+        return port
+    else:
+        #("DEBUG: Using random port.")
+        return choose_port1()
+
 # use the old version:
 #choose_port = choose_port0
 
 
 def get_file_bytes(path):
     # xxxx what about binary files?
     f = open(path, "rb")
@@ -386,14 +424,32 @@
         self.stopped = False
         self.cancelled = False
         self.identifier_to_manager = {}
         #self.counter = 0
         self.out = out
         self.err = err
         self.captured_stdout = None
+        self.validator = None
+
+    async def check_server_name_is_reachable(self):
+        validator = self.validator
+        if validator is None:
+            server = self.server
+            port = self.port
+            validator = ValidateServerConnection(server, port)
+            self.validator = validator
+        await validator.future
+        if not validator.succeeded:
+            # fall back to localhost
+            #print("server", server, "is not reachable -- using localhost.")
+            self.server = "localhost"
+        else:
+            #print("server", server, "reachable")
+            pass
+        return validator.succeeded
 
     def set_url_prefix(self, url_prefix):
         self.url_prefix = url_prefix
 
     def use_local_gui(self):
         "Test whether to try to launch a web browser (gui app) using the local operating system."
         # If the url prefix is set then only launch via browser link mechanisms
@@ -501,30 +557,40 @@
                 self.port = port
             else:
                 #raise ValueError("didn't choose port???")
                 pass
             self.my_print ("runner using port", port)
             if "print" not in args:
                 args["print"] = self.my_print
+            # Start the validator (which delays immediately to permit server start)
+            #H5Gizmos.schedule_task(self.check_server_name_is_reachable())
             await async_run(app, port=port, **args)
         except asyncio.CancelledError:
             self.status = "app has been cancelled,"
             #pr(self.status)
             self.cancelled = True
         finally:
             self.status = "app has stopped."
             #pr(self.status)
             self.stopped = True
 
+    secret = bytes(str(time.time()), "utf8")
+
     def add_routes(self):
         app = self.app
         prefix = "/" + self.prefix
         app.router.add_route(GET, prefix + '/http/{tail:.*}', self.handle_http_get)
         app.router.add_route(POST, prefix + '/http/{tail:.*}', self.handle_http_post)
         app.router.add_route(GET, prefix + '/ws/{tail:.*}', self.handle_web_socket)
+        app.router.add_route(GET, "/ping", self.handle_ping)
+
+    async def handle_ping(self, request):
+        message = b'pong ' + self.secret
+        http_response = web.Response(body=message, content_type="text/plain")
+        return http_response
 
     async def handle(self, request, method="GET", interface=None):
         if interface is None:
             interface = self.interface
         #pr(" ... server handling", request.path)
         i2m = self.identifier_to_manager
         try:
@@ -899,7 +965,79 @@
         pipeline = H5Gizmos.GZPipeline(gizmo, packet_limit=packet_limit, auto_flush=auto_flush)
         self.pipeline = pipeline
         self.ws = None
 
     async def handle(self, info, request, interface):
         #print("**** pipeline handler started")
         await self.pipeline.handle_websocket_request(request)
+
+class ValidateServerConnection:
+
+    "Check that the web server '/ping' is reachable using the current port and server name."
+
+    def __init__(self, server, port, delay=0.1, wait=0.2, verbose=False):
+        self.succeeded = False
+        self.status = "initialized"
+        self.verbose = verbose
+        self.server = server
+        self.port = port
+        self.delay = delay
+        self.wait = wait
+        self.loop = get_or_create_event_loop()
+        self.future = self.loop.create_future()
+        self.task = self.loop.create_task(self.validate())
+
+    def __repr__(self) -> str:
+        return "V" + repr([self.server, self.port, self.status, self.succeeded])
+
+    async def validate(self, verbose=False):
+        from contextlib import redirect_stderr
+        import io
+        if verbose:
+            print("starting connection validation")
+        future = self.future
+        now = str(time.time())
+        server = self.server
+        port = self.port
+        url = "http://%s:%s/ping?now=%s" % (server, port, now)
+        self.my_stderr = io.StringIO()
+        with redirect_stderr(self.my_stderr):
+            try:
+                self.status = "delaying"
+                await asyncio.sleep(self.delay)  # allow time for server to start (?)
+                self.status = "preparing"
+                self.timer = self.loop.create_task(self.timeout())
+                # https://www.twilio.com/blog/asynchronous-http-requests-in-python-with-aiohttp
+                # https://docs.aiohttp.org/en/stable/client_reference.html
+                self.status = "requesting"
+                async with aiohttp.ClientSession() as client:
+                    async with client.get(url) as resp:
+                        status = resp.status
+                        bytes = await resp.read()
+                        text = bytes.decode("utf-8")
+                        self.status = "responded"
+                        future.set_result((status, text))
+                        if verbose:
+                            print("validation succeeded")
+                        self.succeeded = True
+                        self.response = resp
+            except asyncio.CancelledError:
+                if verbose:
+                    print("validation cancelled.")
+                self.status = "cancelled"
+            except Exception as e:
+                self.status = repr(e)
+                if verbose:
+                    print("validation exception", e)
+            if not future.done():
+                if verbose:
+                    print("validation defaults to fail.")
+                future.set_result(False)
+
+    async def timeout(self, verbose=False):
+        future = self.future
+        await asyncio.sleep(self.wait)
+        self.task.cancel()
+        if not future.done():
+            if verbose:
+                print("validation future timeout.")
+            future.set_result(False)
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/H5Gizmos.py` & `H5Gizmos-0.1.9/H5Gizmos/python/H5Gizmos.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 def new_identifier(prefix="Gizmo"):
     Gizmo.COUNTER += 1
     c = Gizmo.COUNTER
     t = int(time.time() * 1000)
     return "%s_%s_%s" % (prefix, t, c)
 
-FORBIDDEN_BROWSERS = ["links"]
+FORBIDDEN_BROWSERS = ["lynx"]
 
 def check_browser():
     import webbrowser
     try:
         name = webbrowser.get().name
         if name in FORBIDDEN_BROWSERS:
             raise SystemError("Cannot browse: This browser is not supported: " + repr(name))
@@ -1001,15 +1001,14 @@
         np.ndarray: np_array_translator,
         tuple: tuple_to_list
         #np.float: float,
         #np.float128: float,
         #np.float16: float,
         #np.float32: float,
         #np.float64: float,
-        #np.int: int,
         #np.int0: int,
         #np.int16: int,
         #np.int32: int,
         #np.int64: int,
     }
     for type_name in "float float128 float16 float32 float64".split():
         if hasattr(np, type_name):
@@ -1346,15 +1345,15 @@
         return task_or_none
 
     def json_error(self, msg):
         # ????
         #pr("pipeline json err", msg)
         self.last_json_error = msg
 
-class TooManyRequests(ValueError):
+class TooManyRequests(AssertionError):
     "A pipeline can only support one request."
 
 def schedule_task(awaitable):
     "Schedule a task in the global event loop."
     # Convenience
     loop = gizmo_server.get_or_create_event_loop()
     task = loop.create_task(awaitable)
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gizmo_link.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gizmo_link.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/test/test_H5Gizmos.py` & `H5Gizmos-0.1.9/H5Gizmos/python/test/test_H5Gizmos.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/test/test_hex_codec.py` & `H5Gizmos-0.1.9/H5Gizmos/python/test/test_hex_codec.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/test/test_gz_resources.py` & `H5Gizmos-0.1.9/H5Gizmos/python/test/test_gz_resources.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/test/test_gizmo_server.py` & `H5Gizmos-0.1.9/H5Gizmos/python/test/test_gizmo_server.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gz_get_blob.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gz_get_blob.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/qd_file_browser.py` & `H5Gizmos-0.1.9/H5Gizmos/python/qd_file_browser.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gz_resources.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gz_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     return result
 
 
 STD_HTML_PAGE_TEMPLATE = """
 <!DOCTYPE html>
 <html>
     <head>
+    <meta charset="UTF-8">
 {HEAD}
     </head>
 
     <body id="GIZMO_BODY" class="gizmobody">
 {BODY}
     </body>
 </html>
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gz_screencap.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gz_screencap.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gz_tools.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gz_tools.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/examine.py` & `H5Gizmos-0.1.9/H5Gizmos/python/examine.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/ping_test.py` & `H5Gizmos-0.1.9/H5Gizmos/python/ping_test.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gizmo_script_support.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gizmo_script_support.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/scripts/lorenz.py` & `H5Gizmos-0.1.9/H5Gizmos/python/scripts/lorenz.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/scripts/hello_env.py` & `H5Gizmos-0.1.9/H5Gizmos/python/scripts/hello_env.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/scripts/show_binary.py` & `H5Gizmos-0.1.9/H5Gizmos/python/scripts/show_binary.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 from H5Gizmos import Html, Stack, Shelf, Slider, Button, serve, bytearray_to_hex
-from H5Gizmos.python.qd_file_browser import FileSelector
+#from H5Gizmos.python.qd_file_browser import FileSelector
+from H5Gizmos.python.file_selector import FileSelector
+
 import os
 
 def main():
     """
     Display binary file content.
     """
     serve(task(), verbose=True)
@@ -74,11 +76,12 @@
         hex_display.text(dhex)
         repr_display.text(drepr)
     else:
         detail.text("Empty file: " + repr(path))
         hex_display.text("")
         repr_display.text("")
 
-selector = FileSelector(on_select=select_click)
+start = os.path.abspath(".")
+selector = FileSelector(on_select=select_click, root_folder="/", start_location=start)
 
 if __name__ == "__main__":
     main()
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gz_jQuery.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gz_jQuery.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #from H5Gizmos.python.gz_resources import MISC_OPERATIONS_TEMPLATE
 from . import gz_components
 from . import H5Gizmos
 from .H5Gizmos import do, get, schedule_task
 import html
 import io
 import asyncio
+import math
 
 # add Markdown(...)
 # new method jqc.append(other_jqc)
 # maybe Prints default to appending...
 
 MISC_JAVASCRIPT = """
 // miscellaneous javascript to support jQuery
@@ -60,14 +61,15 @@
         self.height = None
         self.width = None
         self.tooltips_enabled = False
         self.is_dialog = False
         self.on_click = None
         self.cached_dom_element_reference = None
         self.class_list = []
+        self.event_name_to_callback_and_depth = {}
 
     def __repr__(self):
         def truncate(x):
             if x:
                 x = str(x)
                 if len(x) > 20:
                     x = x[:20] + "..."
@@ -167,17 +169,21 @@
             do(self.element.html(self.init_text))
         if self.title_string:
             do(self.element.prop("title", self.title_string))
         if self.tooltips_enabled:
             self.enable_tooltips()
         do(self.element.appendTo(self.container))
         self.configure_jQuery_element(self.element)
+        # handle deferred event callbacks
         # Set on_click after element has been configured -- order important for Button
         if self.radio_on_click is None:
             self.set_on_click(self.on_click)
+        e2c = self.event_name_to_callback_and_depth.copy()
+        for (event_name, (callback, to_depth)) in e2c.items():
+            self.on(event_name, callback, to_depth)
         result = self.container[0]
         self.cached_dom_element_reference = result
         return result
 
     def add(self, component, title=None):
         """
         Append a JQuery component after a started gizmo.
@@ -320,14 +326,19 @@
             for css_class in classes:
                 if css_class in self.class_list:
                     self.class_list.remove(css_class)
             if self.element is not None:
                 do(self.element.removeClass(class_string))
         return self
 
+    def launcher_link(self, text, component_maker):
+        from . import gizmo_launch_url
+        launcher = gizmo_launch_url.Launcher(self, component_maker)
+        return launcher.anchor(text)
+
     def resize(self, width=None, height=None):
         """
         Set width and/or height of element.
         """
         if width is not None:
             self.width = width
         if height is not None:
@@ -339,20 +350,26 @@
             if height is not None:
                 do(self.element.height(height))
                 do(self.container.height(height))
         return self
 
     def on(self, event_name, callback, to_depth=1):
         "When an event of this type happens to this object, invoke the callback."
-        do(self.element.on(event_name, callback), to_depth=to_depth)
+        self.event_name_to_callback_and_depth[event_name] = (callback, to_depth)
+        if self.element is not None:
+            do(self.element.on(event_name, callback), to_depth=to_depth)
         return self
 
     def off(self, event_name):
         "Cancel event callbacks of this type for this object."
-        do(self.element.off(event_name))
+        e2c = self.event_name_to_callback_and_depth
+        if event_name in e2c:
+            del e2c[event_name]
+        if self.element is not None:
+            do(self.element.off(event_name))
         return self
 
     def empty(self):
         "Remove all content from this element."
         do(self.element.empty())
         return self
 
@@ -362,18 +379,19 @@
         return self
 
 class jQueryButton(jQueryComponent):
 
     options = None  # default
     on_click = None
     
-    def __init__(self, init_text, tag="<button/>", on_click=None, options=None, title=None):
+    def __init__(self, init_text, tag="<button/>", on_click=None, options=None, title=None, enabled=None):
         super().__init__(init_text, tag, title=title)
         self.options = options
         self.on_click = on_click
+        self.enable_override = enabled # None to ignore, else True or False
 
     widget_name = "button"
     on_click_depth = 1
 
     def configure_jQuery_element(self, element):
         options = self.options
         initializer = element[self.widget_name]
@@ -385,22 +403,45 @@
 
     def set_on_click(self, on_click):
         self.on_click = on_click
         if self.element is None:
             return  self # not yet configured.
         if on_click is not None:
             do(self.element.on("click", on_click), to_depth=self.on_click_depth)
+        else:
+            do(self.element.off("click"))
+        enable = (on_click is not None)
+        if self.enable_override is not None:
+            enable = self.enable_override
+        if enable:
             do(self.element.prop("disabled", False))
             do(self.element.css("opacity", 1.0))
         else:
             do(self.element.off("click"))
             do(self.element.prop("disabled", True))
             do(self.element.css("opacity", 0.5))
         return self
 
+    def set_enabled(self, value=True):
+        if self.element is None:
+            # not displayed
+            self.enable_override = value
+            return
+        # otherwise
+        do(self.element.prop("disabled", not value))
+        if value:
+            do(self.element.css("opacity", 1.0))
+            on_click = self.on_click
+            if on_click is not None:
+                do(self.element.off("click"))
+                do(self.element.on("click", on_click), to_depth=self.on_click_depth)
+        else:
+            do(self.element.css("opacity", 0.5))
+            do(self.element.off("click"))
+
 class RadioButtons(jQueryComponent):
 
     # based on https://api.jqueryui.com/checkboxradio/
 
     input_type = "radio"
 
     def __init__(
@@ -1217,45 +1258,100 @@
     # quick and dirty for now
     version = 0
 
     def __init__(
         self, 
         filename=None,   # filename of None generates a fresh "don't care" name.
         bytes_content=None, 
+        array=None,
         height=None, 
         width=None, 
         mime_type=None, 
         alt="image",
         title=None,
         ):
+        assert array is None or bytes_content is None, (
+            "ambiguous content -- both array and bytes provided."
+        )
         if filename is None:
             filename = H5Gizmos.new_identifier("jQueryImage")
         if mime_type is None and bytes_content is None:
             mime_type = "img/png"
             bytes_content = SMALL_PNG_BYTES
         self.filename = filename
         self.alt = alt
         self.tag = '<img src="%s" alt="%s"/>' % (self.versioned_link(), self.alt)
         super().__init__(None, self.tag, title=title)
         self.bytes_content = bytes_content
         self.height = height
         self.width = width
+        self.img_height = self.img_width = self.array = None
+        if array is not None:
+            self.array = array
+            (self.img_height, self.img_width) = array.shape[:2]
+            if height is None:
+                self.height = self.img_height
+            if width is None:
+                self.width = self.img_width
+        self.pixel_click_callback = None
         self.content_type = mime_type
 
+    def on_pixel(self, callback, type="click"):
+        """
+        When the image is clicked call the callback with the pixel_row, pixel_column coordinates added
+        and also the pixel_data, the array entry value at array[row, column]
+        This only works if the image is populated using an array at present.
+        """
+        self.pixel_click_callback = callback
+        self.on(type, self._pixel_callback)
+
+    def _pixel_callback(self, event):
+        assert self.img_height is not None and self.img_width is not None, (
+            "Cannot determine pixel coordinates from non-array data."
+        )
+        cb = self.pixel_click_callback
+        assert cb is not None, "No pixel click callback defined."
+        # https://stackoverflow.com/questions/56451370/how-to-get-pixel-number-from-image-by-click
+        offsetX = event["offsetX"]
+        offsetY = event["offsetY"]
+        iw = self.img_width
+        ih = self.img_height
+        ratioX = iw / self.width
+        ratioY = ih / self.height
+        pixel_i = math.floor(offsetX * ratioX)
+        pixel_j = math.floor(offsetY * ratioY)
+        if pixel_i >= iw:
+            pixel_i = iw-1
+        if pixel_j >= ih:
+            pixel_j = ih - 1
+        event["pixel_column"] = pixel_i
+        event["pixel_row"] = pixel_j
+        if self.array is not None:
+            pixel_data = self.array[pixel_j, pixel_i]
+            event["pixel_data"] = pixel_data
+        return cb(event)
+
     def change_content(self, bytes_content, mime_type=None):
         self.bytes_content = bytes(bytes_content)
         self.getter.set_content(bytes_content, mime_type)
         do(self.element.attr("src", self.versioned_link()))
+        self.img_height = self.img_width = self.array = None
 
     def change_content_url(self, bytes_content, mime_type):
         url = content_url(bytes_content, mime_type)
         do(self.element.attr("src", url))
+        self.img_height = self.img_width = self.array = None
 
     def change_array(self, array, url=True, scale=False, epsilon=1e-12):
         from PIL import Image
+        if self.element is None:
+            # not displayed -- defer.
+            (self.img_height, self.img_width) = array.shape[:2]
+            self.array = array
+            return
         m = array.min()
         M = array.max()
         if scale:
             if (M - m) > epsilon:
                 A = array.astype(np.float)
                 scaled = 255 * (A - m) / (M - m)
                 array = scaled.astype(np.uint8)
@@ -1270,26 +1366,30 @@
         im.save(f, format="PNG")
         byt = f.getvalue()
         mime_type = "img/png"
         if url:
             self.change_content_url(byt, mime_type)
         else:
             self.change_content(byt, mime_type)
+        (self.img_height, self.img_width) = array.shape[:2]
+        self.array = array
 
     def versioned_link(self):
         self.version += 1   # use versioning to foil browser caching.
         return "%s?v=%s" % (self.filename, self.version)
 
     def configure_jQuery_element(self, element):
         gizmo = self.gizmo
         mgr = gizmo._manager
         self.getter = gizmo_server.BytesGetter(self.filename, self.bytes_content, mgr, self.content_type)
         #mgr.add_http_handler(self.filename, self.getter)
         gizmo._add_getter(self.filename, self.getter)
         self.resize(height=self.height, width=self.width)
+        if self.array is not None:
+            self.change_array(self.array)
 
 def content_url(bytes_content, mime_type):
     import base64
     prefix = 'data:%s;base64,' % mime_type
     b64 = base64.b64encode(bytes_content)
     url = prefix + b64.decode("utf8")
     return url
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos/python/gz_components.py` & `H5Gizmos-0.1.9/H5Gizmos/python/gz_components.py`

 * *Files 12% similar despite different names*

```diff
@@ -284,14 +284,15 @@
 
     def dom_element_reference(self, gizmo):
         """
         initialize and return a reference to the DOM element for this component.
         """
         self.gizmo = gizmo
         self.initialize_object_cache()
+        self.window = gizmo.window # define the window shortcut
         return "Undefined gizmo component."  # override return value in subclass.
 
     def initialize_object_cache(self):
         gizmo = self.gizmo
         cache_name = self.cache_name
         if cache_name is None:
             cache_name = self.cache_name = (self.cache_name or self.get_cache_name())
@@ -435,14 +436,70 @@
             data = await postback.wait_for_post(timeout=timeout, on_timeout=self.on_timeout)
         finally:
             gizmo._remove_getter(endpoint)
         (body, query) = data
         data_bytes = bytearray(body)
         return np.frombuffer(data_bytes, dtype=dtype)
 
+    async def get_webgl_image_array(
+        self,
+        context_reference,
+        x=None, 
+        y=None, 
+        w=None, 
+        h=None,
+        timeout=60,
+    ):
+        gizmo = self.gizmo
+        postback = gz_get_blob.BytesPostBack()
+        endpoint = H5Gizmos.new_identifier("webgl_image_endpoint")
+        gizmo._add_getter(endpoint, postback)
+        try:
+            do(gizmo.H5Gizmos.post_webgl_canvas_image(
+                endpoint,
+                context_reference,
+                x, y, w, h))
+            data = await postback.wait_for_post(timeout=timeout, on_timeout=self.on_timeout)
+        finally:
+            gizmo._remove_getter(endpoint)
+        return self.array_from_canvas_data(data)
+
+    async def get_canvas_image_array(
+        self, 
+        canvas_reference,
+        x=None, 
+        y=None, 
+        w=None, 
+        h=None,
+        context_reference=None,
+        timeout=60):
+        gizmo = self.gizmo
+        postback = gz_get_blob.BytesPostBack()
+        endpoint = H5Gizmos.new_identifier("canvas_image_endpoint")
+        gizmo._add_getter(endpoint, postback)
+        try:
+            do(gizmo.H5Gizmos.post_2d_canvas_image(
+                endpoint, 
+                canvas_reference, 
+                context_reference,
+                x, y, w, h))
+            data = await postback.wait_for_post(timeout=timeout, on_timeout=self.on_timeout)
+        finally:
+            gizmo._remove_getter(endpoint)
+        return self.array_from_canvas_data(data)
+
+    def array_from_canvas_data(self, data):
+        (body, query) = data
+        data_bytes = bytearray(body)
+        byte_array = np.frombuffer(data_bytes, dtype=np.uint8)
+        height = query["height"]
+        width = query["width"]
+        result = byte_array.reshape((height, width, 4))
+        return result
+
     def on_timeout(self, *ignored):
         raise TimeoutError("Operation timed out")
 
     def shutdown_parent_only(self, *args):
         import sys
         print("shutting down.")
         sys.exit()
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos/js/H5Gizmos.js` & `H5Gizmos-0.1.9/H5Gizmos/js/H5Gizmos.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -107,15 +107,15 @@
                 throw new Error("Web socket error on halted gizmo.")
             }
             var cb = this.ws_error_message_callback;
             if (cb) {
                 var message = "Web socket error."
                 var ws = this.ws;
                 if ((ws) && (ws.readyState != ws_open)) {
-                    message = "Web socket connection is not open. " + ws.readyState;
+                    message = "Web socket connection is not open. Is this a duplicate connection?" + ws.readyState;
                 }
                 cb(message)
             }
         }
         get_ws_url(location) {
             location = location || window.location;
             var path_split = location.pathname.split("/");
@@ -1057,14 +1057,52 @@
                 parent.postMessage(message, "*");
                 setTimeout(send_height_to_parent, delay);
             }
             setTimeout(send_height_to_parent, delay);
         }
     };
 
+    H5Gizmos.post_2d_canvas_image = function(
+        end_point, dom_canvas, context2d, x, y, w, h, gizmo_translator) {
+        // Send the image data from the canvas to the parent in a POST request
+        context2d = context2d || dom_canvas.getContext("2d");
+        x = x || 0;
+        y = y || 0;
+        w = w || dom_canvas.width;
+        h = h || dom_canvas.height;
+        // default to global interface
+        gizmo_translator = gizmo_translator || H5GIZMO_INTERFACE;
+        var image_data = context2d.getImageData(x, y, w, h);
+        var json_metadata = {
+            height: image_data.height,
+            width: image_data.width
+        };
+        gizmo_translator.post_binary_data(end_point, image_data.data, json_metadata);
+    };
+
+    H5Gizmos.post_webgl_canvas_image = function(
+        end_point, gl_context, x, y, w, h, gizmo_translator) {
+        debugger;
+        var gl = gl_context;
+        x = x || 0;
+        y = y || 0;
+        w = w || (gl.drawingBufferWidth - x);
+        h = h || (gl.drawingBufferHeight - y);
+        // default to global interface
+        gizmo_translator = gizmo_translator || H5GIZMO_INTERFACE;
+        // https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/readPixels
+        const pixels = new Uint8Array(w * h * 4);
+        gl.readPixels(x, y, w, h, gl.RGBA, gl.UNSIGNED_BYTE, pixels);
+        var json_metadata = {
+            height: h,
+            width: w
+        };
+        gizmo_translator.post_binary_data(end_point, pixels, json_metadata);
+    };
+
     H5Gizmos.is_loaded = true;
 
 })(); // execute initialization in protected scope.
 
 try {
     if (module !== undefined) {
         // For node/jest.
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos/js/screen_capture_canvas.js` & `H5Gizmos-0.1.9/H5Gizmos/js/screen_capture_canvas.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6,31 +6,29 @@
 Based on
 https://developer.mozilla.org/en-US/docs/Web/API/Screen_Capture_API/Using_Screen_Capture
 
 */
 
 (function() {
 
+    /* moved to H5Gizmos.js as generally useful
     H5Gizmos.post_2d_canvas_image = function(end_point, dom_canvas, context2d, x, y, w, h, gizmo_translator) {
         // Send the image data from the canvas to the parent in a POST request
         context2d = context2d || dom_canvas.getContext("2d");
         x = x || 0;
         y = y || 0;
         w = w || canvas.width;
         h = h || canvas.height;
         // default to global interface
         gizmo_translator = gizmo_translator || H5GIZMO_INTERFACE;
         var image_data = context2d.getImageData(x, y, w, h);
-        var json_metadata = {
-            height: image_data.height,
-            width: image_data.width
-        };
+        var json_metadata = {height: image_data.height, width: image_data.width};
         gizmo_translator.post_binary_data(end_point, image_data.data, json_metadata);
     };
-
+    */
 
     // XXXX NOTE: This screen capture method only seems to work in recent versions of Chrome (not Firefox, Safari...)
     class ScreenCapture extends H5Gizmos.DeferredValue {
         constructor(element, size_callback, snap_callback, connect_media_now) {
             //console.log("size callback", size_callback)
             super();
             //debugger;
```

### Comparing `H5Gizmos-0.1.8/H5Gizmos/__init__.py` & `H5Gizmos-0.1.9/H5Gizmos/__init__.py`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/icon.png` & `H5Gizmos-0.1.9/H5Gizmos/static/icon.png`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/JQuery_overrides.css` & `H5Gizmos-0.1.9/H5Gizmos/static/JQuery_overrides.css`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/gizmo_link_start.html` & `H5Gizmos-0.1.9/H5Gizmos/static/gizmo_link_start.html`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/gizmo_link_support.js` & `H5Gizmos-0.1.9/H5Gizmos/static/gizmo_link_support.js`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.min.js` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/index.html` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/index.html`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.min.css` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.theme.min.css` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.theme.css` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777777_256x240.png` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_cc0000_256x240.png` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777620_256x240.png` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_ffffff_256x240.png` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_555555_256x240.png` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_444444_256x240.png` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.css` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery.min.js` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/package.json` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/package.json`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.structure.min.css` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/external/jquery/jquery.js` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.structure.css` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/LICENSE.txt` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/AUTHORS.txt` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.js` & `H5Gizmos-0.1.9/H5Gizmos/static/jquery-ui-1.12.1/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/H5Gizmos/static/logo.svg` & `H5Gizmos-0.1.9/H5Gizmos/static/logo.svg`

 * *Files identical despite different names*

### Comparing `H5Gizmos-0.1.8/README.md` & `H5Gizmos-0.1.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 <img src="https://github.com/AaronWatters/H5Gizmos/raw/main/doc/lorenz.gif" width="50%">
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AaronWatters/H5Gizmos/HEAD)
 
 # H5Gizmos
 
+A computer dashboard is a graphical user interface that provides real-time feedback about the state of a system or process. It is typically used in scientific and engineering applications where it is important to monitor the status of complex systems.
+
+The computer dashboard was first developed at Lawrence Livermore National Laboratory in the early 1990s. It was designed to provide immediate feedback about the performance of supercomputers, which were then used for simulations of nuclear weapons tests. The original dashboard included several hundred individual gauges that displayed various aspects of system performance.
+
+Today, computer dashboards are used in a wide variety of applications, from monitoring web servers and databases to tracking the progress of scientific experiments. They have also been adapted for use in business settings, where they can provide information about sales figures, customer satisfaction levels, and other key metrics.
+
 H5Gizmos provides
-tools for building interactive graphical interfaces for applications using browser technology and HTML5. 
+tools for building dashboards and other
+interactive graphical interfaces for applications using browser technology and HTML5. 
 
 A Gizmo "child" interface displays in a standard web browser such as Chrome and communicates
 with a "parent" Python process using a web socket and other HTTP protocols.  H5Gizmos can load and
 use arbitrary Javascript resources to provide sophisticated interactive graphical interfaces.
 
-The H5Gizmo mechanism is designed to facilitate the development of "dashboards" and special purpose
-tools for scientific and technical workflows.
-
 The animation below shows a gizmo script displaying a matplotlib plot running from the VS code editor.
 The gizmo user interface appears as a new HTML frame in the browser instance below the editor.
 
 <img src="https://github.com/AaronWatters/H5Gizmos/raw/main/doc/curves.gif" width="50%">
 
 <a href="https://github.com/AaronWatters/H5Gizmos/blob/main/doc/curves.gif">[Link to image]</a>
```

#### html2text {}

```diff
@@ -1,22 +1,33 @@
 [https://github.com/AaronWatters/H5Gizmos/raw/main/doc/lorenz.gif] [![Binder]
 (https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/AaronWatters/
-H5Gizmos/HEAD) # H5Gizmos H5Gizmos provides tools for building interactive
-graphical interfaces for applications using browser technology and HTML5. A
-Gizmo "child" interface displays in a standard web browser such as Chrome and
-communicates with a "parent" Python process using a web socket and other HTTP
-protocols. H5Gizmos can load and use arbitrary Javascript resources to provide
-sophisticated interactive graphical interfaces. The H5Gizmo mechanism is
-designed to facilitate the development of "dashboards" and special purpose
-tools for scientific and technical workflows. The animation below shows a gizmo
-script displaying a matplotlib plot running from the VS code editor. The gizmo
-user interface appears as a new HTML frame in the browser instance below the
-editor. [https://github.com/AaronWatters/H5Gizmos/raw/main/doc/curves.gif]
-[Link_to_image] Please see the_"hello_curves"_tutorial for a detailed
-discussion of this gizmo. # Documentation The documentation for H5Gizmos starts
-at doc/README.md. The H5Gizmos documentation is provided using Github markdown
-for simplicity. If you wish to view the documentation locally from a clone of
-the repository, please use https://github.com/joeyespo/grip or a similar github
-emulator. # Installation ```bash pip install H5Gizmos ``` # Development (or
-experimental) install To install an experimental version of H5Gizmos, first
-clone or download the H5Gizmos Github repository and then install in developer
-mode as follows: ```bash cd H5Gizmos pip install -e . ```
+H5Gizmos/HEAD) # H5Gizmos A computer dashboard is a graphical user interface
+that provides real-time feedback about the state of a system or process. It is
+typically used in scientific and engineering applications where it is important
+to monitor the status of complex systems. The computer dashboard was first
+developed at Lawrence Livermore National Laboratory in the early 1990s. It was
+designed to provide immediate feedback about the performance of supercomputers,
+which were then used for simulations of nuclear weapons tests. The original
+dashboard included several hundred individual gauges that displayed various
+aspects of system performance. Today, computer dashboards are used in a wide
+variety of applications, from monitoring web servers and databases to tracking
+the progress of scientific experiments. They have also been adapted for use in
+business settings, where they can provide information about sales figures,
+customer satisfaction levels, and other key metrics. H5Gizmos provides tools
+for building dashboards and other interactive graphical interfaces for
+applications using browser technology and HTML5. A Gizmo "child" interface
+displays in a standard web browser such as Chrome and communicates with a
+"parent" Python process using a web socket and other HTTP protocols. H5Gizmos
+can load and use arbitrary Javascript resources to provide sophisticated
+interactive graphical interfaces. The animation below shows a gizmo script
+displaying a matplotlib plot running from the VS code editor. The gizmo user
+interface appears as a new HTML frame in the browser instance below the editor.
+[https://github.com/AaronWatters/H5Gizmos/raw/main/doc/curves.gif] [Link_to
+image] Please see the_"hello_curves"_tutorial for a detailed discussion of this
+gizmo. # Documentation The documentation for H5Gizmos starts at doc/README.md.
+The H5Gizmos documentation is provided using Github markdown for simplicity. If
+you wish to view the documentation locally from a clone of the repository,
+please use https://github.com/joeyespo/grip or a similar github emulator. #
+Installation ```bash pip install H5Gizmos ``` # Development (or experimental)
+install To install an experimental version of H5Gizmos, first clone or download
+the H5Gizmos Github repository and then install in developer mode as follows:
+```bash cd H5Gizmos pip install -e . ```
```

### Comparing `H5Gizmos-0.1.8/setup.py` & `H5Gizmos-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 url = "https://github.com/AaronWatters/H5Gizmos"
-version = "0.1.8"
+version = "0.1.9"
 readme = open('README.md').read()
 
 setup(
     name="H5Gizmos",
     packages=[
         "H5Gizmos", 
         "H5Gizmos.python",
```

