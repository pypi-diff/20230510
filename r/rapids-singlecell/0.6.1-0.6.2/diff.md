# Comparing `tmp/rapids_singlecell-0.6.1.tar.gz` & `tmp/rapids_singlecell-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids_singlecell-0.6.1.tar", last modified: Tue Apr 18 15:37:06 2023, max compression
+gzip compressed data, was "rapids_singlecell-0.6.2.tar", last modified: Wed May 10 13:46:47 2023, max compression
```

## Comparing `rapids_singlecell-0.6.1.tar` & `rapids_singlecell-0.6.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1069 2023-04-18 15:29:50.416825 rapids_singlecell-0.6.1/LICENSE
--rw-r--r--   0        0        0     5989 2023-04-18 15:29:50.416825 rapids_singlecell-0.6.1/README.md
--rw-r--r--   0        0        0      903 2023-04-18 15:36:55.344433 rapids_singlecell-0.6.1/pyproject.toml
--rwxr-xr-x   0        0        0      132 2023-04-18 15:33:39.042766 rapids_singlecell-0.6.1/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0    13190 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0      348 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/__init__.py
--rw-r--r--   0        0        0    33809 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_hvg.py
--rw-r--r--   0        0        0     5655 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_normalize.py
--rw-r--r--   0        0        0     4042 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_pca.py
--rw-r--r--   0        0        0     2801 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_plotting.py
--rw-r--r--   0        0        0     4761 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_regress_out.py
--rw-r--r--   0        0        0     1418 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_scale.py
--rw-r--r--   0        0        0    20228 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_simple.py
--rw-r--r--   0        0        0      574 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_utils.py
--rw-r--r--   0        0        0       29 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       68 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4570 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6256 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0       27 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/gr.py
--rw-r--r--   0        0        0       91 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/pl.py
--rw-r--r--   0        0        0       31 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/pp.py
--rw-r--r--   0        0        0      339 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/__init__.py
--rw-r--r--   0        0        0     5734 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_clustering.py
--rw-r--r--   0        0        0     3515 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_diffmap.py
--rw-r--r--   0        0        0     4075 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_draw_graph.py
--rw-r--r--   0        0        0     5143 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_embedding_density.py
--rw-r--r--   0        0        0    12184 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
--rw-r--r--   0        0        0     1743 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
--rw-r--r--   0        0        0     4177 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_pca.py
--rw-r--r--   0        0        0     2467 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_pymde.py
--rw-r--r--   0        0        0     8052 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
--rw-r--r--   0        0        0     3238 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_tsne.py
--rw-r--r--   0        0        0       40 2023-04-18 15:29:50.580827 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/__init__.py
--rw-r--r--   0        0        0     5785 2023-04-18 15:32:56.994409 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_autocorr.py
--rw-r--r--   0        0        0     5955 2023-04-18 15:29:50.584827 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_gearysc.py
--rw-r--r--   0        0        0     5774 2023-04-18 15:29:50.584827 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_moransi.py
--rw-r--r--   0        0        0     3278 2023-04-18 15:29:50.584827 rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_utils.py
--rw-r--r--   0        0        0       26 2023-04-18 15:29:50.584827 rapids_singlecell-0.6.1/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rapids_singlecell-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-04 12:56:41.030096 rapids_singlecell-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5989 2023-05-10 12:07:48.871399 rapids_singlecell-0.6.2/README.md
+-rw-r--r--   0        0        0      998 2023-05-10 12:34:48.415020 rapids_singlecell-0.6.2/pyproject.toml
+-rwxr-xr-x   0        0        0      132 2023-05-04 09:38:07.620767 rapids_singlecell-0.6.2/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0    13251 2023-05-10 12:07:48.871399 rapids_singlecell-0.6.2/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-09 15:12:57.948246 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/__init__.py
+-rw-r--r--   0        0        0    36337 2023-05-10 12:07:48.871399 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_hvg.py
+-rw-r--r--   0        0        0    14370 2023-05-04 11:39:21.895902 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_normalize.py
+-rw-r--r--   0        0        0     3983 2023-05-04 09:38:07.656769 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_pca.py
+-rw-r--r--   0        0        0     2783 2023-05-04 09:38:07.648769 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_plotting.py
+-rw-r--r--   0        0        0     4823 2023-05-04 09:38:07.656769 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_regress_out.py
+-rw-r--r--   0        0        0     1420 2023-05-04 09:38:07.636768 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_scale.py
+-rw-r--r--   0        0        0    20357 2023-05-10 12:07:48.871399 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_simple.py
+-rw-r--r--   0        0        0      683 2023-05-04 10:15:08.196605 rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_utils.py
+-rw-r--r--   0        0        0       29 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       68 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4609 2023-05-04 09:38:07.676770 rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6349 2023-05-04 09:38:07.700771 rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0       27 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       91 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/pl.py
+-rw-r--r--   0        0        0       30 2023-05-04 09:38:07.620767 rapids_singlecell-0.6.2/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0      341 2023-05-04 09:38:07.624767 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5576 2023-05-04 09:38:07.656769 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_clustering.py
+-rw-r--r--   0        0        0     3422 2023-05-04 09:38:07.648769 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_diffmap.py
+-rw-r--r--   0        0        0     4040 2023-05-04 09:38:07.672770 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_draw_graph.py
+-rw-r--r--   0        0        0     5159 2023-05-04 09:38:07.652769 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_embedding_density.py
+-rw-r--r--   0        0        0    12177 2023-05-04 09:38:07.736773 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
+-rw-r--r--   0        0        0     1745 2023-05-04 09:38:07.624767 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
+-rw-r--r--   0        0        0     4136 2023-05-04 09:38:07.648769 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_pca.py
+-rw-r--r--   0        0        0     2425 2023-05-04 09:38:07.644768 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_pymde.py
+-rw-r--r--   0        0        0     7928 2023-05-04 09:38:07.696771 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3241 2023-05-04 09:38:07.640768 rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_tsne.py
+-rw-r--r--   0        0        0       68 2023-05-04 15:27:48.771998 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5885 2023-05-04 09:38:07.656769 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     6442 2023-05-04 12:11:53.259130 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0    28951 2023-05-10 13:36:21.450416 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_ligrec.py
+-rw-r--r--   0        0        0     6299 2023-05-04 12:11:49.495103 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     5829 2023-05-04 15:55:42.727381 rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0       26 2023-05-04 09:18:25.499970 rapids_singlecell-0.6.2/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     6796 1970-01-01 00:00:00.000000 rapids_singlecell-0.6.2/PKG-INFO
```

### Comparing `rapids_singlecell-0.6.1/LICENSE` & `rapids_singlecell-0.6.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2022 Severin Dicks
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rapids_singlecell-0.6.1/README.md` & `rapids_singlecell-0.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 This repository offers some tools to make analyses of single cell datasets faster by running them on the GPU. 
 The functions are analogous versions of functions that can be found within [scanpy](https://github.com/scverse/scanpy) from the Theis lab or functions from [rapids-single-cell-examples](https://github.com/clara-parabricks/rapids-single-cell-examples) created by the Nvidia RAPIDS team. Most functions are kept close to the original code to ensure compatibility. My aim with this repository was to use the speedup that GPU computing offers and combine it with the ease of use from scanpy.
 
 ## Installation
 ### Conda
 The easiest way to install *rapids-singlecell* is to use one of the *yaml* file provided in the [conda](https://github.com/Intron7/rapids_singlecell/tree/main/conda) folder. These *yaml* files install everything needed to run the example notbooks and get you started.
 ```
-conda env create -f conda/rsc_rapids_22.12.yml
+conda env create -f conda/rsc_rapids_23.04.yml
 # or
 mamba env create -f conda/rsc_rapids_23.02.yml
 ```
 ### PyPI
 As of version 0.4.0 *rapids-singlecell* is now on PyPI.
 ```
 pip install rapids-singlecell
```

### Comparing `rapids_singlecell-0.6.1/pyproject.toml` & `rapids_singlecell-0.6.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -27,12 +27,17 @@
     "matplotlib>=3.4",
     "seaborn",
     "tqdm",
     "statsmodels>=0.12.0",
 ]
 
 [project.optional-dependencies]
-rapids = ["cudf-cu11", "cuml-cu11", "cugraph-cu11"] 
+rapids = ["cudf-cu11", "cuml-cu11", "cugraph-cu11"]
 
 [project.urls]
 Documentation = "https://rapids-singlecell.readthedocs.io"
 Source = "https://github.com/Intron7/rapids_singlecell"
+
+[tool.black]
+line-length = 88
+target-version = ['py38']
+include = '^rapids_singlecell/.*\.py$'
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/cunnData/__init__.py` & `rapids_singlecell-0.6.2/rapids_singlecell/cunnData/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,187 +17,202 @@
 from cupyx.scipy.sparse import issparse as issparse_gpu
 
 
 class Layer_Mapping(dict):
     """
     Dictonary subclass for layers handeling in cunnData
     """
+
     def __init__(self, shape):
         super().__init__({})
         self.shape = shape
-    
-    def update_shape(self,shape):
+
+    def update_shape(self, shape):
         self.shape = shape
 
     def __setitem__(self, key, item):
         if self.shape == item.shape:
+            if issparse_gpu(item):
+                if item.nnz > 2**31 - 1:
+                    raise ValueError(
+                        "Cupy only supports Sparse Matrices with `.nnz`"
+                        "with less than 2**31-1 for the int32 indptr"
+                    )
             super().__setitem__(key, item)
         else:
             raise ValueError(f"Shape of {key} does not match :attr:`.X`")
 
+
 class obsm_Mapping(dict):
     """
     Dictonary subclass for obsm handeling in cunnData
     """
+
     def __init__(self, shape):
         super().__init__({})
         self.shape = shape
-    
-    def update_shape(self,shape):
+
+    def update_shape(self, shape):
         self.shape = shape
 
     def __setitem__(self, key, item):
         if self.shape == item.shape[0]:
             super().__setitem__(key, item)
         else:
             raise ValueError(f"Shape of {key} does not match :attr:`.n_obs`")
-            
+
+
 class varm_Mapping(dict):
     """
     Dictonary subclass for obsm handeling in cunnData
     """
+
     def __init__(self, shape):
         super().__init__({})
         self.shape = shape
-    
-    def update_shape(self,shape):
+
+    def update_shape(self, shape):
         self.shape = shape
 
     def __setitem__(self, key, item):
         if self.shape == item.shape[0]:
             super().__setitem__(key, item)
         else:
             raise ValueError(f"Shape of {key} does not match :attr:`.n_vars`")
 
 
-
-
 class cunnData:
     """
-    The cunnData objects can be used as an AnnData replacement for the inital preprocessing 
-    of single cell Datasets. It replaces some of the most common preprocessing steps within 
+    The cunnData objects can be used as an AnnData replacement for the inital preprocessing
+    of single cell Datasets. It replaces some of the most common preprocessing steps within
     scanpy for annData objects.
-    It can be initalized with a preexisting annData object or with a countmatrix and seperate 
-    Dataframes for var and obs. Index of var will be used as gene_names. Initalization with an 
+    It can be initalized with a preexisting annData object or with a countmatrix and seperate
+    Dataframes for var and obs. Index of var will be used as gene_names. Initalization with an
     AnnData object is advised.
     """
+
     def __init__(
         self,
         adata: Optional[AnnData] = None,
-        X: Optional[Union[np.ndarray,sparse.spmatrix, cp.ndarray, cpx.scipy.sparse.csr_matrix]] = None,
+        X: Optional[
+            Union[np.ndarray, sparse.spmatrix, cp.ndarray, cpx.scipy.sparse.csr_matrix]
+        ] = None,
         obs: Optional[pd.DataFrame] = None,
         var: Optional[pd.DataFrame] = None,
         uns: Optional[Mapping[str, Any]] = None,
         layers: Optional[Mapping[str, Any]] = None,
         obsm: Optional[Mapping[str, Any]] = None,
-        varm: Optional[Mapping[str, Any]] = None):
-            if adata:
-                if not issparse_cpu(adata.X):
-                    inter = sparse.csr_matrix(adata.X)
-                    self._X = cp.sparse.csr_matrix(inter, dtype=cp.float32)
-                    del inter
-                else:
-                    self._X = cp.sparse.csr_matrix(adata.X, dtype=cp.float32)
-                self._obs = adata.obs.copy()
-                self._var = adata.var.copy()
-                self._uns = adata.uns.copy()
-                self._layers = Layer_Mapping(self.shape)
-                self._obsm = obsm_Mapping(self.shape[0])
-                self._varm = varm_Mapping(self.shape[1])
-                self.raw = None
-                if adata.layers:
-                    for key, matrix in adata.layers.items():
-                        if not issparse_cpu(matrix):
-                            inter = sparse.csr_matrix(matrix)
-                            inter = cp.sparse.csr_matrix(inter, dtype=cp.float32)
-                            
-                        else:
-                            inter = cp.sparse.csr_matrix(matrix, dtype=cp.float32)
-                        self._layers[key] = inter.copy()
-                        del inter
-                if adata.obsm:
-                    for key, matrix in adata.obsm.items():
-                        self._obsm[key] = matrix.copy()
-                if adata.varm:
-                    for key, matrix in adata.varm.items():
-                        self._varm[key] = matrix.copy()
-                
+        varm: Optional[Mapping[str, Any]] = None,
+    ):
+        if adata:
+            if not issparse_cpu(adata.X):
+                inter = sparse.csr_matrix(adata.X)
+                self._X = cp.sparse.csr_matrix(inter, dtype=cp.float32)
+                del inter
             else:
-                if issparse_gpu(X):
-                    self._X = X      
-                elif isinstance(X,cp.ndarray):
-                    self._X  = X            
-                elif not issparse_cpu(X):
-                    inter = sparse.csr_matrix(X)
-                    self._X = cp.sparse.csr_matrix(inter, dtype=cp.float32)
-                    del inter
-                else:
-                    self._X = cp.sparse.csr_matrix(X, dtype=cp.float32)
+                self._X = cp.sparse.csr_matrix(adata.X, dtype=cp.float32)
+            self._obs = adata.obs.copy()
+            self._var = adata.var.copy()
+            self._uns = adata.uns.copy()
+            self._layers = Layer_Mapping(self.shape)
+            self._obsm = obsm_Mapping(self.shape[0])
+            self._varm = varm_Mapping(self.shape[1])
+            self.raw = None
+            if adata.layers:
+                for key, matrix in adata.layers.items():
+                    if not issparse_cpu(matrix):
+                        inter = sparse.csr_matrix(matrix)
+                        inter = cp.sparse.csr_matrix(inter, dtype=cp.float32)
+                    else:
+                        inter = cp.sparse.csr_matrix(matrix, dtype=cp.float32)
+                    self._layers[key] = inter
+            if adata.obsm:
+                for key, matrix in adata.obsm.items():
+                    self._obsm[key] = matrix.copy()
+            if adata.varm:
+                for key, matrix in adata.varm.items():
+                    self._varm[key] = matrix.copy()
+
+        else:
+            if issparse_gpu(X):
+                self._X = X
+            elif isinstance(X, cp.ndarray):
+                self._X = X
+            elif not issparse_cpu(X):
+                inter = sparse.csr_matrix(X)
+                self._X = cp.sparse.csr_matrix(inter, dtype=cp.float32)
+                del inter
+            else:
+                self._X = cp.sparse.csr_matrix(X, dtype=cp.float32)
+
+            self._obs = obs
+            self._var = var
+            if uns:
+                self._uns = uns
+            else:
+                self._uns = OrderedDict()
+            self._layers = Layer_Mapping(self.shape)
+            self._obsm = obsm_Mapping(self.shape[0])
+            self._varm = varm_Mapping(self.shape[1])
+            self.raw = None
+
+            if layers:
+                for key, matrix in layers.items():
+                    if issparse_gpu(matrix):
+                        inter = matrix
+                    elif isinstance(matrix, cp.ndarray):
+                        inter = matrix
+                    elif not issparse_cpu(X):
+                        inter = sparse.csr_matrix(matrix)
+                        inter = cp.sparse.csr_matrix(inter, dtype=cp.float32)
+                    else:
+                        inter = cp.sparse.csr_matrix(matrix, dtype=cp.float32)
+                    self.layers[key] = inter
+            if obsm:
+                for key, matrix in obsm.items():
+                    self.obsm[key] = matrix.copy()
+            if varm:
+                for key, matrix in adata.varm.items():
+                    self.varm[key] = matrix
+        if issparse_gpu(self._X):
+            if self._X.nnz > 2**31 - 1:
+                raise ValueError(
+                    "Cupy only supports Sparse Matrices with `.nnz` "
+                    "less than 2**31-1 due to the int32 limit on `indptr`."
+                )
 
-                self._obs = obs
-                self._var = var
-                if uns:
-                    self._uns = uns
-                else:
-                    self._uns = OrderedDict()
-                self._layers = Layer_Mapping(self.shape)
-                self._obsm = obsm_Mapping(self.shape[0])
-                self._varm = varm_Mapping(self.shape[1])
-                self.raw = None
-
-                if layers:
-                    for key, matrix in layers.items():
-                        if issparse_gpu(matrix):
-                            inter = matrix
-                        elif isinstance(matrix,cp.ndarray):
-                            inter = matrix               
-                        elif not issparse_cpu(X):
-                            inter = sparse.csr_matrix(matrix)
-                            inter = cp.sparse.csr_matrix(inter, dtype=cp.float32)
-                        else:
-                            inter = cp.sparse.csr_matrix(matrix, dtype=cp.float32)
-                        self.layers[key] = inter.copy()
-                        del inter
-                if obsm:
-                    for key, matrix in obsm.items():
-                        self.obsm[key] = matrix.copy()
-                if varm:
-                    for key, matrix in adata.varm.items():
-                        self.varm[key] = matrix
-    
-    
     @property
     def X(self):
         """Data matrix of shape :attr:`.n_obs` × :attr:`.n_vars`."""
-        return  self._X
+        return self._X
 
     @X.setter
     def X(self, value: Optional[Union[cp.ndarray, cpx.scipy.sparse.spmatrix]]):
         self._X = value
         self._update_shape()
 
-
     @property
     def obs(self):
-        """One-dimensional annotation of observations (`pd.DataFrame`)."""     
-        return  self._obs
+        """One-dimensional annotation of observations (`pd.DataFrame`)."""
+        return self._obs
 
     @obs.setter
     def obs(self, value: pd.DataFrame):
         if value.shape[0] == self.shape[0]:
             self._obs = value.copy()
         else:
             raise ValueError("dimension mismatch")
+
     @property
     def var(self):
         """One-dimensional annotation of variables/ features (`pd.DataFrame`)."""
         return self._var
 
     @var.setter
-    def var(self,value: pd.DataFrame):
+    def var(self, value: pd.DataFrame):
         if value.shape[0] == self.shape[1]:
             self._var = value
         else:
             raise ValueError("dimension mismatch")
 
     @property
     def uns(self):
@@ -206,15 +221,17 @@
 
     @uns.setter
     def uns(self, value: MutableMapping):
         if not isinstance(value, MutableMapping):
             raise ValueError(
                 "Only mutable mapping types (e.g. dict) are allowed for `.uns`."
             )
-        if isinstance(value, (anndata.compact.OverloadedDict, anndata._core.views.DictView)):
+        if isinstance(
+            value, (anndata.compact.OverloadedDict, anndata._core.views.DictView)
+        ):
             value = value.copy()
         self._uns = value
 
     @uns.deleter
     def uns(self):
         self.uns = OrderedDict()
 
@@ -230,58 +247,56 @@
             adata.layers["spliced"] = ...
         Assign the 10th column of layer `"spliced"` to the variable a::
             a = adata.layers["spliced"][:, 10]
         Delete the `"spliced"` layer::
             del adata.layers["spliced"]
         Return layers’ names::
             adata.layers.keys()
-        """  
-        return  self._layers
+        """
+        return self._layers
 
     @property
     def obsm(self):
         """\
         Multi-dimensional annotation of observations
         (mutable structured :class:`~numpy.ndarray`).
         Stores for each key a two or higher-dimensional :class:`~numpy.ndarray`
         of length :attr:`n_obs`.
         Is sliced with `data` and `obs` but behaves otherwise like a :term:`mapping`.
-        """      
-        return  self._obsm
-
+        """
+        return self._obsm
 
     @property
     def varm(self):
         """\
         Multi-dimensional annotation of variables/features
         (mutable structured :class:`~numpy.ndarray`).
         Stores for each key a two or higher-dimensional :class:`~numpy.ndarray`
         of length :attr:`n_vars`.
         Is sliced with `data` and `var` but behaves otherwise like a :term:`mapping`.
         """
-        return  self._varm
-    
+        return self._varm
 
     @property
     def obs_names(self):
-        """Names of observations (alias for `.obs.index`)."""        
-        return  self.obs.index
+        """Names of observations (alias for `.obs.index`)."""
+        return self.obs.index
 
     @property
     def var_names(self):
         """Names of variables (alias for `.var.index`)."""
         return self.var.index
-    
+
     @property
-    def n_obs(self)->int:
+    def n_obs(self) -> int:
         """Number of observations."""
         return self.shape[0]
 
     @property
-    def n_vars(self)->int:
+    def n_vars(self) -> int:
         """Number of variables/features."""
         return self.shape[1]
 
     @property
     def shape(self):
         """Shape of data matrix (:attr:`.n_obs`, :attr:`.n_vars`)."""
         return self.X.shape
@@ -289,20 +304,20 @@
     @property
     def nnz(self):
         """Get the count of explicitly-stored values (nonzeros) in :attr:`.X`"""
         if issparse_gpu(self.X):
             return self.X.nnz
         else:
             return None
-    
+
     def _update_shape(self):
         self.layers.update_shape(self.shape)
         self.obsm.update_shape(self.shape[0])
         self.varm.update_shape(self.shape[1])
-        
+
     def _sanitize(self):
         dfs = [self.obs, self.var]
         for df in dfs:
             string_cols = [
                 key for key in df.columns if infer_dtype(df[key]) == "string"
             ]
             for key in string_cols:
@@ -312,19 +327,21 @@
                 # Ideally this could be done inplace
                 sorted_categories = natsorted(c.categories)
                 if not np.array_equal(c.categories, sorted_categories):
                     c = c.reorder_categories(sorted_categories)
                 df[key] = c
 
     def __getitem__(self, index):
-        obs_dx,var_dx = _normalize_indices(index, self.obs_names, self.var_names)
-        cudata = cunnData(X =self.X[obs_dx,var_dx].copy(),
-                        obs = self.obs.iloc[obs_dx,:].copy(),
-                        var = self.var.iloc[var_dx,:].copy(),
-                        uns=self.uns)
+        obs_dx, var_dx = _normalize_indices(index, self.obs_names, self.var_names)
+        cudata = cunnData(
+            X=self.X[obs_dx, var_dx].copy(),
+            obs=self.obs.iloc[obs_dx, :].copy(),
+            var=self.var.iloc[var_dx, :].copy(),
+            uns=self.uns,
+        )
 
         if self.layers:
             for key, matrix in self.layers.items():
                 cudata.layers[key] = matrix[obs_dx, var_dx].copy()
         if self.obsm:
             for key, matrix in self.obsm.items():
                 if isinstance(matrix, pd.DataFrame):
@@ -333,16 +350,16 @@
                     cudata.obsm[key] = matrix[obs_dx, :].copy()
         if self.varm:
             for key, matrix in self.varm.items():
                 if isinstance(matrix, pd.DataFrame):
                     cudata.varm[key] = matrix.iloc[var_dx, :].copy()
                 else:
                     cudata.varm[key] = matrix[var_dx, :].copy()
-        return(cudata)
-    
+        return cudata
+
     def _gen_repr(self, n_obs, n_vars) -> str:
         descr = f"cunnData object with n_obs × n_vars = {n_obs} × {n_vars}"
         for attr in [
             "obs",
             "var",
             "uns",
             "obsm",
@@ -351,26 +368,25 @@
         ]:
             keys = getattr(self, attr).keys()
             if len(keys) > 0:
                 descr += f"\n    {attr}: {str(list(keys))[1:-1]}"
         return descr
 
     def __repr__(self) -> str:
-            return self._gen_repr(self.n_obs, self.n_vars)
-
+        return self._gen_repr(self.n_obs, self.n_vars)
 
     def to_AnnData(self):
         """
         Takes the cunnData object and creates an AnnData object
