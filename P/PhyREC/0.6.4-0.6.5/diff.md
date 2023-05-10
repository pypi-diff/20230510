# Comparing `tmp/PhyREC-0.6.4.tar.gz` & `tmp/PhyREC-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PhyREC-0.6.4.tar", last modified: Thu Mar 23 15:47:19 2023, max compression
+gzip compressed data, was "PhyREC-0.6.5.tar", last modified: Wed May 10 09:55:24 2023, max compression
```

## Comparing `PhyREC-0.6.4.tar` & `PhyREC-0.6.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-03-23 15:47:19.864007 PhyREC-0.6.4/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1133 2023-03-23 15:47:19.864007 PhyREC-0.6.4/PKG-INFO
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-03-23 15:47:19.860007 PhyREC-0.6.4/PhyREC/
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-03-23 15:47:19.860007 PhyREC-0.6.4/PhyREC/FDM/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     8160 2023-01-15 16:55:13.000000 PhyREC-0.6.4/PhyREC/FDM/Asic.py
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-03-23 15:47:19.864007 PhyREC-0.6.4/PhyREC/FDM/Config/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     4564 2023-01-15 16:47:23.000000 PhyREC-0.6.4/PhyREC/FDM/Config/AS2_F5_M3RevB_7_IN16_CH32
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     4628 2023-01-15 16:47:23.000000 PhyREC-0.6.4/PhyREC/FDM/Config/AS3_F3_220128_C4
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    88270 2023-01-15 16:47:23.000000 PhyREC-0.6.4/PhyREC/FDM/Config/AS_REVB_211207_1
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)   150322 2023-01-15 16:47:23.000000 PhyREC-0.6.4/PhyREC/FDM/Config/AS_REVB_211207_1_ELC
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    28354 2023-01-15 16:47:23.000000 PhyREC-0.6.4/PhyREC/FDM/Config/S0_AS3_T_220101_V1
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     6741 2023-01-15 16:47:23.000000 PhyREC-0.6.4/PhyREC/FDM/DicAddress.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     2631 2023-01-15 16:47:23.000000 PhyREC-0.6.4/PhyREC/FDM/Lockin.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     7907 2023-01-15 16:47:23.000000 PhyREC-0.6.4/PhyREC/FDM/Processing.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        3 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/FDM/__init__.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     7737 2022-12-15 08:52:13.000000 PhyREC-0.6.4/PhyREC/GtechInterface.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     8996 2023-03-17 17:45:37.000000 PhyREC-0.6.4/PhyREC/ImageSequence.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     4248 2023-01-20 20:16:43.000000 PhyREC-0.6.4/PhyREC/MCSInterface.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    10487 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/NeoInterface.py
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-03-23 15:47:19.864007 PhyREC-0.6.4/PhyREC/OpenEphys/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     5360 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/OpenEphys/Binary.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     6823 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/OpenEphys/Kwik.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    17561 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/OpenEphys/OpenEphys.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     5190 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/OpenEphys/SettingsXML.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        3 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/OpenEphys/__init__.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    30443 2023-03-17 18:23:55.000000 PhyREC-0.6.4/PhyREC/PlotWaves.py
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-03-23 15:47:19.864007 PhyREC-0.6.4/PhyREC/PyGFETdb/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     7056 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/PyGFETdb/AnalyzeData.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    36340 2022-10-10 21:49:04.000000 PhyREC-0.6.4/PhyREC/PyGFETdb/DataClass.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     6983 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/PyGFETdb/DataStructures.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    25360 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/PyGFETdb/PlotDataClass.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       88 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/PyGFETdb/__init__.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    15270 2022-12-15 20:16:23.000000 PhyREC-0.6.4/PhyREC/SignalAnalysis.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    23254 2023-03-17 18:03:31.000000 PhyREC-0.6.4/PhyREC/SignalProcess.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1214 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/SupportFunctions.py
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      130 2022-10-10 21:29:30.000000 PhyREC-0.6.4/PhyREC/__init__.py
-drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-03-23 15:47:19.860007 PhyREC-0.6.4/PhyREC.egg-info/
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1133 2023-03-23 15:47:19.000000 PhyREC-0.6.4/PhyREC.egg-info/PKG-INFO
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      978 2023-03-23 15:47:19.000000 PhyREC-0.6.4/PhyREC.egg-info/SOURCES.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        1 2023-03-23 15:47:19.000000 PhyREC-0.6.4/PhyREC.egg-info/dependency_links.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       49 2023-03-23 15:47:19.000000 PhyREC-0.6.4/PhyREC.egg-info/requires.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        7 2023-03-23 15:47:19.000000 PhyREC-0.6.4/PhyREC.egg-info/top_level.txt
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        7 2022-10-10 21:29:01.000000 PhyREC-0.6.4/README.md
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       38 2023-03-23 15:47:19.864007 PhyREC-0.6.4/setup.cfg
--rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     3334 2023-03-23 15:46:01.000000 PhyREC-0.6.4/setup.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-10 09:55:24.660734 PhyREC-0.6.5/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1133 2023-05-10 09:55:24.660734 PhyREC-0.6.5/PKG-INFO
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-10 09:55:24.652734 PhyREC-0.6.5/PhyREC/
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-10 09:55:24.656734 PhyREC-0.6.5/PhyREC/FDM/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     8160 2023-01-15 16:55:13.000000 PhyREC-0.6.5/PhyREC/FDM/Asic.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-10 09:55:24.656734 PhyREC-0.6.5/PhyREC/FDM/Config/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     4564 2023-01-15 16:47:23.000000 PhyREC-0.6.5/PhyREC/FDM/Config/AS2_F5_M3RevB_7_IN16_CH32
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     4628 2023-01-15 16:47:23.000000 PhyREC-0.6.5/PhyREC/FDM/Config/AS3_F3_220128_C4
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    88270 2023-01-15 16:47:23.000000 PhyREC-0.6.5/PhyREC/FDM/Config/AS_REVB_211207_1
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)   150322 2023-01-15 16:47:23.000000 PhyREC-0.6.5/PhyREC/FDM/Config/AS_REVB_211207_1_ELC
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    28354 2023-01-15 16:47:23.000000 PhyREC-0.6.5/PhyREC/FDM/Config/S0_AS3_T_220101_V1
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     6741 2023-01-15 16:47:23.000000 PhyREC-0.6.5/PhyREC/FDM/DicAddress.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     2631 2023-01-15 16:47:23.000000 PhyREC-0.6.5/PhyREC/FDM/Lockin.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     7907 2023-01-15 16:47:23.000000 PhyREC-0.6.5/PhyREC/FDM/Processing.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        3 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/FDM/__init__.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     7737 2022-12-15 08:52:13.000000 PhyREC-0.6.5/PhyREC/GtechInterface.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     8996 2023-03-17 17:45:37.000000 PhyREC-0.6.5/PhyREC/ImageSequence.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     4248 2023-01-20 20:16:43.000000 PhyREC-0.6.5/PhyREC/MCSInterface.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    10487 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/NeoInterface.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-10 09:55:24.660734 PhyREC-0.6.5/PhyREC/OpenEphys/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     5360 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/OpenEphys/Binary.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     6823 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/OpenEphys/Kwik.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    17561 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/OpenEphys/OpenEphys.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     5190 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/OpenEphys/SettingsXML.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        3 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/OpenEphys/__init__.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    30437 2023-05-10 09:53:27.000000 PhyREC-0.6.5/PhyREC/PlotWaves.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-10 09:55:24.660734 PhyREC-0.6.5/PhyREC/PyGFETdb/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     7056 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/PyGFETdb/AnalyzeData.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    36340 2022-10-10 21:49:04.000000 PhyREC-0.6.5/PhyREC/PyGFETdb/DataClass.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     6983 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/PyGFETdb/DataStructures.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    25360 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/PyGFETdb/PlotDataClass.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       88 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/PyGFETdb/__init__.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    15270 2022-12-15 20:16:23.000000 PhyREC-0.6.5/PhyREC/SignalAnalysis.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)    23976 2023-05-10 09:49:02.000000 PhyREC-0.6.5/PhyREC/SignalProcess.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1214 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/SupportFunctions.py
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      130 2022-10-10 21:29:30.000000 PhyREC-0.6.5/PhyREC/__init__.py
+drwxrwxr-x   0 aguimera  (1000) aguimera  (1000)        0 2023-05-10 09:55:24.652734 PhyREC-0.6.5/PhyREC.egg-info/
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     1133 2023-05-10 09:55:24.000000 PhyREC-0.6.5/PhyREC.egg-info/PKG-INFO
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)      978 2023-05-10 09:55:24.000000 PhyREC-0.6.5/PhyREC.egg-info/SOURCES.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        1 2023-05-10 09:55:24.000000 PhyREC-0.6.5/PhyREC.egg-info/dependency_links.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       49 2023-05-10 09:55:24.000000 PhyREC-0.6.5/PhyREC.egg-info/requires.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        7 2023-05-10 09:55:24.000000 PhyREC-0.6.5/PhyREC.egg-info/top_level.txt
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)        7 2022-10-10 21:29:01.000000 PhyREC-0.6.5/README.md
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)       38 2023-05-10 09:55:24.660734 PhyREC-0.6.5/setup.cfg
+-rw-rw-r--   0 aguimera  (1000) aguimera  (1000)     3334 2023-05-10 09:54:56.000000 PhyREC-0.6.5/setup.py
```

### Comparing `PhyREC-0.6.4/PKG-INFO` & `PhyREC-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PhyREC
-Version: 0.6.4
+Version: 0.6.5
 Summary: Library for electrphysiological analysis based on neo
 Home-page: https://github.com/aguimera/PhyREC
 Download-URL: https://github.com/aguimera/PhyREC
 Author: Anton Guimera-Brunet
 Author-email: anton.guimera@csic.es
 Maintainer: Anton Guimera-Brunet
 Maintainer-email: anton.guimera@csic.es
