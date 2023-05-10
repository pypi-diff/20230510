# Comparing `tmp/mktstructure-0.2.7.tar.gz` & `tmp/mktstructure-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktstructure-0.2.7.tar", last modified: Fri Apr 28 02:03:42 2023, max compression
+gzip compressed data, was "mktstructure-0.2.9.tar", last modified: Wed May 10 03:39:27 2023, max compression
```

## Comparing `mktstructure-0.2.7.tar` & `mktstructure-0.2.9.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:03:42.723733 mktstructure-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-28 02:03:38.000000 mktstructure-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 02:03:42.719733 mktstructure-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-28 02:03:38.000000 mktstructure-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:03:42.719733 mktstructure-0.2.7/mktstructure/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/cmd_download_mktdepth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:03:42.719733 mktstructure-0.2.7/mktstructure/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/bidask_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/effective_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/price_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/realized_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/measures/variance_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/request_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/trth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/trth_parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-28 02:03:38.000000 mktstructure-0.2.7/mktstructure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:03:42.719733 mktstructure-0.2.7/mktstructure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 02:03:42.000000 mktstructure-0.2.7/mktstructure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:03:42.723733 mktstructure-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-28 02:03:38.000000 mktstructure-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:39:27.335621 mktstructure-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-10 03:39:22.000000 mktstructure-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-10 03:39:27.335621 mktstructure-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-10 03:39:22.000000 mktstructure-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:39:27.335621 mktstructure-0.2.9/mktstructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/cmd_classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/cmd_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/cmd_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/cmd_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/cmd_download_mktdepth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:39:27.335621 mktstructure-0.2.9/mktstructure/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/ask_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/bid_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/bidask_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/effective_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/price_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/realized_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/scaled_depth_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/measures/variance_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/request_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/trth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/trth_parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-05-10 03:39:22.000000 mktstructure-0.2.9/mktstructure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:39:27.335621 mktstructure-0.2.9/mktstructure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-10 03:39:27.000000 mktstructure-0.2.9/mktstructure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-10 03:39:27.000000 mktstructure-0.2.9/mktstructure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:39:27.000000 mktstructure-0.2.9/mktstructure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:39:27.000000 mktstructure-0.2.9/mktstructure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:39:27.000000 mktstructure-0.2.9/mktstructure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 03:39:27.000000 mktstructure-0.2.9/mktstructure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:39:27.335621 mktstructure-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-10 03:39:22.000000 mktstructure-0.2.9/setup.py
```

### Comparing `mktstructure-0.2.7/LICENSE` & `mktstructure-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/PKG-INFO` & `mktstructure-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktstructure
-Version: 0.2.7
+Version: 0.2.9
 Summary: Download data from Refinitiv Tick History and compute some market microstructure measures.
 Home-page: https://github.com/mgao6767/mktstructure
 Author: Mingze Gao
 Author-email: mingze.gao@sydney.edu.au
 License: MIT
 Description: # mktstructure
```

### Comparing `mktstructure-0.2.7/README.md` & `mktstructure-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/cmd_classify.py` & `mktstructure-0.2.9/mktstructure/cmd_classify.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/cmd_clean.py` & `mktstructure-0.2.9/mktstructure/cmd_clean.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/cmd_compute.py` & `mktstructure-0.2.9/mktstructure/cmd_compute.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,16 +16,24 @@
     if args.out:
         fout = open(args.out, "w")
 
     for root, _, files in os.walk(args.data_dir):
         for f in files:
             # skip those unsigned ones
             # TODO: .csv vs .csv.gz
-            if "signed" not in f:
+            if ".csv" not in f:
                 continue
