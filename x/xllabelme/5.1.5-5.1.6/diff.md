# Comparing `tmp/xllabelme-5.1.5.tar.gz` & `tmp/xllabelme-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xllabelme-5.1.5.tar", last modified: Thu Apr 20 12:48:18 2023, max compression
+gzip compressed data, was "xllabelme-5.1.6.tar", last modified: Wed May 10 14:46:58 2023, max compression
```

## Comparing `xllabelme-5.1.5.tar` & `xllabelme-5.1.6.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.285127 xllabelme-5.1.5/
--rw-rw-rw-   0        0        0      707 2020-11-09 02:22:17.000000 xllabelme-5.1.5/LICENSE
--rw-rw-rw-   0        0        0       19 2020-08-05 08:41:43.000000 xllabelme-5.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0    11738 2023-04-20 12:48:18.285127 xllabelme-5.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     9202 2022-04-20 05:38:39.000000 xllabelme-5.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.212321 xllabelme-5.1.5/docs/
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.217308 xllabelme-5.1.5/docs/man/
--rw-rw-rw-   0        0        0     2148 2020-08-05 08:41:43.000000 xllabelme-5.1.5/docs/man/labelme.1
--rw-rw-rw-   0        0        0       42 2023-04-20 12:48:18.286124 xllabelme-5.1.5/setup.cfg
--rw-rw-rw-   0        0        0     5290 2023-04-20 12:13:49.000000 xllabelme-5.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.224289 xllabelme-5.1.5/xllabelme/
--rw-rw-rw-   0        0        0     1074 2023-04-20 12:48:16.000000 xllabelme-5.1.5/xllabelme/__init__.py
--rw-rw-rw-   0        0        0     7602 2023-04-18 02:03:52.000000 xllabelme-5.1.5/xllabelme/__main__.py
--rw-rw-rw-   0        0        0    78564 2023-04-20 11:53:57.000000 xllabelme-5.1.5/xllabelme/app.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.232268 xllabelme-5.1.5/xllabelme/cli/
--rw-rw-rw-   0        0        0      129 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/cli/__init__.py
--rw-rw-rw-   0        0        0     1404 2022-04-20 05:42:00.000000 xllabelme-5.1.5/xllabelme/cli/draw_json.py
--rw-rw-rw-   0        0        0      667 2021-06-08 03:21:06.000000 xllabelme-5.1.5/xllabelme/cli/draw_label_png.py
--rw-rw-rw-   0        0        0     2473 2022-04-20 05:42:14.000000 xllabelme-5.1.5/xllabelme/cli/json_to_dataset.py
--rw-rw-rw-   0        0        0     2851 2022-04-20 05:42:22.000000 xllabelme-5.1.5/xllabelme/cli/on_docker.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.234263 xllabelme-5.1.5/xllabelme/config/
--rw-rw-rw-   0        0        0     2784 2021-06-08 03:21:07.000000 xllabelme-5.1.5/xllabelme/config/__init__.py
--rw-rw-rw-   0        0        0     2340 2023-04-16 08:40:27.000000 xllabelme-5.1.5/xllabelme/config/default_config.yaml
--rw-rw-rw-   0        0        0    54316 2023-04-20 11:30:13.000000 xllabelme-5.1.5/xllabelme/config/xllabellib.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.272162 xllabelme-5.1.5/xllabelme/icons/
--rw-rw-rw-   0        0        0     2136 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/cancel.png
--rw-rw-rw-   0        0        0     3111 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/close.png
--rw-rw-rw-   0        0        0     2368 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/color-line.png
--rw-rw-rw-   0        0        0     1461 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/color.png
--rw-rw-rw-   0        0        0      646 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/copy.png
--rw-rw-rw-   0        0        0     1486 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/delete.png
--rw-rw-rw-   0        0        0     2198 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/done.png
--rw-rw-rw-   0        0        0    22632 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/done.svg
--rw-rw-rw-   0        0        0     1092 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/edit.png
--rw-rw-rw-   0        0        0     7718 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/expert.png
--rw-rw-rw-   0        0        0     1264 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/eye.png
--rw-rw-rw-   0        0        0     8059 2019-01-15 04:29:26.000000 xllabelme-5.1.5/xllabelme/icons/feBlend-icon.png
--rw-rw-rw-   0        0        0      765 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/file.png
--rw-rw-rw-   0        0        0     1365 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/fit-width.png
--rw-rw-rw-   0        0        0     1102 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/fit-window.png
--rw-rw-rw-   0        0        0     2262 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/fit.png
--rw-rw-rw-   0        0        0     1587 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/help.png
--rw-rw-rw-   0        0        0   183198 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/icon.ico
--rw-rw-rw-   0        0        0    44771 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/icon.png
--rw-rw-rw-   0        0        0    38362 2023-04-04 10:35:02.000000 xllabelme-5.1.5/xllabelme/icons/icon2.ico
--rw-rw-rw-   0        0        0    34213 2023-04-04 10:24:55.000000 xllabelme-5.1.5/xllabelme/icons/icon2.png
--rw-rw-rw-   0        0        0     2381 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/labels.png
--rw-rw-rw-   0        0        0    37512 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/labels.svg
--rw-rw-rw-   0        0        0      977 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/new.png
--rw-rw-rw-   0        0        0    30288 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/next.png
--rw-rw-rw-   0        0        0     1103 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/objects.png
--rw-rw-rw-   0        0        0     2073 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/open.png
--rw-rw-rw-   0        0        0    18773 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/open.svg
--rw-rw-rw-   0        0        0    30665 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/prev.png
--rw-rw-rw-   0        0        0     1915 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/quit.png
--rw-rw-rw-   0        0        0     2811 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/save-as.png
--rw-rw-rw-   0        0        0    65363 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/save-as.svg
--rw-rw-rw-   0        0        0     1187 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/save.png
--rw-rw-rw-   0        0        0    31292 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/save.svg
--rw-rw-rw-   0        0        0     2004 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/undo-cross.png
--rw-rw-rw-   0        0        0     2018 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/undo.png
--rw-rw-rw-   0        0        0     1099 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/zoom-in.png
--rw-rw-rw-   0        0        0     1074 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/zoom-out.png
--rw-rw-rw-   0        0        0     1139 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/icons/zoom.png
--rw-rw-rw-   0        0        0     7120 2023-04-20 09:45:20.000000 xllabelme-5.1.5/xllabelme/label_file.py
--rw-rw-rw-   0        0        0     1907 2023-03-31 08:56:10.000000 xllabelme-5.1.5/xllabelme/logger.py
--rw-rw-rw-   0        0        0     9649 2022-04-26 01:24:19.000000 xllabelme-5.1.5/xllabelme/shape.py
--rw-rw-rw-   0        0        0      886 2021-06-08 03:21:06.000000 xllabelme-5.1.5/xllabelme/testing.py
--rw-rw-rw-   0        0        0    44799 2023-04-04 12:30:43.000000 xllabelme-5.1.5/xllabelme/ts.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.275153 xllabelme-5.1.5/xllabelme/utils/
--rw-rw-rw-   0        0        0      749 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/utils/__init__.py
--rw-rw-rw-   0        0        0      698 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/utils/_io.py
--rw-rw-rw-   0        0        0     2468 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/utils/image.py
--rw-rw-rw-   0        0        0     6290 2023-04-04 09:31:32.000000 xllabelme-5.1.5/xllabelme/utils/qt.py
--rw-rw-rw-   0        0        0     3764 2021-06-08 03:21:06.000000 xllabelme-5.1.5/xllabelme/utils/shape.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.284129 xllabelme-5.1.5/xllabelme/widgets/
--rw-rw-rw-   0        0        0      554 2022-04-20 05:44:54.000000 xllabelme-5.1.5/xllabelme/widgets/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-03-31 14:44:05.000000 xllabelme-5.1.5/xllabelme/widgets/brightness_contrast_dialog.py
--rw-rw-rw-   0        0        0    35438 2023-04-20 08:18:28.000000 xllabelme-5.1.5/xllabelme/widgets/canvas.py
--rw-rw-rw-   0        0        0     1231 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/widgets/color_dialog.py
--rw-rw-rw-   0        0        0      290 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/widgets/escapable_qlist_widget.py
--rw-rw-rw-   0        0        0     2451 2023-04-15 14:50:00.000000 xllabelme-5.1.5/xllabelme/widgets/file_dialog_preview.py
--rw-rw-rw-   0        0        0    19741 2022-10-24 08:25:25.000000 xllabelme-5.1.5/xllabelme/widgets/label_dialog.py
--rw-rw-rw-   0        0        0     6194 2023-03-31 08:45:59.000000 xllabelme-5.1.5/xllabelme/widgets/label_list_widget.py
--rw-rw-rw-   0        0        0      998 2020-08-05 08:41:43.000000 xllabelme-5.1.5/xllabelme/widgets/tool_bar.py
--rw-rw-rw-   0        0        0     1666 2023-03-31 08:47:05.000000 xllabelme-5.1.5/xllabelme/widgets/unique_label_qlist_widget.py
--rw-rw-rw-   0        0        0      735 2023-04-04 11:11:05.000000 xllabelme-5.1.5/xllabelme/widgets/zoom_widget.py
--rw-rw-rw-   0        0        0    11774 2023-04-20 09:48:46.000000 xllabelme-5.1.5/xllabelme/xlapp.py
-drwxrwxrwx   0        0        0        0 2023-04-20 12:48:18.229276 xllabelme-5.1.5/xllabelme.egg-info/
--rw-rw-rw-   0        0        0    11738 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      281 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      116 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-20 12:48:18.000000 xllabelme-5.1.5/xllabelme.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.873485 xllabelme-5.1.6/
+-rw-rw-rw-   0        0        0      707 2020-11-09 02:22:17.000000 xllabelme-5.1.6/LICENSE
+-rw-rw-rw-   0        0        0       19 2020-08-05 08:41:43.000000 xllabelme-5.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    11738 2023-05-10 14:46:58.872485 xllabelme-5.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9202 2022-04-20 05:38:39.000000 xllabelme-5.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.754389 xllabelme-5.1.6/docs/
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.763365 xllabelme-5.1.6/docs/man/
+-rw-rw-rw-   0        0        0     2148 2020-08-05 08:41:43.000000 xllabelme-5.1.6/docs/man/labelme.1
+-rw-rw-rw-   0        0        0       42 2023-05-10 14:46:58.874481 xllabelme-5.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     5290 2023-04-20 12:13:49.000000 xllabelme-5.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.776331 xllabelme-5.1.6/xllabelme/
+-rw-rw-rw-   0        0        0     1074 2023-05-10 14:46:56.000000 xllabelme-5.1.6/xllabelme/__init__.py
+-rw-rw-rw-   0        0        0     7602 2023-04-18 02:03:52.000000 xllabelme-5.1.6/xllabelme/__main__.py
+-rw-rw-rw-   0        0        0    77978 2023-05-10 09:29:11.000000 xllabelme-5.1.6/xllabelme/app.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.791292 xllabelme-5.1.6/xllabelme/cli/
+-rw-rw-rw-   0        0        0      129 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/cli/__init__.py
+-rw-rw-rw-   0        0        0     1404 2022-04-20 05:42:00.000000 xllabelme-5.1.6/xllabelme/cli/draw_json.py
+-rw-rw-rw-   0        0        0      667 2021-06-08 03:21:06.000000 xllabelme-5.1.6/xllabelme/cli/draw_label_png.py
+-rw-rw-rw-   0        0        0     2473 2022-04-20 05:42:14.000000 xllabelme-5.1.6/xllabelme/cli/json_to_dataset.py
+-rw-rw-rw-   0        0        0     2851 2022-04-20 05:42:22.000000 xllabelme-5.1.6/xllabelme/cli/on_docker.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.794282 xllabelme-5.1.6/xllabelme/config/
+-rw-rw-rw-   0        0        0     2784 2021-06-08 03:21:07.000000 xllabelme-5.1.6/xllabelme/config/__init__.py
+-rw-rw-rw-   0        0        0     2340 2023-04-16 08:40:27.000000 xllabelme-5.1.6/xllabelme/config/default_config.yaml
+-rw-rw-rw-   0        0        0    62043 2023-05-10 14:45:43.000000 xllabelme-5.1.6/xllabelme/config/xllabellib.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.849123 xllabelme-5.1.6/xllabelme/icons/
+-rw-rw-rw-   0        0        0     2136 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/cancel.png
+-rw-rw-rw-   0        0        0     3111 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/close.png
+-rw-rw-rw-   0        0        0     2368 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/color-line.png
+-rw-rw-rw-   0        0        0     1461 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/color.png
+-rw-rw-rw-   0        0        0      646 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/copy.png
+-rw-rw-rw-   0        0        0     1486 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/delete.png
+-rw-rw-rw-   0        0        0     2198 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/done.png
+-rw-rw-rw-   0        0        0    22632 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/done.svg
+-rw-rw-rw-   0        0        0     1092 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/edit.png
+-rw-rw-rw-   0        0        0     7718 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/expert.png
+-rw-rw-rw-   0        0        0     1264 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/eye.png
+-rw-rw-rw-   0        0        0     8059 2019-01-15 04:29:26.000000 xllabelme-5.1.6/xllabelme/icons/feBlend-icon.png
+-rw-rw-rw-   0        0        0      765 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/file.png
+-rw-rw-rw-   0        0        0     1365 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/fit-width.png
+-rw-rw-rw-   0        0        0     1102 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/fit-window.png
+-rw-rw-rw-   0        0        0     2262 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/fit.png
+-rw-rw-rw-   0        0        0     1587 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/help.png
+-rw-rw-rw-   0        0        0   183198 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/icon.ico
+-rw-rw-rw-   0        0        0    44771 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/icon.png
+-rw-rw-rw-   0        0        0    38362 2023-04-04 10:35:02.000000 xllabelme-5.1.6/xllabelme/icons/icon2.ico
+-rw-rw-rw-   0        0        0    34213 2023-04-04 10:24:55.000000 xllabelme-5.1.6/xllabelme/icons/icon2.png
+-rw-rw-rw-   0        0        0     2381 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/labels.png
+-rw-rw-rw-   0        0        0    37512 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/labels.svg
+-rw-rw-rw-   0        0        0      977 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/new.png
+-rw-rw-rw-   0        0        0    30288 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/next.png
+-rw-rw-rw-   0        0        0     1103 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/objects.png
+-rw-rw-rw-   0        0        0     2073 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/open.png
+-rw-rw-rw-   0        0        0    18773 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/open.svg
+-rw-rw-rw-   0        0        0    30665 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/prev.png
+-rw-rw-rw-   0        0        0     1915 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/quit.png
+-rw-rw-rw-   0        0        0     2811 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/save-as.png
+-rw-rw-rw-   0        0        0    65363 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/save-as.svg
+-rw-rw-rw-   0        0        0     1187 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/save.png
+-rw-rw-rw-   0        0        0    31292 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/save.svg
+-rw-rw-rw-   0        0        0     2004 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/undo-cross.png
+-rw-rw-rw-   0        0        0     2018 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/undo.png
+-rw-rw-rw-   0        0        0     1099 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/zoom-in.png
+-rw-rw-rw-   0        0        0     1074 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/zoom-out.png
+-rw-rw-rw-   0        0        0     1139 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/icons/zoom.png
+-rw-rw-rw-   0        0        0     7120 2023-04-20 09:45:20.000000 xllabelme-5.1.6/xllabelme/label_file.py
+-rw-rw-rw-   0        0        0     1907 2023-03-31 08:56:10.000000 xllabelme-5.1.6/xllabelme/logger.py
+-rw-rw-rw-   0        0        0     9649 2022-04-26 01:24:19.000000 xllabelme-5.1.6/xllabelme/shape.py
+-rw-rw-rw-   0        0        0      886 2021-06-08 03:21:06.000000 xllabelme-5.1.6/xllabelme/testing.py
+-rw-rw-rw-   0        0        0    44799 2023-04-04 12:30:43.000000 xllabelme-5.1.6/xllabelme/ts.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.855529 xllabelme-5.1.6/xllabelme/utils/
+-rw-rw-rw-   0        0        0      749 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/utils/__init__.py
+-rw-rw-rw-   0        0        0      698 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/utils/_io.py
+-rw-rw-rw-   0        0        0     2468 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/utils/image.py
+-rw-rw-rw-   0        0        0     6290 2023-04-04 09:31:32.000000 xllabelme-5.1.6/xllabelme/utils/qt.py
+-rw-rw-rw-   0        0        0     3764 2021-06-08 03:21:06.000000 xllabelme-5.1.6/xllabelme/utils/shape.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.871488 xllabelme-5.1.6/xllabelme/widgets/
+-rw-rw-rw-   0        0        0      554 2022-04-20 05:44:54.000000 xllabelme-5.1.6/xllabelme/widgets/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-03-31 14:44:05.000000 xllabelme-5.1.6/xllabelme/widgets/brightness_contrast_dialog.py
+-rw-rw-rw-   0        0        0    35438 2023-04-20 08:18:28.000000 xllabelme-5.1.6/xllabelme/widgets/canvas.py
+-rw-rw-rw-   0        0        0     1231 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/widgets/color_dialog.py
+-rw-rw-rw-   0        0        0      290 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/widgets/escapable_qlist_widget.py
+-rw-rw-rw-   0        0        0     2451 2023-04-15 14:50:00.000000 xllabelme-5.1.6/xllabelme/widgets/file_dialog_preview.py
+-rw-rw-rw-   0        0        0    19741 2022-10-24 08:25:25.000000 xllabelme-5.1.6/xllabelme/widgets/label_dialog.py
+-rw-rw-rw-   0        0        0     6388 2023-05-10 09:32:37.000000 xllabelme-5.1.6/xllabelme/widgets/label_list_widget.py
+-rw-rw-rw-   0        0        0      998 2020-08-05 08:41:43.000000 xllabelme-5.1.6/xllabelme/widgets/tool_bar.py
+-rw-rw-rw-   0        0        0     1666 2023-03-31 08:47:05.000000 xllabelme-5.1.6/xllabelme/widgets/unique_label_qlist_widget.py
+-rw-rw-rw-   0        0        0      735 2023-04-04 11:11:05.000000 xllabelme-5.1.6/xllabelme/widgets/zoom_widget.py
+-rw-rw-rw-   0        0        0    11161 2023-05-10 13:24:58.000000 xllabelme-5.1.6/xllabelme/xlapp.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:46:58.784309 xllabelme-5.1.6/xllabelme.egg-info/
+-rw-rw-rw-   0        0        0    11738 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      281 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      116 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 14:46:58.000000 xllabelme-5.1.6/xllabelme.egg-info/top_level.txt
```

### Comparing `xllabelme-5.1.5/LICENSE` & `xllabelme-5.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/PKG-INFO` & `xllabelme-5.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xllabelme
-Version: 5.1.5
+Version: 5.1.6
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada
 Author-email: 877362867@qq.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xllabelme Version: 5.1.5 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: xllabelme Version: 5.1.6 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada Author-email: 877362867@qq.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `xllabelme-5.1.5/README.md` & `xllabelme-5.1.6/README.md`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/docs/man/labelme.1` & `xllabelme-5.1.6/docs/man/labelme.1`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/setup.py` & `xllabelme-5.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/__init__.py` & `xllabelme-5.1.6/xllabelme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Semantic Versioning 2.0.0: https://semver.org/
 # 1. MAJOR version when you make incompatible API changes;
 # 2. MINOR version when you add functionality in a backwards-compatible manner;
 # 3. PATCH version when you make backwards-compatible bug fixes.
 
 # 每当官方有第2位版本号更新，比如5.2、5.3时，我会尽力做个源码的同步
 # 然后我个人功能，会在第3位上自增，比如5.1.2、5.1.3
-__version__ = "5.1.5"
+__version__ = "5.1.6"
 
 # 2 扩展的更灵活的labelme，兼容官方的功能，但有更强的可视化效果，能查看shape的多个属性值
 __appname__ = f"xllabelme v{__version__}"
 
 QT4 = QT_VERSION[0] == "4"
 QT5 = QT_VERSION[0] == "5"
 del QT_VERSION
```

