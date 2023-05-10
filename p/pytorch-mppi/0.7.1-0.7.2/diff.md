# Comparing `tmp/pytorch_mppi-0.7.1.tar.gz` & `tmp/pytorch_mppi-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_mppi-0.7.1.tar", last modified: Tue May  9 02:19:42 2023, max compression
+gzip compressed data, was "pytorch_mppi-0.7.2.tar", last modified: Wed May 10 18:51:01 2023, max compression
```

## Comparing `pytorch_mppi-0.7.1.tar` & `pytorch_mppi-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 02:19:42.992123 pytorch_mppi-0.7.1/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 04:07:46.000000 pytorch_mppi-0.7.1/LICENSE.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    14016 2023-05-09 02:19:42.992123 pytorch_mppi-0.7.1/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    11944 2023-05-09 02:17:59.000000 pytorch_mppi-0.7.1/README.md
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4321 2023-05-09 02:19:29.000000 pytorch_mppi-0.7.1/pyproject.toml
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2023-05-09 02:19:42.992123 pytorch_mppi-0.7.1/setup.cfg
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 02:19:42.988123 pytorch_mppi-0.7.1/src/
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 02:19:42.988123 pytorch_mppi-0.7.1/src/pytorch_mppi/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       35 2023-02-10 05:03:49.000000 pytorch_mppi-0.7.1/src/pytorch_mppi/__init__.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    10143 2023-05-09 02:17:59.000000 pytorch_mppi-0.7.1/src/pytorch_mppi/autotune.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5596 2023-05-09 02:17:59.000000 pytorch_mppi-0.7.1/src/pytorch_mppi/autotune_global.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3641 2023-05-09 02:17:59.000000 pytorch_mppi-0.7.1/src/pytorch_mppi/autotune_qd.py
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    16444 2023-04-19 01:21:43.000000 pytorch_mppi-0.7.1/src/pytorch_mppi/mppi.py
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 02:19:42.992123 pytorch_mppi-0.7.1/src/pytorch_mppi.egg-info/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    14016 2023-05-09 02:19:42.000000 pytorch_mppi-0.7.1/src/pytorch_mppi.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      414 2023-05-09 02:19:42.000000 pytorch_mppi-0.7.1/src/pytorch_mppi.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2023-05-09 02:19:42.000000 pytorch_mppi-0.7.1/src/pytorch_mppi.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      173 2023-05-09 02:19:42.000000 pytorch_mppi-0.7.1/src/pytorch_mppi.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       13 2023-05-09 02:19:42.000000 pytorch_mppi-0.7.1/src/pytorch_mppi.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-09 02:19:42.992123 pytorch_mppi-0.7.1/tests/
--rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1491 2023-02-10 04:59:55.000000 pytorch_mppi-0.7.1/tests/test_batch_wrapper.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-10 18:51:01.031028 pytorch_mppi-0.7.2/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1075 2023-02-10 04:07:46.000000 pytorch_mppi-0.7.2/LICENSE.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    14016 2023-05-10 18:51:01.031028 pytorch_mppi-0.7.2/PKG-INFO
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    11944 2023-05-09 02:17:59.000000 pytorch_mppi-0.7.2/README.md
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     4321 2023-05-10 18:50:41.000000 pytorch_mppi-0.7.2/pyproject.toml
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       38 2023-05-10 18:51:01.031028 pytorch_mppi-0.7.2/setup.cfg
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-10 18:51:01.031028 pytorch_mppi-0.7.2/src/
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-10 18:51:01.031028 pytorch_mppi-0.7.2/src/pytorch_mppi/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       35 2023-02-10 05:03:49.000000 pytorch_mppi-0.7.2/src/pytorch_mppi/__init__.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    10215 2023-05-10 18:25:33.000000 pytorch_mppi-0.7.2/src/pytorch_mppi/autotune.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     5653 2023-05-10 18:25:33.000000 pytorch_mppi-0.7.2/src/pytorch_mppi/autotune_global.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     3641 2023-05-09 02:17:59.000000 pytorch_mppi-0.7.2/src/pytorch_mppi/autotune_qd.py
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    16444 2023-04-19 01:21:43.000000 pytorch_mppi-0.7.2/src/pytorch_mppi/mppi.py
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-10 18:51:01.031028 pytorch_mppi-0.7.2/src/pytorch_mppi.egg-info/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)    14016 2023-05-10 18:51:01.000000 pytorch_mppi-0.7.2/src/pytorch_mppi.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      414 2023-05-10 18:51:01.000000 pytorch_mppi-0.7.2/src/pytorch_mppi.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)        1 2023-05-10 18:51:01.000000 pytorch_mppi-0.7.2/src/pytorch_mppi.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)      173 2023-05-10 18:51:01.000000 pytorch_mppi-0.7.2/src/pytorch_mppi.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)       13 2023-05-10 18:51:01.000000 pytorch_mppi-0.7.2/src/pytorch_mppi.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1001) zhsh      (1001)        0 2023-05-10 18:51:01.031028 pytorch_mppi-0.7.2/tests/
+-rw-rw-r--   0 zhsh      (1001) zhsh      (1001)     1491 2023-02-10 04:59:55.000000 pytorch_mppi-0.7.2/tests/test_batch_wrapper.py
```

### Comparing `pytorch_mppi-0.7.1/LICENSE.txt` & `pytorch_mppi-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytorch_mppi-0.7.1/PKG-INFO` & `pytorch_mppi-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch_mppi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Model Predictive Path Integral (MPPI) implemented in pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `pytorch_mppi-0.7.1/README.md` & `pytorch_mppi-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pytorch_mppi-0.7.1/pyproject.toml` & `pytorch_mppi-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytorch_mppi"
-version = "0.7.1"
+version = "0.7.2"
 description = "Model Predictive Path Integral (MPPI) implemented in pytorch"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `pytorch_mppi-0.7.1/src/pytorch_mppi/autotune.py` & `pytorch_mppi-0.7.2/src/pytorch_mppi/autotune.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,16 @@
     def ensure_valid_value(self, value):
         sigma = ensure_tensor(self.d, self.dtype, value)
         sigma[sigma < self.eps] = self.eps
         return sigma
 
     def apply_parameter_value(self, value):
         sigma = self.ensure_valid_value(value)
