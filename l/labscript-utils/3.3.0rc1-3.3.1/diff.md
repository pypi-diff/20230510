# Comparing `tmp/labscript-utils-3.3.0rc1.tar.gz` & `tmp/labscript-utils-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labscript-utils-3.3.0rc1.tar", last modified: Thu Apr 13 17:18:07 2023, max compression
+gzip compressed data, was "labscript-utils-3.3.1.tar", last modified: Wed May 10 00:11:15 2023, max compression
```

## Comparing `labscript-utils-3.3.0rc1.tar` & `labscript-utils-3.3.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.889528 labscript-utils-3.3.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.865528 labscript-utils-3.3.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.869528 labscript-utils-3.3.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/BSD-2-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/BSD-3-CLAUSE-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-13 17:18:07.889528 labscript-utils-3.3.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/_templates/autosummary-class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/_templates/autosummary-module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/_templates/components.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.873528 labscript-utils-3.3.0rc1/docs/source/img/
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/blacs_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46681 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/labscript.ico
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/labscript_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/labscript_64x64.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/lyse_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/runmanager_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/img/runviewer_32nx32n.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/labconfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/docs/source/pyqt5-modified-objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript-suite.pth
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.869528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/app_saved_configs/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/app_saved_configs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/labconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/labconfig/example.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.869528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/example_IMAQdx_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table_IMAQdx_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_IMAQdx_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/pythonlib/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/pythonlib/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.877528 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/user_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/user_devices/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.881528 labscript-utils-3.3.0rc1/labscript_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/camera_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/connections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.885528 labscript-utils-3.3.0rc1/labscript_utils/device_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/device_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/device_registry/_device_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/dict_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/double_import_denier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.885528 labscript-utils-3.3.0rc1/labscript_utils/excepthook/
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/excepthook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/excepthook/error.gif
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/excepthook/tk_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/filewatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/h5_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/impprof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/labconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/ls_zprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/memprof.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/modulewatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.885528 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/InputPlotWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/analoginput.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/analogoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/ddsoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/digitaloutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    36434 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/dragdroptab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/elide_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/enumoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/fingertab.py
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/headerview_with_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/imageoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/outputbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    21502 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/toolpalette.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/setup_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/shared_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/shot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/splash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/tracelog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.889528 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/NovaTechDDS9m.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/UnitConversionBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/aom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/detuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/generic_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/linear_coil_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/optotunelens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/quad_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/quad_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/unitconversions/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/zlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/labscript_utils/zlog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:18:07.885528 labscript-utils-3.3.0rc1/labscript_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 17:18:07.000000 labscript-utils-3.3.0rc1/labscript_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-13 17:18:07.889528 labscript-utils-3.3.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 17:17:52.000000 labscript-utils-3.3.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.196653 labscript-utils-3.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.148653 labscript-utils-3.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.160653 labscript-utils-3.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/BSD-2-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/BSD-3-CLAUSE-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-10 00:11:15.196653 labscript-utils-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.164653 labscript-utils-3.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.164653 labscript-utils-3.3.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.164653 labscript-utils-3.3.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.164653 labscript-utils-3.3.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/_templates/autosummary-class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/_templates/autosummary-module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/_templates/components.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.164653 labscript-utils-3.3.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.168653 labscript-utils-3.3.1/docs/source/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/img/blacs_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46681 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98716 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/img/labscript.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/img/labscript_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/img/labscript_64x64.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/img/lyse_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/img/runmanager_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/img/runviewer_32nx32n.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/labconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64143 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/docs/source/pyqt5-modified-objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript-suite.pth
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.168653 labscript-utils-3.3.1/labscript_profile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.152653 labscript-utils-3.3.1/labscript_profile/default_profile/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.172653 labscript-utils-3.3.1/labscript_profile/default_profile/app_saved_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/app_saved_configs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.172653 labscript-utils-3.3.1/labscript_profile/default_profile/labconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/labconfig/example.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.156653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.172653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/analysislib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/analysislib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.172653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/analysislib/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/analysislib/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.172653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/example_IMAQdx_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.172653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.172653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.176653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table_IMAQdx_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_IMAQdx_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.176653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/pythonlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/pythonlib/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.176653 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/user_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_profile/default_profile/userlib/user_devices/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.184653 labscript-utils-3.3.1/labscript_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/camera_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/connections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.188653 labscript-utils-3.3.1/labscript_utils/device_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/device_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/device_registry/_device_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/dict_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/double_import_denier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.188653 labscript-utils-3.3.1/labscript_utils/excepthook/
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/excepthook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/excepthook/error.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/excepthook/tk_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/filewatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/h5_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/impprof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/labconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15266 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/ls_zprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/memprof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/modulewatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.196653 labscript-utils-3.3.1/labscript_utils/qtwidgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/InputPlotWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5511 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/analoginput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/analogoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/ddsoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/digitaloutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36434 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/dragdroptab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/elide_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/enumoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/fingertab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/headerview_with_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/imageoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/outputbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21502 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/qtwidgets/toolpalette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/setup_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/shared_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/shot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/splash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/tracelog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.196653 labscript-utils-3.3.1/labscript_utils/unitconversions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/NovaTechDDS9m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/UnitConversionBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/aom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/detuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/generic_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/linear_coil_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/optotunelens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/quad_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/quad_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/unitconversions/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/zlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/labscript_utils/zlog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 00:11:15.188653 labscript-utils-3.3.1/labscript_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-10 00:11:15.000000 labscript-utils-3.3.1/labscript_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-10 00:11:15.000000 labscript-utils-3.3.1/labscript_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:11:15.000000 labscript-utils-3.3.1/labscript_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 00:11:15.000000 labscript-utils-3.3.1/labscript_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 00:11:14.000000 labscript-utils-3.3.1/labscript_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-10 00:11:15.000000 labscript-utils-3.3.1/labscript_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 00:11:15.000000 labscript-utils-3.3.1/labscript_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-10 00:11:15.196653 labscript-utils-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-10 00:11:00.000000 labscript-utils-3.3.1/setup.py
```

### Comparing `labscript-utils-3.3.0rc1/.github/workflows/release.yml` & `labscript-utils-3.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/.gitignore` & `labscript-utils-3.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/BSD-2-CLAUSE-LICENSE.txt` & `labscript-utils-3.3.1/BSD-2-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/BSD-3-CLAUSE-LICENSE.txt` & `labscript-utils-3.3.1/BSD-3-CLAUSE-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/LICENSE.txt` & `labscript-utils-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/NEWS.md` & `labscript-utils-3.3.1/NEWS.md`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/PKG-INFO` & `labscript-utils-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript-utils
-Version: 3.3.0rc1
+Version: 3.3.1
 Summary: Shared utilities for the labscript suite
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-utils
 Project-URL: Download, https://github.com/labscript-suite/labscript-utils/releases
```