-        
+
         Returns
         -------
         :class:`~anndata.AnnData`
             Annotated data matrix.
-        
+
         """
         adata = AnnData(self.X.get())
         adata.obs = self.obs.copy()
         adata.var = self.var.copy()
         adata.uns = self.uns.copy()
         if self.layers:
             for key, matrix in self.layers.items():
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_hvg.py` & `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_hvg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import cupy as cp
 import cupyx as cpx
 import numpy as np
 import pandas as pd
+import math
 import warnings
 from typing import Optional
 
 from ..cunnData import cunnData
 from ._utils import _check_nonnegative_integers, _get_mean_var
 
+
 def highly_variable_genes(
-    cudata:cunnData,
+    cudata: cunnData,
     layer: str = None,
     min_mean: float = 0.0125,
-    max_mean: float=3,
-    min_disp:float= 0.5,
-    max_disp: float  =np.inf,
+    max_mean: float = 3,
+    min_disp: float = 0.5,
+    max_disp: float = np.inf,
     n_top_genes: int = None,
-    flavor: str = 'seurat',
+    flavor: str = "seurat",
     n_bins: int = 20,
     span: float = 0.3,
     check_values: bool = True,
-    theta:int = 100,
-    clip:bool = None,
-    chunksize:int = 1000,
-    n_samples:int = 10000, 
-    batch_key:str = None) -> None:
-
+    theta: int = 100,
+    clip: bool = None,
+    chunksize: int = 1000,
+    n_samples: int = 10000,
+    batch_key: str = None,
+) -> None:
     """\
     Annotate highly variable genes. 
     Expects logarithmized data, except when `flavor='seurat_v3','pearson_residuals','poisson_gene_selection'`, in which count data is expected.
     
     Reimplentation of scanpy's function. 
     Depending on flavor, this reproduces the R-implementations of Seurat, Cell Ranger, Seurat v3 and Pearson Residuals.
     Flavor `poisson_gene_selection` is an implementation of scvi, which is based on M3Drop. It requiers gpu accelerated pytorch to be installed.
@@ -75,17 +77,16 @@
             The negative binomial overdispersion parameter `theta` for Pearson residuals. 
             Higher values correspond to less overdispersion (`var = mean + mean^2/theta`), and `theta=np.Inf` corresponds to a Poisson model.
         clip
             Only used if `flavor='pearson_residuals'`. Determines if and how residuals are clipped:
                 * If `None`, residuals are clipped to the interval `[-sqrt(n_obs), sqrt(n_obs)]`, where `n_obs` is the number of cells in the dataset (default behavior).
                 * If any scalar `c`, residuals are clipped to the interval `[-c, c]`. Set `clip=np.Inf` for no clipping.
         chunksize
-            If `flavor='pearson_residuals'` or `'poisson_gene_selection'`, this dertermines how many genes are processed at
-            once while computing the residual variance. Choosing a smaller value will reduce
-            the required memory.
+            If `'poisson_gene_selection'`, this dertermines how many genes are processed at
+            once. Choosing a smaller value will reduce the required memory.
         n_samples
             The number of Binomial samples to use to estimate posterior probability
             of enrichment of zeros for each gene (only for `flavor='poisson_gene_selection'`).
         batch_key
             If specified, highly-variable genes are selected within each batch separately and merged.
             
     Returns
@@ -112,234 +113,257 @@
                 For `flavor='seurat_v3','pearson_residuals'`, rank of the gene according to normalized
                 variance, median rank in the case of multiple batches
             `highly_variable_nbatches` : int
                 If batch_key is given, this denotes in how many batches genes are detected as HVG
             `highly_variable_intersection` : bool
                 If batch_key is given, this denotes the genes that are highly variable in all batches
     """
-    if flavor == 'seurat_v3':
+    if flavor == "seurat_v3":
         _highly_variable_genes_seurat_v3(
-            cudata = cudata,
+            cudata=cudata,
             layer=layer,
             n_top_genes=n_top_genes,
             batch_key=batch_key,
             span=span,
-            check_values = check_values,
+            check_values=check_values,
         )
-    elif flavor == 'pearson_residuals':
+    elif flavor == "pearson_residuals":
         _highly_variable_pearson_residuals(
-            cudata = cudata,
-            theta= theta,
-            clip = clip,
+            cudata=cudata,
+            theta=theta,
+            clip=clip,
             n_top_genes=n_top_genes,
             batch_key=batch_key,
-            check_values = check_values,
+            check_values=check_values,
             layer=layer,
-            chunksize= chunksize)
-    elif flavor == 'poisson_gene_selection':
+        )
+    elif flavor == "poisson_gene_selection":
         _poisson_gene_selection(
-            cudata =cudata,
+            cudata=cudata,
             n_top_genes=n_top_genes,
             batch_key=batch_key,
-            check_values = check_values,
+            check_values=check_values,
             layer=layer,
-            n_samples = n_samples,
-            minibatch_size= chunksize)
+            n_samples=n_samples,
+            minibatch_size=chunksize,
+        )
     else:
         if batch_key is None:
             X = cudata.layers[layer] if layer is not None else cudata.X
             df = _highly_variable_genes_single_batch(
                 X.copy(),
                 min_disp=min_disp,
                 max_disp=max_disp,
                 min_mean=min_mean,
                 max_mean=max_mean,
                 n_top_genes=n_top_genes,
                 n_bins=n_bins,
-                flavor=flavor)
+                flavor=flavor,
+            )
         else:
             cudata.obs[batch_key] = cudata.obs[batch_key].astype("category")
             batches = cudata.obs[batch_key].cat.categories
             df = []
             genes = cudata.var.index.to_numpy()
             for batch in batches:
-                inter_matrix = cudata.X[np.where(cudata.obs[batch_key]==batch)[0],].tocsc()
+                inter_matrix = cudata.X[
+                    np.where(cudata.obs[batch_key] == batch)[0],
+                ].tocsc()
                 thr_org = cp.diff(inter_matrix.indptr).ravel()
                 thr = cp.where(thr_org >= 1)[0]
                 thr_2 = cp.where(thr_org < 1)[0]
                 inter_matrix = inter_matrix[:, thr].tocsr()
                 thr = thr.get()
                 thr_2 = thr_2.get()
                 inter_genes = genes[thr]
                 other_gens_inter = genes[thr_2]
-                hvg_inter = _highly_variable_genes_single_batch(inter_matrix,
-                                                                min_disp=min_disp,
-                                                                max_disp=max_disp,
-                                                                min_mean=min_mean,
-                                                                max_mean=max_mean,
-                                                                n_top_genes=n_top_genes,
-                                                                n_bins=n_bins,
-                                                                flavor=flavor)
+                hvg_inter = _highly_variable_genes_single_batch(
+                    inter_matrix,
+                    min_disp=min_disp,
+                    max_disp=max_disp,
+                    min_mean=min_mean,
+                    max_mean=max_mean,
+                    n_top_genes=n_top_genes,
+                    n_bins=n_bins,
+                    flavor=flavor,
+                )
                 hvg_inter["gene"] = inter_genes
                 missing_hvg = pd.DataFrame(
                     np.zeros((len(other_gens_inter), len(hvg_inter.columns))),
                     columns=hvg_inter.columns,
                 )
-                missing_hvg['highly_variable'] = missing_hvg['highly_variable'].astype(bool)
-                missing_hvg['gene'] = other_gens_inter
-                #hvg = hvg_inter.append(missing_hvg, ignore_index=True)
-                hvg = pd.concat([hvg_inter,missing_hvg], ignore_index=True)
+                missing_hvg["highly_variable"] = missing_hvg["highly_variable"].astype(
+                    bool
+                )
+                missing_hvg["gene"] = other_gens_inter
+                # hvg = hvg_inter.append(missing_hvg, ignore_index=True)
+                hvg = pd.concat([hvg_inter, missing_hvg], ignore_index=True)
                 idxs = np.concatenate((thr, thr_2))
                 hvg = hvg.loc[np.argsort(idxs)]
                 df.append(hvg)
-            
+
             df = pd.concat(df, axis=0)
-            df['highly_variable'] = df['highly_variable'].astype(int)
-            df = df.groupby('gene').agg(
+            df["highly_variable"] = df["highly_variable"].astype(int)
+            df = df.groupby("gene").agg(
                 dict(
                     means=np.nanmean,
                     dispersions=np.nanmean,
                     dispersions_norm=np.nanmean,
                     highly_variable=np.nansum,
                 )
             )
             df.rename(
-                columns=dict(highly_variable='highly_variable_nbatches'), inplace=True
+                columns=dict(highly_variable="highly_variable_nbatches"), inplace=True
             )
-            df['highly_variable_intersection'] = df['highly_variable_nbatches'] == len(
+            df["highly_variable_intersection"] = df["highly_variable_nbatches"] == len(
                 batches
             )
             if n_top_genes is not None:
                 # sort genes by how often they selected as hvg within each batch and
                 # break ties with normalized dispersion across batches
-                df=df.sort_values(
-                    ['highly_variable_nbatches', 'dispersions_norm'],
+                df = df.sort_values(
+                    ["highly_variable_nbatches", "dispersions_norm"],
                     ascending=False,
-                    na_position='last'
+                    na_position="last",
                 )
-                
+
                 high_var = np.zeros(df.shape[0])
                 high_var[:n_top_genes] = True
-                df['highly_variable'] = high_var.astype(bool)
+                df["highly_variable"] = high_var.astype(bool)
                 df = df.loc[genes]
             else:
                 df = df.loc[genes]
                 dispersion_norm = df.dispersions_norm.values
                 dispersion_norm[np.isnan(dispersion_norm)] = 0  # similar to Seurat
                 gene_subset = np.logical_and.reduce(
                     (
                         df.means > min_mean,
                         df.means < max_mean,
                         df.dispersions_norm > min_disp,
                         df.dispersions_norm < max_disp,
                     )
                 )
-                df['highly_variable'] = gene_subset
-        
-        cudata.var["highly_variable"] =df['highly_variable'].values
-        cudata.var["means"] = df['means'].values
-        cudata.var["dispersions"]=df['dispersions'].values
-        cudata.var["dispersions_norm"]=df['dispersions_norm'].values
-        cudata.uns['hvg'] = {'flavor': flavor}
+                df["highly_variable"] = gene_subset
+
+        cudata.var["highly_variable"] = df["highly_variable"].values
+        cudata.var["means"] = df["means"].values
+        cudata.var["dispersions"] = df["dispersions"].values
+        cudata.var["dispersions_norm"] = df["dispersions_norm"].values
+        cudata.uns["hvg"] = {"flavor": flavor}
         if batch_key is not None:
-            cudata.var['highly_variable_nbatches'] = df[
-                'highly_variable_nbatches'
+            cudata.var["highly_variable_nbatches"] = df[
+                "highly_variable_nbatches"
             ].values
-            cudata.var['highly_variable_intersection'] = df[
-                'highly_variable_intersection'
+            cudata.var["highly_variable_intersection"] = df[
+                "highly_variable_intersection"
             ].values
 
-def _highly_variable_genes_single_batch(X,min_mean = 0.0125,max_mean =3,min_disp= 0.5,max_disp =np.inf, n_top_genes = None, flavor = 'seurat', n_bins = 20):
-        """\
+
+def _highly_variable_genes_single_batch(
+    X,
+    min_mean=0.0125,
+    max_mean=3,
+    min_disp=0.5,
+    max_disp=np.inf,
+    n_top_genes=None,
+    flavor="seurat",
+    n_bins=20,
+):
+    """\
         See `highly_variable_genes`.
         Returns
         -------
         A DataFrame that contains the columns
         `highly_variable`, `means`, `dispersions`, and `dispersions_norm`.
         """
-        if flavor == 'seurat':
-            X = X.expm1()
-        mean, var = _get_mean_var(X)
-        mean[mean == 0] = 1e-12
-        disp = var/mean
-        if flavor == 'seurat':  # logarithmized mean as in Seurat
-            disp[disp == 0] = np.nan
-            disp = cp.log(disp)
-            mean = cp.log1p(mean)
-        df = pd.DataFrame()
-        mean = mean.get()
-        disp = disp.get()
-        df['means'] = mean
-        df['dispersions'] = disp
-        if flavor == 'seurat':
-            df['mean_bin'] = pd.cut(df['means'], bins=n_bins)
-            disp_grouped = df.groupby('mean_bin')['dispersions']
-            disp_mean_bin = disp_grouped.mean()
-            disp_std_bin = disp_grouped.std(ddof=1)
-            # retrieve those genes that have nan std, these are the ones where
-            # only a single gene fell in the bin and implicitly set them to have
-            # a normalized disperion of 1
-            one_gene_per_bin = disp_std_bin.isnull()
-            gen_indices = np.where(one_gene_per_bin[df['mean_bin'].values])[0].tolist()
-
-            # Circumvent pandas 0.23 bug. Both sides of the assignment have dtype==float32,
-            # but there’s still a dtype error without “.value”.
-            disp_std_bin[one_gene_per_bin.values] = disp_mean_bin[
-                one_gene_per_bin.values
-            ].values
-            disp_mean_bin[one_gene_per_bin.values] = 0
-            # actually do the normalization
-            df['dispersions_norm'] = (
-                df['dispersions'].values  # use values here as index differs
-                - disp_mean_bin[df['mean_bin'].values].values
-            ) / disp_std_bin[df['mean_bin'].values].values
-
-        elif flavor == 'cell_ranger':
-            from statsmodels import robust
-            df['mean_bin'] = pd.cut(
-                    df['means'],
-                    np.r_[-np.inf, np.percentile(df['means'], np.arange(10, 105, 5)), np.inf],
-                )
-            disp_grouped = df.groupby('mean_bin')['dispersions']
-            disp_median_bin = disp_grouped.median()
-            with warnings.catch_warnings():
-                    warnings.simplefilter('ignore')
-                    disp_mad_bin = disp_grouped.apply(robust.mad)
-                    df['dispersions_norm'] = (
-                        df['dispersions'].values - disp_median_bin[df['mean_bin'].values].values
-                    ) / disp_mad_bin[df['mean_bin'].values].values
-
-        dispersion_norm = df['dispersions_norm'].values
-        if n_top_genes is not None:
-            dispersion_norm = dispersion_norm[~np.isnan(dispersion_norm)]
-            dispersion_norm[::-1].sort()# interestingly, np.argpartition is slightly slower
-            if n_top_genes > X.shape[1]:
-                n_top_genes = X.shape[1]
-            disp_cut_off = dispersion_norm[n_top_genes - 1]
-            gene_subset = np.nan_to_num(df['dispersions_norm'].values) >= disp_cut_off
-        else:
-            dispersion_norm[np.isnan(dispersion_norm)] = 0  # similar to Seurat
-            gene_subset = np.logical_and.reduce(
-                (
-                    mean > min_mean,
-                    mean < max_mean,
-                    dispersion_norm > min_disp,
-                    dispersion_norm < max_disp,
-                )
+    if flavor == "seurat":
+        X = X.expm1()
+    mean, var = _get_mean_var(X)
+    mean[mean == 0] = 1e-12
+    disp = var / mean
+    if flavor == "seurat":  # logarithmized mean as in Seurat
+        disp[disp == 0] = np.nan
+        disp = cp.log(disp)
+        mean = cp.log1p(mean)
+    df = pd.DataFrame()
+    mean = mean.get()
+    disp = disp.get()
+    df["means"] = mean
+    df["dispersions"] = disp
+    if flavor == "seurat":
+        df["mean_bin"] = pd.cut(df["means"], bins=n_bins)
+        disp_grouped = df.groupby("mean_bin")["dispersions"]
+        disp_mean_bin = disp_grouped.mean()
+        disp_std_bin = disp_grouped.std(ddof=1)
+        # retrieve those genes that have nan std, these are the ones where
+        # only a single gene fell in the bin and implicitly set them to have
+        # a normalized disperion of 1
+        one_gene_per_bin = disp_std_bin.isnull()
+        gen_indices = np.where(one_gene_per_bin[df["mean_bin"].values])[0].tolist()
+
+        # Circumvent pandas 0.23 bug. Both sides of the assignment have dtype==float32,
+        # but there’s still a dtype error without “.value”.
+        disp_std_bin[one_gene_per_bin.values] = disp_mean_bin[
+            one_gene_per_bin.values
+        ].values
+        disp_mean_bin[one_gene_per_bin.values] = 0
+        # actually do the normalization
+        df["dispersions_norm"] = (
+            df["dispersions"].values  # use values here as index differs
+            - disp_mean_bin[df["mean_bin"].values].values
+        ) / disp_std_bin[df["mean_bin"].values].values
+
+    elif flavor == "cell_ranger":
+        from statsmodels import robust
+
+        df["mean_bin"] = pd.cut(
+            df["means"],
+            np.r_[-np.inf, np.percentile(df["means"], np.arange(10, 105, 5)), np.inf],
+        )
+        disp_grouped = df.groupby("mean_bin")["dispersions"]
+        disp_median_bin = disp_grouped.median()
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            disp_mad_bin = disp_grouped.apply(robust.mad)
+            df["dispersions_norm"] = (
+                df["dispersions"].values - disp_median_bin[df["mean_bin"].values].values
+            ) / disp_mad_bin[df["mean_bin"].values].values
+
+    dispersion_norm = df["dispersions_norm"].values
+    if n_top_genes is not None:
+        dispersion_norm = dispersion_norm[~np.isnan(dispersion_norm)]
+        dispersion_norm[
+            ::-1
+        ].sort()  # interestingly, np.argpartition is slightly slower
+        if n_top_genes > X.shape[1]:
+            n_top_genes = X.shape[1]
+        disp_cut_off = dispersion_norm[n_top_genes - 1]
+        gene_subset = np.nan_to_num(df["dispersions_norm"].values) >= disp_cut_off
+    else:
+        dispersion_norm[np.isnan(dispersion_norm)] = 0  # similar to Seurat
+        gene_subset = np.logical_and.reduce(
+            (
+                mean > min_mean,
+                mean < max_mean,
+                dispersion_norm > min_disp,
+                dispersion_norm < max_disp,
             )
-        df['highly_variable'] = gene_subset
-        return df
+        )
+    df["highly_variable"] = gene_subset
+    return df
+
 
 def _highly_variable_genes_seurat_v3(
     cudata: cunnData,
     layer: Optional[str] = None,
     n_top_genes: int = None,
     batch_key: Optional[str] = None,
     span: float = 0.3,
-    check_values = True):
+    check_values=True,
+):
     """\
     See `highly_variable_genes`.
     For further implementation details see https://www.overleaf.com/read/ckptrbgzzzpg
     Returns
     -------
     updates `.var` with the following fields:
     highly_variable : bool
@@ -361,27 +385,27 @@
             "`flavor='seurat_v3'` expects `n_top_genes`  to be defined, defaulting to 2000 HVGs",
             UserWarning,
         )
     try:
         from skmisc.loess import loess
     except ImportError:
         raise ImportError(
-            'Please install skmisc package via `pip install --user scikit-misc'
+            "Please install skmisc package via `pip install --user scikit-misc"
         )
 
     df = pd.DataFrame(index=cudata.var.index)
     X = cudata.layers[layer] if layer is not None else cudata.X
     if check_values and not _check_nonnegative_integers(X):
         warnings.warn(
             "`flavor='seurat_v3'` expects raw count data, but non-integers were found.",
             UserWarning,
         )
 
     mean, var = _get_mean_var(X)
-    df['means'], df['variances'] = mean.get(), var.get()
+    df["means"], df["variances"] = mean.get(), var.get()
     if batch_key is None:
         batch_info = pd.Categorical(np.zeros(cudata.shape[0], dtype=int))
     else:
         batch_info = cudata.obs[batch_key].values
 
     norm_gene_vars = []
     for b in np.unique(batch_info):
@@ -419,48 +443,48 @@
     num_batches_high_var = cp.sum(
         (ranked_norm_gene_vars < n_top_genes).astype(int), axis=0
     )
     ranked_norm_gene_vars[ranked_norm_gene_vars >= n_top_genes] = np.nan
     ranked_norm_gene_vars = ranked_norm_gene_vars.get()
     ma_ranked = np.ma.masked_invalid(ranked_norm_gene_vars)
     median_ranked = np.ma.median(ma_ranked, axis=0).filled(np.nan)
-    df['highly_variable_nbatches'] = num_batches_high_var.get()
-    df['highly_variable_rank'] = median_ranked
-    df['variances_norm'] = cp.mean(norm_gene_vars, axis=0).get()
+    df["highly_variable_nbatches"] = num_batches_high_var.get()
+    df["highly_variable_rank"] = median_ranked
+    df["variances_norm"] = cp.mean(norm_gene_vars, axis=0).get()
     sorted_index = (
-        df[['highly_variable_rank', 'highly_variable_nbatches']]
+        df[["highly_variable_rank", "highly_variable_nbatches"]]
         .sort_values(
-            ['highly_variable_rank', 'highly_variable_nbatches'],
+            ["highly_variable_rank", "highly_variable_nbatches"],
             ascending=[True, False],
-            na_position='last',
+            na_position="last",
         )
         .index
     )
-    df['highly_variable'] = False
-    df.loc[sorted_index[: int(n_top_genes)], 'highly_variable'] = True
-    cudata.var['highly_variable'] = df['highly_variable'].values
-    cudata.var['highly_variable_rank'] = df['highly_variable_rank'].values
-    cudata.var['means'] = df['means'].values
-    cudata.var['variances'] = df['variances'].values
-    cudata.var['variances_norm'] = df['variances_norm'].values.astype(
-            'float64', copy=False
-        )
-    cudata.var['highly_variable_nbatches'] = df[
-                'highly_variable_nbatches'
-            ].values
-    cudata.uns['hvg'] = {'flavor': 'seurat_v3'}
+    df["highly_variable"] = False
+    df.loc[sorted_index[: int(n_top_genes)], "highly_variable"] = True
+    cudata.var["highly_variable"] = df["highly_variable"].values
+    cudata.var["highly_variable_rank"] = df["highly_variable_rank"].values
+    cudata.var["means"] = df["means"].values
+    cudata.var["variances"] = df["variances"].values
+    cudata.var["variances_norm"] = df["variances_norm"].values.astype(
+        "float64", copy=False
+    )
+    cudata.var["highly_variable_nbatches"] = df["highly_variable_nbatches"].values
+    cudata.uns["hvg"] = {"flavor": "seurat_v3"}
 
-def _highly_variable_pearson_residuals(cudata: cunnData,
+
+def _highly_variable_pearson_residuals(
+    cudata: cunnData,
     theta: float = 100,
     clip: Optional[float] = None,
     n_top_genes: int = 2000,
     batch_key: Optional[str] = None,
     check_values: bool = True,
     layer: Optional[str] = None,
-    chunksize= 1000):
+):
     """
     Select highly variable genes using analytic Pearson residuals.
     Pearson residuals of a negative binomial offset model are computed
     (with overdispersion `theta` shared across genes). By default, overdispersion
     `theta=100` is used and residuals are clipped to `sqrt(n_obs)`. Finally, genes
     are ranked by residual variance.
     Expects raw count input.