-        self.mppi.noise_dist = MultivariateNormal(self.mppi.noise_mu, covariance_matrix=torch.diag(sigma))
+        self.mppi.noise_sigma = torch.diag(sigma)
+        self.mppi.noise_dist = MultivariateNormal(self.mppi.noise_mu, covariance_matrix=self.mppi.noise_sigma)
         self.mppi.noise_sigma_inv = torch.inverse(self.mppi.noise_sigma.detach())
 
     def get_parameter_value_from_config(self, config):
         return torch.tensor([config[f'{self.name()}{i}'] for i in range(self.mppi.nu)], dtype=self.dtype, device=self.d)
 
     def get_config_from_parameter_value(self, value):
         return {f'{self.name()}{i}': value[i].item() for i in range(self.mppi.nu)}
@@ -235,15 +236,14 @@
     eps = 0.0001
 
     def __init__(self, params_to_tune: typing.Sequence[TunableParameter],
                  evaluate_fn: typing.Callable[[], EvaluationResult], optimizer=CMAESOpt()):
         self.evaluate_fn = evaluate_fn
 
         self.params = params_to_tune
-        self.param_values = None
         self.optim = optimizer
         self.optim.tuner = self
         self.results = []
 
         self.get_parameter_values(self.params)
         self.optim.setup_optimization()
 
@@ -259,49 +259,50 @@
 
     def get_best_result(self) -> EvaluationResult:
         return min(self.results, key=lambda res: res.costs.mean().item())
 
     def log_current_result(self, res: EvaluationResult):
         with torch.no_grad():
             iteration = len(self.results)
