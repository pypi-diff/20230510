# Comparing `tmp/iosense_connect_onprem-0.0.3.tar.gz` & `tmp/iosense_connect_onprem-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect_onprem-0.0.3.tar", last modified: Wed Apr 19 09:15:36 2023, max compression
+gzip compressed data, was "dist\iosense_connect_onprem-0.0.4.tar", last modified: Wed May 10 09:17:28 2023, max compression
```

## Comparing `iosense_connect_onprem-0.0.3.tar` & `iosense_connect_onprem-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 09:15:36.600631 iosense_connect_onprem-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect_onprem-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-04-19 09:15:36.520853 iosense_connect_onprem-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      683 2023-04-18 04:44:54.000000 iosense_connect_onprem-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 09:15:36.378030 iosense_connect_onprem-0.0.3/iosense_connect_onprem/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem/__init__.py
--rw-rw-rw-   0        0        0    19478 2023-04-19 09:13:04.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem/data_access.py
-drwxrwxrwx   0        0        0        0 2023-04-19 09:15:36.515374 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-04-19 09:15:35.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-04-19 09:15:35.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 09:15:35.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-19 09:15:35.000000 iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 09:15:36.601637 iosense_connect_onprem-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      626 2023-04-19 09:15:16.000000 iosense_connect_onprem-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:17:28.977842 iosense_connect_onprem-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect_onprem-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-10 09:17:28.941779 iosense_connect_onprem-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-04-18 04:44:54.000000 iosense_connect_onprem-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 09:17:28.887239 iosense_connect_onprem-0.0.4/iosense_connect_onprem/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect_onprem-0.0.4/iosense_connect_onprem/__init__.py
+-rw-rw-rw-   0        0        0    19480 2023-05-10 09:17:02.000000 iosense_connect_onprem-0.0.4/iosense_connect_onprem/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:17:28.938670 iosense_connect_onprem-0.0.4/iosense_connect_onprem.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-10 09:17:28.000000 iosense_connect_onprem-0.0.4/iosense_connect_onprem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-10 09:17:28.000000 iosense_connect_onprem-0.0.4/iosense_connect_onprem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:17:28.000000 iosense_connect_onprem-0.0.4/iosense_connect_onprem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-10 09:17:28.000000 iosense_connect_onprem-0.0.4/iosense_connect_onprem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:17:28.983380 iosense_connect_onprem-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-05-10 09:17:27.000000 iosense_connect_onprem-0.0.4/setup.py
```

### Comparing `iosense_connect_onprem-0.0.3/LICENSE.txt` & `iosense_connect_onprem-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect_onprem-0.0.3/PKG-INFO` & `iosense_connect_onprem-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect_onprem
-Version: 0.0.3
+Version: 0.0.4
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect_onprem-0.0.3/README.md` & `iosense_connect_onprem-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect_onprem-0.0.3/iosense_connect_onprem/data_access.py` & `iosense_connect_onprem-0.0.4/iosense_connect_onprem/data_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             # print(df_meta)
             df_meta = df_meta.set_index('paramName').transpose()
             # print(df_meta)
             if 'm' in df_meta.columns and 'c' in df_meta.columns:
                 # print(df_meta.iloc[0]['m'],type(df_meta.iloc[0]['m']))
                 m = float(df_meta.iloc[0]['m'])
                 # print('M value',m)
-                c = int(df_meta.iloc[0]['c'])
+                c = float(df_meta.iloc[0]['c'])
                 # print(m, type(c))
                 # print(df[str(value2)])
                 df[str(value2)] =  df[str(value2)].replace('BAD 255', '-99999').replace('-','99999').replace('BAD undefined', '-99999').replace('BAD 0', '-99999')
                 df[str(value2)] = df[str(value2)].astype('float')
                 # print('==',df[str(value2)])
                 df[str(value2)] = (df[str(value2)] * m) + c
                 if 'min' in df_meta.columns:
```

### Comparing `iosense_connect_onprem-0.0.3/iosense_connect_onprem.egg-info/PKG-INFO` & `iosense_connect_onprem-0.0.4/iosense_connect_onprem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect-onprem
-Version: 0.0.3
+Version: 0.0.4
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect_onprem-0.0.3/setup.py` & `iosense_connect_onprem-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect_onprem",
-    version = "0.0.3",
+    version = "0.0.4",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect_onprem"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```