### Comparing `xllabelme-5.1.5/xllabelme/__main__.py` & `xllabelme-5.1.6/xllabelme/__main__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/app.py` & `xllabelme-5.1.6/xllabelme/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1675,63 +1675,43 @@
     # User Dialogs #
 
     def loadRecent(self, filename):
         if self.mayContinue():
             self.loadFile(filename)
 
     def openPrevImg(self, _value=False):
-        keep_prev = self._config["keep_prev"]
-        if QtWidgets.QApplication.keyboardModifiers() == (
-                Qt.ControlModifier | Qt.ShiftModifier
-        ):
-            self._config["keep_prev"] = True
-
-        if not self.mayContinue():
-            return
-
-        if len(self.imageList) <= 0:
-            return
-
-        if self.filename is None:
-            return
-
-        fn = XlPath(self.filename).relpath(self.lastOpenDir).as_posix()
-        currIndex = self.imageList.index(fn)
-        # currIndex = self.imageList.index(self.filename)
-        if currIndex - 1 >= 0:
-            filename = self.imageList[currIndex - 1]
-            if filename:
-                self.loadFile(filename)
-
-        self._config["keep_prev"] = keep_prev
+        return self.openNextImg(_value, offset=-1)
 
     def openNextImg(self, _value=False, load=True, offset=1):
         keep_prev = self._config["keep_prev"]
         if QtWidgets.QApplication.keyboardModifiers() == (
                 Qt.ControlModifier | Qt.ShiftModifier
         ):
             self._config["keep_prev"] = True
 
         if not self.mayContinue():
             return
 
         imageList = self.imageList