### Comparing `labscript-utils-3.3.0rc1/README.md` & `labscript-utils-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/Makefile` & `labscript-utils-3.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/make.bat` & `labscript-utils-3.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/_static/custom.css` & `labscript-utils-3.3.1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/_templates/autosummary-class.rst` & `labscript-utils-3.3.1/docs/source/_templates/autosummary-class.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/_templates/autosummary-module.rst` & `labscript-utils-3.3.1/docs/source/_templates/autosummary-module.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/_templates/components.rst` & `labscript-utils-3.3.1/docs/source/_templates/components.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/conf.py` & `labscript-utils-3.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/img/blacs_32nx32n.svg` & `labscript-utils-3.3.1/docs/source/img/blacs_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg` & `labscript-utils-3.3.1/docs/source/img/labscript-suite-rectangular-transparent_138nx70n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/img/labscript.ico` & `labscript-utils-3.3.1/docs/source/img/labscript.ico`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/img/labscript_32nx32n.svg` & `labscript-utils-3.3.1/docs/source/img/labscript_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/img/labscript_64x64.svg` & `labscript-utils-3.3.1/docs/source/img/labscript_64x64.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/img/lyse_32nx32n.svg` & `labscript-utils-3.3.1/docs/source/img/lyse_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/img/runmanager_32nx32n.svg` & `labscript-utils-3.3.1/docs/source/img/runmanager_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/img/runviewer_32nx32n.svg` & `labscript-utils-3.3.1/docs/source/img/runviewer_32nx32n.svg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/index.rst` & `labscript-utils-3.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/labconfig.rst` & `labscript-utils-3.3.1/docs/source/labconfig.rst`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/docs/source/pyqt5-modified-objects.inv` & `labscript-utils-3.3.1/docs/source/pyqt5-modified-objects.inv`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/__init__.py` & `labscript-utils-3.3.1/labscript_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/create.py` & `labscript-utils-3.3.1/labscript_profile/create.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/default_profile/labconfig/example.ini` & `labscript-utils-3.3.1/labscript_profile/default_profile/labconfig/example.ini`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/example_IMAQdx_remote.py` & `labscript-utils-3.3.1/labscript_profile/default_profile/userlib/analysislib/example_apparatus/example_IMAQdx_remote.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table.py` & `labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table_IMAQdx_remote.py` & `labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/connection_table_IMAQdx_remote.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_IMAQdx_remote.py` & `labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_IMAQdx_remote.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_experiment.py` & `labscript-utils-3.3.1/labscript_profile/default_profile/userlib/labscriptlib/example_apparatus/example_experiment.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_profile/default_profile/userlib/user_devices/README.txt` & `labscript-utils-3.3.1/labscript_profile/default_profile/userlib/user_devices/README.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/__init__.py` & `labscript-utils-3.3.1/labscript_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/camera_server.py` & `labscript-utils-3.3.1/labscript_utils/camera_server.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/connections.py` & `labscript-utils-3.3.1/labscript_utils/connections.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/device_registry/__init__.py` & `labscript-utils-3.3.1/labscript_utils/device_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/device_registry/_device_registry.py` & `labscript-utils-3.3.1/labscript_utils/device_registry/_device_registry.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/dict_diff.py` & `labscript-utils-3.3.1/labscript_utils/dict_diff.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/double_import_denier.py` & `labscript-utils-3.3.1/labscript_utils/double_import_denier.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/excepthook/__init__.py` & `labscript-utils-3.3.1/labscript_utils/excepthook/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/excepthook/error.gif` & `labscript-utils-3.3.1/labscript_utils/excepthook/error.gif`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/excepthook/tk_exception.py` & `labscript-utils-3.3.1/labscript_utils/excepthook/tk_exception.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/filewatcher.py` & `labscript-utils-3.3.1/labscript_utils/filewatcher.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/h5_lock.py` & `labscript-utils-3.3.1/labscript_utils/h5_lock.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/impprof.py` & `labscript-utils-3.3.1/labscript_utils/impprof.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/labconfig.py` & `labscript-utils-3.3.1/labscript_utils/labconfig.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/ls_zprocess.py` & `labscript-utils-3.3.1/labscript_utils/ls_zprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 from socket import gethostbyname
 from packaging.version import Version
 import zmq
 
 import zprocess
 import zprocess.process_tree