+            if not (
+                args.bid_slope
+                or args.ask_slope
+                or args.scaled_depth_diff_1
+                or args.scaled_depth_diff_5
+            ):
+                if "signed" not in f:
+                    continue
 
             path = os.path.join(root, f)
             ric, date = os.path.normpath(path).split(os.sep)[-2:]
             date = dt.fromisoformat(
                 date.removesuffix(".csv")
                 .removesuffix(".csv.gz")
                 .removesuffix(".signed")
@@ -49,14 +57,22 @@
                     _compute(measures.effective_spread, path, date, ric, df, fout)
                 if args.realized_spread:
                     _compute(measures.realized_spread, path, date, ric, df, fout)
                 if args.price_impact:
                     _compute(measures.price_impact, path, date, ric, df, fout)
                 if args.variance_ratio:
                     _compute(measures.variance_ratio, path, date, ric, df, fout)
+                if args.bid_slope:
+                    _compute(measures.bid_slope, path, date, ric, df, fout)
+                if args.ask_slope:
+                    _compute(measures.ask_slope, path, date, ric, df, fout)
+                if args.scaled_depth_diff_1:
+                    _compute(measures.sdd1, path, date, ric, df, fout)
+                if args.scaled_depth_diff_5:
+                    _compute(measures.sdd5, path, date, ric, df, fout)
 
     fout.close()
 
 
 def _compute(measure, path, date, ric, data, fout):
     print(f"Computing {measure.name} for {path}")
     result = measure.estimate(data)
```

### Comparing `mktstructure-0.2.7/mktstructure/cmd_download.py` & `mktstructure-0.2.9/mktstructure/cmd_download.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/cmd_download_mktdepth.py` & `mktstructure-0.2.9/mktstructure/cmd_download_mktdepth.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/main.py` & `mktstructure-0.2.9/mktstructure/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,14 +332,42 @@
     parser_compute.add_argument(
         "--variance_ratio",
         default=False,
         const=True,
         action="store_const",
         help="if set, compute the variance ratio and test statistics",
     )
+    parser_compute.add_argument(
+        "--bid_slope",
+        default=False,
+        const=True,
+        action="store_const",
+        help="if set, compute the bid slope",
+    )
+    parser_compute.add_argument(
+        "--ask_slope",
+        default=False,
+        const=True,
+        action="store_const",
+        help="if set, compute the ask slope",
+    )
+    parser_compute.add_argument(
+        "--scaled_depth_diff_1",
+        default=False,
+        const=True,
+        action="store_const",
+        help="if set, compute the scaled depth difference at the 1st level",
+    )
+    parser_compute.add_argument(
+        "--scaled_depth_diff_5",
+        default=False,
+        const=True,
+        action="store_const",
+        help="if set, compute the scaled depth difference at the 5th level",
+    )
 
     return parser
 
 
 def main():
     parser = init_argparse()
     args = parser.parse_args()
```

### Comparing `mktstructure-0.2.7/mktstructure/measures/bidask_spread.py` & `mktstructure-0.2.9/mktstructure/measures/bidask_spread.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/measures/effective_spread.py` & `mktstructure-0.2.9/mktstructure/measures/effective_spread.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/measures/price_impact.py` & `mktstructure-0.2.9/mktstructure/measures/price_impact.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/measures/realized_spread.py` & `mktstructure-0.2.9/mktstructure/measures/realized_spread.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/measures/variance_ratio.py` & `mktstructure-0.2.9/mktstructure/measures/variance_ratio.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/request_templates.py` & `mktstructure-0.2.9/mktstructure/request_templates.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/trth.py` & `mktstructure-0.2.9/mktstructure/trth.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/trth_parser.c` & `mktstructure-0.2.9/mktstructure/trth_parser.c`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure/utils.py` & `mktstructure-0.2.9/mktstructure/utils.py`

 * *Files identical despite different names*

### Comparing `mktstructure-0.2.7/mktstructure.egg-info/PKG-INFO` & `mktstructure-0.2.9/mktstructure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktstructure
-Version: 0.2.7
+Version: 0.2.9
 Summary: Download data from Refinitiv Tick History and compute some market microstructure measures.
 Home-page: https://github.com/mgao6767/mktstructure
 Author: Mingze Gao
 Author-email: mingze.gao@sydney.edu.au
 License: MIT
 Description: # mktstructure
```

### Comparing `mktstructure-0.2.7/mktstructure.egg-info/SOURCES.txt` & `mktstructure-0.2.9/mktstructure.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -15,13 +15,16 @@
 mktstructure.egg-info/PKG-INFO
 mktstructure.egg-info/SOURCES.txt
 mktstructure.egg-info/dependency_links.txt
 mktstructure.egg-info/entry_points.txt
 mktstructure.egg-info/requires.txt
 mktstructure.egg-info/top_level.txt
 mktstructure/measures/__init__.py
+mktstructure/measures/ask_slope.py
+mktstructure/measures/bid_slope.py
 mktstructure/measures/bidask_spread.py
 mktstructure/measures/effective_spread.py
 mktstructure/measures/exceptions.py
 mktstructure/measures/price_impact.py
 mktstructure/measures/realized_spread.py
+mktstructure/measures/scaled_depth_difference.py
 mktstructure/measures/variance_ratio.py
```

### Comparing `mktstructure-0.2.7/setup.py` & `mktstructure-0.2.9/setup.py`

 * *Files identical despite different names*

