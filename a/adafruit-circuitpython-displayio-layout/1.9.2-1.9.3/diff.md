# Comparing `tmp/adafruit-circuitpython-displayio-layout-1.9.2.tar.gz` & `tmp/adafruit-circuitpython-displayio-layout-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-displayio-layout-1.9.2.tar", last modified: Thu Apr 29 17:38:37 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-displayio-layout-1.9.3.tar", last modified: Mon May 31 19:31:38 2021, max compression
```

## Comparing `adafruit-circuitpython-displayio-layout-1.9.2.tar` & `adafruit-circuitpython-displayio-layout-1.9.3.tar`

### file list

```diff
@@ -1,94 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.257755 adafruit-circuitpython-displayio-layout-1.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.245755 adafruit-circuitpython-displayio-layout-1.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.245755 adafruit-circuitpython-displayio-layout-1.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.245755 adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/OFL-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-04-29 17:38:37.253755 adafruit-circuitpython-displayio-layout-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2407 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.245755 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_circuitpython_displayio_layout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-04-29 17:38:36.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_circuitpython_displayio_layout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2821 2021-04-29 17:38:37.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_circuitpython_displayio_layout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-29 17:38:36.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_circuitpython_displayio_layout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-04-29 17:38:36.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_circuitpython_displayio_layout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-04-29 17:38:36.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_circuitpython_displayio_layout.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.245755 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.245755 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/layouts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4435 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/layouts/grid_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.249755 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7337 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/annotation.py
--rw-r--r--   0 runner    (1001) docker     (121)    17187 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/cartesian.py
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/control.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    40783 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/dial.py
--rw-r--r--   0 runner    (1001) docker     (121)    10393 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/easing.py
--rw-r--r--   0 runner    (1001) docker     (121)    24309 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/flip_input.py
--rw-r--r--   0 runner    (1001) docker     (121)    12834 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/icon_animated.py
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/icon_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    39355 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/switch_round.py
--rw-r--r--   0 runner    (1001) docker     (121)    13303 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.253755 adafruit-circuitpython-displayio-layout-1.9.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.253755 adafruit-circuitpython-displayio-layout-1.9.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     4979 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/annotation_example.png
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/annotation_example.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian.gif
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian.gif.license
--rw-r--r--   0 runner    (1001) docker     (121)     5032 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian_explanation.png
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian_explanation.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian_zones.png
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian_zones.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     5629 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)   193259 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial.gif
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial.gif.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    71718 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_angles.png
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_angles.png.license
--rw-r--r--   0 runner    (1001) docker     (121)    67753 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_clip_needle.png
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_clip_needle.png.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    25030 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_min_max_values.png
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_min_max_values.png.license
--rwxr-xr-x   0 runner    (1001) docker     (121)    60800 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_ticks.png
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_ticks.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)   128416 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/gui_layout_coordinates.png
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/gui_layout_coordinates.png.license
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.253755 adafruit-circuitpython-displayio-layout-1.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_annotation_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_cartesian_advanced_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_cartesian_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_dial_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3624 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_flip_input_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_gridlayout_pygame_display_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_gridlayout_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_icon_animated_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1624 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3462 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_switch_multiple.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_switch_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.253755 adafruit-circuitpython-displayio-layout-1.9.2/examples/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (121)    41204 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/fonts/DSEG14Classic-Regular-64-ModS.pcf
--rw-r--r--   0 runner    (1001) docker     (121)       99 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/fonts/DSEG14Classic-Regular-64-ModS.pcf.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:38:37.253755 adafruit-circuitpython-displayio-layout-1.9.2/examples/icons/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1302 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/icons/Play_48x48_small.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/examples/icons/Play_48x48_small.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      342 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-29 17:38:37.257755 adafruit-circuitpython-displayio-layout-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2021-04-29 17:38:24.000000 adafruit-circuitpython-displayio-layout-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.389389 adafruit-circuitpython-displayio-layout-1.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.373389 adafruit-circuitpython-displayio-layout-1.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.377389 adafruit-circuitpython-displayio-layout-1.9.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.377389 adafruit-circuitpython-displayio-layout-1.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2510 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.377389 adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4695 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/OFL-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-05-31 19:31:38.389389 adafruit-circuitpython-displayio-layout-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2407 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.377389 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_circuitpython_displayio_layout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-05-31 19:31:38.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_circuitpython_displayio_layout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2937 2021-05-31 19:31:38.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_circuitpython_displayio_layout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-31 19:31:38.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_circuitpython_displayio_layout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-05-31 19:31:38.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_circuitpython_displayio_layout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2021-05-31 19:31:38.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_circuitpython_displayio_layout.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.377389 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.381389 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/layouts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4435 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/layouts/grid_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.381389 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/
+-rw-r--r--   0 runner    (1001) docker     (121)     1765 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7337 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17187 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3207 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/control.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    40783 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/dial.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10393 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/easing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24309 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/flip_input.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12834 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/icon_animated.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3427 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/icon_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39355 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/switch_round.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13303 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.385389 adafruit-circuitpython-displayio-layout-1.9.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.385389 adafruit-circuitpython-displayio-layout-1.9.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4979 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/annotation_example.png
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/annotation_example.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian.gif
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian.gif.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5032 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian_explanation.png
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian_explanation.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian_zones.png
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian_zones.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5629 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)   193259 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial.gif
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial.gif.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    71718 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_angles.png
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_angles.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)    67753 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_clip_needle.png
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_clip_needle.png.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    25030 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_min_max_values.png
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_min_max_values.png.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)    60800 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_ticks.png
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_ticks.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)   128416 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/gui_layout_coordinates.png
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/gui_layout_coordinates.png.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.385389 adafruit-circuitpython-displayio-layout-1.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_annotation_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_cartesian_advanced_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1343 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_cartesian_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_dial_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3624 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_flip_input_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_gridlayout_pygame_display_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_gridlayout_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1598 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_icon_animated_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1624 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3462 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_switch_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_switch_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.389389 adafruit-circuitpython-displayio-layout-1.9.3/examples/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)    41204 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/fonts/DSEG14Classic-Regular-64-ModS.pcf
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/fonts/DSEG14Classic-Regular-64-ModS.pcf.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-31 19:31:38.389389 adafruit-circuitpython-displayio-layout-1.9.3/examples/icons/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1302 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/icons/Play_48x48_small.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/examples/icons/Play_48x48_small.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-31 19:31:38.389389 adafruit-circuitpython-displayio-layout-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2434 2021-05-31 19:31:27.000000 adafruit-circuitpython-displayio-layout-1.9.3/setup.py
```

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/.github/workflows/build.yml` & `adafruit-circuitpython-displayio-layout-1.9.3/.github/workflows/build.yml`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.6
+    - name: Set up Python 3.7
       uses: actions/setup-python@v1
       with:
