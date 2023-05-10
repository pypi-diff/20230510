# Comparing `tmp/aps_common_libraries-1.0.5.tar.gz` & `tmp/aps_common_libraries-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps_common_libraries-1.0.5.tar", last modified: Wed May 10 01:17:14 2023, max compression
+gzip compressed data, was "aps_common_libraries-1.0.6.tar", last modified: Wed May 10 12:50:35 2023, max compression
```

## Comparing `aps_common_libraries-1.0.5.tar` & `aps_common_libraries-1.0.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.069131 aps_common_libraries-1.0.5/
--rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.5/LICENSE
--rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.5/LICENSE.pdf
--rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.5/MANIFEST.in
--rw-r--r--   0 bishop    (1601)      907      876 2023-05-10 01:17:14.068785 aps_common_libraries-1.0.5/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.5/README.md
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.017822 aps_common_libraries-1.0.5/aps/
--rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.5/aps/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.023426 aps_common_libraries-1.0.5/aps/common/
--rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.5/aps/common/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.025596 aps_common_libraries-1.0.5/aps/common/__test/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.5/aps/common/__test/__init__.py
--rw-r--r--   0 bishop    (1601)      907     3683 2023-05-05 00:42:24.000000 aps_common_libraries-1.0.5/aps/common/__test/singletons.py
--rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.5/aps/common/__test/test.py
--rw-r--r--   0 bishop    (1601)      907     5739 2023-05-05 00:41:47.000000 aps_common_libraries-1.0.5/aps/common/__test/test2.py
--rw-rw-rw-   0 bishop    (1601)      907    10116 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.5/aps/common/initializer.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.029054 aps_common_libraries-1.0.5/aps/common/io/
--rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.5/aps/common/io/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.5/aps/common/io/printout.py
--rw-r--r--   0 bishop    (1601)      907     3693 2023-05-04 23:44:10.000000 aps_common_libraries-1.0.5/aps/common/io/sys_commands.py
--rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.5/aps/common/io/tcp_client.py
--rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.5/aps/common/io/tiff_file.py
--rw-rw-rw-   0 bishop    (1601)      907    20774 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.5/aps/common/logger.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.029576 aps_common_libraries-1.0.5/aps/common/measurment/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.5/aps/common/measurment/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.031442 aps_common_libraries-1.0.5/aps/common/measurment/beamline/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/__init__.py
--rw-r--r--   0 bishop    (1601)      907    10472 2023-03-29 01:21:24.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/image_collector.py
--rw-r--r--   0 bishop    (1601)      907    32561 2023-03-31 13:27:26.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/image_processor.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.041110 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/
--rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/SPINNet_estimate.py
--rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/WXST.py
--rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/diffraction_process.py
--rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/euclidean_dist.py
--rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/func.py
--rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/func_light.py
--rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/gui_func.py
--rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/integration.py
--rw-rw-rw-   0 bishop    (1601)      907    77489 2023-03-31 13:34:40.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/main.py
--rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/pattern_find.py
--rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/pattern_propagate.py
--rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/utils.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.043408 aps_common_libraries-1.0.5/aps/common/ml/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.5/aps/common/ml/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.5/aps/common/ml/data_structures.py
--rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.5/aps/common/ml/mocks.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.046676 aps_common_libraries-1.0.5/aps/common/plot/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.5/aps/common/plot/__init__.py
--rw-r--r--   0 bishop    (1601)      907    44717 2023-04-08 13:27:45.000000 aps_common_libraries-1.0.5/aps/common/plot/gui.py
--rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.5/aps/common/plot/image.py
--rw-rw-rw-   0 bishop    (1601)      907     6365 2023-02-16 16:28:45.000000 aps_common_libraries-1.0.5/aps/common/plot/qt_application.py
--rw-rw-rw-   0 bishop    (1601)      907    16735 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.5/aps/common/plotter.py
--rw-r--r--   0 bishop    (1601)      907     5229 2023-05-02 21:11:06.000000 aps_common_libraries-1.0.5/aps/common/reflection.py
--rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.5/aps/common/registry.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.051147 aps_common_libraries-1.0.5/aps/common/scripts/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.5/aps/common/scripts/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.5/aps/common/scripts/abstract_command_line_script.py
--rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.5/aps/common/scripts/generic_process_manager.py
--rw-rw-rw-   0 bishop    (1601)      907     8024 2023-05-10 00:09:44.000000 aps_common_libraries-1.0.5/aps/common/scripts/generic_qt_script.py
--rw-rw-rw-   0 bishop    (1601)      907     4121 2023-02-07 23:10:48.000000 aps_common_libraries-1.0.5/aps/common/scripts/script_data.py
--rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.5/aps/common/scripts/script_registry.py
--rw-rw-rw-   0 bishop    (1601)      907     4677 2023-05-05 00:43:28.000000 aps_common_libraries-1.0.5/aps/common/singleton.py
--rw-rw-rw-   0 bishop    (1601)      907    10093 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.5/aps/common/traffic_light.py
--rw-r--r--   0 bishop    (1601)      907     3543 2023-05-03 14:01:58.000000 aps_common_libraries-1.0.5/aps/common/utilities.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.063564 aps_common_libraries-1.0.5/aps/common/widgets/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.5/aps/common/widgets/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4081 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.5/aps/common/widgets/close_app_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.5/aps/common/widgets/context_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.5/aps/common/widgets/generic_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.5/aps/common/widgets/log_stream_widget.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 01:17:14.068108 aps_common_libraries-1.0.5/aps_common_libraries.egg-info/
--rw-rw-rw-   0 bishop    (1601)      907      876 2023-05-10 01:17:13.000000 aps_common_libraries-1.0.5/aps_common_libraries.egg-info/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907     2268 2023-05-10 01:17:13.000000 aps_common_libraries-1.0.5/aps_common_libraries.egg-info/SOURCES.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2023-05-10 01:17:13.000000 aps_common_libraries-1.0.5/aps_common_libraries.egg-info/dependency_links.txt
--rw-rw-rw-   0 bishop    (1601)      907       15 2023-05-10 01:17:13.000000 aps_common_libraries-1.0.5/aps_common_libraries.egg-info/namespace_packages.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.5/aps_common_libraries.egg-info/not-zip-safe
--rw-rw-rw-   0 bishop    (1601)      907      150 2023-05-10 01:17:13.000000 aps_common_libraries-1.0.5/aps_common_libraries.egg-info/requires.txt
--rw-rw-rw-   0 bishop    (1601)      907        4 2023-05-10 01:17:13.000000 aps_common_libraries-1.0.5/aps_common_libraries.egg-info/top_level.txt
--rw-r--r--   0 bishop    (1601)      907       38 2023-05-10 01:17:14.069279 aps_common_libraries-1.0.5/setup.cfg
--rw-r--r--   0 bishop    (1601)      907     5571 2023-05-10 01:16:51.000000 aps_common_libraries-1.0.5/setup.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.342385 aps_common_libraries-1.0.6/
+-rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.6/LICENSE
+-rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.6/LICENSE.pdf
+-rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.6/MANIFEST.in
+-rw-r--r--   0 bishop    (1601)      907      876 2023-05-10 12:50:35.341837 aps_common_libraries-1.0.6/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.6/README.md
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.273540 aps_common_libraries-1.0.6/aps/
+-rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.6/aps/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.281082 aps_common_libraries-1.0.6/aps/common/
+-rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.6/aps/common/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.285956 aps_common_libraries-1.0.6/aps/common/__test/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.6/aps/common/__test/__init__.py
+-rw-r--r--   0 bishop    (1601)      907     3683 2023-05-05 00:42:24.000000 aps_common_libraries-1.0.6/aps/common/__test/singletons.py
+-rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.6/aps/common/__test/test.py
+-rw-r--r--   0 bishop    (1601)      907     5739 2023-05-05 00:41:47.000000 aps_common_libraries-1.0.6/aps/common/__test/test2.py
+-rw-rw-rw-   0 bishop    (1601)      907    10116 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.6/aps/common/initializer.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.290631 aps_common_libraries-1.0.6/aps/common/io/
+-rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.6/aps/common/io/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.6/aps/common/io/printout.py
+-rw-r--r--   0 bishop    (1601)      907     3693 2023-05-04 23:44:10.000000 aps_common_libraries-1.0.6/aps/common/io/sys_commands.py
+-rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.6/aps/common/io/tcp_client.py
+-rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.6/aps/common/io/tiff_file.py
+-rw-rw-rw-   0 bishop    (1601)      907    20774 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.6/aps/common/logger.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.291362 aps_common_libraries-1.0.6/aps/common/measurment/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.6/aps/common/measurment/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.294193 aps_common_libraries-1.0.6/aps/common/measurment/beamline/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    10472 2023-03-29 01:21:24.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/image_collector.py
+-rw-r--r--   0 bishop    (1601)      907    32561 2023-03-31 13:27:26.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/image_processor.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.310077 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/
+-rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/SPINNet_estimate.py
+-rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/WXST.py
+-rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/diffraction_process.py
+-rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/euclidean_dist.py
+-rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/func.py
+-rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/func_light.py
+-rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/gui_func.py
+-rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/integration.py
+-rw-rw-rw-   0 bishop    (1601)      907    77489 2023-03-31 13:34:40.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/main.py
+-rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/pattern_find.py
+-rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/pattern_propagate.py
+-rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/utils.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.313506 aps_common_libraries-1.0.6/aps/common/ml/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.6/aps/common/ml/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.6/aps/common/ml/data_structures.py
+-rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.6/aps/common/ml/mocks.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.317649 aps_common_libraries-1.0.6/aps/common/plot/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.6/aps/common/plot/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    45238 2023-05-10 12:48:38.000000 aps_common_libraries-1.0.6/aps/common/plot/gui.py
+-rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.6/aps/common/plot/image.py
+-rw-rw-rw-   0 bishop    (1601)      907     6365 2023-02-16 16:28:45.000000 aps_common_libraries-1.0.6/aps/common/plot/qt_application.py
+-rw-rw-rw-   0 bishop    (1601)      907    16735 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.6/aps/common/plotter.py
+-rw-r--r--   0 bishop    (1601)      907     5229 2023-05-02 21:11:06.000000 aps_common_libraries-1.0.6/aps/common/reflection.py
+-rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.6/aps/common/registry.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.324843 aps_common_libraries-1.0.6/aps/common/scripts/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.6/aps/common/scripts/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.6/aps/common/scripts/abstract_command_line_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.6/aps/common/scripts/generic_process_manager.py
+-rw-rw-rw-   0 bishop    (1601)      907     8024 2023-05-10 00:09:44.000000 aps_common_libraries-1.0.6/aps/common/scripts/generic_qt_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     4121 2023-02-07 23:10:48.000000 aps_common_libraries-1.0.6/aps/common/scripts/script_data.py
+-rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.6/aps/common/scripts/script_registry.py
+-rw-rw-rw-   0 bishop    (1601)      907     4677 2023-05-05 00:43:28.000000 aps_common_libraries-1.0.6/aps/common/singleton.py
+-rw-rw-rw-   0 bishop    (1601)      907    10093 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.6/aps/common/traffic_light.py
+-rw-r--r--   0 bishop    (1601)      907     3543 2023-05-03 14:01:58.000000 aps_common_libraries-1.0.6/aps/common/utilities.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.331738 aps_common_libraries-1.0.6/aps/common/widgets/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.6/aps/common/widgets/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     4081 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.6/aps/common/widgets/close_app_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.6/aps/common/widgets/context_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.6/aps/common/widgets/generic_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.6/aps/common/widgets/log_stream_widget.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 12:50:35.340570 aps_common_libraries-1.0.6/aps_common_libraries.egg-info/
+-rw-rw-rw-   0 bishop    (1601)      907      876 2023-05-10 12:50:35.000000 aps_common_libraries-1.0.6/aps_common_libraries.egg-info/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907     2268 2023-05-10 12:50:35.000000 aps_common_libraries-1.0.6/aps_common_libraries.egg-info/SOURCES.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2023-05-10 12:50:35.000000 aps_common_libraries-1.0.6/aps_common_libraries.egg-info/dependency_links.txt
+-rw-rw-rw-   0 bishop    (1601)      907       15 2023-05-10 12:50:35.000000 aps_common_libraries-1.0.6/aps_common_libraries.egg-info/namespace_packages.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.6/aps_common_libraries.egg-info/not-zip-safe
+-rw-rw-rw-   0 bishop    (1601)      907      150 2023-05-10 12:50:35.000000 aps_common_libraries-1.0.6/aps_common_libraries.egg-info/requires.txt
+-rw-rw-rw-   0 bishop    (1601)      907        4 2023-05-10 12:50:35.000000 aps_common_libraries-1.0.6/aps_common_libraries.egg-info/top_level.txt
+-rw-r--r--   0 bishop    (1601)      907       38 2023-05-10 12:50:35.342594 aps_common_libraries-1.0.6/setup.cfg
+-rw-r--r--   0 bishop    (1601)      907     5571 2023-05-10 12:48:38.000000 aps_common_libraries-1.0.6/setup.py
```

### Comparing `aps_common_libraries-1.0.5/LICENSE` & `aps_common_libraries-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/LICENSE.pdf` & `aps_common_libraries-1.0.6/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/PKG-INFO` & `aps_common_libraries-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aps_common_libraries
-Version: 1.0.5
+Version: 1.0.6
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
```

### Comparing `aps_common_libraries-1.0.5/aps/__init__.py` & `aps_common_libraries-1.0.6/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/__init__.py` & `aps_common_libraries-1.0.6/aps/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/__test/__init__.py` & `aps_common_libraries-1.0.6/aps/common/__test/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/__test/singletons.py` & `aps_common_libraries-1.0.6/aps/common/__test/singletons.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/__test/test.py` & `aps_common_libraries-1.0.6/aps/common/__test/test.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/__test/test2.py` & `aps_common_libraries-1.0.6/aps/common/__test/test2.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/initializer.py` & `aps_common_libraries-1.0.6/aps/common/initializer.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/io/__init__.py` & `aps_common_libraries-1.0.6/aps/common/io/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/io/printout.py` & `aps_common_libraries-1.0.6/aps/common/io/printout.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/io/sys_commands.py` & `aps_common_libraries-1.0.6/aps/common/io/sys_commands.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/io/tcp_client.py` & `aps_common_libraries-1.0.6/aps/common/io/tcp_client.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/io/tiff_file.py` & `aps_common_libraries-1.0.6/aps/common/io/tiff_file.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/logger.py` & `aps_common_libraries-1.0.6/aps/common/logger.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/__init__.py` & `aps_common_libraries-1.0.6/aps/common/measurment/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/__init__.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/image_collector.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/image_collector.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/image_processor.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/image_processor.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/SPINNet_estimate.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/SPINNet_estimate.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/WXST.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/WXST.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/__init__.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/diffraction_process.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/diffraction_process.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/euclidean_dist.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/euclidean_dist.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/func.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/func_light.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/func_light.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/gui_func.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/gui_func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/integration.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/integration.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/main.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/main.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/pattern_find.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/pattern_find.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/measurment/beamline/wf/pattern_propagate.py` & `aps_common_libraries-1.0.6/aps/common/measurment/beamline/wf/pattern_propagate.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/ml/__init__.py` & `aps_common_libraries-1.0.6/aps/common/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/ml/data_structures.py` & `aps_common_libraries-1.0.6/aps/common/ml/data_structures.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/ml/mocks.py` & `aps_common_libraries-1.0.6/aps/common/ml/mocks.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/plot/__init__.py` & `aps_common_libraries-1.0.6/aps/common/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/plot/gui.py` & `aps_common_libraries-1.0.6/aps/common/plot/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 # POSSIBILITY OF SUCH DAMAGE.                                             #
 # ----------------------------------------------------------------------- #
 
 
 ##########################################################################
 # WIDGETS UTILS FROM OASYS
 
