# Comparing `tmp/metobs_toolkit-0.0.2a1.tar.gz` & `tmp/metobs_toolkit-0.0.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metobs_toolkit-0.0.2a1.tar", max compression
+gzip compressed data, was "metobs_toolkit-0.0.2a2.tar", max compression
```

## Comparing `metobs_toolkit-0.0.2a1.tar` & `metobs_toolkit-0.0.2a2.tar`

### file list

```diff
@@ -1,33 +1,40 @@
--rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a1/LICENSE
--rw-r--r--   0        0        0      403 2023-04-14 14:06:24.419816 metobs_toolkit-0.0.2a1/README.md
--rw-r--r--   0        0        0     1032 2023-04-14 14:41:28.643473 metobs_toolkit-0.0.2a1/metobs_toolkit/__init__.py
--rw-r--r--   0        0        0     2596 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/convertors.py
--rw-r--r--   0        0        0    11411 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/data_import.py
--rw-r--r--   0        0        0     3066 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/db_templates.py
--rw-r--r--   0        0        0     1435 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/import_templates.py
--rw-r--r--   0        0        0      931 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/template_defaults/default_template.csv
--rw-r--r--   0        0        0    51034 2023-04-14 14:28:43.809424 metobs_toolkit-0.0.2a1/metobs_toolkit/dataset.py
--rw-r--r--   0        0        0     6522 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/df_helpers.py
--rw-r--r--   0        0        0    22588 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/gap.py
--rw-r--r--   0        0        0    14894 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/gap_filling.py
--rw-r--r--   0        0        0      686 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/geometry_functions.py
--rw-r--r--   0        0        0    18373 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/landcover_functions.py
--rw-r--r--   0        0        0     3884 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/missingobs.py
--rw-r--r--   0        0        0     4950 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/modeldata.py
--rw-r--r--   0        0        0    14086 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/plotting_functions.py
--rw-r--r--   0        0        0     1587 2023-04-14 14:06:24.499817 metobs_toolkit-0.0.2a1/metobs_toolkit/printing.py
--rw-r--r--   0        0        0    23064 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/qc_checks.py
--rw-r--r--   0        0        0     3381 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/qc_statistics.py
--rw-r--r--   0        0        0    13092 2023-04-14 14:21:45.347574 metobs_toolkit-0.0.2a1/metobs_toolkit/settings.py
--rw-r--r--   0        0        0       73 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/app_print_settings.json
--rw-r--r--   0        0        0      114 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/dataset_resolution_settings.json
--rw-r--r--   0        0        0     4182 2023-04-14 14:20:24.511222 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/default_formats_settings.py
--rw-r--r--   0        0        0     1567 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/gaps_settings.py
--rw-r--r--   0        0        0     4823 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/gee_settings.py
--rw-r--r--   0        0        0     3982 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/qc_settings.py
--rw-r--r--   0        0        0      132 2023-04-14 14:06:24.503816 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/server_login.json
--rw-r--r--   0        0        0  8385556 2023-04-14 14:06:24.563817 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
--rw-r--r--   0        0        0     2108 2023-04-14 14:06:24.563817 metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
--rw-r--r--   0        0        0     2599 2023-04-14 14:06:24.563817 metobs_toolkit-0.0.2a1/metobs_toolkit/writing_files.py
--rw-r--r--   0        0        0      834 2023-04-14 14:41:28.563471 metobs_toolkit-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.0.2a2/LICENSE
+-rw-r--r--   0        0        0      403 2023-05-10 06:57:22.583568 metobs_toolkit-0.0.2a2/README.md
+-rw-r--r--   0        0        0     2438 2023-05-10 12:42:06.812133 metobs_toolkit-0.0.2a2/metobs_toolkit/__init__.py
+-rw-r--r--   0        0        0    19751 2023-05-10 07:27:19.656930 metobs_toolkit-0.0.2a2/metobs_toolkit/analysis.py
+-rw-r--r--   0        0        0     2566 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a2/metobs_toolkit/convertors.py
+-rw-r--r--   0        0        0    12056 2023-05-10 07:27:19.656930 metobs_toolkit-0.0.2a2/metobs_toolkit/data_import.py
+-rw-r--r--   0        0        0     2378 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/db_templates.py
+-rw-r--r--   0        0        0     1701 2023-05-10 07:27:19.656930 metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/import_templates.py
+-rw-r--r--   0        0        0      931 2023-05-10 06:57:22.695567 metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/template_defaults/default_template.csv
+-rwxr-xr-x   0        0        0  9062298 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_datafile.csv
+-rw-r--r--   0        0        0     2306 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_metadatafile.csv
+-rw-r--r--   0        0        0      931 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/datafiles/demo_templatefile.csv
+-rw-r--r--   0        0        0    68547 2023-05-10 11:47:22.343657 metobs_toolkit-0.0.2a2/metobs_toolkit/dataset.py
+-rw-r--r--   0        0        0    17115 2023-05-10 11:47:22.343657 metobs_toolkit-0.0.2a2/metobs_toolkit/dataset_settings_updater.py
+-rw-r--r--   0        0        0    11623 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/df_helpers.py
+-rw-r--r--   0        0        0    22073 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/gap.py
+-rw-r--r--   0        0        0    15267 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/gap_filling.py
+-rw-r--r--   0        0        0      673 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/geometry_functions.py
+-rw-r--r--   0        0        0    18129 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/landcover_functions.py
+-rw-r--r--   0        0        0     7973 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/missingobs.py
+-rw-r--r--   0        0        0     4723 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/modeldata.py
+-rw-r--r--   0        0        0    20492 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/plotting_functions.py
+-rw-r--r--   0        0        0     1847 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/printing.py
+-rw-r--r--   0        0        0    22903 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/qc_checks.py
+-rw-r--r--   0        0        0     4159 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/qc_statistics.py
+-rw-r--r--   0        0        0    14146 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/settings.py
+-rw-r--r--   0        0        0       73 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/app_print_settings.json
+-rw-r--r--   0        0        0      237 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/dataset_resolution_settings.json
+-rw-r--r--   0        0        0     4509 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/default_formats_settings.py
+-rw-r--r--   0        0        0     1831 2023-05-10 07:27:19.692932 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/gaps_and_missing_settings.py
+-rw-r--r--   0        0        0     3880 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/gee_settings.py
+-rw-r--r--   0        0        0     2851 2023-05-10 11:47:22.347657 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/qc_settings.py
+-rw-r--r--   0        0        0      132 2023-05-10 06:57:22.727566 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/server_login.json
+-rw-r--r--   0        0        0  8385556 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
+-rw-r--r--   0        0        0     2108 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
+-rw-r--r--   0        0        0      916 2023-05-10 07:27:19.688931 metobs_toolkit-0.0.2a2/metobs_toolkit/station.py
+-rw-r--r--   0        0        0        0 2023-05-10 12:30:33.435807 metobs_toolkit-0.0.2a2/metobs_toolkit/test.py
+-rw-r--r--   0        0        0     2441 2023-05-10 06:57:22.787565 metobs_toolkit-0.0.2a2/metobs_toolkit/writing_files.py
+-rw-r--r--   0        0        0      835 2023-05-10 12:42:06.732132 metobs_toolkit-0.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 metobs_toolkit-0.0.2a2/PKG-INFO
```

### Comparing `metobs_toolkit-0.0.2a1/LICENSE` & `metobs_toolkit-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/convertors.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/convertors.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,58 +5,56 @@
 
 @author: thoverga
 """
 
 import sys
 import numpy as np
 from collections.abc import Iterable
+
 # =============================================================================
 # Unit defenitions and coversions
 # =============================================================================
-#Keys are the toolkit-units!! (not persee SI)
-#values expresions are of the form x $ val, where x is the numeric value,
+# Keys are the toolkit-units!! (not persee SI)
+# values expresions are of the form x $ val, where x is the numeric value,
 # $ an operator (+-*/) and val a concersion value
 unit_convertors = {
-                'Celsius': {'K': 'x - 273.15'},
-    
-                }
-
-
+    "Celsius": {"K": "x - 273.15"},
+}
 
 
 # =============================================================================
 # Convert functions
 # =============================================================================
 
+
 def expression_calculator(equation, x):
     if isinstance(x, Iterable):
         x = np.array(x)
-    
-    if '+' in equation:
-        y = equation.split('+')
-        return x+float(y[1])
-    elif '-' in equation:
-        y = equation.split('-')
-        return x-float(y[1])
-    elif '/' in equation:
-        y = equation.split('/')
-        return x/float(y[1])
-    elif '*' in equation:
-        y = equation.split('*')
-        return x*float(y[1])
-    else: 
-        sys.exit(f'expression {equation}, can not be converted to mathematical.')
-        
-        
+
+    if "+" in equation:
+        y = equation.split("+")
+        return x + float(y[1])
+    elif "-" in equation:
+        y = equation.split("-")
+        return x - float(y[1])
+    elif "/" in equation:
+        y = equation.split("/")
+        return x / float(y[1])
+    elif "*" in equation:
+        y = equation.split("*")
+        return x * float(y[1])
+    else:
+        sys.exit(f"expression {equation}, can not be converted to mathematical.")
+
 
 def convert_to_toolkit_units(data, data_unit):
     """
-    Convert the data to the toolkit perfered unit. Data can be a numeric value or an iterable. 
+    Convert the data to the toolkit perfered unit. Data can be a numeric value or an iterable.
     Data_unit is the unit of the input data.
-    
+
     The converted data AND the corresponding toolkit unit is returned.
 
     Parameters
     ----------
     data : numeric, iterable
         numeric data to be converted.
     data_unit : String
@@ -66,23 +64,26 @@
     -------
     numeric, numpy.array
         The data in toolkit units.
     String
         Corresponding toolkit unit name.
 
     """
-    #check if unit is already a toolkit unit
+    # check if unit is already a toolkit unit
     if data_unit in unit_convertors.keys():
         return data, data_unit
-    
-    #scan the units to find conversion
-    expr = { toolk_unit: other_unit[data_unit]  for toolk_unit, other_unit in unit_convertors.items() if data_unit in other_unit.keys()}
 
-    if len(expr) == 1: #unique conversion found
-    
+    # scan the units to find conversion
+    expr = {
+        toolk_unit: other_unit[data_unit]
+        for toolk_unit, other_unit in unit_convertors.items()
+        if data_unit in other_unit.keys()
+    }
+
+    if len(expr) == 1:  # unique conversion found
         conv_data = expression_calculator(next(iter(expr.values())), data)
         return conv_data, next(iter(expr.keys()))
-    
+
     elif len(expr) > 1:
-        sys.exit(f' Multiple possible conversions found for {data_unit}')
+        sys.exit(f" Multiple possible conversions found for {data_unit}")
     else:
-        sys.exit(f'No conversion found for {data_unit}')
+        sys.exit(f"No conversion found for {data_unit}")
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/data_import.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/data_import.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 import mysql.connector
 from mysql.connector import errorcode
 from metobs_toolkit.df_helpers import init_multiindexdf
 from metobs_toolkit.data_templates.import_templates import read_csv_template
 
 
 def template_to_package_space(specific_template):
+    returndict = {
+        val["varname"]: {"orig_name": key} for key, val in specific_template.items()
+    }
+    for key, item in returndict.items():
+        orig_dict = dict(specific_template[item["orig_name"]])
+        orig_dict.pop("varname")
+        returndict[key].update(orig_dict)
+    return returndict
 
-   returndict = {val['varname']: {'orig_name': key} for key, val in specific_template.items()}
-   for key, item in returndict.items():
-       orig_dict = dict(specific_template[item['orig_name']])
-       orig_dict.pop('varname')
-       returndict[key].update(orig_dict)
-   return returndict
 
 def find_compatible_templatefor(df_columns, template_list):
-   for templ in template_list:
-     found = all(keys in list(df_columns) for keys in templ.keys())
-     if found:
-         print('Compatible template found. ')
-         return templ
-   sys.exit("No compatible teplate found!")
-
+    for templ in template_list:
+        found = all(keys in list(df_columns) for keys in templ.keys())
+        if found:
+            print("Compatible template found. ")
+            return templ
+    sys.exit("No compatible teplate found!")
 
 
 def compress_dict(nested_dict, valuesname):
     """
     This function unnests a nested dictionary for a specific valuename that is a key in the nested dict.
 
     Parameters
@@ -58,308 +59,321 @@
     returndict = {}
     for key, item in nested_dict.items():
         if valuesname in item:
             returndict[key] = item[valuesname]
     return returndict
 
 
-
-
-# def coarsen_time_resolution(df, freq='H', method='bfill'):
-
-#     #TODO: implement buffer method
-
-#     if method=='bfill':
-#         #apply per station
-#         resample_df = pd.DataFrame()
-#         for stationname in df['name'].unique():
-#             subdf = df[df['name'] == stationname]
-
-
-#             #  Check if index is unique
-#             if not subdf.index.is_unique:
-#                 print('Duplicate timestamp found !!, this will be removed')
-#                 dup_mask = subdf.index.duplicated(keep='first')
-#                 subdf = subdf[~dup_mask]
-#                 subdf = subdf.sort_index()
-
-
-
-#             resample_subdf = subdf.resample(rule=freq,
-#                                             axis='index').bfill()
-
-#             resample_df = pd.concat([resample_df, resample_subdf])
-
-#         return resample_df
-
 def check_template_compatibility(template, df_columns):
-
     # test if all df_columns are in template keys
     if not all(col in template.keys() for col in df_columns):
         unmapped = list(set(df_columns) - set(template.keys()))
-        print(f'WARNING! The following columns are not pressent in the template,\
-              and cannot be mapped: {unmapped}')
+        print(
+            f"WARNING! The following columns are not pressent in the template,\
+              and cannot be mapped: {unmapped}"
+        )
 
     if len(list(set(df_columns) - set(template.keys()))) == len(df_columns):
-        sys.exit(f'Fatal: The given template does not match with any of the data columns.')
-
-
-
-
-
-
-
-
+        sys.exit(
+            f"Fatal: The given template does not match with any of the data columns."
+        )
 
 
 def import_metadata_from_csv(input_file, template_file):
-
-    common_seperators = [';',',','    ','.']
+    common_seperators = [";", ",", "    ", "."]
     assert not isinstance(input_file, type(None)), "Specify input file in the settings!"
     for sep in common_seperators:
-
         df = pd.read_csv(input_file, sep=sep)
         assert not df.empty, "Dataset is empty!"
 
         if len(df.columns) > 1:
             break
 
-    assert len(df.columns) > 1, f'Only one column detected from import using these seperators: {common_seperators}. See if csv template is correct.'
-
+    assert (
+        len(df.columns) > 1
+    ), f"Only one column detected from import using these seperators: {common_seperators}. See if csv template is correct."
 
     # validate template
     template = read_csv_template(template_file)
     check_template_compatibility(template, df.columns)
 
-
     # rename columns to toolkit attriute names
-    df = df.rename(columns=compress_dict(template, 'varname'))
+    df = df.rename(columns=compress_dict(template, "varname"))
 
     return df
+def wide_to_long(df, template, obstype):
+
+    print('Converting wide data to long')
+    mapped_colnames = [val['varname'] for val in template.values()]
+    data_colnames = [col for col in df.columns if not col in mapped_colnames]
+    longdf = pd.melt(df, id_vars=['Tijd'], value_vars=data_colnames,
+                   var_name='name', value_name=obstype)
+
+    # update template
+    template[obstype] = template['_wide_dummy']
+    del template['_wide_dummy']
+
+    template['name'] = {'varname': 'name', 'dtype':'object'}
 
+    return longdf, template
 
 
-def import_data_from_csv(input_file, template_file):
 
-    common_seperators = [';',',','    ','.']
+def wide_to_long(df, template, obstype):
+    print("Converting wide data to long")
+    mapped_colnames = [val["varname"] for val in template.values()]
+    data_colnames = [col for col in df.columns if not col in mapped_colnames]
+    longdf = pd.melt(
+        df,
+        id_vars=["Tijd"],
+        value_vars=data_colnames,
+        var_name="name",
+        value_name=obstype,
+    )
+
+    # update template
+    template[obstype] = template["_wide_dummy"]
+    del template["_wide_dummy"]
+
+    template["name"] = {"varname": "name", "dtype": "object"}
+
+    return longdf, template
+
+
+
+def import_data_from_csv(input_file, template_file, long_format, obstype):
+    common_seperators = [";", ",", "    ", "."]
     assert not isinstance(input_file, type(None)), "Specify input file in the settings!"
     for sep in common_seperators:
-
         df = pd.read_csv(input_file, sep=sep)
         assert not df.empty, "Dataset is empty!"
 
         if len(df.columns) > 1:
             break
 
-    assert len(df.columns) > 1, f'Only one column detected from import using these seperators: {common_seperators}. See if csv template is correct.'
-
+    assert (
+        len(df.columns) > 1
+    ), f"Only one column detected from import using these seperators: {common_seperators}. See if csv template is correct."
 
     # LINES TO DEAL WITH RANDOM PIECES OF TEXT BEFORE ACTUAL MEASUREMENTS
-    if (True in df.columns.str.contains(pat = 'Unnamed')):
+    if True in df.columns.str.contains(pat="Unnamed"):
         num_columns = df.iloc[-3].count().sum()
 
         rows_to_skip = 0
         for row in range(len(df)):
-            if df.iloc[row:(row+1),:].count().sum() != num_columns:
+            if df.iloc[row : (row + 1), :].count().sum() != num_columns:
                 rows_to_skip += 1
             else:
                 break
-        df = df.iloc[rows_to_skip:,:]
-        df = df.rename(columns=df.iloc[0]).iloc[1:,:]
+        df = df.iloc[rows_to_skip:, :]
+        df = df.rename(columns=df.iloc[0]).iloc[1:, :]
     df.index = range(len(df))
 
-
-
     # validate template
-    template = read_csv_template(template_file)
+    template = read_csv_template(template_file, long_format, obstype)
+    # convert wide data to long if needed
+    if not long_format:
+        df, template = wide_to_long(df, template, obstype)
+
     check_template_compatibility(template, df.columns)
 
 
 
     for key, value in template.items():
-        if value['dtype'] == 'float64':
-
-            df[key] = pd.to_numeric(df[key], errors='coerce')
-
-
+        if value["dtype"] == "float64":
+            df[key] = pd.to_numeric(df[key], errors="coerce")
 
     # rename columns to toolkit attriute names
-    df = df.rename(columns=compress_dict(template, 'varname'))
+    df = df.rename(columns=compress_dict(template, "varname"))
 
-    #COnvert template to package-space
-    invtemplate =template_to_package_space(template)
+    # COnvert template to package-space
+    invtemplate = template_to_package_space(template)
 
-    #format columns
-    #df = df.astype(dtype=compress_dict(template, 'dtype'))
+    # format columns
+    # df = df.astype(dtype=compress_dict(template, 'dtype'))
 
-
-    if 'datetime' in df.columns:
-        df['datetime'] =pd.to_datetime(df['datetime'],
-                                        format=invtemplate['datetime']['format'])
+    if "datetime" in df.columns:
+        df["datetime"] = pd.to_datetime(
+            df["datetime"], format=invtemplate["datetime"]["format"]
+        )
 
     else:
-        datetime_fmt = invtemplate['_date']['format'] + ' ' + invtemplate['_time']['format']
-        df['datetime'] =pd.to_datetime(df['_date'] +' ' + df['_time'], format=datetime_fmt)
-        df = df.drop(columns=['_date', '_time'])
-
-    #Set datetime index
-    df = df.set_index('datetime', drop=True, verify_integrity=False)
-    #TODO implement timezone settings
-
+        datetime_fmt = (
+            invtemplate["_date"]["format"] + " " + invtemplate["_time"]["format"]
+        )
+        df["datetime"] = pd.to_datetime(
+            df["_date"] + " " + df["_time"], format=datetime_fmt
+        )
+        df = df.drop(columns=["_date", "_time"])
+
+    # Set datetime index
+    df = df.set_index("datetime", drop=True, verify_integrity=False)
+    # TODO implement timezone settings
 
-
-    #Keep only columns as defined in the template
+    # Keep only columns as defined in the template
     for column in df.columns:
-
         if not (column in invtemplate.keys()):
             df = df.drop(columns=[column])
 
     # add template to the return
 
     return df, invtemplate
 
-#%%
-def import_data_from_db(db_settings,
-                            start_datetime,
-                            end_datetime):
 
+# %%
+def import_data_from_db(db_settings, start_datetime, end_datetime):
     # =============================================================================
     # Make connection to database
     # =============================================================================
 
-    #Make connection with database (needs ugent VPN active)
+    # Make connection with database (needs ugent VPN active)
 
     try:
-        connection = mysql.connector.connect(host=db_settings['db_host'],
-                                      database=db_settings['db_database'],
-                                      user=db_settings['db_user'],
-                                      password=db_settings['db_passw'],
-                                      connection_timeout=1)
+        connection = mysql.connector.connect(
+            host=db_settings["db_host"],
+            database=db_settings["db_database"],
+            user=db_settings["db_user"],
+            password=db_settings["db_passw"],
+            connection_timeout=1,
+        )
     except mysql.connector.Error as err:
         if err.errno == errorcode.ER_ACCESS_DENIED_ERROR:
             print("Something is wrong with your user name or password!")
-            print('Make shure the following envrionment variables are defind:')
-            print('    VLINDER_DB_USER_NAME')
-            print('    VLINDER_DB_USER_PASW')
-            print('or update the Settings.db_user and Settings.db_passw')
+            print("Make shure the following envrionment variables are defind:")
+            print("    VLINDER_DB_USER_NAME")
+            print("    VLINDER_DB_USER_PASW")
+            print("or update the Settings.db_user and Settings.db_passw")
 
-            #TODO use default return
+            # TODO use default return
             return init_multiindexdf()
         elif err.errno == 2003:
-            print("Can't connect to ", db_settings['db_host'], ' host. Make shure your Ugent VPN is on!')
+            print(
+                "Can't connect to ",
+                db_settings["db_host"],
+                " host. Make shure your Ugent VPN is on!",
+            )
             # sys.exit()
-            #TODO use default return
+            # TODO use default return
             return init_multiindexdf()
 
-
-
     # =============================================================================
     # Read all meta data from database
     # =============================================================================
 
-
-    metadata_Query = "select * from " + db_settings['db_meta_table']
+    metadata_Query = "select * from " + db_settings["db_meta_table"]
     cursor = connection.cursor()
     cursor.execute(metadata_Query)
     metadata = cursor.fetchall()
     metadata = pd.DataFrame(metadata)
     # metadata_columns = list(cursor.column_names)
 
     metadata.columns = list(cursor.column_names)
 
-    #subset relevent columns
-    metadata = metadata[list(db_settings['vlinder_db_meta_template'].keys())]
-
-    #rename columns to standards
-    metadata = metadata.rename(columns=compress_dict(db_settings['vlinder_db_meta_template'], 'varname'))
-
-    #COnvert template to package-space
-    template = template_to_package_space(db_settings['vlinder_db_meta_template'])
+    # subset relevent columns
+    metadata = metadata[list(db_settings["vlinder_db_meta_template"].keys())]
 
+    # rename columns to standards
+    metadata = metadata.rename(
+        columns=compress_dict(db_settings["vlinder_db_meta_template"], "varname")
+    )
 
-    #format columns
-    metadata = metadata.astype(dtype=compress_dict(template, 'dtype'))
+    # COnvert template to package-space
+    template = template_to_package_space(db_settings["vlinder_db_meta_template"])
 
+    # format columns
+    metadata = metadata.astype(dtype=compress_dict(template, "dtype"))
 
     # =============================================================================
     # Read observations data
     # =============================================================================
 
-
-
-    assert start_datetime < end_datetime, "start_datetime is not earlier thand end_datetime!"
-
-    observation_types = ['all']
-
-
-    #observation types to strig
-    if observation_types[0] == 'all':
-        obs_type_query_str = '*'
-    else: #TODO
-        print( "NOT IMPLEMENTED YET")
-        obs_type_query_str = '*'
-
-    #format datetime
-
-    datetime_db_info = [item for item in db_settings['vlinder_db_obs_template'].values() if item['varname'] == 'datetime'][0]
-
-    startstring = start_datetime.strftime(format=datetime_db_info['fmt']) #datetime to string
-    endstring = end_datetime.strftime(format=datetime_db_info['fmt']) #datetime to string
-    _inverted_template = template_to_package_space(db_settings['vlinder_db_obs_template'])
-    datetime_column_name = _inverted_template['datetime']['orig_name']
-
-
-    #select all stations
-    obsdata_Query=str(r"SELECT ") + obs_type_query_str + ' ' + \
-            str(r"FROM ") + db_settings['db_obs_table'] + str(' ') + \
-            str(r"WHERE ") + datetime_column_name +  str(r">='") + startstring  + str(r"' AND ") + \
-            datetime_column_name +  str(r"<='") + endstring  + str(r"'  ") + \
-            str(r"ORDER BY ") + datetime_column_name
-
-
-
-
-
+    assert (
+        start_datetime < end_datetime
+    ), "start_datetime is not earlier thand end_datetime!"
+
+    observation_types = ["all"]
+
+    # observation types to strig
+    if observation_types[0] == "all":
+        obs_type_query_str = "*"
+    else:  # TODO
+        print("NOT IMPLEMENTED YET")
+        obs_type_query_str = "*"
+
+    # format datetime
+
+    datetime_db_info = [
+        item
+        for item in db_settings["vlinder_db_obs_template"].values()
+        if item["varname"] == "datetime"
+    ][0]
+
+    startstring = start_datetime.strftime(
+        format=datetime_db_info["fmt"]
+    )  # datetime to string
+    endstring = end_datetime.strftime(
+        format=datetime_db_info["fmt"]
+    )  # datetime to string
+    _inverted_template = template_to_package_space(
+        db_settings["vlinder_db_obs_template"]
+    )
+    datetime_column_name = _inverted_template["datetime"]["orig_name"]
+
+    # select all stations
+    obsdata_Query = (
+        str(r"SELECT ")
+        + obs_type_query_str
+        + " "
+        + str(r"FROM ")
+        + db_settings["db_obs_table"]
+        + str(" ")
+        + str(r"WHERE ")
+        + datetime_column_name
+        + str(r">='")
+        + startstring
+        + str(r"' AND ")
+        + datetime_column_name
+        + str(r"<='")
+        + endstring
+        + str(r"'  ")
+        + str(r"ORDER BY ")
+        + datetime_column_name
+    )
 
     print(obsdata_Query)
 
-
-
     cursor.execute(obsdata_Query)
     obsdata = cursor.fetchall()
     obsdata = pd.DataFrame(obsdata)
 
-
-
     obsdata.columns = list(cursor.column_names)
 
-    #subset relevent columns
-    obsdata = obsdata[list(db_settings['vlinder_db_obs_template'])]
-
-    #format columns
-    obsdata = obsdata.astype(dtype=compress_dict(db_settings['vlinder_db_obs_template'], 'dtype'))
-
-    #rename columns to standards
-    obsdata = obsdata.rename(columns=compress_dict(db_settings['vlinder_db_obs_template'], 'varname'))
+    # subset relevent columns
+    obsdata = obsdata[list(db_settings["vlinder_db_obs_template"])]
 
+    # format columns
+    obsdata = obsdata.astype(
+        dtype=compress_dict(db_settings["vlinder_db_obs_template"], "dtype")
+    )
+
+    # rename columns to standards
+    obsdata = obsdata.rename(
+        columns=compress_dict(db_settings["vlinder_db_obs_template"], "varname")
+    )
 
     connection.close()
 
-
     # =============================================================================
     # merge Observatios and metadata
     # =============================================================================
 
-    combdata = obsdata.merge(metadata,
-                             how='left',
-                             on='id')
-    combdata = combdata.drop(columns=['id'])
-    combdata['datetime'] =pd.to_datetime(combdata['datetime'],
-                                    format=datetime_db_info['fmt'])
-    #TODO implement timezone settings
+    combdata = obsdata.merge(metadata, how="left", on="id")
+    combdata = combdata.drop(columns=["id"])
+    combdata["datetime"] = pd.to_datetime(
+        combdata["datetime"], format=datetime_db_info["fmt"]
+    )
+    # TODO implement timezone settings
 
-
-    #Set datetime index
-    combdata = combdata.set_index('datetime', drop=True, verify_integrity=False)
+    # Set datetime index
+    combdata = combdata.set_index("datetime", drop=True, verify_integrity=False)
 
     return combdata
-
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/import_templates.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/import_templates.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,48 +6,52 @@
 @author: thoverga
 """
 import os, sys
 from pathlib import Path
 import pandas as pd
 
 
-default_template_file = os.path.join(str(Path(__file__).parent),
-                                     'template_defaults',
-                                     'default_template.csv')
+default_template_file = os.path.join(
+    str(Path(__file__).parent), "template_defaults", "default_template.csv"
+)
 
 
 # =============================================================================
 # templates
 # =============================================================================
 
 
-#templates have nested dict structure where the keys are the column names in the csv file, and the
+# templates have nested dict structure where the keys are the column names in the csv file, and the
 # values contain the mapping information to the toolkit classes and names.
 
 
-
-
-def read_csv_template(file):
-    common_seperators = [';',',','    ','.']
+def read_csv_template(file, data_long_format=True, obstype=None):
+    common_seperators = [";", ",", "    ", "."]
     for sep in common_seperators:
-
         templ = pd.read_csv(file, sep=sep)
-        assert not templ.empty, "Dataset is empty!"
+        assert not templ.empty, "Template is empty!"
 
         if len(templ.columns) > 1:
             break
 
-    #Drop emty rows
-    templ = templ.dropna(axis='index', how='all')
+    # Drop emty rows
+    templ = templ.dropna(axis="index", how="all")
+
+    if data_long_format:
+        # Drop variables that are not present in templ
+        templ = templ[templ["template column name"].notna()]
+
+    else:
+        # Do not do this for wide dataframes since the present obstype
+        # is not specified in template oclumn name, but the defenition and datatype do.
+        templ.loc[templ["varname"] == obstype, "template column name"] = "_wide_dummy"
 
-    #Drop variables that are not present in templ
-    templ = templ[templ['template column name'].notna()]
 
-    #create dictionary from templframe
-    templ = templ.set_index('template column name')
+    # create dictionary from templframe
+    templ = templ.set_index("template column name")
 
-    #create a dict from the dataframe, remove Nan value row wise
+    # create a dict from the dataframe, remove Nan value row wise
     template = {}
     for idx, row in templ.iterrows():
         template[idx] = row[~row.isnull()].to_dict()
 
     return template
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/data_templates/template_defaults/default_template.csv` & `metobs_toolkit-0.0.2a2/metobs_toolkit/data_templates/template_defaults/default_template.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/dataset.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,722 +2,945 @@
 # -*- coding: utf-8 -*-
 """
 The class object for a Vlinder/mocca station
 @author: thoverga
 """
 
 import os
+import copy
 from datetime import datetime
 from pytz import all_timezones, common_timezones
 import logging
 import pandas as pd
 import numpy as np
 
 
 from metobs_toolkit.settings import Settings
-from metobs_toolkit.data_import import (import_data_from_csv,
-                                         import_data_from_db,
-                                         template_to_package_space,
-                                         import_metadata_from_csv)
+from metobs_toolkit.data_import import (
+    import_data_from_csv,
+    import_data_from_db,
+    template_to_package_space,
+    import_metadata_from_csv,
+)
 
 from metobs_toolkit.printing import print_dataset_info
-from metobs_toolkit.landcover_functions import (connect_to_gee,
-                                                 lcz_extractor,
-                                                 height_extractor,
-                                                 lc_fractions_extractor,
-                                                 )
-
-from metobs_toolkit.plotting_functions import (geospatial_plot,
-                                                timeseries_plot,
-                                                qc_stats_pie)
-
-from metobs_toolkit.qc_checks import (gross_value_check,
-                                       persistance_check,
-                                       repetitions_check,
-                                       duplicate_timestamp_check,
-                                       step_check,
-                                       window_variation_check,
-                                       invalid_input_check)
+from metobs_toolkit.landcover_functions import (
+    connect_to_gee,
+    lcz_extractor,
+    height_extractor,
+    lc_fractions_extractor,
+)
+
+from metobs_toolkit.plotting_functions import (
+    geospatial_plot,
+    timeseries_plot,
+    qc_stats_pie,
+)
+
+from metobs_toolkit.qc_checks import (
+    gross_value_check,
+    persistance_check,
+    repetitions_check,
+    duplicate_timestamp_check,
+    step_check,
+    window_variation_check,
+    invalid_input_check,
+)
 
 
 from metobs_toolkit.qc_statistics import get_freq_statistics
 from metobs_toolkit.writing_files import write_dataset_to_csv
 
 from metobs_toolkit.missingobs import Missingob_collection
 
-from metobs_toolkit.gap import (Gap_collection,
-                                 missing_timestamp_and_gap_check,
-                                 get_freqency_series)
-
-
-from metobs_toolkit.df_helpers import (add_final_label_to_outliersdf,
-                                        multiindexdf_datetime_subsetting,
-                                        remove_outliers_from_obs,
-                                        init_multiindexdf,
-                                        metadf_to_gdf)
-
+from metobs_toolkit.gap import (
+    Gap_collection,
+    missing_timestamp_and_gap_check,
+)
+
+
+from metobs_toolkit.df_helpers import (
+    multiindexdf_datetime_subsetting,
+    remove_outliers_from_obs,
+    init_multiindexdf,
+    init_triple_multiindexdf,
+    metadf_to_gdf,
+    conv_applied_qc_to_df,
+    get_freqency_series,
+)
 
+from metobs_toolkit.analysis import Analysis
 from metobs_toolkit.modeldata import Modeldata
 
-
-logger = logging.getLogger(__name__)
+from metobs_toolkit import observation_types
 
 
+logger = logging.getLogger(__name__)
 
 
 # =============================================================================
 # Dataset class
 # =============================================================================
 
+
 class Dataset:
     def __init__(self):
         """
         Constructs all the necessary attributes for Dataset object.
 
         """
-        logger.info('Initialise dataset')
+        logger.info("Initialise dataset")
 
         # Dataset with 'good' observations
         self.df = pd.DataFrame()
 
         # Dataset with outlier observations
-        self.outliersdf = init_multiindexdf()
+        self.outliersdf = init_triple_multiindexdf()
 
         self.missing_obs = None  # becomes a Missingob_collection after import
         self.gaps = None  # becomes a gap_collection after import
 
         self.gapfilldf = init_multiindexdf()
-
+        self.missing_fill_df = init_multiindexdf()
 
         # Dataset with metadata (static)
         self.metadf = pd.DataFrame()
         # dataframe containing all information on the description and mapping
         self.data_template = pd.DataFrame()
 
-        self._istype = 'Dataset'
+        self._istype = "Dataset"
         self._freqs = pd.Series(dtype=object)
 
+        self._applied_qc = pd.DataFrame(columns=["obstype", "checkname"])
+        self._qc_checked_obstypes = []  # list with qc-checked obstypes
 
-        self.settings = Settings()
-
-
-    def update_settings(self, output_folder=None, input_data_file=None,
-                  input_metadata_file=None, data_template_file=None,
-                  metadata_template_file=None):
+        self.settings = copy.deepcopy(Settings())
 
-        """
-        Update the most common input-output (IO) settings.
-        (This should be applied before importing the observations.)
-
-        When an update value is None, the specific setting will not be updated.
-
-
-        :param output_folder: a directory to store the output to, defaults to None.
-        :type output_folder: String, optional
-        :param input_data_file: Path to the input data file with observations, defaults to None.
-        :type input_data_file: String, optional
-        :param input_metadata_file: Path to the input metadata file, defaults to None
-        :type input_metadata_file: String, optional
-        :param data_template_file: Path to the mapper-template csv file to be used on the observations.
-        If not given, the default template is used.
-        :type data_template_file: String, optional
-        :param metadata_template_file: Path to the mapper-template csv file to be used on the metadata.
-        If not given, the default template is used.
-        :type metadata_template_file: String, optional
-        :return: No return
-        :rtype: No return
-        """
 
-        self.settings.update_IO(output_folder=output_folder,
-                                input_data_file=input_data_file,
-                                input_metadata_file=input_metadata_file,
-                                data_template_file=data_template_file,
-                                metadata_template_file=metadata_template_file)
 
-    def update_timezone(self, timezonestr):
-        """
-        Change the timezone of the input data. By default the Brussels timezone is assumed.
-        A valid timezonestring is an element of the pytz.all_timezones.
-
-        :param timezonestr: Timezone string of the input observations.
-        :type timezonestr: String
-        :return: None
-        :rtype: None
-        """
-        self.settings.update_timezone(timezonestr)
-
-    def update_default_name(self, default_name):
-        """
-        Update the default name (the name of the station). This name will be
-        used when no names are found in the observational dataset.
 
