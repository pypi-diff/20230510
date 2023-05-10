# Comparing `tmp/proteus_cli-0.3.0.tar.gz` & `tmp/proteus_cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-0.3.0.tar", max compression
+gzip compressed data, was "proteus_cli-0.3.1.tar", max compression
```

## Comparing `proteus_cli-0.3.0.tar` & `proteus_cli-0.3.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1330 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/buckets/commands.py
--rw-r--r--   0        0        0     2621 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/config.py
--rw-r--r--   0        0        0        0 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0      939 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0      323 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/case/__init__.py
--rw-r--r--   0        0        0      851 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/case/cnn_pca.py
--rw-r--r--   0        0        0     3447 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/case/hm.py
--rw-r--r--   0        0        0     3054 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/case/well_model.py
--rw-r--r--   0        0        0      446 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/common/__init__.py
--rw-r--r--   0        0        0     3238 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/common/cnn_pca.py
--rw-r--r--   0        0        0     2009 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/common/hm.py
--rw-r--r--   0        0        0     1542 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/common/well_model.py
--rw-r--r--   0        0        0     2665 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/default.py
--rw-r--r--   0        0        0      418 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/step/__init__.py
--rw-r--r--   0        0        0      125 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/step/cnn_pca.py
--rw-r--r--   0        0        0     2415 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/step/hm.py
--rw-r--r--   0        0        0      128 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/config/step/well_model.py
--rw-r--r--   0        0        0      673 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    13633 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     4446 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0     8185 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/utils.py
--rw-r--r--   0        0        0      411 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     5316 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/sources/az.py
--rw-r--r--   0        0        0      871 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     2366 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     9008 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/cli/simulations/opm.py
--rw-r--r--   0        0        0      449 2023-05-08 16:47:07.486649 proteus_cli-0.3.0/logging.ini
--rw-r--r--   0        0        0     1530 2023-05-08 16:47:07.490648 proteus_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 proteus_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1330 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2621 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/config.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/case/__init__.py
+-rw-r--r--   0        0        0      958 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/case/cnn_pca.py
+-rw-r--r--   0        0        0     3447 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/case/hm.py
+-rw-r--r--   0        0        0     3054 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/case/well_model.py
+-rw-r--r--   0        0        0      446 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/common/__init__.py
+-rw-r--r--   0        0        0     3251 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/common/cnn_pca.py
+-rw-r--r--   0        0        0     2009 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/common/hm.py
+-rw-r--r--   0        0        0     1542 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/common/well_model.py
+-rw-r--r--   0        0        0     2665 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/default.py
+-rw-r--r--   0        0        0      418 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/step/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/step/cnn_pca.py
+-rw-r--r--   0        0        0     2415 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/step/hm.py
+-rw-r--r--   0        0        0      128 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/config/step/well_model.py
+-rw-r--r--   0        0        0      673 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    14707 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     4944 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0     8656 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/utils.py
+-rw-r--r--   0        0        0      411 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     6419 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0      871 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     2712 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     9158 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-05-10 18:11:47.525506 proteus_cli-0.3.1/cli/simulations/opm.py
+-rw-r--r--   0        0        0      449 2023-05-10 18:11:47.529506 proteus_cli-0.3.1/logging.ini
+-rw-r--r--   0        0        0     1530 2023-05-10 18:11:47.529506 proteus_cli-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 proteus_cli-0.3.1/PKG-INFO
```

### Comparing `proteus_cli-0.3.0/cli/__init__.py` & `proteus_cli-0.3.1/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/api/decorators.py` & `proteus_cli-0.3.1/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/api/hooks.py` & `proteus_cli-0.3.1/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/buckets/commands.py` & `proteus_cli-0.3.1/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/config.py` & `proteus_cli-0.3.1/cli/config.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/commands.py` & `proteus_cli-0.3.1/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/__init__.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/case/cnn_pca.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/case/cnn_pca.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,22 @@
         List all cases and its steps to generate the .GRDECL iterator
 
         Args: -
 
         Returns:
             iterator: the list of steps to preprocess
         """
-
+        mapping = [*filter(lambda x: x["name"] == "LITHO_INPUT", self._get_mapping())]
         return (
             {
                 "input": [
                     f'{case["root"]}/SIMULATION_{case["number"]}.GRDECL',
                 ],
                 "output": [f'{case["root"]}/litho.h5'],
                 "preprocessing": "export_litho",
                 "case": case["number"],
                 "keep": True,
                 "additional_info": {"get_mapping": self._get_mapping},
             }
             for case in self.cases
-            if "BASE_CASE" not in str(case["root"])
+            if len(mapping) > 0 and "BASE_CASE" not in str(case["root"])
         )
```

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/case/hm.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/case/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/case/well_model.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/case/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/common/cnn_pca.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/common/cnn_pca.py`

 * *Files 20% similar despite different names*

```diff
@@ -56,51 +56,51 @@
 
         Args: -
 
         Returns:
             iterator: the list of steps to preprocess
         """
 