-from PyQt5.QtWidgets import QWidget, QMessageBox, QTextEdit, QFileDialog
+from PyQt5.QtWidgets import QWidget, QMessageBox, QTextEdit, QFileDialog, QLineEdit
+from PyQt5.QtGui import QFont, QPalette, QColor
 
 def _set_size(dialog, width, height):
     stylesheet_string = "QLabel{"
     if not width is None:  stylesheet_string += "min-width: " + str(width) + "px;"
     if not height is None: stylesheet_string += "min-height: " + str(height) + "px;"
     stylesheet_string += "}"
     if not (width is None and height is None): dialog.setStyleSheet(stylesheet_string)
@@ -164,19 +165,30 @@
 def widgetLabel(widget, label="", labelWidth=None, **misc):
     lbl = QLabel(label, widget)
     if labelWidth: lbl.setFixedSize(labelWidth, lbl.sizeHint().height())
     __miscellanea(lbl, None, widget, **misc)
 
     return lbl
 
+def setReadOnly(lineedit: QLineEdit):
+    lineedit.setReadOnly(True)
+    font = QFont(lineedit.font())
+    font.setBold(True)
+    lineedit.setFont(font)
+    palette = QPalette(lineedit.palette())
+    palette.setColor(QPalette.Text, QColor('dark blue'))
+    lineedit.setPalette(palette)
+    lineedit.setStyleSheet("QLineEdit { background: rgb(243, 240, 160); selection-background-color: rgb(233, 99, 0); }")
+
+
 def lineEdit(widget, master, value, label=None, labelWidth=None,
              orientation='vertical', box=None, callback=None,
              valueType=str, validator=None, controlWidth=None,
              callbackOnType=False, focusInCallback=None,
-             enterPlaceholder=False, **misc):
+             enterPlaceholder=False, readOnly=False, **misc):
     if box or label:
         b = widgetBox(widget, box, orientation, addToLayout=False)
         widgetLabel(b, label, labelWidth)
         hasHBox = orientation == 'horizontal' or not orientation
     else:
         b = widget
         hasHBox = False