-        (All observations are assumed to come from one station.)
-
-        :param default_name: Default name to use when no names are present in the data.
-        :type default_name: String
-        :return: None
-        :rtype: None
-
-        """
-        self.settings.app['default_name'] = str(default_name)
 
     def show_settings(self):
         """
         A function that prints out all the settings, structured per thematic.
-        :return: No return
-        :rtype: No return
+
+        Returns
+        -------
+        None.
 
         """
+
         self.settings.show()
 
     def get_station(self, stationname):
         """
-        Extract a station object from the dataset by name.
+        Extract a metobs_toolkit.Station object from the dataset by name.
 
-        :param stationname: The name of the station
-        :type stationname: String
-        :return: The station object.
-        :rtype: metobs_toolkit.Station
+        Parameters
+        ----------
+        stationname : string
+            The name of the station.
+
+        Returns
+        -------
+        metobs_toolkit.Station
+            The station object.
 
         """
+        from metobs_toolkit.station import Station
 
-        logger.info(f'Extract {stationname} from dataset.')
+        logger.info(f"Extract {stationname} from dataset.")
 
         # important: make shure all station attributes are of the same time as dataset.
         # so that all methods can be inherited.
 
         try:
-            sta_df = self.df.xs(stationname, level='name', drop_level=False)
+            sta_df = self.df.xs(stationname, level="name", drop_level=False)
             sta_metadf = self.metadf.loc[stationname].to_frame().transpose()
         except KeyError:
-            logger.warning(f'{stationname} not found in the dataset.')
-            print(f'{stationname} not found in the dataset.')
+            logger.warning(f"{stationname} not found in the dataset.")
+            print(f"{stationname} not found in the dataset.")
             return None
 
         try:
             sta_outliers = self.outliersdf.xs(
-                stationname, level='name', drop_level=False)
+                stationname, level="name", drop_level=False
+            )
         except KeyError:
             sta_outliers = init_multiindexdf()
 
         sta_gaps = self.gaps.get_station_gaps(stationname)
         sta_missingobs = self.missing_obs.get_station_missingobs(stationname)
 
         try:
-            sta_gapfill=self.gapfilldf.xs(
-                stationname, level='name', drop_level=False)
+            sta_gapfill = self.gapfilldf.xs(stationname, level="name", drop_level=False)
         except KeyError:
             sta_gapfill = init_multiindexdf()
 
-        return Station(name=stationname,
-                       df=sta_df,
-                       outliersdf=sta_outliers,
-                       gaps=sta_gaps,
-                       missing_obs=sta_missingobs,
-                       gapfilldf=sta_gapfill,
-                       metadf=sta_metadf,
-                       data_template=self.data_template,
-                       settings = self.settings)
+        try:
+            sta_missingfill = self.missing_fill_df.xs(stationname, level="name", drop_level=False)
+        except KeyError:
+            sta_missingfill = init_multiindexdf()
+
+        return Station(
+            name=stationname,
+            df=sta_df,
+            outliersdf=sta_outliers,
+            gaps=sta_gaps,
+            missing_obs=sta_missingobs,
+            gapfilldf=sta_gapfill,
+            missing_fill_df = sta_missingfill,
+            metadf=sta_metadf,
+            data_template=self.data_template,
+            settings=self.settings,
+            _qc_checked_obstypes=self._qc_checked_obstypes,
+            _applied_qc=self._applied_qc,
+        )
 
     def show(self):
         """
         A function to print out some overview information about the Dataset.
 
-        :return: No return
-        :rtype: No return
+        Returns
+        -------
+        None.
+
         """
 
-        logger.info('Show basic info of dataset.')
+        logger.info("Show basic info of dataset.")
 
         try:
             gapsdf = self.gaps.to_df()
         except:
-            gapsdf=init_multiindexdf()
+            gapsdf = init_multiindexdf()
 
+        if self.missing_obs is None:
+            missing_obs_series = pd.Series(dtype=object)
+        else:
+            missing_obs_series = self.missing_obs.series
 
-        print_dataset_info(self.df, self.outliersdf, gapsdf,
-                           self.settings.app['print_fmt_datetime'])
-
-    def make_plot(self, stationnames=None, obstype='temp', colorby='name',
-                  starttime=None, endtime=None,
-                  title=None, legend=True, show_outliers=True):
+        print_dataset_info(
+            self.df,
+            self.outliersdf,
+            gapsdf,
+            missing_obs_series,
+            self.settings.app["print_fmt_datetime"],
+        )
+
+    def make_plot(
+        self,
+        stationnames=None,
+        obstype="temp",
+        colorby="name",
+        starttime=None,
+        endtime=None,
+        title=None,
+        legend=True,
+        show_outliers=True,
+    ):
         """
         This function creates a timeseries plot for the dataset. The variable observation type
         is plotted for all stationnames from a starttime to an endtime.
 
 
-        :param stationnames: A list with stationnames to include in the timeseries. If None is given, all the stations are used, defaults to None.
-        :type stationnames: list or None, optional
-        :param obstype: The observation type to plot, defaults to 'temp'.
-        :type variable: String, optional
-        :param colorby: Indicate how colors should be assigned to the lines. 'label' will color the lines by their quality control label. 'name' will color by each station, defaults to 'name'.
-        :type colorby: 'label' or 'name', optional
-        :param starttime: Specifiy the start datetime for the plot. If None is given it will use the start datetime of the dataset, defaults to None.
-        :type starttime: datetime.datetime, optional
-        :param endtime: Specifiy the end datetime for the plot. If None is given it will use the end datetime of the dataset, defaults to None.
-        :type endtime: datetime.datetime, optional
-        :param title: The title for the plot. If None is given a default title is used, defaults to None.
-        :type title: String, optional
-        :param legend: When thrue a legend is added to the plot, defaults to True
-        :type legend: Boolean, optional
-        :param show_outliers: If true the observations labeld as outliers will be included in the plot, defaults to True
-        :type show_outliers: boolean, optional
-        :return: The plot axis
-        :rtype: matplotlib.pyplot.axis
+         All styling attributes are extracted from the Settings.
+
+         Parameters
+         ----------
+         stationnames : list, optional
+             A list with stationnames to include in the timeseries. If None is given, all the stations are used, defaults to None.
+         obstype : string, optional
+             Fieldname to visualise. This can be an observation or station
+             attribute. The default is 'temp'.
+         colorby : 'label' or 'name', optional
+             Indicate how colors should be assigned to the lines. 'label' will color the lines by their quality control label. 'name' will color by each station, defaults to 'name'.
+         starttime : datetime.datetime, optional
+             Specifiy the start datetime for the plot. If None is given it will use the start datetime of the dataset, defaults to None.
+         endtime : datetime.datetime, optional
+             Specifiy the end datetime for the plot. If None is given it will use the end datetime of the dataset, defaults to None.
+         title : string, optional
+             Title of the figure, if None a default title is generated. The default is None.
+         legend : bool, optional
+             I True, a legend is added to the plot. The default is True.
+         show_outliers : bool, optional
+             If true the observations labeld as outliers will be included in the plot, defaults to True
+
+
+         Returns
+         -------
+         axis : matplotlib.pyplot.axes
+             The timeseries axes of the plot is returned.
 
         """
 
-        logger.info(f'Make {obstype}-timeseries plot for {stationnames}')
+        logger.info(f"Make {obstype}-timeseries plot for {stationnames}")
 
         # combine all dataframes
         mergedf = self.combine_all_to_obsspace()
 
         # Subset on stationnames
-        if not isinstance(stationnames, type(None)):
-            mergedf = mergedf.loc[mergedf.index.get_level_values(
-                'name').isin(stationnames)]
+        if not stationnames is None:
+            mergedf = mergedf.loc[
+                mergedf.index.get_level_values("name").isin(stationnames)
+            ]
 
         # Subset on start and endtime
         mergedf = multiindexdf_datetime_subsetting(mergedf, starttime, endtime)
 
         # Get plot styling attributes
-        if isinstance(title, type(None)):
-            if isinstance(stationnames, type(None)):
-                if self._istype == 'Dataset':
-                    title = self.settings.app['display_name_mapper'][obstype] + \
-                        ' for all stations. '
-                elif self._istype == 'Station':
-                    title = self.settings.app['display_name_mapper'][obstype] + \
-                        ' of ' + self.name
+        if title is None:
+            if stationnames is None:
+                if self._istype == "Dataset":
+                    title = (
+                        self.settings.app["display_name_mapper"][obstype]
+                        + " for all stations. "
+                    )
+                elif self._istype == "Station":
+                    title = (
+                        self.settings.app["display_name_mapper"][obstype]
+                        + " of "
+                        + self.name
+                    )
 
             else:
-                title = self.settings.app['display_name_mapper'][obstype] + \
-                    ' for stations: ' + str(stationnames)
-
-        if ((obstype+'_final_label' not in mergedf.columns) &
-            ((colorby == 'label') | (show_outliers))):
+                title = (
+                    self.settings.app["display_name_mapper"][obstype]
+                    + " for stations: "
+                    + str(stationnames)
+                )
+
+        if (obstype + "_final_label" not in mergedf.columns) & (
+            (colorby == "label") | (show_outliers)
+        ):
             # user whant outier information but no QC is applied on this obstype
-            print(f' No quality control is applied on {obstype}! \
-                  No outlier information is available.')
-            print('Colorby is set to "name" and show_outliers \
-                  is set to False.')
-            colorby = 'name'
+            print(
+                f" No quality control is applied on {obstype}! \
+                  No outlier information is available."
+            )
+            print(
+                'Colorby is set to "name" and show_outliers \
+                  is set to False.'
+            )
+            colorby = "name"
             show_outliers = False
 
         # Make plot
-        ax = timeseries_plot(mergedf=mergedf,
-                             obstype=obstype,
-                             title=title,
-                             xlabel='Timestamp',
-                             ylabel=self.data_template[obstype]['orig_name'],
-                             colorby=colorby,
-                             show_legend=legend,
-                             show_outliers=show_outliers,
-                             plot_settings = self.settings.app['plot_settings'],
-                             gap_settings = self.settings.gap,
-                             qc_info_settings=self.settings.qc['qc_checks_info'])
+        ax = timeseries_plot(
+            mergedf=mergedf,
+            obstype=obstype,
+            title=title,
+            xlabel="Timestamp",
+            ylabel=self.data_template[obstype]["orig_name"],
+            colorby=colorby,
+            show_legend=legend,
+            show_outliers=show_outliers,
+            plot_settings=self.settings.app["plot_settings"],
+            gap_settings=self.settings.gap,
+            qc_info_settings=self.settings.qc["qc_checks_info"],
+        )
 
         return ax
 
-    def make_geo_plot(self, obstype='temp', title=None,
-                      timeinstance=None, legend=True,
-                      vmin=None, vmax=None):
+    def make_geo_plot(
+        self,
+        obstype="temp",
+        title=None,
+        timeinstance=None,
+        legend=True,
+        vmin=None,
+        vmax=None,
+    ):
         """
         This functions creates a geospatial plot for a field
         (observations or attributes) of all stations.
 
         If the field is timedepending, than the timeinstance is used to plot
         the field status at that datetime.
 
         If the field is categorical than the leged will have categorical
         values, else a colorbar is used.
 
         All styling attributes are extracted from the Settings.
 
-
         Parameters
-
-        variable : String, optional
+        ----------
+        obstype : string, optional
             Fieldname to visualise. This can be an observation or station
             attribute. The default is 'temp'.
-        title : String, optional
-            Title of the figure, if None a default title is generated. The
-            default is None.
-        timeinstance : datetime, optional
-            Datetime moment of the geospatial plot. The default is None and the
-            first datetime available is used.
-        legend : Bool, optional
-            Add legend to the figure. The default is True.
-        vmin : float, optional
-            The minimum value corresponding to the minimum color.
-            The default is None and the minimum of the variable is used.
-        vmax : float, optional
-           The maximum value corresponding to the minimum color. The default is
-           None and the maximum of the variable is used.
+        title : string, optional
+            Title of the figure, if None a default title is generated. The default is None.
+        timeinstance : datetime.datetime, optional
+            Datetime moment of the geospatial plot. If None, the first available datetime is used. The default is None.
+        legend : bool, optional
+            I True, a legend is added to the plot. The default is True.
+        vmin : numeric, optional
+            The value corresponding with the minimum color. If None, the minimum of the presented observations is used. The default is None.
+        vmax : numeric, optional
+            The value corresponding with the maximum color. If None, the maximum of the presented observations is used. The default is None.
 
         Returns
-
-        ax : Geoaxes
-            The geoaxes is returned.
+        -------
+        axis : matplotlib.pyplot.geoaxes
+            The geoaxes of the plot is returned.
 
         """
 
         # Load default plot settings
         # default_settings=Settings.plot_settings['spatial_geo']
 
         # get first timeinstance of the dataset if not given
-        if isinstance(timeinstance, type(None)):
-            timeinstance = self.df.index.get_level_values('datetime').min()
+        if timeinstance is None:
+            timeinstance = self.df.index.get_level_values("datetime").min()
 
-        logger.info(f'Make {obstype}-geo plot at {timeinstance}')
+        logger.info(f"Make {obstype}-geo plot at {timeinstance}")
 
         # subset to timeinstance
-        plotdf = self.df.xs(timeinstance, level='datetime')
+        plotdf = self.df.xs(timeinstance, level="datetime")
 
         # merge metadata
-        plotdf = plotdf.merge(self.metadf, how='left',
-                              left_index=True, right_index=True)
-
-        axis = geospatial_plot(plotdf=plotdf,
-                             variable=obstype,
-                             timeinstance=timeinstance,
-                             title=title,
-                             legend=legend,
-                             vmin=vmin,
-                             vmax=vmax,
-                             plotsettings=self.settings.app['plot_settings'],
-                             categorical_fields=self.settings.app['categorical_fields'],
-                             static_fields = self.settings.app['static_fields'],
-                             display_name_mapper=self.settings.app['display_name_mapper'],
-                             world_boundaries_map = self.settings.app['world_boundary_map'])
+        plotdf = plotdf.merge(
+            self.metadf, how="left", left_index=True, right_index=True
+        )
+
+        axis = geospatial_plot(
+            plotdf=plotdf,
+            variable=obstype,
+            timeinstance=timeinstance,
+            title=title,
+            legend=legend,
+            vmin=vmin,
+            vmax=vmax,
+            plotsettings=self.settings.app["plot_settings"],
+            categorical_fields=self.settings.app["categorical_fields"],
+            static_fields=self.settings.app["static_fields"],
+            display_name_mapper=self.settings.app["display_name_mapper"],
+            world_boundaries_map=self.settings.app["world_boundary_map"],
+        )
 
         return axis
+
     # =============================================================================
     #   Gap Filling
     # =============================================================================
-    def get_modeldata(self, modelname='ERA5_hourly', stations=None, startdt=None, enddt=None):
+    def get_modeldata(
+        self, modelname="ERA5_hourly", stations=None, startdt=None, enddt=None
+    ):
+        """
+        Make a metobs_toolkit.Modeldata object with modeldata at the locations
+        of the stations present in the dataset.
+
+        Parameters
+        ----------
+        modelname : 'ERA5_hourly', optional
+            Which dataset to download timeseries from. The default is 'ERA5_hourly'.
+        stations : string or list of strings, optional
+            Stationnames to subset the modeldata to. If None, all stations will be used. The default is None.
+        startdt : datetime.datetime, optional
+            Start datetime of the model timeseries. If None, the start datetime of the dataset is used. The default is None.
+        enddt : datetime.datetime, optional
+            End datetime of the model timeseries. If None, the last datetime of the dataset is used. The default is None.
+
+        Returns
+        -------
+        Modl : metobs_toolkit.Modeldata
+            The extracted modeldata for period and a set of stations.
+
+        """
+
         Modl = Modeldata(modelname)
 
-        #Filters
-        if isinstance(startdt, type(None)):
-            startdt=self.df.index.get_level_values('datetime').min()
-        if isinstance(enddt, type(None)):
-            enddt=self.df.index.get_level_values('datetime').max()
-        if not isinstance(stations, type(None)):
+        # Filters
+        if startdt is None:
+            startdt = self.df.index.get_level_values("datetime").min()
+        if enddt is None:
+            enddt = self.df.index.get_level_values("datetime").max()
+        if not stations is None:
             if isinstance(stations, str):
-                metadf=self.metadf.loc[[stations]]
+                metadf = self.metadf.loc[[stations]]
             if isinstance(stations, list):
                 metadf = self.metadf.iloc[self.metadf.index.isin(stations)]
         else:
             metadf = self.metadf
 
-
         # fill modell with data
-        if modelname == 'ERA5_hourly':
+        if modelname == "ERA5_hourly":
             Modl.get_ERA5_data(metadf, startdt, enddt)
 
             return Modl
         else:
             print(f"{modelname} for set_modeldata is not implemented yet")
             return None
 
     # =============================================================================
     #   Gap Filling
     # =============================================================================
 
-    def fill_gaps_linear(self, obstype='temp'):
-        #TODO logging
-        fill_settings =self.settings.gap['gaps_fill_settings']['linear']
-        fill_info = self.settings.gap['gaps_fill_info']
+    def fill_gaps_linear(self, obstype="temp"):
+        """
+        Fill the gaps using linear interpolation.
 
+        Parameters
+        ----------
+        obstype : string, optional
+            Fieldname to visualise. This can be an observation or station
+            attribute. The default is 'temp'.
+
+        Returns
+        -------
+        None.
+
+        """
+        # TODO logging
+        fill_settings = self.settings.gap["gaps_fill_settings"]["linear"]
+        fill_info = self.settings.gap["gaps_fill_info"]
 
-        #fill gaps
+        # fill gaps
         self.gapfilldf[obstype] = self.gaps.apply_interpolate_gaps(
-                                    obsdf = self.df,
-                                    outliersdf = self.outliersdf,
-                                    dataset_res=self.metadf['dataset_resolution'],
-                                    obstype=obstype,
-                                    method=fill_settings['method'],
-                                    max_consec_fill=fill_settings['max_consec_fill'])
+            obsdf=self.df,
+            outliersdf=self.outliersdf,
+            dataset_res=self.metadf["dataset_resolution"],
+            obstype=obstype,
+            method=fill_settings["method"],
+            max_consec_fill=fill_settings["max_consec_fill"],
+        )
 
-        #add label column
-        self.gapfilldf[obstype + '_' + fill_info['label_columnname']] = fill_info['label']['linear']
+        # add label column
+        self.gapfilldf[obstype + "_" + fill_info["label_columnname"]] = fill_info[
+            "label"
+        ]["linear"]
 
+    def fill_missing_obs_linear(self, obstype='temp'):
+        # TODO logging
+        fill_settings = self.settings.missing_obs['missing_obs_fill_settings']['linear']
+        fill_info = self.settings.missing_obs['missing_obs_fill_info']
 
-    def fill_gaps_era5(self, modeldata, method='debias', obstype='temp', overwrite=True):
 
-        fill_info = self.settings.gap['gaps_fill_info']
+
+        # fill missing obs
+        self.missing_obs.interpolate_missing(
+                                            obsdf=self.df,
+                                            resolutionseries=self.metadf["dataset_resolution"],
+                                            obstype=obstype,
+                                            method=fill_settings["method"],
+        )
+        missing_fill_df = self.missing_obs.fill_df
+        missing_fill_df[obstype+'_' + fill_info["label_columnname"]] = fill_info["label"]["linear"]
+
+        # Update attribute
+
+        self.missing_fill_df = missing_fill_df
+
+
+
+    def get_analysis(self):
+        """
+        Create a MetObs_toolkit.Analysis instance from the Dataframe
+
+        Returns
+        -------
+        metobs_toolkit.Analysis
+            The Analysis instance of the Dataset.
+
+        """
+
+        return Analysis(obsdf = self.df,
+                        metadf = self.metadf,
+                        settings = self.settings,
+                        data_template=self.data_template)
+
+
+    def fill_gaps_era5(
+        self, modeldata, method="debias", obstype="temp", overwrite=True
+    ):
+        """
+        Fill the gaps using a metobs_toolkit.Modeldata object.
+
+
+        Parameters
+        ----------
+        modeldata : metobs_toolkit.Modeldata
+            The modeldata to use for the gapfill. This model data should the required
+            timeseries to fill all gaps present in the dataset.
+        method : 'debias', optional
+            Specify which method to use. The default is 'debias'.
+        obstype : TYPE, optional
+            Fieldname to visualise. This can be an observation or station
+            attribute. The default is 'temp'.
+        overwrite : bool, optional
+            If True, the Dataset.Gapfilldf will be overwritten. The default is True.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        fill_info = self.settings.gap["gaps_fill_info"]
 
         # check if modeldata is available
-        if isinstance(modeldata, type(None)):
-            print('The dataset has no modeldate. Use the set_modeldata() function to add modeldata.')
+        if modeldata is None:
+            print(
+                "The dataset has no modeldate. Use the set_modeldata() function to add modeldata."
+            )
             return None
         # check if obstype is present in eramodel
-        assert obstype in modeldata.df.columns, f'{obstype} is not present in the modeldate: {modeldata}'
+        assert (
+            obstype in modeldata.df.columns
+        ), f"{obstype} is not present in the modeldate: {modeldata}"
         # check if all station are present in eramodeldata
         stations = self.gaps.to_df().index.unique().to_list()
-        assert all([sta in modeldata.df.index.get_level_values('name') for sta in stations]),\
-            f'Not all stations with gaps are in the modeldata!'
+        assert all(
+            [sta in modeldata.df.index.get_level_values("name") for sta in stations]
+        ), f"Not all stations with gaps are in the modeldata!"
 
         if not self.gapfilldf.empty:
             if overwrite:
-                print('Gapfilldf will be overwritten!')
+                print("Gapfilldf will be overwritten!")
                 self.gapfilldf = init_multiindexdf()
             else:
                 print('Gapfilldf is not empty, set "overwrite=True" to overwrite it!')
-                print('CANCEL gap fill with ERA5')
+                print("CANCEL gap fill with ERA5")
                 return
 
-
-
-
-        if method=='debias':
-            test = self.gaps.apply_debias_era5_gapfill(dataset=self,
-                                                       eraModelData=modeldata,
-                                                       obstype=obstype,
-                                                       debias_settings=self.settings.gap['gaps_fill_settings']['model_debias'])
+        if method == "debias":
+            test = self.gaps.apply_debias_era5_gapfill(
+                dataset=self,
+                eraModelData=modeldata,
+                obstype=obstype,
+                debias_settings=self.settings.gap["gaps_fill_settings"]["model_debias"],
+            )
 
             self.gapfilldf[obstype] = test
-            #add label column
-            self.gapfilldf[obstype + '_' + fill_info['label_columnname']] = fill_info['label']['model_debias']
+            # add label column
+            self.gapfilldf[obstype + "_" + fill_info["label_columnname"]] = fill_info[
+                "label"
+            ]["model_debias"]
         else:
-            print('not implemented yet')
-
-
+            print("not implemented yet")
 
-    def write_to_csv(self, filename=None, include_outliers=True,
-                     include_gapfill=True,
-                     add_final_labels=True, use_tlk_obsnames=True):
-        """
-            Write the dataset to a file where the observations, metadata and
-            (if available) the quality labels per observation type are merged
-            together.
-
-            A final qualty controll label for each
-            quality-controlled-observation type can be added in the outputfile.
-
-            The file will be writen to the Settings.outputfolder.
+    def write_to_csv(
+        self,
+        filename=None,
+        include_outliers=True,
+        include_gapfill=True,
+        add_final_labels=True,
+        use_tlk_obsnames=True,
+    ):
+        """
+        Write the dataset to a file where the observations, metadata and
+        (if available) the quality labels per observation type are merged
+        together.
 
-            Parameters
+        A final qualty control label for each
+        quality-controlled-observation type can be added in the outputfile.
 
-            filename : string, optional
-                The name of the output csv file. If none, a standard-filename
-                is generated based on the period of data. The default is None.
-            add_final_labels : Bool, optional
-                If True, a final qualty control label per observation type
-                is added as a column. The default is True.
+        The file will be writen to the outputfolder specified in the settings.
 
-            Returns
+        Parameters
+        ----------
+        filename : string, optional
+            The name of the output csv file. If none, a standard-filename
+            is generated based on the period of data. The default is None.
+        include_outliers : bool, optional
+            If True, the outliers will be present in the csv file. The default is True.
+        include_gapfill : bool, optional
+            If True, the filled gap values will be present in the csv file. The default is True.
+        add_final_labels : bool, optional
+            If True, a column is added containing the final label of an observation. The default is True.
+        use_tlk_obsnames : bool, optional
+            If True, the standard naming of the metobs_toolkit is used, else
+            the original names for obstypes is used. The default is True.
 
-            None
+        Returns
+        -------
+        None.
 
-            """
+        """
 
-        logger.info('Writing the dataset to a csv file')
+        logger.info("Writing the dataset to a csv file")
 
-        assert not isinstance(self.settings.IO['output_folder'], type(None)), 'Specify \
-            Settings.output_folder in order to export a csv.'
-        assert os.path.isdir(self.settings.IO['output_folder']), f'The outputfolder: \
+        assert (
+            not self.settings.IO["output_folder"] is None
+        ), "Specify Settings.output_folder in order to export a csv."
+
+        assert os.path.isdir(
+            self.settings.IO["output_folder"]
+        ), f'The outputfolder: \
             {self.settings.IO["output_folder"]} is not found. '
 
         # combine all dataframes
         mergedf = self.combine_all_to_obsspace()  # with outliers
 
         # select which columns to keep
         if include_outliers:
             if not add_final_labels:
-                _fin_cols = [col for col in mergedf.columns
-                             if col.endswith('_final_label')]
+                _fin_cols = [
+                    col for col in mergedf.columns if col.endswith("_final_label")
+                ]
                 mergedf = mergedf.drop(columns=_fin_cols)
 
         else:  # exclude outliers
             if add_final_labels:
-                cols_to_keep = [col for col in mergedf.columns
-                                if col in self.settings.app['observation_types']]
-                cols_to_keep.extend([col for col in mergedf.columns
-                                     if col.endswith('_final_label')])
+                cols_to_keep = [
+                    col for col in mergedf.columns if col in observation_types
+                ]
+                cols_to_keep.extend(
+                    [col for col in mergedf.columns if col.endswith("_final_label")]
+                )
                 mergedf = mergedf[cols_to_keep]
 
         if not include_gapfill:
             # locate all filled values
-            filled_df =  init_multiindexdf()
-            final_columns = [col for col in mergedf.columns if col.endswith('_final_label')]
+            filled_df = init_multiindexdf()
+            final_columns = [
+                col for col in mergedf.columns if col.endswith("_final_label")
+            ]
             for final_column in final_columns:
-                filled_df = pd.concat([filled_df,
-                                       mergedf.loc[mergedf[final_column] ==
-                                                   self.settings.gaps['gaps_fill_info']['label']]])
+                filled_df = pd.concat(
+                    [
+                        filled_df,
+                        mergedf.loc[
+                            mergedf[final_column]
+                            == self.settings.gaps["gaps_fill_info"]["label"]
+                        ],
+                    ]
+                )
 
             # drop filled values from mergedf
-            mergedf = mergedf.drop(filled_df.index, errors='ignore')
+            mergedf = mergedf.drop(filled_df.index, errors="ignore")
 
-            #fill with numpy nan
-            nan_columns = {col: np.nan for col in mergedf.columns if col in self.settings.app['observation_types']}
+            # fill with numpy nan
+            nan_columns = {
+                col: np.nan for col in mergedf.columns if col in observation_types
+            }
             filled_df = filled_df.assign(**nan_columns)
             # rename label
-            filled_df = filled_df.replace({self.settings.gaps['gaps_fill_info']['label']: self.settings.gaps['gaps_info']['gap']['outlier_flag']})
-            #add to mergedf
+            filled_df = filled_df.replace(
+                {
+                    self.settings.gaps["gaps_fill_info"]["label"]: self.settings.gaps[
+                        "gaps_info"
+                    ]["gap"]["outlier_flag"]
+                }
+            )
+            # add to mergedf
             mergedf = pd.concat([mergedf, filled_df]).sort_index()
 
-
-
-
-
+        present_obstypes = [col for col in observation_types if col in mergedf.columns]
 
         # Map obstypes columns
         if not use_tlk_obsnames:
             # TODO
-            print('not implemented yet')
+            print("not implemented yet")
 
         # TODO Convert units if needed.
 
         # columns to write
-        write_dataset_to_csv(df=mergedf,
-                             metadf=self.metadf,
-                             filename=filename,
-                             outputfolder = self.settings.IO['output_folder'],
-                             location_info = self.settings.app['location_info'],
-                             observation_types=self.settings.app['observation_types']
-                             )
-
+        write_dataset_to_csv(
+            df=mergedf,
+            metadf=self.metadf,
+            filename=filename,
+            outputfolder=self.settings.IO["output_folder"],
+            location_info=self.settings.app["location_info"],
+            observation_types=present_obstypes,
+        )
 
     # =============================================================================
     #     Quality control
     # =============================================================================
 
