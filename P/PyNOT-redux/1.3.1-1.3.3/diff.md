# Comparing `tmp/PyNOT-redux-1.3.1.tar.gz` & `tmp/PyNOT-redux-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNOT-redux-1.3.1.tar", last modified: Tue May  9 07:53:04 2023, max compression
+gzip compressed data, was "PyNOT-redux-1.3.3.tar", last modified: Wed May 10 07:23:45 2023, max compression
```

## Comparing `PyNOT-redux-1.3.1.tar` & `PyNOT-redux-1.3.3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.928146 PyNOT-redux-1.3.1/
--rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-05-07 20:58:18.000000 PyNOT-redux-1.3.1/.DS_Store
--rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/.gitattributes
--rw-r--r--   0 krogager   (501) staff       (20)     1898 2023-05-09 07:51:28.000000 PyNOT-redux-1.3.1/.gitignore
--rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/LICENSE
--rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/MANIFEST.in
--rw-r--r--   0 krogager   (501) staff       (20)    13890 2023-05-09 07:53:04.927996 PyNOT-redux-1.3.1/PKG-INFO
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.913170 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/
--rw-r--r--   0 krogager   (501) staff       (20)    13890 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/SOURCES.txt
--rw-r--r--   0 krogager   (501) staff       (20)        1 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/dependency_links.txt
--rw-r--r--   0 krogager   (501) staff       (20)       42 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/entry_points.txt
--rw-r--r--   0 krogager   (501) staff       (20)      113 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/requires.txt
--rw-r--r--   0 krogager   (501) staff       (20)        6 2023-05-09 07:53:04.000000 PyNOT-redux-1.3.1/PyNOT_redux.egg-info/top_level.txt
--rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/README.md
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.921216 PyNOT-redux-1.3.1/pynot/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/.extract_msg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/.identify_msg
--rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.3.1/pynot/.instrument.cfg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/.response_msg
--rw-r--r--   0 krogager   (501) staff       (20)        6 2023-05-09 07:51:38.000000 PyNOT-redux-1.3.1/pynot/VERSION
--rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.3.1/pynot/alfosc.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.923966 PyNOT-redux-1.3.1/pynot/calib/
--rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/HeAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/HeNe_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ThAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/al-gr18_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/al-gr19_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/al-gr4_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/al-gr7_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/alfosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/default_options.yml
--rw-r--r--   0 krogager   (501) staff       (20)     3751 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.1/pynot/calib/default_options_img.yml
--rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ef-gr13_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ef-gr14_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ef-gr1_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/ef-gr3_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/efosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/lapalma.ext
--rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/lasilla.ext
--rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/paranal.ext
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.926647 PyNOT-redux-1.3.1/pynot/calib/std/
--rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/bd174708.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/bd262606.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/bd332642.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/bd75325.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/eg21.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/feige110.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/feige34.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/gd153.dat
--rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/gd50.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/gd71.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/hd19445.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/hd84937.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/hd93521.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/he3.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/hiltner600.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/ltt3864.dat
--rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/tcs_namelist.txt
--rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/calib/std/wolf1346.dat
--rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.3.1/pynot/calibs.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.927325 PyNOT-redux-1.3.1/pynot/data/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/alfosc.rules
--rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/efosc.rules
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-09 07:53:04.927772 PyNOT-redux-1.3.1/pynot/data/help/
--rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_extract.html
--rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_identify.html
--rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_response.html
--rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/io.py
--rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/obs.py
--rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/data/organizer.py
--rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.3.1/pynot/efosc.py
--rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.3.1/pynot/extract_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.3.1/pynot/extraction.py
--rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.1/pynot/fitsio.py
--rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/functions.py
--rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.3.1/pynot/identify_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.3.1/pynot/insconfig.py
--rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/logging.py
--rw-r--r--   0 krogager   (501) staff       (20)    47613 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.1/pynot/main.py
--rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.3.1/pynot/phot.py
--rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/phot_redux.py
--rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.3.1/pynot/redux.py
--rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/reports.py
--rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/response.py
--rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/response_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.3.1/pynot/scired.py
--rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.1/pynot/scombine.py
--rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/tasks.py
--rw-r--r--   0 krogager   (501) staff       (20)     9913 2023-04-25 14:38:05.000000 PyNOT-redux-1.3.1/pynot/transients.py
--rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.1/pynot/txtio.py
--rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/wavecal.py
--rw-r--r--   0 krogager   (501) staff       (20)    13346 2023-05-09 07:51:11.000000 PyNOT-redux-1.3.1/pynot/wcs.py
--rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pynot/welcome.py
--rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.1/pyproject.toml
--rw-r--r--   0 krogager   (501) staff       (20)       38 2023-05-09 07:53:04.928182 PyNOT-redux-1.3.1/setup.cfg
--rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.3.1/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.767178 PyNOT-redux-1.3.3/
+-rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-05-07 20:58:18.000000 PyNOT-redux-1.3.3/.DS_Store
+-rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/.gitattributes
+-rw-r--r--   0 krogager   (501) staff       (20)     1898 2023-05-09 07:51:28.000000 PyNOT-redux-1.3.3/.gitignore
+-rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/LICENSE
+-rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/MANIFEST.in
+-rw-r--r--   0 krogager   (501) staff       (20)    13890 2023-05-10 07:23:45.766965 PyNOT-redux-1.3.3/PKG-INFO
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.752210 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/
+-rw-r--r--   0 krogager   (501) staff       (20)    13890 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/SOURCES.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        1 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/dependency_links.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       42 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/entry_points.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      113 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/requires.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        6 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/top_level.txt
+-rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/README.md
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.760118 PyNOT-redux-1.3.3/pynot/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/.extract_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/.identify_msg
+-rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.3.3/pynot/.instrument.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/.response_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        6 2023-05-10 07:22:14.000000 PyNOT-redux-1.3.3/pynot/VERSION
+-rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.3.3/pynot/alfosc.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.762767 PyNOT-redux-1.3.3/pynot/calib/
+-rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/HeAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/HeNe_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ThAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/al-gr18_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/al-gr19_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/al-gr4_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/al-gr7_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/alfosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/default_options.yml
+-rw-r--r--   0 krogager   (501) staff       (20)     3827 2023-05-10 07:21:25.000000 PyNOT-redux-1.3.3/pynot/calib/default_options_img.yml
+-rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ef-gr13_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ef-gr14_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ef-gr1_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ef-gr3_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/efosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/lapalma.ext
+-rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/lasilla.ext
+-rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/paranal.ext
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.765610 PyNOT-redux-1.3.3/pynot/calib/std/
+-rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/bd174708.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/bd262606.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/bd332642.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/bd75325.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/eg21.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/feige110.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/feige34.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/gd153.dat
+-rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/gd50.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/gd71.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/hd19445.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/hd84937.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/hd93521.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/he3.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/hiltner600.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/ltt3864.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/tcs_namelist.txt
+-rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/wolf1346.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.3.3/pynot/calibs.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.766326 PyNOT-redux-1.3.3/pynot/data/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/alfosc.rules
+-rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/efosc.rules
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.766764 PyNOT-redux-1.3.3/pynot/data/help/
+-rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_extract.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_identify.html
+-rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_response.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/io.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/obs.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/organizer.py
+-rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.3.3/pynot/efosc.py
+-rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.3.3/pynot/extract_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.3.3/pynot/extraction.py
+-rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.3/pynot/fitsio.py
+-rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/functions.py
+-rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.3.3/pynot/identify_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.3.3/pynot/insconfig.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/logging.py
+-rw-r--r--   0 krogager   (501) staff       (20)    47613 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.3/pynot/main.py
+-rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.3.3/pynot/phot.py
+-rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/phot_redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.3.3/pynot/redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/reports.py
+-rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/response.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/response_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.3.3/pynot/scired.py
+-rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.3/pynot/scombine.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/tasks.py
+-rw-r--r--   0 krogager   (501) staff       (20)     9913 2023-04-25 14:38:05.000000 PyNOT-redux-1.3.3/pynot/transients.py
+-rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.3/pynot/txtio.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/wavecal.py
+-rw-r--r--   0 krogager   (501) staff       (20)    13619 2023-05-10 07:20:54.000000 PyNOT-redux-1.3.3/pynot/wcs.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/welcome.py
+-rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pyproject.toml
+-rw-r--r--   0 krogager   (501) staff       (20)       38 2023-05-10 07:23:45.767213 PyNOT-redux-1.3.3/setup.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.3.3/setup.py
```

### Comparing `PyNOT-redux-1.3.1/.DS_Store` & `PyNOT-redux-1.3.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/.gitignore` & `PyNOT-redux-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/LICENSE` & `PyNOT-redux-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/PKG-INFO` & `PyNOT-redux-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.3.1
+Version: 1.3.3
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyNOT-redux-1.3.1/PyNOT_redux.egg-info/PKG-INFO` & `PyNOT-redux-1.3.3/PyNOT_redux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.3.1
+Version: 1.3.3
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyNOT-redux-1.3.1/PyNOT_redux.egg-info/SOURCES.txt` & `PyNOT-redux-1.3.3/PyNOT_redux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/README.md` & `PyNOT-redux-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/__init__.py` & `PyNOT-redux-1.3.3/pynot/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/alfosc.py` & `PyNOT-redux-1.3.3/pynot/alfosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/HeAr_linelist.dat` & `PyNOT-redux-1.3.3/pynot/calib/HeAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/HeNe_linelist.dat` & `PyNOT-redux-1.3.3/pynot/calib/HeNe_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/ThAr_linelist.dat` & `PyNOT-redux-1.3.3/pynot/calib/ThAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/alfosc_filters.dat` & `PyNOT-redux-1.3.3/pynot/calib/alfosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/default_options.yml` & `PyNOT-redux-1.3.3/pynot/calib/default_options.yml`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/default_options_img.yml` & `PyNOT-redux-1.3.3/pynot/calib/default_options_img.yml`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,17 @@
   deblend_cont:     0.005    # Minimum contrast ratio used for object deblending. Disable deblending by setting to 1.0
   clean:            True     # Perform cleaning?
   clean_param:      1.0      # Cleaning parameter (see SExtractor manual)
   segmentation_map: True     # Create a segmentation map?
 
 wcs:
   min_num:          6        # Minimum number of targets required.
