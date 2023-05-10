# Comparing `tmp/PyBerries-0.2.7.tar.gz` & `tmp/PyBerries-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBerries-0.2.7.tar", last modified: Fri May  5 15:52:40 2023, max compression
+gzip compressed data, was "PyBerries-0.2.8.tar", last modified: Wed May 10 09:43:04 2023, max compression
```

## Comparing `PyBerries-0.2.7.tar` & `PyBerries-0.2.8.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.351626 PyBerries-0.2.7/
--rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.7/LICENSE
--rw-rw-rw-   0        0        0    13971 2023-05-05 15:52:40.351626 PyBerries-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.319625 PyBerries-0.2.7/PyBerries.egg-info/
--rw-rw-rw-   0        0        0    13971 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13653 2023-05-05 12:20:59.000000 PyBerries-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.323625 PyBerries-0.2.7/pyberries/
--rw-rw-rw-   0        0        0      118 2023-05-04 14:10:33.000000 PyBerries-0.2.7/pyberries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.331703 PyBerries-0.2.7/pyberries/data/
--rw-rw-rw-   0        0        0    16106 2023-05-05 15:50:23.000000 PyBerries-0.2.7/pyberries/data/DatasetPool.py
--rw-rw-rw-   0        0        0     1886 2023-05-04 10:56:45.000000 PyBerries-0.2.7/pyberries/data/Fitting.py
--rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.7/pyberries/data/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.7/pyberries/data/util.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.335624 PyBerries-0.2.7/pyberries/file_utilities/
--rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.7/pyberries/file_utilities/Filename_utils.py
--rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.7/pyberries/file_utilities/Stack_tiffs.py
--rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.7/pyberries/file_utilities/Unpack_omero_folders.py
--rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.7/pyberries/file_utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.339626 PyBerries-0.2.7/pyberries/metrics/
--rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.7/pyberries/metrics/Metrics.py
--rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.7/pyberries/metrics/Time_metrics.py
--rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.7/pyberries/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.347625 PyBerries-0.2.7/pyberries/plots/
--rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.7/pyberries/plots/Fits.py
--rw-rw-rw-   0        0        0     4813 2023-05-04 10:28:45.000000 PyBerries-0.2.7/pyberries/plots/Plot_presets.py
--rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.7/pyberries/plots/Plot_utilities.py
--rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.7/pyberries/plots/Plots.py
--rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.7/pyberries/plots/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-05 15:52:40.351626 PyBerries-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      690 2023-05-05 15:51:17.000000 PyBerries-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:04.716822 PyBerries-0.2.8/
+-rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0    13971 2023-05-10 09:43:04.716822 PyBerries-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:04.678941 PyBerries-0.2.8/PyBerries.egg-info/
+-rw-rw-rw-   0        0        0    13971 2023-05-10 09:43:04.000000 PyBerries-0.2.8/PyBerries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-05-10 09:43:04.000000 PyBerries-0.2.8/PyBerries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:43:04.000000 PyBerries-0.2.8/PyBerries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-05-10 09:43:04.000000 PyBerries-0.2.8/PyBerries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 09:43:04.000000 PyBerries-0.2.8/PyBerries.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13653 2023-05-05 12:20:59.000000 PyBerries-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:04.682942 PyBerries-0.2.8/pyberries/
+-rw-rw-rw-   0        0        0      118 2023-05-04 14:10:33.000000 PyBerries-0.2.8/pyberries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:04.692804 PyBerries-0.2.8/pyberries/data/
+-rw-rw-rw-   0        0        0    15384 2023-05-10 08:44:01.000000 PyBerries-0.2.8/pyberries/data/DatasetPool.py
+-rw-rw-rw-   0        0        0     3083 2023-05-08 13:08:41.000000 PyBerries-0.2.8/pyberries/data/Fitting.py
+-rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.8/pyberries/data/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.8/pyberries/data/util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:04.700820 PyBerries-0.2.8/pyberries/file_utilities/
+-rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.8/pyberries/file_utilities/Filename_utils.py
+-rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.8/pyberries/file_utilities/Stack_tiffs.py
+-rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.8/pyberries/file_utilities/Unpack_omero_folders.py
+-rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.8/pyberries/file_utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:04.704820 PyBerries-0.2.8/pyberries/metrics/
+-rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.8/pyberries/metrics/Metrics.py
+-rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.8/pyberries/metrics/Time_metrics.py
+-rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.8/pyberries/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:43:04.712825 PyBerries-0.2.8/pyberries/plots/
+-rw-rw-rw-   0        0        0     5459 2023-05-10 09:21:07.000000 PyBerries-0.2.8/pyberries/plots/Plot_presets.py
+-rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.8/pyberries/plots/Plot_utilities.py
+-rw-rw-rw-   0        0        0     1463 2023-05-10 08:28:13.000000 PyBerries-0.2.8/pyberries/plots/Plots.py
+-rw-rw-rw-   0        0        0       96 2023-05-08 14:30:38.000000 PyBerries-0.2.8/pyberries/plots/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:43:04.716822 PyBerries-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-05-10 09:30:22.000000 PyBerries-0.2.8/setup.py
```

### Comparing `PyBerries-0.2.7/LICENSE` & `PyBerries-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.7/PKG-INFO` & `PyBerries-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.7
+Version: 0.2.8
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PyBerries-0.2.7/PyBerries.egg-info/PKG-INFO` & `PyBerries-0.2.8/PyBerries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.7
+Version: 0.2.8
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PyBerries-0.2.7/PyBerries.egg-info/SOURCES.txt` & `PyBerries-0.2.8/PyBerries.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,12 +14,11 @@
 pyberries/file_utilities/Filename_utils.py
 pyberries/file_utilities/Stack_tiffs.py
 pyberries/file_utilities/Unpack_omero_folders.py
 pyberries/file_utilities/__init__.py
 pyberries/metrics/Metrics.py
 pyberries/metrics/Time_metrics.py
 pyberries/metrics/__init__.py