-        if len(imageList) <= 0:
+        num = len(imageList)
+        if num <= 0:
             return
 
         if self.filename is None:
             filename = imageList[0]
         else:
             try:
                 fn = XlPath(self.filename).relpath(self.lastOpenDir).as_posix()
-                currIndex = imageList.index(fn)
-                if currIndex + offset < len(imageList):
-                    filename = imageList[currIndex + offset]
-                else:
-                    filename = imageList[-1]
+                lastIndex = imageList.index(fn)
+                currIndex = lastIndex + offset
+                if currIndex < 0:
+                    currIndex, load = 0, lastIndex != currIndex
+                elif currIndex >= num:
+                    currIndex, load = num - 1, lastIndex != currIndex
+                filename = imageList[currIndex]
             except ValueError:  # 找不到则默认用第1个
                 filename = imageList[0]
         self.filename = XlPath(self.lastOpenDir, filename)
 
         if self.filename and load:
             self.loadFile(filename)
```

### Comparing `xllabelme-5.1.5/xllabelme/cli/draw_json.py` & `xllabelme-5.1.6/xllabelme/cli/draw_json.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/cli/draw_label_png.py` & `xllabelme-5.1.6/xllabelme/cli/draw_label_png.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/cli/json_to_dataset.py` & `xllabelme-5.1.6/xllabelme/cli/json_to_dataset.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/cli/on_docker.py` & `xllabelme-5.1.6/xllabelme/cli/on_docker.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/config/__init__.py` & `xllabelme-5.1.6/xllabelme/config/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/config/default_config.yaml` & `xllabelme-5.1.6/xllabelme/config/default_config.yaml`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/config/xllabellib.py` & `xllabelme-5.1.6/xllabelme/config/xllabellib.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from pyxllib.file.specialist import XlPath
 from pyxllib.algo.geo import rect_bounds
 from pyxllib.algo.pupil import make_index_function
 from pyxllib.prog.pupil import DictTool
 from pyxlpr.ai.clientlib import XlAiClient
 from pyxllib.algo.shapelylib import ShapelyPolygon
 # from pyxllib.xlcv import xlcv
+from pyxllib.cv.rgbfmt import RgbFormatter
 
 from xllabelme import utils
 from xllabelme.widgets import LabelListWidgetItem
 from xllabelme.shape import Shape
 
 _CONFIGS = {
     '原版labelme': {},
@@ -44,15 +45,19 @@
          'label_shape_color2': ['line_id'],
          'default_label': json.dumps({'line_id': 1,
                                       'content_type': '印刷体',
                                       'content_class': '文本',
                                       'text': ''}, ensure_ascii=False),
          },
     'm2303表格标注': {},
-    'm2303表格标注二阶段': {},
+    'm2303表格标注二阶段': {
+        '_attrs': [['text', 1, 'str', ('可见横线', '可见竖线', '不可见横线', '不可见竖线')]],
+        'label_shape_color': ['text'],
+    },
+    'm2305公式符号标注': {},
     # '渊亭OCR':  # 这是比较旧的一套配置字段名
     #     {'_attrs':
     #          [['content_type', 1, 'str', ('印刷体', '手写体', '印章', '其它')],
     #           ['content_kv', 1, 'str', ('key', 'value')],
     #           ["content_class", 1, "str", ("姓名", "身份证号", "联系方式", "采样时间", "检测时间", "核酸结果", "其它类")],
     #           ['text', 1, 'str'],
     #           ],
@@ -520,97 +525,43 @@
         """ 新建框的时候，使用的默认label值
 
         在这里可以定制不同项目生成新标注框的规则
         这里有办法获取原图，也有办法获取标注的shape，从而可以智能推断，给出识别值的
         """
         return self.mainwin.labelDialog.edit.text()
 
+    def open_last_workspace(self):
+        """ 打开上一次退出软件的工作空间状态 """
+        # 如果保存了目录和文件，打开上次工作状态
+        if 'lastOpenDir' in self.xllabel.meta_cfg:
+            d = XlPath(self.xllabel.meta_cfg['lastOpenDir'])
+            if d.is_dir():
+                if 'filename' in self.xllabel.meta_cfg:
+                    p = d / self.xllabel.meta_cfg['filename']
+                    if p.is_file():
+                        self.mainwin.importDirImages(d, filename=str(p), offset=0)
+                        return
+                self.mainwin.importDirImages(d)
+
+    def set_label_color(self, label, color=None):
+        """ 对普通文本值，做固定颜色映射 """
+        from xllabelme.xlapp import _COLORS
+
+        if isinstance(color, str):
+            color = RgbFormatter.from_name(color).to_tuple()
+
+        self.mainwin.labelDialog.addLabelHistory(label)  # 文本加入检索
+        # 主要为了兼容xllabelme的一个tolist操作，所以要转np
+        _COLORS[label] = np.array(color, 'uint8')  # 颜色做固定映射
+        _COLORS[str({'text': label})] = np.array(color, 'uint8')  # 被转成字典的时候，也要带颜色映射规则
+
 
 class 增强版xllabelme(原版labelme):
     """ xllabelme扩展功能 """
 
-    def create(self):
-        super().create()
-        mainwin = self.mainwin
-
-        action = functools.partial(utils.newAction, mainwin)
-        self.changeCheckAction = action(
-            "切换检查",
-            self.change_check,
-            'F1',  # 快捷键
-            None,
-            "（快捷键：F1）切换不同的数据检查模式，有不同的高亮方案。",
-            enabled=True,
-        )
-        resortShapesAction = action(
-            "标注排序",
-            self.resortShapes,
-            None,
-            None,
-            "重新对目前标注的框进行排序。",
-            enabled=True,
-        )
-        self.change_check(update=False)  # 把更精细的tip提示更新出来
-        mainwin.actions.tool = list(mainwin.actions.tool) + [None, self.changeCheckAction, resortShapesAction]
-
-        mainwin.populateModeActions()
-
-    def change_check(self, *, update=True):
-        """ 设置不同的高亮格式 """
-        if update:
-            self.xllabel.default_shape_color_mode += 1
-            self.xllabel.reset()
-            self.mainwin.updateLabelListItems()
-
-        # 提示给出更具体的使用的范式配置
-        act = self.changeCheckAction
-        tip = act.toolTip()
-        tip = re.sub(r'当前配置.*$', '', tip)
-        tip += '当前配置：' + ', '.join(self.xllabel.cfg['label_shape_color'])
-        act.setStatusTip(tip)
-        act.setToolTip(tip)
-
-    def resortShapes(self):
-        """ m2302中科院题库用，更新行号问题 """
-        from pyxlpr.data.imtextline import TextlineShape
-
-        mainwin = self.mainwin
-        # 目前只用于一个项目
-        if self.xllabel.meta_cfg['current_mode'] != 'm2302中科院题库':
-            return
-
-        # 0 数据预处理
-        def parse(sp):
-            points = [(p.x(), p.y()) for p in sp.points]
-            return [sp, json.loads(sp.label), TextlineShape(points)]
-
-        data = [parse(sp) for sp in mainwin.canvas.shapes]
-
-        # 1 按照标记的line_id大小重排序
-        # 先按行排序，然后行内按重心的x轴值排序（默认文本是从左往右读）。
-        data.sort(key=lambda x: (x[1]['line_id'], x[2].centroid.x))
-
-        # 2 编号重置，改成连续的自然数
-        cur_line_id, last_tag = 0, ''
-        for item in data:
-            sp, label = item[0], item[1]
-            if label['line_id'] != last_tag:
-                cur_line_id += 1
-                last_tag = label['line_id']
-            label['line_id'] = cur_line_id
-            sp.label = json.dumps(label, ensure_ascii=False)
-
-        # 3 更新回数据
-        mainwin.updateShapes([x[0] for x in data])
-
-    def destroy(self):
-        self.mainwin.actions.tool = self.mainwin.actions.tool[:-3]
-        self.mainwin.populateModeActions()
-        super().destroy()
-
     def update_shape(self, shape, label_list_item=None):
         """
         :param shape:
         :param label_list_item: item是shape的父级，挂在labelList下的项目
         """
         mainwin = self.mainwin
         # 1 确定显示的文本 text
@@ -685,14 +636,24 @@
         shape.fill_color = QtGui.QColor(*seleter('fill_color', (r, g, b, 128)))
         # 选中时的线、填充颜色
         shape.select_line_color = QtGui.QColor(*seleter('select_line_color', (255, 255, 255)))
         shape.select_fill_color = QtGui.QColor(*seleter('select_fill_color', (r, g, b, 155)))
 
         return label_list_item
 
+    def get_default_label(self, shape=None):
+        xllabel = self.mainwin.xllabel
+        label = xllabel.cfg.get('default_label', '')
+        if xllabel.auto_rec_text and xllabel.xlapi and shape:
+            k = 'label' if 'label' in xllabel.keys else 'text'
+            text, score = xllabel.rec_text(shape.points)
+            label = xllabel.set_label_attr(label, k, text)
+            label = xllabel.set_label_attr(label, 'score', score)
+        return label
+
     def new_shape(self):
         """ 新建标注框时的规则
         """
         mainwin = self.mainwin
         items = mainwin.uniqLabelList.selectedItems()
         text = None
         if items:
@@ -728,24 +689,14 @@
             mainwin.actions.undoLastPoint.setEnabled(False)
             mainwin.actions.undo.setEnabled(True)
             mainwin.setDirty()
         else:
             mainwin.canvas.undoLastLine()
             mainwin.canvas.shapesBackups.pop()
 
-    def get_default_label(self, shape=None):
-        xllabel = self.mainwin.xllabel
-        label = xllabel.cfg.get('default_label', '')
-        if xllabel.auto_rec_text and xllabel.xlapi and shape:
-            k = 'label' if 'label' in xllabel.keys else 'text'
-            text, score = xllabel.rec_text(shape.points)
-            label = xllabel.set_label_attr(label, k, text)
-            label = xllabel.set_label_attr(label, 'score', score)
-        return label
-
 
 class 文字通用(增强版xllabelme):
     def get_default_label(self, shape=None):
         d = {'text': '', 'category': '', 'text_kv': 'value', 'text_type': '印刷体'}
         return json.dumps(d, ensure_ascii=False)
 
 
@@ -780,14 +731,139 @@
                 line_id = line_id0
             else:
                 line_id = line_id0 + 1
         d['line_id'] = line_id
 
         return json.dumps(d, ensure_ascii=False)
 
+    def create(self):
+        super().create()
+        mainwin = self.mainwin
+
+        action = functools.partial(utils.newAction, mainwin)
+        self.changeCheckAction = action(
+            "切换检查",
+            self.change_check,
+            'F1',  # 快捷键
+            None,
+            "（快捷键：F1）切换不同的数据检查模式，有不同的高亮方案。",
+            enabled=True,
+        )
+        resortShapesAction = action(
+            "标注排序",
+            self.resortShapes,
+            None,
+            None,
+            "重新对目前标注的框进行排序。",
+            enabled=True,
+        )
+        self.change_check(update=False)  # 把更精细的tip提示更新出来
+
+        checkFormulaAction = action(
+            "检查全文章",
+            self.browser_paper,
+            None,
+            None,
+            "将内容按照shapes的顺序拼接成完整的文章，并检查公式渲染效率",
+            enabled=True,
+        )
+        # 检查文本行
+        # 检查小分块
+        mainwin.actions.tool = list(mainwin.actions.tool) + [
+            None,
+            self.changeCheckAction,
+            resortShapesAction,
+            checkFormulaAction,
+        ]
+
+        mainwin.populateModeActions()
+
+    def change_check(self, *, update=True):
+        """ 设置不同的高亮格式 """
+        if update:
+            self.xllabel.default_shape_color_mode += 1
+            self.xllabel.reset()
+            self.mainwin.updateLabelListItems()
+
+        # 提示给出更具体的使用的范式配置
+        act = self.changeCheckAction
+        tip = act.toolTip()
+        tip = re.sub(r'当前配置.*$', '', tip)
+        tip += '当前配置：' + ', '.join(self.xllabel.cfg['label_shape_color'])
+        act.setStatusTip(tip)
+        act.setToolTip(tip)
+
+    def resortShapes(self):
+        """ m2302中科院题库用，更新行号问题 """
+        from pyxlpr.data.imtextline import TextlineShape
+
+        mainwin = self.mainwin
+        # 目前只用于一个项目
+        if self.xllabel.meta_cfg['current_mode'] != 'm2302中科院题库':
+            return
+
+        # 0 数据预处理
+        def parse(sp):
+            points = [(p.x(), p.y()) for p in sp.points]
+            return [sp, json.loads(sp.label), TextlineShape(points)]
+
+        data = [parse(sp) for sp in mainwin.canvas.shapes]
+
+        # 1 按照标记的line_id大小重排序
+        # 先按行排序，然后行内按重心的x轴值排序（默认文本是从左往右读）。
+        data.sort(key=lambda x: (x[1]['line_id'], x[2].centroid.x))
+
+        # 2 编号重置，改成连续的自然数
+        cur_line_id, last_tag = 0, ''
+        for item in data:
+            sp, label = item[0], item[1]
+            if label['line_id'] != last_tag:
+                cur_line_id += 1
+                last_tag = label['line_id']
+            label['line_id'] = cur_line_id
+            sp.label = json.dumps(label, ensure_ascii=False)
+
+        # 3 更新回数据
+        mainwin.updateShapes([x[0] for x in data])
+
+    def browser_paper(self):
+        """ 将当前标注的text内容拼接并在公式文章渲染网页打开 """
+        # 1 拼接内容
+        shapes = self.mainwin.canvas.shapes
+        last_line_id = 1
+        paper_text = []
+        line_text = []
+        for sp in shapes:
+            label = json.loads(sp.label)
+            if label['line_id'] != last_line_id:
+                last_line_id = label['line_id']
+                paper_text.append(' '.join(line_text))
+                line_text = []
+
+            if label['content_class'] == '公式':
+                t = '$' + label['text'] + '$'
+            else:
+                t = label['text']
+            line_text.append(t)
+
+        paper_text.append(' '.join(line_text))
+        content = '\n\n'.join(paper_text)
+
+        # 2 获取渲染网页
+        title = self.mainwin.get_label_path().stem
+        r = requests.post('https://xmutpriu.com/latex/paper', json={'title': title, 'content': content})
+        p = XlPath.init(title + '.html', XlPath.tempdir())
+        p.write_text(r.text)
+        webbrowser.open(p)
+
+    def destroy(self):
+        self.mainwin.actions.tool = self.mainwin.actions.tool[:-4]
+        self.mainwin.populateModeActions()
+        super().destroy()
+
 
 class m2303表格标注(原版labelme):
     def get_default_label(self, shape=None):
         return '表格'
 
     def move_file(self, dst):
         # 0 准备
@@ -832,31 +908,148 @@
 
     def destroy(self):
         self.mainwin.menus.help.removeAction(self.help_action)
         self.fileListWidget.customContextMenuRequested.disconnect()
         super().destroy()
 
 
-class m2303表格标注二阶段(m2303表格标注):
+class m2303表格标注二阶段(增强版xllabelme):
+
+    def create(self):
+        super().create()
+
+        mainwin = self.mainwin
+        url = "https://www.yuque.com/xlpr/data/kvq2g82zvk5x1lkb?singleDoc#"
+        self.help_action = utils.newAction(mainwin, mainwin.tr("表格二阶段标注说明"),
+                                           lambda: webbrowser.open(url))
+        mainwin.menus.help.addAction(self.help_action)
+
+        self.set_label_color('可见横线', (0, 123, 255))  # 蓝色
+        self.set_label_color('可见竖线', (40, 167, 69))  # 绿色
+        self.set_label_color('不可见横线', (174, 223, 247))  # 不可见是可见对应的浅色
+        self.set_label_color('不可见竖线', (180, 244, 190))
+
+    def destroy(self):
+        self.mainwin.menus.help.removeAction(self.help_action)
+
+        super().destroy()
+
     def get_default_label(self, shape=None):
-        """ 这个识别可以做的更精细的，不过这个项目不一定接，现在只做一个最基础性的功能 """
-        # 表格, 可见横线, 可见竖线, 不可见横线, 不可见竖线
+        """ 还有些细节要调，如果弹窗，应该给出默认的几种类别文本 """
+        from pyxllib.cv.xlcvlib import xlcv
 
+        # 0 注意：标注过程中，是可以修改框的位置的
+        # shape.points = [QPointF(100, 100), QPointF(200, 200)]
+
+        # 1 框的基本几何信息
         poly = ShapelyPolygon.gen([(p.x(), p.y()) for p in shape.points])
         bounds = poly.bounds
         width = bounds[2] - bounds[0]
         height = bounds[3] - bounds[1]
 
-        # 注意：标注过程中，是可以修改框的位置的
-        # shape.points = [QPointF(100, 100), QPointF(200, 200)]
+        # 2 图片信息
+        # 表格, 可见横线, 可见竖线, 不可见横线, 不可见竖线
+        mainwin = self.mainwin
+        points = [(p.x(), p.y()) for p in shape.points]
+        im = xlcv.get_sub(mainwin.arr_image, points, warp_quad=True)
+        im = xlcv.read(im, 0)  # 先转灰度图
+        im = xlcv.replace_ground_color(im, 0, 255)  # 然后转白底黑字图
+        color = im.mean()  # 计算平均颜色，越接近255，表示越是空白图。
+
+        # 3 自动识别线类型
+        visible_tag = '可见' if color < 250 else '不可见'
+        line_tag = '竖线' if height > width else '横线'
+        return json.dumps({'text': visible_tag + line_tag}, ensure_ascii=False)
+
+    def new_shape(self):
+        """ 不用弹窗，直接给类别
+        """
+        mainwin = self.mainwin
+        items = mainwin.uniqLabelList.selectedItems()
+        text = None
+        if items:
+            text = items[0].data(Qt.UserRole)
+        flags = {}
+        group_id = None
+        if mainwin._config["display_label_popup"] or not text:
+            previous_text = mainwin.labelDialog.edit.text()
 
-        if height > width:
-            return '可见竖线'
+            shape = Shape()
+            shape.label = self.get_default_label(shape=mainwin.canvas.shapes[-1])
+            # shape = mainwin.labelDialog.popUp2(shape, mainwin)
+            if shape is not None:
+                text, flags, group_id = shape.label, shape.flags, shape.group_id
+
+            if not text:
+                mainwin.labelDialog.edit.setText(previous_text)
+
+        if text and not mainwin.validateLabel(text):
+            mainwin.errorMessage(
+                mainwin.tr("Invalid label"),
+                mainwin.tr("Invalid label '{}' with validation type '{}'").format(
+                    text, mainwin._config["validate_label"]
+                ),
+            )
+            text = ""
+        if text:
+            mainwin.labelList.clearSelection()
+            shape = mainwin.canvas.setLastLabel(text, flags)
+            shape.group_id = group_id
+            mainwin.addLabel(shape)
+            mainwin.actions.editMode.setEnabled(True)
+            mainwin.actions.undoLastPoint.setEnabled(False)
+            mainwin.actions.undo.setEnabled(True)
+            mainwin.setDirty()
         else:
-            return '可见横线'
+            mainwin.canvas.undoLastLine()
+            mainwin.canvas.shapesBackups.pop()
+
+class m2305公式符号标注(原版labelme):
+    def create(self):
+        super().create()
+
+        mainwin = self.mainwin
+        url = "https://www.yuque.com/xlpr/data/sn3uglc7g6l49akv?singleDoc#"
+        self.help_action = utils.newAction(mainwin, mainwin.tr("公式符号标注说明"),
+                                           lambda: webbrowser.open(url))
+        mainwin.menus.help.addAction(self.help_action)
+
+    def destroy(self):
+        self.mainwin.menus.help.removeAction(self.help_action)
+
+        super().destroy()
+
+    def new_shape(self):
+        """ 这个项目的new_shape比较特别，并不实际添加shape，而是把无效的矩形框重新替换标注
+
+        这个功能是有一定通用性的，以后可以考虑怎么加到一般功能性框架。
+        """
+        # 1 找到第一个未显示的shape
+        mainwin = self.mainwin
+        model = mainwin.labelList.model()
+        for index in range(model.rowCount()):
+            item = model.item(index, 0)
+            if not item.checkState():
+                break
+        else:  # 如果已经全部修复，则创建不了新矩形
+            return
+
+        # 2 更新shapes位置
+        shapes = mainwin.canvas.shapes
+
+        mainwin.labelList.clearSelection()
+
+        item.shape().points = shapes[-1].points
+        item.setCheckState(Qt.Checked)
+        mainwin.canvas.shapes = shapes[:-1]
+
+        mainwin.actions.editMode.setEnabled(True)
+        mainwin.actions.undoLastPoint.setEnabled(False)
+        mainwin.actions.undo.setEnabled(True)
+        mainwin.setDirty()
 
 
 def __2_xllabel中介组件():
     pass
 
 
 class XlLabel:
```