-  G_lim:            15       # Bright limit of Gaia sources. Reject targets brighter than G < G_lim
+  G_lim:            5        # Bright limit of Gaia sources. Reject targets brighter than G < G_lim
   q_lim:            0.8      # Reject elliptical sources with axis ratio < `q_lim`
   p_kde:            0.5      # Probability threshold for projected vector filtering.
   kde_factor:       0.1      # Smoothing scale for the Gaussian kernel density estimator.
+  plot:             False    # Make a diagnostic plot of the WCS alignment?
 
 sdss_flux:
   q_lim:            0.8      # Reject elliptical sources with axis ratio < `q_lim`
   kappa:              3      # Threshold for magnitude filtering.
   match_radius:       1      # Matching radius in arcsec for source catalog and SDSS catalog
```

### Comparing `PyNOT-redux-1.3.1/pynot/calib/efosc_filters.dat` & `PyNOT-redux-1.3.3/pynot/calib/efosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/lapalma.ext` & `PyNOT-redux-1.3.3/pynot/calib/lapalma.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/lasilla.ext` & `PyNOT-redux-1.3.3/pynot/calib/lasilla.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/paranal.ext` & `PyNOT-redux-1.3.3/pynot/calib/paranal.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/bd174708.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/bd174708.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/bd262606.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/bd262606.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/bd332642.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/bd332642.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/bd75325.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/bd75325.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/eg21.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/eg21.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/feige110.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/feige110.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/feige34.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/feige34.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/gd153.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/gd153.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/gd50.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/gd50.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/gd71.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/gd71.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/hd19445.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/hd19445.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/hd84937.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/hd84937.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/hd93521.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/hd93521.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/he3.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/he3.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/hiltner600.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/ltt3864.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/ltt3864.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calib/std/wolf1346.dat` & `PyNOT-redux-1.3.3/pynot/calib/std/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/calibs.py` & `PyNOT-redux-1.3.3/pynot/calibs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/data/alfosc.rules` & `PyNOT-redux-1.3.3/pynot/data/alfosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/data/efosc.rules` & `PyNOT-redux-1.3.3/pynot/data/efosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_extract.html` & `PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_extract.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_identify.html` & `PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_identify.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/data/help/welcome_msg_response.html` & `PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_response.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/data/io.py` & `PyNOT-redux-1.3.3/pynot/data/io.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/data/obs.py` & `PyNOT-redux-1.3.3/pynot/data/obs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/data/organizer.py` & `PyNOT-redux-1.3.3/pynot/data/organizer.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/efosc.py` & `PyNOT-redux-1.3.3/pynot/efosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/extract_gui.py` & `PyNOT-redux-1.3.3/pynot/extract_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/extraction.py` & `PyNOT-redux-1.3.3/pynot/extraction.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/fitsio.py` & `PyNOT-redux-1.3.3/pynot/fitsio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/functions.py` & `PyNOT-redux-1.3.3/pynot/functions.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/identify_gui.py` & `PyNOT-redux-1.3.3/pynot/identify_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/insconfig.py` & `PyNOT-redux-1.3.3/pynot/insconfig.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/logging.py` & `PyNOT-redux-1.3.3/pynot/logging.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/main.py` & `PyNOT-redux-1.3.3/pynot/main.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/phot.py` & `PyNOT-redux-1.3.3/pynot/phot.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/phot_redux.py` & `PyNOT-redux-1.3.3/pynot/phot_redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/redux.py` & `PyNOT-redux-1.3.3/pynot/redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/reports.py` & `PyNOT-redux-1.3.3/pynot/reports.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/response.py` & `PyNOT-redux-1.3.3/pynot/response.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/response_gui.py` & `PyNOT-redux-1.3.3/pynot/response_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/scired.py` & `PyNOT-redux-1.3.3/pynot/scired.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/scombine.py` & `PyNOT-redux-1.3.3/pynot/scombine.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/tasks.py` & `PyNOT-redux-1.3.3/pynot/tasks.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/transients.py` & `PyNOT-redux-1.3.3/pynot/transients.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/txtio.py` & `PyNOT-redux-1.3.3/pynot/txtio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/wavecal.py` & `PyNOT-redux-1.3.3/pynot/wavecal.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/pynot/wcs.py` & `PyNOT-redux-1.3.3/pynot/wcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,16 @@
                                 output_file=catalog_fname)
     result = job.get_results()
     return result
 
 
 
 