-        def _get_dat_files():
-            return filter(
-                lambda f: f["name"].lower() not in ["litho", "actnum"],
-                self._get_mapping(),
-            )
-
+        mapping = [*filter(lambda x: x["name"] not in ["LITHO_INPUT", "ACTNUM"], self._get_mapping())]
         return iter(
             [
                 {
-                    "input": [f'{f.get("source")}.dat' for f in _get_dat_files()],
-                    "output": [f'{f["name"].lower()}.h5' for f in _get_dat_files()],
+                    "input": [RequiredFilePath(f'{f.get("source") or f.get("name")}.dat') for f in mapping],
+                    "output": [f'{f["name"]}.h5' for f in mapping],
                     "preprocessing": "export_dat_properties",
                     "keep": True,
-                    "additional_info": {"get_mapping": self._get_mapping},
+                    "additional_info": {"get_mapping": lambda: mapping},
                 }
             ]
         )
 
-    # def step_4_actnum_prop(self):
-    #     """
-    #     List all cases and its steps to generate the .DATA iterator
-    #
-    #     Args: -
-    #
-    #     Returns:
-    #         iterator: the list of steps to preprocess
-    #     """
-    #     first_case = self.cases[0]
-    #     return iter(
-    #         [
-    #             {
-    #                 "input": [
-    #                     RequiredFilePath(
-    #                         f'{str(first_case["root"]).rstrip("/")}/' f"*ACTNUM.GRDECL", download_name="actnum"
-    #                     )
-    #                 ],
-    #                 "output": ["actnum.h5"],
-    #                 "preprocessing": "export_actnum",
-    #                 "case": first_case["number"],
-    #                 "keep": True,
-    #                 "additional_info": {"get_mapping": self._get_mapping},
-    #             }
-    #         ]
-    #     )
+    def step_4_actnum_prop(self):
+        """
+        List all cases and its steps to generate the .DATA iterator
+
+        Args: -
+
+        Returns:
+            iterator: the list of steps to preprocess
+        """
+        first_case = self.cases[0]
+        mapping = [*filter(lambda x: x["name"] == "ACTNUM", self._get_mapping())]
+
+        if len(mapping) == 0:
+            return iter([])
+
+        return iter(
+            [
+                {
+                    "input": [
+                        RequiredFilePath(
+                            f'{str(first_case["root"]).rstrip("/")}/' f"*ACTNUM.GRDECL", download_name="actnum"
+                        )
+                    ],
+                    "output": ["actnum.h5"],
+                    "preprocessing": "export_actnum",
+                    "case": first_case["number"],
+                    "keep": True,
+                    "additional_info": {"get_mapping": self._get_mapping},
+                }
+            ]
+        )
```

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/common/hm.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/common/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/common/well_model.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/common/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/default.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/default.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/config/step/hm.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/config/step/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-0.3.1/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 import cwrap
 import h5py
 import numpy as np
 from ecl.eclfile import EclInitFile, EclFile
 from ecl.grid import EclGrid
 from ecl.summary import EclSum
-
+from preprocessing.deck import ecl_deck
 from preprocessing.deck.runspec import preprocess as preprocess_runspec
-from preprocessing.deck.section import find_section
-from preprocessing.modular.dat import preprocess as preprocess_dat
+from preprocessing.deck.section import find_section, get_includes
+from preprocessing.modular import dat
 from preprocessing.modular.data import WellSpecsProcessor
 from preprocessing.modular.egrid import preprocess as preprocess_egrid
 from preprocessing.modular.grdecl import preprocess as preprocess_grdecl
 from preprocessing.modular.init import preprocess as preprocess_init
 from preprocessing.modular.s import WellSummaryProcessor
 from preprocessing.modular.x import preprocess as preprocess_x
+
 from .config.case.well_model import SMSPEC_WELL_KEYWORDS, SMSPEC_FIELD_KEYWORDS
 from .utils import upload_file, find_ext, find_file, get_case_info
 from ... import proteus
 
 DEFAULT_COMMON_PROPERTIES = {"max_pressure": -100000, "min_pressure": 100000}
 
 
@@ -168,15 +169,43 @@
 
     return data_file_loc, runspec_dest_loc, None
 
 
 """ Cases preprocessing """
 
 
-def export_egrid_properties(case_loc, case_dest_loc, input_src, *_):
+def export_egrid_properties(case_loc, case_dest_loc, input_src, source, *_, allow_missing_files=tuple(), base_dir=None):
+
+    if getattr(input_src, "download_name", None) == "data":
+        return _export_egrid_properties_from_data(
+            case_loc, case_dest_loc, input_src, source, *_, allow_missing_files=allow_missing_files, base_dir=base_dir
+        )
+    else:
+        return _export_egrid_properties_from_egrid(case_loc, case_dest_loc, input_src, *_)
+
+
+def _export_egrid_properties_from_data(
+    case_loc, case_dest_loc, input_src, source, *_, allow_missing_files=tuple(), base_dir=None
+):
+    def download_func(source_path, destination_path):
+        from .utils import download_file
+
+        download_file(source_path, destination_path, source)
+
+    get_includes(input_src.full_path, download_func, allow_missing_files=allow_missing_files, base_dir=base_dir)
+
+    grid = ecl_deck.extract_actnum(input_src.full_path)
+    grid_dest_loc = os.path.join(case_dest_loc, "grid.h5")
+    props = preprocess_egrid(grid)
+    write_h5_from_dict(props, grid_dest_loc)
+
+    return None, grid_dest_loc, None
+
+
+def _export_egrid_properties_from_egrid(case_loc, case_dest_loc, input_src, *_):
 
     if getattr(input_src, "full_path", None):
         grid_src_loc = getattr(input_src, "full_path", None)
     else:
         grid_src_loc = find_ext(case_loc=case_loc, ext="EGRID", required=True, one=True)
 
     grid_dest_loc = os.path.join(case_dest_loc, "grid.h5")
@@ -280,52 +309,49 @@
     case_dest_loc,
     input_src,
     source,
     cases_url,
     get_mapping,
     *args,
 ):
-    grdecl_src_loc = find_ext(case_loc=case_loc, ext="GRDECL")
-    mapping = filter(lambda x: x["name"] == "ACTNUM", get_mapping())
+    mapping = [*filter(lambda x: x["name"] == "ACTNUM", get_mapping())]
+    grdecl_src_loc = find_ext(case_loc=case_loc, ext="GRDECL", required=False, one=True)
 
-    with cwrap.open(str(grdecl_src_loc), "r") as f:
-        props = preprocess_grdecl(f, mapping)
+    if mapping and grdecl_src_loc:
+        with cwrap.open(str(grdecl_src_loc), "r") as f:
+            props = preprocess_grdecl(f, mapping)
 
-    _write_keywords_to_h5(props, case_dest_loc)
-    return grdecl_src_loc, case_dest_loc, None
+        _write_keywords_to_h5(props, case_dest_loc)
 
-
-def _extract_dat_mappings(mapping):
-    return [*filter(lambda f: f["name"].lower() not in ["litho", "actnum"], mapping)]
+    return grdecl_src_loc, case_dest_loc, None
 
 
 def export_dat_properties(
     case_loc,
     case_dest_loc,
     input_src,
     source,
     cases_url,
     get_mapping,
     *args,
 ):
-    dat_src_locs = [str(find_file(case_loc, src.split("/")[-1])) for src in input_src]
-
-    mapping = _extract_dat_mappings(get_mapping())
+    dat_src_locs = [str(find_file(case_loc, src.split("/")[-1])) for src in input_src[None]]
+    mapping = get_mapping()
 
     dat_files = {}
     for keyword in mapping:
         source = keyword.get("source", keyword["name"])
         file = next(
             filter(lambda f: f"{source}.dat" in f, dat_src_locs),
             None,
         )
         if file:
-            dat_files[keyword["name"].lower()] = file
+            dat_files[keyword["name"]] = file
 
-    props = preprocess_dat(dat_files, mapping)
+    props = dat.preprocess(dat_files, mapping)
 
     _write_keywords_to_h5(props, case_dest_loc)
 
     return dat_src_locs, case_dest_loc, None
 
 
 def _write_keywords_to_h5(props, dest_loc):
```

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/process_step.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/process_step.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,42 +60,53 @@
     if not replace and files_exist_in_bucket(outputs, bucket_url):
         return outputs
 
     if "cases/SIMULATION_" in outputs[0]:
         path_name = os.path.join(tmpdirname, "cases", f"SIMULATION_{case}")
     else:
         path_name = os.path.join(tmpdirname, "cases", f"{split}/SIMULATION_{case}") if (split and case) else tmpdirname