### Comparing `xllabelme-5.1.5/xllabelme/icons/cancel.png` & `xllabelme-5.1.6/xllabelme/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/close.png` & `xllabelme-5.1.6/xllabelme/icons/close.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/color-line.png` & `xllabelme-5.1.6/xllabelme/icons/color-line.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/color.png` & `xllabelme-5.1.6/xllabelme/icons/color.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/copy.png` & `xllabelme-5.1.6/xllabelme/icons/copy.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/delete.png` & `xllabelme-5.1.6/xllabelme/icons/delete.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/done.png` & `xllabelme-5.1.6/xllabelme/icons/done.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/done.svg` & `xllabelme-5.1.6/xllabelme/icons/done.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/edit.png` & `xllabelme-5.1.6/xllabelme/icons/edit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/expert.png` & `xllabelme-5.1.6/xllabelme/icons/expert.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/eye.png` & `xllabelme-5.1.6/xllabelme/icons/eye.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/feBlend-icon.png` & `xllabelme-5.1.6/xllabelme/icons/feBlend-icon.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/file.png` & `xllabelme-5.1.6/xllabelme/icons/file.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/fit-width.png` & `xllabelme-5.1.6/xllabelme/icons/fit-width.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/fit-window.png` & `xllabelme-5.1.6/xllabelme/icons/fit-window.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/fit.png` & `xllabelme-5.1.6/xllabelme/icons/fit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/help.png` & `xllabelme-5.1.6/xllabelme/icons/help.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/icon.ico` & `xllabelme-5.1.6/xllabelme/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/icon.png` & `xllabelme-5.1.6/xllabelme/icons/icon.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/icon2.ico` & `xllabelme-5.1.6/xllabelme/icons/icon2.ico`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/icon2.png` & `xllabelme-5.1.6/xllabelme/icons/icon2.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/labels.png` & `xllabelme-5.1.6/xllabelme/icons/labels.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/labels.svg` & `xllabelme-5.1.6/xllabelme/icons/labels.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/new.png` & `xllabelme-5.1.6/xllabelme/icons/new.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/next.png` & `xllabelme-5.1.6/xllabelme/icons/next.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/objects.png` & `xllabelme-5.1.6/xllabelme/icons/objects.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/open.png` & `xllabelme-5.1.6/xllabelme/icons/open.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/open.svg` & `xllabelme-5.1.6/xllabelme/icons/open.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/prev.png` & `xllabelme-5.1.6/xllabelme/icons/prev.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/quit.png` & `xllabelme-5.1.6/xllabelme/icons/quit.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/save-as.png` & `xllabelme-5.1.6/xllabelme/icons/save-as.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/save-as.svg` & `xllabelme-5.1.6/xllabelme/icons/save-as.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/save.png` & `xllabelme-5.1.6/xllabelme/icons/save.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/save.svg` & `xllabelme-5.1.6/xllabelme/icons/save.svg`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/undo-cross.png` & `xllabelme-5.1.6/xllabelme/icons/undo-cross.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/undo.png` & `xllabelme-5.1.6/xllabelme/icons/undo.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/zoom-in.png` & `xllabelme-5.1.6/xllabelme/icons/zoom-in.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/zoom-out.png` & `xllabelme-5.1.6/xllabelme/icons/zoom-out.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/icons/zoom.png` & `xllabelme-5.1.6/xllabelme/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/label_file.py` & `xllabelme-5.1.6/xllabelme/label_file.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/logger.py` & `xllabelme-5.1.6/xllabelme/logger.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/shape.py` & `xllabelme-5.1.6/xllabelme/shape.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/testing.py` & `xllabelme-5.1.6/xllabelme/testing.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/ts.py` & `xllabelme-5.1.6/xllabelme/ts.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/utils/__init__.py` & `xllabelme-5.1.6/xllabelme/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/utils/_io.py` & `xllabelme-5.1.6/xllabelme/utils/_io.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/utils/image.py` & `xllabelme-5.1.6/xllabelme/utils/image.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/utils/qt.py` & `xllabelme-5.1.6/xllabelme/utils/qt.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/utils/shape.py` & `xllabelme-5.1.6/xllabelme/utils/shape.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/__init__.py` & `xllabelme-5.1.6/xllabelme/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/brightness_contrast_dialog.py` & `xllabelme-5.1.6/xllabelme/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/canvas.py` & `xllabelme-5.1.6/xllabelme/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/color_dialog.py` & `xllabelme-5.1.6/xllabelme/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/file_dialog_preview.py` & `xllabelme-5.1.6/xllabelme/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/label_dialog.py` & `xllabelme-5.1.6/xllabelme/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/label_list_widget.py` & `xllabelme-5.1.6/xllabelme/widgets/label_list_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,14 +163,20 @@
 
     def scrollToItem(self, item):
         self.scrollTo(self.model().indexFromItem(item))
 
     def addItem(self, item):
         if not isinstance(item, LabelListWidgetItem):
             raise TypeError("item must be LabelListWidgetItem")