-from zprocess.security import SecureContext
+from zprocess.security import SecureContext, SecureSocket
 from labscript_utils.labconfig import LabConfig
 from labscript_utils import dedent
 import zprocess.zlog
 import zprocess.zlock
 import zprocess.remote
 from zprocess import KillLock
 
@@ -244,18 +244,27 @@
 
     @classmethod
     def instance(cls):
         config = get_config()
         # Super required to call unbound class method of parent class:
         return super(Context, cls).instance(shared_secret=config['shared_secret'])
 
-    def socket(self, *args, **kwargs):
-        config = get_config()
-        kwargs['allow_insecure'] = config['allow_insecure']
-        return SecureContext.socket(self, *args, **kwargs)
+    def socket(self, socket_type, socket_class=None, **kwargs):
+        # socket_class kwarg introduced in pyzmq 25. Pass it through if it was given,
+        # otherwise don't.
+        if socket_class is not None:
+            kwargs['socket_class'] = socket_class
+        # Only insert our security-related args to the socket if we know it's going to
+        # be a SecureSocket. If caller has explicitly requested a different socket type
+        # (e.g since pyzmq 25, ThreadAuthenticator sets up an internal socket by calling
+        # `Context.socket(..., socket_class=zmq.Socket)), then don't.`
+        if socket_class is None or issubclass(socket_class, SecureContext):
+            config = get_config()
+            kwargs['allow_insecure'] = config['allow_insecure']
+        return SecureContext.socket(self, socket_type=socket_type, **kwargs)
 
 
 def Lock(*args, **kwargs):
     if 'read_only' in kwargs and not _zlock_server_supports_readwrite:
         # Ignore read_only argument if the server does not support it:
         del kwargs['read_only']
     return ProcessTree.instance().lock(*args, **kwargs)