-    def apply_quality_control(self, obstype='temp',
-                              gross_value=True,
-                              persistance=True,
-                              repetitions=True,
-                              step=True,
-                              window_variation=True,
-                              # internal_consistency=True,
-                              ):
-        """
-        Apply quality control methods to the dataset. The default settings
-        are used, and can be changed in the settings_files/qc_settings.py
-
-        The checks are performed in a sequence: gross_vallue -->
-        persistance --> ..., Outliers by a previous check are ignored in the
-        following checks!
+    def apply_quality_control(
+        self,
+        obstype="temp",
+        gross_value=True,
+        persistance=True,
+        repetitions=True,
+        step=True,
+        window_variation=True,
+        # internal_consistency=True,
+    ):
+        """
+         Apply quality control methods to the dataset.
+
+         The default settings are used, and can be changed in the
+         settings_files/qc_settings.py
+
+         The checks are performed in a sequence: gross_vallue -->
+         persistance --> ..., Outliers by a previous check are ignored in the
+         following checks!
+
+         The dataset is updated inline.
+
+         Parameters
+         ----------
+         obstype : String, optional
+             Name of the observationtype you want to apply the checks on. The
+             default is 'temp'.
+         gross_value : Bool, optional
+             If True the gross_value check is applied if False not. The default
+             is True.
+         persistance : Bool, optional
+            If True the persistance check is applied if False not. The default
+            is True.. The default is True.
+         step : Bool, optional
+            If True the step check is applied if False not. The default is True.
+        internal_consistency : Bool, optional
+            If True the internal consistency check is applied if False not. The
+            default is True.
+        qc_info: Bool, optional
+            If True info about the quality control is printed if False not. The
+            default is True.
+         ignore_val : numeric, optional
+             Values to ignore in the quality checks. The default is np.nan.
 
-        The dataset is updated inline.
+         Returns
 
-        Parameters
-
-        obstype : String, optional
-            Name of the observationtype you want to apply the checks on. The
-            default is 'temp'.
-        gross_value : Bool, optional
-            If True the gross_value check is applied if False not. The default
-            is True.
-        persistance : Bool, optional
-           If True the persistance check is applied if False not. The default
-           is True.. The default is True.
-        step : Bool, optional
-           If True the step check is applied if False not. The default is True.
-       internal_consistency : Bool, optional
-           If True the internal consistency check is applied if False not. The
-           default is True.
-       qc_info: Bool, optional
-           If True info about the quality control is printed if False not. The
-           default is True.
-        ignore_val : numeric, optional
-            Values to ignore in the quality checks. The default is np.nan.
-
-        Returns
-
-        None.
+         None.
 
         """
 
         if repetitions:
-
-            print('Applying the repetitions-check on all stations.')
-            logger.info('Applying repetitions check on the full dataset')
+            print("Applying the repetitions-check on all stations.")
+            logger.info("Applying repetitions check on the full dataset")
 
             obsdf, outl_df = repetitions_check(
-                                            obsdf=self.df,
-                                            obstype=obstype,
-                                            checks_info=self.settings.qc['qc_checks_info'],
-                                            checks_settings = self.settings.qc['qc_check_settings'])
+                obsdf=self.df,
+                obstype=obstype,
+                checks_info=self.settings.qc["qc_checks_info"],
+                checks_settings=self.settings.qc["qc_check_settings"],
+            )
 
             # update the dataset and outliers
             self.df = obsdf
             if not outl_df.empty:
-                self.update_outliersdf(outl_df)
+                self.outliersdf = pd.concat([self.outliersdf, outl_df])
+
+            # add this check to the applied checks
+            self._applied_qc = pd.concat(
+                [
+                    self._applied_qc,
+                    conv_applied_qc_to_df(
+                        obstypes=obstype, ordered_checknames="repetitions"
+                    ),
+                ],
+                ignore_index=True,
+            )
 
         if gross_value:
-            print('Applying the gross-value-check on all stations.')
-            logger.info('Applying gross value check on the full dataset')
+            print("Applying the gross-value-check on all stations.")
+            logger.info("Applying gross value check on the full dataset")
 
             obsdf, outl_df = gross_value_check(
-                                            obsdf=self.df,
-                                            obstype=obstype,
-                                            checks_info=self.settings.qc['qc_checks_info'],
-                                            checks_settings = self.settings.qc['qc_check_settings'])
+                obsdf=self.df,
+                obstype=obstype,
+                checks_info=self.settings.qc["qc_checks_info"],
+                checks_settings=self.settings.qc["qc_check_settings"],
+            )
 
             # update the dataset and outliers
             self.df = obsdf
             if not outl_df.empty:
-                self.update_outliersdf(outl_df)
+                self.outliersdf = pd.concat([self.outliersdf, outl_df])
+
+            # add this check to the applied checks
+            self._applied_qc = pd.concat(
+                [
+                    self._applied_qc,
+                    conv_applied_qc_to_df(
+                        obstypes=obstype, ordered_checknames="gross_value"
+                    ),
+                ],
+                ignore_index=True,
+            )
 
         if persistance:
-            print('Applying the persistance-check on all stations.')
-            logger.info('Applying persistance check on the full dataset')
+            print("Applying the persistance-check on all stations.")
+            logger.info("Applying persistance check on the full dataset")
 
             obsdf, outl_df = persistance_check(
-                        station_frequencies=self.metadf['dataset_resolution'],
-                        obsdf=self.df,
-                        obstype=obstype,
-                        checks_info=self.settings.qc['qc_checks_info'],
-                        checks_settings = self.settings.qc['qc_check_settings'])
+                station_frequencies=self.metadf["dataset_resolution"],
+                obsdf=self.df,
+                obstype=obstype,
+                checks_info=self.settings.qc["qc_checks_info"],
+                checks_settings=self.settings.qc["qc_check_settings"],
+            )
 
             # update the dataset and outliers
             self.df = obsdf
             if not outl_df.empty:
-                self.update_outliersdf(outl_df)
+                self.outliersdf = pd.concat([self.outliersdf, outl_df])
 
-        if step:
-            print('Applying the step-check on all stations.')
-            logger.info('Applying step-check on the full dataset')
+            # add this check to the applied checks
+            self._applied_qc = pd.concat(
+                [
+                    self._applied_qc,
+                    conv_applied_qc_to_df(
+                        obstypes=obstype, ordered_checknames="persistance"
+                    ),
+                ],
+                ignore_index=True,
+            )
 
-            obsdf, outl_df = step_check(obsdf=self.df,
-                                        obstype=obstype,
-                                        checks_info=self.settings.qc['qc_checks_info'],
-                                        checks_settings = self.settings.qc['qc_check_settings'])
+        if step:
+            print("Applying the step-check on all stations.")
+            logger.info("Applying step-check on the full dataset")
 
+            obsdf, outl_df = step_check(
+                obsdf=self.df,
+                obstype=obstype,
+                checks_info=self.settings.qc["qc_checks_info"],
+                checks_settings=self.settings.qc["qc_check_settings"],
+            )
 
             # update the dataset and outliers
             self.df = obsdf
-            if  not outl_df.empty:
-                self.update_outliersdf(outl_df)
+            if not outl_df.empty:
+                self.outliersdf = pd.concat([self.outliersdf, outl_df])
+
+            # add this check to the applied checks
+            self._applied_qc = pd.concat(
+                [
+                    self._applied_qc,
+                    conv_applied_qc_to_df(obstypes=obstype, ordered_checknames="step"),
+                ],
+                ignore_index=True,
+            )
 
         if window_variation:
-            print('Applying the window variation-check on all stations.')
-            logger.info('Applying window variation-check on the full dataset')
+            print("Applying the window variation-check on all stations.")
+            logger.info("Applying window variation-check on the full dataset")
 
             obsdf, outl_df = window_variation_check(
-                        station_frequencies=self.metadf['dataset_resolution'],
-                        obsdf=self.df,
-                        obstype=obstype,
-                        checks_info=self.settings.qc['qc_checks_info'],
-                        checks_settings = self.settings.qc['qc_check_settings'])
-
+                station_frequencies=self.metadf["dataset_resolution"],
+                obsdf=self.df,
+                obstype=obstype,
+                checks_info=self.settings.qc["qc_checks_info"],
+                checks_settings=self.settings.qc["qc_check_settings"],
+            )
 
             # update the dataset and outliers
             self.df = obsdf
             if not outl_df.empty:
-                self.update_outliersdf(outl_df)
+                self.outliersdf = pd.concat([self.outliersdf, outl_df])
 
+            # add this check to the applied checks
+            self._applied_qc = pd.concat(
+                [
+                    self._applied_qc,
+                    conv_applied_qc_to_df(
+                        obstypes=obstype, ordered_checknames="window_variation"
+                    ),
+                ],
+                ignore_index=True,
+            )
 
+        self._qc_checked_obstypes.append(obstype)
+        self._qc_checked_obstypes = list(set(self._qc_checked_obstypes))
         self.outliersdf = self.outliersdf.sort_index()
 
-
-
-    def combine_all_to_obsspace(self):
+    def combine_all_to_obsspace(self, repr_outl_as_nan=False):
         """
         Combine observations, outliers, gaps and missing timesteps to one
         dataframe in the resolution of the dataset. Final quality labels are
         calculated for all checked obstypes.
 
         If an observation value exist for an outlier, it will be used in the
         corresponding obstype column.
@@ -725,97 +948,154 @@
         Returns
 
         comb_df : pandas.DataFrame()
             Multi index dataframe with observations and labels.
 
         """
 
-
+        # =============================================================================
+        # Unstack outliers to regular multiindex
+        # =============================================================================
         outliersdf = self.outliersdf
 
-        # if outliersdf is empty, create columns with 'not checked'
-        if outliersdf.empty:
-            outliercolumns = [col['label_columnname']
-                              for col in self.settings.qc['qc_checks_info'].values()]
+        # remove duplicate indixes (needed for update)
+        outliersdf = outliersdf[~outliersdf.index.duplicated(keep="first")]
+
+        if not outliersdf.empty:
+            outliersdf_values = outliersdf["value"].unstack()  # for later use
+            # convert to wide df with labels
+            outliersdf = outliersdf["label"].unstack()
+
+            # convert to final label names for columns
+            outliersdf = outliersdf.rename(
+                columns={col: col + "_final_label" for col in outliersdf.columns}
+            )
+
+        else:
+            outliersdf = init_multiindexdf()
+            outliersdf_values = init_multiindexdf()  # for later use
+            outliercolumns = [
+                col + "_final_label" for col in self.df if col in observation_types
+            ]
             for column in outliercolumns:
-                outliersdf[column] = 'not checked'
-        # get final label
-        outliersdf = add_final_label_to_outliersdf(
-                        outliersdf=self.outliersdf,
-                        data_res_series=self.metadf['dataset_resolution'],
-                        observation_types=self.settings.app['observation_types'],
-                        checks_info=self.settings.qc['qc_checks_info'])
+                outliersdf[column] = "not checked"
 
-        #remove duplicate indixes (needed for update)
-        outliersdf = outliersdf[~outliersdf.index.duplicated(keep='first')]
+        # =============================================================================
+        # Combine observations and outliers
+        # =============================================================================
+        # get observations
+        df = self.df
+
+        # 0. make shure there is a final column for each obstype in the df,
+        # if qc did not found any outliers, then there is apriori no final label column
+        present_obstypes = [col for col in observation_types if col in df.columns]
+        for presen_obstype in present_obstypes:
+            final_label = presen_obstype + "_final_label"
+            if not final_label in outliersdf.columns:
+                outliersdf[final_label] = np.nan
+
+        # 1. Merge the label columns
+        df_and_outl = df.merge(
+            outliersdf, how="outer", left_index=True, right_index=True
+        )
+
+        # 2. fill the missing labels
+
+        # split between obstype that are checked by qc and obstypes that are not checked
+        checked_cols = [
+            col + "_final_label" for col in list(set(self._qc_checked_obstypes))
+        ]
+        not_checked_cols = [
+            col
+            for col in df_and_outl.columns
+            if ((col.endswith("_final_label")) and (not col in checked_cols))
+        ]
+
+        # if obstype checked, and value is nan --> label ok
+        df_and_outl[checked_cols] = df_and_outl[checked_cols].fillna("ok")
+        # if obstype is not checked and label is missing --> label 'not checked'
+        df_and_outl[not_checked_cols] = df_and_outl[not_checked_cols].fillna(
+            "not checked"
+        )
+
+        # 3. Update the values if needed
+        if not repr_outl_as_nan:
+            # Merge obs and outliers, where obs values will be updated by outliers
+            df_and_outl.update(
+                other=outliersdf_values, join="left", overwrite=True, errors="ignore"
+            )
 
+        # =============================================================================
+        # Make gaps, gapsfill and missing dataframes
+        # =============================================================================
 
         # add gaps observations and fill with default values
         gapsidx = self.gaps.get_gaps_indx_in_obs_space(
-            self.df, self.outliersdf, self.metadf['dataset_resolution'])
+            self.df, self.outliersdf, self.metadf["dataset_resolution"]
+        )
         gapsdf = gapsidx.to_frame()
 
-        # add missing observations if they occure in observation space
-        missingidx = self.missing_obs.get_missing_indx_in_obs_space(
-            self.df, self.metadf['dataset_resolution'])
-        missingdf = missingidx.to_frame()
-
         # add gapfill and remove the filled records from gaps
         gapsfilldf = self.gapfilldf.copy()
+        gapsdf = gapsdf.drop(gapsfilldf.index, errors="ignore")
 
-        gapsdf = gapsdf.drop(gapsfilldf.index, errors='ignore')
-        # missingdf = missingdf.drop(gapsfilldf, errors='ignore') #for future when missing are filled
 
+        # add missing observations if they occure in observation space
+        missingidx = self.missing_obs.get_missing_indx_in_obs_space(
+            self.df, self.metadf["dataset_resolution"]
+        )
+        missingdf = missingidx.to_frame()
+        missingfilldf = self.missing_fill_df.copy()
+        missingdf = missingdf.drop(missingfilldf.index, errors="ignore")
 
-        # get observations
-        df = self.df
-        #fill QC outlier columns with custom values
-        label_cols = [col for col in outliersdf.columns if col.endswith('_label')]
-        for col in label_cols:
-            df[col] = 'ok'
-
-        # Merge obs and outliers, where obs values will be updated by outliers
-        df.update(other=outliersdf,
-                         join='left',
-                         overwrite=True,
-                         errors='ignore')
 
 
-        # initiate default values
-        for col in df.columns:
-            if col in self.settings.app['observation_types']:
+        # initiate default values for gaps and missing that are not filled
+        for col in df_and_outl.columns:
+            if col in observation_types:
                 default_value_gap = np.nan  # nan for observations
                 default_value_missing = np.nan
 
-            elif col.endswith('_final_label'):
+            elif col.endswith("_final_label"):
                 # 'gap' for final label
-                default_value_gap = self.settings.gap['gaps_info']['gap']['outlier_flag']
+                default_value_gap = self.settings.gap["gaps_info"]["gap"][
+                    "outlier_flag"
+                ]
+
                 # 'is_missing_timestamp' for final label
-                default_value_missing = self.settings.gap['gaps_info']['missing_timestamp']['outlier_flag']
+                default_value_missing = self.settings.gap["gaps_info"][
+                    "missing_timestamp"
+                ]["outlier_flag"]
 
             else:
-                default_value_gap = 'not checked'
-                default_value_missing = 'not checked'
-                gapsfilldf[col] = 'not checked'
+                default_value_gap = "not checked"
+                default_value_missing = "not checked"
+
 
             gapsdf[col] = default_value_gap
             missingdf[col] = default_value_missing
+            if not col in gapsfilldf.columns:
+                gapsfilldf[col] = default_value_gap
+            if not col in missingfilldf.columns:
+                missingfilldf[col] = default_value_missing
 
         # sort columns
-        gapsdf = gapsdf[list(df.columns)]
-        missingdf = missingdf[list(df.columns)]
-
+        column_order = df_and_outl.columns.to_list()
+        gapsdf = gapsdf[column_order]
+        gapsfilldf=gapsfilldf[column_order]
+        missingdf = missingdf[column_order]
+        missingfilldf = missingfilldf[column_order]
 
         # Merge all together
-        comb_df = pd.concat([df, gapsdf, missingdf, gapsfilldf]).sort_index()
+        comb_df = pd.concat([df_and_outl, gapsdf, missingdf,
+                             gapsfilldf, missingfilldf]).sort_index()
 
         return comb_df
 
-
-    def get_qc_stats(self, obstype='temp', stationnames=None, make_plot=True):
+    def get_qc_stats(self, obstype="temp", stationnames=None, make_plot=True):
         """
         Compute frequency statistics on the qc labels for an observationtype.
         The output is a dataframe containing the frequency statistics presented
         as percentages.
 
         These frequencies can also be presented as a collection of piecharts
         per check.
@@ -840,448 +1120,772 @@
             as percentages0.
 
         """
 
         # cobmine all and get final label
         comb_df = self.combine_all_to_obsspace()
 
-        # drop observation columns that are not obstype
-        ignore_obstypes = self.settings.app['observation_types'].copy()
-        ignore_obstypes.remove(obstype)
-        comb_df = comb_df.drop(columns=ignore_obstypes)
-
-        # drop label columns not applicable on obstype
-        relevant_columns = [col for col in comb_df.columns if col.startswith(obstype)]
-
-        # add all columns of checks applied on records (i.g. without obs prefix like duplicate timestamp)
-        record_check = {key: item['label_columnname'] for key, item in self.settings.qc['qc_checks_info'].items() if item['apply_on'] == 'record'}
-        relevant_columns.extend(list(record_check.values()))
-        relevant_columns = [col for col in relevant_columns if col in comb_df.columns]
-        # filter relevant columns
-        comb_df = comb_df[relevant_columns]
-
+        # subset to relevant columnt
+        relev_columns = [obstype, obstype + "_final_label"]
+        comb_df = comb_df[relev_columns]
 
         # compute freq statistics
         final_freq, outl_freq, specific_freq = get_freq_statistics(
-            comb_df = comb_df,
+            comb_df=comb_df,
             obstype=obstype,
-            checks_info=self.settings.qc['qc_checks_info'],
-            gaps_info =self.settings.gap['gaps_info'],
-            )
-
-        if any([isinstance(stat, type(None)) for stat in [final_freq,
-                                                          outl_freq,
-                                                          specific_freq]]):
+            checks_info=self.settings.qc["qc_checks_info"],
+            gaps_info=self.settings.gap["gaps_info"],
+            applied_qc_order=self._applied_qc,
+        )
 
+        if any([stat is None for stat in [final_freq, outl_freq, specific_freq]]):
             return None
 
         if make_plot:
             # make pie plots
-            qc_stats_pie(final_stats=final_freq,
-                         outlier_stats=outl_freq,
-                         specific_stats=specific_freq,
-                         plot_settings=self.settings.app['plot_settings'],
-                         qc_check_info=self.settings.qc['qc_checks_info'])
+            qc_stats_pie(
+                final_stats=final_freq,
+                outlier_stats=outl_freq,
+                specific_stats=specific_freq,
+                plot_settings=self.settings.app["plot_settings"],
+                qc_check_info=self.settings.qc["qc_checks_info"],
+            )
 
         return (final_freq, outl_freq, specific_freq)
 
     def update_outliersdf(self, add_to_outliersdf):
+        """V5"""
 
-        # Get the flag column labels and find the newly added columnlabelname
-        previous_performed_checks_columns = [
-            col for col in self.outliersdf.columns if col.endswith('_label')]
-        new_performed_checks_columns = list(set([
-                    col for col in add_to_outliersdf.columns
-                    if col.endswith('_label')])
-                    - set(previous_performed_checks_columns))
-
-        # add to the outliersdf
         self.outliersdf = pd.concat([self.outliersdf, add_to_outliersdf])
 
-        # Fix labels
-        self.outliersdf[previous_performed_checks_columns] = self.outliersdf[
-                        previous_performed_checks_columns].fillna(value='ok')
-
-        self.outliersdf[new_performed_checks_columns] = self.outliersdf[
-            new_performed_checks_columns].fillna(value='not checked')
-
-
     # =============================================================================
     #     importing data
     # =============================================================================
 
-    def coarsen_time_resolution(self, freq='1H', method='nearest', limit=1):
-        logger.info(f'Coarsening the timeresolution to {freq} using \
-                    the {method}-method (with limit={limit}).')
+    def coarsen_time_resolution(
+        self, origin=None, origin_tz=None, freq=None, method=None, limit=None
+    ):
+        """
+        Resample the observations to coarser timeresolution. The assumed
+        dataset resolution (stored in the metadf attribute) will be updated.
+
+        Parameters
+        ----------
+        origin : datetime.datetime, optional
+            Define the origin (first timestamp) for the obervations. The origin
+            is timezone naive, and is assumed to have the same timezone as the
+            obervations. If None, the earliest occuring timestamp is used as
+            origin. The default is None.
+        origin_tz : str, optional
+            Timezone string of the input observations. Element of
+            pytz.all_timezones. If None, the timezone from the settings is
+            used. The default is None.
+        freq : DateOffset, Timedelta or str, optional
+            The offset string or object representing target conversion.
+            Ex: '15T' is 15 minuts, '1H', is one hour. If None, the target time
+            resolution of the dataset.settings is used. The default is None.
+        method : 'nearest' or 'bfill', optional
+            Method to apply for the resampling. If None, the resample method of
+            the dataset.settings is used. The default is None.
+        limit : int, optional
+            Limit of how many values to fill with one original observations. If
+            None, the target limit of the dataset.settings is used. The default
+            is None.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        if freq is None:
+            freq = self.settings.time_settings["target_time_res"]
+        if method is None:
+            method = self.settings.time_settings["resample_method"]
+        if limit is None:
+            limit = int(self.settings.time_settings["resample_limit"])
+        if origin_tz is None:
+            origin_tz = self.settings.time_settings["timezone"]
+
+        logger.info(
+            f"Coarsening the timeresolution to {freq} using \
+                    the {method}-method (with limit={limit})."
+        )
         # TODO: implement buffer method
         # TODO: implement startdt point
-        # Coarsen timeresolution
         df = self.df.reset_index()
-        if method == 'nearest':
-            df = df.set_index('datetime').groupby(
-                'name').resample(freq).nearest(limit=limit)
-
-        elif method == 'bfill':
-            df = df.set_index('datetime').groupby(
-                'name').resample(freq).bfill(limit=limit)
+
+        if origin is None:
+            # find earlyest timestamp, if it is on the hour, use it else use the following hour
+            tstart = df["datetime"].min()
+
+            if tstart.minute != 0 or tstart.second != 0 or tstart.microsecond != 0:
+                # Round up to nearest hour
+                tstart = tstart.ceil(freq=freq)
+        else:
+            origin_tz_aware = pytz.timezone(origin_tz).localize(origin)
+            tstart = origin_tz_aware.astimezone(
+                pytz.timezone(self.settings.time_settings["timezone"])
+            )
+
+        # Coarsen timeresolution
+
+        if method == "nearest":
+            df = (
+                df.set_index("datetime")
+                .groupby("name")
+                .resample(freq, origin=tstart)
+                .nearest(limit=limit)
+            )
+
+        elif method == "bfill":
+            df = (
+                df.set_index("datetime")
+                .groupby("name")
+                .resample(freq, origin=tstart)
+                .bfill(limit=limit)
+            )
 
         else:
-            print(f'The coarsening method: {method}, is not implemented yet.')
-            df = df.set_index(['name', 'datetime'])
+            print(f"The coarsening method: {method}, is not implemented yet.")
+            df = df.set_index(["name", "datetime"])
 
-        if 'name' in df.columns:
-            df = df.drop(columns=['name'])
+        if "name" in df.columns:
+            df = df.drop(columns=["name"])
 
         # Update resolution info in metadf
-        self.metadf['dataset_resolution'] = pd.to_timedelta(freq)
+        self.metadf["dataset_resolution"] = pd.to_timedelta(freq)
         # update df
         self.df = df
 
-    def import_data_from_file(self, network='vlinder', coarsen_timeres=False):
+        # Remove gaps and missing from the observatios
+        # most gaps and missing are already removed but when increasing timeres,
+        # some records should be removed as well.
+        self.df = self.gaps.remove_gaps_from_obs(obsdf=self.df)
+        self.df = self.missing_obs.remove_missing_from_obs(obsdf=self.df)
+
+
+    def sync_observations(self, tollerance, verbose=True):
+        """
+        Simplify and syncronize the observation timestamps along different stations.
+
+        To simplify the resolution (per station), a tollerance is use to shift timestamps. The tollerance indicates the
+        maximum translation in time that can be applied to an observation.
+
+        The sycronisation tries to group stations that have an equal simplified resolution, and syncronize them. The origin
+        of the sycronized timestamps will be set to round hours, round 10-minutes or round-5 minutes if possible given the tollerance.
+
+        The observations present in the input file are used.
+
+        After syncronization, the IO outliers, missing observations and gaps are recomputed.
+
+        Parameters
+        ----------
+        tollerance, Timedelta or str
+            The tollerance string or object representing the maximum translation in time.
+            Ex: '5T' is 5 minuts, '1H', is one hour.
+        verbose : bool, optional
+            If True, a dataframe illustrating the mapping from original datetimes to simplified and syncronized is returned. The default is True.
+
+        Note
+        --------
+        Keep in mind that this method will overwrite the df, outliersdf, missing timestamps and gaps.
+
+        Note
+        --------
+        Because the used observations are from the input file, previously coarsend timeresolutions are ignored.
+
+
+        Returns
+        -------
+        pandas.DataFrame (if verbose is True)
+            A dataframe containing the original observations with original timestamps and the corresponding target timestamps.
+
+        """
+
+
+
+        df = self.input_df
+
+        self.df = init_multiindexdf()
+        self.outliersdf = init_triple_multiindexdf()
+        self.gapfilldf = init_multiindexdf()
+        self.missing_obs = None
+        self.gaps = None
+
+        # find simplified resolution
+        simplified_resolution = get_freqency_series(
+            df=df, method="median", simplify=True, max_simplify_error=tollerance
+        )
+
+        occuring_resolutions = simplified_resolution.unique()
+
+        df = df.reset_index()
+
+        def find_simple_origin(tstart, tollerance):
+            if tstart.minute == 0 and tstart.second == 0 and tstart.microsecond == 0:
+                return tstart  # already a round hour
+
+            # try converting to a round hour
+            tstart_round_hour = tstart.round("60min")
+            if abs(tstart - tstart_round_hour) <= pd.to_timedelta(tollerance):
+                return tstart_round_hour
+
+            # try converting to a tenfold in minutes
+            tstart_round_tenfold = tstart.round("10min")
+            if abs(tstart - tstart_round_tenfold) <= pd.to_timedelta(tollerance):
+                return tstart_round_tenfold
+
+            # try converting to a fivefold in minutes
+            tstart_round_fivefold = tstart.round("5min")
+
+            if abs(tstart - tstart_round_fivefold) <= pd.to_timedelta(tollerance):
+                return tstart_round_fivefold
+
+            # no suitable conversion found
+            return tstart
+
+        merged_df = pd.DataFrame()
+        _total_verbose_df = pd.DataFrame()
+        for occur_res in occuring_resolutions:
+            group_stations = simplified_resolution[
+                simplified_resolution == occur_res
+            ].index.to_list()
+            print(
+                f" Grouping stations with simplified resolution of {pd.to_timedelta(occur_res)}: {group_stations}"
+            )
+            groupdf = df[df["name"].isin(group_stations)]
+
+            tstart = groupdf["datetime"].min()
+            tend = groupdf["datetime"].max()
+
+            # find a good origin point
+            origin = find_simple_origin(tstart=tstart, tollerance=tollerance)
+
+            # Create records index
+            target_records = pd.date_range(
+                start=origin, end=tend, freq=pd.Timedelta(occur_res)
+            ).to_series()
+
+            target_records.name = "target_datetime"
+            # convert records to new target records, station per station
+
+            for sta in group_stations:
+                stadf = groupdf[groupdf["name"] == sta]
+                # Drop all nan values! these will be added later from the outliersdf
+                stadf = stadf.set_index(["name", "datetime"])
+                stadf = stadf.dropna(axis=0, how="all")
+                stadf = stadf.reset_index()
+
+                mergedstadf = pd.merge_asof(
+                    left=stadf.sort_values("datetime"),
+                    right=target_records.to_frame(),
+                    right_on="target_datetime",
+                    left_on="datetime",
+                    direction="nearest",
+                    tolerance=pd.Timedelta(tollerance),
+                )
+
+                # possibility 1: record is mapped crrectly
+                correct_mapped = mergedstadf[~mergedstadf["target_datetime"].isnull()]
+
+
+                # possibility2: records that ar not mapped to target
+                # not_mapped_records =mergedstadf[mergedstadf['target_datetime'].isnull()]
+
+
+                # possibilyt 3 : no suitable candidates found for the target
+                # these will be cached by the missing and gap check
+                # no_record_candidates = target_records[~target_records.isin(mergedstadf['target_datetime'])].values
+
+
+                merged_df = pd.concat([merged_df, correct_mapped])
+                if verbose:
+                    _total_verbose_df = pd.concat([_total_verbose_df, mergedstadf])
+
+        # overwrite the df with the synced observations
+        merged_df = (
+            merged_df.rename(
+                columns={"datetime": "original_datetime", "target_datetime": "datetime"}
+            )
+            .set_index(["name", "datetime"])
+            .drop(["original_datetime"], errors="ignore", axis=1)
+            .sort_index()
+        )
+        # self.df = merged_df
+
+        # Recompute the dataset attributes, apply qc, gap and missing searches, etc.
+        self._construct_dataset(
+            df=merged_df,
+            freq_estimation_method="highest",
+            freq_estimation_simplify=False,
+            freq_estimation_simplify_error=None,
+            fixed_freq_series=simplified_resolution,
+            update_full_metadf=False,
+        )  # Do not overwrite full metadf, only the frequencies
+
+        if verbose:
+            _total_verbose_df = _total_verbose_df.rename(
+                columns={"datetime": "original_datetime", "target_datetime": "datetime"}
+            ).set_index(["name", "datetime"])
+            return _total_verbose_df
+
+    def import_data_from_file(
+        self,
+        long_format=True,
+        obstype=None,
+        freq_estimation_method=None,
+        freq_estimation_simplify=None,
+        freq_estimation_simplify_error=None,
+    ):
+
         """
         Read observations from a csv file as defined in the
         Settings.input_file. The input file columns should have a template
         that is stored in Settings.template_list.
 
         If the metadata is stored in a seperate file, and the
         Settings.input_metadata_file is correct, than this metadata is also
         imported (if a suitable template is in the Settings.template_list.)
 
+        The dataset is by default assumed to be in long-format (each column represent an observation type, one column indicates the stationname).
+        Wide-format can be used if 'long_format' is set to False and if the observation type is specified by obstype.
 
-        It is possible to apply a
-        resampling (downsampling) of the observations as defined in the settings.
+        An estimation of the observational frequency is made per station. This is used
+        to find missing observations and gaps.
 
-        After the import there is always a call to Dataset.update_dataset_by_df, that
-        sets up the dataset with the observations and applies some sanity checks.
 
-        Parameters
+        The Dataset attributes are set and the following checks are executed:
+                * Duplicate check
+                * Invalid input check
+                * Find missing observations
+                * Find gaps
 
-        network : String, optional
-            The name of the network for these observations. The default
-            is 'vlinder'.
-        coarsen_timeres : Bool, optional
-            If True, the observations will be interpolated to a coarser
-            time resolution as is defined in the Settings. The default
-            is False.
 
-        Returns
+        Parameters
+        ----------
+        long_format : bool, optional
+            True if the inputdata has a long-format, False if it has a wide-format. The default is True.
+        obstype : str, optional
+            If the dataformat is wide, specify which observation type the
+            observations represent. The obstype should be an element of
+            metobs_toolkit.observation_types. The default is None.
+        freq_estimation_method : 'highest' or 'median', optional
+            Select wich method to use for the frequency estimation. If
+            'highest', the highest apearing frequency is used. If 'median', the
+            median of the apearing frequencies is used. If None, the method
+            stored in the
+            Dataset.settings.time_settings['freq_estimation_method'] is used.
+            The default is None.
+        freq_estimation_simplify : bool, optional
+            If True, the likely frequency is converted to round hours, or round minutes.
+            The "freq_estimation_simplify_error' is used as a constrain. If the constrain is not met,
+            the simplification is not performed. If None, the method
+            stored in the
+            Dataset.settings.time_settings['freq_estimation_simplify'] is used.
+            The default is None.
+        freq_estimation_simplify_error : Timedelta or str, optional
+            The tollerance string or object representing the maximum translation in time to form a simplified frequency estimation.
+            Ex: '5T' is 5 minuts, '1H', is one hour. If None, the method
+            stored in the
+            Dataset.settings.time_settings['freq_estimation_simplify_error'] is
+            used. The default is None.
 
+        Returns
+        -------
         None.
 
         """