-    try:
-        os.makedirs(path_name)
-    except Exception:
-        pass
+    os.makedirs(path_name, exist_ok=True)
 
     # Download the required files. Keep the file if necessary
     downloaded_inputs = OrderedDict()
 
     def process_input(input):
         # Preserve RequiredFilePath with input.__class__
         source_path = getattr(input, "clone", input.__class__)(f"/{input}")
-        transformed_input, output_path = download_file(source_path, os.path.join(tmpdirname, str(input)), source)
-        transformed_input = getattr(input, "clone", lambda x: PathMeta(x, download_name=input))(transformed_input)
+        try:
+            transformed_input, output_path = download_file(source_path, os.path.join(tmpdirname, str(input)), source)
+        except FileNotFoundError:
+            transformed_input, output_path = None, None
+
+        if transformed_input is None and getattr(input, "replace_with", None) is not None:
+            transformed_input, output_path = process_input(input.replace_with)
+            transformed_input.replaces = input
+        elif transformed_input is not None:
+            transformed_input = getattr(input, "clone", lambda x: PathMeta(x, download_name=input))(transformed_input)
+        else:
+            transformed_input = input
+
         return transformed_input, output_path
 
     for transformed_input, output_path in proteus.bucket.each_item_parallel(
         total=len(inputs), items=inputs, each_item_fn=process_input, workers=download_workers
     ):