-        python-version: 3.6
+        python-version: 3.7
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
@@ -70,7 +70,9 @@
     - name: Build Python package
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
       run: |
         pip install --upgrade setuptools wheel twine readme_renderer testresources
         python setup.py sdist
         python setup.py bdist_wheel --universal
         twine check dist/*
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/.github/workflows/release.yml` & `adafruit-circuitpython-displayio-layout-1.9.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/.pre-commit-config.yaml` & `adafruit-circuitpython-displayio-layout-1.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/.pylintrc` & `adafruit-circuitpython-displayio-layout-1.9.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-displayio-layout-1.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/LICENSE` & `adafruit-circuitpython-displayio-layout-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/MIT.txt` & `adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/OFL-1.1.txt` & `adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/OFL-1.1.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-displayio-layout-1.9.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/PKG-INFO` & `adafruit-circuitpython-displayio-layout-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-layout
-Version: 1.9.2
+Version: 1.9.3
 Summary: CircuitPython helper library for displayio layouts and widgets.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_Layout
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/README.rst` & `adafruit-circuitpython-displayio-layout-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_circuitpython_displayio_layout.egg-info/PKG-INFO` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_circuitpython_displayio_layout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-layout
-Version: 1.9.2
+Version: 1.9.3
 Summary: CircuitPython helper library for displayio layouts and widgets.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_Layout
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_circuitpython_displayio_layout.egg-info/SOURCES.txt` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_circuitpython_displayio_layout.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
+.readthedocs.yml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 pyproject.toml
 requirements.txt
 setup.py
+.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
+.github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/OFL-1.1.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_displayio_layout.egg-info/PKG-INFO
 adafruit_circuitpython_displayio_layout.egg-info/SOURCES.txt
```

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/layouts/grid_layout.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/layouts/grid_layout.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/__init__.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/annotation.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/annotation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/cartesian.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/cartesian.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/control.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/control.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/dial.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/dial.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/easing.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/easing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/flip_input.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/flip_input.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/icon_animated.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/icon_animated.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/icon_widget.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/switch_round.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/switch_round.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/adafruit_displayio_layout/widgets/widget.py` & `adafruit-circuitpython-displayio-layout-1.9.3/adafruit_displayio_layout/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/_static/favicon.ico` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/annotation_example.png` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/annotation_example.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/api.rst` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian.gif` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian.gif`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian_explanation.png` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian_explanation.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/cartesian_zones.png` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/cartesian_zones.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/conf.py` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/dial.gif` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/dial.gif`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_angles.png` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_angles.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_clip_needle.png` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_clip_needle.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_min_max_values.png` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_min_max_values.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/dial_variables_ticks.png` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/dial_variables_ticks.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/examples.rst` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/gui_layout_coordinates.png` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/gui_layout_coordinates.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/docs/index.rst` & `adafruit-circuitpython-displayio-layout-1.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_annotation_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_annotation_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_cartesian_advanced_test.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_cartesian_advanced_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_cartesian_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_cartesian_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_dial_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_dial_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_flip_input_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_flip_input_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_gridlayout_pygame_display_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_gridlayout_pygame_display_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_gridlayout_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_gridlayout_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_icon_animated_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_icon_animated_simpletest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # SPDX-FileCopyrightText: 2021 Kevin Matocha
 #
 # SPDX-License-Identifier: MIT
 """
 Creates two animated icons with touch response: zoom and shrink animations.
 """
-import gc
 import time
 import board
 import displayio
 import adafruit_touchscreen
 from adafruit_displayio_layout.widgets.icon_animated import IconAnimated
 
 display = board.DISPLAY
```

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_switch_multiple.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_switch_multiple.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/displayio_layout_switch_simpletest.py` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/displayio_layout_switch_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/fonts/DSEG14Classic-Regular-64-ModS.pcf` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/fonts/DSEG14Classic-Regular-64-ModS.pcf`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/examples/icons/Play_48x48_small.bmp` & `adafruit-circuitpython-displayio-layout-1.9.3/examples/icons/Play_48x48_small.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-layout-1.9.2/setup.py` & `adafruit-circuitpython-displayio-layout-1.9.3/setup.py`

 * *Files identical despite different names*