-        print('Settings input data file: ', self.settings.IO['input_data_file'])
+
+        print("Settings input data file: ", self.settings.IO["input_data_file"])
         logger.info(f'Importing data from file: {self.settings.IO["input_data_file"]}')
 
+        if freq_estimation_method is None:
+
+            freq_estimation_method = self.settings.time_settings[
+                "freq_estimation_method"
+            ]
+        if freq_estimation_simplify is None:
+            freq_estimation_simplify = self.settings.time_settings[
+                "freq_estimation_simplify"
+            ]
+        if freq_estimation_simplify_error is None:
+            freq_estimation_simplify_error = self.settings.time_settings[
+                "freq_estimation_simplify_error"
+            ]
+
+        # check if obstype is valid
+        if not obstype is None:
+            assert (
+                obstype in observation_types
+            ), f'{obstype} is not a default obstype. Use one of: {self.settings.app["observation_types"]}'
+
+
         # Read observations into pandas dataframe
         df, template = import_data_from_csv(
-                            input_file=self.settings.IO['input_data_file'],
-                            template_file=self.settings.templates['data_template_file'])
+            input_file=self.settings.IO["input_data_file"],
+            template_file=self.settings.templates["data_template_file"],
+            long_format=long_format,
+            obstype=obstype,  # only relevant in wide format
+        )
 
-        # Set timezone information
-        df.index = df.index.tz_localize(tz=self.settings.time_settings['timezone'],
-                                        ambiguous='infer',
-                                        nonexistent='shift_forward')
 
-        logger.debug(f'Data from {self.settings.IO["input_data_file"]} \
-                     imported to dataframe.')
+        # Set timezone information
+        df.index = df.index.tz_localize(
+            tz=self.settings.time_settings["timezone"],
+            ambiguous="infer",
+            nonexistent="shift_forward",
+        )
+
+        logger.debug(
+            f'Data from {self.settings.IO["input_data_file"]} \
+                     imported to dataframe.'
+        )
 
         # drop Nat datetimes if present
         df = df.loc[pd.notnull(df.index)]
 
-        if not 'name' in df.columns:
-            logger.warning(f'No station names find in the observations! \
+        if not "name" in df.columns:
+            logger.warning(
+                f'No station names find in the observations! \
                            Assume the dataset is for ONE station with the \
-                         default name: {self.settings.app["default_name"]}.')
-            df['name'] =str(self.settings.app["default_name"])
+                         default name: {self.settings.app["default_name"]}.'
+            )
+            df["name"] = str(self.settings.app["default_name"])
 
-        if isinstance(self.settings.IO['input_metadata_file'], type(None)):
-            print('WARNING: No metadata file is defined.\
-                  Add your settings object.')
-            logger.warning('No metadata file is defined,\
-                    no metadata attributes can be set!')
+        if self.settings.IO["input_metadata_file"] is None:
+            print(
+                "WARNING: No metadata file is defined.\
+                  Add your settings object."
+            )
+            logger.warning(
+                "No metadata file is defined,\
+                    no metadata attributes can be set!"
+            )
         else:
-            logger.info(f'Importing metadata from file:\
-                        {self.settings.IO["input_metadata_file"]}')
+            logger.info(
+                f'Importing metadata from file:\
+                        {self.settings.IO["input_metadata_file"]}'
+            )
             meta_df = import_metadata_from_csv(
-                        input_file=self.settings.IO["input_metadata_file"],
-                        template_file=self.settings.templates['metadata_template_file'])
+                input_file=self.settings.IO["input_metadata_file"],
+                template_file=self.settings.templates["metadata_template_file"],
+            )
 
             # merge additional metadata to observations
-            meta_cols = [colname for colname in meta_df.columns
-                         if not colname.startswith('_')]
+            meta_cols = [
+                colname for colname in meta_df.columns if not colname.startswith("_")
+            ]
             additional_meta_cols = list(set(meta_cols).difference(df.columns))
 
             if bool(additional_meta_cols):
-                logger.debug(f'Merging metadata ({additional_meta_cols})\
-                             to dataset data by name.')
-                additional_meta_cols.append('name')  # merging on name
+                logger.debug(
+                    f"Merging metadata ({additional_meta_cols})\
+                             to dataset data by name."
+                )
+                additional_meta_cols.append("name")  # merging on name
                 # merge deletes datetime index somehow? so add it back.
                 df_index = df.index
-                df = df.merge(right=meta_df[additional_meta_cols],
-                              how='left',
-                              on='name')
+                df = df.merge(
+                    right=meta_df[additional_meta_cols], how="left", on="name"
+                )
                 df.index = df_index
 
         # update dataset object
         self.data_template = pd.DataFrame().from_dict(template)
 
         # convert dataframe to multiindex (datetime - name)
-        df = df.set_index(['name', df.index])
+        df = df.set_index(["name", df.index])
 
         # dataframe with all data of input file
-        self.input_df = df
+        self.input_df = df.sort_index()
 
-        self.update_dataset_by_df(dataframe=df,
-                                  coarsen_timeres=coarsen_timeres)
-
-    def import_data_from_database(self,
-                                  start_datetime=None,
-                                  end_datetime=None,
-                                  coarsen_timeres=False):
+        self._construct_dataset(
+            df=df,
+            freq_estimation_method=freq_estimation_method,
+            freq_estimation_simplify=freq_estimation_simplify,
+            freq_estimation_simplify_error=freq_estimation_simplify_error,
+        )
+
+    def import_data_from_database(
+        self, start_datetime=None, end_datetime=None, coarsen_timeres=False
+    ):
         """
         Function to import data directly from the framboos database and
         updating the network and station objects.
 
 
         Parameters
+        ----------
 
         start_datetime : datetime, optional
             Start datetime of the observations. The default is None and using
             yesterday's midnight.
         end_datetime : datetime, optional
             End datetime of the observations. The default is None and using
             todays midnight.
         coarsen_timeres : Bool, optional
             If True, the observations will be interpolated to a coarser
             time resolution as is defined in the Settings. The default
             is False.
 
         Returns
+        ----------
 
         None.
 
+        Note
+        ----------
+        A Ugent VPN connection must be present, as well as the username and password
+        stored in the settings.
+
         """
-        if isinstance(start_datetime, type(None)):
+        if start_datetime is None:
             start_datetime = datetime.date.today() - datetime.timedelta(days=1)
-        if isinstance(end_datetime, type(None)):
+        if end_datetime is None:
             end_datetime = datetime.date.today()
 
         # Read observations into pandas dataframe
-        df = import_data_from_db(self.settings.db,
-                                start_datetime=start_datetime,
-                                end_datetime=end_datetime)
+        df = import_data_from_db(
+            self.settings.db, start_datetime=start_datetime, end_datetime=end_datetime
+        )
 
-        if df.empty: #No data has, probably connection error
+        if df.empty:  # No data has, probably connection error
             return
 
         # Make data template
         self.data_template = pd.DataFrame().from_dict(
-            template_to_package_space(self.settings.db['vlinder_db_obs_template']))
+            template_to_package_space(self.settings.db["vlinder_db_obs_template"])
+        )
 
         # convert dataframe to multiindex (datetime - name)
-        df = df.set_index(['name', df.index])
+        df = df.set_index(["name", df.index])
         df = df.sort_index()
 
         # If an ID has changed or not present in the metadatafile,
         # the stationname and metadata is Nan
         # These observations will be removed
-        unknown_obs = df[df.index.get_level_values('name').isnull()]
+        unknown_obs = df[df.index.get_level_values("name").isnull()]
         if not unknown_obs.empty:
-            logger.warning('There is an unknown station in the dataset \
+            logger.warning(
+                "There is an unknown station in the dataset \
                            (probaply due to an ID that is not present in \
-                           the metadata file). This will be removed.')
-            df = df[~df.index.get_level_values('name').isnull()]
+                           the metadata file). This will be removed from the dataset."
+            )
+            df = df[~df.index.get_level_values("name").isnull()]
+        self._construct_dataset(df)
 
-        self.update_dataset_by_df(
-            dataframe=df, coarsen_timeres=coarsen_timeres)
 
-    def update_dataset_by_df(self, dataframe, coarsen_timeres=False):
+    def _construct_dataset(
+        self,
+        df,
+        freq_estimation_method,
+        freq_estimation_simplify,
+        freq_estimation_simplify_error,
+        fixed_freq_series=None,
+        update_full_metadf=True,
+    ):
 
         """
-        Update the dataset object by a dataframe.
+        Helper function to construct the Dataset class from a IO dataframe.
 
+        The df, metadf, outliersdf, gaps and missing timestamps attributes are set.
 
-        When filling the observations, there is an automatic check for
-        missing timestamps and duplicating timestamps. If a missing timestamp
-        is detected, the timestamp is created with Nan values for all
-        observation types.
-
-        If metadata is present and a LCZ-tiff file availible, than the LCZ's
-        of the stations are computed.
+        Qc on IO is applied (duplicated check and invalid check) + gaps and missing
+        values are defined by assuming a frequency per station.
 
         Parameters
-
-        dataframe : pandas.DataFrame
-        A dataframe that has an datetimeindex and following columns:
-            'name, temp, radiation_temp, humidity, ...'
+        ----------
+        df : pandas.dataframe
+            The dataframe containing the input observations and metadata.
+        freq_estimation_method : 'highest' or 'median'
+            Select wich method to use for the frequency estimation. If
+            'highest', the highest apearing frequency is used. If 'median', the
+            median of the apearing frequencies is used.
+        freq_estimation_simplify : bool
+            If True, the likely frequency is converted to round hours, or round minutes.
+            The "freq_estimation_simplify_error' is used as a constrain. If the constrain is not met,
+            the simplification is not performed.
+        freq_estimation_simplify_error : Timedelta or str, optional
+            The tollerance string or object representing the maximum translation in time to form a simplified frequency estimation.
+            Ex: '5T' is 5 minuts, '1H', is one hour.
+        fixed_freq_series : pandas.series or None, optional
+            If you do not want the frequencies to be recalculated, one can pass the
+            frequency series to update the metadf["dataset_resolution"]. If None, the frequencies will be estimated. The default is None.
+        update_full_metadf : bool, optional
+            If True, the full Dataset.metadf will be updated. If False, only the frequency columns in the Dataset.metadf will be updated. The default is True.
 
 
         Returns
-
+        -------
         None.
 
         """
 
 
-        logger.info(f'Updating dataset by dataframe with shape:\
-                    {dataframe.shape}.')
+        # Convert dataframe to dataset attributes
+        self._initiate_df_attribute(dataframe=df, update_metadf=update_full_metadf)
 
-        # Create dataframe with fixed number and order of observational columns
-        df = dataframe.reindex(columns=self.settings.app['observation_types'])
-        self.df = df
+        # Apply quality control on Import resolution
+        self._apply_qc_on_import()
+
+
+        if fixed_freq_series is None:
+            freq_series = get_freqency_series(
+                df=self.df,
+                method=freq_estimation_method,
+                simplify=freq_estimation_simplify,
+                max_simplify_error=freq_estimation_simplify_error,
+            )
 
-        # create metadataframe with fixed number and order of columns
-        metadf = dataframe.reindex(columns=self.settings.app['location_info'])
-        metadf.index = metadf.index.droplevel('datetime')  # drop datetimeindex
-        # drop dubplicates due to datetime
-        metadf = metadf[~metadf.index.duplicated(keep='first')]
-
-        self.metadf = metadf_to_gdf(metadf)
-
-        # add import frequencies to metadf
-        self.metadf['assumed_import_frequency'] = get_freqency_series(self.df)
-        self.df = df.sort_index()
-        self.original_df = df.sort_index()
+            freq_series_import = freq_series
 
+        else:
+            if "assumed_import_frequency" in self.metadf.columns:
+                freq_series_import = self.metadf[
+                    "assumed_import_frequency"
+                ]  # No update
+            else:
+                freq_series_import = fixed_freq_series
+            freq_series = fixed_freq_series
+
+
+        # add import frequencies to metadf (after import qc!)
+        self.metadf["assumed_import_frequency"] = freq_series_import
+
+        self.metadf["dataset_resolution"] = freq_series
+
+        # Remove gaps and missing from the observations AFTER timecoarsening
+        self.df = self.gaps.remove_gaps_from_obs(obsdf=self.df)
+        self.df = self.missing_obs.remove_missing_from_obs(obsdf=self.df)
+
+
+    def _initiate_df_attribute(self, dataframe, update_metadf=True):
+        logger.info(
+            f"Updating dataset by dataframe with shape:\
+                    {dataframe.shape}."
+        )
+
+        # Create dataframe with fixed order of observational columns
+        obs_col_order = [col for col in observation_types if col in dataframe.columns]
+
+        self.df = dataframe[obs_col_order].sort_index()
+
+        if update_metadf:
+            # create metadataframe with fixed number and order of columns
+            metadf = dataframe.reindex(columns=self.settings.app["location_info"])
+            metadf.index = metadf.index.droplevel("datetime")  # drop datetimeindex
+            # drop dubplicates due to datetime
+            metadf = metadf[~metadf.index.duplicated(keep="first")]
+
+            self.metadf = metadf_to_gdf(metadf)
+
+
+    def _apply_qc_on_import(self):
         # find missing obs and gaps, and remove them from the df
         self.df, missing_obs, gaps_df = missing_timestamp_and_gap_check(
             df=self.df,
-            gapsize_n=self.settings.gap['gaps_settings']['gaps_finder']['gapsize_n'])
+            gapsize_n=self.settings.gap["gaps_settings"]["gaps_finder"]["gapsize_n"],
+        )
 
         # Create gaps and missing obs objects
         self.gaps = Gap_collection(gaps_df)
         self.missing_obs = Missingob_collection(missing_obs)
 
         # Perform QC checks on original observation frequencies
-
-        self.df, dup_outl_df = duplicate_timestamp_check(df=self.df,
-                                                         checks_info=self.settings.qc['qc_checks_info'],
-                                                         checks_settings = self.settings.qc['qc_check_settings'])
+        self.df, dup_outl_df = duplicate_timestamp_check(
+            df=self.df,
+            checks_info=self.settings.qc["qc_checks_info"],
+            checks_settings=self.settings.qc["qc_check_settings"],
+        )
         if not dup_outl_df.empty:
-            self.update_outliersdf(dup_outl_df)
+            self.update_outliersdf(add_to_outliersdf=dup_outl_df)
 
-        self.df, nan_outl_df = invalid_input_check(self.df,
-                                                   checks_info=self.settings.qc['qc_checks_info'])
+        self.df, nan_outl_df = invalid_input_check(
+            self.df, checks_info=self.settings.qc["qc_checks_info"]
+        )
         if not nan_outl_df.empty:
             self.update_outliersdf(nan_outl_df)
 
+        self.outliersdf = self.outliersdf.sort_index()
 
-        if coarsen_timeres:
-            self.coarsen_time_resolution(freq=self.settings.time_settings['target_time_res'],
-                                          method=self.settings.time_settings['resample_method'],
-                                          limit=self.settings.time_settings['resample_limit'])
+        # update the order and which qc is applied on which obstype
+        checked_obstypes = [obs for obs in self.df.columns if obs in observation_types]
 
+        checknames = ["duplicated_timestamp", "invalid_input"]  # KEEP order
 
-        else:
-            self.metadf['dataset_resolution'] = self.metadf['assumed_import_frequency']
-
-        # Remove gaps and missing from the observations AFTER timecoarsening
-        self.df = self.gaps.remove_gaps_from_obs(obsdf=self.df)
-        self.df = self.missing_obs.remove_missing_from_obs(obsdf=self.df)
+        self._applied_qc = pd.concat(
+            [
+                self._applied_qc,
+                conv_applied_qc_to_df(
+                    obstypes=checked_obstypes, ordered_checknames=checknames
+                ),
+            ],
+            ignore_index=True,
+        )
 
     # =============================================================================
     # Physiography extractions
     # =============================================================================
 
     def get_lcz(self):
         # connect to gee
         connect_to_gee()
 
         # Extract LCZ for all stations
-        lcz_series = lcz_extractor(metadf = self.metadf,
-                                   mapinfo=self.settings.gee['gee_dataset_info']['global_lcz_map'])
-
-        #drop column if it was already present
-        if 'lcz' in self.metadf:
-            self.metadf = self.metadf.drop(columns=['lcz'])
+        lcz_series = lcz_extractor(
+            metadf=self.metadf,
+            mapinfo=self.settings.gee["gee_dataset_info"]["global_lcz_map"],
+        )
+
+        # drop column if it was already present
+        if "lcz" in self.metadf:
+            self.metadf = self.metadf.drop(columns=["lcz"])
 
         # update metadata
-        self.metadf = self.metadf.merge(lcz_series.to_frame(),
-                                        how='left',
-                                        left_index=True, right_index=True)
+        self.metadf = self.metadf.merge(
+            lcz_series.to_frame(), how="left", left_index=True, right_index=True
+        )
         return lcz_series
 
-
     def get_altitude(self):
         # connect to gee
         connect_to_gee()
 
         # Extract LCZ for all stations
-        altitude_series = height_extractor(metadf = self.metadf,
-                                   mapinfo=self.settings.gee['gee_dataset_info']['DEM'])
-
-        #drop column if it was already present
-        if 'altitude' in self.metadf:
-            self.metadf = self.metadf.drop(columns=['altitude'])
+        altitude_series = height_extractor(
+            metadf=self.metadf, mapinfo=self.settings.gee["gee_dataset_info"]["DEM"]
+        )
+
+        # drop column if it was already present
+        if "altitude" in self.metadf:
+            self.metadf = self.metadf.drop(columns=["altitude"])
 
         # update metadata
-        self.metadf = self.metadf.merge(altitude_series.to_frame(),
-                                        how='left',
-                                        left_index=True, right_index=True)
+        self.metadf = self.metadf.merge(
+            altitude_series.to_frame(), how="left", left_index=True, right_index=True
+        )
         return altitude_series
 
-
     def get_landcover(self, buffer=100, aggregate=True):
-
-
         # connect to gee
         connect_to_gee()
 
         # Extract landcover fractions for all stations
-        lc_frac_df = lc_fractions_extractor(metadf = self.metadf,
-                                   mapinfo=self.settings.gee['gee_dataset_info']['worldcover'],
-                                   buffer=buffer,
-                                   agg=aggregate)
+        lc_frac_df = lc_fractions_extractor(
+            metadf=self.metadf,
+            mapinfo=self.settings.gee["gee_dataset_info"]["worldcover"],
+            buffer=buffer,
+            agg=aggregate,
+        )
 
         # remove columns if they exists
-        self.metadf = self.metadf.drop(columns=list(lc_frac_df.columns),
-                                       errors='ignore')
+        self.metadf = self.metadf.drop(
+            columns=list(lc_frac_df.columns), errors="ignore"
+        )
 
         # update metadf
-        self.metadf = self.metadf.merge(lc_frac_df,
-                                        how='left',
-                                        left_index=True, right_index=True)
+        self.metadf = self.metadf.merge(
+            lc_frac_df, how="left", left_index=True, right_index=True
+        )
 
         return lc_frac_df
-
-
-
-# =============================================================================
-# Class stations (inherit all methods from dataset)
-# =============================================================================
-
-class Station(Dataset):
-    def __init__(self, name, df, outliersdf, gaps, missing_obs, gapfilldf,
-                 metadf, data_template, settings):
-        self.name = name
-        self.df = df
-        self.outliersdf = outliersdf
-        self.gaps = gaps
-        self.missing_obs = missing_obs
-        self.gapfilldf = gapfilldf
-        self.metadf = metadf
-        self.data_template = data_template
-        self.settings=settings
-
-
-        self._istype = 'Station'
-
-
-
-
-def loggin_nan_warnings(df):
-    """
-    Function to feed the logger if Nan values are found in the df
-
-    """
-    for column in df.columns:
-        bool_series = df[column].isnull()
-        if bool_series.values.any():
-            if bool_series.values.all():
-                logger.warning(f'No values for {column}, they are initiated\
-                               as Nan.')
-            else:
-                outliers = bool_series[bool_series]
-                logger.warning(f'No values for stations: \
-                               {outliers.index.to_list()}, for {column},\
-                                   they are initiated as Nan.')
-
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/gap.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/gap.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,31 +13,39 @@
 import pandas as pd
 import numpy as np
 import logging
 from datetime import datetime, timedelta
 import math
 
 
-from metobs_toolkit.gap_filling import (interpolate_gap,
-                                         create_leading_trailing_debias_periods,
-                                         make_era_bias_correction)
+from metobs_toolkit.gap_filling import (
+    interpolate_gap,
+    create_leading_trailing_debias_periods,
+    make_era_bias_correction,
+)
+
+from metobs_toolkit.df_helpers import (
+    format_outliersdf_to_doubleidx,
+    get_likely_frequency,
+)
 
 
-logger = logging.getLogger(__name__)
 
+logger = logging.getLogger(__name__)
 
 
 # =============================================================================
 # Gap class
 
 # a gap is a sequence of repeting missing obs
 # =============================================================================
 
+
 class Gap:
-    """ Gap class holds all gap information and methods for gaps."""
+    """Gap class holds all gap information and methods for gaps."""
 
     def __init__(self, name, startdt, enddt):
         """
         Initiate Gap object with a name, startdt and enddt.
 
         Parameters
         ----------
@@ -51,50 +59,47 @@
         Returns
         -------
         None
 
         """
         # init attributes
         self.name = name
-        self.startgap = startdt #in IO space
-        self.endgap = enddt #in IO space
-
-
+        self.startgap = startdt  # in IO space
+        self.endgap = enddt  # in IO space
 
         # computed attributes
-        self.leading_timestamp=None #last ob_dt before gap in datset space
-        self.trailing_timestamp=None #first ob_dt after gap in dataset space
+        self.leading_timestamp = None  # last ob_dt before gap in datset space
+        self.trailing_timestamp = None  # first ob_dt after gap in dataset space
 
         self.exp_gap_idx = None
 
         # gap fill (only for conventional saving)
         self.gapfill_values = None
         self.gapfill_technique = None
 
     def __str__(self):
-
-        return f'Gap instance: {self.name}: {self.startgap} --> {self.endgap} applied fill technique: {self.gapfill_technique}'
+        return f"Gap instance of {self.name} for {self.startgap} --> {self.endgap}"
+    def __repr__(self):
+        return self.__str__()
 
 
     def to_df(self):
         """
         Convert a Gap object to a dataframe (with one row). The station name is
         the index and two colums ('start_gap', 'end_gap') are constructed.
 
         Returns
         -------
         pandas.DataFrame()
             Gap in dataframe format.
 
         """
-        return pd.DataFrame(index=[self.name],
-                            data={'start_gap': self.startgap,
-                                  'end_gap': self.endgap})
-
-
+        return pd.DataFrame(
+            index=[self.name], data={"start_gap": self.startgap, "end_gap": self.endgap}
+        )
 
     def update_leading_trailing_obs(self, obsdf, outliersdf):
         """
         Add the leading (last obs before gap) and trailing (first obs after gap)
         as extra columns to the self.df.
 
         The obsdf and outliersdf are both used to scan for the leading and trailing obs.
@@ -107,47 +112,42 @@
             Dataset.outliersdf
 
         Returns
         -------
         None.
 
         """
-
+        outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
         # combine timestamps of observations and outliers
-        sta_obs = obsdf.xs(self.name, level='name').index
-        sta_outl = outliersdf.xs(self.name, level='name').index
+        sta_obs = obsdf.xs(self.name, level="name").index
+        sta_outl = outliersdf.xs(self.name, level="name").index
         sta_comb = sta_obs.append(sta_outl)
 
+        # find minimium timediff before
+        before_diff = _find_closes_occuring_date(
+            refdt=self.startgap, series_of_dt=sta_comb, where="before"
+        )
 
-        #find minimium timediff before
-        before_diff = _find_closes_occuring_date(refdt = self.startgap,
-                                                series_of_dt = sta_comb,
-                                                where='before')
-
-        #if no timestamps are before gap, assume gap at the start of the observations
+        # if no timestamps are before gap, assume gap at the start of the observations
         if math.isnan(before_diff):
             before_diff = 0.0
 
         # find minimum timediff after gap
-        after_diff = _find_closes_occuring_date(refdt = self.endgap,
-                                                series_of_dt = sta_comb,
-                                                where='after')
-        #if no timestamps are after gap, assume gap at the end of the observations
+        after_diff = _find_closes_occuring_date(
+            refdt=self.endgap, series_of_dt=sta_comb, where="after"
+        )
+        # if no timestamps are after gap, assume gap at the end of the observations
         if math.isnan(after_diff):
             after_diff = 0.0
 
-
         # get before and after timestamps
         self.leading_timestamp = self.startgap - timedelta(seconds=before_diff)
         self.trailing_timestamp = self.endgap + timedelta(seconds=after_diff)
 
-
-
-
     def update_gaps_indx_in_obs_space(self, obsdf, outliersdf, dataset_res):
         """
 
         Explode the gap, to the dataset resolution and format to a multiindex
         with name -- datetime.
 
         In addition the last observation before the gap (leading), and first
@@ -168,38 +168,41 @@
 
         Returns
         -------
         None
 
         """
 
-
+        outliersdf = format_outliersdf_to_doubleidx(outliersdf)
         self.update_leading_trailing_obs(obsdf, outliersdf)
 
-
-
-        gaprange = pd.date_range(start=self.leading_timestamp,
-                                 end=self.trailing_timestamp,
-                                 freq = dataset_res,
-                                 inclusive="neither")
-
-        self.exp_gap_idx = pd.MultiIndex.from_arrays(arrays=[[self.name]*len(gaprange),
-                                                          gaprange],
-                                                  names=[u'name', u'datetime'])
-
-
-
-
+        gaprange = pd.date_range(
+            start=self.leading_timestamp,
+            end=self.trailing_timestamp,
+            freq=dataset_res,
+            inclusive="neither",
+        )
+
+        self.exp_gap_idx = pd.MultiIndex.from_arrays(
+            arrays=[[self.name] * len(gaprange), gaprange], names=["name", "datetime"]
+        )
 
     # =============================================================================
     #         Gapfill
     # =============================================================================
 
-    def apply_interpolate_gap(self, obsdf, outliersdf, dataset_res, obstype='temp',
-                              method='time', max_consec_fill=100):
+    def apply_interpolate_gap(
+        self,
+        obsdf,
+        outliersdf,
+        dataset_res,
+        obstype="temp",
+        method="time",
+        max_consec_fill=100,
+    ):
         """
         Fill a Gap using a linear interpolation gapfill method for an obstype.
 
         The filled datetimes (in dataset resolution) are returned in the form
         af a multiindex pandas Series (name -- datetime) as index.
 
         Parameters
@@ -222,68 +225,79 @@
         Returns
         -------
         Pandas.Series
             Multiindex Series with filled gap values in dataset space.
 
         """
 
+        outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
-        gapfill_series = interpolate_gap(gap=self,
-                                         obsdf=obsdf,
-                                         outliersdf=outliersdf,
-                                         dataset_res=dataset_res,
-                                         obstype=obstype,
-                                         method=method,
-                                         max_consec_fill=max_consec_fill)
+        gapfill_series = interpolate_gap(
+            gap=self,
+            obsdf=obsdf,
+            outliersdf=outliersdf,
+            dataset_res=dataset_res,
+            obstype=obstype,
+            method=method,
+            max_consec_fill=max_consec_fill,
+        )
         gapdf = gapfill_series.to_frame().reset_index()
-        gapdf['name'] = self.name
-        gapdf.index = pd.MultiIndex.from_arrays(arrays=[gapdf['name'].values,
-                                                        gapdf['datetime'].values],
-                                                  names=[u'name', u'datetime'])
+        gapdf["name"] = self.name
+        gapdf.index = pd.MultiIndex.from_arrays(
+            arrays=[gapdf["name"].values, gapdf["datetime"].values],
+            names=["name", "datetime"],
+        )
         return gapdf[obstype]
 
-
     def get_leading_trailing_debias_periods(self, station, obstype, debias_periods):
         # get debias periods
 
         leading_period, trailing_period = create_leading_trailing_debias_periods(
-                                            station=station,
-                                            gap=self,
-                                            debias_period_settings=debias_periods,
-                                            obstype=obstype)
-
+            station=station,
+            gap=self,
+            debias_period_settings=debias_periods,
+            obstype=obstype,
+        )
 
         return leading_period, trailing_period
 
 
-
 class Gap_collection:
     def __init__(self, gapsdf):
-        self.list = [Gap(sta, row['start_gap'], row['end_gap']) for sta, row in gapsdf.iterrows()]
+        self.list = [
+            Gap(sta, row["start_gap"], row["end_gap"]) for sta, row in gapsdf.iterrows()
+        ]
 
+    def __str__(self):
+        if not bool(self.list):
+            return f'Empty gap collection'
+        longstring = ''
+        for gap in self.list:
+            longstring += str(gap) + '\n'
+        return f"Gap collection for: \n {longstring}"
+    def __repr__(self):
+        return self.__str__()
 
     def to_df(self):
-
         gaps_names = []
         gaps_startdt = []
         gaps_enddt = []
         for gap in self.list:
             gaps_names.append(gap.name)
             gaps_startdt.append(gap.startgap)
             gaps_enddt.append(gap.endgap)
 
-
-        df = pd.DataFrame(index=pd.Index(gaps_names),
-                          data={'start_gap': gaps_startdt,
-                                'end_gap': gaps_enddt})
-        df.index.name = 'name'
+        df = pd.DataFrame(
+            index=pd.Index(gaps_names),
+            data={"start_gap": gaps_startdt, "end_gap": gaps_enddt},
+        )
+        df.index.name = "name"
 
         return df
 
-
     def get_station_gaps(self, name):
         """
         Extract a Gap_collection specific to one station. If no gaps are found
         for the station, an empty Gap_collection is returned.
 
         Parameters
         ----------
@@ -299,16 +313,14 @@
         gapdf = self.to_df()
 
         if name in gapdf.index:
             return Gap_collection(gapdf.loc[name])
         else:
             return Gap_collection(pd.DataFrame())
 
-
-
     def remove_gaps_from_obs(self, obsdf):
         """
         Remove station - datetime records that are in the gaps from the obsdf.
 
         (Usefull when filling timestamps to a df, and if you whant to remove the
          gaps.)
 
@@ -320,37 +332,39 @@
         Returns
         -------
         obsdf : pandas.DataFrame()
             The same dataframe with records inside gaps removed.
 
         """
 
-        #Create index for gaps records in the obsdf
-        expanded_gabsidx = pd.MultiIndex(levels=[['name'],['datetime']],
-                                 codes=[[],[]],
-                                 names=[u'name', u'datetime'])
+        # Create index for gaps records in the obsdf
+        expanded_gabsidx = pd.MultiIndex(
+            levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
+        )
 
         for gap in self.list:
+            sta_records = obsdf.xs(gap.name, level="name").index  # filter by name
 
-            sta_records = obsdf.xs(gap.name, level='name').index #filter by name
-
-            gaps_dt = sta_records[(sta_records >= gap.startgap) & #filter if the observations are within a gap
-                                  (sta_records <= gap.endgap)]
-
-            gaps_multiidx = pd.MultiIndex.from_arrays(arrays=[[gap.name]*len(gaps_dt),
-                                                              gaps_dt],
-                                                      names=[u'name', u'datetime'])
+            gaps_dt = sta_records[
+                (sta_records >= gap.startgap)
+                & (  # filter if the observations are within a gap
+                    sta_records <= gap.endgap
+                )
+            ]
+
+            gaps_multiidx = pd.MultiIndex.from_arrays(
+                arrays=[[gap.name] * len(gaps_dt), gaps_dt], names=["name", "datetime"]
+            )
 
             expanded_gabsidx = expanded_gabsidx.append(gaps_multiidx)
 
-        #remove gaps idx from the obsdf
+        # remove gaps idx from the obsdf
         obsdf = obsdf.drop(index=expanded_gabsidx)
         return obsdf
 
-
     def get_gaps_indx_in_obs_space(self, obsdf, outliersdf, resolutionseries):
         """
 
         Explode the gaps, to the dataset resolution and format to a multiindex
         with name -- datetime.
 
         In addition the last observation before the gap (leading), and first