```

### Comparing `PhyREC-0.6.4/PhyREC/FDM/Asic.py` & `PhyREC-0.6.5/PhyREC/FDM/Asic.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/FDM/Config/AS2_F5_M3RevB_7_IN16_CH32` & `PhyREC-0.6.5/PhyREC/FDM/Config/AS2_F5_M3RevB_7_IN16_CH32`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/FDM/Config/AS3_F3_220128_C4` & `PhyREC-0.6.5/PhyREC/FDM/Config/AS3_F3_220128_C4`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/FDM/Config/AS_REVB_211207_1` & `PhyREC-0.6.5/PhyREC/FDM/Config/AS_REVB_211207_1`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/FDM/Config/AS_REVB_211207_1_ELC` & `PhyREC-0.6.5/PhyREC/FDM/Config/AS_REVB_211207_1_ELC`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/FDM/Config/S0_AS3_T_220101_V1` & `PhyREC-0.6.5/PhyREC/FDM/Config/S0_AS3_T_220101_V1`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/FDM/DicAddress.py` & `PhyREC-0.6.5/PhyREC/FDM/DicAddress.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/FDM/Lockin.py` & `PhyREC-0.6.5/PhyREC/FDM/Lockin.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/FDM/Processing.py` & `PhyREC-0.6.5/PhyREC/FDM/Processing.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/GtechInterface.py` & `PhyREC-0.6.5/PhyREC/GtechInterface.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/ImageSequence.py` & `PhyREC-0.6.5/PhyREC/ImageSequence.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/MCSInterface.py` & `PhyREC-0.6.5/PhyREC/MCSInterface.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/NeoInterface.py` & `PhyREC-0.6.5/PhyREC/NeoInterface.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/OpenEphys/Binary.py` & `PhyREC-0.6.5/PhyREC/OpenEphys/Binary.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/OpenEphys/Kwik.py` & `PhyREC-0.6.5/PhyREC/OpenEphys/Kwik.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/OpenEphys/OpenEphys.py` & `PhyREC-0.6.5/PhyREC/OpenEphys/OpenEphys.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/OpenEphys/SettingsXML.py` & `PhyREC-0.6.5/PhyREC/OpenEphys/SettingsXML.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/PlotWaves.py` & `PhyREC-0.6.5/PhyREC/PlotWaves.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 
     def PlotSignal(self, Time, Units=None):
         sig = self.GetSignal(Time, Units)
 
         if self.MaxPoints is not None:
             sig = Spro.Resample(sig, MaxPoints=self.MaxPoints)
 
-        img = self.Ax.imshow(np.array(sig).astype(np.float).transpose(),
+        img = self.Ax.imshow(np.array(sig).astype(float).transpose(),
                              aspect='auto',
                              extent=(sig.t_start, sig.t_stop,
                                      0, sig.shape[1]),
                              **self.imKwargs,
                              )
         self.img = img
         self.current_time = (sig.t_start.rescale('s'),
@@ -268,15 +268,15 @@
         if 'spec' in sig.annotations:
             spec = sig
         else:
             spec = Spro.Spectrogram(sig, **self.specKwargs)
 
         f = spec.annotations['Freq']
         data = Spro.Resample(spec, MaxPoints=self.MaxPoints)
-        img = self.Ax.imshow(np.array(data).astype(np.float).transpose(),
+        img = self.Ax.imshow(np.array(data).astype(float).transpose(),
                              origin='lower',
                              aspect='auto',
                              extent=(spec.t_start, spec.t_stop,
                                      np.min(f), np.max(f)),
                              **self.imKwargs,
                              )
         self.img = img
```