-def correct_wcs(img_fname, sep_fname, output='', fig_fname='', min_num=6, G_lim=15, q_lim=0.8, kde_factor=0.1,
-                p_kde=0.5, debug=False):
+def correct_wcs(img_fname, sep_fname, output='', fig_fname='', min_num=6, G_lim=5, q_lim=0.8, kde_factor=0.1,
+                p_kde=0.5, debug=False, plot=False):
     """
     WCS calibration using Gaia
 
     Sources are matched using the initial WCS solution from the header. Outliers are rejected
     based on projected distance. The WCS solution is then matched to match the Gaia positions.
 
     Parameters
@@ -121,15 +121,15 @@
 
     fig_fname : string
         Filename of the diagnostic figure. Autogenerated by default.
 
     min_num : int  [default=6]
         Minimum number of targets required.
 
-    G_lim : float  [default=15]
+    G_lim : float  [default=5]
         Bright limit of Gaia sources. Reject targets brighter than G < G_lim as these are
         very likely saturated in the ALFOSC image.
 
     q_lim : float  [default=0.8]
         Reject elliptical sources with axis ratio < `q_lim`.
         Axis ratio is defined as minor/major.
 
@@ -137,14 +137,17 @@
         Smoothing factor for the kernel density estimator used for source filtering
         in the distance-orientation space.
     
     p_kde : float  [default=0.5]
         Threshold for projected vector filtering. The clustering of sources in the distance-orientation space
         is estimated using a kernel density estimator with a smoothing scale of `kde_factor`.
         A given source is rejected if its KDE probability is less than this threshold.
+    
+    plot : bool  [default=False]
+        Plot a diagnostic plot of the identified sources after WCS alignment?
 
     Returns
     -------
     output_msg : string
         Log of messages from the function call.
     """
     msg = list()
