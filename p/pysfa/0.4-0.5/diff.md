# Comparing `tmp/pysfa-0.4.tar.gz` & `tmp/pysfa-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysfa-0.4.tar", last modified: Tue May  9 17:31:05 2023, max compression
+gzip compressed data, was "pysfa-0.5.tar", last modified: Wed May 10 18:20:17 2023, max compression
```

## Comparing `pysfa-0.4.tar` & `pysfa-0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 17:30:54.000000 pysfa-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-09 17:31:05.849717 pysfa-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-09 17:30:54.000000 pysfa-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/pysfa/
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/SFA.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/pysfa/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/data/41Firm.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/data/electricityFirms.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/pysfa/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-09 17:30:54.000000 pysfa-0.4/pysfa/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:31:05.849717 pysfa-0.4/pysfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 17:31:05.000000 pysfa-0.4/pysfa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 17:31:05.849717 pysfa-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-09 17:30:54.000000 pysfa-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 18:20:06.000000 pysfa-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-10 18:20:17.631670 pysfa-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-10 18:20:06.000000 pysfa-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/pysfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/SFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/pysfa/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/data/41Firm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/data/electricityFirms.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/pysfa/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-10 18:20:06.000000 pysfa-0.5/pysfa/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:17.631670 pysfa-0.5/pysfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 18:20:17.000000 pysfa-0.5/pysfa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:20:17.631670 pysfa-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-10 18:20:06.000000 pysfa-0.5/setup.py
```

### Comparing `pysfa-0.4/LICENSE` & `pysfa-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysfa-0.4/PKG-INFO` & `pysfa-0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.4
+Version: 0.5
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
 Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
@@ -47,15 +47,15 @@
 # import the data from Tim Coelli Frontier 4.1
 df = load_Tim_Coelli_frontier(x_select=['labour', 'capital'],
                               y_select=['output'])
 y = np.log(df.y)
 x = np.log(df.x)
 
 # Estimate SFA model
-res = SFA.SFA(y, x, fun=SFA.FUN_PROD, lamda0=1, method=SFA.TE_teJ)
+res = SFA.SFA(y, x, fun=SFA.FUN_PROD, method=SFA.TE_teJ)
 
 # print estimates
 print(res.get_beta())
 print(res.get_residuals())
 
 # print estimated parameters
 print(res.get_lambda())
```

### Comparing `pysfa-0.4/README.md` & `pysfa-0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # import the data from Tim Coelli Frontier 4.1
 df = load_Tim_Coelli_frontier(x_select=['labour', 'capital'],
                               y_select=['output'])
 y = np.log(df.y)
 x = np.log(df.x)
 
 # Estimate SFA model
-res = SFA.SFA(y, x, fun=SFA.FUN_PROD, lamda0=1, method=SFA.TE_teJ)
+res = SFA.SFA(y, x, fun=SFA.FUN_PROD, method=SFA.TE_teJ)
 
 # print estimates
 print(res.get_beta())
 print(res.get_residuals())
 
 # print estimated parameters
 print(res.get_lambda())
```

### Comparing `pysfa-0.4/pysfa/SFA.py` & `pysfa-0.5/pysfa/SFA.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,60 +7,77 @@
 from .utils import tools
 
 
 class SFA:
     """Stochastic frontier analysis (SFA) 
     """
 
-    def __init__(self, y, x, fun=FUN_PROD, lamda0=1, method=TE_teJ):
+    def __init__(self, y, x, fun=FUN_PROD, intercept=True, lamda0=1, method=TE_teJ):
         """SFA model
 
           Args:
               y (float) : output variable. 
               x (float) : input variables.
+              intercept (bool, optional): whether to include intercept. Defaults to True.
+              lamda0 (float, optional): initial value of lambda. Defaults to 1.
               fun (String, optional): FUN_PROD (production function) or FUN_COST (cost function). Defaults to FUN_PROD.
+              method (String, optional): TE_teJ, TE_te, or TE_teMod. Defaults to TE_teJ.
           """
         self.y, self.x = tools.assert_valid_basic_data(y, x, fun)
-        self.fun, self.lamda0, self.method = fun, lamda0, method
+        self.fun, self.intercept, self.lamda0, self.method = fun, intercept, lamda0, method
 
     def __mle(self):
 
         # initial OLS regression