@@ -474,62 +498,160 @@
     if n_top_genes is None:
         n_top_genes = 2000
         warnings.warn(
             "`flavor='pearson_residuals'` expects `n_top_genes`  to be defined, defaulting to 2000 HVGs",
             UserWarning,
         )
     if theta <= 0:
-        raise ValueError('Pearson residuals require theta > 0')
+        raise ValueError("Pearson residuals require theta > 0")
     if batch_key is None:
         batch_info = pd.Categorical(np.zeros(cudata.shape[0], dtype=int))
     else:
         batch_info = cudata.obs[batch_key].values
-        
+
     n_batches = len(np.unique(batch_info))
     residual_gene_vars = []
+    sparse_kernel = cp.RawKernel(
+        r"""
+    extern "C" __global__
+    void calculate_sum_cg(const int *indptr,const int *index,const float *data, 
+                                        float* sums_genes, float* sums_cells,
+                                        int n_genes) {
+        int gene = blockDim.x * blockIdx.x + threadIdx.x;
+        if(gene >= n_genes){
+            return;
+        }
+        int start_idx = indptr[gene];
+        int stop_idx = indptr[gene+1];
+
+        for(int cell = start_idx; cell < stop_idx; cell++){
+            float value = data[cell];
+            int cell_number = index[cell];
+            atomicAdd(&sums_genes[gene], value);
+            atomicAdd(&sums_cells[cell_number], value);
+
+        }
+    }
+    """,
+        "calculate_sum_cg",
+    )
+    sparse_kernel_res = cp.RawKernel(
+        r"""
+    extern "C" __global__
+    void calculate_res(const int *indptr,const int *index,const float *data, 
+                            const float* sums_genes,const float* sums_cells,
+                            float* residuals ,float* sum_total,float* clip,float* theta,int n_genes, int n_cells) {
+        int gene = blockDim.x * blockIdx.x + threadIdx.x;
+        if(gene >= n_genes){
+            return;
+        }
+        int start_idx = indptr[gene];
+        int stop_idx = indptr[gene + 1];
+
+        int sparse_idx = start_idx;
+        float var_sum = 0.0;
+        float sum_clipped_res = 0.0;
+        for(int cell = 0; cell < n_cells; cell++){
+            float mu = sums_genes[gene]*sums_cells[cell]/sum_total[0];
+            float value = 0.0;
+            if (sparse_idx < stop_idx && index[sparse_idx] == cell){
+                value = data[sparse_idx];
+                sparse_idx++;
+            }
+            float mu_sum = value - mu;
+            float pre_res =  mu_sum / sqrt(mu + mu * mu / theta[0]);
+            float clipped_res = fminf(fmaxf(pre_res, -clip[0]), clip[0]);
+            sum_clipped_res += clipped_res;
+        }
+
+        float mean_clipped_res = sum_clipped_res / n_cells;
+        sparse_idx = start_idx;
+        for(int cell = 0; cell < n_cells; cell++){
+            float mu = sums_genes[gene]*sums_cells[cell]/sum_total[0];
+            float value = 0.0;
+            if (sparse_idx < stop_idx && index[sparse_idx] == cell){
+                value = data[sparse_idx];
+                sparse_idx++;
+            }
+            float mu_sum = value - mu;
+            float pre_res =  mu_sum / sqrt(mu + mu * mu / theta[0]);
+            float clipped_res = fminf(fmaxf(pre_res, -clip[0]), clip[0]);
+            float diff = clipped_res - mean_clipped_res;
+            var_sum += diff * diff;
+        }
+        residuals[gene] = var_sum / n_cells;
+    }
+
+    """,
+        "calculate_res",
+    )
+
     for b in np.unique(batch_info):
         X_batch = X[batch_info == b].tocsc()
         thr_org = cp.diff(X_batch.indptr).ravel()
         nonzero_genes = cp.array(thr_org >= 1)
         X_batch = X_batch[:, nonzero_genes]
         if clip is None:
             n = X_batch.shape[0]
-            clip = cp.sqrt(n)
+            clip = cp.sqrt(n, dtype=cp.float32)
         if clip < 0:
             raise ValueError("Pearson residuals require `clip>=0` or `clip=None`.")
-        sums_cells = X_batch.sum(axis=1)
-        X_batch =X_batch.tocsr()
-        sums_genes = X_batch.sum(axis=0)
+
+        theta = cp.array([theta], dtype=cp.float32)
+        sums_genes = cp.zeros(X_batch.shape[1], dtype=cp.float32)
+        sums_cells = cp.zeros(X_batch.shape[0], dtype=cp.float32)
+        block = (32,)
+        grid = (int(math.ceil(X_batch.shape[1] / block[0])),)
+        sparse_kernel(
+            grid,
+            block,
+            (
+                X_batch.indptr,
+                X_batch.indices,
+                X_batch.data,
+                sums_genes,
+                sums_cells,
+                X_batch.shape[1],
+            ),
+        )
         sum_total = sums_genes.sum().squeeze()
-        # Compute pearson residuals in chunks
-        residual_gene_var = cp.empty((X_batch.shape[1]))
-        X_batch = X_batch.tocsc()
-        for start in np.arange(0, X_batch.shape[1], chunksize):
-            stop = start + chunksize
-            mu = cp.array(sums_cells @ sums_genes[:, start:stop] / sum_total)
-            X_dense = X_batch[:, start:stop].toarray()
-            residuals = (X_dense - mu) / cp.sqrt(mu + mu**2 / theta)
-            residuals = cp.clip(residuals, a_min=-clip, a_max=clip)
-            residual_gene_var[start:stop] = cp.var(residuals, axis=0)
+        residual_gene_var = cp.zeros(X_batch.shape[1], dtype=cp.float32, order="C")
 
+        sparse_kernel_res(
+            grid,
+            block,
+            (
+                X_batch.indptr,
+                X_batch.indices,
+                X_batch.data,
+                sums_genes,
+                sums_cells,
+                residual_gene_var,
+                sum_total,
+                clip,
+                theta,
+                X_batch.shape[1],
+                X_batch.shape[0],
+            ),
+        )
         unmasked_residual_gene_var = cp.zeros(len(nonzero_genes))
         unmasked_residual_gene_var[nonzero_genes] = residual_gene_var
         residual_gene_vars.append(unmasked_residual_gene_var.reshape(1, -1))
-        
+
     residual_gene_vars = cp.concatenate(residual_gene_vars, axis=0)
     # Get rank per gene within each batch
     # argsort twice gives ranks, small rank means most variable
     ranks_residual_var = cp.argsort(cp.argsort(-residual_gene_vars, axis=1), axis=1)
     ranks_residual_var = ranks_residual_var.astype(np.float32)
     # count in how many batches a genes was among the n_top_genes
     highly_variable_nbatches = cp.sum(
         (ranks_residual_var < n_top_genes).astype(int), axis=0
     ).get()
     ranks_residual_var[ranks_residual_var >= n_top_genes] = np.nan
-    ranks_residual_var= ranks_residual_var.get()
+    ranks_residual_var = ranks_residual_var.get()
     ranks_masked_array = np.ma.masked_invalid(ranks_residual_var)
     # Median rank across batches, ignoring batches in which gene was not selected
     medianrank_residual_var = np.ma.median(ranks_masked_array, axis=0).filled(np.nan)
     means, variances = _get_mean_var(X)
     means, variances = means.get(), variances.get()
     df = pd.DataFrame.from_dict(
         dict(
@@ -539,47 +661,46 @@
             highly_variable_rank=medianrank_residual_var,
             highly_variable_nbatches=highly_variable_nbatches.astype(np.int64),
             highly_variable_intersection=highly_variable_nbatches == n_batches,
         )
     )
     df = df.set_index(cudata.var_names)
     df.sort_values(
-        ['highly_variable_nbatches', 'highly_variable_rank'],
+        ["highly_variable_nbatches", "highly_variable_rank"],
         ascending=[False, True],
-        na_position='last',
+        na_position="last",
         inplace=True,
     )
     high_var = np.zeros(df.shape[0], dtype=bool)
     high_var[:n_top_genes] = True
-    df['highly_variable'] = high_var
+    df["highly_variable"] = high_var
     df = df.loc[cudata.var_names, :]
-    
-    computed_on = layer if layer else 'adata.X'
-    cudata.uns['hvg'] = {'flavor': 'pearson_residuals', 'computed_on': computed_on}
-    cudata.var['means'] = df['means'].values
-    cudata.var['variances'] = df['variances'].values
-    cudata.var['residual_variances'] = df['residual_variances']
-    cudata.var['highly_variable_rank'] = df['highly_variable_rank'].values
+
+    computed_on = layer if layer else "adata.X"
+    cudata.uns["hvg"] = {"flavor": "pearson_residuals", "computed_on": computed_on}
+    cudata.var["means"] = df["means"].values
+    cudata.var["variances"] = df["variances"].values
+    cudata.var["residual_variances"] = df["residual_variances"]
+    cudata.var["highly_variable_rank"] = df["highly_variable_rank"].values
     if batch_key is not None:
-        cudata.var['highly_variable_nbatches'] = df[
-            'highly_variable_nbatches'
-        ].values
-        cudata.var['highly_variable_intersection'] = df[
-            'highly_variable_intersection'
+        cudata.var["highly_variable_nbatches"] = df["highly_variable_nbatches"].values
+        cudata.var["highly_variable_intersection"] = df[
+            "highly_variable_intersection"
         ].values
-    cudata.var['highly_variable'] = df['highly_variable'].values
+    cudata.var["highly_variable"] = df["highly_variable"].values
+
 
 def _poisson_gene_selection(
-    cudata:cunnData,
+    cudata: cunnData,
     layer: Optional[str] = None,
     n_top_genes: int = None,
     n_samples: int = 10000,
     batch_key: str = None,
     minibatch_size: int = 1000,
-    check_values:bool = True,
+    check_values: bool = True,
     **kwargs,
 ) -> None:
     """
     Rank and select genes based on the enrichment of zero counts.
     Enrichment is considered by comparing data to a Poisson count model.
     This is based on M3Drop: https://github.com/tallulandrews/M3Drop
     The method accounts for library size internally, a raw count matrix should be provided.
@@ -616,55 +737,56 @@
     prob_zero_enrichment : float
         Probability of zero enrichment, median across batches in the case of multiple batches
     prob_zero_enrichment_rank : float
         Rank of the gene according to probability of zero enrichment, median rank in the case of multiple batches
     prob_zero_enriched_nbatches : int
         If batch_key is given, this denotes in how many batches genes are detected as zero enriched
     """
-    
+
     try:
         import torch
     except ImportError:
-        raise ImportError(
-            'Please install pytorch package via `pip install pytorch'
-        )
+        raise ImportError("Please install pytorch package via `pip install pytorch")
     if n_top_genes is None:
         n_top_genes = 2000
         warnings.warn(
             "`flavor='seurat_v3'` expects `n_top_genes`  to be defined, defaulting to 2000 HVGs",
             UserWarning,
         )
-    
+
     X = cudata.layers[layer] if layer is not None else cudata.X
     if check_values and not _check_nonnegative_integers(X):
         warnings.warn(
             "`flavor='pearson_residuals'` expects raw count data, but non-integers were found.",
             UserWarning,
         )
     if batch_key is None:
         batch_info = pd.Categorical(np.zeros(cudata.shape[0], dtype=int))
     else:
         batch_info = cudata.obs[batch_key].values
 
     prob_zero_enrichments = []
     obs_frac_zeross = []
     exp_frac_zeross = []
-    
+
     with torch.no_grad():
         for b in np.unique(batch_info):
             X_batch = X[batch_info == b]
-            total_counts = torch.tensor(X_batch.sum(1).ravel(), device = "cuda")
+            total_counts = torch.tensor(X_batch.sum(1).ravel(), device="cuda")
             X_batch = X_batch.tocsc()
             # Calculate empirical statistics.
-            sum_0 = X_batch.sum(axis =0).ravel()
-            scaled_means = torch.tensor(sum_0 / sum_0.sum(), device = "cuda")
+            sum_0 = X_batch.sum(axis=0).ravel()
+            scaled_means = torch.tensor(sum_0 / sum_0.sum(), device="cuda")
 
             observed_fraction_zeros = torch.tensor(
-                cp.asarray(1.0 - cp.diff(X_batch.indptr).ravel() / X_batch.shape[0]).ravel(),
-                device = "cuda")
+                cp.asarray(
+                    1.0 - cp.diff(X_batch.indptr).ravel() / X_batch.shape[0]
+                ).ravel(),
+                device="cuda",
+            )
             # Calculate probability of zero for a Poisson model.
             # Perform in batches to save memory.
             minibatch_size = min(total_counts.shape[0], minibatch_size)
             n_batches = total_counts.shape[0] // minibatch_size
 
             expected_fraction_zeros = torch.zeros(scaled_means.shape, device="cuda")
 
@@ -683,21 +805,22 @@
             ).sum(1)
             expected_fraction_zeros /= X_batch.shape[0]
 
             # Compute probability of enriched zeros through sampling from Binomial distributions.
             observed_zero = torch.distributions.Binomial(probs=observed_fraction_zeros)
             expected_zero = torch.distributions.Binomial(probs=expected_fraction_zeros)
 
-            #extra_zeros = torch.zeros(expected_fraction_zeros.shape, device="cuda")
-            
-            
-            extra_zeros = observed_zero.sample((n_samples,))>expected_zero.sample((n_samples,))
-            #for i in range(n_samples):
+            # extra_zeros = torch.zeros(expected_fraction_zeros.shape, device="cuda")
+
+            extra_zeros = observed_zero.sample((n_samples,)) > expected_zero.sample(
+                (n_samples,)
+            )
+            # for i in range(n_samples):
             #    extra_zeros += observed_zero.sample() > expected_zero.sample()
-            
+
             extra_zeros = extra_zeros.sum(0)
             prob_zero_enrichment = (extra_zeros / n_samples).cpu().numpy()
 
             obs_frac_zeros = observed_fraction_zeros.cpu().numpy()
             exp_frac_zeros = expected_fraction_zeros.cpu().numpy()
 
             # Clean up memory (tensors seem to stay in GPU unless actively deleted).
@@ -741,15 +864,15 @@
     top_genes = df.nlargest(n_top_genes, sort_columns).index
     df.loc[top_genes, "highly_variable"] = True
 
     cudata.uns["hvg"] = {"flavor": "poisson_zeros"}
     cudata.var["highly_variable"] = df["highly_variable"].values
     cudata.var["observed_fraction_zeros"] = df["observed_fraction_zeros"].values
     cudata.var["expected_fraction_zeros"] = df["expected_fraction_zeros"].values
-    cudata.var["prob_zero_enriched_nbatches"] = df[
-        "prob_zero_enriched_nbatches"
-    ].values
+    cudata.var["prob_zero_enriched_nbatches"] = df["prob_zero_enriched_nbatches"].values
     cudata.var["prob_zero_enrichment"] = df["prob_zero_enrichment"].values
     cudata.var["prob_zero_enrichment_rank"] = df["prob_zero_enrichment_rank"].values
 
     if batch_key is not None:
-        cudata.var["prob_zero_enriched_nbatches"] = df["prob_zero_enriched_nbatches"].values
+        cudata.var["prob_zero_enriched_nbatches"] = df[
+            "prob_zero_enriched_nbatches"
+        ].values
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_pca.py` & `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_pca.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,111 +3,114 @@
 from cuml.decomposition import PCA, TruncatedSVD
 from typing import Optional
 
 from cupy.sparse import issparse
 import math
 import numpy as np
 
-def pca(cudata: cunnData, 
-        layer:str = None, 
-        n_comps:int = 50,
-        zero_center:bool = True,
-        use_highly_variable: Optional[bool] = None,
-        chunked:bool = False,
-        chunk_size:int = None)->None:
 
+def pca(
+    cudata: cunnData,
+    layer: str = None,
+    n_comps: int = 50,
+    zero_center: bool = True,
+    use_highly_variable: Optional[bool] = None,
+    chunked: bool = False,
+    chunk_size: int = None,
+) -> None:
     """
     Performs PCA using the cuML decomposition function for the :class:`~rapids_singlecell.cunnData.cunnData` object.
-    
+
     Parameters
     ----------
-        cudata : 
+        cudata :
             cunnData object
-        
+
         layer
             If provided, use `cudata.layers[layer]` for expression values instead of `cudata.X`.
 
         n_comps
             Number of principal components to compute. Defaults to 50
-        
+
         zero_center
             If `True`, compute standard PCA from covariance matrix.
             If `False`, omit zero-centering variables
-        
+
         use_highly_variable
             Whether to use highly variable genes only, stored in
             `.var['highly_variable']`.
             By default uses them if they have been determined beforehand.
-            
+
         chunked
             If `True`, perform an incremental PCA on segments of `chunk_size`.
             The incremental PCA automatically zero centers and ignores settings of
             `random_seed` and `svd_solver`. If `False`, perform a full PCA.
-            
+
         chunk_size
             Number of observations to include in each chunk.
             Required if `chunked=True` was passed.
-    
+
     Returns
     -------
         adds fields to `cudata` :
             `.obsm['X_pca']`
                 PCA representation of data.
             `.varm['PCs']`
                 The principal components containing the loadings.
             `.uns['pca']['variance_ratio']`
                 Ratio of explained variance.
             `.uns['pca']['variance']`
                 Explained variance, equivalent to the eigenvalues of the
                 covariance matrix.
     """
 
-    if use_highly_variable is True and 'highly_variable' not in cudata.var.keys():
+    if use_highly_variable is True and "highly_variable" not in cudata.var.keys():
         raise ValueError(
-            'Did not find cudata.var[\'highly_variable\']. '
-            'Either your data already only consists of highly-variable genes '
-            'or consider running `highly_variable_genes` first.'
+            "Did not find cudata.var['highly_variable']. "
+            "Either your data already only consists of highly-variable genes "
+            "or consider running `highly_variable_genes` first."
         )
 
     X = cudata.layers[layer] if layer is not None else cudata.X
 
     if use_highly_variable is None:
-        use_highly_variable = True if 'highly_variable' in cudata.var.keys() else False
+        use_highly_variable = True if "highly_variable" in cudata.var.keys() else False
 
     if use_highly_variable:
-        X = X[:, cudata.var['highly_variable']]
-
+        X = X[:, cudata.var["highly_variable"]]
 
-        
     if chunked:
         from cuml.decomposition import IncrementalPCA
 
         X_pca = np.zeros((X.shape[0], n_comps), X.dtype)
 
-        pca_func = IncrementalPCA(n_components=n_comps, output_type="numpy",batch_size=chunk_size)
+        pca_func = IncrementalPCA(
+            n_components=n_comps, output_type="numpy", batch_size=chunk_size
+        )
         pca_func.fit(X)
-        
+
         n_batches = math.ceil(X.shape[0] / chunk_size)
         for batch in range(n_batches):
             start_idx = batch * chunk_size
             stop_idx = min(batch * chunk_size + chunk_size, X.shape[0])