+
+        # 非法形状初始化的时候不显示
+        sp = item.shape()
+        if sp.shape_type == 'rectangle' and len(sp.points) == 1:
+            item.setCheckState(Qt.Unchecked)
+
         self.model().setItem(self.model().rowCount(), 0, item)
         item.setSizeHint(self.itemDelegate().sizeHint(None, None))
 
     def removeItem(self, item):
         index = self.model().indexFromItem(item)
         self.model().removeRows(index.row(), 1)
```

### Comparing `xllabelme-5.1.5/xllabelme/widgets/tool_bar.py` & `xllabelme-5.1.6/xllabelme/widgets/tool_bar.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/unique_label_qlist_widget.py` & `xllabelme-5.1.6/xllabelme/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/widgets/zoom_widget.py` & `xllabelme-5.1.6/xllabelme/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `xllabelme-5.1.5/xllabelme/xlapp.py` & `xllabelme-5.1.6/xllabelme/xlapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             output_file=None,
             output_dir=None,
     ):
         super(XlMainWindow, self).__init__(config, filename, output, output_file, output_dir)
         self.arr_image = None  # cv2格式的图片
         self.xllabel = XlLabel(self)
         self.project = self.xllabel.open_project()
-        self.open_last_workspace()
+        self.project.open_last_workspace()
 
     def extendShapeMessage(self, shape):
         """ shape中自定义字段等信息
 
         :param shape: shape对象
         :return: 格式化的字符串内容
         """
@@ -293,20 +293,7 @@
         return tip
 
     def showMessage(self, text):
         """ setStatusBar只是设置值，而不是显示值
         显示值得用下述方式实现~~
         """
         self.statusBar().showMessage(text)
-
-    def open_last_workspace(self):
-        """ 打开上一次退出软件的工作空间状态 """
-        # 如果保存了目录和文件，打开上次工作状态
-        if 'lastOpenDir' in self.xllabel.meta_cfg:
-            d = XlPath(self.xllabel.meta_cfg['lastOpenDir'])
-            if d.is_dir():
-                if 'filename' in self.xllabel.meta_cfg:
-                    p = d / self.xllabel.meta_cfg['filename']
-                    if p.is_file():
-                        self.importDirImages(d, filename=str(p), offset=0)
-                        return
-                self.importDirImages(d)
```

### Comparing `xllabelme-5.1.5/xllabelme.egg-info/PKG-INFO` & `xllabelme-5.1.6/xllabelme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xllabelme
-Version: 5.1.5
+Version: 5.1.6
 Summary: Image Polygonal Annotation with Python
 Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada
 Author-email: 877362867@qq.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xllabelme Version: 5.1.5 Summary: Image Polygonal
+Metadata-Version: 2.1 Name: xllabelme Version: 5.1.6 Summary: Image Polygonal
 Annotation with Python Home-page: https://github.com/XLPRUtils/xllabelme
 Author: code4101,Kentaro Wada Author-email: 877362867@qq.com License: GPLv3
 Keywords: Image Annotation,Machine Learning Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
```

### Comparing `xllabelme-5.1.5/xllabelme.egg-info/SOURCES.txt` & `xllabelme-5.1.6/xllabelme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