-        reg = LinearRegression().fit(X=self.x, y=self.y)
-        beta0 = np.concatenate(([reg.intercept_], reg.coef_), axis=0)
-        parm = np.concatenate((beta0, [self.lamda0]), axis=0)
+        if self.intercept == False:
+            reg = LinearRegression(fit_intercept=False).fit(X=self.x, y=self.y)
+            parm = np.concatenate((reg.coef_, [self.lamda0]), axis=0)
+        elif self.intercept == True:
+            reg = LinearRegression().fit(X=self.x, y=self.y)
+            parm = np.concatenate(
+                ([reg.intercept_], reg.coef_, [self.lamda0]), axis=0)
 
         # Maximum Likelihood Estimation
         def __loglik(parm):
             ''' Log-likelihood function'''
-            N, K = len(self.x), len(self.x[0]) + 1
+            N = len(self.x)
+            if self.intercept == False:
+                K = len(self.x[0])
+            elif self.intercept == True:
+                K = len(self.x[0]) + 1
             beta0, lamda0 = parm[0:K], parm[K]
             e = self.__resfun(beta0)
             s = np.sum(e**2)/N
             z = -lamda0*e/sqrt(s)
             pz = np.maximum(norm.cdf(z), 1e-323)
             return N/2*log(pi/2) + N/2*log(s) - np.sum(np.log(pz)) + N/2.0
 
         fit = opt.minimize(__loglik, parm, method='BFGS').x
 
         # beta, residuals, lambda, sigma^2
-        K = len(self.x[0]) + 1
+        if self.intercept == False:
+            K = len(self.x[0])
+        elif self.intercept == True:
+            K = len(self.x[0]) + 1
         self.beta = fit[0:K]
         self.residuals = self.__resfun(self.beta)
         self.lamda = fit[K]
         self.sigma2 = np.sum(self.residuals ** 2)/self.residuals.shape[0]
 
         # sigma_u^2, sigma_v^2
         self.s2u = self.lamda**2 / (1+self.lamda**2) * self.sigma2
         self.s2v = self.sigma2 / (1+self.lamda**2)
 
         return self.beta, self.residuals, self.lamda, self.sigma2, self.s2u, self.s2v
 
     def __resfun(self, beta):
-        return self.y - beta[0] - np.dot(self.x, beta[1:])
+        if self.intercept == False:
+            return self.y - np.dot(self.x, beta[0:])
+        elif self.intercept == True:
+            return self.y - beta[0] - np.dot(self.x, beta[1:])
 
     def __teJ(self):
         '''Efficiencies estimates using the conditional mean approach 
             Jondrow et al. (1982, 235)'''
 
         if self.fun == FUN_COST:
             self.sign == -1
```

### Comparing `pysfa-0.4/pysfa/constant.py` & `pysfa-0.5/pysfa/constant.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.4/pysfa/data/41Firm.csv` & `pysfa-0.5/pysfa/data/41Firm.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.4/pysfa/data/electricityFirms.csv` & `pysfa-0.5/pysfa/data/electricityFirms.csv`

 * *Files identical despite different names*

### Comparing `pysfa-0.4/pysfa/dataset.py` & `pysfa-0.5/pysfa/dataset.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.4/pysfa/utils/tools.py` & `pysfa-0.5/pysfa/utils/tools.py`

 * *Files identical despite different names*

### Comparing `pysfa-0.4/pysfa.egg-info/PKG-INFO` & `pysfa-0.5/pysfa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysfa
-Version: 0.4
+Version: 0.5
 Summary: A Python Package for Stochastic Frontier Analysis
 Home-page: https://github.com/gEAPA/pySFA
 Download-URL: https://pypi.org/project/pysfa/
 Author: Sheng Dai, Zhiqiang Liao
 Author-email: sheng.dai@utu.fi
 License: MIT
 Keywords: SFA,MLE,TE
@@ -47,15 +47,15 @@
 # import the data from Tim Coelli Frontier 4.1
 df = load_Tim_Coelli_frontier(x_select=['labour', 'capital'],
                               y_select=['output'])
 y = np.log(df.y)
 x = np.log(df.x)
 
 # Estimate SFA model
-res = SFA.SFA(y, x, fun=SFA.FUN_PROD, lamda0=1, method=SFA.TE_teJ)
+res = SFA.SFA(y, x, fun=SFA.FUN_PROD, method=SFA.TE_teJ)
 
 # print estimates
 print(res.get_beta())
 print(res.get_residuals())
 
 # print estimated parameters
 print(res.get_lambda())
```

### Comparing `pysfa-0.4/setup.py` & `pysfa-0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='pysfa',
-    version='0.4',
+    version='0.5',
     description='A Python Package for Stochastic Frontier Analysis',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Sheng Dai, Zhiqiang Liao',
     author_email='sheng.dai@utu.fi',
```