@@ -369,169 +383,180 @@
 
         Returns
         -------
         expanded_gabsidx_obsspace : TYPE
             DESCRIPTION.
 
         """
-        expanded_gabsidx_obsspace = pd.MultiIndex(levels=[['name'],['datetime']],
-                                  codes=[[],[]],
-                                  names=[u'name', u'datetime'])
+        outliersdf = format_outliersdf_to_doubleidx(outliersdf)
+
+        expanded_gabsidx_obsspace = pd.MultiIndex(
+            levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
+        )
 
         for gap in self.list:
-            gap.update_gaps_indx_in_obs_space(obsdf,
-                                              outliersdf,
-                                              resolutionseries.loc[gap.name])
-            expanded_gabsidx_obsspace = expanded_gabsidx_obsspace.append(gap.exp_gap_idx)
+            gap.update_gaps_indx_in_obs_space(
+                obsdf, outliersdf, resolutionseries.loc[gap.name]
+            )
+            expanded_gabsidx_obsspace = expanded_gabsidx_obsspace.append(
+                gap.exp_gap_idx
+            )
 
         return expanded_gabsidx_obsspace
 
-
-
-    def apply_interpolate_gaps(self, obsdf, outliersdf, dataset_res, obstype='temp',
-                              method='time', max_consec_fill=100):
-
-
-
-        expanded_gabsidx_obsspace = pd.MultiIndex(levels=[['name'],['datetime']],
-                                 codes=[[],[]],
-                                 names=[u'name', u'datetime'])
-        filled_gaps_series = pd.Series(data=[], index=expanded_gabsidx_obsspace,
-                                       dtype=object)
+    def apply_interpolate_gaps(
+        self,
+        obsdf,
+        outliersdf,
+        dataset_res,
+        obstype="temp",
+        method="time",
+        max_consec_fill=100,
+    ):
+        outliersdf = format_outliersdf_to_doubleidx(outliersdf)
+
+        expanded_gabsidx_obsspace = pd.MultiIndex(
+            levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
+        )
+        filled_gaps_series = pd.Series(
+            data=[], index=expanded_gabsidx_obsspace, dtype=object
+        )
 
         for gap in self.list:
-            gapfill_series = interpolate_gap(gap=gap,
-                                             obsdf=obsdf,
-                                             outliersdf=outliersdf,
-                                             dataset_res=dataset_res.loc[gap.name],
-                                             obstype=obstype,
-                                             method=method,
-                                             max_consec_fill=max_consec_fill)
+            gapfill_series = interpolate_gap(
+                gap=gap,
+                obsdf=obsdf,
+                outliersdf=outliersdf,
+                dataset_res=dataset_res.loc[gap.name],
+                obstype=obstype,
+                method=method,
+                max_consec_fill=max_consec_fill,
+            )
 
             gapdf = gapfill_series.to_frame().reset_index()
-            gapdf['name'] = gap.name
-            gapdf.index = pd.MultiIndex.from_arrays(arrays=[gapdf['name'].values,
-                                                            gapdf['datetime'].values],
-                                                      names=[u'name', u'datetime'])
+            gapdf["name"] = gap.name
+            gapdf = gapdf.set_index(['name', 'datetime'])
+            # gapdf.index = pd.MultiIndex.from_arrays(
+            #     arrays=[gapdf["name"].values, gapdf["datetime"].values],
+            #     names=["name", "datetime"],
+            # )
 
-            #Update gap
-            gap.gapfill_technique = 'interpolation'
+            # Update gap
+            gap.gapfill_technique = "interpolation"
             gap.gapfill_values = gapdf[obstype]
 
-
             filled_gaps_series = pd.concat([filled_gaps_series, gapdf[obstype]])
         return filled_gaps_series
 
-
-    def apply_debias_era5_gapfill(self, dataset, eraModelData, debias_settings, obstype='temp'):
-        expanded_gabsidx_obsspace = pd.MultiIndex(levels=[['name'],['datetime']],
-                                 codes=[[],[]],
-                                 names=[u'name', u'datetime'])
-        filled_gaps_series = pd.Series(data=[], index=expanded_gabsidx_obsspace,
-                                       dtype=object)
+    def apply_debias_era5_gapfill(
+        self, dataset, eraModelData, debias_settings, obstype="temp"
+    ):
+        expanded_gabsidx_obsspace = pd.MultiIndex(
+            levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
+        )
+        filled_gaps_series = pd.Series(
+            data=[], index=expanded_gabsidx_obsspace, dtype=object
+        )
 
         for gap in self.list:
-
-            #avoid passing full dataset around
+            # avoid passing full dataset around
             station = dataset.get_station(gap.name)
 
-            #Update gap attributes
-            gap.update_gaps_indx_in_obs_space(obsdf = station.df,
-                                              outliersdf=station.outliersdf,
-                                              dataset_res=station.metadf['dataset_resolution'].squeeze())
+            # Update gap attributes
+            gap.update_gaps_indx_in_obs_space(
+                obsdf=station.df,
+                outliersdf=station.outliersdf,
+                dataset_res=station.metadf["dataset_resolution"].squeeze(),
+            )
 
-            #get leading and trailing period
+            # get leading and trailing period
             leading_obs, trailing_obs = gap.get_leading_trailing_debias_periods(
-                                        obstype=obstype,
-                                        station=dataset.get_station(gap.name),
-                                        debias_periods=debias_settings['debias_period'])
-            #check if leading/trailing is valid
-            if (leading_obs.empty | trailing_obs.empty):
-                print("No suitable leading or trailing period found. Gapfill not possible")
-                gap.gapfill_technique = 'debias era5 gapfill (not possible: no leading/trailing period)'
-                default_return = pd.Series(index=gap.exp_gap_idx, name=obstype, dtype='object')
+                obstype=obstype,
+                station=dataset.get_station(gap.name),
+                debias_periods=debias_settings["debias_period"],
+            )
+            # check if leading/trailing is valid
+            if leading_obs.empty | trailing_obs.empty:
+                print(
+                    "No suitable leading or trailing period found. Gapfill not possible"
+                )
+                gap.gapfill_technique = (
+                    "debias era5 gapfill (not possible: no leading/trailing period)"
+                )
+                default_return = pd.Series(
+                    index=gap.exp_gap_idx, name=obstype, dtype="object"
+                )
                 gap.gapfill_values = default_return
                 filled_gaps_series = pd.concat([filled_gaps_series, default_return])
                 continue
 
-
-            #extract model values at leading and trailing period
+            # extract model values at leading and trailing period
             leading_model = eraModelData.interpolate_modeldata(leading_obs.index)
             trailing_model = eraModelData.interpolate_modeldata(trailing_obs.index)
 
-            #TODO check if there is modeldata for the leading and trailing + obs period
-            if (leading_model[obstype].isnull().any()) | (trailing_model[obstype].isnull().any()) :
-                print("No modeldata for the full leading/trailing period found. Gapfill not possible")
-                gap.gapfill_technique = 'debias era5 gapfill (not possible: not enough modeldata)'
-                default_return = pd.Series(index=gap.exp_gap_idx, name=obstype, dtype='object')
+            # TODO check if there is modeldata for the leading and trailing + obs period
+            if (leading_model[obstype].isnull().any()) | (
+                trailing_model[obstype].isnull().any()
+            ):
+                print(
+                    "No modeldata for the full leading/trailing period found. Gapfill not possible"
+                )
+                gap.gapfill_technique = (
+                    "debias era5 gapfill (not possible: not enough modeldata)"
+                )
+                default_return = pd.Series(
+                    index=gap.exp_gap_idx, name=obstype, dtype="object"
+                )
                 gap.gapfill_values = default_return
                 filled_gaps_series = pd.concat([filled_gaps_series, default_return])
 
             # Get model data for gap timestamps
             gap_model = eraModelData.interpolate_modeldata(gap.exp_gap_idx)
 
             # apply bias correction
-            filled_gap_series = make_era_bias_correction(leading_model=leading_model,
-                                                          trailing_model=trailing_model,
-                                                          gap_model=gap_model,
-                                                          leading_obs=leading_obs,
-                                                          trailing_obs=trailing_obs,
-                                                          obstype=obstype)
+            filled_gap_series = make_era_bias_correction(
+                leading_model=leading_model,
+                trailing_model=trailing_model,
+                gap_model=gap_model,
+                leading_obs=leading_obs,
+                trailing_obs=trailing_obs,
+                obstype=obstype,
+            )
 
-            #Update gap
-            gap.gapfill_technique = 'debias era5 gapfill'
+            # Update gap
+            gap.gapfill_technique = "debias era5 gapfill"
             gap.gapfill_values = filled_gap_series
 
             filled_gaps_series = pd.concat([filled_gaps_series, filled_gap_series])
 
         filled_gaps_series.name = obstype
         return filled_gaps_series
 
 
-
 # =============================================================================
 # Find gaps and missing values
 # =============================================================================
 
-def get_freqency_series(df):
-    freqs = {}
-    for station in df.index.get_level_values(level='name').unique():
-        timestamps = df.xs(station, level='name').index
-        freqs[station] = get_likely_frequency(timestamps)
-    return pd.Series(data=freqs)
-
 
-def get_likely_frequency(timestamps):
-    assume_freq = abs(timestamps.to_series().diff().value_counts().index).sort_values(ascending=True)[0]
-
-    if assume_freq == pd.to_timedelta(0): #highly likely due to a duplicated record
-        # select the second highest frequency
-        assume_freq = abs(timestamps.to_series().diff().value_counts().index).sort_values(ascending=True)[1]
-
-    return assume_freq
-
-
-def _find_closes_occuring_date(refdt, series_of_dt, where='before'):
-    if where=='before':
+def _find_closes_occuring_date(refdt, series_of_dt, where="before"):
+    if where == "before":
         diff = refdt - (series_of_dt[series_of_dt < refdt])
-    elif where=='after':
-        diff =(series_of_dt[series_of_dt > refdt]) - refdt
-
+    elif where == "after":
+        diff = (series_of_dt[series_of_dt > refdt]) - refdt
 
     if diff.empty:
-        #no occurences before of after
+        # no occurences before of after
 
         return np.nan
     else:
-
         return min(diff).total_seconds()
 
 
 def missing_timestamp_and_gap_check(df, gapsize_n):
-    #TODO update docstring
+    # TODO update docstring
     """
 
     V3
     Looking for missing timestaps by assuming an observation frequency. The assumed frequency is the highest occuring frequency PER STATION.
     If missing observations are detected, they can be catogirized as a missing timestamp or as gap.
 
     A gap is define as a sequence of missing values with more than N repetitive missing values. N is define in the QC settings.
@@ -551,74 +576,95 @@
     outlier_df : pandas.DataFrame()
         The dataframe containing the missing timestamps (not gaps) with the outlier label.
     gap_df : pandas.Dataframe()
         The dataframe containing the start and end date of a specific gap.
 
     """
 
-
-
     gap_df = pd.DataFrame()
     gap_indices = []
     missing_timestamp_series = pd.Series(dtype=object)
     station_freqs = {}
 
-    #missing timestamp per station (because some stations can have other frequencies!)
+    # missing timestamp per station (because some stations can have other frequencies!)
 
-    stationnames = df.index.get_level_values(level='name').unique()
+    stationnames = df.index.get_level_values(level="name").unique()
     for station in stationnames:
+        # find missing timestamps
+        timestamps = df.xs(station, level="name").index
+        likely_freq = get_likely_frequency(timestamps, method="highest", simplify=False)
 
-        #find missing timestamps
-        timestamps = df.xs(station, level='name').index
-        likely_freq = get_likely_frequency(timestamps)
 
-        assert likely_freq.seconds > 0, f'The frequency is not positive!'
+        assert likely_freq.seconds > 0, f"The frequency is not positive!"
 
         station_freqs[station] = likely_freq
 
-        missing_datetimeseries = pd.date_range(start = timestamps.min(),
-                                                end = timestamps.max(),
-                                                freq=likely_freq).difference(timestamps).to_series().diff()
+        missing_datetimeseries = (pd.date_range(start=timestamps.min(),
+                                               end=timestamps.max(),
+                                               freq=likely_freq)
+                                  .difference(timestamps)
+                                  .to_series()
+                                  .diff())
 
 
         if missing_datetimeseries.empty:
             continue
 
-        #Check for gaps
+        # Check for gaps
         gap_defenition = ((missing_datetimeseries != likely_freq)).cumsum()
         consec_missing_groups = missing_datetimeseries.groupby(gap_defenition)
         group_sizes = consec_missing_groups.size()
 
         gap_groups = group_sizes[group_sizes > gapsize_n]
 
-        #iterate over the gabs and fill the gapsdf
+        # iterate over the gabs and fill the gapsdf
         for gap_idx in gap_groups.index:
-
-            #fill the gaps df
+            # fill the gaps df
             datetime_of_gap_records = consec_missing_groups.get_group(gap_idx).index
-            gap_df = pd.concat([gap_df,
-                                pd.DataFrame(data=[[datetime_of_gap_records.min(),
-                                                  datetime_of_gap_records.max()]],
-                                            index=[station],
-                                            columns=['start_gap', 'end_gap'])])
-
-            logger.debug(f'Data gap from {datetime_of_gap_records.min()} --> {datetime_of_gap_records.max()} found for {station}.')
-            gap_indices.extend(list(zip([station]*datetime_of_gap_records.shape[0],
-                                        datetime_of_gap_records)))
+            gap_df = pd.concat(
+                [
+                    gap_df,
+                    pd.DataFrame(
+                        data=[
+                            [
+                                datetime_of_gap_records.min(),
+                                datetime_of_gap_records.max(),
+                            ]
+                        ],
+                        index=[station],
+                        columns=["start_gap", "end_gap"],
+                    ),
+                ]
+            )
+
+            logger.debug(
+                f"Data gap from {datetime_of_gap_records.min()} --> {datetime_of_gap_records.max()} found for {station}."
+            )
+            gap_indices.extend(
+                list(
+                    zip(
+                        [station] * datetime_of_gap_records.shape[0],
+                        datetime_of_gap_records,
+                    )
+                )
+            )
 
         # combine the missing timestams values
         missing_timestamp_groups = group_sizes[group_sizes <= gapsize_n]
         for missing_idx in missing_timestamp_groups.index:
-            datetime_of_missing_records=consec_missing_groups.get_group(missing_idx).index.to_list()
-
-
-            missing_timestamp_series = pd.concat([missing_timestamp_series,
-                                                  pd.Series(index=[station] * len(datetime_of_missing_records),
-                                                            data=datetime_of_missing_records)])
-
-
-
+            datetime_of_missing_records = consec_missing_groups.get_group(
+                missing_idx
+            ).index.to_list()
+
+            missing_timestamp_series = pd.concat(
+                [
+                    missing_timestamp_series,
+                    pd.Series(
+                        index=[station] * len(datetime_of_missing_records),
+                        data=datetime_of_missing_records,
+                    ),
+                ]
+            )
 
     df = df.sort_index()
 
-
-    return df, missing_timestamp_series, gap_df
+    return df, missing_timestamp_series, gap_df
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/gap_filling.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/gap_filling.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,334 +5,384 @@
 
 @author: thoverga
 """
 import numpy as np
 import pandas as pd
 from datetime import timedelta
 
-from metobs_toolkit.df_helpers import (remove_outliers_from_obs,
-                                        init_multiindexdf)
+from metobs_toolkit.df_helpers import (
+    remove_outliers_from_obs,
+    init_multiindexdf,
+    format_outliersdf_to_doubleidx,
+)
+
+# def interpolate_missing_obs(missing_ob, obsdf, outliersdf, obstype, method):
+#     # 1 get trailing and leading obs
 
 
 
 # =============================================================================
 # Gap fillers
 # =============================================================================
 
-def interpolate_gap(gap, obsdf, outliersdf, dataset_res, obstype,
-                    method, max_consec_fill):
 
+def interpolate_gap(
+    gap, obsdf, outliersdf, dataset_res, obstype, method, max_consec_fill
+):
+    outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
-    #1 get trailing and leading + exploded index
+    # 1 get trailing and leading + exploded index
     gap.update_leading_trailing_obs(obsdf, outliersdf)
     gap.update_gaps_indx_in_obs_space(obsdf, outliersdf, dataset_res)
 
-
     # initiate return value when no interpolation can be performed
-    empty_interp = pd.Series(data=np.nan, index=gap.exp_gap_idx.droplevel('name'))
-    empty_interp.name=obstype
-
+    empty_interp = pd.Series(data=np.nan, index=gap.exp_gap_idx.droplevel("name"))
+    empty_interp.name = obstype
 
     # 2 check if there is a trailing and leading gap
-    if (gap.startgap == gap.leading_timestamp):
-        print(f'No leading timestamp found for gap ({gap.name}): {gap.startgap} --> {gap.endgap}')
-        return  empty_interp
-
-
-    if (gap.endgap == gap.trailing_timestamp):
-        print(f'No trailing timestamp found for gap ({gap.name}): {gap.startgap} --> {gap.endgap}')
-        return  empty_interp
-
-
-
+    if gap.startgap == gap.leading_timestamp:
+        print(
+            f"No leading timestamp found for gap ({gap.name}): {gap.startgap} --> {gap.endgap}"
+        )
+        return empty_interp
+
+    if gap.endgap == gap.trailing_timestamp:
+        print(
+            f"No trailing timestamp found for gap ({gap.name}): {gap.startgap} --> {gap.endgap}"
+        )
+        return empty_interp
 
     # 3 check both leading and trailing are in obs, and look for alternative leading/trailing if the original is an outlier.
-    sta_obs = obsdf.xs(gap.name, level='name')
+    sta_obs = obsdf.xs(gap.name, level="name")
 
     # leading
     if gap.leading_timestamp in sta_obs.index:
         # leading found in obs
         leading_dt = gap.leading_timestamp
         leading_val = sta_obs.loc[gap.leading_timestamp, obstype]
     else:
         # look for last observation before leading timestamp
-        delta_dt = (gap.leading_timestamp - sta_obs.index[sta_obs.index < gap.leading_timestamp])
+        delta_dt = (
+            gap.leading_timestamp - sta_obs.index[sta_obs.index < gap.leading_timestamp]
+        )
         if delta_dt.empty:
-            print(f'No cadidate for leading {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}')
-            return  empty_interp
+            print(
+                f"No cadidate for leading {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}"
+            )
+            return empty_interp
 
         leading_dt = gap.leading_timestamp - delta_dt.min()
         leading_val = sta_obs.loc[leading_dt, obstype]
 
-    #trailing
+    # trailing
     if gap.trailing_timestamp in sta_obs.index:
         # leading found in obs
         trailing_dt = gap.trailing_timestamp
         trailing_val = sta_obs.loc[gap.trailing_timestamp, obstype]
     else:
         # look for last observation before leading timestamp
-        delta_dt = (sta_obs.index[sta_obs.index > gap.trailing_timestamp] - gap.trailing_timestamp)
+        delta_dt = (
+            sta_obs.index[sta_obs.index > gap.trailing_timestamp]
+            - gap.trailing_timestamp
+        )
         if delta_dt.empty:
-            print(f'No cadidate for trailing {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}')
-            return  empty_interp
+            print(
+                f"No cadidate for trailing {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}"
+            )
+            return empty_interp
         # TODO: settings restrictions on maximum delta_dt ??
         trailing_dt = gap.trailing_timestamp + delta_dt.min()
         trailing_val = sta_obs.loc[trailing_dt, obstype]
 
     # Make interpolation series
-    gaps_series = pd.Series(data=np.nan, index=gap.exp_gap_idx.droplevel('name'))
-    gaps_series = pd.concat([gaps_series,
-                             pd.Series(index=[leading_dt, trailing_dt],
-                                               data=[leading_val, trailing_val])])
+    gaps_series = pd.Series(data=np.nan, index=gap.exp_gap_idx.droplevel("name"))
+    gaps_series = pd.concat(
+        [
+            gaps_series,
+            pd.Series(
+                index=[leading_dt, trailing_dt], data=[leading_val, trailing_val]
+            ),
+        ]
+    )
     gaps_series = gaps_series.sort_index()
 
-
-
     # Interpolate series
-    gaps_series.interpolate(method=method,
-                            limit=max_consec_fill, # Maximum number of consecutive NaNs to fill. Must be greater than 0.
-                            limit_area='inside',
-                            inplace=True)
+    gaps_series.interpolate(
+        method=method,
+        limit=max_consec_fill,  # Maximum number of consecutive NaNs to fill. Must be greater than 0.
+        limit_area="inside",
+        inplace=True,
+    )
 
     # Subset only gap indixes
-    gaps_series = gaps_series[gap.exp_gap_idx.droplevel('name')]
-    gaps_series.name=obstype
+    gaps_series = gaps_series[gap.exp_gap_idx.droplevel("name")]
+    gaps_series.name = obstype
 
     return gaps_series
 
 
-
 # =============================================================================
 # Debiasing period
 # =============================================================================
 
+
 def get_sample_size(sample_duration_hours, sta):
-    stares = sta.metadf['dataset_resolution'].squeeze()
-    sample_size =  timedelta(hours=sample_duration_hours)/stares
+    stares = sta.metadf["dataset_resolution"].squeeze()
+    sample_size = timedelta(hours=sample_duration_hours) / stares
     return int(sample_size)
 
 
-
-def create_leading_trailing_debias_periods(station, gap, debias_period_settings, obstype):
-
-    #Get samplesizes
-    debias_pref_sample_size_leading = get_sample_size(debias_period_settings['prefered_leading_sample_duration_hours'],
-                                                      station)
-    debias_pref_sample_size_trailing = get_sample_size(debias_period_settings['prefered_trailing_sample_duration_hours'],
-                                                      station)
-    debias_min_sample_size_leading = get_sample_size(debias_period_settings['minimum_leading_sample_duration_hours'],
-                                                  station)
-    debias_min_sample_size_trailing = get_sample_size(debias_period_settings['minimum_trailing_sample_duration_hours'],
-                                                  station)
+def create_leading_trailing_debias_periods(
+    station, gap, debias_period_settings, obstype
+):
+    # Get samplesizes
+    debias_pref_sample_size_leading = get_sample_size(
+        debias_period_settings["prefered_leading_sample_duration_hours"], station
+    )
+    debias_pref_sample_size_trailing = get_sample_size(
+        debias_period_settings["prefered_trailing_sample_duration_hours"], station
+    )
+    debias_min_sample_size_leading = get_sample_size(
+        debias_period_settings["minimum_leading_sample_duration_hours"], station
+    )
+    debias_min_sample_size_trailing = get_sample_size(
+        debias_period_settings["minimum_trailing_sample_duration_hours"], station
+    )
 
     # get all observations that can be used for debias training
     obs = station.df
 
-
     # remove blacklist
-    #TODO
-    obs = remove_outliers_from_obs(obs, station.outliersdf)
+    # TODO
+    obs = remove_outliers_from_obs(
+        obs, format_outliersdf_to_doubleidx(station.outliersdf)
+    )
 
     # add whitelist
-    #TODO
-
+    # TODO
 
     # only datetimes are relevant
     obs = obs.reset_index()
-    obs = obs[['name', 'datetime', obstype]]
-
+    obs = obs[["name", "datetime", obstype]]
 
     # Select all leading and all trailing obs
-    leading_period = obs[obs['datetime'] < gap.startgap]
-    trailing_period = obs[obs['datetime'] > gap.endgap]
+    leading_period = obs[obs["datetime"] < gap.startgap]
+    trailing_period = obs[obs["datetime"] > gap.endgap]
 
     # some derived integers
     poss_shrinkage_leading = leading_period.shape[0] - debias_min_sample_size_leading
     poss_shrinkage_trailing = trailing_period.shape[0] - debias_min_sample_size_trailing
     poss_extention_leading = leading_period.shape[0] - debias_pref_sample_size_leading
-    poss_extention_trailing = trailing_period.shape[0] - debias_pref_sample_size_trailing
-
+    poss_extention_trailing = (
+        trailing_period.shape[0] - debias_pref_sample_size_trailing
+    )
 
     # check if desired sample sizes for leading and trailing are possible
-    if ((leading_period.shape[0] >= debias_pref_sample_size_leading) &
-        (trailing_period.shape[0] >= debias_pref_sample_size_trailing)):
-        print(f'leading and trailing periods are both available for debiassing.')
+    if (leading_period.shape[0] >= debias_pref_sample_size_leading) & (
+        trailing_period.shape[0] >= debias_pref_sample_size_trailing
+    ):
+        print(f"leading and trailing periods are both available for debiassing.")
         # both periods are oke
         leading_df = leading_period[-debias_pref_sample_size_leading:]
         trailing_df = trailing_period[:debias_pref_sample_size_trailing]
 
-
-    elif ((leading_period.shape[0] <= debias_pref_sample_size_leading) &
-        (trailing_period.shape[0] >= debias_pref_sample_size_trailing)):
-        print(f'leading periods for debiassing does not have a preferable size. Try translation/shrinkage ...')
+    elif (leading_period.shape[0] <= debias_pref_sample_size_leading) & (
+        trailing_period.shape[0] >= debias_pref_sample_size_trailing
+    ):
+        print(
+            f"leading periods for debiassing does not have a preferable size. Try translation/shrinkage ..."
+        )
 
         # leading period to small, trailing period is OK
 
         missing_records = debias_pref_sample_size_leading - leading_period.shape[0]
 
-
-
         # 1 if the leading period is smaller thatn the minimum leading size --> return default
         if poss_shrinkage_leading < 0:
             leading_df = init_multiindexdf()
-            trailing_df = init_multiindexdf()  #this might be to strict
-            print('The available leading debias samplesize is smaller than the minimum. A translation/shrinking is not possible.')
+            trailing_df = init_multiindexdf()  # this might be to strict
+            print(
+                "The available leading debias samplesize is smaller than the minimum. A translation/shrinking is not possible."
+            )
 
         # 2 Try translation without shrinkage
 
         elif missing_records <= poss_extention_trailing:
             # translation without shrinkage is possible
             translation_trailing = missing_records
 
             leading_df = leading_period
-            trailing_df = trailing_period[0:(debias_pref_sample_size_trailing + translation_trailing)]
-
-            print(f'A translation of {translation_trailing} records is done towards the trailing period. (n_leading + n_trailing is conserved: {leading_df.shape[0] + trailing_df.shape[0]}')
-
+            trailing_df = trailing_period[
+                0 : (debias_pref_sample_size_trailing + translation_trailing)
+            ]
+
+            print(
+                f"A translation of {translation_trailing} records is done towards the trailing period. (n_leading + n_trailing is conserved: {leading_df.shape[0] + trailing_df.shape[0]}"
+            )
 
         # 3. Try if a translation is within the limits of shrinkage
         elif (missing_records - poss_extention_trailing) <= poss_shrinkage_leading:
             translation_trailing = poss_extention_trailing
 
-            leading_df=leading_period
-            trailing_df = trailing_period[0:debias_pref_sample_size_trailing + translation_trailing]
-            print(f'A translation of {translation_trailing} records is done towards the trailing period. Since there was not engough translation space for the trailing obs, the condition n_leading + n_trailing is NOT conserved: {leading_df.shape[0] + trailing_df.shape[0]}. \
-                  Both leading and trailing sizes still achieves minimal size restrictions.')
+            leading_df = leading_period
+            trailing_df = trailing_period[
+                0 : debias_pref_sample_size_trailing + translation_trailing
+            ]
+            print(
+                f"A translation of {translation_trailing} records is done towards the trailing period. Since there was not engough translation space for the trailing obs, the condition n_leading + n_trailing is NOT conserved: {leading_df.shape[0] + trailing_df.shape[0]}. \
+                  Both leading and trailing sizes still achieves minimal size restrictions."
+            )
         # 4. If all else fails, it is not possible to make a leading period
         else:
-            print('The available leading samplesize can not reach minimal size restrictions.')
+            print(
+                "The available leading samplesize can not reach minimal size restrictions."
+            )
             # no translation is possible, even with shrinking
             leading_df = init_multiindexdf()
-            trailing_df = init_multiindexdf() #this might be to strict
+            trailing_df = init_multiindexdf()  # this might be to strict
 
-
-
-    elif ((leading_period.shape[0] >= debias_pref_sample_size_leading) &
-        (trailing_period.shape[0] <= debias_pref_sample_size_trailing)):
+    elif (leading_period.shape[0] >= debias_pref_sample_size_leading) & (
+        trailing_period.shape[0] <= debias_pref_sample_size_trailing
+    ):
         # leading period is ok, trailing period is to short
-        print(f'trailing periods for debiassing does not have a preferable size. Try translation/shrinkage ...')
+        print(
+            f"trailing periods for debiassing does not have a preferable size. Try translation/shrinkage ..."
+        )
         missing_records = debias_pref_sample_size_trailing - trailing_period.shape[0]
 
-
-
         # 1 if the trailing period is smaller thatn the minimum trailing size --> return default
         if poss_shrinkage_trailing < 0:
-            leading_df= init_multiindexdf() #might be to strict
+            leading_df = init_multiindexdf()  # might be to strict
             trailing_df = init_multiindexdf()
-            print('The available trailing debias samplesize is smaller than the minimum. A translation/shrinking is not possible.')
+            print(
+                "The available trailing debias samplesize is smaller than the minimum. A translation/shrinking is not possible."
+            )
             # return
 
         # 2 Try translation without shrinkage
         elif missing_records <= poss_extention_leading:
             # translation without shrinkage is possible
             translation_leading = missing_records
 
-            leading_df = leading_period[-(debias_pref_sample_size_leading+translation_leading):]
+            leading_df = leading_period[
+                -(debias_pref_sample_size_leading + translation_leading) :
+            ]
             trailing_df = trailing_period
-            print(f'A translation of {translation_leading} records is done towards the leading period. (n_leading + n_trailing is conserved: {leading_df.shape[0] + trailing_df.shape[0]}')
+            print(
+                f"A translation of {translation_leading} records is done towards the leading period. (n_leading + n_trailing is conserved: {leading_df.shape[0] + trailing_df.shape[0]}"
+            )
 
         # 3. Try if a translation is within the limits of shrinkage
         elif (missing_records - poss_extention_leading) <= poss_shrinkage_trailing:
             translation_leading = poss_extention_leading
 
-            leading_df=leading_period[-(debias_pref_sample_size_leading+translation_leading)]
+            leading_df = leading_period[
+                -(debias_pref_sample_size_leading + translation_leading)
+            ]
             trailing_df = trailing_period
-            print(f'A translation of {translation_leading} records is done towards the leading period. Since there was not engough translation space for the leading obs, the condition n_leading + n_trailing is NOT conserved: {leading_df.shape[0] + trailing_df.shape[0]}. \
-                  Both leading and trailing sizes still achieves minimal size restrictions.')
+            print(
+                f"A translation of {translation_leading} records is done towards the leading period. Since there was not engough translation space for the leading obs, the condition n_leading + n_trailing is NOT conserved: {leading_df.shape[0] + trailing_df.shape[0]}. \
+                  Both leading and trailing sizes still achieves minimal size restrictions."
+            )
         # 4. If all else fails, it is not possible to make a trailing period
         else:
             # no translation is possible, even with shrinking
-            print('The available trailing samplesize can not reach minimal size restrictions.')
-            leading_df = init_multiindexdf() #this might be to strict
+            print(
+                "The available trailing samplesize can not reach minimal size restrictions."
+            )
+            leading_df = init_multiindexdf()  # this might be to strict
             trailing_df = init_multiindexdf()
 
-
     else:
         # Both leading and trailing periods are not to small
 
         # 1 does both (leading and trailing) still acchieves the minimal size condition for shrinking?
         if (poss_shrinkage_leading >= 0) & (poss_shrinkage_trailing >= 0):
-            print('Both leading and trailing periods do not have a prefered size, but still meet the minimal conditions.')
-            leading_df=leading_period
+            print(
+                "Both leading and trailing periods do not have a prefered size, but still meet the minimal conditions."
+            )
+            leading_df = leading_period
             trailing_df = trailing_period
 
         else:
-            print('Both leading and trailing periods do not have a prefered size, and eighter of them does NOT meet minimal condition.')
+            print(
+                "Both leading and trailing periods do not have a prefered size, and eighter of them does NOT meet minimal condition."
+            )
             # either one of the periods does not reach minimal condition, so return default
             leading_df = init_multiindexdf()
             trailing_df = init_multiindexdf()
 
     # convert to multiindex
     if not leading_df.empty:
-        leading_df = leading_df.set_index(['name', 'datetime'])
+        leading_df = leading_df.set_index(["name", "datetime"])
     if not trailing_df.empty:
-        trailing_df = trailing_df.set_index(['name', 'datetime'])
-
+        trailing_df = trailing_df.set_index(["name", "datetime"])
 
     return leading_df, trailing_df
 
 
-
-
-
 def get_time_specific_biases(model, obs, obstype, period):
     diff = model - obs
-    diff = diff.reset_index().set_index('datetime')
-    diff['hours'] = diff.index.hour
-    diff['minutes'] = diff.index.minute
-    diff['seconds'] = diff.index.second
+    diff = diff.reset_index().set_index("datetime")
+    diff["hours"] = diff.index.hour
+    diff["minutes"] = diff.index.minute
+    diff["seconds"] = diff.index.second
 
-    biases = diff.groupby(['name', 'hours', 'minutes', 'seconds'])[obstype].mean()
-    biases.name = obstype+'_bias_' + period
+    biases = diff.groupby(["name", "hours", "minutes", "seconds"])[obstype].mean()
+    biases.name = obstype + "_bias_" + period
 
     biases = biases.reset_index()
     return biases
 
 
-def make_era_bias_correction(leading_model, trailing_model, gap_model, leading_obs, trailing_obs, obstype):
-
+def make_era_bias_correction(
+    leading_model, trailing_model, gap_model, leading_obs, trailing_obs, obstype
+):
     # 1. get lead timestamp biases