-            chunk = X[start_idx:stop_idx,:]
+            chunk = X[start_idx:stop_idx, :]
             chunk = chunk.toarray() if issparse(chunk) else chunk
             X_pca[start_idx:stop_idx] = pca_func.transform(chunk)
     else:
         if zero_center:
             pca_func = PCA(n_components=n_comps, output_type="numpy")
-            X_pca= pca_func.fit_transform(X)
+            X_pca = pca_func.fit_transform(X)
 
         elif not zero_center:
             pca_func = TruncatedSVD(n_components=n_comps, output_type="numpy")
             X_pca = pca_func.fit_transform(X)
-        
-    
+
     cudata.obsm["X_pca"] = X_pca
-    cudata.uns['pca'] ={'variance':pca_func.explained_variance_, 'variance_ratio':pca_func.explained_variance_ratio_}
+    cudata.uns["pca"] = {
+        "variance": pca_func.explained_variance_,
+        "variance_ratio": pca_func.explained_variance_ratio_,
+    }
     if use_highly_variable:
-        cudata.varm['PCs'] = np.zeros(shape=(cudata.n_vars, n_comps))
-        cudata.varm['PCs'][cudata.var['highly_variable']] = pca_func.components_.T
+        cudata.varm["PCs"] = np.zeros(shape=(cudata.n_vars, n_comps))
+        cudata.varm["PCs"][cudata.var["highly_variable"]] = pca_func.components_.T
     else:
-        cudata.varm['PCs'] = pca_func.components_.T
-        
+        cudata.varm["PCs"] = pca_func.components_.T
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_plotting.py` & `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_plotting.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 import os
 
-def scatter(cudata:cunnData, 
-                x:str, 
-                y:str,
-                color:str = None,
-                save:str = None,
-                show:bool =True,
-                dpi:int =300)-> None:
+
+def scatter(
+    cudata: cunnData,
+    x: str,
+    y: str,
+    color: str = None,
+    save: str = None,
+    show: bool = True,
+    dpi: int = 300,
+) -> None:
     """
     Violin plot.
     Wraps :func:`seaborn.scatterplot` for :class:`~rapids_singlecell.cunnData.cunnData`. This plotting function so far is really basic and doesnt include all the features form :func:`scanpy.pl.scatter`.
-    
+
     Parameters
     ---------
     cudata
         cunnData object
     x
         Keys for accessing variables of fields of `.obs`.
     y
@@ -28,41 +31,43 @@
     save
         file name to save plot as in ./figures
     show
         if you want to display the plot
     dpi
         The resolution in dots per inch for save
 
-    
+
     """
-    fig,ax = plt.subplots()
+    fig, ax = plt.subplots()
     if color == None:
-        sns.scatterplot(data=cudata.obs, x=x, y=y,s=2, color="grey", edgecolor="grey")
+        sns.scatterplot(data=cudata.obs, x=x, y=y, s=2, color="grey", edgecolor="grey")
     else:
-        sns.scatterplot(data=cudata.obs, x=x, y=y,s=2, hue=color)
+        sns.scatterplot(data=cudata.obs, x=x, y=y, s=2, hue=color)
 
     if save:
-        os.makedirs("./figures/",exist_ok=True)
-        fig_path = "./figures/"+save
-        plt.savefig(fig_path, dpi=dpi ,bbox_inches = 'tight')
+        os.makedirs("./figures/", exist_ok=True)
+        fig_path = "./figures/" + save
+        plt.savefig(fig_path, dpi=dpi, bbox_inches="tight")
     if show is False:
         plt.close()
 
-        
-def violin(cudata:cunnData,
-            key:str,
-            groupby:str=None,
-            size:float =1,
-            save:str = None,
-            show:bool =True,
-            dpi:int =300):
+
+def violin(
+    cudata: cunnData,
+    key: str,
+    groupby: str = None,
+    size: float = 1,
+    save: str = None,
+    show: bool = True,
+    dpi: int = 300,
+):
     """
     Violin plot.
     Wraps :func:`seaborn.violinplot` for :class:`~rapids_singlecell.cunnData.cunnData`. This plotting function so far is really basic and doesnt include all the features form :func:`scanpy.pl.violin`.
-    
+
     Parameters
     ---------
         cudata
             cunnData object
         key
             Keys for accessing variables of fields of `.obs`.
         groupby
@@ -71,23 +76,31 @@
             pt_size for stripplot if 0 no strip plot will be shown.
         save
             file name to save plot as in ./figures
         show
             if you want to display the plot
         dpi
             The resolution in dots per inch for save
-    
+
     Returns
     ------
     nothing
-    
+
     """
-    fig,ax = plt.subplots()
-    ax = sns.violinplot(data=cudata.obs, y=key,scale='width',x= groupby, inner = None)
+    fig, ax = plt.subplots()
+    ax = sns.violinplot(data=cudata.obs, y=key, scale="width", x=groupby, inner=None)
     if size:
-        ax = sns.stripplot(data=cudata.obs, y=key,x= groupby, color='k', size= size, dodge = True, jitter = True)
+        ax = sns.stripplot(
+            data=cudata.obs,
+            y=key,
+            x=groupby,
+            color="k",
+            size=size,
+            dodge=True,
+            jitter=True,
+        )
     if save:
-        os.makedirs("./figures/",exist_ok=True)
-        fig_path = "./figures/"+save
-        plt.savefig(fig_path, dpi=dpi ,bbox_inches = 'tight')
+        os.makedirs("./figures/", exist_ok=True)
+        fig_path = "./figures/" + save
+        plt.savefig(fig_path, dpi=dpi, bbox_inches="tight")
     if show is False:
         plt.close()
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_regress_out.py` & `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_regress_out.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import cupy as cp
 import cupyx as cpx
 from cuml.linear_model import LinearRegression
 from rapids_singlecell.cunnData import cunnData
-from typing import Literal, Union,Optional
+from typing import Literal, Union, Optional
 from ..cunnData import cunnData
 import math
 
-def regress_out(cudata:cunnData,
-                keys:Union[str,list],
-                layer: Optional[str] = None,
-                inplace:bool = True,
-                batchsize: Union[int,Literal["all"],None] = 100,
-                verbose:bool=False)-> Optional[cp.ndarray]:
 
+def regress_out(
+    cudata: cunnData,
+    keys: Union[str, list],
+    layer: Optional[str] = None,
+    inplace: bool = True,
+    batchsize: Union[int, Literal["all"], None] = 100,
+    verbose: bool = False,
+) -> Optional[cp.ndarray]:
     """
     Use linear regression to adjust for the effects of unwanted noise
     and variation. 
     
     Parameters
     ----------
         cudata
@@ -41,69 +43,75 @@
             Print debugging information
         
     Returns
     -------
     Returns a corrected copy or  updates `cudata` with a corrected version of the \
     original `cudata.X` and `cudata.layers['layer']`, depending on `inplace`.
     """
-    
+
     if batchsize != "all" and type(batchsize) not in [int, type(None)]:
         raise ValueError("batchsize must be `int`, `None` or `'all'`")
-    
-    X= cudata.layers[layer] if layer is not None else cudata.X
+
+    X = cudata.layers[layer] if layer is not None else cudata.X
 
     if cpx.scipy.sparse.issparse(X) and not cpx.scipy.sparse.isspmatrix_csc(X):
         X = X.tocsc()
 
-    dim_regressor= 2
-    if type(keys)is list:
-        dim_regressor = len(keys)+1
-
-    regressors = cp.ones((X.shape[0]*dim_regressor)).reshape((X.shape[0], dim_regressor), order="F")
-    if dim_regressor==2:
+    dim_regressor = 2
+    if type(keys) is list:
+        dim_regressor = len(keys) + 1
+
+    regressors = cp.ones((X.shape[0] * dim_regressor)).reshape(
+        (X.shape[0], dim_regressor), order="F"
+    )
+    if dim_regressor == 2:
         regressors[:, 1] = cp.array(cudata.obs[keys]).ravel()
     else:
-        for i in range(dim_regressor-1):
-            regressors[:, i+1] = cp.array(cudata.obs[keys[i]]).ravel()
+        for i in range(dim_regressor - 1):
+            regressors[:, i + 1] = cp.array(cudata.obs[keys[i]]).ravel()
 
     outputs = cp.empty(X.shape, dtype=X.dtype, order="F")
 
-    cuml_supports_multi_target = LinearRegression._get_tags()['multioutput']
+    cuml_supports_multi_target = LinearRegression._get_tags()["multioutput"]
 
     if cuml_supports_multi_target and batchsize:
         if batchsize == "all" and X.shape[0] < 100000:
-            if cpx.scipy.sparse.issparse(X): 
+            if cpx.scipy.sparse.issparse(X):
                 X = X.todense()
-            lr = LinearRegression(fit_intercept=False, output_type="cupy", algorithm='svd')
+            lr = LinearRegression(
+                fit_intercept=False, output_type="cupy", algorithm="svd"
+            )
             lr.fit(regressors, X, convert_dtype=True)
             outputs[:] = X - lr.predict(regressors)
         else:
             if batchsize == "all":
                 batchsize = 100
             n_batches = math.ceil(X.shape[1] / batchsize)
             for batch in range(n_batches):
                 start_idx = batch * batchsize
                 stop_idx = min(batch * batchsize + batchsize, X.shape[1])
                 if cpx.scipy.sparse.issparse(X):
-                    arr_batch = X[:,start_idx:stop_idx].todense()
+                    arr_batch = X[:, start_idx:stop_idx].todense()
                 else:
-                    arr_batch = X[:,start_idx:stop_idx].copy()
-                lr = LinearRegression(fit_intercept=False, output_type="cupy", algorithm='svd')
+                    arr_batch = X[:, start_idx:stop_idx].copy()
+                lr = LinearRegression(
+                    fit_intercept=False, output_type="cupy", algorithm="svd"
+                )
                 lr.fit(regressors, arr_batch, convert_dtype=True)
-                outputs[:,start_idx:stop_idx] =arr_batch - lr.predict(regressors)
+                outputs[:, start_idx:stop_idx] = arr_batch - lr.predict(regressors)
     else:
         if X.shape[0] < 100000 and cpx.scipy.sparse.issparse(X):
             X = X.todense()
         for i in range(X.shape[1]):
             if verbose and i % 500 == 0:
-                print("Regressed %s out of %s" %(i, X.shape[1]))
-            
-            y = X[:,i]
+                print("Regressed %s out of %s" % (i, X.shape[1]))
+
+            y = X[:, i]
             outputs[:, i] = _regress_out_chunk(regressors, y)
-    
+
     if inplace:
         if layer:
             cudata.layers[layer] = outputs
         else:
             cudata.X = outputs
     else:
         return outputs
@@ -125,8 +133,12 @@
         Adjusted column
     """
     if cp.sparse.issparse(y):
         y = y.todense()
 
     lr = LinearRegression(fit_intercept=False, output_type="cupy")
     lr.fit(X, y, convert_dtype=True)
-    return y.reshape(y.shape[0],) - lr.predict(X).reshape(y.shape[0])
+    return y.reshape(
+        y.shape[0],
+    ) - lr.predict(
+        X
+    ).reshape(y.shape[0])
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_scale.py` & `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_scale.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import cupy as cp
 from ..cunnData import cunnData
 from typing import Optional
 
 
-def scale(cudata:cunnData, 
-        max_value: int=10,
-        layer: Optional[str] = None,
-        inplace:bool = True)->Optional[cp.ndarray]:
-
+def scale(
+    cudata: cunnData,
+    max_value: int = 10,
+    layer: Optional[str] = None,
+    inplace: bool = True,
+) -> Optional[cp.ndarray]:
     """
     Scales matrix to unit variance and clips values
     
     Parameters
     ----------
         cudata
             cunnData object
@@ -33,22 +34,22 @@
     """
     X = cudata.layers[layer] if layer is not None else cudata.X
 
     if type(X) is not cp._core.core.ndarray:
         print("densifying _.X")
         X = X.toarray()
     else:
-        X =X.copy()
+        X = X.copy()
     mean = X.sum(axis=0).flatten() / X.shape[0]
     X -= mean
     del mean
     stddev = cp.sqrt(X.var(axis=0))
     X /= stddev
     del stddev
-    X= cp.clip(X,a_max=max_value)
+    X = cp.clip(X, a_max=max_value)
     if inplace:
         if layer:
             cudata.layers[layer] = X
         else:
             cudata.X = X
     else:
         return X
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/cunnData_funcs/_utils.py` & `rapids_singlecell-0.6.2/rapids_singlecell/cunnData_funcs/_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import cupy as cp
+from cupy.sparse import issparse
+
 
 def _get_mean_var(X):
     mean = (X.sum(axis=0) / X.shape[0]).flatten()
-    mean_sq = cp.sparse.csr_matrix((X.data ** 2,X.indices, X.indptr)).sum(axis=0).flatten() / X.shape[0]
-    var = (mean_sq - mean ** 2) * (X.shape[0] / (X.shape[0] - 1))
+    mean_sq = (
+        cp.sparse.csr_matrix((X.data**2, X.indices, X.indptr)).sum(axis=0).flatten()
+        / X.shape[0]
+    )
+    var = (mean_sq - mean**2) * (X.shape[0] / (X.shape[0] - 1))
     return mean, var
 
+
 def _check_nonnegative_integers(X):
-    """Checks values of X to ensure it is count data"""
-    data = X.data
+    if issparse(X):
+        data = X.data
+    else:
+        data = data
+    """Checks values of data to ensure it is count data"""
     # Check no negatives
     if cp.signbit(data).any():
         return False
     elif cp.any(~cp.equal(cp.mod(data, 1), 0)):
         return False
     else:
         return True
-
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,73 +6,76 @@
 
 from anndata import AnnData
 from scipy import stats
 
 from tqdm import tqdm
 from typing import Union, Optional
 
+
 def fit_mlm(X, y, inv, df):
     X = cp.ascontiguousarray(X)
     n_samples = y.shape[1]
     n_fsets = X.shape[1]
-    coef, sse, _, _ = cp.linalg.lstsq(X, y,rcond=-1)
+    coef, sse, _, _ = cp.linalg.lstsq(X, y, rcond=-1)
     if len(sse) == 0:
-        raise ValueError("""Couldn\'t fit a multivariate linear model. This can happen because there are more sources
+        raise ValueError(
+            """Couldn\'t fit a multivariate linear model. This can happen because there are more sources
         (covariates) than unique targets (samples), or because the network\'s matrix rank is smaller than the number of
-        sources.""")
+        sources."""
+        )
     sse = sse / df
     inv = cp.diag(inv)
-    sse = cp.reshape(sse, (sse.shape[0],1))
-    inv = cp.reshape(inv, (1,inv.shape[0]))
-    se= cp.sqrt(sse * inv)
-    t = coef.T/se
+    sse = cp.reshape(sse, (sse.shape[0], 1))
+    inv = cp.reshape(inv, (1, inv.shape[0]))
+    se = cp.sqrt(sse * inv)
+    t = coef.T / se
     return t.astype(np.float32)
 
 
 def mlm(mat, net, batch_size=10000, verbose=False):
-
     # Get number of batches
     n_samples = mat.shape[0]
     n_features, n_fsets = net.shape
     n_batches = int(np.ceil(n_samples / batch_size))
 
     # Add intercept to network
-    net = cp.column_stack((cp.ones((n_features, ), dtype=np.float32), cp.array(net)))
+    net = cp.column_stack((cp.ones((n_features,), dtype=np.float32), cp.array(net)))
 
     # Compute inv and df for lm
     inv = cp.linalg.inv(cp.dot(net.T, net))
     df = n_features - n_fsets
 
     # Init empty acts
     es = cp.zeros((n_samples, n_fsets), dtype=np.float32)
     for i in tqdm(range(n_batches), disable=not verbose):
-
         # Subset batch
-        srt, end = i*batch_size, i*batch_size+batch_size
+        srt, end = i * batch_size, i * batch_size + batch_size
         y = mat[srt:end].A.T
 
         # Compute MLM for batch
         es[srt:end] = fit_mlm(net, cp.array(y), inv, df)[:, 1:]
 
     # Get p-values
     es = es.get()
     pvals = 2 * (1 - stats.t.cdf(np.abs(es), df))
 
     return es, pvals
 
 
-def run_mlm(mat:Union[AnnData,pd.DataFrame,list], 
-            net:pd.DataFrame, 
-            source:str='source',
-            target:str='target', 
-            weight:str='weight', 
-            batch_size:int=10000,
-            min_n:int=5, 
-            verbose:bool=False, 
-            use_raw:bool=True)-> Optional[tuple]:
+def run_mlm(
+    mat: Union[AnnData, pd.DataFrame, list],
+    net: pd.DataFrame,
+    source: str = "source",
+    target: str = "target",
+    weight: str = "weight",
+    batch_size: int = 10000,
+    min_n: int = 5,
+    verbose: bool = False,
+    use_raw: bool = True,
+) -> Optional[tuple]:
     """
     Multivariate Linear Model (MLM).
     MLM fits a multivariate linear model for each sample, where the observed molecular readouts in `mat` are the response
     variable and the regulator weights in `net` are the covariates. Target features with no associated weight are set to
     zero. The obtained t-values from the fitted model are the activities (`mlm_estimate`) of the regulators in `net`.
 
     Parameters
@@ -91,15 +94,15 @@
             Size of the samples to use for each batch. Increasing this will consume more memmory but it will run faster.
         min_n
             Minimum of targets per source. If less, sources are removed.
         verbose
             Whether to show progress.
         use_raw
             Use raw attribute of mat if present.
-        
+
     Returns
     -------
         Updates `adata` with the following fields.
 
             **estimate** : DataFrame
                 MLM scores. Stored in `.obsm['mlm_estimate']` if `mat` is AnnData.
             **pvals** : DataFrame
@@ -114,24 +117,28 @@
     net = filt_min_n(c, net, min_n=min_n)
     sources, targets, net = get_net_mat(net)
 
     # Match arrays
     net = match(c, targets, net)
 
     if verbose:
-        print('Running mlm on mat with {0} samples and {1} targets for {2} sources.'.format(m.shape[0], len(c), net.shape[1]))
+        print(
+            "Running mlm on mat with {0} samples and {1} targets for {2} sources.".format(
+                m.shape[0], len(c), net.shape[1]
+            )
+        )
 
     # Run MLM
     estimate, pvals = mlm(m, net, batch_size=batch_size, verbose=verbose)
 
     # Transform to df
     estimate = pd.DataFrame(estimate, index=r, columns=sources)
-    estimate.name = 'mlm_estimate'
+    estimate.name = "mlm_estimate"
     pvals = pd.DataFrame(pvals, index=r, columns=sources)
-    pvals.name = 'mlm_pvals'
+    pvals.name = "mlm_pvals"
 
     # AnnData support
     if isinstance(mat, AnnData):
         # Update obsm AnnData object
         mat.obsm[estimate.name] = estimate
         mat.obsm[pvals.name] = pvals
     else:
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.6.2/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,74 +21,83 @@
     for i in range(times):
         cp.random.shuffle(idxs)
         null_dst[:, :, i] = mat.dot(net[idxs])
         pvals += cp.abs(null_dst[:, :, i]) > cp.abs(estimate)
 
     # Compute empirical p-value
     pvals = cp.where(pvals == 0.0, 1.0, pvals).astype(np.float32)
-    pvals = cp.where(pvals == times, times-1, pvals).astype(np.float32)
+    pvals = cp.where(pvals == times, times - 1, pvals).astype(np.float32)
     pvals = pvals / times
-    pvals = cp.where(pvals >= 0.5, 1-(pvals), pvals)
+    pvals = cp.where(pvals >= 0.5, 1 - (pvals), pvals)
     pvals = pvals * 2
-    
+
     # Compute z-score
-    norm = (estimate-null_dst.mean(axis=2))/null_dst.std(ddof=1,axis=2)
+    norm = (estimate - null_dst.mean(axis=2)) / null_dst.std(ddof=1, axis=2)
 
     # Compute corr score
     corr = (estimate * -cp.log10(pvals)).astype(np.float32)
-    
+
     estimate_return = estimate.get()
     norm_return = norm.get()
     corr_return = corr.get()
-    pvals_return =pvals.get()
-    del estimate,norm,corr,pvals,mat,null_dst
-    return estimate_return,norm_return ,corr_return , pvals_return
+    pvals_return = pvals.get()
+    del estimate, norm, corr, pvals, mat, null_dst
+    return estimate_return, norm_return, corr_return, pvals_return
 
 
 def wsum(mat, net, times, batch_size, seed, verbose):
     # Get number of batches
     n_samples = mat.shape[0]
     n_features, n_fsets = net.shape
     n_batches = int(np.ceil(n_samples / batch_size))
 
     if verbose:
-        print('Infering activities on {0} batches.'.format(n_batches))
+        print("Infering activities on {0} batches.".format(n_batches))
 
     # Init empty acts
     estimate = np.zeros((n_samples, n_fsets), dtype=np.float32)
     if times > 1:
         norm = np.zeros((n_samples, n_fsets), dtype=np.float32)
         corr = np.zeros((n_samples, n_fsets), dtype=np.float32)
         pvals = np.zeros((n_samples, n_fsets), dtype=np.float32)
     else:
         norm, corr, pvals = None, None, None
 
     for i in tqdm(range(n_batches), disable=not verbose):
         # Subset batch
-        srt, end = i*batch_size, i*batch_size+batch_size
+        srt, end = i * batch_size, i * batch_size + batch_size
         tmp = mat[srt:end].A
         # Run WSUM
         estimate[srt:end] = tmp.dot(net)
         if times > 1:
             idxs = np.arange(n_features, dtype=np.int32)
-            estimate[srt:end],norm[srt:end], corr[srt:end], pvals[srt:end] = run_perm(cp.array(estimate[srt:end]), cp.array(tmp), cp.array(net), cp.array(idxs), times, seed)
+            estimate[srt:end], norm[srt:end], corr[srt:end], pvals[srt:end] = run_perm(
+                cp.array(estimate[srt:end]),
+                cp.array(tmp),
+                cp.array(net),
+                cp.array(idxs),
+                times,
+                seed,
+            )
     return estimate, norm, corr, pvals
 
 