```

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/memprof.py` & `labscript-utils-3.3.1/labscript_utils/memprof.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/modulewatcher.py` & `labscript-utils-3.3.1/labscript_utils/modulewatcher.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/properties.py` & `labscript-utils-3.3.1/labscript_utils/properties.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/InputPlotWindow.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/InputPlotWindow.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/__init__.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/analoginput.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/analoginput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/analogoutput.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/analogoutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/ddsoutput.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/ddsoutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/digitaloutput.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/digitaloutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/dragdroptab.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/dragdroptab.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/elide_label.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/elide_label.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/enumoutput.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/enumoutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/fingertab.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/fingertab.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/headerview_with_widgets.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/headerview_with_widgets.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/imageoutput.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/imageoutput.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/outputbox.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/outputbox.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/qtwidgets/toolpalette.py` & `labscript-utils-3.3.1/labscript_utils/qtwidgets/toolpalette.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/remote.py` & `labscript-utils-3.3.1/labscript_utils/remote.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/settings.py` & `labscript-utils-3.3.1/labscript_utils/settings.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/setup_logging.py` & `labscript-utils-3.3.1/labscript_utils/setup_logging.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/shared_drive.py` & `labscript-utils-3.3.1/labscript_utils/shared_drive.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/shot_utils.py` & `labscript-utils-3.3.1/labscript_utils/shot_utils.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/splash.py` & `labscript-utils-3.3.1/labscript_utils/splash.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,23 @@
                 python -m labscript_utils.winshell --fix-shortcuts."""
         raise ImportError(dedent(msg))
     raise
     
 Qt = QtCore.Qt
 
 
+# Set auto high-DPI scaling - this ensures pixel metrics are scaled
+# appropriately so that we don't get a weird mix of large fonts and small
+# everything else on High DPI displays:
+QtWidgets.QApplication.setAttribute(Qt.AA_EnableHighDpiScaling, True)
+# Use high res pixmaps if available, instead of rendering at low resolution and
+# upscaling:
+QtWidgets.QApplication.setAttribute(Qt.AA_UseHighDpiPixmaps, True)
+
+
 class Splash(QtWidgets.QFrame):
     w = 250
     h = 230
     imwidth = 150
     imheight = 150
     alpha = 0.875
     icon_frac = 0.65
```

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/testing_utils.py` & `labscript-utils-3.3.1/labscript_utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/tracelog.py` & `labscript-utils-3.3.1/labscript_utils/tracelog.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/NovaTechDDS9m.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/NovaTechDDS9m.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/UnitConversionBase.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/UnitConversionBase.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/__init__.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/__init__.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/aom.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/aom.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/detuning.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/detuning.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/example.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/example.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/generic_frequency.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/generic_frequency.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/linear_coil_driver.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/linear_coil_driver.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/optotunelens.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/optotunelens.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/quad_driver.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/quad_driver.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/quad_monitor.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/quad_monitor.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/unitconversions/test.py` & `labscript-utils-3.3.1/labscript_utils/unitconversions/test.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/versions.py` & `labscript-utils-3.3.1/labscript_utils/versions.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/zlock.py` & `labscript-utils-3.3.1/labscript_utils/zlock.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils/zlog.py` & `labscript-utils-3.3.1/labscript_utils/zlog.py`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/labscript_utils.egg-info/PKG-INFO` & `labscript-utils-3.3.1/labscript_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labscript-utils
-Version: 3.3.0rc1
+Version: 3.3.1
 Summary: Shared utilities for the labscript suite
 Home-page: http://labscriptsuite.org
 Author: The labscript suite community
 Author-email: labscriptsuite@googlegroups.com
 License: BSD
 Project-URL: Source Code, https://github.com/labscript-suite/labscript-utils
 Project-URL: Download, https://github.com/labscript-suite/labscript-utils/releases
```

### Comparing `labscript-utils-3.3.0rc1/labscript_utils.egg-info/SOURCES.txt` & `labscript-utils-3.3.1/labscript_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/readthedocs.yaml` & `labscript-utils-3.3.1/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/setup.cfg` & `labscript-utils-3.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `labscript-utils-3.3.0rc1/setup.py` & `labscript-utils-3.3.1/setup.py`

 * *Files identical despite different names*