-pyberries/plots/Fits.py
 pyberries/plots/Plot_presets.py
 pyberries/plots/Plot_utilities.py
 pyberries/plots/Plots.py
 pyberries/plots/__init__.py
```

### Comparing `PyBerries-0.2.7/README.md` & `PyBerries-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.7/pyberries/data/DatasetPool.py` & `PyBerries-0.2.8/pyberries/data/DatasetPool.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from os import listdir
 from os.path import join, exists
 import json
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
-import h5py
 from IPython.display import display
 from warnings import warn
 from .util import dict_val_to_list, arg_to_list, set_to_several_objects
 import pyberries as pyb
 
 class DatasetPool():
     
@@ -21,20 +20,24 @@
                  metadata={},
                  filters={},
                  preprocessing={}
                  ):
         
         path = arg_to_list(path)
         dsList = arg_to_list(dsList)
+        preprocessing = dict_val_to_list(preprocessing)
+
+        # One item per dataset
         self.path = path
         self.dsList = dsList
+
+        # One item per Bacmman object
         self.table = dict()
         self.parent = dict()
         self.channel = dict()
-        preprocessing = dict_val_to_list(preprocessing)
 
         for i, ds in enumerate(dsList):
             ds_path = path[0] if len(path) == 1 else path[i]
             assert exists(ds_path), f'Bacmman folder not found: {ds_path}'
             assert exists(join(ds_path, ds)), f'Dataset {ds} not found.\nMaybe looking for {" or ".join([x for x in listdir(ds_path) if x.startswith(ds[0:6])])}?'
             assert (len(groups) >= len(dsList)) or not groups, 'If groups are provided, one group should be defined per dataset'
 
@@ -106,27 +109,25 @@
                 display(df_out)
     
     def add_metadata(self, metadata):
         metadata = set_to_several_objects(metadata, self.objects)
         metadata = dict_val_to_list(metadata)
         for obj in metadata.keys():
             if not self.table[obj].empty:
-                # channel = self.channel[obj]
-                channel = 0 # Other channels often miss metadata information so maybe better to always use this one?
                 df = self.table[obj]
                 for var in metadata[obj]:
                     df[var.replace(' ', '_')] = 0
                     if var == 'DateTime':
                         df['TimeDelta'] = 0
                         df['Time_min'] = 0
                     for i, ds in enumerate(self.dsList):
                         ds_path = self.path[0] if len(self.path) == 1 else self.path[i]
                         for pos in df.loc[df['Dataset'] == ds].Position.unique():