-def run_wsum(mat:Union[AnnData,pd.DataFrame,list], 
-            net:pd.DataFrame, 
-            source='source', 
-            target='target', 
-            weight='weight', 
-            times=1000, 
-            batch_size:int=10000, 
-            min_n:int=5, 
-            seed:int=42,
-            verbose:bool=False,
-            use_raw:bool=True)-> Optional[tuple]:
+def run_wsum(
+    mat: Union[AnnData, pd.DataFrame, list],
+    net: pd.DataFrame,
+    source="source",
+    target="target",
+    weight="weight",
+    times=1000,
+    batch_size: int = 10000,
+    min_n: int = 5,
+    seed: int = 42,
+    verbose: bool = False,
+    use_raw: bool = True,
+) -> Optional[tuple]:
     """
     Weighted sum (WSUM).
     WSUM infers regulator activities by first multiplying each target feature by its associated weight which then are summed
     to an enrichment score (`wsum_estimate`). Furthermore, permutations of random target features can be performed to obtain a
     null distribution that can be used to compute a z-score (`wsum_norm`), or a corrected estimate (`wsum_corr`) by multiplying
     `wsum_estimate` by the minus log10 of the obtained empirical p-value.
 
@@ -106,21 +115,21 @@
             Column name in net with weights.
         times
             How many random permutations to do.
         batch_size
             Size of the batches to use. Increasing this will consume more memmory but it will run faster.
         min_n
             Minimum of targets per source. If less, sources are removed.
-        seed 
+        seed
             Random seed to use.
         verbose
             Whether to show progress.
         use_raw
             Use raw attribute of mat if present.
-        
+
     Returns
     -------
         Updates `adata` with the following fields.
 
             **estimate** : DataFrame
                 WSUM scores. Stored in `.obsm['wsum_estimate']` if `mat` is AnnData.
             **norm**: DataFrame
@@ -138,37 +147,40 @@
     net = filt_min_n(c, net, min_n=min_n)
     sources, targets, net = get_net_mat(net)
 
     # Match arrays
     net = match(c, targets, net)
 
     if verbose:
-        print('Running wsum on mat with {0} samples and {1} targets for {2} sources.'.format(m.shape[0], len(c), net.shape[1]))
+        print(
+            "Running wsum on mat with {0} samples and {1} targets for {2} sources.".format(
+                m.shape[0], len(c), net.shape[1]
+            )
+        )
 
     # Run WSUM
     estimate, norm, corr, pvals = wsum(m, net, times, batch_size, seed, verbose)
 
     # Transform to df
     estimate = pd.DataFrame(estimate, index=r, columns=sources)
-    estimate.name = 'wsum_estimate'
+    estimate.name = "wsum_estimate"
     if pvals is not None:
         norm = pd.DataFrame(norm, index=r, columns=sources)
-        norm.name = 'wsum_norm'
+        norm.name = "wsum_norm"
         corr = pd.DataFrame(corr, index=r, columns=sources)
-        corr.name = 'wsum_corr'
+        corr.name = "wsum_corr"
         pvals = pd.DataFrame(pvals, index=r, columns=sources)
-        pvals.name = 'wsum_pvals'
+        pvals.name = "wsum_pvals"
 
     # AnnData support
     if isinstance(mat, AnnData):
         # Update obsm AnnData object
         mat.obsm[estimate.name] = estimate
         if pvals is not None:
             mat.obsm[norm.name] = norm
             mat.obsm[corr.name] = corr
             mat.obsm[pvals.name] = pvals
     else:
         if pvals is not None:
-             return estimate, norm, corr, pvals
+            return estimate, norm, corr, pvals
         else:
-             return estimate
-            
+            return estimate
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_clustering.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,175 +8,187 @@
 from anndata import AnnData
 
 from typing import Optional
 from natsort import natsorted
 
 import warnings
 
-def leiden(adata: AnnData, 
-           resolution: float =1.0,
-           n_iterations:int = -1,
-           use_weights: bool =True,
-           neighbors_key: Optional[int] = None,
-           key_added: str = 'leiden')-> None:
+
+def leiden(
+    adata: AnnData,
+    resolution: float = 1.0,
+    n_iterations: int = -1,
+    use_weights: bool = True,
+    neighbors_key: Optional[int] = None,
+    key_added: str = "leiden",
+) -> None:
     """
     Performs Leiden Clustering using cuGraph
 
     Parameters
     ----------
-        adata : 
+        adata :
             annData object with 'neighbors' field.
-        
-        resolution 
+
+        resolution
             A parameter value controlling the coarseness of the clustering.
             Higher values lead to more clusters.
-        
+
         n_iterations
             How many iterations of the Leiden clustering algorithm to perform.
             Positive values above 2 define the total number of iterations to perform,
             -1 has the algorithm run until it reaches its optimal clustering.
 
         use_weights
             If `True`, edge weights from the graph are used in the computation
             (placing more emphasis on stronger edges).
-        
+
         neighbors_key
             If not specified, `leiden` looks at `.obsp['connectivities']` for neighbors connectivities
             If specified, `leiden` looks at `.obsp['neighbors_key_ connectivities']` for neighbors connectivities
-        
+
         key_added
             `adata.obs` key under which to add the cluster labels.
-        
+
     """
     # Adjacency graph
-    
+
     if neighbors_key:
-        adjacency = adata.obsp[neighbors_key+"_connectivities"]
+        adjacency = adata.obsp[neighbors_key + "_connectivities"]
     else:
         adjacency = adata.obsp["connectivities"]
     offsets = cudf.Series(adjacency.indptr)
     indices = cudf.Series(adjacency.indices)
     if use_weights:
-
         weights = cudf.Series(adjacency.data)
     else:
         weights = None
-    
+
     g = cugraph.Graph()
 
     g.from_cudf_adjlist(offsets, indices, weights)
 
     # Cluster
-    leiden_parts, _ = cugraph.leiden(g,resolution = resolution,max_iter=n_iterations)
-    
+    leiden_parts, _ = cugraph.leiden(g, resolution=resolution, max_iter=n_iterations)
+
     # Format output
-    groups = leiden_parts.to_pandas().sort_values('vertex')[['partition']].to_numpy().ravel()
-   
+    groups = (
+        leiden_parts.to_pandas().sort_values("vertex")[["partition"]].to_numpy().ravel()
+    )
+
     adata.obs[key_added] = pd.Categorical(
-        values=groups.astype('U'),
+        values=groups.astype("U"),
         categories=natsorted(map(str, np.unique(groups))),
     )
     # store information on the clustering parameters
-    adata.uns['leiden'] = {}
-    adata.uns['leiden']['params'] = dict(
+    adata.uns["leiden"] = {}
+    adata.uns["leiden"]["params"] = dict(
         resolution=resolution,
         n_iterations=n_iterations,
     )
 
-    
-def louvain(adata: AnnData, 
-            resolution: float=1.0,
-            n_iterations: int = 100,
-            use_weights: bool =True,
-            neighbors_key: Optional[str] = None,
-            key_added: str = 'louvain')-> None:
+
+def louvain(
+    adata: AnnData,
+    resolution: float = 1.0,
+    n_iterations: int = 100,
+    use_weights: bool = True,
+    neighbors_key: Optional[str] = None,
+    key_added: str = "louvain",
+) -> None:
     """
     Performs Louvain Clustering using cuGraph
-    
+
     Parameters
     ----------
-        adata : 
+        adata :
             annData object with 'neighbors' field.
-        
-        resolution 
+
+        resolution
             A parameter value controlling the coarseness of the clustering.
             Higher values lead to more clusters.
-        
+
         n_iterations
-            This controls the maximum number of levels/iterations of the Louvain algorithm. 
-            When specified the algorithm will terminate after no more than the specified number of iterations. 
+            This controls the maximum number of levels/iterations of the Louvain algorithm.
+            When specified the algorithm will terminate after no more than the specified number of iterations.
             No error occurs when the algorithm terminates early in this manner.
 
-        use_weights 
+        use_weights
             If `True`, edge weights from the graph are used in the computation
             (placing more emphasis on stronger edges).
-            
-        neighbors_key 
+
+        neighbors_key
             If not specified, `louvain` looks at `.obsp['connectivities']` for neighbors connectivities
             If specified, `louvain` looks at `.obsp['neighbors_key_ connectivities']` for neighbors connectivities
-        
+
         key_added
             `adata.obs` key under which to add the cluster labels.
 
     """
     # Adjacency graph
-    
+
     if neighbors_key:
-        adjacency = adata.obsp[neighbors_key+"_connectivities"]
+        adjacency = adata.obsp[neighbors_key + "_connectivities"]
     else:
         adjacency = adata.obsp["connectivities"]
-    
+
     offsets = cudf.Series(adjacency.indptr)
     indices = cudf.Series(adjacency.indices)
     if use_weights:
-
         weights = cudf.Series(adjacency.data)
     else:
         weights = None
-    
+
     g = cugraph.Graph()
 
     g.from_cudf_adjlist(offsets, indices, weights)
 
     # Cluster
-    louvain_parts, _ = cugraph.louvain(g,resolution = resolution,max_iter=n_iterations)
-    
+    louvain_parts, _ = cugraph.louvain(g, resolution=resolution, max_iter=n_iterations)
+
     # Format output
-    groups = louvain_parts.to_pandas().sort_values('vertex')[['partition']].to_numpy().ravel()
+    groups = (
+        louvain_parts.to_pandas()
+        .sort_values("vertex")[["partition"]]
+        .to_numpy()
+        .ravel()
+    )
 
     adata.obs[key_added] = pd.Categorical(
-        values=groups.astype('U'),
+        values=groups.astype("U"),
         categories=natsorted(map(str, np.unique(groups))),
     )
-    adata.uns['louvain'] = {}
-    adata.uns['louvain']['params'] = dict(
-        resolution=resolution
-    )
-    
-def kmeans(adata: AnnData, 
-           n_clusters:int =8,
-           key_added:str = "kmeans",
-           random_state:float= 42)-> None:
+    adata.uns["louvain"] = {}
+    adata.uns["louvain"]["params"] = dict(resolution=resolution)
+
+
+def kmeans(
+    adata: AnnData,
+    n_clusters: int = 8,
+    key_added: str = "kmeans",
+    random_state: float = 42,
+) -> None:
     """
-    KMeans is a basic but powerful clustering method which is optimized via Expectation Maximization. 
+    KMeans is a basic but powerful clustering method which is optimized via Expectation Maximization.
 
     Parameters
     ----------
         adata: adata object with `.obsm['X_pca']`
-        
+
         n_clusters: int (default:8)
             Number of clusters to compute
-            
+
         random_state: float (default: 42)
             if you want results to be the same when you restart Python, select a
             state.
-    
+
     """
 
-    
-    kmeans_out = KMeans(n_clusters=n_clusters, random_state=random_state).fit(adata.obsm['X_pca'])
+    kmeans_out = KMeans(n_clusters=n_clusters, random_state=random_state).fit(
+        adata.obsm["X_pca"]
+    )
     groups = kmeans_out.labels_.astype(str)
 
     adata.obs[key_added] = pd.Categorical(
-        values=groups.astype('U'),
+        values=groups.astype("U"),
         categories=natsorted(map(str, np.unique(groups))),
     )
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_diffmap.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_diffmap.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,91 +2,93 @@
 from scipy.sparse import issparse
 import cupyx.scipy.sparse.linalg
 import cupyx.scipy.sparse
 import cupyx as cpx
 import cupy as cp
 
 
-def diffmap(adata: AnnData, 
-            n_comps: int=15, 
-            neighbors_key: str = None, 
-            sort: str = 'decrease',
-            density_normalize: bool = True)-> None:
+def diffmap(
+    adata: AnnData,
+    n_comps: int = 15,
+    neighbors_key: str = None,
+    sort: str = "decrease",
+    density_normalize: bool = True,
+) -> None:
     """
     Diffusion maps has been proposed for visualizing single-cell data.
-    
+
     This is a reimplementation of scanpys function.
-    
+
     The width ("sigma") of the connectivity kernel is implicitly determined by
     the number of neighbors used to compute the single-cell graph in
-    :func:`~scanpy.pp.neighbors`. 
-    
+    :func:`~scanpy.pp.neighbors`.
+
     Parameters
     ----------
         adata
             Annotated data matrix.
-        n_comps 
+        n_comps
             The number of dimensions of the representation.
         neighbors_key
             If not specified, diffmap looks at `.obsp['connectivities']` for neighbors connectivities
             If specified, diffmap looks at `.obsp['neighbors_key_ connectivities']` for neighbors connectivities
         sort
             Leave as is for the same behavior as sc.tl.diffmap
         density_normalize
             Leave as is for the same behavior as sc.tl.diffmap
-    
+
     Returns
     ----------
         updates `adata` with the following fields.
-        
+
             `X_diffmap` : :class:`numpy.ndarray` (`adata.obsm`)
                 Diffusion map representation of data, which is the right eigen basis of
                 the transition matrix with eigenvectors as columns.
             `diffmap_evals` : :class:`numpy.ndarray` (`adata.uns`)
                 Array of size (number of eigen vectors).
                 Eigenvalues of transition matrix.
     """
 
     if neighbors_key:
-        connectivities = adata.obsp[neighbors_key+"_connectivities"]
+        connectivities = adata.obsp[neighbors_key + "_connectivities"]
     else:
         connectivities = adata.obsp["connectivities"]
     if issparse(connectivities):
         W = cp.sparse.csr_matrix(connectivities, dtype=cp.float32)
     else:
         W = cp.asarray(connectivities)
     if density_normalize:
-            # q[i] is an estimate for the sampling density at point i
-            # it's also the degree of the underlying graph
-            q = cp.asarray(W.sum(axis=0))
-            if not cpx.scipy.sparse.issparse(W):
-                Q = cp.diag(1.0 / q)
-            else:
-                Q = cpx.scipy.sparse.spdiags(1.0 / q, 0, W.shape[0], W.shape[0])
-            K = Q @ W @ Q
+        # q[i] is an estimate for the sampling density at point i
+        # it's also the degree of the underlying graph
+        q = cp.asarray(W.sum(axis=0))
+        if not cpx.scipy.sparse.issparse(W):
+            Q = cp.diag(1.0 / q)
+        else:
+            Q = cpx.scipy.sparse.spdiags(1.0 / q, 0, W.shape[0], W.shape[0])
+        K = Q @ W @ Q
     else:
         K = W
-            # z[i] is the square root of the row sum of K
+        # z[i] is the square root of the row sum of K
     z = cp.sqrt(cp.asarray(K.sum(axis=0)))
     if not cpx.scipy.sparse.issparse(K):
         Z = cp.diag(1.0 / z)
     else:
         Z = cpx.scipy.sparse.spdiags(1.0 / z, 0, K.shape[0], K.shape[0])
     matrix = Z @ K @ Z
     if n_comps == 0:
-                evals, evecs = cpx.scipy.sparse.linalg.eigsh(matrix)
+        evals, evecs = cpx.scipy.sparse.linalg.eigsh(matrix)
     else:
         n_comps = min(matrix.shape[0] - 1, n_comps)
         # ncv = max(2 * n_comps + 1, int(np.sqrt(matrix.shape[0])))
         ncv = None
-        which = 'LM' if sort == 'decrease' else 'SM'
+        which = "LM" if sort == "decrease" else "SM"
         # it pays off to increase the stability with a bit more precision
         matrix = matrix.astype(cp.float64)
         evals, evecs = cpx.scipy.sparse.linalg.eigsh(
             matrix, k=n_comps, which=which, ncv=ncv
         )
         evals, evecs = evals.astype(cp.float32), evecs.astype(cp.float32)
-    if sort == 'decrease':
+    if sort == "decrease":
         evals = evals[::-1]
         evecs = evecs[:, ::-1]
     adata.uns["diffmap_evals"] = evals.get()
     adata.obsm["X_diffmap"] = evecs.get()
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_draw_graph.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_draw_graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,109 @@
 from anndata import AnnData
 import cudf
 import cugraph
 import numpy as np
 import cupy as cp
 from typing import Union
 
-def draw_graph(adata: AnnData,
-               init_pos: Union[str, bool, None]= None,
-               max_iter:int = 500)-> None:
+
+def draw_graph(
+    adata: AnnData, init_pos: Union[str, bool, None] = None, max_iter: int = 500
+) -> None:
     """
     Force-directed graph drawing with cugraph's implementation of Force Atlas 2.
     This is a reimplementation of scanpys function for GPU compute.
 
     Parameters
     ----------
-        adata 
+        adata
             annData object with 'neighbors' field.
-        
+
         init_pos
             `'paga'`/`True`, `None`/`False`, or any valid 2d-`.obsm` key.
             Use precomputed coordinates for initialization.
             If `False`/`None` (the default), initialize randomly.
-        max_iter 
+        max_iter
             This controls the maximum number of levels/iterations of the
             Force Atlas algorithm. When specified the algorithm will terminate
             after no more than the specified number of iterations.
             No error occurs when the algorithm terminates in this manner.
             Good short-term quality can be achieved with 50-100 iterations.
             Above 1000 iterations is discouraged.
-    
+
     Returns
     ----------
         updates `adata` with the following fields.
-        
+
             X_draw_graph_layout_fa : `adata.obsm`
                 Coordinates of graph layout.
     """
-    
+
     from cugraph.layout import force_atlas2
+
     # Adjacency graph
     adjacency = adata.obsp["connectivities"]
     offsets = cudf.Series(adjacency.indptr)
     indices = cudf.Series(adjacency.indices)
     g = cugraph.Graph()
-    if hasattr(g, 'add_adj_list'):
+    if hasattr(g, "add_adj_list"):
         g.add_adj_list(offsets, indices, None)
     else:
         g.from_cudf_adjlist(offsets, indices, None)
-    #Get Intial Positions
+    # Get Intial Positions
     if init_pos in adata.obsm.keys():
         init_coords = adata.obsm[init_pos]
-    elif init_pos == 'paga' or init_pos:
-        if 'paga' in adata.uns and 'pos' in adata.uns['paga']:
-            groups = adata.obs[adata.uns['paga']['groups']]
-            pos = adata.uns['paga']['pos']
-            connectivities_coarse = adata.uns['paga']['connectivities']
+    elif init_pos == "paga" or init_pos:
+        if "paga" in adata.uns and "pos" in adata.uns["paga"]:
+            groups = adata.obs[adata.uns["paga"]["groups"]]
+            pos = adata.uns["paga"]["pos"]
+            connectivities_coarse = adata.uns["paga"]["connectivities"]
             init_coords = np.ones((adjacency.shape[0], 2))
             for i, group_pos in enumerate(pos):
                 subset = (groups == groups.cat.categories[i]).values
                 neighbors = connectivities_coarse[i].nonzero()
                 if len(neighbors[1]) > 0:
                     connectivities = connectivities_coarse[i][neighbors]
                     nearest_neighbor = neighbors[1][np.argmax(connectivities)]
                     noise = np.random.random((len(subset[subset]), 2))
                     dist = pos[i] - pos[nearest_neighbor]
                     noise = noise * dist
                     init_coords[subset] = group_pos - 0.5 * dist + noise
                 else:
                     init_coords[subset] = group_pos
         else:
-            raise ValueError('Plot PAGA first, so that adata.uns[\'paga\']' 'with key \'pos\'.')
-        
+            raise ValueError(
+                "Plot PAGA first, so that adata.uns['paga']" "with key 'pos'."
+            )
+
     else:
         init_coords = None
-    
-    if init_coords is not None: 
-        x,y = np.hsplit(init_coords, init_coords.shape[1])
-        inital_df = cudf.DataFrame({"x":x.ravel(),"y":y.ravel()})
+
+    if init_coords is not None:
+        x, y = np.hsplit(init_coords, init_coords.shape[1])
+        inital_df = cudf.DataFrame({"x": x.ravel(), "y": y.ravel()})
         inital_df["vertex"] = inital_df.index
     else:
-        inital_df= None
-    #Run cugraphs Force Atlas 2 
-    positions = force_atlas2(input_graph = g, pos_list=inital_df, max_iter= max_iter,outbound_attraction_distribution=False,  
-            lin_log_mode=False,  
-            edge_weight_influence=1.0,
-            # Performance
-            jitter_tolerance=1.0,  # Tolerance
-            barnes_hut_optimize=True,
-            barnes_hut_theta=1.2,
-            # Tuning
-            scaling_ratio=2.0,
-            strong_gravity_mode=False,
-            gravity=1.0,)
-    positions = cp.vstack((positions["x"].to_cupy(),positions["y"].to_cupy())).T
+        inital_df = None
+    # Run cugraphs Force Atlas 2
+    positions = force_atlas2(
+        input_graph=g,
+        pos_list=inital_df,
+        max_iter=max_iter,
+        outbound_attraction_distribution=False,
+        lin_log_mode=False,
+        edge_weight_influence=1.0,
+        # Performance
+        jitter_tolerance=1.0,  # Tolerance
+        barnes_hut_optimize=True,
+        barnes_hut_theta=1.2,
+        # Tuning
+        scaling_ratio=2.0,
+        strong_gravity_mode=False,
+        gravity=1.0,
+    )
+    positions = cp.vstack((positions["x"].to_cupy(), positions["y"].to_cupy())).T
     layout = "fa"
-    adata.uns['draw_graph'] = {}
-    adata.uns['draw_graph']['params'] = dict(layout=layout, random_state=0)
-    key_added = f'X_draw_graph_{layout}'
-    adata.obsm[key_added] = positions.get()    # Format output
+    adata.uns["draw_graph"] = {}
+    adata.uns["draw_graph"]["params"] = dict(layout=layout, random_state=0)
+    key_added = f"X_draw_graph_{layout}"
+    adata.obsm[key_added] = positions.get()  # Format output
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_embedding_density.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_embedding_density.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from anndata import AnnData
 import cupy as cp
 import numpy as np
 
+
 def embedding_density(
     adata: AnnData,
-    basis: str = 'umap',
-    groupby = None,
-    key_added = None,
-    components = None,
+    basis: str = "umap",
+    groupby=None,
+    key_added=None,
+    components=None,
 ) -> None:
     """\
     Calculate the density of cells in an embedding (per condition).
     Gaussian kernel density estimation is used to calculate the density of
     cells in an embedded space. This can be performed per category over a
     categorical cell annotation. The cell density can be plotted using the
     `pl.embedding_density` function.