@@ -260,16 +263,16 @@
         peak_theta = y[peak[0]]
         plt.contourf(xx, yy, pdf, cmap='Blues')
         plt.contour(xx, yy, pdf, [p_kde, 1.0], colors=['r', 'r'])
         plt.plot(dist, theta, 'k+')
         plt.plot(dist[mask], theta[mask], 'ro', alpha=0.5)
         plt.axvline(peak_dist, color='r', ls=':', alpha=0.5)
         plt.axhline(peak_theta, color='r', ls=':', alpha=0.5)
-        plt.xlabel("Source distance (arcsec)")
-        plt.ylabel("Source orientation, $\\theta$ (radians)")
+        plt.xlabel("Offset (arcsec)")
+        plt.ylabel("Offset orientation, $\\theta$ (radians)")
         plt.show()
     
     matched_sep = matched_sep[mask]
     matched_ref = matched_ref[mask]
 
     if np.sum(mask) < min_num:
         msg.append(" [ERROR]  - Not enough targets found in the image!")
@@ -284,33 +287,34 @@
     hdr.update(wcs_keys)
     hdr.add_comment("PyNOT: WCS calibration using Gaia %s" % gaia_dr.upper())
     hdr['RADESYSa'] = 'ICRS'
     msg.append("          - Updating WCS information")
 
 
     # -- Plot solution:
-    plt.close('all')
-    warnings.simplefilter('ignore', category=AstropyWarning)
-    wcs_new = WCS(hdr)
-    fig = plt.figure()
-    ax = fig.add_subplot(111, projection=wcs_new)
-    med_val = np.median(img)
-    ax.imshow(img, vmin=med_val-1*mad(img), vmax=med_val+10*mad(img),
-              origin='lower', cmap=plt.cm.gray_r)
-    ax.scatter(matched_ref[:, 0], matched_ref[:, 1],
-               transform=ax.get_transform('fk5'), edgecolor='r', facecolor='none', s=50)
-    if debug:
-        ax.scatter(matched_sep[:, 0], matched_sep[:, 1],
-                   transform=ax.get_transform('fk5'), edgecolor='green', facecolor='none', s=10, alpha=0.7)
-        for i, r in zip(matched_sep, matched_ref):
-            ax.plot([i[0], r[0]], [i[1], r[1]], 'k', alpha=0.5, transform=ax.get_transform('fk5'))
-    ax.set_xlabel("Right Ascension")
-    ax.set_ylabel("Declination")
-    fig.savefig(fig_fname)
-    msg.append(" [OUTPUT] - Saving WCS solution figure: %s" % fig_fname)
+    if plot:
+        plt.close('all')
+        warnings.simplefilter('ignore', category=AstropyWarning)
+        wcs_new = WCS(hdr)
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection=wcs_new)
+        med_val = np.median(img)
+        ax.imshow(img, vmin=med_val-1*mad(img), vmax=med_val+10*mad(img),
+                origin='lower', cmap=plt.cm.gray_r)
+        ax.scatter(matched_ref[:, 0], matched_ref[:, 1],
+                transform=ax.get_transform('fk5'), edgecolor='r', facecolor='none', s=50)
+        if debug:
+            ax.scatter(matched_sep[:, 0], matched_sep[:, 1],
+                    transform=ax.get_transform('fk5'), edgecolor='green', facecolor='none', s=10, alpha=0.7)
+            for i, r in zip(matched_sep, matched_ref):
+                ax.plot([i[0], r[0]], [i[1], r[1]], 'k', alpha=0.5, transform=ax.get_transform('fk5'))
+        ax.set_xlabel("Right Ascension")
+        ax.set_ylabel("Declination")
+        fig.savefig(fig_fname)
+        msg.append(" [OUTPUT] - Saving WCS solution figure: %s" % fig_fname)
 
 
     # -- Calculate Dispersion in WCS Solution:
     sep_wcs = pixel_to_radec(sep_coords, hdr)
     ref_coords = np.array([ref_cat['ra'], ref_cat['dec']]).T
     ref_coords = ref_coords[bright_cut]
     if len(ref_coords) < len(sep_wcs):
@@ -318,14 +322,15 @@
     else:
         matched_sep, matched_ref = match_catalogs(sep_wcs, ref_coords)
     dist = np.sqrt(np.sum((matched_ref - matched_sep)**2, axis=1)) * 3600
     wcs_resid = mad(dist) * 1.48
     wcs_offset = np.median(dist)
     msg.append("          - WCS precision: %.3f arcsec" % wcs_resid)
     msg.append("          - average WCS offset: %.3f arcsec" % wcs_offset)
+    msg.append("[WARNING] - Large WCS offset!")
 
 
     # Update photometric table:
     sep_cat['ra'] = sep_wcs[:, 0]
     sep_cat['dec'] = sep_wcs[:, 1]
     sep_cat.write(sep_fname, format='fits', overwrite=True)
     msg.append(" [OUTPUT] - Updating source identification table: %s" % sep_fname)
@@ -335,14 +340,15 @@
     if output == '':
         with fits.open(img_fname, mode='update') as hdu_list:
             if 'DATA' not in hdu_list:
                 hdu_list[0].header = hdr
             else:
                 hdu_list['DATA'].header = hdr
             hdu_list['ERR'].header.update(wcs_keys)
+        output = img_fname
     else:
         with fits.open(img_fname) as hdu_list:
             if 'DATA' not in hdu_list:
                 hdu_list[0].header = hdr
             else:
                 hdu_list['DATA'].header = hdr
             hdu_list['ERR'].header.update(wcs_keys)
```

### Comparing `PyNOT-redux-1.3.1/pynot/welcome.py` & `PyNOT-redux-1.3.3/pynot/welcome.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.1/setup.py` & `PyNOT-redux-1.3.3/setup.py`

 * *Files identical despite different names*