### Comparing `PhyREC-0.6.4/PhyREC/PyGFETdb/AnalyzeData.py` & `PhyREC-0.6.5/PhyREC/PyGFETdb/AnalyzeData.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/PyGFETdb/DataClass.py` & `PhyREC-0.6.5/PhyREC/PyGFETdb/DataClass.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/PyGFETdb/DataStructures.py` & `PhyREC-0.6.5/PhyREC/PyGFETdb/DataStructures.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/PyGFETdb/PlotDataClass.py` & `PhyREC-0.6.5/PhyREC/PyGFETdb/PlotDataClass.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/SignalAnalysis.py` & `PhyREC-0.6.5/PhyREC/SignalAnalysis.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC/SignalProcess.py` & `PhyREC-0.6.5/PhyREC/SignalProcess.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from scipy.interpolate import UnivariateSpline
 from scipy.signal import medfilt
 import elephant
 from numpy.lib.stride_tricks import sliding_window_view
 
 def Spectrogram(sig, Fres=2*pq.Hz, TimeRes=0.01*pq.s,
                 Fmin=1*pq.Hz, Fmax=200*pq.Hz, Zscored=True, NormTime=None,
-                dtype=np.float,
+                dtype=float,
                 **specKwarg):
 
     nFFT = int(2**(np.around(np.log2(sig.sampling_rate/Fres))+1))
     Ts = sig.sampling_period
     noverlap = int((Ts*nFFT - TimeRes)/Ts)
 
     f, t, Sxx = signal.spectrogram(sig,
@@ -731,13 +731,37 @@
 
 #    CalSig.annotate(**annotations)
     CalSig.array_annotate(**annotations)
 
     return CalSig
 
 
+def NoiseBlanking(sig, NoiseLimitRMS=20*pq.uV, MinNoiseFreeTime=5*pq.s, timewidth=1*pq.s ,Value=0):
+    sRMS = sliding_window(sig, timewidth)
+    
+    noisets = sRMS.times[np.where(sRMS>NoiseLimitRMS)[0]]
+
+    if len(noisets) == 0:
+        return sig
+
+    inds = np.where(np.diff(noisets)>MinNoiseFreeTime)[0]
+
+    NoiseBlocks = []
+    NoiseBlocks.append((noisets[0], noisets[inds[0]]))
+    for ic, ind in enumerate(inds[:-1]):
+        NoiseBlocks.append((noisets[ind+1], noisets[inds[ic+1]]))
+    NoiseBlocks.append((noisets[inds[-1]+1],noisets[-1]))
+
+    for ti, te in NoiseBlocks:
+        i1 = sig.time_index(ti)
+        i2 = sig.time_index(te)
+        sig[i1:i2] = np.ones((i2-i1,1))*Value*sig.units
+   
+    return sig
+
+
 def ApplyProcessChain(sig, ProcessChain):
     sl = sig.copy()
     for Proc in ProcessChain:
         sl = Proc['function'](sl, **Proc['args'])
 
     return sl
```

### Comparing `PhyREC-0.6.4/PhyREC/SupportFunctions.py` & `PhyREC-0.6.5/PhyREC/SupportFunctions.py`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/PhyREC.egg-info/PKG-INFO` & `PhyREC-0.6.5/PhyREC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PhyREC
-Version: 0.6.4
+Version: 0.6.5
 Summary: Library for electrphysiological analysis based on neo
 Home-page: https://github.com/aguimera/PhyREC
 Download-URL: https://github.com/aguimera/PhyREC
 Author: Anton Guimera-Brunet
 Author-email: anton.guimera@csic.es
 Maintainer: Anton Guimera-Brunet
 Maintainer-email: anton.guimera@csic.es
```

### Comparing `PhyREC-0.6.4/PhyREC.egg-info/SOURCES.txt` & `PhyREC-0.6.5/PhyREC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PhyREC-0.6.4/setup.py` & `PhyREC-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Foobar.  If not, see <http://www.gnu.org/licenses/>.
 
 
 from setuptools import setup, find_packages
 
-_version = '0.6.4'
+_version = '0.6.5'
 
 long_description = "Library for electrphysiological analysis based on neo"
 
 install_requires = ['numpy',
                     'matplotlib',
                     'quantities',
                     'scipy',
```