-        downloaded_inputs.setdefault(getattr(input, "download_name", transformed_input), []).append(output_path)
+        if output_path:
+            downloaded_inputs.setdefault(getattr(transformed_input, "download_name", transformed_input), []).append(
+                output_path
+            )
 
     # Process the files
     func = getattr(preprocess_functions, preprocessing_function_name)
     func_input = None
     if len(inputs) > 1:
         func_input = downloaded_inputs
     if len(inputs) == 1:
-        download_name, output_path = next(iter(downloaded_inputs.items()))
-        if len(output_path) == 1:
+        download_name, output_path = next(iter(downloaded_inputs.items()), (inputs[0], None))
+        if output_path and len(output_path) == 1:
             output_path = output_path[0]
 
         func_input = PathMeta(download_name, download_name=download_name, full_path=output_path)
 
     # Parameters not fully supported by old preprocessing configurations
     fn_args = set(inspect.getfullargspec(func).args).union(inspect.getfullargspec(func).kwonlyargs)
     if "allow_missing_files" in fn_args:
```

### Comparing `proteus_cli-0.3.0/cli/datasets/preprocessor/utils.py` & `proteus_cli-0.3.1/cli/datasets/preprocessor/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,40 +53,43 @@
             raise RuntimeError("A file path can not include more than one glob symbol ('*')")
         items_and_paths = list(source.list_contents(starts_with=prefix, ends_with=suffix))
 
         if len(items_and_paths) > 1:
             globbed_paths = ",".join(str(x) for x in items_and_paths)
             raise RuntimeError(f'"f{source_path}" defines more than one file: {globbed_paths}')
 
-        if len(items_and_paths) != 1:
+        cannot_resolve_glob = (
+            len(items_and_paths) > 1 or len(items_and_paths) == 0 and isinstance(source_path, RequiredFilePath)
+        )
+        if cannot_resolve_glob:
             raise FileNotFoundError(f'Cannot resolve glob "{source_path}"')
 
         assert len(destination_path.split("*")) in (1, 2)
 