@@ -205,14 +217,16 @@
                                                   callbackOnType and callback, ledit.textChanged[str],
                                                   __CallFrontLineEdit(ledit), fvcb=value and valueType)[1]
 
     __miscellanea(ledit, b, widget, **misc)
     if value and (valueType != str): ledit.setAlignment(Qt.AlignRight)
     ledit.setStyleSheet("background-color: white;")
 
+    if readOnly: setReadOnly(ledit)
+
     return ledit
 
 def button(widget, master, label, callback=None, width=None, height=None,
            toggleButton=False, value="", default=False, autoDefault=True,
            buttonType=QPushButton, **misc):
     button = buttonType(widget)
     if label:
```

### Comparing `aps_common_libraries-1.0.5/aps/common/plot/image.py` & `aps_common_libraries-1.0.6/aps/common/plot/image.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/plot/qt_application.py` & `aps_common_libraries-1.0.6/aps/common/plot/qt_application.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/plotter.py` & `aps_common_libraries-1.0.6/aps/common/plotter.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/reflection.py` & `aps_common_libraries-1.0.6/aps/common/reflection.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/registry.py` & `aps_common_libraries-1.0.6/aps/common/registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/scripts/__init__.py` & `aps_common_libraries-1.0.6/aps/common/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/scripts/abstract_command_line_script.py` & `aps_common_libraries-1.0.6/aps/common/scripts/abstract_command_line_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/scripts/generic_process_manager.py` & `aps_common_libraries-1.0.6/aps/common/scripts/generic_process_manager.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/scripts/generic_qt_script.py` & `aps_common_libraries-1.0.6/aps/common/scripts/generic_qt_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/scripts/script_data.py` & `aps_common_libraries-1.0.6/aps/common/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/scripts/script_registry.py` & `aps_common_libraries-1.0.6/aps/common/scripts/script_registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/singleton.py` & `aps_common_libraries-1.0.6/aps/common/singleton.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/traffic_light.py` & `aps_common_libraries-1.0.6/aps/common/traffic_light.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/utilities.py` & `aps_common_libraries-1.0.6/aps/common/utilities.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/widgets/__init__.py` & `aps_common_libraries-1.0.6/aps/common/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/widgets/close_app_widget.py` & `aps_common_libraries-1.0.6/aps/common/widgets/close_app_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/widgets/context_widget.py` & `aps_common_libraries-1.0.6/aps/common/widgets/context_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/widgets/generic_widget.py` & `aps_common_libraries-1.0.6/aps/common/widgets/generic_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps/common/widgets/log_stream_widget.py` & `aps_common_libraries-1.0.6/aps/common/widgets/log_stream_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/aps_common_libraries.egg-info/PKG-INFO` & `aps_common_libraries-1.0.6/aps_common_libraries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aps-common-libraries
-Version: 1.0.5
+Version: 1.0.6
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
```

### Comparing `aps_common_libraries-1.0.5/aps_common_libraries.egg-info/SOURCES.txt` & `aps_common_libraries-1.0.6/aps_common_libraries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.5/setup.py` & `aps_common_libraries-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'aps_common_libraries'
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 ISRELEASED = False
 
 DESCRIPTION = 'APS Common Libraries'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
```