+            kv = self.get_parameter_values(self.params)
             res = res._replace(iteration=iteration,
                                params={k: v.detach().clone() if torch.is_tensor(v) else v for k, v in
-                                       self.param_values.items()})
-            logger.info(f"i:{iteration} cost: {res.costs.mean().item()} params:{self.param_values}")
+                                       kv.items()})
+            logger.info(f"i:{iteration} cost: {res.costs.mean().item()} params:{kv}")
             self.results.append(res)
         return res
 
     def get_parameter_values(self, params_to_tune: typing.Sequence[TunableParameter]):
         # take on the assigned values to the MPPI
-        self.param_values = {p.name(): p.get_current_parameter_value() for p in params_to_tune}
+        return {p.name(): p.get_current_parameter_value() for p in params_to_tune}
 
     def flatten_params(self):
         x = []
+        kv = self.get_parameter_values(self.params)
         # TODO ensure this is the same order as define and unflatten
-        for k, v in self.param_values.items():
+        for k, v in kv.items():
             if torch.is_tensor(v):
                 x.append(v.detach().cpu().numpy())
             else:
                 x.append([v])
         x = np.concatenate(x)
         return x
 
     def unflatten_params(self, x, apply=True):
         # have to be in the same order as the flattening
-        params = {}
+        param_values = {}
         i = 0
         for p in self.params:
             raw_value = x[i:i + p.dim()]
-            params[p.name()] = p.ensure_valid_value(raw_value)
+            param_values[p.name()] = p.ensure_valid_value(raw_value)
             i += p.dim()
         if apply:
-            self.apply_parameters(params)
-        return params
+            self.apply_parameters(param_values)
+        return param_values
 
-    def apply_parameters(self, params):
+    def apply_parameters(self, param_values):
         for p in self.params:
-            p.apply_parameter_value(params[p.name()])
-        self.param_values = params
+            p.apply_parameter_value(param_values[p.name()])
 
     def config_to_params(self, config):
         """Configs are param dictionaries where each must be a scalar"""
         return {p.name(): p.get_parameter_value_from_config(config) for p in self.params}
```

### Comparing `pytorch_mppi-0.7.1/src/pytorch_mppi/autotune_global.py` & `pytorch_mppi-0.7.2/src/pytorch_mppi/autotune_global.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,17 +98,18 @@
         for p in self.params:
             assert isinstance(p, GlobalTunableParameter)
             v.extend(p.get_linearized_search_space_value(param_values))
         return np.array(v)
 
     def initial_value(self):
         init = {}
+        param_values = self.get_parameter_values(self.params)
         for p in self.params:
             assert isinstance(p, GlobalTunableParameter)
-            init.update(p.get_config_from_parameter_value(self.param_values[p.name()]))
+            init.update(p.get_config_from_parameter_value(param_values[p.name()]))
         return init
 
 
 class RayOptimizer(autotune.Optimizer):
     def __init__(self, search_alg=HyperOptSearch,
                  default_iterations=100):
         self.iterations = default_iterations
```

### Comparing `pytorch_mppi-0.7.1/src/pytorch_mppi/autotune_qd.py` & `pytorch_mppi-0.7.2/src/pytorch_mppi/autotune_qd.py`

 * *Files identical despite different names*

### Comparing `pytorch_mppi-0.7.1/src/pytorch_mppi/mppi.py` & `pytorch_mppi-0.7.2/src/pytorch_mppi/mppi.py`

 * *Files identical despite different names*

### Comparing `pytorch_mppi-0.7.1/src/pytorch_mppi.egg-info/PKG-INFO` & `pytorch_mppi-0.7.2/src/pytorch_mppi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-mppi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Model Predictive Path Integral (MPPI) implemented in pytorch
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 University of Michigan ARM Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `pytorch_mppi-0.7.1/tests/test_batch_wrapper.py` & `pytorch_mppi-0.7.2/tests/test_batch_wrapper.py`

 * *Files identical despite different names*