-        glob_replacement_in_destination_path = suffix.join(
-            items_and_paths[0].path.split(prefix, 1)[1].split(suffix)[:-1]
-        )
-
-        if "*" in destination_path:
-            destination_path_parts = destination_path.split("*")
-            destination_path = (
-                destination_path_parts[0] + glob_replacement_in_destination_path + destination_path_parts[1]
+        if items_and_paths:
+            glob_replacement_in_destination_path = suffix.join(
+                items_and_paths[0].path.split(prefix, 1)[1].split(suffix)[:-1]
             )
 
-        if "*" in source_path:
-            transformed_source_path = prefix + glob_replacement_in_destination_path + suffix
-        else:
-            transformed_source_path = source_path
+            if "*" in destination_path:
+                destination_path_parts = destination_path.split("*")
+                destination_path = (
+                    destination_path_parts[0] + glob_replacement_in_destination_path + destination_path_parts[1]
+                )
+
+            if "*" in source_path:
+                transformed_source_path = prefix + glob_replacement_in_destination_path + suffix
+            else:
+                transformed_source_path = source_path
 
-        proteus.logger.info(
-            f'Glob "{source_path}" resolved to {items_and_paths[0]}. Output path rewritten to f{destination_path}'
-        )
+            proteus.logger.info(
+                f'Glob "{source_path}" resolved to {items_and_paths[0]}. Output path rewritten to f{destination_path}'
+            )
 
         items_and_paths = iter(items_and_paths)
-
     else:
         items_and_paths = source.list_contents(starts_with=source_path)
         transformed_source_path = source_path
 
     path_list = destination_path.split("/")[0:-1]
     Path("/".join(path_list)).mkdir(parents=True, exist_ok=True)
 
@@ -127,14 +130,15 @@
             os.rename(f"{destination_path}.tmp", destination_path)
 
             return transformed_source_path, destination_path
         except StopIteration:
             if isinstance(source_path, RequiredFilePath):
                 raise FileNotFoundError(f"Required file {source_path} is not found")
             proteus.logger.error(f"The following file was not found: {source_path}")
+            return None, None
 
 
 @proteus.may_insist_up_to()
 def upload_file(source_path, file_path, url):
     """
     Upload a file to proteus
 
@@ -142,21 +146,16 @@
         source_path (string): Path of the file inside proteus
         file_path (string): Path of the file in the local system
         bucket_uuid (string): Uuid of the proteus bucket
 
     Returns: -
     """
     modified = get_creation_date(file_path)
-    with open(file_path, "rb") as file_content:
-        proteus.api.post_file(url, source_path, content=file_content, modified=modified, retry=False)
-    try:
-        if not os.path.isdir(file_path):
-            os.remove(file_path)
-    except Exception:
-        pass
+    file_path = Path(file_path)
+    proteus.api.post_file(url, source_path, content=file_path, modified=modified, retry=False)
 
 
 """ Destructuring helper function of an object """
 
 
 def pluck(dict, *args):
     return (dict.get(arg, None) for arg in args)
@@ -233,21 +232,36 @@
     return r.json().get("case")
 
 
 class PathMeta(str):
     download_name = None
     cloned_from = None
     full_path = None
+    replace_with = None
+    replaces = None
 
-    def __new__(cls, value, download_name=None, cloned_from=None, full_path=None):
+    def __new__(cls, value, download_name=None, cloned_from=None, full_path=None, replace_with=None):
         path_meta = str.__new__(cls, value)
         path_meta.download_name = download_name
         path_meta.cloned_from = cloned_from
         path_meta.full_path = full_path
+        path_meta.replace_with = replace_with
         return path_meta
 
     def clone(self, value):
-        return self.__class__(value, download_name=self.download_name, cloned_from=self)
+        cloned = self.__class__(
+            value,
+            download_name=self.download_name,
+            cloned_from=self,
+            full_path=self.full_path,
+            replace_with=self.replace_with,
+        )
+        cloned.replaces = self.replaces
+        return cloned
 
 
 class RequiredFilePath(PathMeta):
     pass
+
+
+class OptionalFilePath(PathMeta):
+    pass
```

### Comparing `proteus_cli-0.3.0/cli/datasets/sources/az.py` & `proteus_cli-0.3.1/cli/datasets/sources/az.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 
 # from azure.storage.blob._models import BlobProperties as AzureBlobProperties
 from io import BytesIO
 
 from azure.storage.blob import ContainerClient
 from azure.core.credentials import AzureSasCredential
-from azure.core.exceptions import HttpResponseError
+from azure.core.exceptions import HttpResponseError, ClientAuthenticationError
 from azure.identity import DefaultAzureCredential
 
 from .common import Source, SourcedItem
 from ... import proteus
 from cli.config import config
 
 AZURE_SAS_TOKEN = config.AZURE_SAS_TOKEN
@@ -25,43 +25,72 @@
     def __init__(self, uri):
         super().__init__(uri)
         match = self.URI_re.match(uri.rstrip("/"))
         assert match is not None, f"{uri} must be an s3 URI"
         container_name = match.groupdict()["container_name"]
         storage_url = f'https://{match.groupdict()["bucket_name"]}'
 
+        auth_methods = [
+            "exclude_environment_credential",
+            "exclude_cli_credential",
+            "exclude_shared_token_cache_credential",
+            "exclude_visual_studio_code_credential",
+            "exclude_interactive_browser_credential",
+            "exclude_powershell_credential",
+            "exclude_managed_identity_credential",
+        ]
+
         if AZURE_SAS_TOKEN:
-            credential = AzureSasCredential(AZURE_SAS_TOKEN)
-        else:
-            credential = DefaultAzureCredential(exclude_managed_identity_credential=True)
-
-        self.container_client = ContainerClient(
-            storage_url,
-            credential=credential,
-            container_name=container_name,
-        )
+            self.container_client = ContainerClient(
+                storage_url,
+                credential=AzureSasCredential(AZURE_SAS_TOKEN),
+                container_name=container_name,
+            )
+            return
+
+        errors = []
+        login_successful = False
+        for auth_method in auth_methods:
+            try:
+                flags = {auth: True for auth in auth_methods}
+                flags[auth_method] = False
+                self.container_client = ContainerClient(
+                    storage_url,
+                    credential=DefaultAzureCredential(**flags),
+                    container_name=container_name,
+                )
+                self.container_client.exists()
+                login_successful = True
+                break
+            except ClientAuthenticationError as e:
+                errors.append(e)
+
+        if not login_successful:
+            for error in errors:
+                proteus.logger.error(error)
+            raise RuntimeError("Cannot authenticate into azure")
 
     @proteus.may_insist_up_to(5, 1)
     def list_contents(self, starts_with="", ends_with=None):
         bucket_uri = self.uri
         match = self.URI_re.match(bucket_uri.rstrip("/"))
         assert match is not None, f"{bucket_uri} must be an s3 URI"
         prefix = match.groupdict()["prefix"]
         try:
             for item in self.container_client.list_blobs(name_starts_with=prefix + starts_with):
                 item_name = f'/{item["name"]}'
                 assert item_name.startswith("/" + prefix + starts_with)
                 if ends_with is None or item_name.endswith(ends_with):
                     yield SourcedItem(item, item_name, self, item.size)
-        except HttpResponseError as e:
+        except HttpResponseError:
             proteus.logger.error(
                 "Missing Azure credentials to perform this operation, please "
                 "provide a SAS token or provide another authentication method on Azure"
             )
-            raise e
+            raise
 
     def open(self, reference):
         reference_path = reference.get("name")
         file_size = reference["size"]
         modified = reference["last_modified"]
 
         stream = BytesIO()
```

### Comparing `proteus_cli-0.3.0/cli/datasets/sources/common.py` & `proteus_cli-0.3.1/cli/datasets/sources/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/sources/local.py` & `proteus_cli-0.3.1/cli/datasets/sources/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,19 +35,25 @@
     @lru_cache(maxsize=50000)
     def _list_dir_files(self, source_uri):
         files = []
         by_extension = {}
         if os.path.isdir(source_uri):
             for file in os.listdir(source_uri):
                 fq_file_path = Path(os.path.join(source_uri, file))
-                files.append(fq_file_path)
-                parts = file.split(".")
-                if len(parts) == 2:
-                    extension = "." + parts[1]
-                    by_extension.setdefault(extension, []).append(fq_file_path)
+                if os.path.isdir(fq_file_path):
+                    f_files, f_by_extension = self._list_dir_files(fq_file_path)
+                    files.extend(f_files)
+                    for ext, files in f_by_extension.items():
+                        by_extension.setdefault(ext, []).extend(files)
+                else:
+                    files.append(fq_file_path)
+                    parts = file.split(".")
+                    if len(parts) == 2:
+                        extension = "." + parts[1]
+                        by_extension.setdefault(extension, []).append(fq_file_path)
 
         return files, by_extension
 
     def open(self, reference):
         stats = reference.stat()
         reference_path = str(reference)
         modified = datetime.fromtimestamp(stats.st_mtime, tz=timezone.utc)
```

### Comparing `proteus_cli-0.3.0/cli/datasets/sources/s3.py` & `proteus_cli-0.3.1/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/datasets/upload.py` & `proteus_cli-0.3.1/cli/datasets/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,30 +48,33 @@
     )
 
     dataset_version_url = f"/api/v1/datasets/{dataset_uuid}/versions"
     proteus.api.post(dataset_version_url, new_version)
 
 
 def get_total_steps(cases, workflow):