-                            # Open metadata file
-                            with open(join(ds_path, ds, 'SourceImageMetadata', f'{pos}_c{channel}.txt')) as f:
+                            metadata_filename = f'{pos}_c0.txt' if exists(join(ds_path, ds, 'SourceImageMetadata', f'{pos}_c0.txt')) else f'{pos}_c0_t0.txt'
+                            with open(join(ds_path, ds, 'SourceImageMetadata', metadata_filename)) as f:
                                 value = next((line for line in f if var in line), None)
                                 # Add metadata value to the current dataset and position
                                 df.loc[(df['Position'] == pos) & (df['Dataset'] == ds), var.replace(' ', '_')] = value.split('=')[-1][:-1] # Remove line break (last character)
                         if 'DateTime' in df.columns:
                             df.loc[df['Dataset'] == ds] = (df.loc[df['Dataset'] == ds]
                                                             .assign(DateTime = lambda df: pd.to_datetime(df.DateTime, format='%Y%m%d %H:%M:%S.%f'),
                                                                     TimeDelta = lambda df: df.DateTime - df.DateTime.iloc[0],
@@ -199,32 +200,14 @@
     
     def propagate_filters(self, parent:str, child:str):
         self.get_parent_indices(obj=child)
         self.table[child] = (self.table[child]
                             .merge(self.table[parent][['Dataset', 'PositionIdx', 'Indices']], suffixes=(None, '_tmp'), left_on = ['Dataset', 'PositionIdx', 'ParentIndices'], right_on=['Dataset', 'PositionIdx', 'Indices'])
                             .transform(lambda df: df.loc[:, ~df.columns.str.contains('_tmp')])
                             )
-    
-    def add_background(self, object_name:str, h5filenames:list, selection_name:str='Viewfield', raw_keyword:str='raw', seg_keyword:str='cells'):
-        df = self.table[object_name]
-        for i, ds in enumerate(self.dsList):
-            ds_path = self.path[0] if len(self.path) == 1 else self.path[i]
-            h5filename = h5filenames[0] if len(h5filenames) == 1 else h5filenames[i]
-            h5file = join(ds_path, ds, h5filename)
-            assert exists(h5file), 'h5 file not found'
-            f = h5py.File(h5file, "r")
-            for p in df.loc[df['Dataset'] == ds].Position.unique():
-                # Get raw fluorescence image
-                raw = np.array(f[f'{selection_name}/{ds}/{p}/{raw_keyword}'])   
-                # Get segmentation mask for current image
-                cells_seg = np.array(f[f'{selection_name}/{ds}/{p}/{seg_keyword}'])
-                for im in range(raw.shape[0]):
-                    df.loc[(df.Dataset == ds) & (df.Position == p) & (df.Frame == im), ('Background')] = np.mean(raw[im, cells_seg[im,] == 0])
-            f.close()
-        self.table[object_name] = df
 
     def add_from_parent(self, object_name:str, col:list=[]):
         parent = self.parent[object_name]
         self.get_parent_indices(obj=object_name)
         df = self.table[object_name]
         for c in col:
             df = (df
@@ -266,14 +249,18 @@
         elif metric == 'Fluo_intensity':
             df_out = pyb.metrics.Fluo_intensity(df_in, **kwargs)
         else:
             ValueError(f'Metric "{metric}" not found')
         self.timeseries[object_name] = df_out
 
     def plot_preset(self, preset:str, object_name:str='', timeseries:bool=False, drop_duplicates_by=[], return_axes:bool=False, **kwargs):
+        hue = kwargs.get('hue','')
+        if isinstance(hue, list):
+            self.fuse_columns(obj=object_name, cols=hue, new='_'.join(hue))
+            kwargs['hue'] = '_'.join(hue)
         if object_name:
             df_in = self.timeseries[object_name] if timeseries else self.table[object_name]
             if drop_duplicates_by:
                 df_in = df_in.drop_duplicates(subset = drop_duplicates_by)
         _,ax = plt.subplots(dpi=130)
         if preset == 'histogram':
             ax = pyb.plots.plot_histogram(df_in, ax=ax, **kwargs)
@@ -289,22 +276,26 @@
             ax = pyb.plots.scatterplot(df_in, ax=ax, **kwargs)
         elif preset == 'datapoints_and_mean':
             ax = pyb.plots.plot_datapoints_and_mean(df_in, dsList=self.dsList, ax=ax, **kwargs)
         elif preset == 'heatmap':
             ax = pyb.plots.plot_heatmap(df_in, ax=ax, **kwargs)
         elif preset == 'timeseries':
             ax = pyb.plots.plot_timeseries(df_in, ax=ax, **kwargs)
+        elif preset == 'boxplot':
+            ax = pyb.plots.boxplot(df_in, ax=ax, **kwargs)
         elif preset == 'boxenplot':
             ax = pyb.plots.plot_boxenplot(df_in, ax=ax, **kwargs)
         elif preset == 'spot_tracks':
             lineage = kwargs.pop('lineage','')
             self.fuse_columns(obj=object_name, cols=['Idx','BacteriaLineage'], new='Track')
             if lineage:
                 df = df_in.copy().query('BacteriaLineage == @lineage')
             else:
                 df = df_in.copy()
             ax=pyb.plots.lineplot(df, hue='Track', sort=False, ax=ax, **kwargs)
         elif preset == 'rates_summary':
             ax = pyb.plots.plot_rates_summary(ax=ax, **kwargs)
+        elif preset == 'grey_lines_and_highlight':
+            ax = pyb.plots.plot_grey_lines_and_highlight(df_in, ax=ax, **kwargs)
         else:
             warn('Plot preset not found!')
         if return_axes: return ax
```

### Comparing `PyBerries-0.2.7/pyberries/data/Fitting.py` & `PyBerries-0.2.8/pyberries/data/Fitting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 import inspect
+from warnings import warn
 from scipy.optimize import curve_fit
 from .util import arg_to_list
 
 def get_model(model_type=''):
     if model_type == 'monoexp_decay':
         def model(x, a, b):
             return a*np.exp(-b*x, dtype='float64')
@@ -15,31 +16,48 @@
         def model(x, a, b, c):
             return a*np.exp(-b*x) + c
     return model
 
 def make_fit(df_in, x:str, y:str, model, groupby:str='Group', p0=None):
     fit_results = dict()
     for name, data in df_in.groupby(groupby, sort=False):
+        groupName = '-'.join(map(str, name)) if isinstance(name, tuple) else str(name)
         try:
             popt,_ = curve_fit(model, data[x], data[y], p0=p0)
-            fit_results[name] = popt
+            fit_results[groupName] = popt
         except:
             print(f'Fit for dataset {name} failed')
     return fit_results
 
-def get_rates(fit_results, model, dt=1):
+def get_rates(fit_results, model, model_type, dt=1):
     dt = arg_to_list(dt)
-    rates = pd.DataFrame(columns=['Group', 'Rate type', 'Rate', 'Population'])
-    i=0
-    for j, grp in enumerate(fit_results.keys()):
-        popt = fit_results[grp]
-        dt_grp = dt[j] if len(dt) > 1 else dt[0]
-        if len(inspect.getfullargspec(model).args) == 3:
-            rates.loc[i] = {'Group':grp, 'Rate type':1, 'Rate':popt[1]/dt_grp, 'Population':1}
-            i+=1
-        elif len(inspect.getfullargspec(model).args) == 5:
+    if model_type == 'monoexp_decay':
+        assert len(inspect.getfullargspec(model).args) == 3, 'Model does not match with model type'
+        rates = pd.DataFrame(columns=['Group', 'Rate'])
+        for j, grp in enumerate(fit_results.keys()):
+            popt = fit_results[grp]
+            dt_grp = dt[j] if len(dt) > 1 else dt[0]
+            rates.loc[j] = {'Group':grp, 'Rate':popt[1]/dt_grp}
+        rates = rates.astype({'Group':'category', 'Rate':'float64'})
+    elif model_type == 'biexp_decay':
+        assert len(inspect.getfullargspec(model).args) == 5, 'Model does not match with model type'
+        rates = pd.DataFrame(columns=['Group', 'Rate type', 'Rate', 'Population'])
+        i=0
+        for j, grp in enumerate(fit_results.keys()):
+            popt = fit_results[grp]
+            dt_grp = dt[j] if len(dt) > 1 else dt[0]
             rates.loc[i] = {'Group':grp, 'Rate type':'Fast', 'Rate':popt[1]/dt_grp, 'Population':popt[0]/(popt[0]+popt[2])}
             i+=1
             rates.loc[i] = {'Group':grp, 'Rate type':'Slow', 'Rate':popt[3]/dt_grp, 'Population':popt[2]/(popt[0]+popt[2])}
             i+=1
-    rates = rates.astype({'Group':'category', 'Rate type':'category', 'Rate':'float64', 'Population':'float64'})
+        rates = rates.astype({'Group':'category', 'Rate type':'category', 'Rate':'float64', 'Population':'float64'})
+    elif model_type == 'monoexp_decay_offset':
+        assert len(inspect.getfullargspec(model).args) == 4, 'Model does not match with model type'
+        rates = pd.DataFrame(columns=['Group', 'Amplitude', 'Rate', 'Offset'])
+        for j, grp in enumerate(fit_results.keys()):
+            popt = fit_results[grp]
+            dt_grp = dt[j] if len(dt) > 1 else dt[0]
+            rates.loc[j] = {'Group':grp, 'Amplitude':popt[0], 'Rate':popt[1]/dt_grp, 'Offset':popt[2]}
+        rates = rates.astype({'Group':'category', 'Amplitude':'float64', 'Rate':'float64', 'Offset':'float64'})
+    else:
+        warn(f'Model type "{model_type}" not found')
     return rates
```

### Comparing `PyBerries-0.2.7/pyberries/data/util.py` & `PyBerries-0.2.8/pyberries/data/util.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.7/pyberries/file_utilities/Filename_utils.py` & `PyBerries-0.2.8/pyberries/file_utilities/Filename_utils.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.7/pyberries/file_utilities/Stack_tiffs.py` & `PyBerries-0.2.8/pyberries/file_utilities/Stack_tiffs.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.7/pyberries/file_utilities/Unpack_omero_folders.py` & `PyBerries-0.2.8/pyberries/file_utilities/Unpack_omero_folders.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.7/pyberries/metrics/Metrics.py` & `PyBerries-0.2.8/pyberries/metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.7/pyberries/metrics/Time_metrics.py` & `PyBerries-0.2.8/pyberries/metrics/Time_metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.7/pyberries/plots/Plot_presets.py` & `PyBerries-0.2.8/pyberries/plots/Plot_presets.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,19 +73,31 @@
         fit_df = pd.concat([fit_df, df], axis=0)
     ax = pyb.plots.histplot(df_in, ax=ax, **kwargs)
     ax = sns.lineplot(data=fit_df, x='x', y='Fit', hue=groupby, legend=False, ax=ax, linestyle='dashed')
 
 def plot_line_fit(df_in, model, ax, fit_results:dict, **kwargs):
     groupby = kwargs.get('hue','Group')
     x = kwargs.get('x', 'Frame')
-    fit_df = pd.DataFrame(columns=['x','Fit',groupby])
+    fit_df = pd.DataFrame(columns=['x', 'Fit', groupby])
     for grp, data in df_in.groupby(groupby, sort=False):
-        x_model = np.linspace(data[x].iloc[0], data[x].iloc[-1], 300)
-        df = pd.DataFrame({'x':x_model, 'Fit':model(x_model, *fit_results[grp]), groupby:grp})
-        fit_df = pd.concat([fit_df, df], axis=0)
+        if grp in fit_results.keys():
+            x_model = np.linspace(data[x].iloc[0], data[x].iloc[-1], 300)
+            df = pd.DataFrame({'x':x_model, 'Fit':model(x_model, *fit_results[grp]), groupby:grp})
+            fit_df = pd.concat([fit_df, df], axis=0)
     ax = pyb.plots.lineplot(df_in, ax=ax, **kwargs)
     ax = sns.lineplot(data=fit_df, x='x', y='Fit', hue=groupby, hue_order=fit_df[groupby].unique(), legend=False, ax=ax, linestyle='dashed')
 
 def plot_rates_summary(rates, ax, **kwargs):
-    df = rates.astype({'Group':'category', 'Rate type':'category', 'Rate':'float64'})
-    ax = pyb.plots.stripplot(df, ax=ax, jitter=False, **kwargs)
-    sns.move_legend(ax, "upper left", bbox_to_anchor=(1, 1), labelspacing=1)
+    ax = pyb.plots.stripplot(rates, ax=ax, jitter=False, **kwargs)
+    sns.move_legend(ax, "upper left", bbox_to_anchor=(1, 1), labelspacing=1)
+
+def plot_grey_lines_and_highlight(df_in, ax, color='gray', estimator=None, alpha=0.4, highlight=None, **kwargs):
+    highlight_by_index = kwargs.pop('highlight_by_index', False)
+    units = kwargs.get('units')
+    ax = pyb.plots.lineplot(df_in, color=color, estimator=estimator, alpha=alpha, legend=False, ax=ax, **kwargs)
+    df = df_in.copy()
+    n_units = len(df[units].unique())
+    if highlight_by_index:
+        highlight = df[units].unique()[highlight]
+    df = df[df[units] == highlight]
+    print(f'Displaying unit {highlight} ({n_units} units available)')
+    ax = sns.lineplot(data=df, x=kwargs.get('x'), y=kwargs.get('y'), color='red', legend=False)
```

### Comparing `PyBerries-0.2.7/pyberries/plots/Plots.py` & `PyBerries-0.2.8/pyberries/plots/Plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,7 +43,12 @@
     return g
 
 @plot
 def boxenplot(df, **kwargs):
     g = sns.boxenplot(data=df, **kwargs)
     return g
 
+@plot
+def boxplot(df, **kwargs):
+    g = sns.boxplot(data=df, **kwargs)
+    return g
+
```

### Comparing `PyBerries-0.2.7/setup.py` & `PyBerries-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyBerries",
-    version="0.2.7",
+    version="0.2.8",
     author="Daniel Thedie",
     author_email="daniel.thedie@ed.ac.uk",
     description="Processing of Bacmman measurement tables",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/MEKlab/pyberries",
     packages=setuptools.find_packages(),
```