@@ -51,93 +52,96 @@
     """
     # to ensure that newly created covariates are categorical
     # to test for category numbers
     adata._sanitize()
     # Test user inputs
     basis = basis.lower()
 
-    if basis == 'fa':
-        basis = 'draw_graph_fa'
+    if basis == "fa":
+        basis = "draw_graph_fa"
 
-    if f'X_{basis}' not in adata.obsm_keys():
+    if f"X_{basis}" not in adata.obsm_keys():
         raise ValueError(
             "Cannot find the embedded representation "
             f"`adata.obsm['X_{basis}']`. Compute the embedding first."
         )
 
     if components is None:
-        components = '1,2'
+        components = "1,2"
     if isinstance(components, str):
-        components = components.split(',')
+        components = components.split(",")
     components = np.array(components).astype(int) - 1
 
     if len(components) != 2:
-        raise ValueError('Please specify exactly 2 components, or `None`.')
+        raise ValueError("Please specify exactly 2 components, or `None`.")
 
-    if basis == 'diffmap':
+    if basis == "diffmap":
         components += 1
 
     if groupby is not None:
         if groupby not in adata.obs:
-            raise ValueError(f'Could not find {groupby!r} `.obs` column.')
+            raise ValueError(f"Could not find {groupby!r} `.obs` column.")
 
-        if adata.obs[groupby].dtype.name != 'category':
-            raise ValueError(f'{groupby!r} column does not contain categorical data')
+        if adata.obs[groupby].dtype.name != "category":
+            raise ValueError(f"{groupby!r} column does not contain categorical data")
 
     # Define new covariate name
     if key_added is not None:
         density_covariate = key_added
     elif groupby is not None:
-        density_covariate = f'{basis}_density_{groupby}'
+        density_covariate = f"{basis}_density_{groupby}"
     else:
-        density_covariate = f'{basis}_density'
+        density_covariate = f"{basis}_density"
 
     # Calculate the densities over each category in the groupby column
     if groupby is not None:
         categories = adata.obs[groupby].cat.categories
 
         density_values = np.zeros(adata.n_obs)
 
         for cat in categories:
             cat_mask = adata.obs[groupby] == cat
-            embed_x = adata.obsm[f'X_{basis}'][cat_mask, components[0]]
-            embed_y = adata.obsm[f'X_{basis}'][cat_mask, components[1]]
+            embed_x = adata.obsm[f"X_{basis}"][cat_mask, components[0]]
+            embed_y = adata.obsm[f"X_{basis}"][cat_mask, components[1]]
 
             dens_embed = _calc_density(cp.array(embed_x), cp.array(embed_y))
             density_values[cat_mask] = dens_embed
 
         adata.obs[density_covariate] = density_values
     else:  # if groupby is None
         # Calculate the density over the whole embedding without subsetting
-        embed_x = adata.obsm[f'X_{basis}'][:, components[0]]
-        embed_y = adata.obsm[f'X_{basis}'][:, components[1]]
+        embed_x = adata.obsm[f"X_{basis}"][:, components[0]]
+        embed_y = adata.obsm[f"X_{basis}"][:, components[1]]
 
-        adata.obs[density_covariate] = _calc_density(cp.array(embed_x), cp.array(embed_y))
+        adata.obs[density_covariate] = _calc_density(
+            cp.array(embed_x), cp.array(embed_y)
+        )
 
     # Reduce diffmap components for labeling
     # Note: plot_scatter takes care of correcting diffmap components
     #       for plotting automatically
-    if basis != 'diffmap':
+    if basis != "diffmap":
         components += 1
 
-    adata.uns[f'{density_covariate}_params'] = dict(
+    adata.uns[f"{density_covariate}_params"] = dict(
         covariate=groupby, components=components.tolist()
     )
 
+
 def _calc_density(x: cp.ndarray, y: cp.ndarray):
     """\
     Calculates the density of points in 2 dimensions.
     """
     from cuml.neighbors import KernelDensity
-    
+
     # Calculate the point density
     xy = cp.vstack([x, y]).T
-    bandwidth = cp.power(xy.shape[0],(-1./(xy.shape[1]+4)))
-    kde = KernelDensity(kernel='gaussian', bandwidth=bandwidth).fit(xy)
+    bandwidth = cp.power(xy.shape[0], (-1.0 / (xy.shape[1] + 4)))
+    kde = KernelDensity(kernel="gaussian", bandwidth=bandwidth).fit(xy)
     z = kde.score_samples(xy)
     min_z = cp.min(z)
     max_z = cp.max(z)
 
     # Scale between 0 and 1
     scaled_z = (z - min_z) / (max_z - min_z)
-    
+
     return scaled_z.get()
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,46 +20,46 @@
 import numpy as np
 import cupy as cp
 
 from cuml import KMeans
 import logging
 
 # create logger
-logger = logging.getLogger('harmonypy_gpu')
+logger = logging.getLogger("harmonypy_gpu")
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
-formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 
 # from IPython.core.debugger import set_trace
 
+
 def run_harmony(
     data_mat: np.ndarray,
     meta_data: pd.DataFrame,
     vars_use,
-    theta = None,
-    lamb = None,
-    sigma = 0.1, 
-    nclust = None,
-    tau = 0,
-    block_size = 0.05, 
-    max_iter_harmony = 10,
-    max_iter_kmeans = 20,
-    epsilon_cluster = 1e-5,
-    epsilon_harmony = 1e-4, 
-    plot_convergence = False,
-    verbose = True,
-    reference_values = None,
-    cluster_prior = None,
-    random_state = 0
+    theta=None,
+    lamb=None,
+    sigma=0.1,
+    nclust=None,
+    tau=0,
+    block_size=0.05,
+    max_iter_harmony=10,
+    max_iter_kmeans=20,
+    epsilon_cluster=1e-5,
+    epsilon_harmony=1e-4,
+    plot_convergence=False,
+    verbose=True,
+    reference_values=None,
+    cluster_prior=None,
+    random_state=0,
 ):
-    """Run Harmony.
-    """
+    """Run Harmony."""
 
     # theta = None
     # lamb = None
     # sigma = 0.1
     # nclust = None
     # tau = 0
     # block_size = 0.05
@@ -71,152 +71,175 @@
     # cluster_prior = None
     # random_state = 0
 
     N = meta_data.shape[0]
     if data_mat.shape[1] != N:
         data_mat = data_mat.T
 
-    assert data_mat.shape[1] == N, \
-       "data_mat and meta_data do not have the same number of cells" 
+    assert (
+        data_mat.shape[1] == N
+    ), "data_mat and meta_data do not have the same number of cells"
 
     if nclust is None:
         nclust = np.min([np.round(N / 30.0), 100]).astype(int)
 
     if type(sigma) is float and nclust > 1:
         sigma = np.repeat(sigma, nclust)
 
     if isinstance(vars_use, str):
         vars_use = [vars_use]
 
     phi = pd.get_dummies(meta_data[vars_use]).to_numpy().T
-    phi_n = meta_data[vars_use].describe().loc['unique'].to_numpy().astype(int)
+    phi_n = meta_data[vars_use].describe().loc["unique"].to_numpy().astype(int)
 
     if theta is None:
         theta = np.repeat([1] * len(phi_n), phi_n)
     elif isinstance(theta, float) or isinstance(theta, int):
         theta = np.repeat([theta] * len(phi_n), phi_n)
     elif len(theta) == len(phi_n):
         theta = np.repeat([theta], phi_n)
 
-    assert len(theta) == np.sum(phi_n), \
-        "each batch variable must have a theta"
+    assert len(theta) == np.sum(phi_n), "each batch variable must have a theta"
 
     if lamb is None:
         lamb = np.repeat([1] * len(phi_n), phi_n)
     elif isinstance(lamb, float) or isinstance(lamb, int):
         lamb = np.repeat([lamb] * len(phi_n), phi_n)
     elif len(lamb) == len(phi_n):
         lamb = np.repeat([lamb], phi_n)
 
-    assert len(lamb) == np.sum(phi_n), \
-        "each batch variable must have a lambda"
+    assert len(lamb) == np.sum(phi_n), "each batch variable must have a lambda"
 
     # Number of items in each category.
-    N_b = phi.sum(axis = 1)
+    N_b = phi.sum(axis=1)
     # Proportion of items in each category.
     Pr_b = N_b / N
 
     if tau > 0:
-        theta = theta * (1 - np.exp(-(N_b / (nclust * tau)) ** 2))
+        theta = theta * (1 - np.exp(-((N_b / (nclust * tau)) ** 2)))
 
     lamb_mat = np.diag(np.insert(lamb, 0, 0))
 
     phi_moe = np.vstack((np.repeat(1, N), phi))
 
     np.random.seed(random_state)
 
     ho = Harmony(
-        data_mat, phi, phi_moe, Pr_b, sigma, theta, max_iter_harmony, max_iter_kmeans,
-        epsilon_cluster, epsilon_harmony, nclust, block_size, lamb_mat, verbose
+        data_mat,
+        phi,
+        phi_moe,
+        Pr_b,
+        sigma,
+        theta,
+        max_iter_harmony,
+        max_iter_kmeans,
+        epsilon_cluster,
+        epsilon_harmony,
+        nclust,
+        block_size,
+        lamb_mat,
+        verbose,
     )
 
     return ho
 
+
 class Harmony(object):
     def __init__(
-            self, Z, Phi, Phi_moe, Pr_b, sigma,
-            theta, max_iter_harmony, max_iter_kmeans, 
-            epsilon_kmeans, epsilon_harmony, K, block_size,
-            lamb, verbose
+        self,
+        Z,
+        Phi,
+        Phi_moe,
+        Pr_b,
+        sigma,
+        theta,
+        max_iter_harmony,
+        max_iter_kmeans,
+        epsilon_kmeans,
+        epsilon_harmony,
+        K,
+        block_size,
+        lamb,
+        verbose,
     ):
         self.Z_corr = cp.array(Z)
         self.Z_orig = cp.array(Z)
 
         self.Z_cos = self.Z_orig / self.Z_orig.max(axis=0)
         self.Z_cos = self.Z_cos / cp.linalg.norm(self.Z_cos, ord=2, axis=0)
 
-        self.Phi             = cp.array(Phi)
-        self.Phi_moe         = cp.array(Phi_moe)
-        self.N               = self.Z_corr.shape[1]
-        self.Pr_b            = cp.array(Pr_b)
-        self.B               = self.Phi.shape[0] # number of batch variables
-        self.d               = self.Z_corr.shape[0]
-        self.window_size     = 3
-        self.epsilon_kmeans  = epsilon_kmeans
+        self.Phi = cp.array(Phi)
+        self.Phi_moe = cp.array(Phi_moe)
+        self.N = self.Z_corr.shape[1]
+        self.Pr_b = cp.array(Pr_b)
+        self.B = self.Phi.shape[0]  # number of batch variables
+        self.d = self.Z_corr.shape[0]
+        self.window_size = 3
+        self.epsilon_kmeans = epsilon_kmeans
         self.epsilon_harmony = epsilon_harmony
 
-        self.lamb            = cp.array(lamb)
-        self.sigma           = cp.array(sigma)
-        self.sigma_prior     = cp.array(sigma)
-        self.block_size      = block_size
-        self.K               = K                # number of clusters
+        self.lamb = cp.array(lamb)
+        self.sigma = cp.array(sigma)
+        self.sigma_prior = cp.array(sigma)
+        self.block_size = block_size
+        self.K = K  # number of clusters
         self.max_iter_harmony = max_iter_harmony
         self.max_iter_kmeans = max_iter_kmeans
-        self.verbose         = verbose
-        self.theta           = cp.array(theta)
+        self.verbose = verbose
+        self.theta = cp.array(theta)
 
-        self.objective_harmony        = []
-        self.objective_kmeans         = []
-        self.objective_kmeans_dist    = []
+        self.objective_harmony = []
+        self.objective_kmeans = []
+        self.objective_kmeans_dist = []
         self.objective_kmeans_entropy = []
-        self.objective_kmeans_cross   = []
-        self.kmeans_rounds  = []
+        self.objective_kmeans_cross = []
+        self.kmeans_rounds = []
 
         self.allocate_buffers()
         self.init_cluster()
         self.harmonize(self.max_iter_harmony, self.verbose)
 
     def result(self):
         return self.Z_corr
 
     def allocate_buffers(self):
         self._scale_dist = cp.zeros((self.K, self.N))
-        self.dist_mat    = cp.zeros((self.K, self.N))
-        self.O           = cp.zeros((self.K, self.B))
-        self.E           = cp.zeros((self.K, self.B))
-        self.W           = cp.zeros((self.B + 1, self.d))
-        self.Phi_Rk      = cp.zeros((self.B + 1, self.N))
+        self.dist_mat = cp.zeros((self.K, self.N))
+        self.O = cp.zeros((self.K, self.B))
+        self.E = cp.zeros((self.K, self.B))
+        self.W = cp.zeros((self.B + 1, self.d))
+        self.Phi_Rk = cp.zeros((self.B + 1, self.N))
 
     def init_cluster(self):
         # Start with cluster centroids
-        kmeans_obj= KMeans(n_clusters= self.K, init='k-means++').fit(self.Z_cos.T)
+        kmeans_obj = KMeans(n_clusters=self.K, init="k-means++").fit(self.Z_cos.T)
         self.Y = kmeans_obj.cluster_centers_.T
         # (1) Normalize
         self.Y = self.Y / cp.linalg.norm(self.Y, ord=2, axis=0)
         # (2) Assign cluster probabilities
         self.dist_mat = 2 * (1 - cp.dot(self.Y.T, self.Z_cos))
         self.R = -self.dist_mat
-        self.R = self.R / self.sigma[:,None]
-        self.R -= cp.max(self.R, axis = 0)
+        self.R = self.R / self.sigma[:, None]
+        self.R -= cp.max(self.R, axis=0)
         self.R = cp.exp(self.R)
-        self.R = self.R / cp.sum(self.R, axis = 0)
+        self.R = self.R / cp.sum(self.R, axis=0)
         # (3) Batch diversity statistics
         self.E = cp.outer(cp.sum(self.R, axis=1), self.Pr_b)
-        self.O = cp.inner(self.R , self.Phi)
+        self.O = cp.inner(self.R, self.Phi)
         self.compute_objective()
         # Save results
         self.objective_harmony.append(self.objective_kmeans[-1])
 
     def compute_objective(self):
         kmeans_error = cp.sum(cp.multiply(self.R, self.dist_mat))
         # Entropy
-        _entropy = cp.sum(safe_entropy(self.R) * self.sigma[:,cp.newaxis])
+        _entropy = cp.sum(safe_entropy(self.R) * self.sigma[:, cp.newaxis])
         # Cross Entropy
-        x = (self.R * self.sigma[:,cp.newaxis])
-        y = cp.tile(self.theta[:,cp.newaxis], self.K).T
+        x = self.R * self.sigma[:, cp.newaxis]
+        y = cp.tile(self.theta[:, cp.newaxis], self.K).T
         z = cp.log((self.O + 1) / (self.E + 1))
         w = cp.dot(y * z, self.Phi)
         _cross_entropy = cp.sum(x * w)
         # Save results
         self.objective_kmeans.append(kmeans_error + _entropy + _cross_entropy)
         self.objective_kmeans_dist.append(kmeans_error)
         self.objective_kmeans_entropy.append(_entropy)
@@ -228,24 +251,30 @@
             if verbose:
                 logger.info("Iteration {} of {}".format(i, iter_harmony))
             # STEP 1: Clustering
             self.cluster()
             # STEP 2: Regress out covariates
             # self.moe_correct_ridge()
             self.Z_cos, self.Z_corr, self.W, self.Phi_Rk = moe_correct_ridge(
-                self.Z_orig, self.Z_cos, self.Z_corr, self.R, self.W, self.K,
-                self.Phi_Rk, self.Phi_moe, self.lamb
+                self.Z_orig,
+                self.Z_cos,
+                self.Z_corr,
+                self.R,
+                self.W,
+                self.K,
+                self.Phi_Rk,
+                self.Phi_moe,
+                self.lamb,
             )
             # STEP 3: Check for convergence
             converged = self.check_convergence(1)
             if converged:
                 if verbose:
                     logger.info(
-                        "Converged after {} iteration{}"
-                        .format(i, 's' if i > 1 else '')
+                        "Converged after {} iteration{}".format(i, "s" if i > 1 else "")
                     )
                 break
         if verbose and not converged:
             logger.info("Stopped before convergence")
         return 0
 
     def cluster(self):
@@ -270,39 +299,38 @@
                     break
         self.kmeans_rounds.append(i)
         self.objective_harmony.append(self.objective_kmeans[-1])
         return 0
 
     def update_R(self):
         self._scale_dist = -self.dist_mat
-        self._scale_dist = self._scale_dist / self.sigma[:,None]
+        self._scale_dist = self._scale_dist / self.sigma[:, None]
         self._scale_dist -= cp.max(self._scale_dist, axis=0)
         self._scale_dist = cp.exp(self._scale_dist)
         # Update cells in blocks
         update_order = cp.arange(self.N)
         cp.random.shuffle(update_order)
         n_blocks = cp.ceil(1 / self.block_size).astype(int)
         blocks = cp.array_split(update_order, int(n_blocks))
         for b in blocks:
             # STEP 1: Remove cells
-            self.E -= cp.outer(cp.sum(self.R[:,b], axis=1), self.Pr_b)
-            self.O -= cp.dot(self.R[:,b], self.Phi[:,b].T)
+            self.E -= cp.outer(cp.sum(self.R[:, b], axis=1), self.Pr_b)
+            self.O -= cp.dot(self.R[:, b], self.Phi[:, b].T)
             # STEP 2: Recompute R for removed cells
-            self.R[:,b] = self._scale_dist[:,b]
-            self.R[:,b] = cp.multiply(
-                self.R[:,b],
+            self.R[:, b] = self._scale_dist[:, b]
+            self.R[:, b] = cp.multiply(
+                self.R[:, b],
                 cp.dot(
-                    cp.power((self.E + 1) / (self.O + 1), self.theta),
-                    self.Phi[:,b]
-                )
+                    cp.power((self.E + 1) / (self.O + 1), self.theta), self.Phi[:, b]
+                ),
             )
-            self.R[:,b] = self.R[:,b] / cp.linalg.norm(self.R[:,b], ord=1, axis=0)
+            self.R[:, b] = self.R[:, b] / cp.linalg.norm(self.R[:, b], ord=1, axis=0)
             # STEP 3: Put cells back
-            self.E += cp.outer(cp.sum(self.R[:,b], axis=1), self.Pr_b)
-            self.O += cp.dot(self.R[:,b], self.Phi[:,b].T)
+            self.E += cp.outer(cp.sum(self.R[:, b], axis=1), self.Pr_b)
+            self.O += cp.dot(self.R[:, b], self.Phi[:, b].T)
         return 0
 
     def check_convergence(self, i_type):
         obj_old = 0.0
         obj_new = 0.0
         # Clustering, compute new window mean
         if i_type == 0:
@@ -324,17 +352,18 @@
 
 
 def safe_entropy(x: cp.array):
     y = cp.multiply(x, cp.log(x))
     y[~cp.isfinite(y)] = 0.0
     return y
 
+
 def moe_correct_ridge(Z_orig, Z_cos, Z_corr, R, W, K, Phi_Rk, Phi_moe, lamb):
     Z_corr = Z_orig.copy()
     for i in range(K):
-        Phi_Rk = cp.multiply(Phi_moe, R[i,:])
+        Phi_Rk = cp.multiply(Phi_moe, R[i, :])
         x = cp.dot(Phi_Rk, Phi_moe.T) + lamb
         W = cp.dot(cp.dot(cp.linalg.inv(x), Phi_Rk), Z_orig.T)
-        W[0,:] = 0 # do not remove the intercept
+        W[0, :] = 0  # do not remove the intercept
         Z_corr -= cp.dot(W.T, Phi_Rk)
     Z_cos = Z_corr / cp.linalg.norm(Z_corr, ord=2, axis=0)
     return Z_cos, Z_corr, W, Phi_Rk
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_harmony_integrate.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def harmony_integrate(
     adata: AnnData,
     key: str,
     basis: str = "X_pca",
     adjusted_basis: str = "X_pca_harmony",
     **kwargs,
-)-> None:
+) -> None:
     """
     Use harmonypy to integrate different experiments.
     Harmony is an algorithm for integrating single-cell
     data from multiple experiments. This function uses the python
     gpu-computing based port of Harmony, to integrate single-cell data
     stored in an AnnData object. As Harmony works by adjusting the
     principal components, this function should be run after performing
@@ -39,10 +39,11 @@
     -------
         Updates adata with the field ``adata.obsm[adjusted_basis]``, \
         containing principal components adjusted by Harmony such that \
         different experiments are integrated.
     
     """
     from . import _harmonpy_gpu
+
     harmony_out = _harmonpy_gpu.run_harmony(adata.obsm[basis], adata.obs, key, **kwargs)
 
     adata.obsm[adjusted_basis] = harmony_out.Z_corr.T.get()
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_pca.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_pca.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,111 +3,119 @@
 from typing import Optional
 
 from scipy.sparse import issparse
 import warnings
 import math
 import numpy as np
 
-def pca(adata: AnnData, 
-        layer:str = None, 
-        n_comps:int = 50,
-        zero_center:bool = True,
-        use_highly_variable: Optional[bool] = None,
-        chunked:bool = False,
-        chunk_size:int = None)-> None:
+
+def pca(
+    adata: AnnData,
+    layer: str = None,
+    n_comps: int = 50,
+    zero_center: bool = True,
+    use_highly_variable: Optional[bool] = None,
+    chunked: bool = False,
+    chunk_size: int = None,
+) -> None:
     """
     Performs PCA using the cuML decomposition function for the :class:`~anndata.AnnData` object.