-    lead_biases = get_time_specific_biases(model=leading_model,
-                                           obs=leading_obs,
-                                           obstype=obstype,
-                                           period='lead')
-
+    lead_biases = get_time_specific_biases(
+        model=leading_model, obs=leading_obs, obstype=obstype, period="lead"
+    )
 
     # 2. get trailing timestamp biases
-    trail_biases = get_time_specific_biases(model=trailing_model,
-                                           obs=trailing_obs,
-                                           obstype=obstype,
-                                           period='trail')
+    trail_biases = get_time_specific_biases(
+        model=trailing_model, obs=trailing_obs, obstype=obstype, period="trail"
+    )
 
     # 3. apply bias correction on modeldata in gap
 
     # linear interpolation of bias along the gap method:
-    gap_model['trail_weight'] = np.linspace(0.0, 1.0, gap_model.shape[0])
-    gap_model['lead_weight'] = 1.0 - gap_model['trail_weight']
+    gap_model["trail_weight"] = np.linspace(0.0, 1.0, gap_model.shape[0])
+    gap_model["lead_weight"] = 1.0 - gap_model["trail_weight"]
 
-    #aggregate to timestamps
-    gap_model['hours'] = gap_model.index.get_level_values('datetime').hour
-    gap_model['minutes'] = gap_model.index.get_level_values('datetime').minute
-    gap_model['seconds'] = gap_model.index.get_level_values('datetime').second
+    # aggregate to timestamps
+    gap_model["hours"] = gap_model.index.get_level_values("datetime").hour
+    gap_model["minutes"] = gap_model.index.get_level_values("datetime").minute
+    gap_model["seconds"] = gap_model.index.get_level_values("datetime").second
 
     # 4. merge biases and model values together
-    gap_debias = gap_model.merge(right=lead_biases[['hours', 'minutes', 'seconds', obstype+'_bias_lead']],
-                                how='left',
-                                on=['hours', 'minutes', 'seconds'])
-
-    gap_debias = gap_debias.merge(right=trail_biases[['hours', 'minutes', 'seconds', obstype+'_bias_trail']],
-                                how='left',
-                                on=['hours', 'minutes', 'seconds'])
-
-    gap_debias.index=gap_model.index #TODO: this might be dangerous, but the merge removes the index ??
-
+    gap_debias = gap_model.merge(
+        right=lead_biases[["hours", "minutes", "seconds", obstype + "_bias_lead"]],
+        how="left",
+        on=["hours", "minutes", "seconds"],
+    )
+
+    gap_debias = gap_debias.merge(
+        right=trail_biases[["hours", "minutes", "seconds", obstype + "_bias_trail"]],
+        how="left",
+        on=["hours", "minutes", "seconds"],
+    )
+
+    gap_debias.index = (
+        gap_model.index
+    )  # TODO: this might be dangerous, but the merge removes the index ??
 
     # 5. compute the debiased fill value
-    #leave this dataframe for debugging
-    gap_debias[obstype+'_fill'] = (gap_debias[obstype] -
-                                   ((gap_debias['lead_weight'] * gap_debias[obstype+'_bias_lead']) +
-                                    (gap_debias['trail_weight'] * gap_debias[obstype+'_bias_trail'])))
+    # leave this dataframe for debugging
+    gap_debias[obstype + "_fill"] = gap_debias[obstype] - (
+        (gap_debias["lead_weight"] * gap_debias[obstype + "_bias_lead"])
+        + (gap_debias["trail_weight"] * gap_debias[obstype + "_bias_trail"])
+    )
 
     # 6. make returen
-    returnseries = gap_debias[obstype+'_fill']
+    returnseries = gap_debias[obstype + "_fill"]
     returnseries.name = obstype
     return returnseries
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/geometry_functions.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/geometry_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 Created on Fri Oct 21 09:13:01 2022
 
 @author: thoverga
 """
 # import geopandas as gpd
 from shapely.geometry import box
 
+
 def gpd_to_extent_box(geodf):
     return box(*geodf.total_bounds)
 
+
 def extent_list_to_box(extentlist):
     return box(*extentlist)
 
 
 def find_largest_extent(geodf, extentlist):
-    
     # get extent of geodf as a box
     geodf_extent_box = gpd_to_extent_box(geodf)
-    
+
     # get extendbox of extendlist
     default_extent_box = extent_list_to_box(extentlist)
-    
-    #Check if default covers the geodf
+
+    # Check if default covers the geodf
     if default_extent_box.covers(geodf_extent_box):
         return extentlist
-    
-    return geodf.total_bounds
+
+    return geodf.total_bounds
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/landcover_functions.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/landcover_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,222 +15,225 @@
 
 from metobs_toolkit.df_helpers import init_multiindexdf
 
 # =============================================================================
 #  Connection functions
 # =============================================================================
 
+
 def connect_to_gee():
-    if not ee.data._credentials: #check if ee connection is initialized
+    if not ee.data._credentials:  # check if ee connection is initialized
         ee.Authenticate()
         ee.Initialize()
     return
 
+
 # =============================================================================
 # Top level functions (can be called by dataset)
 # =============================================================================
 
 
 def lcz_extractor(metadf, mapinfo):
-
     # make return in case something went wrong
-    default_return = pd.Series(index=metadf.index, data='Location_unknown',
-                               name='lcz', dtype=object)
+    default_return = pd.Series(
+        index=metadf.index, data="Location_unknown", name="lcz", dtype=object
+    )
     # test if metadata is suitable
     if not _validate_metadf(metadf):
-        print(f'Metadf is not suitable for GEE extractiond: {metadf}')
+        print(f"Metadf is not suitable for GEE extractiond: {metadf}")
         return default_return
 
-    relevant_metadf = metadf.reset_index()[['name', 'lat', 'lon']]
+    relevant_metadf = metadf.reset_index()[["name", "lat", "lon"]]
 
     lcz_df = extract_pointvalues(
-                metadf=relevant_metadf,
-                mapinfo=mapinfo,
-                output_column_name='lcz')
-    return lcz_df['lcz'] #return series
+        metadf=relevant_metadf, mapinfo=mapinfo, output_column_name="lcz"
+    )
+    return lcz_df["lcz"]  # return series
 
 
 def lc_fractions_extractor(metadf, mapinfo, buffer, agg):
-
     # make return in case something went wrong
     default_return = pd.DataFrame(index=metadf.index)
 
     # test if metadata is suitable
     if not _validate_metadf(metadf):
-        print(f'Metadf is not suitable for GEE extractiond: {metadf}')
+        print(f"Metadf is not suitable for GEE extractiond: {metadf}")
         return default_return
 
-    relevant_metadf = metadf.reset_index()[['name', 'lat', 'lon']]
+    relevant_metadf = metadf.reset_index()[["name", "lat", "lon"]]
 
-    freqs_df = extract_buffer_frequencies(metadf=relevant_metadf,
-                                          mapinfo=mapinfo,
-                                          bufferradius=buffer)
+    freqs_df = extract_buffer_frequencies(
+        metadf=relevant_metadf, mapinfo=mapinfo, bufferradius=buffer
+    )
 
     # apply aggregation if required
     if agg:
-        print('aggregateion')
+        print("aggregateion")
         agg_df = pd.DataFrame()
-        for agg_name, agg_classes  in mapinfo['aggregation'].items():
-            present_agg_classes = [str(num) for num in agg_classes if str(num) in freqs_df.columns]
-            agg_df[agg_name+'_'+str(buffer)+'m'] = freqs_df[present_agg_classes].sum(axis=1)
+        for agg_name, agg_classes in mapinfo["aggregation"].items():
+            present_agg_classes = [
+                str(num) for num in agg_classes if str(num) in freqs_df.columns
+            ]
+            agg_df[agg_name + "_" + str(buffer) + "m"] = freqs_df[
+                present_agg_classes
+            ].sum(axis=1)
 
         return agg_df
 
-
     else:
         # map numeric classes to human
-        mapper = {str(num): human+'_'+str(buffer)+'m' for num, human in
-                  mapinfo['categorical_mapper'].items()}
+        mapper = {
+            str(num): human + "_" + str(buffer) + "m"
+            for num, human in mapinfo["categorical_mapper"].items()
+        }
         freqs_df = freqs_df.rename(columns=mapper)
 
         return freqs_df
 
 
-
 def height_extractor(metadf, mapinfo):
     # make return in case something went wrong
-    default_return = pd.Series(index=metadf.index, data='Location_unknown',
-                                name='altitude', dtype=object)
+    default_return = pd.Series(
+        index=metadf.index, data="Location_unknown", name="altitude", dtype=object
+    )
 
     # test if metadata is suitable
     if not _validate_metadf(metadf):
-        print(f'Metadf is not suitable for GEE extractiond: {metadf}')
+        print(f"Metadf is not suitable for GEE extractiond: {metadf}")
         return default_return
 
-    relevant_metadf = metadf.reset_index()[['name', 'lat', 'lon']]
+    relevant_metadf = metadf.reset_index()[["name", "lat", "lon"]]
 
     altitude_df = extract_pointvalues(
-                metadf=relevant_metadf,
-                mapinfo=mapinfo,
-                output_column_name='altitude')
-    return altitude_df['altitude'] #return series
-
-
-
+        metadf=relevant_metadf, mapinfo=mapinfo, output_column_name="altitude"
+    )
+    return altitude_df["altitude"]  # return series
 
 
 # =============================================================================
 # Object convertors
 # =============================================================================
 
 
 def _datetime_to_gee_datetime(datetime):
     # covert to UTC!
     utcdt = datetime.astimezone(pytz.utc)
-    return ee.Date(utcdt.strftime('%Y-%m-%dT%H:%M:%S'))
+    return ee.Date(utcdt.strftime("%Y-%m-%dT%H:%M:%S"))
+
 
 def get_ee_obj(mapinfo, band=None):
-    if mapinfo['is_image']:
-        obj = ee.Image(mapinfo['location'])
-    elif mapinfo['is_imagecollection']:
+    if mapinfo["is_image"]:
+        obj = ee.Image(mapinfo["location"])
+    elif mapinfo["is_imagecollection"]:
         if isinstance(band, type(None)):
-            obj = ee.ImageCollection(mapinfo['location'])
+            obj = ee.ImageCollection(mapinfo["location"])
         else:
-            obj = ee.ImageCollection(mapinfo['location']).select(band)
+            obj = ee.ImageCollection(mapinfo["location"]).select(band)
 
     else:
-        sys.exit('Map type is not an Image or Imagecollection.')
+        sys.exit("Map type is not an Image or Imagecollection.")
     return obj
 
 
-
-
-def coords_to_geometry(lat=[], lon=[], proj='EPSG:4326'):
+def coords_to_geometry(lat=[], lon=[], proj="EPSG:4326"):
     if len(lat) == 1:
         return ee.Geometry.Point(coords=[lon[0], lat[0]], proj=proj)
     else:
         return ee.Geometry.MultiPoint(list(zip(lon, lat)), proj=proj)
 
+
 # =============================================================================
 # Helpers
 # =============================================================================
 
+
 def _validate_metadf(metadf):
     """
     Returns True if metadata is suitable for gee extraction.
 
     :param metadf: metadata dataframe
     :type metadf: pd.DataFrame
     :return: True if oke, else False
     :rtype: Bool
 
     """
 
-    if metadf['geometry'].x.isnull().values.all():
+    if metadf["geometry"].x.isnull().values.all():
         return False
-    if metadf['geometry'].y.isnull().values.all():
+    if metadf["geometry"].y.isnull().values.all():
         return False
     try:
         # Just testing if it can be converted
-        metadf = metadf.to_crs('epsg:4326')
+        metadf = metadf.to_crs("epsg:4326")
     except:
         return False
 
     return True
 
+
 def _addDate(image):
-    """ add the image datetime as a band """
+    """add the image datetime as a band"""
     img_date = ee.Date(image.date())
-    img_date = ee.Number.parse(img_date.format('YYYYMMddHHmmss'))
-    return image.addBands(ee.Image(img_date).rename('datetime'))
-
+    img_date = ee.Number.parse(img_date.format("YYYYMMddHHmmss"))
+    return image.addBands(ee.Image(img_date).rename("datetime"))
 
 
 def _df_to_features_point_collection(df):
-    """ Convert a dataframe to a featurecollections row-wise"""
-    features=[]
+    """Convert a dataframe to a featurecollections row-wise"""
+    features = []
     for index, row in df.reset_index().iterrows():
-    #     construct the geometry from dataframe
-        poi_geometry = ee.Geometry.Point([row['lon'], row['lat']])
-    #     construct the attributes (properties) for each point
-        poi_properties = poi_properties = {'name': row['name']}
-    #     construct feature combining geometry and properties
+        #     construct the geometry from dataframe
+        poi_geometry = ee.Geometry.Point([row["lon"], row["lat"]])
+        #     construct the attributes (properties) for each point
+        poi_properties = poi_properties = {"name": row["name"]}
+        #     construct feature combining geometry and properties
         poi_feature = ee.Feature(poi_geometry, poi_properties)
         features.append(poi_feature)
 
     return ee.FeatureCollection(features)
 
 
 def _df_to_features_buffer_collection(df, bufferradius):
-    """ Convert a dataframe to a featurecollections row-wise"""
-    features=[]
+    """Convert a dataframe to a featurecollections row-wise"""
+    features = []
     for index, row in df.reset_index().iterrows():
-    #     construct the geometry from dataframe
-        poi_geometry = ee.Geometry.Point([row['lon'], row['lat']]).buffer(distance=bufferradius)
-    #     construct the attributes (properties) for each point
-        poi_properties = poi_properties = {'name': row['name']}
-    #     construct feature combining geometry and properties
+        #     construct the geometry from dataframe
+        poi_geometry = ee.Geometry.Point([row["lon"], row["lat"]]).buffer(
+            distance=bufferradius
+        )
+        #     construct the attributes (properties) for each point
+        poi_properties = poi_properties = {"name": row["name"]}
+        #     construct feature combining geometry and properties
         poi_feature = ee.Feature(poi_geometry, poi_properties)
         features.append(poi_feature)
 
     return ee.FeatureCollection(features)
 
-def coordinates_available(metadf, latcol='lat', loncol='lon'):
+
+def coordinates_available(metadf, latcol="lat", loncol="lon"):
     if metadf[latcol].isnull().all():
-        print('No coordinates are found!')
+        print("No coordinates are found!")
         return False
     if metadf[loncol].isnull().all():
-        print('No coordinates are found!')
+        print("No coordinates are found!")
         return False
     return True
 
 
 def _estimate_data_size(metadf, startdt, enddt, mapinfo):
-    datatimerange = pd.date_range(start=startdt, end=enddt, freq=mapinfo['time_res'])
+    datatimerange = pd.date_range(start=startdt, end=enddt, freq=mapinfo["time_res"])
 
     return metadf.shape[0] * len(datatimerange)
 
 
-
 # =============================================================================
 # Data extractors
 # =============================================================================
 
 
-
 def extract_pointvalues(metadf, mapinfo, output_column_name):
     """
     Extract values for point locations from a GEE dataset.
     The pointlocations are defined in a dataframe by EPSG:4326 lat lon coordinates.
 
 
     A dataframe with the extracted values is returned.
@@ -252,75 +255,74 @@
 
     Returns
     -------
     pd.DataFrame
         A dataframe with name as index, all columns from the metadf + extracted extracted values column.
 
     """
-    scale=mapinfo['scale']
-
+    scale = mapinfo["scale"]
 
     # test if coordiantes are available
-    if not coordinates_available(metadf, 'lat', 'lon'):
+    if not coordinates_available(metadf, "lat", "lon"):
         return pd.DataFrame()
 
     # =============================================================================
     # df to featurecollection
     # =============================================================================
 
     ee_fc = _df_to_features_point_collection(metadf)
 
     # =============================================================================
     # extract raster values
     # =============================================================================
 
+    raster = get_ee_obj(mapinfo, mapinfo["band_of_use"])  # dataset
+    if mapinfo["is_imagecollection"]:
 
-
-    raster = get_ee_obj(mapinfo, mapinfo['band_of_use']) #dataset
-    if mapinfo['is_imagecollection']:
         def rasterExtraction(image):
             feature = image.sampleRegions(
-                collection = ee_fc, # feature collection here
-                scale = scale # Cell size of raster
+                collection=ee_fc,  # feature collection here
+                scale=scale,  # Cell size of raster
             )
             return feature
 
-        results = raster.map(rasterExtraction) \
-                    .flatten() \
-                    .getInfo()
-    elif mapinfo['is_image']:
-        raster = get_ee_obj(mapinfo, mapinfo['band_of_use']) #dataset
-        results = raster.sampleRegions(collection = ee_fc, # feature collection here
-                                       scale = scale)\
-                        .getInfo()
+        results = raster.map(rasterExtraction).flatten().getInfo()
+    elif mapinfo["is_image"]:
+        raster = get_ee_obj(mapinfo, mapinfo["band_of_use"])  # dataset
+        results = raster.sampleRegions(
+            collection=ee_fc, scale=scale  # feature collection here
+        ).getInfo()
     else:
-        sys.exit(f'gee dataset {mapinfo["location"]} is neighter image nor imagecollection.')
-
+        sys.exit(
+            f'gee dataset {mapinfo["location"]} is neighter image nor imagecollection.'
+        )
 
     # =============================================================================
     # to dataframe
     # =============================================================================
 
     # extract properties
-    properties = [x['properties'] for x in results['features']]
+    properties = [x["properties"] for x in results["features"]]
     df = pd.DataFrame(properties)
 
-    #map to human space if categorical
-    if mapinfo['value_type'] == 'categorical':
-        df[mapinfo['band_of_use']] = df[mapinfo['band_of_use']].map(mapinfo['categorical_mapper'])
+    # map to human space if categorical
+    if mapinfo["value_type"] == "categorical":
+        df[mapinfo["band_of_use"]] = df[mapinfo["band_of_use"]].map(
+            mapinfo["categorical_mapper"]
+        )
 
-    #rename to values to toolkit space
-    df = df.rename(columns={mapinfo['band_of_use']: output_column_name})
+    # rename to values to toolkit space
+    df = df.rename(columns={mapinfo["band_of_use"]: output_column_name})
 
     # #format index
-    df = df.set_index(['name'])
-
+    df = df.set_index(["name"])
 
     return df
 
+
 def extract_buffer_frequencies(metadf, mapinfo, bufferradius):
     """
     Extract values for circular buffers for a given radius arround a point locations from a GEE categorical dataset.
     The pointlocations are defined in a dataframe by EPSG:4326 lat lon coordinates.
 
 
     A dataframe with the extracted values is returned.
@@ -340,75 +342,71 @@
 
     Returns
     -------
     pd.DataFrame
         A dataframe with name as index, all columns from the metadf + extracted extracted values column.
 
     """
-    scale=mapinfo['scale']
-
+    scale = mapinfo["scale"]
 
     # test if coordiantes are available
-    if not coordinates_available(metadf, 'lat', 'lon'):
+    if not coordinates_available(metadf, "lat", "lon"):
         return pd.DataFrame()
 
     # test if map is categorical
-    if not mapinfo['value_type'] == 'categorical':
-        print('ERROR: Extract buffer frequencies is only implemented for categorical datasets!')
+    if not mapinfo["value_type"] == "categorical":
+        print(
+            "ERROR: Extract buffer frequencies is only implemented for categorical datasets!"
+        )
         return pd.DataFrame()
 
-
     # =============================================================================
     # df to featurecollection
     # =============================================================================
 
     ee_fc = _df_to_features_buffer_collection(metadf, bufferradius)
 
-
-
     # =============================================================================
     # extract raster values
     # =============================================================================
 
-
     def rasterExtraction(image):
         feature = image.reduceRegions(
-            reducer = ee.Reducer.frequencyHistogram(),
-            collection = ee_fc, # feature collection here
-            scale = scale # Cell size of raster
+            reducer=ee.Reducer.frequencyHistogram(),
+            collection=ee_fc,  # feature collection here
+            scale=scale,  # Cell size of raster
         )
         return feature
 
-
-    raster = get_ee_obj(mapinfo, mapinfo['band_of_use']) #dataset
-    results = raster.map(rasterExtraction) \
-                    .flatten() \
-                    .getInfo()
+    raster = get_ee_obj(mapinfo, mapinfo["band_of_use"])  # dataset
+    results = raster.map(rasterExtraction).flatten().getInfo()
 
     # =============================================================================
     # to dataframe
     # =============================================================================
 
-    freqs = { staprop['properties']['name']: staprop['properties']['histogram'] for staprop in results['features']}
+    freqs = {
+        staprop["properties"]["name"]: staprop["properties"]["histogram"]
+        for staprop in results["features"]
+    }
     freqsdf = pd.DataFrame(freqs)
 
     # format frequency df
     freqsdf = freqsdf.transpose().fillna(0)
-    freqsdf.index.name = 'name'
+    freqsdf.index.name = "name"
 
     # normalize freqs
     freqsdf = freqsdf.div(freqsdf.sum(axis=1), axis=0)
 
     return freqsdf
 
 
-
-
-
-def gee_extract_timeseries(metadf, mapinfo, startdt, enddt, obstype='temp', latcolname='lat', loncolname='lon'):
+def gee_extract_timeseries(
+    metadf, mapinfo, startdt, enddt, obstype="temp", latcolname="lat", loncolname="lon"
+):
     """
     Extract a timeseries, for a given obstype, for point locations from a GEE dataset. The pointlocations are defined in a dataframe by EPSG:4326 lat lon coordinates.
 
     The startdate is included, the enddate is excluded.
 
     A multi-index dataframe with the timeseries is returned
 
@@ -433,122 +431,119 @@
     -------
     pd.DataFrame
         A dataframe with name - datetime multiindex, all columns from the metadf + extracted timeseries
         column with the same name as the obstype.
 
     """
 
-
-
-    scale=mapinfo['scale']
-    bandname=mapinfo['band_of_use'][obstype]['name']
-
-
+    scale = mapinfo["scale"]
+    bandname = mapinfo["band_of_use"][obstype]["name"]
 
     # test if coordiantes are available
     if not coordinates_available(metadf, latcolname, loncolname):
         return pd.DataFrame()
 
-    use_drive=False
+    use_drive = False
     _est_data_size = _estimate_data_size(metadf, startdt, enddt, mapinfo)
     if _est_data_size > 4000:
-        print('THE DATA AMOUT IS TO LAREGE FOR INTERACTIVE SESSION, THE DATA WILL BE EXPORTED TO YOUR GOOGLE DRIVE!')
-        use_drive=True
+        print(
+            "THE DATA AMOUT IS TO LAREGE FOR INTERACTIVE SESSION, THE DATA WILL BE EXPORTED TO YOUR GOOGLE DRIVE!"
+        )
+        use_drive = True
     # =============================================================================
     # df to featurecollection
     # =============================================================================
 
-    ee_fc = _df_to_features_point_collection(metadf, loncolname, latcolname)
-
-
-
+    ee_fc = _df_to_features_point_collection(metadf)
 
     # =============================================================================
     # extract raster values
     # =============================================================================
 
     def rasterExtraction(image):
         feature = image.sampleRegions(
-            collection = ee_fc, # feature collection here
-            scale = scale # Cell size of raster
+            collection=ee_fc,  # feature collection here
+            scale=scale,  # Cell size of raster
         )
         return feature
 
-
-    raster = get_ee_obj(mapinfo, bandname) #dataset
-    results = raster.filter(ee.Filter.date(_datetime_to_gee_datetime(startdt),
-                                           _datetime_to_gee_datetime(enddt))) \
-                    .map(_addDate) \
-                    .map(rasterExtraction) \
-                    .flatten()
-
+    raster = get_ee_obj(mapinfo, bandname)  # dataset
+    results = (
+        raster.filter(
+            ee.Filter.date(
+                _datetime_to_gee_datetime(startdt), _datetime_to_gee_datetime(enddt)
+            )
+        )
+        .map(_addDate)
+        .map(rasterExtraction)
+        .flatten()
+    )
 
     def format_df(df, obstype, bandname):
-        #format datetime
-        df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d%H%M%S')
+        # format datetime
+        df["datetime"] = pd.to_datetime(df["datetime"], format="%Y%m%d%H%M%S")
         # set timezone
-        df['datetime'] = df['datetime'].dt.tz_localize('UTC')
+        df["datetime"] = df["datetime"].dt.tz_localize("UTC")
 
-        #format index
-        df = df.set_index(['name', 'datetime'])
+        # format index
+        df = df.set_index(["name", "datetime"])
         df = df.sort_index()
 
-        #rename to values to toolkit space
+        # rename to values to toolkit space
         df = df.rename(columns={bandname: obstype})
 
         return df[obstype].to_frame()
 
-
     if not use_drive:
         results = results.getInfo()
 
         # =============================================================================
         # to dataframe
         # =============================================================================
 
         # extract properties
-        properties = [x['properties'] for x in results['features']]
+        properties = [x["properties"] for x in results["features"]]
         df = pd.DataFrame(properties)
 
         df = format_df(df, obstype, bandname)
         return df
 
     else:
-        _filename = 'era5_data'
-        _drivefolder = 'era5_timeseries'
+        _filename = "era5_data"
+        _drivefolder = "era5_timeseries"
 
-        print(f'The timeseries will be writen to your Drive in {_drivefolder}/{_filename} ')
+        print(
+            f"The timeseries will be writen to your Drive in {_drivefolder}/{_filename} "
+        )
 
-        task=ee.batch.Export.table.toDrive(collection=results,
-                                            description='extracting_era5',
-                                            folder=_drivefolder,
-                                            fileNamePrefix=_filename,
-                                            fileFormat='CSV',
-                                            selectors=['datetime', 'name', bandname]
-                                            )
+        task = ee.batch.Export.table.toDrive(
+            collection=results,
+            description="extracting_era5",
+            folder=_drivefolder,
+            fileNamePrefix=_filename,
+            fileFormat="CSV",
+            selectors=["datetime", "name", bandname],
+        )
 
         task.start()
-        print('The google server is handling your request ...')
+        print("The google server is handling your request ...")
         sleep(3)
-        finished=False
+        finished = False
         while finished == False:
-            if task.status()['state'] == "READY":
-                print('Awaitening execution ...')
+            if task.status()["state"] == "READY":
+                print("Awaitening execution ...")
                 sleep(4)
-            elif task.status()['state'] == 'RUNNING':
-                print('Running ...')
+            elif task.status()["state"] == "RUNNING":
+                print("Running ...")
                 sleep(4)
             else:
-                print('finished')
-                finished=True
+                print("finished")
+                finished = True
 
-        doc_folder_id = task.status()['destination_uris'][0]
-        print('The data is transfered! Open the following link in your browser: \n\n')
-        print(f'{doc_folder_id} \n\n')
-        print('To upload the data to the model, use the Modeldata.set_model_from_csv() method')
+        doc_folder_id = task.status()["destination_uris"][0]
+        print("The data is transfered! Open the following link in your browser: \n\n")
+        print(f"{doc_folder_id} \n\n")
+        print(
+            "To upload the data to the model, use the Modeldata.set_model_from_csv() method"
+        )
 
         return init_multiindexdf()
-
-
-
-
-
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/modeldata.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/modeldata.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,125 +3,134 @@
 """
 Created on Wed Mar 22 13:50:17 2023
 
 @author: thoverga
 """
 import pandas as pd
 
-from metobs_toolkit.df_helpers import (init_multiindexdf,
-                                        conv_tz_multiidxdf)
+from metobs_toolkit.df_helpers import init_multiindexdf, conv_tz_multiidxdf
 
-from metobs_toolkit.landcover_functions import (connect_to_gee,
-                                                 gee_extract_timeseries)
+from metobs_toolkit.landcover_functions import connect_to_gee, gee_extract_timeseries
 
 from metobs_toolkit.convertors import convert_to_toolkit_units
 
 from metobs_toolkit.settings import Settings
 
 # =============================================================================
 # Class Model data (collection of external model data)
 # =============================================================================
 
-class Modeldata():
+
+class Modeldata:
     def __init__(self, modelname):
         self.df = init_multiindexdf
         self.modelname = modelname
 
         self._settings = Settings()
-        self.mapinfo=self._settings.gee['gee_dataset_info']
+        self.mapinfo = self._settings.gee["gee_dataset_info"]
 
     def __repr__(self):
-        return f'ModelData instance: {self.modelname} model data of {list(self.df.columns)}'
+        return f"ModelData instance: {self.modelname} model data of {list(self.df.columns)}"
 
     # def _conv_to_timezone(self, tz):
 
+    def get_ERA5_data(self, metadf, startdt, enddt, obstype="temp"):
+        # startdt and enddt IN UTC FORMAT!!!!!
 
-    def get_ERA5_data(self, metadf, startdt, enddt, obstype='temp'):
-
-        #startdt and enddt IN UTC FORMAT!!!!!
-
-        era_mapinfo=self.mapinfo['ERA5_hourly']
+        era_mapinfo = self.mapinfo["ERA5_hourly"]
         # Connect to Gee
         connect_to_gee()
         # Get data using GEE
-        df = gee_extract_timeseries(metadf = metadf,
-                                    mapinfo=era_mapinfo,
-                                    startdt=startdt,
-                                    enddt=enddt,
-                                    obstype=obstype,
-                                    latcolname='lat',
-                                    loncolname='lon')
+        df = gee_extract_timeseries(
+            metadf=metadf,
+            mapinfo=era_mapinfo,
+            startdt=startdt,
+            enddt=enddt,
+            obstype=obstype,
+            latcolname="lat",
+            loncolname="lon",
+        )
         if not df.empty:
             # Convert to toolkit units
-            df[obstype], _tlk_unit = convert_to_toolkit_units(data=df[obstype],
-                                                   data_unit = era_mapinfo['band_of_use'][obstype]['units'])
-
+            df[obstype], _tlk_unit = convert_to_toolkit_units(
+                data=df[obstype], data_unit=era_mapinfo["band_of_use"][obstype]["units"]
+            )
 
         self.df = df
-        self.modelname = 'ERA5_hourly'
-
-    def set_model_from_csv(self, csvpath, modelname='ERA5_hourly', convert_units=True,
-                           obstype='temp', datatimezone='UTC'):
-
-
-
-         df = pd.read_csv(csvpath, sep=',')
-         #format datetime
-         df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d%H%M%S')
-         df['datetime'] = df['datetime'].dt.tz_localize(datatimezone)
-
-         #format index
-         df = df.set_index(['name', 'datetime'])
-         df = df.sort_index()
-
-         #rename to values to toolkit space
-         bandname=self.mapinfo[modelname]['band_of_use'][obstype]['name']
-         df = df.rename(columns={bandname: obstype})
-
-         #convert units
-         if convert_units:
-             df[obstype], _tlk_unit = convert_to_toolkit_units(data=df[obstype],
-                                                    data_unit = self.mapinfo[modelname]['band_of_use'][obstype]['units'])
-         df = df[obstype].to_frame()
-         self.df = df
-         self.modelname=modelname
-
+        self.modelname = "ERA5_hourly"
 
+    def set_model_from_csv(
+        self,
+        csvpath,
+        modelname="ERA5_hourly",
+        convert_units=True,
+        obstype="temp",
+        datatimezone="UTC",
+    ):
+        df = pd.read_csv(csvpath, sep=",")
+        # format datetime
+        df["datetime"] = pd.to_datetime(df["datetime"], format="%Y%m%d%H%M%S")
+        df["datetime"] = df["datetime"].dt.tz_localize(datatimezone)
+
+        # format index
+        df = df.set_index(["name", "datetime"])
+        df = df.sort_index()
+
+        # rename to values to toolkit space
+        bandname = self.mapinfo[modelname]["band_of_use"][obstype]["name"]
+        df = df.rename(columns={bandname: obstype})
+
+        # convert units
+        if convert_units:
+            df[obstype], _tlk_unit = convert_to_toolkit_units(
+                data=df[obstype],
+                data_unit=self.mapinfo[modelname]["band_of_use"][obstype]["units"],
+            )
+        df = df[obstype].to_frame()
+        self.df = df
+        self.modelname = modelname
 
-    def interpolate_modeldata(self, to_multiidx, obstype='temp'):
+    def interpolate_modeldata(self, to_multiidx, obstype="temp"):
         returndf = init_multiindexdf()
 
         recordsdf = init_multiindexdf()
         recordsdf.index = to_multiidx
         # iterate over stations check to avoid extrapolation is done per stations
-        for sta in recordsdf.index.get_level_values('name').unique():
-            sta_recordsdf = recordsdf.xs(sta, level='name', drop_level=False)
-            sta_moddf = self.df.xs(sta, level='name', drop_level=False)
+        for sta in recordsdf.index.get_level_values("name").unique():
+            sta_recordsdf = recordsdf.xs(sta, level="name", drop_level=False)
+            sta_moddf = self.df.xs(sta, level="name", drop_level=False)
 
             # convert modeldata to timezone of observations
-            sta_moddf = conv_tz_multiidxdf(df=sta_moddf,
-                                           timezone=sta_recordsdf.index.get_level_values('datetime').tz)
+            sta_moddf = conv_tz_multiidxdf(
+                df=sta_moddf,
+                timezone=sta_recordsdf.index.get_level_values("datetime").tz,
+            )
 
             # check if modeldata is will not be extrapolated !
-            if min(sta_recordsdf.index.get_level_values('datetime')) < min(sta_moddf.index.get_level_values('datetime')):
-                print('Extrapolation')
-            if max(sta_recordsdf.index.get_level_values('datetime')) > max(sta_moddf.index.get_level_values('datetime')):
-                print('Extrapolation')
+            if min(sta_recordsdf.index.get_level_values("datetime")) < min(
+                sta_moddf.index.get_level_values("datetime")
+            ):
+                print("Extrapolation")
+            if max(sta_recordsdf.index.get_level_values("datetime")) > max(
+                sta_moddf.index.get_level_values("datetime")
+            ):
+                print("Extrapolation")
 
             # combine model and records
-            mergedf = sta_recordsdf.merge(sta_moddf, how='outer',
-                                          left_index=True, right_index=True)
+            mergedf = sta_recordsdf.merge(
+                sta_moddf, how="outer", left_index=True, right_index=True
+            )
 
             # reset index for time interpolation
-            mergedf = mergedf.reset_index().set_index('datetime').sort_index()
+            mergedf = mergedf.reset_index().set_index("datetime").sort_index()
 
             # interpolate missing modeldata
-            mergedf[obstype].interpolate(method='time',
-                                        limit_area='inside',
-                                        inplace=True)
+            mergedf[obstype].interpolate(
+                method="time", limit_area="inside", inplace=True
+            )
             # convert back to multiindex
-            mergedf = mergedf.reset_index().set_index(['name', 'datetime']).sort_index()
-            #filter only records
+            mergedf = mergedf.reset_index().set_index(["name", "datetime"]).sort_index()
+            # filter only records
             mergedf = mergedf.loc[sta_recordsdf.index]
 
             returndf = pd.concat([returndf, mergedf])
         return returndf
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/printing.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/printing.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,36 +6,43 @@
 @author: thoverga
 """
 
 
 from datetime import datetime
 
 