-    training_cases = [*filter(lambda c: c["group"] == "training" and c["number"] == 1, cases)]
-    if not training_cases and cases:
-        first_training_case = cases[0]
-    else:
-        first_training_case = next(iter(training_cases), None)
-    first_case_response = proteus.api.get(first_training_case.get("case_url"))
-    first_case_json = first_case_response.json().get("case")
-    initial_step = first_case_json.get("initialStep")
-    final_step = first_case_json.get("finalStep")
-    workflow = workflow.lower()
-    common_step = CommonConfigMapper[workflow].number_of_steps()
-    cases_steps = CaseConfigMapper[workflow].number_of_steps()
-    timesteps_steps = (
-        StepConfigMapper[workflow].number_of_steps() - 1 if StepConfigMapper[workflow].number_of_steps() > 0 else 0
-    )
-    return common_step + (cases_steps + timesteps_steps * (final_step - initial_step + 1)) * len(cases)
+    for case_kind in ["training", "validation", "testing"]:
+        filtered_cases = [*filter(lambda c: c["group"] == case_kind and c["number"] == 1, cases)]
+        if not filtered_cases:
+            continue
+        else:
+            first_training_case = next(iter(filtered_cases), None)
+        first_case_response = proteus.api.get(first_training_case.get("case_url"))
+        first_case_json = first_case_response.json().get("case")
+        initial_step = first_case_json.get("initialStep")
+        final_step = first_case_json.get("finalStep")
+        workflow = workflow.lower()
+        common_step = CommonConfigMapper[workflow].number_of_steps()
+        cases_steps = CaseConfigMapper[workflow].number_of_steps()
+        timesteps_steps = (
+            StepConfigMapper[workflow].number_of_steps() - 1 if StepConfigMapper[workflow].number_of_steps() > 0 else 0
+        )
+        return common_step + (cases_steps + timesteps_steps * (final_step - initial_step + 1)) * len(cases)
+
+    raise RuntimeError("No cases found to extract steps")
 
 
 def upload(
     bucket, dataset_uuid, workers=WORKERS_COUNT, replace=False, allow_missing_files=tuple(), temp_folder_override=False
 ):
     assert proteus.api.auth.access_token is not None
     set_dataset_version(dataset_uuid)
```

### Comparing `proteus_cli-0.3.0/cli/debugger/commands.py` & `proteus_cli-0.3.1/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/debugger/init_keyword_check.py` & `proteus_cli-0.3.1/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/jobs/commands.py` & `proteus_cli-0.3.1/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/jobs/list.py` & `proteus_cli-0.3.1/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/simulations/commands.py` & `proteus_cli-0.3.1/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/simulations/create.py` & `proteus_cli-0.3.1/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/simulations/dependencySolver.py` & `proteus_cli-0.3.1/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/cli/simulations/opm.py` & `proteus_cli-0.3.1/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.3.0/pyproject.toml` & `proteus_cli-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
```

### Comparing `proteus_cli-0.3.0/PKG-INFO` & `proteus_cli-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteus-cli
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
 Requires-Dist: boto3 (>=1.17.79,<2.0.0)
```