-    
+
     Parameters
     ----------
         adata
             annData object
-        
+
         layer
             If provided, use `adata.layers[layer]` for expression values instead of `adata.X`.
 
         n_comps
             Number of principal components to compute. Defaults to 50
-        
+
         zero_center
             If `True`, compute standard PCA from covariance matrix.
             If `False`, omit zero-centering variables
-        
+
         use_highly_variable
             Whether to use highly variable genes only, stored in
             `.var['highly_variable']`.
             By default uses them if they have been determined beforehand.
-            
+
         chunked
             If `True`, perform an incremental PCA on segments of `chunk_size`.
             The incremental PCA automatically zero centers and ignores settings of
             `random_seed` and `svd_solver`. If `False`, perform a full PCA.
-            
+
         chunk_size
             Number of observations to include in each chunk.
             Required if `chunked=True` was passed.
-    
+
     Returns
     --------
         adds fields to `adata`:
-        
+
             `.obsm['X_pca']`
-                    PCA representation of data.  
+                    PCA representation of data.
             `.varm['PCs']`
                     The principal components containing the loadings.
             `.uns['pca']['variance_ratio']`
                     Ratio of explained variance.
             `.uns['pca']['variance']`
                     Explained variance, equivalent to the eigenvalues of the
                     covariance matrix.
     """
 
-    if use_highly_variable is True and 'highly_variable' not in adata.var.keys():
+    if use_highly_variable is True and "highly_variable" not in adata.var.keys():
         raise ValueError(
-            'Did not find adata.var[\'highly_variable\']. '
-            'Either your data already only consists of highly-variable genes '
-            'or consider running `highly_variable_genes` first.'
+            "Did not find adata.var['highly_variable']. "
+            "Either your data already only consists of highly-variable genes "
+            "or consider running `highly_variable_genes` first."
         )
 
     X = adata.layers[layer] if layer is not None else adata.X
 
     if use_highly_variable is None:
-        use_highly_variable = True if 'highly_variable' in adata.var.keys() else False
+        use_highly_variable = True if "highly_variable" in adata.var.keys() else False
 
     if use_highly_variable:
-        X = X[:, adata.var['highly_variable']]
+        X = X[:, adata.var["highly_variable"]]
 
     if issparse(X) and zero_center:
         warnings.warn(
             "Your Countmatrix seems to be sparse, this can lead to a massive performance penalty.",
             UserWarning,
         )
-        
+
     if chunked:
         from cuml.decomposition import IncrementalPCA
 
         X_pca = np.zeros((X.shape[0], n_comps), X.dtype)
 
-        pca_func = IncrementalPCA(n_components=n_comps, output_type="numpy",batch_size=chunk_size)
+        pca_func = IncrementalPCA(
+            n_components=n_comps, output_type="numpy", batch_size=chunk_size
+        )
         pca_func.fit(X)
 
         n_batches = math.ceil(X.shape[0] / chunk_size)
         for batch in range(n_batches):
             start_idx = batch * chunk_size
             stop_idx = min(batch * chunk_size + chunk_size, X.shape[0])
-            chunk = X[start_idx:stop_idx,:]
+            chunk = X[start_idx:stop_idx, :]
             chunk = chunk.toarray() if issparse(chunk) else chunk
             X_pca[start_idx:stop_idx] = pca_func.transform(chunk)
     elif zero_center:
         pca_func = PCA(n_components=n_comps, output_type="numpy")
-        X_pca= pca_func.fit_transform(X)
-    
+        X_pca = pca_func.fit_transform(X)
+
     elif not zero_center:
         pca_func = TruncatedSVD(n_components=n_comps, output_type="numpy")
         X_pca = pca_func.fit_transform(X)
     adata.obsm["X_pca"] = X_pca
-    adata.uns['pca'] ={'variance':pca_func.explained_variance_, 'variance_ratio':pca_func.explained_variance_ratio_}
+    adata.uns["pca"] = {
+        "variance": pca_func.explained_variance_,
+        "variance_ratio": pca_func.explained_variance_ratio_,
+    }
     if use_highly_variable:
-        adata.varm['PCs'] = np.zeros(shape=(adata.n_vars, n_comps))
-        adata.varm['PCs'][adata.var['highly_variable']] = pca_func.components_.T
+        adata.varm["PCs"] = np.zeros(shape=(adata.n_vars, n_comps))
+        adata.varm["PCs"][adata.var["highly_variable"]] = pca_func.components_.T
     else:
-        adata.varm['PCs'] = pca_func.components_.T
+        adata.varm["PCs"] = pca_func.components_.T
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_pymde.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_pymde.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 from anndata import AnnData
 from typing import Optional, Literal
 import pandas as pd
 
+
 def mde(
     adata: AnnData,
     device: Optional[Literal["cpu", "cuda"]] = None,
     n_neighbors: int = 15,
-    n_pcs:int = None,
-    use_rep:str = None,
+    n_pcs: int = None,
+    use_rep: str = None,
     **kwargs,
 ) -> None:
     """
     Util to run :func:`pymde.preserve_neighbors` for visualization of single cell embeddings.
 
     Parameters
     ----------
         adata
             Annotated data matrix.
         device
             Whether to run on cpu or gpu ("cuda"). If None, tries to run on gpu if available.
         n_neighbors
-            use this many neighbors  
+            use this many neighbors
         n_pcs
-            use this many PCs    
+            use this many PCs
         use_rep
             use this obsm keys (defaults to `X_pca`)
         kwargs
             Keyword args to :func:`pymde.preserve_neighbors`
 
     Returns
     -------
         Updates `adata` with the following fields.
-        
+
             **X_mde** : `np.ndarray` (`adata.obs`, dtype `float`)
                 X_mde coordinates of data.
-        
+
     Notes
     -----
         This function adapted from scvi-tools.
         The appropriateness of use of visualization of high-dimensional spaces in single-
         cell omics remains an open research questions. See:
         Chari, Tara, Joeyta Banerjee, and Lior Pachter. "The specious art of single-cell genomics." bioRxiv (2021).
         If you use this function in your research please cite:
         Agrawal, Akshay, Alnur Ali, and Stephen Boyd. "Minimum-distortion embedding." arXiv preprint arXiv:2103.02559 (2021).
     """
     try:
         import torch
         import pymde
     except ImportError:
         raise ImportError("Please install pymde package via `pip install pymde`")
-        
+
     if use_rep == None:
         data = adata.obsm["X_pca"]
     else:
         data = adata.obsm[use_rep]
-        
+
     if isinstance(data, pd.DataFrame):
         data = data.values
     if n_pcs is not None:
-        data = data[:,:n_pcs]
-    
+        data = data[:, :n_pcs]
+
     device = "cpu" if not torch.cuda.is_available() else "cuda"
     _kwargs = dict(
         embedding_dim=2,
         constraint=pymde.Standardized(),
         repulsive_fraction=0.7,
         verbose=False,
         device=device,
@@ -73,8 +74,8 @@
 
     emb = pymde.preserve_neighbors(data, **_kwargs).embed(verbose=_kwargs["verbose"])
 
     if isinstance(emb, torch.Tensor):
         emb = emb.cpu().numpy()
         torch.cuda.empty_cache()
 
-    adata.obsm["X_mde"] = emb    
+    adata.obsm["X_mde"] = emb
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,62 +2,59 @@
 from anndata import AnnData
 import numpy as np
 import pandas as pd
 import warnings
 from typing import Iterable, Union, Optional, Literal
 
 
-def _select_groups(labels, groups_order_subset='all'):
+def _select_groups(labels, groups_order_subset="all"):
     groups_order = labels.cat.categories
     groups_masks = np.zeros(
         (len(labels.cat.categories), len(labels.cat.codes)), dtype=bool
     )
     for iname, name in enumerate(labels.cat.categories):
         # if the name is not found, fallback to index retrieval
         if labels.cat.categories[iname] in labels.cat.codes:
             mask = labels.cat.categories[iname] == labels.cat.codes
         else:
             mask = iname == labels.cat.codes
         groups_masks[iname] = mask.values
     groups_ids = list(range(len(groups_order)))
-    if groups_order_subset != 'all':
+    if groups_order_subset != "all":
         groups_ids = []
         for name in groups_order_subset:
-            groups_ids.append(
-                np.where(name == labels.cat.categories)[0]
-            )
+            groups_ids.append(np.where(name == labels.cat.categories)[0])
         if len(groups_ids) == 0:
             # fallback to index retrieval
             groups_ids = np.where(
                 np.in1d(
                     np.arange(len(labels.cat.categories)).astype(str),
                     np.array(groups_order_subset),
                 )
             )[0]
         groups_ids = [groups_id.item() for groups_id in groups_ids]
-        if len(groups_ids) >2:    
+        if len(groups_ids) > 2:
             groups_ids = np.sort(groups_ids)
         groups_masks = groups_masks[groups_ids]
         groups_order_subset = labels.cat.categories[groups_ids].to_numpy()
     else:
         groups_order_subset = groups_order.to_numpy()
     return groups_order_subset, groups_masks
 
 
 def rank_genes_groups_logreg(
     adata: AnnData,
-    groupby:str,  
-    groups:Union[Literal['all'], Iterable[str]]="all",
-    use_raw:bool = None,
-    reference:str='rest',
-    n_genes:int = None,
-    layer:str= None,
+    groupby: str,
+    groups: Union[Literal["all"], Iterable[str]] = "all",
+    use_raw: bool = None,
+    reference: str = "rest",
+    n_genes: int = None,
+    layer: str = None,
     **kwds,
-)-> None:
-
+) -> None:
     """
     Rank genes for characterizing groups.
 
     Parameters
     ----------
         adata
             Annotated data matrix.
@@ -85,135 +82,132 @@
                 Structured array to be indexed by group id storing the gene
                 names. Ordered according to scores.
 
             **scores** : structured `np.ndarray` (`.uns['rank_genes_groups']`)
                 Structured array to be indexed by group id storing the z-score
                 underlying the computation of a p-value for each gene for each
                 group. Ordered according to scores.
-                
+
             **pvals** : structured `np.ndarray` (`.uns['rank_genes_groups']`)
                 p-values.
 
             **pvals_adj** : structured `np.ndarray` (`.uns['rank_genes_groups']`)
                 Corrected p-values.
     """
 
     #### Wherever we see "adata.obs[groupby], we should just replace w/ the groups"
-        
+
     # for clarity, rename variable
-    if groups == 'all' or groups == None:
-        groups_order = 'all'
+    if groups == "all" or groups == None:
+        groups_order = "all"
     elif isinstance(groups, (str, int)):
-        raise ValueError('Specify a sequence of groups')
+        raise ValueError("Specify a sequence of groups")
     else:
         groups_order = list(groups)
         if isinstance(groups_order[0], int):
             groups_order = [str(n) for n in groups_order]
-        if reference != 'rest' and reference not in set(groups_order):
+        if reference != "rest" and reference not in set(groups_order):
             groups_order += [reference]
     labels = pd.Series(adata.obs[groupby]).reset_index(drop="True")
-    if (
-        reference != 'rest'
-        and reference not in set(labels.cat.categories)
-    ):
+    if reference != "rest" and reference not in set(labels.cat.categories):
         cats = labels.cat.categories.tolist()
         raise ValueError(
-            f'reference = {reference} needs to be one of groupby = {cats}.'
+            f"reference = {reference} needs to be one of groupby = {cats}."
         )
 
     groups_order, groups_masks = _select_groups(labels, groups_order)
-    
-    if layer and use_raw== True:
+
+    if layer and use_raw == True:
         raise ValueError("Cannot specify `layer` and have `use_raw=True`.")
     elif layer:
         X = adata.layers[layer]
         var_names = adata.var_names
     elif use_raw == None and adata.raw:
         print("defaulting to using `.raw`")
         X = adata.raw.X
         var_names = adata.raw.var_names
     elif use_raw == True:
         X = adata.raw.X
         var_names = adata.raw.var_names
     else:
         X = adata.X
         var_names = adata.var_names
-    
+
     # for clarity, rename variable
     n_genes_user = n_genes
     # make sure indices are not OoB in case there are less genes than n_genes
     if n_genes == None or n_genes_user > X.shape[1]:
         n_genes_user = X.shape[1]
     # in the following, n_genes is simply another name for the total number of genes
 
-
     n_groups = groups_masks.shape[0]
     ns = np.zeros(n_groups, dtype=int)
     for imask, mask in enumerate(groups_masks):
         ns[imask] = np.where(mask)[0].size
-    if reference != 'rest':
+    if reference != "rest":
         reference = np.where(groups_order == reference)[0][0]
     reference_indices = cp.arange(X.shape[1], dtype=int)
 
     rankings_gene_scores = []
     rankings_gene_names = []
 
     # Perform LogReg
-        
+
     # if reference is not set, then the groups listed will be compared to the rest
     # if reference is set, then the groups listed will be compared only to the other groups listed
     refname = reference
     from cuml.linear_model import LogisticRegression
+
     reference = groups_order[0]
     if len(groups) == 1:
-        raise Exception('Cannot perform logistic regression on a single cluster.')
-        
+        raise Exception("Cannot perform logistic regression on a single cluster.")
+
     grouping_mask = labels.isin(pd.Series(groups_order))
     grouping = labels.loc[grouping_mask]
-    
+
     X = X[grouping_mask.values, :]
     # Indexing with a series causes issues, possibly segfault
-        
-    grouping_logreg = grouping.cat.codes.to_numpy().astype('float32')
+
+    grouping_logreg = grouping.cat.codes.to_numpy().astype("float32")
     uniques = np.unique(grouping_logreg)
     for idx, cat in enumerate(uniques):
         grouping_logreg[np.where(grouping_logreg == cat)] = idx
 
-    
     clf = LogisticRegression(**kwds)
-    clf.fit(X, grouping_logreg)    
+    clf.fit(X, grouping_logreg)
     scores_all = cp.array(clf.coef_)
-    
-    if len(groups_order)== scores_all.shape[1]:
-        scores_all= scores_all.T
+
+    if len(groups_order) == scores_all.shape[1]:
+        scores_all = scores_all.T
     for igroup, group in enumerate(groups_order):
         if len(groups_order) <= 2:  # binary logistic regression
             scores = scores_all[0]
         else:
             scores = scores_all[igroup]
-        
+
         partition = cp.argpartition(scores, -n_genes_user)[-n_genes_user:]
         partial_indices = cp.argsort(scores[partition])[::-1]
         global_indices = reference_indices[partition][partial_indices]
-        rankings_gene_scores.append(scores[global_indices].get())  
+        rankings_gene_scores.append(scores[global_indices].get())
         rankings_gene_names.append(var_names[global_indices.get()])
         if len(groups_order) <= 2:
             break
 
     groups_order_save = [str(g) for g in groups_order]
-    if (len(groups) == 2):
+    if len(groups) == 2:
         groups_order_save = [groups_order_save[0]]
 
-    
     scores = np.rec.fromarrays(
         [n for n in rankings_gene_scores],
-        dtype=[(rn, 'float32') for rn in groups_order_save],
+        dtype=[(rn, "float32") for rn in groups_order_save],
     )
-    
+
     names = np.rec.fromarrays(
         [n for n in rankings_gene_names],
-        dtype=[(rn, 'U50') for rn in groups_order_save],
+        dtype=[(rn, "U50") for rn in groups_order_save],
     )
     adata.uns["rank_genes_groups"] = {}
-    adata.uns["rank_genes_groups"]["params"] = dict(groupby=groupby,method="logreg", reference=refname, use_raw=use_raw)
-    adata.uns["rank_genes_groups"]['scores'] = scores
-    adata.uns["rank_genes_groups"]['names'] = names
+    adata.uns["rank_genes_groups"]["params"] = dict(
+        groupby=groupby, method="logreg", reference=refname, use_raw=use_raw
+    )
+    adata.uns["rank_genes_groups"]["scores"] = scores
+    adata.uns["rank_genes_groups"]["names"] = names
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/scanpy_gpu/_tsne.py` & `rapids_singlecell-0.6.2/rapids_singlecell/scanpy_gpu/_tsne.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from anndata import AnnData
 from cuml.manifold import TSNE
 from typing import Optional
 
-def tsne(adata: AnnData, 
-         n_pcs:int = None,
-         use_rep:str= None,
-         perplexity:int = 30, 
-         early_exaggeration:int = 12,
-         learning_rate:int =200,
-         method:str = "barnes_hut",
-         metric:str = "euclidean",
-         )->None:
+
+def tsne(
+    adata: AnnData,
+    n_pcs: int = None,
+    use_rep: str = None,
+    perplexity: int = 30,
+    early_exaggeration: int = 12,
+    learning_rate: int = 200,
+    method: str = "barnes_hut",
+    metric: str = "euclidean",
+) -> None:
     """
-    Performs t-distributed stochastic neighborhood embedding (tSNE) using cuML libraray. 
+    Performs t-distributed stochastic neighborhood embedding (tSNE) using cuML libraray.
 
     Parameters
     ---------
         adata
             Annotated data matrix.
         n_pcs
             use this many PCs
@@ -25,44 +27,50 @@
         perplexity
             The perplexity is related to the number of nearest neighbors that is used
             in other manifold learning algorithms. Larger datasets usually require a larger
             perplexity. Consider selecting a value between 5 and 50. The choice is not extremely
             critical since t-SNE is quite insensitive to this parameter.
         early_exaggeration
             Controls how tight natural clusters in the original space are in the embedded space
-            and how much space will be between them. For larger values, the space between natural 
-            clusters will be larger in the embedded space. Again, the choice of this parameter is 
-            not very critical. If the cost function increases during initial optimization, the early 
+            and how much space will be between them. For larger values, the space between natural
+            clusters will be larger in the embedded space. Again, the choice of this parameter is
+            not very critical. If the cost function increases during initial optimization, the early
             exaggeration factor or the learning rate might be too high.
         learning_rate
-            Note that the R-package “Rtsne” and cuML uses a default of 200. The learning rate can be 
-            a critical parameter. It should be between 100 and 1000. If the cost function increases 
-            during initial optimization, the early exaggeration factor or the learning rate might 
-            be too high. If the cost function gets stuck in a bad local minimum increasing the 
+            Note that the R-package “Rtsne” and cuML uses a default of 200. The learning rate can be
+            a critical parameter. It should be between 100 and 1000. If the cost function increases
+            during initial optimization, the early exaggeration factor or the learning rate might
+            be too high. If the cost function gets stuck in a bad local minimum increasing the
             learning rate helps sometimes.
         method
             'barnes_hut' and 'fft' are fast approximations. 'exact' is more accurate but slower.
         metric