-
-def print_dataset_info(df, outliersdf, gapsdf, fmt_datetime):
-
+def print_dataset_info(df, outliersdf, gapsdf, missing_obs, fmt_datetime):
     if df.empty:
         print("This dataset is empty!")
         # logger.error('The dataset is empty!')
     else:
-        print('\n','--------  General ---------', '\n')
-        print(' .... ')
-
+        print("\n", "--------  General ---------", "\n")
+        print(" .... ")
 
+        print("\n", "--------  Observations ---------", "\n")
+        starttimestr = datetime.strftime(
+            min(df.index.get_level_values(level="datetime")), fmt_datetime
+        )
+        endtimestr = datetime.strftime(
+            max(df.index.get_level_values(level="datetime")), fmt_datetime
+        )
 
-        print('\n','--------  Observations ---------', '\n')
-        starttimestr = datetime.strftime(min(df.index.get_level_values(level='datetime')),
-                                         fmt_datetime)
-        endtimestr = datetime.strftime(max(df.index.get_level_values(level='datetime')),
-                                       fmt_datetime)
-
-        stations_available = list(df.index.get_level_values(level='name').unique())
-        print(f'Observations found for period: {starttimestr} --> {endtimestr}')
+        stations_available = list(df.index.get_level_values(level="name").unique())
+        print(f"Observations found for period: {starttimestr} --> {endtimestr}")
         # logger.debug(f'Observations found for period: {starttimestr} --> {endtimestr}')
-        print(f'Following stations are in dataset: {stations_available}')
+        print(f"Following stations are in dataset: {stations_available}")
         # logger.debug(f'Following stations are in dataset: {stations_available}')
 
-        print('\n', '--------  Outliers ---------', '\n')
-        print(f'There are {outliersdf.shape[0]} flagged observations found in total. They occure in these stations: {list(outliersdf.index.get_level_values("name").unique())}')
-
-        print('\n', '--------  Gaps ---------', '\n')
-        print(f'There are {gapsdf.shape[0]} gaps found in total. They occure in these stations: {list(gapsdf.index.unique())}')
+        print("\n", "--------  Outliers ---------", "\n")
+        print(
+            f'There are {outliersdf.shape[0]} flagged observations found in total. They occure in these stations: {list(outliersdf.index.get_level_values("name").unique())}'
+        )
+
+        print("\n", "--------  Missing observations ---------", "\n")
+        print(
+            f"There are {missing_obs.shape[0]} missing observations in total. They occure in these stations: {list(missing_obs.index.unique())}"
+        )
+
+        print("\n", "--------  Gaps ---------", "\n")
+        print(
+            f"There are {gapsdf.shape[0]} gaps found in total. They occure in these stations: {list(gapsdf.index.unique())}"
+        )
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/qc_checks.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/qc_checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import sys
 import pandas as pd
 import numpy as np
 import logging
 
 
-from metobs_toolkit.df_helpers import (init_multiindex,
-                                        init_multiindexdf)
-
-
-
+from metobs_toolkit.df_helpers import (
+    init_multiindex,
+    init_multiindexdf,
+    init_triple_multiindexdf,
+)
 
 
 logger = logging.getLogger(__name__)
 
 
-
 # =============================================================================
 # Helper functions
 # =============================================================================
 
 
-def make_outlier_df_for_check(station_dt_list, obsdf, obstype,
-                              flagcolumnname, flag,
-                              add_obstype_prefix_to_label=True,
-                              stationname=None, datetimelist=None):
+def make_outlier_df_for_check(
+    station_dt_list, obsdf, obstype, flag, stationname=None, datetimelist=None
+):
     """
-    V4
+    V5
     Helper function to create an outlier dataframe for the given station(s) and datetimes. This will be returned by
     a quality control check and later added to the dastes.outlierdf.
 
     Multiple commum inputstructures can be handles
 
     A multiindex dataframe with the relevant observationtypes i.e. the values_in_dict and a specific quality flag column (i.g. the labels) is returned.
 
@@ -59,94 +57,105 @@
     Returns
 
     check_outliers : pd.Dataframe
         A multiindex (name -- datetime) datatframe with one column (columname) and all
         values are the flag.
     """
 
-    if add_obstype_prefix_to_label:
-        flagcolumnname = obstype + '_' + flagcolumnname
-
-
-    columnorder =[obstype, flagcolumnname]
-
-    #Create outliersdf
-
     if isinstance(station_dt_list, pd.MultiIndex):
         multi_idx = station_dt_list
 
-    elif isinstance(station_dt_list, list): #list of tuples: (name, datetime)
-        multi_idx = pd.MultiIndex.from_tuples(station_dt_list, names=['name', 'datetime'])
+    elif isinstance(station_dt_list, list):  # list of tuples: (name, datetime)
+        multi_idx = pd.MultiIndex.from_tuples(
+            station_dt_list, names=["name", "datetime"]
+        )
     elif not isinstance(stationname, type(None)):
         if isinstance(datetimelist, pd.DatetimeIndex):
             datetimelist = datetimelist.to_list()
         if isinstance(datetimelist, list):
-            indexarrays = list(zip([stationname]*len(datetimelist), datetimelist))
-            multi_idx = pd.MultiIndex.from_tuples(indexarrays, names=['name', 'datetime'])
+            indexarrays = list(zip([stationname] * len(datetimelist), datetimelist))
+            multi_idx = pd.MultiIndex.from_tuples(
+                indexarrays, names=["name", "datetime"]
+            )
 
         else:
-            sys.exit(f'Type of datetimelist: {type(datetimelist)} is not implemented.')
+            sys.exit(f"Type of datetimelist: {type(datetimelist)} is not implemented.")
+
+    # subset outliers
+    outliersdf = obsdf.loc[multi_idx]
+
+    # make the triple multiindex
+    outliersdf["obstype"] = obstype
+    outliersdf = outliersdf.set_index("obstype", append=True)
 
-    # create outliers df
-    check_outliers = pd.DataFrame(data=flag, index=station_dt_list, columns=[flagcolumnname])
-    check_outliers[obstype] = obsdf.loc[multi_idx, obstype]
-    check_outliers = check_outliers[columnorder]
+    # add flag
+    outliersdf["label"] = flag
 
-    #replace values in obsdf by Nan
+    # subset columns
+    outliersdf = outliersdf[[obstype, "label"]].rename(columns={obstype: "value"})
+
+    # replace values in obsdf by Nan
     obsdf.loc[multi_idx, obstype] = np.nan
 
-    return obsdf, check_outliers
+    return obsdf, outliersdf
+
 
 # =============================================================================
 # Quality assesment checks on data import
 # =============================================================================
 
 
-
 def invalid_input_check(df, checks_info):
-
-    checkname = 'invalid_input'
+    checkname = "invalid_input"
 
     # fast scan wich stations and obstypes have nan outliers
-    groups = df.reset_index().groupby('name').apply(lambda x: (np.isnan(x).any()) & (np.isnan(x).all() == False))
-
+    groups = (
+        df.reset_index()
+        .groupby("name")
+        .apply(lambda x: (np.isnan(x).any()) & (np.isnan(x).all() == False))
+    )
 
-    #extract all obstype that have outliers
+    # extract all obstype that have outliers
     outl_obstypes = groups.apply(lambda x: x.any(), axis=0)
     outl_obstypes = outl_obstypes[outl_obstypes].index.to_list()
 
-    #first loop over the smallest sample: outlier obstypes
+    # first loop over the smallest sample: outlier obstypes
     outl_dict = {}
 
     for obstype in outl_obstypes:
-        #get stations that have ouliers for this obstype
+        # get stations that have ouliers for this obstype
         outl_stations = groups.loc[groups[obstype], obstype].index.to_list()
 
         outl_multiidx = init_multiindex()
         for sta in outl_stations:
-            #apply check per station
-            outl_idx = df.xs(sta, level='name', drop_level=False)[obstype].isnull().loc[lambda x: x].index
+            # apply check per station
+            outl_idx = (
+                df.xs(sta, level="name", drop_level=False)[obstype]
+                .isnull()
+                .loc[lambda x: x]
+                .index
+            )
             outl_multiidx = outl_multiidx.append(outl_idx)
 
-        outl_dict[obstype]=outl_multiidx
+        outl_dict[obstype] = outl_multiidx
 
-    #create outliersdf for all outliers for all osbtypes
+    # create outliersdf for all outliers for all osbtypes
     outl_df = init_multiindexdf()
     for obstype, outliers in outl_dict.items():
-        df, specific_outl_df = make_outlier_df_for_check(station_dt_list=outliers,
-                                                     obsdf=df,
-                                                     obstype=obstype,
-                                                     flagcolumnname= checks_info[checkname]['label_columnname'],
-                                                     flag=checks_info[checkname]['outlier_flag'])
+        df, specific_outl_df = make_outlier_df_for_check(
+            station_dt_list=outliers,
+            obsdf=df,
+            obstype=obstype,
+            flag=checks_info[checkname]["outlier_flag"],
+        )
         outl_df = pd.concat([outl_df, specific_outl_df])
 
     return df, outl_df
 
 
-
 def duplicate_timestamp_check(df, checks_info, checks_settings):
     """
     V3
     Looking for duplcate timestaps per station. Duplicated records are removed by the method specified in the qc_settings.
 
     Parameters
 
@@ -156,49 +165,68 @@
     Returns
 
     df : pandas.DataFrame()
         The observations dataframe updated for duplicate timestamps. Duplicated timestamps are removed.
 
     """
 
-    checkname = 'duplicated_timestamp'
-
+    checkname = "duplicated_timestamp"
 
-
-    duplicates = pd.Series(data=df.index.duplicated(keep=checks_settings[checkname]['keep']),
-                           index=df.index)
+    duplicates = pd.Series(
+        data=df.index.duplicated(keep=checks_settings[checkname]["keep"]),
+        index=df.index,
+    )
 
     if not df.loc[duplicates].empty:
-        logging.warning(f' Following records are labeld as duplicates: {df.loc[duplicates]}, and are removed')
-
-
-    #Fill the outlierdf with the duplicates
-    outliers = df[df.index.duplicated(keep=checks_settings[checkname]['keep'])]
+        logging.warning(
+            f" Following records are labeld as duplicates: {df.loc[duplicates]}, and are removed"
+        )
 
+    # Fill the outlierdf with the duplicates
+    outliers = df[df.index.duplicated(keep=checks_settings[checkname]["keep"])]
 
-    # replace observation values by nan
+    # convert values to nan in obsdf
     for obstype in df.columns:
         df.loc[outliers.index, obstype] = np.nan
 
+    # ------- Create a outliersdf -----------#
+    # the 'make outliersdf' function cannont be use because of duplicated indices
+
+    outliers = outliers.rename(
+        columns={col: "value_" + col for col in outliers.columns}
+    )
+    outliers = outliers.reset_index()
+    outliers["_to_get_unique_idx"] = np.arange(outliers.shape[0])
+
+    outliersdf = pd.wide_to_long(
+        df=outliers,
+        stubnames="value",
+        sep="_",
+        suffix=r"\w+",  # to use non-integer suffexes
+        i=["name", "datetime", "_to_get_unique_idx"],
+        j="obstype",
+    )
+    # remove the temorary level from the index
+    outliersdf = outliersdf.droplevel("_to_get_unique_idx", axis=0)
+
+    # add label column
+    outliersdf["label"] = checks_info[checkname]["outlier_flag"]
+
     # drop duplicates in the obsdf, because this gives a lot of troubles
     # The method does not really mater because the values are set to nan in the observations
-    df = df[~df.index.duplicated(keep='first')]
+    df = df[~df.index.duplicated(keep="first")]
 
+    return df, outliersdf
 
-    #add label
-    outliers[checks_info[checkname]['label_columnname']] = checks_info[checkname]['outlier_flag']
-
-    return df, outliers
 
 # =============================================================================
 # Quality assesment checks on dataset
 # =============================================================================
 
 
-
 def gross_value_check(obsdf, obstype, checks_info, checks_settings):
     """
     Looking for values of an observation type that are not physical. These values are labeled and the physical limits are specified in the qc_settings.
 
     Parameters
 
     input_series : pandas.Series
@@ -214,48 +242,48 @@
         The observations series updated for this check. Observations that didn't pass are removed.
 
     outlier_df : pandas.DataFrame
         The collection of records flagged as outliers by this check.
 
     """
 
