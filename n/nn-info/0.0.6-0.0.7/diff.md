# Comparing `tmp/nn_info-0.0.6.tar.gz` & `tmp/nn_info-0.0.7.tar.gz`

## Comparing `nn_info-0.0.6.tar` & `nn_info-0.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0   635751 2020-02-02 00:00:00.000000 nn_info-0.0.6/src/.ipynb_checkpoints/examples_notebook-checkpoint.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nn_info-0.0.6/src/nn_info/__init__.py
--rw-r--r--   0        0        0     8665 2020-02-02 00:00:00.000000 nn_info-0.0.6/src/nn_info/estimators.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 nn_info-0.0.6/src/nn_info/theory.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 nn_info-0.0.6/LICENSE
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 nn_info-0.0.6/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 nn_info-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nn_info-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0   635751 2020-02-02 00:00:00.000000 nn_info-0.0.7/src/.ipynb_checkpoints/examples_notebook-checkpoint.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nn_info-0.0.7/src/nn_info/__init__.py
+-rw-r--r--   0        0        0     8667 2020-02-02 00:00:00.000000 nn_info-0.0.7/src/nn_info/estimators.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 nn_info-0.0.7/src/nn_info/theory.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 nn_info-0.0.7/LICENSE
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 nn_info-0.0.7/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 nn_info-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nn_info-0.0.7/PKG-INFO
```

### Comparing `nn_info-0.0.6/src/.ipynb_checkpoints/examples_notebook-checkpoint.ipynb` & `nn_info-0.0.7/src/.ipynb_checkpoints/examples_notebook-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `nn_info-0.0.6/src/nn_info/estimators.py` & `nn_info-0.0.7/src/nn_info/estimators.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from numpy.random import choice
 import sympy
 
 
 
 #%%
 
-def BannMI(tpl, measure = 'MI', k = 15, unit='bits', prior='empiric'):
+def BannMI(tpl, measure = 'MI', k = 15, unit='bits', prior='empiric', estimate='mean'):
     
     """
     Bayesian nearest neighbor ratio estimation for mutual information
     and Kullback-Leibler divergences, as proposed in
     Schmidt et al., 2023, soon to come...
     In particular, we recommend BannMI for dependency analysis 
-    of phosphoproteomic data (protein-protein-interactions)
+    of phosphoproteomic data (multivariate protein-protein-interactions)
     The algorithm was inspired by NMI (see function)
     """
     
     X = np.array(tpl[0])
     Y = np.array(tpl[1])
     
     if X.ndim == 1:
@@ -42,15 +42,15 @@
     n2 = 2*n
 
 
     both = np.concatenate((p, q))
     # shuffle data such that neighbors are mixed in case of identical values
     permut = choice(n2,n2,replace = False)
     both[permut]
-   
+
     
     label = np.concatenate((np.zeros(n), np.ones(n)))
     label[permut]
     nbrs = NearestNeighbors(n_neighbors=k).fit(both)
     indices = nbrs.kneighbors(p, return_distance=False)
 
     q_neighbors = np.sum(label[indices], axis=1)
@@ -74,30 +74,33 @@
     else:
         b = prior
         a = prior
 
     a_new = a + c
     b_new = b + k - c
 
-    theta = (a_new)/(a_new + b_new) 
+    if estimate == 'mean':
+        theta = (a_new)/(a_new + b_new)
+    elif estimate == 'mode':
+        theta = (a_new + 1)/(a_new + b_new + 2)
     ratio = theta/(1-theta)
     
     if unit == 'bits':
         res = np.mean(np.log2(ratio))
     elif unit == 'nats':
         res = np.mean(np.log(ratio))
     else:
         print('please select nats or bits as unit')
     
     return max(res, 0.)
 
 
 #%%
     
-def WMI(tpl, measure = 'KLD', k = 5, unit='nats', epsilon=False):
+def WMI(tpl, measure = 'KLD', k = 5, unit='nats', eps=False):
     
     """
     Erstimation of (multivariate) differential Kullback-Leibler Divergence
     via nearest neighbor distances as proposed in 
     Wang, Q. et al. (2009). Divergence Estimation for Multidimensional
     Densities Via k-Nearest-Neighbor Distances. IEEE Transactions of
     Information Theory, 55(5), 2392–2405.
@@ -132,15 +135,15 @@
     Xnbrs = NearestNeighbors(n_neighbors= k + 1).fit(p)
     Ynbrs = NearestNeighbors(n_neighbors= k).fit(q)
     Xdistances, indices = Xnbrs.kneighbors(p, return_distance=True)
     Ydistances, indices = Ynbrs.kneighbors(p, return_distance=True)
     xdist = Xdistances[:,k]
     ydist = Ydistances[:,k-1]
     
-    if epsilon:
+    if eps:
         xdist[xdist==0]=np.finfo(float).eps
         ydist[ydist==0]=np.finfo(float).eps
             
     px = k/(xdist**d*(n-1))
     py = k/(ydist**d*n)
     
     if unit == 'bits':
@@ -237,89 +240,81 @@
         res = np.mean(np.log(px))
     else:
         print('please select nats or bits as unit')
            
     return max(-res, 0.)
 
 
-#%%        
-    
-def NMI(tpl, measure = 'KLD', k=50, unit='nats', epsilon=True, reverse=True):
+
+#%%
+
+def NMI(tpl, k=50, eps=True, measure = 'KLD', algo='ball_tree', leaf=30, unit='nats'):
     
     """
     Estimation of (multivariate) Kullback-Leibler divergence 
     estimation via nearest neighbor ratios. The algorithm was proposen 
     in Noshad, M. et al. (2017). Direct estimation of information divergence
     using nearest neighbor ratios. In 2017 IEEE International Symposium
     on Information Theory (ISIT 2017)", pages 903 – 907, Aachen, Germany.
     Institute of Electrical and Electronics Engineers ( IEEE ).
+    The proposed f-divergence estimator is adjusted for Kullback-
+    Leibler divergence estimation (with functional '-log' as plug-in). 
+    As the nearest neighbor of a datapoint is the datapoint itself, 
+    there is no need for '+1' adjustment. Furthermore, we case discriminate
+    the ratio directly via application of max function instead of -log(ratio)
+    as in the latter case, eps would be a large number
     """
-    
+        
     X = np.array(tpl[0])
     Y = np.array(tpl[1])
-
-    # f-Divergence D(p|q)=Kullb.-Leibler Div. KLD(q|p) when f=-log
-    # to compute KLD(p|q) use reverse==True
-    if reverse:
-        Z = X.copy()
-        X = Y.copy()
-        Y = Z
     
     if X.ndim == 1:
         X = X.reshape(-1,1)
     if Y.ndim == 1:
-        Y = Y.reshape(-1,1)        
-    
+        Y = Y.reshape(-1,1)
+
     if measure == 'KLD':
         p = X
         q = Y
     
-    elif measure == 'MI':
-        #shuffle data such that dependencies disappear
+    elif measure == 'MI': 
         Y_per = Y.copy()
         np.random.shuffle(Y_per)
         p = np.hstack((X,Y))
         q = np.hstack((X,Y_per))
+        
+    n = p.shape[0]
+    d = p.shape[1] 
+    
     
-   
-    n = len(p)
-    m = len(q)
+    if eps:
+        eps = np.finfo(float).eps
+    elif eps == 'adapt':
+        eps = 1/(n*d)
 
 
-    # flexible number of neighbors according to sample size 
-    # suggested in paper: big-O(sqrt(m)) 
     if k == 'adapt':
-        k = 3*int(np.sqrt(m))
-    
-    both = np.concatenate((q,p))
-    # shuffle data such that neighbors of both distributions are considered
-    # in case of doublets
-    permut = choice(n+m,n+m,replace = False)
-    both[permut]
-    label = np.concatenate((np.ones(m), np.zeros(n)))
-    label = label[permut]
+        k = 3*int(np.sqrt(n))
 
-    nbrs = NearestNeighbors(n_neighbors=k).fit(both)
-    indices = nbrs.kneighbors(q, return_distance=False)
 
-    # count Y-neighbors of (Y_i)s
-    M = np.sum(label[indices], axis=1)
-    N = k - M
-    
-    ratio = N/(M + 1)
-    if epsilon:
-        if epsilon =='adapt':
-            epsilon = 1/(m*p.shape[1])
-        else:
-            epsilon = np.finfo(float).eps
-    
-    # here, we use max(ratio) instead of max(f(ratio)) as max(-log(0))=inf
-    ratio = np.max((ratio, epsilon*np.ones(len(ratio))), axis=0)
-    
-    if unit=='nats':
-        res = np.mean(-np.log(ratio))
+    both = np.concatenate((p, q))
+    label = np.concatenate((np.zeros(n), np.ones(n)))
+    nbrs = NearestNeighbors(n_neighbors=k, algorithm=algo, 
+                            leaf_size=leaf).fit(both)
+    indices = nbrs.kneighbors(p, return_distance=False)
+
+    # sum over q-label neighbors
+    q_neighbors = np.sum(label[indices], axis=1)
+    p_neighbors = k - q_neighbors
+    ratio = q_neighbors/p_neighbors
+    ratio[ratio < eps] = eps
+    # p dist on top
+    #ratio = 1/ratio
+        
+    if unit == 'nats':
+        res = -np.mean(np.log(ratio))
     elif unit=='bits':
-        res = np.mean(-np.log2(ratio))
+        res = -np.mean(np.log2(ratio))
     else:
         print('please select nats or bits as unit')
-    
-    return max(res,0.)
+        
+    return max(res,0.)
```

### Comparing `nn_info-0.0.6/src/nn_info/theory.py` & `nn_info-0.0.7/src/nn_info/theory.py`

 * *Files identical despite different names*

### Comparing `nn_info-0.0.6/LICENSE` & `nn_info-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nn_info-0.0.6/pyproject.toml` & `nn_info-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "nn_info"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Bettina Schmidt", email="bettina.schmidt@charite.de" },
 ]
 description = "nearest neighbor based estimators for measures of information theory"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `nn_info-0.0.6/PKG-INFO` & `nn_info-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nn_info
-Version: 0.0.6
+Version: 0.0.7
 Summary: nearest neighbor based estimators for measures of information theory
 Project-URL: Homepage, https://github.com/zuiop11/nn_info
 Project-URL: Bug Tracker, https://github.com/zuiop11/nn_info
 Author-email: Bettina Schmidt <bettina.schmidt@charite.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