-            Distance metric to use. Supported distances are ['l1, 'cityblock', 'manhattan', 'euclidean', 
+            Distance metric to use. Supported distances are ['l1, 'cityblock', 'manhattan', 'euclidean',
             'l2', 'sqeuclidean', 'minkowski', 'chebyshev', 'cosine', 'correlation']
 
     Returns
     -------
         Updates `adata` with the following fields.
-        
+
             **X_tsne** : `np.ndarray` (`adata.obs`, dtype `float`)
                 tSNE coordinates of data.
     """
     if use_rep == None:
         data = adata.obsm["X_pca"]
     else:
         data = adata.obsm[use_rep]
     if n_pcs is not None:
-        data = data[:,:n_pcs]
-    adata.obsm['X_tsne'] = TSNE(perplexity=perplexity, early_exaggeration=early_exaggeration,learning_rate=learning_rate,method=method,metric = metric).fit_transform(data)
+        data = data[:, :n_pcs]
+    adata.obsm["X_tsne"] = TSNE(
+        perplexity=perplexity,
+        early_exaggeration=early_exaggeration,
+        learning_rate=learning_rate,
+        method=method,
+        metric=metric,
+    ).fit_transform(data)
     adata.uns["tsne"] = {
         "params": {
             k: v
             for k, v in {
                 "perplexity": perplexity,
                 "early_exaggeration": early_exaggeration,
                 "learning_rate": learning_rate,
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_autocorr.py` & `rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_autocorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 from scipy import sparse
 import cupy as cp
 from ._moransi import _morans_I_cupy
 from ._gearysc import _gearys_C_cupy
 from ._utils import _p_value_calc
 from statsmodels.stats.multitest import multipletests
 
+
 def spatial_autocorr(
     adata: AnnData,
     connectivity_key: str = "spatial_connectivities",
-    genes: Union[str, Sequence[str],None] = None,
+    genes: Union[str, Sequence[str], None] = None,
     mode: Literal["moran", "geary"] = "moran",
     transformation: bool = True,
-    n_perms: Union[int,None]= None,
+    n_perms: Union[int, None] = None,
     two_tailed: bool = False,
-    corr_method: Union[str,None] = "fdr_bh",
-    layer: Union[str,None] = None,
+    corr_method: Union[str, None] = "fdr_bh",
+    layer: Union[str, None] = None,
     use_raw: bool = False,
-    use_sparse:bool = False,
+    use_sparse: bool = False,
     copy: bool = False,
 ) -> Optional[pd.DataFrame]:
     """
     Calculate spatial autocorrelation for genes in an AnnData object.
 
     This function computes spatial autocorrelation scores (Moran's I or Geary's C) for each gene in an AnnData object. 
     The function also calculates p-values and corrected p-values for multiple testing.
@@ -70,61 +71,67 @@
             If True, return the results as a DataFrame instead of storing them in `adata.uns`, by default False.
 
     Returns
     -------
             DataFrame containing the autocorrelation scores, p-values, and corrected p-values for each gene. \
             If `copy` is False, the results are stored in `adata.uns` and None is returned.
     """
-    
+
     if genes is None:
         if "highly_variable" in adata.var:
             genes = adata[:, adata.var["highly_variable"]].var_names.values
         else:
             genes = adata.var_names.values
     if isinstance(genes, str):
-        genes= [genes]
+        genes = [genes]
     if use_raw:
         if adata.raw is None:
-            raise AttributeError("No `.raw` attribute found. Try specifying `use_raw=False`.")
+            raise AttributeError(
+                "No `.raw` attribute found. Try specifying `use_raw=False`."
+            )
         genes = list(set(genes) & set(adata.raw.var_names))
         vals = adata.raw[:, genes].X
     else:
         if layer:
-            vals =  adata[:, genes].layers["layer"]
+            vals = adata[:, genes].layers["layer"]
         else:
-            vals =  adata[:, genes].X
+            vals = adata[:, genes].X
     # create Adj-Matrix
     adj_matrix = adata.obsp[connectivity_key]
-    adj_matrix_cupy = cp.sparse.csr_matrix(adj_matrix,dtype=cp.float32)
-    
+    adj_matrix_cupy = cp.sparse.csr_matrix(adj_matrix, dtype=cp.float32)
+
     if transformation:  # row-normalize
         row_sums = adj_matrix_cupy.sum(axis=1).reshape(-1, 1)
         non_zero_rows = row_sums != 0
         row_sums[non_zero_rows] = 1.0 / row_sums[non_zero_rows]
-        adj_matrix_cupy = adj_matrix_cupy.multiply(cp.sparse.csr_matrix(row_sums)) 
-        
+        adj_matrix_cupy = adj_matrix_cupy.multiply(cp.sparse.csr_matrix(row_sums))
+
     params = {"two_tailed": two_tailed}
 
-    #check sparse:
+    # check sparse:
     if use_sparse:
         vals = sparse.csr_matrix(vals)
         data = cp.sparse.csr_matrix(vals)
     else:
         if sparse.issparse(vals):
             vals = vals.toarray()
         data = cp.array(vals)
     # Run Spartial Autocorr
     if mode == "moran":
-        score, score_perms = _morans_I_cupy(data,adj_matrix_cupy,n_permutations=n_perms)
+        score, score_perms = _morans_I_cupy(
+            data, adj_matrix_cupy, n_permutations=n_perms
+        )
         params["stat"] = "I"
         params["expected"] = -1.0 / (adata.shape[0] - 1)  # expected score
         params["ascending"] = False
         params["mode"] = "moranI"
-    elif mode =="geary":
-        score, score_perms = _gearys_C_cupy(data,adj_matrix_cupy,n_permutations=n_perms)
+    elif mode == "geary":
+        score, score_perms = _gearys_C_cupy(
+            data, adj_matrix_cupy, n_permutations=n_perms
+        )
         params["stat"] = "C"
         params["expected"] = 1.0
         params["ascending"] = True
         params["mode"] = "gearyC"
     else:
         raise NotImplementedError(f"Mode `{mode}` is not yet implemented.")
     g = sparse.csr_matrix(adj_matrix_cupy.get())
@@ -133,14 +140,16 @@
     with np.errstate(divide="ignore"):
         pval_results = _p_value_calc(score, score_perms, g, params)
 
     df = pd.DataFrame({params["stat"]: score, **pval_results}, index=genes)
 
     if corr_method is not None:
         for pv in filter(lambda x: "pval" in x, df.columns):
-            _, pvals_adj, _, _ = multipletests(df[pv].values, alpha=0.05, method=corr_method)
+            _, pvals_adj, _, _ = multipletests(
+                df[pv].values, alpha=0.05, method=corr_method
+            )
             df[f"{pv}_{corr_method}"] = pvals_adj
 
     df.sort_values(by=params["stat"], ascending=params["ascending"], inplace=True)
     if copy:
         return df
     adata.uns[params["mode"]] = df
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_gearysc.py` & `rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_gearysc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import cupy as cp
 import math
 
 
-kernel_gearys_C_num_dense = '''
+kernel_gearys_C_num_dense = r"""
 extern "C" __global__ void gearys_C_num_dense(const float* data, 
 const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, const float* adj_matrix_data, 
 float* num, int n_samples, int n_features) {
     int f = blockIdx.x * blockDim.x + threadIdx.x;
     int i = blockIdx.y * blockDim.y + threadIdx.y;
 
     if (i >= n_samples || f >= n_features) {
@@ -19,119 +19,157 @@
     for (int k = k_start; k < k_end; ++k) {
         int j = adj_matrix_col_ind[k];
         float edge_weight = adj_matrix_data[k];
         float diff_sq = (data[i * n_features + f] - data[j * n_features + f]) * (data[i * n_features + f] - data[j * n_features + f]);
         atomicAdd(&num[f], edge_weight * diff_sq);
     }
 }
-'''
+"""
 
 
 def _gearys_C_cupy_dense(data, adj_matrix_cupy, n_permutations=100):
     n_samples, n_features = data.shape
     # Calculate the numerator for Geary's C
     num = cp.zeros(n_features, dtype=cp.float32)
-    num_kernel = cp.RawKernel(kernel_gearys_C_num_dense, 'gearys_C_num_dense')
-    
+    num_kernel = cp.RawKernel(kernel_gearys_C_num_dense, "gearys_C_num_dense")
+
     block_size = 8
     fg = int(math.ceil(n_features / block_size))
     sg = int(math.ceil(n_samples / block_size))
-    grid_size = (fg, sg,1)
-    num_kernel(grid_size, 
-               (block_size, block_size,1), 
-               (data, adj_matrix_cupy.indptr, adj_matrix_cupy.indices, 
-                adj_matrix_cupy.data, num, n_samples, n_features))
+    grid_size = (fg, sg, 1)
+    num_kernel(
+        grid_size,
+        (block_size, block_size, 1),
+        (
+            data,
+            adj_matrix_cupy.indptr,
+            adj_matrix_cupy.indices,
+            adj_matrix_cupy.data,
+            num,
+            n_samples,
+            n_features,
+        ),
+    )
     # Calculate the denominator for Geary's C
     gene_mean = data.mean(axis=0).ravel()
     preden = cp.sum((data - gene_mean) ** 2, axis=0)
     den = 2 * adj_matrix_cupy.sum() * preden
-    
+
     # Calculate Geary's C
     gearys_C = (n_samples - 1) * num / den
-    
+
     # Calculate p-values using permutation tests
     if n_permutations:
         gearys_C_permutations = cp.zeros((n_permutations, n_features), dtype=cp.float32)
         for p in range(n_permutations):
             idx_shuffle = cp.random.permutation(adj_matrix_cupy.shape[0])
-            adj_matrix_permuted = adj_matrix_cupy[idx_shuffle,:]
+            adj_matrix_permuted = adj_matrix_cupy[idx_shuffle, :]
             num_permuted = cp.zeros(n_features, dtype=data.dtype)
-            num_kernel(grid_size, 
-                       (block_size, block_size,1), 
-                       (data, adj_matrix_permuted.indptr, adj_matrix_permuted.indices, 
-                        adj_matrix_permuted.data, num_permuted, n_samples, n_features))
-            #den_permuted = 2 * adj_matrix_permuted.sum() * preden
-            gearys_C_permutations[p,:] = (n_samples - 1) * num_permuted / den
+            num_kernel(
+                grid_size,
+                (block_size, block_size, 1),
+                (
+                    data,
+                    adj_matrix_permuted.indptr,
+                    adj_matrix_permuted.indices,
+                    adj_matrix_permuted.data,
+                    num_permuted,
+                    n_samples,
+                    n_features,
+                ),
+            )
+            # den_permuted = 2 * adj_matrix_permuted.sum() * preden
+            gearys_C_permutations[p, :] = (n_samples - 1) * num_permuted / den
             cp.cuda.Stream.null.synchronize()
     else:
         gearys_C_permutations = None
     return gearys_C, gearys_C_permutations
 
+
 def _gearys_C_cupy_sparse(data, adj_matrix_cupy, n_permutations=100):
     n_samples, n_features = data.shape
-        
+
     # Calculate the denominator for Geary's C
     gene_mean = data.mean(axis=0).ravel()
     preden = cp.sum((data - gene_mean) ** 2, axis=0)
-    den = 2 * adj_matrix_cupy.sum() * preden    
-    
+    den = 2 * adj_matrix_cupy.sum() * preden
+
     # Calculate the numerator for Geary's C
     data = data.tocsc()
     num = cp.zeros(n_features, dtype=data.dtype)
     block_size = 8
     sg = int(math.ceil(n_samples / block_size))
-    num_kernel = cp.RawKernel(kernel_gearys_C_num_dense, 'gearys_C_num_dense')
+    num_kernel = cp.RawKernel(kernel_gearys_C_num_dense, "gearys_C_num_dense")
     batchsize = 1000
     n_batches = math.ceil(n_features / batchsize)
     for batch in range(n_batches):
         start_idx = batch * batchsize
         stop_idx = min(batch * batchsize + batchsize, n_features)
-        data_block = data[:,start_idx:stop_idx].toarray()
+        data_block = data[:, start_idx:stop_idx].toarray()
         num_block = cp.zeros(data_block.shape[1], dtype=data.dtype)
         fg = int(math.ceil(data_block.shape[1] / block_size))
         grid_size = (fg, sg, 1)
 
-        num_kernel(grid_size, 
-                   (block_size, block_size, 1), 
-                   (data_block, adj_matrix_cupy.indptr, adj_matrix_cupy.indices, 
-                    adj_matrix_cupy.data, num_block, n_samples, data_block.shape[1]))
+        num_kernel(
+            grid_size,
+            (block_size, block_size, 1),
+            (
+                data_block,
+                adj_matrix_cupy.indptr,
+                adj_matrix_cupy.indices,
+                adj_matrix_cupy.data,
+                num_block,
+                n_samples,
+                data_block.shape[1],
+            ),
+        )
         num[start_idx:stop_idx] = num_block
         cp.cuda.Stream.null.synchronize()
-       
+
     # Calculate Geary's C
     gearys_C = (n_samples - 1) * num / den
-    
+
     # Calculate p-values using permutation tests
     if n_permutations:
         gearys_C_permutations = cp.zeros((n_permutations, n_features), dtype=cp.float32)
         for p in range(n_permutations):
             idx_shuffle = cp.random.permutation(adj_matrix_cupy.shape[0])
-            adj_matrix_permuted = adj_matrix_cupy[idx_shuffle,:]
+            adj_matrix_permuted = adj_matrix_cupy[idx_shuffle, :]
             num_permuted = cp.zeros(n_features, dtype=data.dtype)
             for batch in range(n_batches):
                 start_idx = batch * batchsize
                 stop_idx = min(batch * batchsize + batchsize, n_features)
-                data_block = data[:,start_idx:stop_idx].toarray()
+                data_block = data[:, start_idx:stop_idx].toarray()
                 num_block = cp.zeros(data_block.shape[1], dtype=data.dtype)
                 fg = int(math.ceil(data_block.shape[1] / block_size))
                 grid_size = (fg, sg, 1)
 
-                num_kernel(grid_size, 
-                           (block_size, block_size, 1), 
-                           (data_block, adj_matrix_permuted.indptr, adj_matrix_permuted.indices, 
-                            adj_matrix_permuted.data, num_block, n_samples, data_block.shape[1]))
-                num_permuted[start_idx:stop_idx] = num_block            
+                num_kernel(
+                    grid_size,
+                    (block_size, block_size, 1),
+                    (
+                        data_block,
+                        adj_matrix_permuted.indptr,
+                        adj_matrix_permuted.indices,
+                        adj_matrix_permuted.data,
+                        num_block,
+                        n_samples,
+                        data_block.shape[1],
+                    ),
+                )
+                num_permuted[start_idx:stop_idx] = num_block
 
-            #den_permuted = 2 * adj_matrix_permuted.sum() * preden
-            gearys_C_permutations[p,:] = (n_samples - 1) * num_permuted / den
+            # den_permuted = 2 * adj_matrix_permuted.sum() * preden
+            gearys_C_permutations[p, :] = (n_samples - 1) * num_permuted / den
             cp.cuda.Stream.null.synchronize()
     else:
         gearys_C_permutations = None
     return gearys_C, gearys_C_permutations
 
+
 def _gearys_C_cupy(data, adj_matrix_cupy, n_permutations=100):
     if cp.sparse.isspmatrix_csr(data):
         return _gearys_C_cupy_sparse(data, adj_matrix_cupy, n_permutations)
     elif isinstance(data, cp.ndarray):
         return _gearys_C_cupy_dense(data, adj_matrix_cupy, n_permutations)
     else:
         raise ValueError("Datatype not supported")
```

### Comparing `rapids_singlecell-0.6.1/rapids_singlecell/squidpy_gpu/_moransi.py` & `rapids_singlecell-0.6.2/rapids_singlecell/squidpy_gpu/_moransi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import cupy as cp
 import math
 
-kernel_morans_I_num_dense = '''
+kernel_morans_I_num_dense = r"""
 extern "C" __global__
 void morans_I_num_dense(const float* data_centered, const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, 
 const float* adj_matrix_data, float* num, int n_samples, int n_features) {
     int f = blockIdx.x * blockDim.x + threadIdx.x;
     int i = blockIdx.y * blockDim.y + threadIdx.y;
 
     if (i >= n_samples || f >= n_features) {
@@ -18,109 +18,147 @@
     for (int k = k_start; k < k_end; ++k) {
         int j = adj_matrix_col_ind[k];
         float edge_weight = (adj_matrix_data[k]);
         float product = data_centered[i * n_features + f] * data_centered[j * n_features + f];
         atomicAdd(&num[f], edge_weight * product);
     }
 }
-'''
+"""
+
 
 def _morans_I_cupy_dense(data, adj_matrix_cupy, n_permutations=100):
     n_samples, n_features = data.shape
     data_centered_cupy = data - data.mean(axis=0)
 
     # Calculate the numerator and denominator for Moran's I
     num = cp.zeros(n_features, dtype=cp.float32)
     block_size = 8
     fg = int(math.ceil(n_features / block_size))
     sg = int(math.ceil(n_samples / block_size))
     grid_size = (fg, sg, 1)
 
-    num_kernel = cp.RawKernel(kernel_morans_I_num_dense, 'morans_I_num_dense')
-    num_kernel(grid_size, 
-               (block_size, block_size, 1), 
-               (data_centered_cupy, adj_matrix_cupy.indptr, adj_matrix_cupy.indices, 
-                adj_matrix_cupy.data, num, n_samples, n_features))
-    den = cp.sum(data_centered_cupy ** 2, axis=0)
+    num_kernel = cp.RawKernel(kernel_morans_I_num_dense, "morans_I_num_dense")
+    num_kernel(
+        grid_size,
+        (block_size, block_size, 1),
+        (
+            data_centered_cupy,
+            adj_matrix_cupy.indptr,
+            adj_matrix_cupy.indices,
+            adj_matrix_cupy.data,
+            num,
+            n_samples,
+            n_features,
+        ),
+    )
+    den = cp.sum(data_centered_cupy**2, axis=0)
     morans_I = num / den
     # Calculate p-values using permutation tests
     if n_permutations:
         morans_I_permutations = cp.zeros((n_permutations, n_features), dtype=cp.float32)
         for p in range(n_permutations):
             idx_shuffle = cp.random.permutation(adj_matrix_cupy.shape[0])
-            adj_matrix_permuted = adj_matrix_cupy[idx_shuffle,:]
+            adj_matrix_permuted = adj_matrix_cupy[idx_shuffle, :]
             num_permuted = cp.zeros(n_features, dtype=cp.float32)
-            num_kernel(grid_size, 
-                       (block_size, block_size, 1), 
-                       (data_centered_cupy, adj_matrix_permuted.indptr, adj_matrix_permuted.indices, 
-                       adj_matrix_permuted.data, num_permuted, n_samples, n_features))
-            morans_I_permutations[p,:] = num_permuted / den
+            num_kernel(
+                grid_size,
+                (block_size, block_size, 1),
+                (
+                    data_centered_cupy,
+                    adj_matrix_permuted.indptr,
+                    adj_matrix_permuted.indices,
+                    adj_matrix_permuted.data,
+                    num_permuted,
+                    n_samples,
+                    n_features,
+                ),
+            )
+            morans_I_permutations[p, :] = num_permuted / den
             cp.cuda.Stream.null.synchronize()
     else:
-        morans_I_permutations=None
+        morans_I_permutations = None
     return morans_I, morans_I_permutations
 
+
 def _morans_I_cupy_sparse(data, adj_matrix_cupy, n_permutations=100):
     n_samples, n_features = data.shape
     data_mean = data.mean(axis=0).ravel()
 
     # Calculate den
-    den = cp.sum((data- data_mean) ** 2, axis=0)
-    
+    den = cp.sum((data - data_mean) ** 2, axis=0)
+
     # Calculate the numerator and denominator for Moran's I
     data = data.tocsc()
     num = cp.zeros(n_features, dtype=data.dtype)
     block_size = 8
-    
+
     sg = int(math.ceil(n_samples / block_size))
-    
-    num_kernel = cp.RawKernel(kernel_morans_I_num_dense, 'morans_I_num_dense')
+
+    num_kernel = cp.RawKernel(kernel_morans_I_num_dense, "morans_I_num_dense")
     batchsize = 1000
     n_batches = math.ceil(n_features / batchsize)
     for batch in range(n_batches):
         start_idx = batch * batchsize
         stop_idx = min(batch * batchsize + batchsize, n_features)
-        data_centered_cupy = data[:,start_idx:stop_idx].toarray()
-        data_centered_cupy = data_centered_cupy-data_mean[start_idx:stop_idx]
+        data_centered_cupy = data[:, start_idx:stop_idx].toarray()
+        data_centered_cupy = data_centered_cupy - data_mean[start_idx:stop_idx]
         num_block = cp.zeros(data_centered_cupy.shape[1], dtype=data.dtype)
         fg = int(math.ceil(data_centered_cupy.shape[1] / block_size))
         grid_size = (fg, sg, 1)
 
-        num_kernel(grid_size, 
-                   (block_size, block_size, 1), 
-                   (data_centered_cupy, adj_matrix_cupy.indptr, adj_matrix_cupy.indices, 
-                    adj_matrix_cupy.data, num_block, n_samples, data_centered_cupy.shape[1]))
+        num_kernel(
+            grid_size,
+            (block_size, block_size, 1),
+            (
+                data_centered_cupy,
+                adj_matrix_cupy.indptr,
+                adj_matrix_cupy.indices,
+                adj_matrix_cupy.data,
+                num_block,
+                n_samples,
+                data_centered_cupy.shape[1],
+            ),
+        )
         num[start_idx:stop_idx] = num_block
         cp.cuda.Stream.null.synchronize()
-    
+
     morans_I = num / den
     # Calculate p-values using permutation tests
     if n_permutations:
         morans_I_permutations = cp.zeros((n_permutations, n_features), dtype=cp.float32)
         for p in range(n_permutations):
             idx_shuffle = cp.random.permutation(adj_matrix_cupy.shape[0])
-            adj_matrix_permuted = adj_matrix_cupy[idx_shuffle,:]
+            adj_matrix_permuted = adj_matrix_cupy[idx_shuffle, :]
             num_permuted = cp.zeros(n_features, dtype=data.dtype)
             for batch in range(n_batches):
                 start_idx = batch * batchsize
                 stop_idx = min(batch * batchsize + batchsize, n_features)
-                data_centered_cupy = data[:,start_idx:stop_idx].toarray()
-                data_centered_cupy = data_centered_cupy-data_mean[start_idx:stop_idx]
+                data_centered_cupy = data[:, start_idx:stop_idx].toarray()
+                data_centered_cupy = data_centered_cupy - data_mean[start_idx:stop_idx]
                 num_block = cp.zeros(data_centered_cupy.shape[1], dtype=data.dtype)
                 fg = int(math.ceil(data_centered_cupy.shape[1] / block_size))
                 grid_size = (fg, sg, 1)
-                num_kernel(grid_size, 
-                           (block_size, block_size, 1), 
-                           (data_centered_cupy, adj_matrix_permuted.indptr, adj_matrix_permuted.indices, 
-                            adj_matrix_permuted.data, num_block, n_samples, data_centered_cupy.shape[1]))
+                num_kernel(
+                    grid_size,
+                    (block_size, block_size, 1),
+                    (
+                        data_centered_cupy,
+                        adj_matrix_permuted.indptr,
+                        adj_matrix_permuted.indices,
+                        adj_matrix_permuted.data,
+                        num_block,
+                        n_samples,
+                        data_centered_cupy.shape[1],
+                    ),
+                )
                 num_permuted[start_idx:stop_idx] = num_block
                 cp.cuda.Stream.null.synchronize()
-            morans_I_permutations[p,:] = num_permuted / den
+            morans_I_permutations[p, :] = num_permuted / den
     else:
-        morans_I_permutations=None
+        morans_I_permutations = None
     return morans_I, morans_I_permutations
 
 
 def _morans_I_cupy(data, adj_matrix_cupy, n_permutations=100):
     if cp.sparse.isspmatrix_csr(data):
         return _morans_I_cupy_sparse(data, adj_matrix_cupy, n_permutations)
     elif isinstance(data, cp.ndarray):
```

### Comparing `rapids_singlecell-0.6.1/PKG-INFO` & `rapids_singlecell-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids_singlecell
-Version: 0.6.1
+Version: 0.6.2
 Summary: running single cell analysis on Nvidia GPUs
 Author: Severin Dicks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: decoupler>=1.3.2
@@ -34,15 +34,15 @@
 This repository offers some tools to make analyses of single cell datasets faster by running them on the GPU. 
 The functions are analogous versions of functions that can be found within [scanpy](https://github.com/scverse/scanpy) from the Theis lab or functions from [rapids-single-cell-examples](https://github.com/clara-parabricks/rapids-single-cell-examples) created by the Nvidia RAPIDS team. Most functions are kept close to the original code to ensure compatibility. My aim with this repository was to use the speedup that GPU computing offers and combine it with the ease of use from scanpy.
 
 ## Installation
 ### Conda
 The easiest way to install *rapids-singlecell* is to use one of the *yaml* file provided in the [conda](https://github.com/Intron7/rapids_singlecell/tree/main/conda) folder. These *yaml* files install everything needed to run the example notbooks and get you started.
 ```
-conda env create -f conda/rsc_rapids_22.12.yml
+conda env create -f conda/rsc_rapids_23.04.yml
 # or
 mamba env create -f conda/rsc_rapids_23.02.yml
 ```
 ### PyPI
 As of version 0.4.0 *rapids-singlecell* is now on PyPI.
 ```
 pip install rapids-singlecell
```