-    checkname = 'gross_value'
+    checkname = "gross_value"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
-        logger.warning(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
+        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
+        logger.warning(
+            f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
+        )
         return obsdf, init_multiindexdf()
 
-
     # drop outliers from the series (these are Nan's)
     input_series = obsdf[obstype].dropna()
 
-
-    #find outlier observations as a list of tuples [(name, datetime), (name, datetime)]
-    outl_obs = input_series.loc[(input_series <= specific_settings['min_value']) |
-                                (input_series >= specific_settings['max_value'])
-                                ].index.to_list()
-
-    #make new obsdf and outlierdf
-    obsdf, outlier_df = make_outlier_df_for_check(station_dt_list=outl_obs,
-                                           obsdf=obsdf,
-                                           obstype=obstype,
-                                           flagcolumnname=checks_info[checkname]['label_columnname'],
-                                           flag=checks_info[checkname]['outlier_flag'])
-
+    # find outlier observations as a list of tuples [(name, datetime), (name, datetime)]
+    outl_obs = input_series.loc[
+        (input_series <= specific_settings["min_value"])
+        | (input_series >= specific_settings["max_value"])
+    ].index.to_list()
+
+    # make new obsdf and outlierdf
+    obsdf, outlier_df = make_outlier_df_for_check(
+        station_dt_list=outl_obs,
+        obsdf=obsdf,
+        obstype=obstype,
+        flag=checks_info[checkname]["outlier_flag"],
+    )
 
     return obsdf, outlier_df
 
 
-
-def persistance_check(station_frequencies, obsdf, obstype, checks_info,
-                      checks_settings):
-
+def persistance_check(
+    station_frequencies, obsdf, obstype, checks_info, checks_settings
+):
     """
     V3
     Looking for values of an observation type that do not change during a timewindow. These are flagged as outliers.
 
     In order to perform this check, at least N observations chould be in that time window.
 
 
@@ -274,79 +302,101 @@
             The observations series updated for this check. Observations that didn't pass are removed.
 
         outlier_df : pandas.DataFrame
             The collection of records flagged as outliers by this check.
 
     """
 
-    checkname = 'persistance'
+    checkname = "persistance"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
-        logger.warning(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
+        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
+        logger.warning(
+            f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
+        )
         return obsdf, init_multiindexdf()
 
-    invalid_windows_check_df = pd.to_timedelta(specific_settings['time_window_to_check'])/station_frequencies < specific_settings['min_num_obs']
-    invalid_stations = list(invalid_windows_check_df[invalid_windows_check_df == True].index)
+    invalid_windows_check_df = (
+        pd.to_timedelta(specific_settings["time_window_to_check"]) / station_frequencies
+        < specific_settings["min_num_obs"]
+    )
+    invalid_stations = list(
+        invalid_windows_check_df[invalid_windows_check_df == True].index
+    )
     if bool(invalid_stations):
-        print(f'The windows are too small for stations  {invalid_stations} to perform persistance check')
-        logger.info(f'The windows are too small for stations  {invalid_stations} to perform persistance check')
+        print(
+            f"The windows are too small for stations  {invalid_stations} to perform persistance check"
+        )
+        logger.info(
+            f"The windows are too small for stations  {invalid_stations} to perform persistance check"
+        )
 
-    subset_not_used = obsdf[obsdf.index.get_level_values('name').isin(invalid_stations)]
-    subset_used = obsdf[~obsdf.index.get_level_values('name').isin(invalid_stations)]
+    subset_not_used = obsdf[obsdf.index.get_level_values("name").isin(invalid_stations)]
+    subset_used = obsdf[~obsdf.index.get_level_values("name").isin(invalid_stations)]
 
     if not subset_used.empty:
         # drop outliers from the series (these are Nan's)
         input_series = subset_used[obstype].dropna()
 
-
-        #apply persistance
-        def is_unique(window):   #comp order of N (while using the 'unique' function is Nlog(N))
+        # apply persistance
+        def is_unique(
+            window,
+        ):  # comp order of N (while using the 'unique' function is Nlog(N))
             a = window.values
             a = a[~np.isnan(a)]
             return (a[0] == a).all()
 
-        #TODO: Tis is very expensive if no coarsening is applied !!!! Can we speed this up?
-        window_output = input_series.reset_index(level=0).groupby('name').rolling(window= specific_settings['time_window_to_check'],
-                                                                                closed='both',
-                                                                                center=True,
-                                                                                min_periods=specific_settings['min_num_obs']).apply(is_unique)
-
+        # TODO: Tis is very expensive if no coarsening is applied !!!! Can we speed this up?
+        window_output = (
+            input_series.reset_index(level=0)
+            .groupby("name")
+            .rolling(
+                window=specific_settings["time_window_to_check"],
+                closed="both",
+                center=True,
+                min_periods=specific_settings["min_num_obs"],
+            )
+            .apply(is_unique)
+        )
 
         list_of_outliers = []
         outl_obs = window_output.loc[window_output[obstype] == True].index
         for outlier in outl_obs:
-            outliers_list = get_outliers_in_daterange(input_series, outlier[1], outlier[0], specific_settings['time_window_to_check'], station_frequencies)
+            outliers_list = get_outliers_in_daterange(
+                input_series,
+                outlier[1],
+                outlier[0],
+                specific_settings["time_window_to_check"],
+                station_frequencies,
+            )
 
             list_of_outliers.extend(outliers_list)
 
         list_of_outliers = list(set(list_of_outliers))
 
-
-        #make new obsdf and outlierdf
-        subset_used, outlier_df = make_outlier_df_for_check(station_dt_list=list_of_outliers,
-                                               obsdf=subset_used,
-                                               obstype=obstype,
-                                               flagcolumnname=checks_info[checkname]['label_columnname'],
-                                               flag=checks_info[checkname]['outlier_flag'])
+        # make new obsdf and outlierdf
+        subset_used, outlier_df = make_outlier_df_for_check(
+            station_dt_list=list_of_outliers,
+            obsdf=subset_used,
+            obstype=obstype,
+            flag=checks_info[checkname]["outlier_flag"],
+        )
 
         obsdf = pd.concat([subset_used, subset_not_used])
 
         return obsdf, outlier_df
 
     else:
         obsdf = pd.concat([subset_used, subset_not_used])
 
         return obsdf, init_multiindexdf()
 
 
-
-
 def repetitions_check(obsdf, obstype, checks_info, checks_settings):
     """
     Looking for values of an observation type that are repeated at least with the frequency specified in the qc_settings. These values are labeled.
 
     Parameters
 
     input_series : pandas.Series
@@ -363,59 +413,58 @@
 
     outlier_df : pandas.DataFrame
         The collection of records flagged as outliers by this check.
 
 
     """
 
-    checkname = 'repetitions'
+    checkname = "repetitions"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
-        logger.warning(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
+        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
+        logger.warning(
+            f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
+        )
         return obsdf, init_multiindexdf()
 
-
     # drop outliers from the series (these are Nan's)
     input_series = obsdf[obstype].dropna()
 
-    #find outlier datetimes
+    # find outlier datetimes
 
-    #add time interval between two consecutive records, group by consecutive records without missing records
+    # add time interval between two consecutive records, group by consecutive records without missing records
 
-    time_diff = input_series.index.get_level_values('datetime').to_series().diff()
-    time_diff.index = input_series.index #back to multiindex
+    time_diff = input_series.index.get_level_values("datetime").to_series().diff()
+    time_diff.index = input_series.index  # back to multiindex
 
     persistance_filter = ((input_series.shift() != input_series)).cumsum()
 
-
-    grouped = input_series.groupby(['name', persistance_filter])
-    #the above line groups the observations which have the same value and consecutive datetimes.
+    grouped = input_series.groupby(["name", persistance_filter])
+    # the above line groups the observations which have the same value and consecutive datetimes.
     group_sizes = grouped.size()
-    outlier_groups = group_sizes[group_sizes > specific_settings['max_valid_repetitions']]
-
-
+    outlier_groups = group_sizes[
+        group_sizes > specific_settings["max_valid_repetitions"]
+    ]
 
-    #add to outl_obs.
+    # add to outl_obs.
     outl_obs = []
     for group_idx in outlier_groups.index:
         groupseries = grouped.get_group(group_idx)
-        if len(set(groupseries)) == 1: #Check if all observations are equal in group
+        if len(set(groupseries)) == 1:  # Check if all observations are equal in group
             outl_obs.extend(groupseries.index.to_list())
 
-
-    #make new obsdf and outlierdf
-    obsdf, outlier_df = make_outlier_df_for_check(station_dt_list=outl_obs,
-                                           obsdf=obsdf,
-                                           obstype=obstype,
-                                           flagcolumnname=checks_info[checkname]['label_columnname'],
-                                           flag=checks_info[checkname]['outlier_flag'])
-
+    # make new obsdf and outlierdf
+    obsdf, outlier_df = make_outlier_df_for_check(
+        station_dt_list=outl_obs,
+        obsdf=obsdf,
+        obstype=obstype,
+        flag=checks_info[checkname]["outlier_flag"],
+    )
 
     return obsdf, outlier_df
 
 
 def step_check(obsdf, obstype, checks_info, checks_settings):
     """
 
@@ -441,54 +490,68 @@
          The observations series updated for this check. Observations that didn't pass are removed.
 
      outlier_df : pandas.DataFrame
          The collection of records flagged as outliers by this check.
 
     """
 
-    checkname='step'
+    checkname = "step"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
-        logger.warning(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
+        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
+        logger.warning(
+            f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
+        )
         return obsdf, init_multiindexdf()
 
     # drop outliers from the series (these are Nan's)
     input_series = obsdf[obstype].dropna()
 
-
     list_of_outliers = []
 
-    for name in input_series.index.droplevel('datetime').unique():
-        subdata = input_series.xs(name, level='name', drop_level=False)
-
-        time_diff = subdata.index.get_level_values('datetime').to_series().diff()
-        time_diff.index = subdata.index #back to multiindex
-        #define filter
-        step_filter = (((subdata - subdata.shift(1)) > (specific_settings['max_increase_per_second']*time_diff.dt.total_seconds())) | ((subdata - subdata.shift(1)) < (specific_settings['max_decrease_per_second']*time_diff.dt.total_seconds()))) #&
-                       #(time_diff == station_frequencies[name]))
-        outl_obs = step_filter[step_filter==True].index
+    for name in input_series.index.droplevel("datetime").unique():
+        subdata = input_series.xs(name, level="name", drop_level=False)
 
+        time_diff = subdata.index.get_level_values("datetime").to_series().diff()
+        time_diff.index = subdata.index  # back to multiindex
+        # define filter
+        step_filter = (
+            (subdata - subdata.shift(1))
+            > (
+                specific_settings["max_increase_per_second"]
+                * time_diff.dt.total_seconds()
+            )
+        ) | (
+            (subdata - subdata.shift(1))
+            < (
+                specific_settings["max_decrease_per_second"]
+                * time_diff.dt.total_seconds()
+            )
+        )  # &
+        # (time_diff == station_frequencies[name]))
+        outl_obs = step_filter[step_filter == True].index
 
         list_of_outliers.extend(outl_obs)
 
-
-
-    #make new obsdf and outlierdf
-    obsdf, outlier_df = make_outlier_df_for_check(station_dt_list=list_of_outliers,
-                                           obsdf=obsdf,
-                                           obstype=obstype,
-                                           flagcolumnname=checks_info[checkname]['label_columnname'],
-                                           flag=checks_info[checkname]['outlier_flag'])
+    # make new obsdf and outlierdf
+    obsdf, outlier_df = make_outlier_df_for_check(
+        station_dt_list=list_of_outliers,
+        obsdf=obsdf,
+        obstype=obstype,
+        flag=checks_info[checkname]["outlier_flag"],
+    )
 
     return obsdf, outlier_df
 
-def window_variation_check(station_frequencies, obsdf, obstype, checks_info, checks_settings):
+
+def window_variation_check(
+    station_frequencies, obsdf, obstype, checks_info, checks_settings
+):
     """
 
     V3
     Looking for jumps of the values of an observation type that are larger than the limit specified in the qc_settings. These values are removed from
     the input series and combined in the outlier df.
 
     There is a increament threshold (that is if there is a max value difference and the maximum value occured later than the minimum value occured.)
@@ -515,99 +578,127 @@
      updated_obs_series : pandas.Series
          The observations series updated for this check. Observations that didn't pass are removed.
 
      outlier_df : pandas.DataFrame
          The collection of records flagged as outliers by this check.
 
     """
-    checkname='window_variation'
+    checkname = "window_variation"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
-        logger.warning(f'No {checkname} settings found for obstype={obstype}. Check is skipped!')
+        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
+        logger.warning(
+            f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
+        )
         return obsdf, init_multiindexdf()
 
-    invalid_windows_check_df = pd.to_timedelta(specific_settings['time_window_to_check'])/station_frequencies < specific_settings['min_window_members']
-    invalid_stations = list(invalid_windows_check_df[invalid_windows_check_df == True].index)
+    invalid_windows_check_df = (
+        pd.to_timedelta(specific_settings["time_window_to_check"]) / station_frequencies
+        < specific_settings["min_window_members"]
+    )
+    invalid_stations = list(
+        invalid_windows_check_df[invalid_windows_check_df == True].index
+    )
     if bool(invalid_stations):
-        print(f'The windows are too small for stations  {invalid_stations} to perform window variation check')
-        logger.info(f'The windows are too small for stations  {invalid_stations} to perform window variation check')
+        print(
+            f"The windows are too small for stations  {invalid_stations} to perform window variation check"
+        )
+        logger.info(
+            f"The windows are too small for stations  {invalid_stations} to perform window variation check"
+        )
 
-    subset_not_used = obsdf[obsdf.index.get_level_values('name').isin(invalid_stations)]
-    subset_used = obsdf[~obsdf.index.get_level_values('name').isin(invalid_stations)]
+    subset_not_used = obsdf[obsdf.index.get_level_values("name").isin(invalid_stations)]
+    subset_used = obsdf[~obsdf.index.get_level_values("name").isin(invalid_stations)]
 
     if not subset_used.empty:
-
         # drop outliers from the series (these are Nan's)
         input_series = subset_used[obstype].dropna()
 
-
         # Calculate window thresholds (by linear extarpolation)
-        windowsize_seconds = pd.Timedelta(specific_settings['time_window_to_check']).total_seconds()
-        max_window_increase = specific_settings['max_increase_per_second'] * windowsize_seconds
-        max_window_decrease = specific_settings['max_decrease_per_second'] * windowsize_seconds
+        windowsize_seconds = pd.Timedelta(
+            specific_settings["time_window_to_check"]
+        ).total_seconds()
+        max_window_increase = (
+            specific_settings["max_increase_per_second"] * windowsize_seconds
+        )
+        max_window_decrease = (
+            specific_settings["max_decrease_per_second"] * windowsize_seconds
+        )
 
-
-        #apply steptest
+        # apply steptest
         def variation_test(window):
-            if ((max(window) - min(window) > max_window_increase) &
-                (window.idxmax() > window.idxmin())):
+            if (max(window) - min(window) > max_window_increase) & (
+                window.idxmax() > window.idxmin()
+            ):
                 return 1
 
-            if ((max(window) - min(window) > max_window_decrease) &
-                (window.idxmax() < window.idxmin())):
+            if (max(window) - min(window) > max_window_decrease) & (
+                window.idxmax() < window.idxmin()
+            ):
                 return 1
             else:
                 return 0
 
-        window_output = input_series.reset_index(level=0).groupby('name').rolling(window=specific_settings['time_window_to_check'],
-                                                                                  closed='both',
-                                                                                  center=True,
-                                                                                  min_periods=specific_settings['min_window_members']).apply(variation_test)
+        window_output = (
+            input_series.reset_index(level=0)
+            .groupby("name")
+            .rolling(
+                window=specific_settings["time_window_to_check"],
+                closed="both",
+                center=True,
+                min_periods=specific_settings["min_window_members"],
+            )
+            .apply(variation_test)
+        )
 
         list_of_outliers = []
         outl_obs = window_output.loc[window_output[obstype] == 1].index
 
         for outlier in outl_obs:
-            outliers_list = get_outliers_in_daterange(input_series, outlier[1], outlier[0], specific_settings['time_window_to_check'], station_frequencies)
+            outliers_list = get_outliers_in_daterange(
+                input_series,
+                outlier[1],
+                outlier[0],
+                specific_settings["time_window_to_check"],
+                station_frequencies,
+            )
 
             list_of_outliers.extend(outliers_list)
 
         list_of_outliers = list(set(list_of_outliers))
 
-        #make new obsdf and outlierdf
-        subset_used, outlier_df = make_outlier_df_for_check(station_dt_list=list_of_outliers,
-                                                      obsdf=subset_used,
-                                                      obstype=obstype,
-                                                      flagcolumnname=checks_info[checkname]['label_columnname'],
-                                                      flag=checks_info[checkname]['outlier_flag'])
+        # make new obsdf and outlierdf
+        subset_used, outlier_df = make_outlier_df_for_check(
+            station_dt_list=list_of_outliers,
+            obsdf=subset_used,
+            obstype=obstype,
+            flag=checks_info[checkname]["outlier_flag"],
+        )
 
         obsdf = pd.concat([subset_used, subset_not_used])
 
         return obsdf, outlier_df
 
     else:
         obsdf = pd.concat([subset_used, subset_not_used])
 
         return obsdf, init_multiindexdf()
 
 
 def get_outliers_in_daterange(input_data, date, name, time_window, station_freq):
-    end_date = date + (pd.Timedelta(time_window)/2).floor(station_freq[name])
-    start_date = date - (pd.Timedelta(time_window)/2).floor(station_freq[name])
-
-    daterange = pd.date_range(start=start_date, end = end_date, freq=station_freq[name])
+    end_date = date + (pd.Timedelta(time_window) / 2).floor(station_freq[name])
+    start_date = date - (pd.Timedelta(time_window) / 2).floor(station_freq[name])
 
-    multi_idx = pd.MultiIndex.from_arrays(arrays=[[name]*len(daterange), daterange.to_list()],
-                                          sortorder=1,
-                                          names=['name', 'datetime'])
-    outlier_sub_df = pd.DataFrame(data=None,
-                                         index=multi_idx,
-                                         columns=None)
+    daterange = pd.date_range(start=start_date, end=end_date, freq=station_freq[name])
 
+    multi_idx = pd.MultiIndex.from_arrays(
+        arrays=[[name] * len(daterange), daterange.to_list()],
+        sortorder=1,
+        names=["name", "datetime"],
+    )
+    outlier_sub_df = pd.DataFrame(data=None, index=multi_idx, columns=None)
 
     intersection = outlier_sub_df.index.intersection(input_data.dropna().index).values
 
     return intersection
-
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/qc_statistics.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/qc_statistics.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,98 +9,121 @@
 """
 
 
 import pandas as pd
 import logging
 
 
-
 logger = logging.getLogger(__name__)
 
-def get_freq_statistics(comb_df, obstype, checks_info, gaps_info):
 
-    outlier_labels = [qc['outlier_flag'] for qc in checks_info.values()]
+def get_freq_statistics(comb_df, obstype, checks_info, gaps_info, applied_qc_order):
+    outlier_labels = [qc["outlier_flag"] for qc in checks_info.values()]
 
-    if not obstype+'_final_label' in comb_df.columns:
-        print(f'Final observation label for {obstype} is not computed!')
+    if not obstype + "_final_label" in comb_df.columns:
+        print(f"Final observation label for {obstype} is not computed!")
         return (None, None, None)
 
-    final_counts = comb_df[obstype+'_final_label'].value_counts()
+    final_counts = comb_df[obstype + "_final_label"].value_counts()
 
-    #add missing labels
+    # add missing labels
     # QC labels
     non_triggered_labels_dict = {}
-    #fill with zeros for non-triggered checks
+    # fill with zeros for non-triggered checks
     for outl_label in outlier_labels:
         if not outl_label in final_counts.index:
             non_triggered_labels_dict[outl_label] = 0
 
-    #gaps
-    if not gaps_info['gap']['outlier_flag'] in final_counts.index:
-        non_triggered_labels_dict[gaps_info['gap']['outlier_flag']] = 0
-
-    #missing timestamps
-    if not gaps_info['missing_timestamp']['outlier_flag'] in final_counts.index:
-        non_triggered_labels_dict[gaps_info['missing_timestamp']['outlier_flag']] = 0
-
+    # gaps
+    if not gaps_info["gap"]["outlier_flag"] in final_counts.index:
+        non_triggered_labels_dict[gaps_info["gap"]["outlier_flag"]] = 0
+
+    # missing timestamps
+    if not gaps_info["missing_timestamp"]["outlier_flag"] in final_counts.index:
+        non_triggered_labels_dict[gaps_info["missing_timestamp"]["outlier_flag"]] = 0
 
     non_triggered_labels = pd.Series(non_triggered_labels_dict)
     final_counts = pd.concat([final_counts, non_triggered_labels])
-    tot_n_obs= final_counts.sum()
+    tot_n_obs = final_counts.sum()
 
     # to percentages
-    final_counts = (final_counts/tot_n_obs)*100.0
-
-
+    final_counts = (final_counts / tot_n_obs) * 100.0
 
     # ------- aggregate outliers ----------
 
-
-
     # 1 agg to ok - outlier - gap - missing
 
-    agg_dict = {
-        'ok': final_counts["ok"].squeeze(),
-        'QC outliers': final_counts.loc[final_counts.index.isin(outlier_labels)].sum(),
-        'missing (gaps)': final_counts[gaps_info['gap']['outlier_flag']].squeeze(),
-        'missing (individual)': final_counts[gaps_info['missing_timestamp']['outlier_flag']].squeeze()
-        }
-
+    try:
+        agg_ok = final_counts["ok"].squeeze()
+    except KeyError:
+        agg_ok = 0.0
 
-    #2 indevidual outliers
-    outl_dict =  final_counts.loc[final_counts.index.isin(outlier_labels)].to_dict()
+    agg_dict = {
+        "ok": agg_ok,
+        "QC outliers": final_counts.loc[final_counts.index.isin(outlier_labels)].sum(),
+        "missing (gaps)": final_counts[gaps_info["gap"]["outlier_flag"]].squeeze(),
+        "missing (individual)": final_counts[
+            gaps_info["missing_timestamp"]["outlier_flag"]
+        ].squeeze(),
+    }
 
+    # 2 indevidual outliers
+    outl_dict = final_counts.loc[final_counts.index.isin(outlier_labels)].to_dict()
 
     # 3 Effectivenes per check
 
-    qc_label_columns = [col for col in comb_df.columns if not col in [obstype, obstype+'_final_label' ] ]
+    specific_counts = {}
+    # Note: some complexity because observations can be removed by privious executed checsk,
+    # so construct the counts in the order of the applied checks
+
+    applied_qc_order = (
+        applied_qc_order.drop_duplicates()
+    )  # when qc applied mulitple times on same obstype
+    applied_checks = applied_qc_order.loc[applied_qc_order["obstype"] == obstype][
+        "checkname"
+    ].to_list()
+
+    percent_rejected_before = 0.0
+
+    for checkname in applied_checks:
+        try:
+            specific_outliers = final_counts.loc[checks_info[checkname]["outlier_flag"]]
+        except KeyError:
+            specific_outliers = 0.0
+
+        not_checked = percent_rejected_before
+        ok = 100.0 - specific_outliers - not_checked
+
+        specific_counts[checkname] = {
+            "not checked": not_checked,
+            "ok": ok,
+            "outlier": specific_outliers,
+        }
 
-    mapper = {qc_type['outlier_flag']: 'outlier' for qc_type in checks_info.values()}
-    specific_counts = comb_df.replace(mapper).reset_index()[qc_label_columns] \
-                            .transpose().apply(pd.Series.value_counts, axis=1).fillna(0) #\
-                            # .to_dict(orient='index')
+        percent_rejected_before += specific_outliers
 
-    # convert to percentages and dict
-    specific_counts = ((specific_counts/tot_n_obs) * 100).to_dict(orient='index')
+    # add checks that are not performed
+    not_perf_checknames = [
+        check for check in checks_info.keys() if not check in applied_checks
+    ]
+    for checkname in not_perf_checknames:
+        specific_counts[checkname] = {"not checked": 100.0, "ok": 0.0, "outlier": 0.0}
 
-    # specific_counts[Settings.gaps_info['gap']['label_columnname']] = {}
+    # add Gaps
     gap_specific_counts = {
-        'not checked': 0, #all obs are always checked
-        'ok': 100.0 - final_counts[gaps_info['gap']['outlier_flag']],
-        'outlier': final_counts[gaps_info['gap']['outlier_flag']]
-        }
-    specific_counts[gaps_info['gap']['label_columnname']] = gap_specific_counts
+        "not checked": 0,  # all obs are always checked
+        "ok": 100.0 - final_counts[gaps_info["gap"]["outlier_flag"]],
+        "outlier": final_counts[gaps_info["gap"]["outlier_flag"]],
+    }
+    specific_counts[gaps_info["gap"]["label_columnname"]] = gap_specific_counts
 
-
-    #misssing timestamps
+    # misssing timestamps
     missing_specific_counts = {
-        'not checked': 0, #all obs are always checked
-        'ok': 100.0 - final_counts[gaps_info['missing_timestamp']['outlier_flag']],
-        'outlier': final_counts[gaps_info['missing_timestamp']['outlier_flag']]
-        }
-    specific_counts[gaps_info['missing_timestamp']['label_columnname']] = missing_specific_counts
+        "not checked": 0,  # all obs are always checked
+        "ok": 100.0 - final_counts[gaps_info["missing_timestamp"]["outlier_flag"]],
+        "outlier": final_counts[gaps_info["missing_timestamp"]["outlier_flag"]],
+    }
+    specific_counts[
+        gaps_info["missing_timestamp"]["label_columnname"]
+    ] = missing_specific_counts
 
     return (agg_dict, outl_dict, specific_counts)
-
-
-
-
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/settings.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,31 +14,33 @@
 
 # connect to logger
 logger = logging.getLogger(__name__)
 
 
 class Settings:
     # make settingsfiles path
-    _settings_files_path = os.path.join(
-        str(Path(__file__).parent), 'settings_files')
+    _settings_files_path = os.path.join(str(Path(__file__).parent), "settings_files")
 
     def __init__(self):
-        logger.info('Initialising settings')
+        logger.info("Initialising settings")
 
         # define thematics in settings. Corresponds to settings files.
         self.db = {}
         self.time_settings = {}
         self.app = {}
         self.qc = {}
         self.gap = {}
+        self.missing_obs = {}
         self.templates = {}
         self.gee = {}
-        self.IO = {'output_folder': None,
-                   'input_data_file': None,
-                   'input_metadata_file': None}
+        self.IO = {
+            "output_folder": None,
+            "input_data_file": None,
+            "input_metadata_file": None,
+        }
 
         # Update (instance and class variables) what can be updated by setingsfiles
         self._update_db_settings()
         self._update_time_res_settings()
         self._update_app_settings()
         self._update_qc_settings()
         self._update_gap_settings()
@@ -52,163 +54,198 @@
     def _update_db_settings(self):
         """
         Update the database settings of self using the default settings templates
         and the 'db_user' and 'db_passw' envrionment variables if available.
         :return: No return
         :rtype: No return
         """
-        logger.debug('Updating Database settings.')
-        f = open(os.path.join(Settings._settings_files_path,
-                              "server_login.json"))
+        logger.debug("Updating Database settings.")
+        f = open(os.path.join(Settings._settings_files_path, "server_login.json"))
         login_data = json.load(f)
         f.close()
 
-        self.db['db_host'] = login_data['host']
+        self.db["db_host"] = login_data["host"]
 
         # self.db_host = Settings.db_host
-        self.db['db_database'] = login_data['database']
-        self.db['db_obs_table'] = login_data['obs_table']
-        self.db['db_meta_table'] = login_data['meta_table']
+        self.db["db_database"] = login_data["database"]
+        self.db["db_obs_table"] = login_data["obs_table"]
+        self.db["db_meta_table"] = login_data["meta_table"]
 
-        self.db['db_user'] = os.getenv('VLINDER_DB_USER_NAME')
-        self.db['db_passw'] = os.getenv('VLINDER_DB_USER_PASW')
+        self.db["db_user"] = os.getenv("VLINDER_DB_USER_NAME")
+        self.db["db_passw"] = os.getenv("VLINDER_DB_USER_PASW")
 
         # import db templates
-        from .data_templates.db_templates import vlinder_metadata_db_template, vlinder_observations_db_template
-        self.db['vlinder_db_meta_template'] = vlinder_metadata_db_template
-        self.db['vlinder_db_obs_template'] = vlinder_observations_db_template
+        from .data_templates.db_templates import (
+            vlinder_metadata_db_template,
+            vlinder_observations_db_template,
+        )
+
+        self.db["vlinder_db_meta_template"] = vlinder_metadata_db_template
+        self.db["vlinder_db_obs_template"] = vlinder_observations_db_template
 
     def _update_time_res_settings(self):
         """
         Update settings on time resolutions of self using the default settings templates.
 
         :return: No return
         :rtype: No return
         """
-        logger.debug('Updating time resolution settings.')
-        f = open(os.path.join(Settings._settings_files_path,
-                 "dataset_resolution_settings.json"))
+        logger.debug("Updating time resolution settings.")
+        f = open(
+            os.path.join(
+                Settings._settings_files_path, "dataset_resolution_settings.json"
+            )
+        )
         res_settings = json.load(f)
         f.close()
 
-        self.time_settings['target_time_res'] = res_settings['target_time_resolution']
-        self.time_settings['resample_method'] = res_settings['method']
-        self.time_settings['resample_limit'] = res_settings['limit']
-        self.time_settings['timezone'] = res_settings['timezone']
+        self.time_settings["target_time_res"] = res_settings["target_time_resolution"]
+        self.time_settings["resample_method"] = res_settings["method"]
+        self.time_settings["resample_limit"] = res_settings["limit"]
+        self.time_settings["timezone"] = res_settings["timezone"]
+
+        # Freq estimation
+        self.time_settings['freq_estimation_method'] = res_settings["freq_estimation_method"]
+        self.time_settings['freq_estimation_simplify'] = bool(res_settings["freq_estimation_simplify"])
+        self.time_settings['freq_estimation_simplify_error'] = res_settings["freq_estimation_simplify_error"]
+
 
     def _update_app_settings(self):
         """
         Update prefered display, print, plot and staticinfo settings of self using the default settings templates.
         :return: No return
         :rtype: No return
         """
-        logger.debug('Updating app settings.')
-        from .settings_files.default_formats_settings import plot_settings, print_settings, vars_display, default_name
-        from .settings_files.default_formats_settings import static_fields, categorical_fields, observation_types, location_info
+        logger.debug("Updating app settings.")
+        from .settings_files.default_formats_settings import (
+            plot_settings,
+            print_settings,
+            vars_display,
+            default_name,
+        )
+        from .settings_files.default_formats_settings import (
+            static_fields,
+            categorical_fields,
+            location_info,
+        )
 
         # 1. Print settings
-        self.app['print_fmt_datetime'] = print_settings['fmt_datetime']
-        self.app['print_max_n'] = int(print_settings["max_print_per_line"])
+        self.app["print_fmt_datetime"] = print_settings["fmt_datetime"]
+        self.app["print_max_n"] = int(print_settings["max_print_per_line"])
         # 2. Plot settings
-        self.app['plot_settings'] = plot_settings
-        self.app['world_boundary_map'] = os.path.join(Settings._settings_files_path,
-                                                      "world_boundaries",
-                                                      "WB_countries_Admin0_10m.shp")
+        self.app["plot_settings"] = plot_settings
+        self.app["world_boundary_map"] = os.path.join(
+            Settings._settings_files_path,
+            "world_boundaries",
+            "WB_countries_Admin0_10m.shp",
+        )
 
         # 3. display name mappers
-        self.app['display_name_mapper'] = vars_display
+        self.app["display_name_mapper"] = vars_display
 
         # 4 Fields settings
         # fields without timeevolution
-        self.app['static_fields'] = static_fields
-        self.app['categorical_fields'] = categorical_fields  # wind and lcz
-        # order of all possible observations
-        self.app['observation_types'] = observation_types
-        self.app['location_info'] = location_info  # all possible metadata
+        self.app["static_fields"] = static_fields
+        self.app["categorical_fields"] = categorical_fields  # wind and lcz
+        self.app["location_info"] = location_info  # all possible metadata
 
-        #5. default name (when station name is not present in dataset)
-        self.app['default_name'] = default_name
+        # 5. default name (when station name is not present in dataset)
+        self.app["default_name"] = default_name
 
     def _update_qc_settings(self):
         """
         Update quality control settings of self using the default settings templates.
         :return: No return
         :rtype: No return
         """
-        logger.debug('Updating QC settings.')
+        logger.debug("Updating QC settings.")
         from .settings_files.qc_settings import check_settings, checks_info
-        self.qc['qc_check_settings'] = check_settings
-        self.qc['qc_checks_info'] = checks_info
+
+        self.qc["qc_check_settings"] = check_settings
+        self.qc["qc_checks_info"] = checks_info
 
     def _update_gap_settings(self):
         """
         Update gap defenition and fill settings of self using the default settings templates.
         :return: No return
         :rtype: No return
         """
-        logger.debug('Updating gap settings.')
-        from .settings_files.gaps_settings import (gaps_settings, gaps_info,
-                                                   gaps_fill_settings,
-                                                   gaps_fill_info)
-
-        self.gap['gaps_settings'] = gaps_settings
-        self.gap['gaps_info'] = gaps_info
-        self.gap['gaps_fill_settings'] = gaps_fill_settings
-        self.gap['gaps_fill_info'] = gaps_fill_info
+        logger.debug("Updating gap settings.")
+        from .settings_files.gaps_and_missing_settings import (
+            gaps_settings,
+            gaps_info,
+            gaps_fill_settings,
+            gaps_fill_info,
+            missing_obs_fill_settings,
+            missing_obs_fill_info
+        )
+
+        self.gap["gaps_settings"] = gaps_settings
+        self.gap["gaps_info"] = gaps_info
+        self.gap["gaps_fill_settings"] = gaps_fill_settings
+        self.gap["gaps_fill_info"] = gaps_fill_info
+
+        self.missing_obs['missing_obs_fill_settings'] = missing_obs_fill_settings
+        self.missing_obs['missing_obs_fill_info'] = missing_obs_fill_info
 
     def _update_templates(self):
         """
         Import the default mapper-template, and assign it to be used on the
         observations and metadata.
         :return: No return
         :rtype: No return
 
         """
-        logger.debug('Updating data templates settings.')
+        logger.debug("Updating data templates settings.")
         from .data_templates.import_templates import default_template_file
 
         # Set default templates
-        self.templates['data_template_file'] = default_template_file
-        self.templates['metadata_template_file'] = default_template_file
+        self.templates["data_template_file"] = default_template_file
+        self.templates["metadata_template_file"] = default_template_file
 
     def _update_gee_settings(self):
         """
         Update the google earth enginge settings using the default settings templates.
         :return: No return
         :rtype: No return
         """
-        logger.debug('Updating gee settings.')
+        logger.debug("Updating gee settings.")
         from .settings_files.gee_settings import gee_datasets
 
-        self.gee['gee_dataset_info'] = gee_datasets
+        self.gee["gee_dataset_info"] = gee_datasets
 
     def update_timezone(self, timezonestr):
         """
         Change the timezone of the input data.
 
         :param timezonestr: Timezone string of the input observations.
         :type timezonestr: String
         :return: None
         :rtype: None
         """
         if not timezonestr in all_timezones:
             print(
-                f'timezone: {timezonestr}, is not a valid timezone. Select one of the following:')
-            print(f'{common_timezones}')
+                f"timezone: {timezonestr}, is not a valid timezone. Select one of the following:"
+            )
+            print(f"{common_timezones}")
             return
         else:
-
             print(
-                f'Update timezone: {self.time_settings["timezone"]} --> {timezonestr}')
-            self.time_settings['timezone'] = timezonestr
-
-
-    def update_IO(self, output_folder=None, input_data_file=None,
-                  input_metadata_file=None, data_template_file=None,
-                  metadata_template_file=None):
+                f'Update timezone: {self.time_settings["timezone"]} --> {timezonestr}'
+            )
+            self.time_settings["timezone"] = timezonestr
+
+    def update_IO(
+        self,
+        output_folder=None,
+        input_data_file=None,
+        input_metadata_file=None,
+        data_template_file=None,
+        metadata_template_file=None,
+    ):
         """
         Update some settings that are relevent before data is imported. The self
         object will be updated.
 
 
         :param output_folder: a directory to store the output to, defaults to None.
         :type output_folder: String, optional
@@ -222,70 +259,93 @@
         :param metadata_template_file: Path to the mapper-template csv file to be used on the metadata.
         If not given, the default template is used.
         :type metadata_template_file: String, optional
         :return: No return
         :rtype: No return
         """
 
-        logger.info('Updating settings with input: ')
+        logger.info("Updating settings with input: ")
 
         if not isinstance(output_folder, type(None)):
-            print('Update output_folder: ',
-                  self.IO['output_folder'], ' --> ', output_folder)
+            print(
+                "Update output_folder: ",
+                self.IO["output_folder"],
+                " --> ",
+                output_folder,
+            )
             logger.info(
-                f'Update output_folder:  {self.IO["output_folder"]}  -->  {output_folder}')
-            self.IO['output_folder'] = output_folder
+                f'Update output_folder:  {self.IO["output_folder"]}  -->  {output_folder}'
+            )
+            self.IO["output_folder"] = output_folder
 
         if not isinstance(input_data_file, type(None)):
-            print('Update input_data_file: ',
-                  self.IO['input_data_file'], ' --> ', input_data_file)
+            print(
+                "Update input_data_file: ",
+                self.IO["input_data_file"],
+                " --> ",
+                input_data_file,
+            )
             logger.info(
-                f'Update input_data_file:  {self.IO["input_data_file"]}  -->  {input_data_file}')
-            self.IO['input_data_file'] = input_data_file
+                f'Update input_data_file:  {self.IO["input_data_file"]}  -->  {input_data_file}'
+            )
+            self.IO["input_data_file"] = input_data_file
 
         if not isinstance(input_metadata_file, type(None)):
-            print('Update input_metadata_file: ',
-                  self.IO['input_metadata_file'], ' --> ', input_metadata_file)
+            print(
+                "Update input_metadata_file: ",
+                self.IO["input_metadata_file"],
+                " --> ",
+                input_metadata_file,
+            )
             logger.info(
-                f'Update meta_data_file:  {self.IO["input_metadata_file"]}  -->  {input_metadata_file}')
-            self.IO['input_metadata_file'] = input_metadata_file
+                f'Update meta_data_file:  {self.IO["input_metadata_file"]}  -->  {input_metadata_file}'
+            )
+            self.IO["input_metadata_file"] = input_metadata_file
 
         if not isinstance(data_template_file, type(None)):
-            print('Update data template file: ',
-                  self.templates['data_template_file'], ' --> ', data_template_file)
+            print(
+                "Update data template file: ",
+                self.templates["data_template_file"],
+                " --> ",
+                data_template_file,
+            )
             logger.info(
-                f'Update data template file:  {self.templates["data_template_file"]}  -->  {data_template_file}')
-            self.templates['data_template_file'] = data_template_file
+                f'Update data template file:  {self.templates["data_template_file"]}  -->  {data_template_file}'
+            )
+            self.templates["data_template_file"] = data_template_file
 
         if not isinstance(metadata_template_file, type(None)):
-            print('Update metadata template file: ',
-                  self.templates['metadata_template_file'], ' --> ', metadata_template_file)
+            print(
+                "Update metadata template file: ",
+                self.templates["metadata_template_file"],
+                " --> ",
+                metadata_template_file,
+            )
             logger.info(
-                f'Update metadata template file:  {self.templates["metadata_template_file"]}  -->  {metadata_template_file}')
-            self.templates['metadata_template_file'] = metadata_template_file
+                f'Update metadata template file:  {self.templates["metadata_template_file"]}  -->  {metadata_template_file}'
+            )
+            self.templates["metadata_template_file"] = metadata_template_file
 
     def copy_template_csv_files(self, target_folder):
         """
         A function to copy the default template file to an other location. This
         can be of use when creating a template file to start from the default.
 
         :param target_folder: Directory to copy the default template to (default_template.csv).
         :type target_folder: String
         :return: No return
         :rtype: No return
         """
 
-
-
         from .data_templates.import_templates import default_template_file
 
         # test if target_folder is a folder
-        assert os.path.isdir(target_folder), f'{target_folder} is not a folder'
+        assert os.path.isdir(target_folder), f"{target_folder} is not a folder"
 
-        target_file = os.path.join(target_folder, 'default_template.csv')
+        target_file = os.path.join(target_folder, "default_template.csv")
 
         shutil.copy2(default_template_file, target_file)
 
         print("Templates copied to : ", target_file)
 
     # =============================================================================
     #     Check settings
@@ -294,33 +354,43 @@
     def show(self):
         """
         A function that prints out all the settings, structured per thematic.
         :return: No return
         :rtype: No return
 
         """
-        logger.info('Show settings.')
-        class_vars_name = [attr for attr in dir(Settings) if not callable(
-            getattr(Settings, attr)) and not attr.startswith("__")]
-
-        attr_list = ['IO', 'db', 'time_settings',
-                     'app', 'qc', 'gap', 'templates', 'gee']
+        logger.info("Show settings.")
+        class_vars_name = [
+            attr
+            for attr in dir(Settings)
+            if not callable(getattr(Settings, attr)) and not attr.startswith("__")
+        ]
+
+        attr_list = [
+            "IO",
+            "db",
+            "time_settings",
+            "app",
+            "qc",
+            "gap",
+            "templates",
+            "gee",
+        ]
 
         # Drop variables starting with _
-        class_vars_name = [
-            mem for mem in class_vars_name if not mem.startswith('_')]
+        class_vars_name = [mem for mem in class_vars_name if not mem.startswith("_")]
         print("All settings:")
-        print(' \n ---------------------------------------\n')
+        print(" \n ---------------------------------------\n")
 
         for theme in attr_list:
-            print(f' ---------------- {theme} ----------------------\n')
+            print(f" ---------------- {theme} ----------------------\n")
             printdict = getattr(self, theme)
             for key1, item1 in printdict.items():
-                print(f'* {key1}: \n')
+                print(f"* {key1}: \n")
                 if isinstance(item1, type({})):
                     # nested dict level 1
                     for key2, item2 in item1.items():
-                        print(f'  - {key2}: \n')
-                        print(f'    -{item2} \n')
+                        print(f"  - {key2}: \n")
+                        print(f"    -{item2} \n")
                 else:
                     # not nested
-                    print(f'  -{item1} \n')
+                    print(f"  -{item1} \n")
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/gaps_settings.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/gaps_and_missing_settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,61 +5,68 @@
 
 @author: thoverga
 """
 
 from numpy import nan
 
 gaps_settings = {
-    "gaps_finder": {'gapsize_n': 40}, #gaps defined as n times the highest frequency on IO.
-
-
-
-
-    }
+    "gaps_finder": {
+        "gapsize_n": 40
+    },  # gaps defined as n times the highest frequency on IO.
+}
 
 gaps_info = {
-    'gap':{'label_columnname': 'is_gap',
-           'outlier_flag': 'gap',
-           'negative_flag': 'no gap',
-           'numeric_flag': 12,
-           'apply_on': 'record'
-           },
-    'missing_timestamp':{'label_columnname': 'is_missing_timestamp',
-                         'outlier_flag': 'missing timestamp',
-                         'negative flag': 'not missing',
-                         'numeric_flag': 13,
-                         'apply_on': 'record'
-                         },
-
-    }
+    "gap": {
+        "label_columnname": "is_gap",
+        "outlier_flag": "gap",
+        "negative_flag": "no gap",
+        "numeric_flag": 12,
+        "apply_on": "record",
+    },
+    "missing_timestamp": {
+        "label_columnname": "is_missing_timestamp",
+        "outlier_flag": "missing timestamp",
+        "negative flag": "not missing",
+        "numeric_flag": 13,
+        "apply_on": "record",
+    },
+}
 
 
 # =============================================================================
 #  Gap filling settings
 # =============================================================================
 
 
-gaps_fill_settings={
-    'linear': {'method': 'time',
-               'max_consec_fill': 100},
-
-    'model_debias':{
-        'debias_period': {'prefered_leading_sample_duration_hours': 48,
-                          'prefered_trailing_sample_duration_hours': 48,
-                          'minimum_leading_sample_duration_hours': 24,
-                          'minimum_trailing_sample_duration_hours': 24}
-
+gaps_fill_settings = {
+    "linear": {"method": "time", "max_consec_fill": 100},
+    "model_debias": {
+        "debias_period": {
+            "prefered_leading_sample_duration_hours": 48,
+            "prefered_trailing_sample_duration_hours": 48,
+            "minimum_leading_sample_duration_hours": 24,
+            "minimum_trailing_sample_duration_hours": 24,
         }
-
-
-    }
+    },
+}
 
 
 gaps_fill_info = {
+    "label_columnname": "final_label",
+    "label": {"linear": "gap_interpolation", "model_debias": "gap_debiased_era5"},
+    "numeric_flag": 21,
+}
+
+# =============================================================================
+#  Missing obs filling settings
+# =============================================================================
+missing_obs_fill_settings={
+    'linear': {'method': 'time'}
 
-    'label_columnname': 'fill_method',
-    'label': {'linear': 'interpolation',
-              'model_debias': 'debiased_era5'},
-     'numeric_flag': 21,
+}
 
-    }
+missing_obs_fill_info = {
+    "label_columnname": "final_label",
+    "label": {"linear": "missing_obs_interpolation"},
+    "numeric_flag": 23,
 
+}
```

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp` & `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx` & `metobs_toolkit-0.0.2a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.0.2a1/metobs_toolkit/writing_files.py` & `metobs_toolkit-0.0.2a2/metobs_toolkit/writing_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,81 +5,74 @@
 
 @author: thoverga
 """
 # --
 import os
 
 
-def write_dataset_to_csv(df,  metadf, filename, outputfolder, location_info,
-                         observation_types):
+def write_dataset_to_csv(
+    df, metadf, filename, outputfolder, location_info, observation_types
+):
     """
-        Write the dataset to a file where the observations, metadata and (if available)
-        the quality labels per observation type are merged together.
+    Write the dataset to a file where the observations, metadata and (if available)
+    the quality labels per observation type are merged together.
 
-        A final qualty controll label for each quality-controlled-observation type
-        can be added in the outputfile.
+    A final qualty controll label for each quality-controlled-observation type
+    can be added in the outputfile.
 
-        The file will be writen to the Settings.outputfolder.
+    The file will be writen to the Settings.outputfolder.
 
-        Parameters
-        ----------
-        df: pandas.DataFrame
-            The merged dataframe containing observations, gaps, outliers and missing timestamps.
-        metadf: pandas.DataFrame
-            The Dataset.metadf attribute.
-        filename : string, optional
-            The name of the output csv file. If none, a standard-filename is generated
-            based on the period of data. The default is None.
-
-
-        Returns
-        -------
-        None
-
-        """
+    Parameters
+    ----------
+    df: pandas.DataFrame
+        The merged dataframe containing observations, gaps, outliers and missing timestamps.
+    metadf: pandas.DataFrame
+        The Dataset.metadf attribute.
+    filename : string, optional
+        The name of the output csv file. If none, a standard-filename is generated
+        based on the period of data. The default is None.
+
+
+    Returns
+    -------
+    None
 
+    """
 
-    #make column ordering 'datetime', 'name', obs, QC, Qc final metadata
-    write_cols = ['datetime', 'name']
+    # make column ordering 'datetime', 'name', obs, QC, Qc final metadata
+    write_cols = ["datetime", "name"]
     write_cols.extend([col for col in df.columns if col in observation_types])
-    write_cols.extend([col for col in df.columns if col.endswith('_label')])
-    write_cols.extend(location_info) #metadata
+    write_cols.extend([col for col in df.columns if col.endswith("_label")])
+    write_cols.extend(location_info)  # metadata
 
     df = df.reset_index()
 
-    #merge metadata
-    df = df.merge(metadf, how='left', left_on='name',
-                  right_index=True)
+    # merge metadata
+    df = df.merge(metadf, how="left", left_on="name", right_index=True)
 
-    #subset and order columns
+    # subset and order columns
     df = df[write_cols]
 
-
-
-    #find observation type that are not present
+    # find observation type that are not present
     ignore_obstypes = [col for col in observation_types if df[col].isnull().all()]
     df = df.drop(columns=ignore_obstypes)
 
-    #find metadata that are not present
+    # find metadata that are not present
     ignore_metadat = [col for col in location_info if df[col].isnull().all()]
     df = df.drop(columns=ignore_metadat)
 
+    df = df.sort_values(["name", "datetime"])
 
-    df = df.sort_values(['name', 'datetime'])
-
-    #make filename
+    # make filename
     if isinstance(filename, type(None)):
-        startstr = df['datetime'].min().strftime('%Y%m%d')
-        endstr = df['datetime'].max().strftime('%Y%m%d')
-        filename= 'dataset_' + startstr + '_' + endstr
+        startstr = df["datetime"].min().strftime("%Y%m%d")
+        endstr = df["datetime"].max().strftime("%Y%m%d")
+        filename = "dataset_" + startstr + "_" + endstr
     else:
-        if filename.endswith('.csv'):
-            filename = filename[:-4] #to avoid two times .csv.csv
+        if filename.endswith(".csv"):
+            filename = filename[:-4]  # to avoid two times .csv.csv
 
-    filepath = os.path.join(outputfolder, filename + '.csv')
+    filepath = os.path.join(outputfolder, filename + ".csv")
 
-    #write to csv in output folder
-    print(f'write dataset to file: {filepath}')
-    df.to_csv(path_or_buf=filepath,
-                   sep=';',
-                   na_rep='NaN',
-                   index=False)
+    # write to csv in output folder
+    print(f"write dataset to file: {filepath}")
+    df.to_csv(path_or_buf=filepath, sep=";", na_rep="NaN", index=False)
```

### Comparing `metobs_toolkit-0.0.2a1/pyproject.toml` & `metobs_toolkit-0.0.2a2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MetObs-toolkit"
-version = "0.0.2a1"
+version = "0.0.2a2"
 description = "A Meteorological observations toolkit for scientists"
 authors = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 maintainers = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 license = "LICENSE"
 readme = "README.md"
 documentation = "https://python-poetry.org/docs/"
 packages = [{include = "metobs_toolkit"}]
@@ -19,13 +19,14 @@
 geopandas = "^0.9.0"
 pyproj = "~3.4"
 #rasterstats = "^0.16.0"
 mapclassify = "^2.4.0"
 earthengine-api = "^0.1.340"
 
 
+
 [tool.poetry.group.dev.dependencies]
 poetry = "^1.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `metobs_toolkit-0.0.2a1/PKG-INFO` & `metobs_toolkit-0.0.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metobs-toolkit
-Version: 0.0.2a1
+Version: 0.0.2a2
 Summary: A Meteorological observations toolkit for scientists
 License: LICENSE
 Keywords: meteorology,observations,urban climate
 Author: Thomas Vergauwen
 Author-email: thomas.vergauwen@meteo.be
 Maintainer: Thomas Vergauwen
 Maintainer-email: thomas.vergauwen@meteo.be
```

