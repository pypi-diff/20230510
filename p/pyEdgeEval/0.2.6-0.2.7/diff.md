# Comparing `tmp/pyEdgeEval-0.2.6.tar.gz` & `tmp/pyEdgeEval-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyEdgeEval-0.2.6.tar", last modified: Sun Nov 20 07:59:32 2022, max compression
+gzip compressed data, was "pyEdgeEval-0.2.7.tar", last modified: Wed May 10 03:26:26 2023, max compression
```

## Comparing `pyEdgeEval-0.2.6.tar` & `pyEdgeEval-0.2.7.tar`

### file list

```diff
@@ -1,121 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.383894 pyEdgeEval-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (116)     1072 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     1644 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/LICENSES.md
--rw-r--r--   0 runner    (1001) docker     (116)      136 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7088 2022-11-20 07:59:32.383894 pyEdgeEval-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6320 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.363894 pyEdgeEval-0.2.6/pyEdgeEval/
--rw-r--r--   0 runner    (1001) docker     (116)      174 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.367894 pyEdgeEval-0.2.6/pyEdgeEval/_lib/
--rw-r--r--   0 runner    (1001) docker     (116)      349 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)   838124 2022-11-20 07:59:29.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/correspond_pixels.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     2556 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/correspond_pixels.pyx
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.371894 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/
--rw-r--r--   0 runner    (1001) docker     (116)     7929 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Array.hh
--rw-r--r--   0 runner    (1001) docker     (116)     1576 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Exception.hh
--rw-r--r--   0 runner    (1001) docker     (116)    13527 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Matrix.hh
--rw-r--r--   0 runner    (1001) docker     (116)     1132 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Point.hh
--rw-r--r--   0 runner    (1001) docker     (116)     3568 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Random.hh
--rw-r--r--   0 runner    (1001) docker     (116)     7593 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Sort.hh
--rw-r--r--   0 runner    (1001) docker     (116)     4583 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/String.hh
--rw-r--r--   0 runner    (1001) docker     (116)     2612 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Timer.hh
--rw-r--r--   0 runner    (1001) docker     (116)      182 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/benms.hh
--rw-r--r--   0 runner    (1001) docker     (116)    61126 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/csa.hh
--rw-r--r--   0 runner    (1001) docker     (116)     4860 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/csa_defs.h
--rw-r--r--   0 runner    (1001) docker     (116)     4536 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/csa_types.h
--rw-r--r--   0 runner    (1001) docker     (116)      111 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/kofn.hh
--rw-r--r--   0 runner    (1001) docker     (116)      280 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/match.hh
--rw-r--r--   0 runner    (1001) docker     (116)   819335 2022-11-20 07:59:30.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/nms.cpp
--rw-r--r--   0 runner    (1001) docker     (116)     1587 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/nms.pyx
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.371894 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/
--rw-r--r--   0 runner    (1001) docker     (116)     1157 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/Exception.cc
--rw-r--r--   0 runner    (1001) docker     (116)    47460 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/Matrix.cc
--rw-r--r--   0 runner    (1001) docker     (116)     1802 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/Random.cc
--rw-r--r--   0 runner    (1001) docker     (116)     3775 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/String.cc
--rw-r--r--   0 runner    (1001) docker     (116)     2416 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/Timer.cc
--rw-r--r--   0 runner    (1001) docker     (116)     2248 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/benms.cc
--rw-r--r--   0 runner    (1001) docker     (116)      701 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/csa.cc
--rw-r--r--   0 runner    (1001) docker     (116)     1673 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/kofn.cc
--rw-r--r--   0 runner    (1001) docker     (116)    12044 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/match.cc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.375894 pyEdgeEval-0.2.6/pyEdgeEval/common/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.375894 pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/
--rw-r--r--   0 runner    (1001) docker     (116)      540 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4416 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/calculate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     5380 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/evaluate_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (116)     2337 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/io.py
--rw-r--r--   0 runner    (1001) docker     (116)     2960 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/visualize.py
--rw-r--r--   0 runner    (1001) docker     (116)     1753 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.375894 pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/
--rw-r--r--   0 runner    (1001) docker     (116)      881 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4516 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/calculate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)     2139 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/edge_decoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     1927 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/edge_encoding.py
--rw-r--r--   0 runner    (1001) docker     (116)     3896 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/evaluate_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (116)     2837 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/io.py
--rw-r--r--   0 runner    (1001) docker     (116)      737 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/options.py
--rw-r--r--   0 runner    (1001) docker     (116)     1008 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.375894 pyEdgeEval-0.2.6/pyEdgeEval/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)      353 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2135 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/datasets/bsds.py
--rw-r--r--   0 runner    (1001) docker     (116)     2150 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1450 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/datasets/cityscapes_attributes.py
--rw-r--r--   0 runner    (1001) docker     (116)     2106 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/datasets/generic_binary.py
--rw-r--r--   0 runner    (1001) docker     (116)     5892 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/datasets/otf_cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (116)     8280 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/datasets/sbd.py
--rw-r--r--   0 runner    (1001) docker     (116)     1017 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/datasets/sbd_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.379894 pyEdgeEval-0.2.6/pyEdgeEval/edge_tools/
--rw-r--r--   0 runner    (1001) docker     (116)      394 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/edge_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3497 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/edge_tools/mask2edge_loop.py
--rw-r--r--   0 runner    (1001) docker     (116)     8708 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/edge_tools/mask2edge_mp.py
--rw-r--r--   0 runner    (1001) docker     (116)     4644 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/edge_tools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.379894 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/
--rw-r--r--   0 runner    (1001) docker     (116)      360 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5637 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/base.py
--rw-r--r--   0 runner    (1001) docker     (116)      125 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/binary_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (116)     5137 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/bsds.py
--rw-r--r--   0 runner    (1001) docker     (116)     9871 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (116)     3342 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/half_cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (116)      124 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/multilabel_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (116)     3902 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/otf_cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (116)     7782 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/evaluators/sbd.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.379894 pyEdgeEval-0.2.6/pyEdgeEval/helpers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15175 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/helpers/convert_cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (116)     8247 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/helpers/convert_sbd.py
--rw-r--r--   0 runner    (1001) docker     (116)     4283 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/helpers/evaluate_bsds500.py
--rw-r--r--   0 runner    (1001) docker     (116)     8692 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/helpers/evaluate_cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (116)    11337 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/helpers/evaluate_sbd.py
--rw-r--r--   0 runner    (1001) docker     (116)      311 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/info.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.379894 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/
--rw-r--r--   0 runner    (1001) docker     (116)      101 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.383894 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/nms/
--rw-r--r--   0 runner    (1001) docker     (116)       86 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/nms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4632 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/nms/fast_nms.py
--rw-r--r--   0 runner    (1001) docker     (116)     1504 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/nms/toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.383894 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/thin/
--rw-r--r--   0 runner    (1001) docker     (116)      147 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/thin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7064 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/thin/bwmorph_thin.py
--rw-r--r--   0 runner    (1001) docker     (116)     6586 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/preprocess/thin/thin.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.383894 pyEdgeEval-0.2.6/pyEdgeEval/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      960 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2330 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/utils/convert_formats.py
--rw-r--r--   0 runner    (1001) docker     (116)     1231 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/utils/distance_transforms.py
--rw-r--r--   0 runner    (1001) docker     (116)     4089 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (116)     1019 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/utils/mat_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     2534 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (116)     7284 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (116)     3142 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.383894 pyEdgeEval-0.2.6/pyEdgeEval/visualization/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3854 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyEdgeEval/visualization/pr_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-20 07:59:32.363894 pyEdgeEval-0.2.6/pyEdgeEval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7088 2022-11-20 07:59:32.000000 pyEdgeEval-0.2.6/pyEdgeEval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3390 2022-11-20 07:59:32.000000 pyEdgeEval-0.2.6/pyEdgeEval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-20 07:59:32.000000 pyEdgeEval-0.2.6/pyEdgeEval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-20 07:59:32.000000 pyEdgeEval-0.2.6/pyEdgeEval.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-11-20 07:59:32.000000 pyEdgeEval-0.2.6/pyEdgeEval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-11-20 07:59:32.000000 pyEdgeEval-0.2.6/pyEdgeEval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      278 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-20 07:59:32.383894 pyEdgeEval-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4368 2022-11-20 07:59:02.000000 pyEdgeEval-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.267857 pyEdgeEval-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1644 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/LICENSES.md
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7088 2023-05-10 03:26:26.267857 pyEdgeEval-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6320 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.255858 pyEdgeEval-0.2.7/pyEdgeEval/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.255858 pyEdgeEval-0.2.7/pyEdgeEval/_lib/
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   838181 2023-05-10 03:26:24.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/correspond_pixels.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/correspond_pixels.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.259858 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/
+-rw-r--r--   0 runner    (1001) docker     (122)     7929 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Array.hh
+-rw-r--r--   0 runner    (1001) docker     (122)     1576 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Exception.hh
+-rw-r--r--   0 runner    (1001) docker     (122)    13527 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Matrix.hh
+-rw-r--r--   0 runner    (1001) docker     (122)     1132 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Point.hh
+-rw-r--r--   0 runner    (1001) docker     (122)     3568 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Random.hh
+-rw-r--r--   0 runner    (1001) docker     (122)     7593 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Sort.hh
+-rw-r--r--   0 runner    (1001) docker     (122)     4583 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/String.hh
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Timer.hh
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/benms.hh
+-rw-r--r--   0 runner    (1001) docker     (122)    61126 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/csa.hh
+-rw-r--r--   0 runner    (1001) docker     (122)     4860 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/csa_defs.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/csa_types.h
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/kofn.hh
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/match.hh
+-rw-r--r--   0 runner    (1001) docker     (122)   819423 2023-05-10 03:26:25.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/nms.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/nms.pyx
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.259858 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1157 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/Exception.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    47460 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/Matrix.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/Random.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/String.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/Timer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/benms.cc
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/csa.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/kofn.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    12044 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/match.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.259858 pyEdgeEval-0.2.7/pyEdgeEval/common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.259858 pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4416 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/calculate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5380 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/evaluate_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2960 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.259858 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4516 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/calculate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/edge_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1927 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/edge_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/evaluate_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2837 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.263857 pyEdgeEval-0.2.7/pyEdgeEval/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)      353 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/datasets/bsds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/datasets/cityscapes_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/datasets/generic_binary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5892 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/datasets/otf_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2337 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/datasets/sbd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/datasets/sbd_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.263857 pyEdgeEval-0.2.7/pyEdgeEval/edge_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/edge_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3562 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/edge_tools/mask2edge_loop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8708 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/edge_tools/mask2edge_mp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4644 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/edge_tools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.263857 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/binary_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5137 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/bsds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9871 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3342 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/half_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/multilabel_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/otf_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12006 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/evaluators/sbd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.263857 pyEdgeEval-0.2.7/pyEdgeEval/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15175 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/helpers/convert_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13192 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/helpers/convert_sbd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/helpers/evaluate_bsds500.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8775 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/helpers/evaluate_cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11043 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/helpers/evaluate_sbd.py
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/info.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.263857 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.263857 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/nms/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/nms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4632 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/nms/fast_nms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/nms/toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.263857 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/thin/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/thin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7064 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/thin/bwmorph_thin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6654 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/preprocess/thin/thin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.267857 pyEdgeEval-0.2.7/pyEdgeEval/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/utils/convert_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/utils/distance_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4089 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/utils/mat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2534 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.267857 pyEdgeEval-0.2.7/pyEdgeEval/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3854 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyEdgeEval/visualization/pr_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.255858 pyEdgeEval-0.2.7/pyEdgeEval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7088 2023-05-10 03:26:26.000000 pyEdgeEval-0.2.7/pyEdgeEval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3469 2023-05-10 03:26:26.000000 pyEdgeEval-0.2.7/pyEdgeEval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 03:26:26.000000 pyEdgeEval-0.2.7/pyEdgeEval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 03:26:26.000000 pyEdgeEval-0.2.7/pyEdgeEval.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-10 03:26:26.000000 pyEdgeEval-0.2.7/pyEdgeEval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-10 03:26:26.000000 pyEdgeEval-0.2.7/pyEdgeEval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 03:26:26.267857 pyEdgeEval-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4368 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 03:26:26.267857 pyEdgeEval-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/tests/test_bsds500.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3471 2023-05-10 03:26:03.000000 pyEdgeEval-0.2.7/tests/test_sbd.py
```

### Comparing `pyEdgeEval-0.2.6/LICENSE` & `pyEdgeEval-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/LICENSES.md` & `pyEdgeEval-0.2.7/LICENSES.md`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/PKG-INFO` & `pyEdgeEval-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEdgeEval
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python Edge Evaluation Tools
 Home-page: https://github.com/haruishi43/py-edge-eval
 Author: haruishi43
 Author-email: haruyaishikawa@keio.jp
 License: MIT
 Keywords: Edge Detection,Semantic Boundary Detection,Computer Vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyEdgeEval-0.2.6/README.md` & `pyEdgeEval-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/correspond_pixels.cpp` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/correspond_pixels.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "pyEdgeEval/_lib/include/Matrix.hh",
             "pyEdgeEval/_lib/include/match.hh"
@@ -37,16 +37,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -115,15 +115,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -231,15 +231,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -270,15 +270,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -594,35 +594,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1344,26 +1344,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -3612,15 +3612,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -5590,15 +5590,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -7893,15 +7893,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -7966,15 +7966,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -16169,15 +16169,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -16558,15 +16558,15 @@
  *         fmt = __Pyx_TypeInfoToFormat(type)
  */
     __pyx_t_4 = __Pyx_PyBytes_Join(__pyx_v_alignment, __pyx_v_parts); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_kp_b__23); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(1, 1487, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(1, 1487, __pyx_L1_error)
     __pyx_v_result = ((PyObject*)__pyx_t_5);
     __pyx_t_5 = 0;
 
     /* "BufferFormatFromTypeInfo":1470
  *     cdef bytes part, result
  * 
  *     if type.typegroup == 'S':             # <<<<<<<<<<<<<<
@@ -16637,15 +16637,15 @@
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = __Pyx_PyObject_FromString(__pyx_v_fmt.string); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1492, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = PyNumber_Add(__pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1492, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 1492, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 1492, __pyx_L1_error)
       __pyx_v_result = ((PyObject*)__pyx_t_4);
       __pyx_t_4 = 0;
 
       /* "BufferFormatFromTypeInfo":1490
  *     else:
  *         fmt = __Pyx_TypeInfoToFormat(type)
  *         if type.arraysize[0]:             # <<<<<<<<<<<<<<
@@ -17896,15 +17896,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_0 = PyFloat_FromDouble(0.0); if (unlikely(!__pyx_float_0_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_100_0 = PyFloat_FromDouble(100.0); if (unlikely(!__pyx_float_100_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_0075 = PyFloat_FromDouble(0.0075); if (unlikely(!__pyx_float_0_0075)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -18204,15 +18204,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pyEdgeEval___lib__correspond_pixels) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -19256,28 +19256,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -19332,18 +19332,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
@@ -19619,15 +19617,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -20433,15 +20431,15 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/correspond_pixels.pyx` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/correspond_pixels.pyx`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Array.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Array.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Exception.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Exception.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Matrix.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Matrix.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Point.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Point.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Random.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Random.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Sort.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Sort.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/String.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/String.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/Timer.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/Timer.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/csa.hh` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/csa.hh`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/csa_defs.h` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/csa_defs.h`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/include/csa_types.h` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/include/csa_types.h`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/nms.cpp` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/nms.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "pyEdgeEval/_lib/include/Matrix.hh",
             "pyEdgeEval/_lib/include/benms.hh"
@@ -35,16 +35,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -113,15 +113,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -229,15 +229,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -268,15 +268,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -592,35 +592,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1478,26 +1478,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -3313,15 +3313,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -5291,15 +5291,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -7594,15 +7594,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -7667,15 +7667,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -15870,15 +15870,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -16259,15 +16259,15 @@
  *         fmt = __Pyx_TypeInfoToFormat(type)
  */
     __pyx_t_4 = __Pyx_PyBytes_Join(__pyx_v_alignment, __pyx_v_parts); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_kp_b__23); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 1487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(1, 1487, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(1, 1487, __pyx_L1_error)
     __pyx_v_result = ((PyObject*)__pyx_t_5);
     __pyx_t_5 = 0;
 
     /* "BufferFormatFromTypeInfo":1470
  *     cdef bytes part, result
  * 
  *     if type.typegroup == 'S':             # <<<<<<<<<<<<<<
@@ -16338,15 +16338,15 @@
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_t_2 = __Pyx_PyObject_FromString(__pyx_v_fmt.string); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1492, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = PyNumber_Add(__pyx_t_5, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 1492, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 1492, __pyx_L1_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 1492, __pyx_L1_error)
       __pyx_v_result = ((PyObject*)__pyx_t_4);
       __pyx_t_4 = 0;
 
       /* "BufferFormatFromTypeInfo":1490
  *     else:
  *         fmt = __Pyx_TypeInfoToFormat(type)
  *         if type.arraysize[0]:             # <<<<<<<<<<<<<<
@@ -17594,15 +17594,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_1_01 = PyFloat_FromDouble(1.01); if (unlikely(!__pyx_float_1_01)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_5 = PyInt_FromLong(5); if (unlikely(!__pyx_int_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -17901,15 +17901,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pyEdgeEval___lib__nms) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -18852,28 +18852,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -19285,15 +19285,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -20112,15 +20112,15 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/nms.pyx` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/nms.pyx`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/Exception.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/Exception.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/Matrix.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/Matrix.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/Random.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/Random.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/String.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/String.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/Timer.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/Timer.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/benms.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/benms.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/csa.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/csa.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/kofn.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/kofn.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/_lib/src/match.cc` & `pyEdgeEval-0.2.7/pyEdgeEval/_lib/src/match.cc`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/__init__.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/calculate_metrics.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/evaluate_boundaries.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/evaluate_boundaries.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/io.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/io.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/binary_label/visualize.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/binary_label/visualize.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/metrics.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/metrics.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/__init__.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 from .io import (
     save_category_results,
     save_sample_metrics,
     save_threshold_metrics,
     save_overall_metric,
     save_pretty_metrics,
 )
+from .utils import (
+    add_ignore_pixel,
+    convert_inst_seg,
+)
 
 __all__ = [
     "calculate_metrics",
     "evaluate_boundaries_threshold",
     "binary_multilabel_decoding",
     "load_scaled_edge",
     "decode_png",
@@ -32,8 +36,10 @@
     "default_multilabel_encoding",
     "rgb_multilabel_encoding",
     "save_category_results",
     "save_sample_metrics",
     "save_threshold_metrics",
     "save_overall_metric",
     "save_pretty_metrics",
+    "add_ignore_pixel",
+    "convert_inst_seg",
 ]
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/calculate_metrics.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/calculate_metrics.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/edge_decoding.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/edge_decoding.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/edge_encoding.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/edge_encoding.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/evaluate_boundaries.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/evaluate_boundaries.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/io.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/io.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/multi_label/options.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/multi_label/options.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/common/utils.py` & `pyEdgeEval-0.2.7/pyEdgeEval/common/utils.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/datasets/bsds.py` & `pyEdgeEval-0.2.7/pyEdgeEval/datasets/bsds.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/datasets/cityscapes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/datasets/cityscapes_attributes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/datasets/cityscapes_attributes.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/datasets/generic_binary.py` & `pyEdgeEval-0.2.7/pyEdgeEval/datasets/generic_binary.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/datasets/otf_cityscapes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/datasets/otf_cityscapes.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/datasets/sbd_attributes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/datasets/sbd_attributes.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/edge_tools/mask2edge_loop.py` & `pyEdgeEval-0.2.7/pyEdgeEval/edge_tools/mask2edge_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 
 from warnings import warn
 
 import numpy as np
 
 from pyEdgeEval.preprocess import binary_thin
+
+# from pyEdgeEval.preprocess import bwmorph_thin as binary_thin
 from pyEdgeEval.utils import mask2bdry
 
 __all__ = [
     "loop_mask2edge",
     "loop_instance_mask2edge",
 ]
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/edge_tools/mask2edge_mp.py` & `pyEdgeEval-0.2.7/pyEdgeEval/edge_tools/mask2edge_mp.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/edge_tools/transforms.py` & `pyEdgeEval-0.2.7/pyEdgeEval/edge_tools/transforms.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/evaluators/base.py` & `pyEdgeEval-0.2.7/pyEdgeEval/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/evaluators/bsds.py` & `pyEdgeEval-0.2.7/pyEdgeEval/evaluators/bsds.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/evaluators/cityscapes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/evaluators/cityscapes.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/evaluators/half_cityscapes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/evaluators/half_cityscapes.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/evaluators/otf_cityscapes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/evaluators/otf_cityscapes.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/evaluators/sbd.py` & `pyEdgeEval-0.2.7/pyEdgeEval/evaluators/sbd.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,41 +35,70 @@
         "person",
         "potted plant",
         "sheep",
         "sofa",
         "train",
         "tv/monitor",
     )
-    GT_SUFFIX = ".mat"
-    PRED_SUFFIX = ".bmp"
+
+    GT_DIR = "gtEval"  # pre-processed GTs
+
+    EDGE_SUFFIX = None
+    ISEDGE_SUFFIX = None
+    RAW_EDGE_SUFFIX = "_raw_edge.png"
+    THIN_EDGE_SUFFIX = "_thin_edge.png"
+    RAW_ISEDGE_SUFFIX = "_raw_isedge.png"
+    THIN_ISEDGE_SUFFIX = "_thin_isedge.png"
+
+    SEG_SUFFIX = "_labelIds.png"
+    PRED_SUFFIX = ".png"
 
     def __init__(
         self,
         dataset_root: str,
         pred_root: str,
         split: str = "val",
-        cls_dir: str = "cls",
-        inst_dir: str = "inst",
+        thin: bool = False,
+        gt_dir=None,
         pred_suffix=None,
         **kwargs,
     ):
         self.dataset_root = dataset_root
         self.pred_root = pred_root
 
         assert split in ("val", "test")
         self.split = split
+        self.thin = thin
+        if self.thin:
+            print_log(
+                "Using `thin` mode; setting the suffix respectively",
+                logger=self._logger,
+            )
+            self.EDGE_SUFFIX = self.THIN_EDGE_SUFFIX
+            self.ISEDGE_SUFFIX = self.THIN_ISEDGE_SUFFIX
+        else:
+            print_log(
+                "Using `raw` mode; setting the suffix respectively",
+                logger=self._logger,
+            )
+            self.EDGE_SUFFIX = self.RAW_EDGE_SUFFIX
+            self.ISEDGE_SUFFIX = self.RAW_ISEDGE_SUFFIX
 
-        self.CLS_root = osp.join(
-            self.dataset_root,
-            cls_dir,
-        )
-        self.INST_root = osp.join(
-            self.dataset_root,
-            inst_dir,
-        )
+        # change dataset directory and suffix
+        if gt_dir:
+            print_log(f"changing GT_DIR to {gt_dir}", logger=self._logger)
+            self.GT_DIR = gt_dir
+        if pred_suffix:
+            print_log(
+                f"changing PRED_SUFFIX to {pred_suffix}", logger=self._logger
+            )
+            self.PRED_SUFFIX = pred_suffix
+
+        # set parameters
+        self.gtEval_root = osp.join(self.dataset_root, self.GT_DIR)
 
         if pred_suffix is not None:
             print_log(f"changed suffix to {pred_suffix}")
             self.PRED_SUFFIX = pred_suffix
 
         # we can try to load some sample names
         try:
@@ -125,32 +154,29 @@
 
             if instance_sensitive:
                 warn("Pre-SEAL mode doesn't support instance sensitive")
             self.instance_sensitive = False
         elif eval_mode == "post-seal":
             print_log("Using Post-SEAL params", logger=self._logger)
             self.max_dist = 0.02
-            self.kill_internal = False
-            self.skip_if_nonexistent = False
-            self.instance_sensitive = instance_sensitive
-        elif eval_mode == "reanno":
-            print_log(
-                "Using params for re-annotated test split", logger=self._logger
-            )
-            self.max_dist = 0.0075
-            self.kill_internal = False
-            self.skip_if_nonexistent = False
-            self.instance_sensitive = instance_sensitive
+            if instance_sensitive:
+                self.instance_sensitive = True
+                self.kill_internal = False
+                self.skip_if_nonexistent = False
+            else:
+                self.instance_sensitive = False
+                self.kill_internal = True
+                self.skip_if_nonexistent = True
         else:
             print_log("Using custom params", logger=self._logger)
             self.max_dist = max_dist
             self.kill_internal = kill_internal
             self.skip_if_nonexistent = skip_if_nonexistent
-
             self.instance_sensitive = instance_sensitive
+
         if self.kill_internal and self.instance_sensitive:
             print_log(
                 "kill_internal and instance_sensitive are both True which will conflict with each either",
                 logger=self._logger,
             )
 
     @property
@@ -158,24 +184,27 @@
         return dict(
             scale=self.scale,
             apply_thinning=self.apply_thinning,
             apply_nms=self.apply_nms,
             max_dist=self.max_dist,
             kill_internal=self.kill_internal,
             skip_if_nonexistent=self.skip_if_nonexistent,
+            num_classes=len(self.CLASSES),
         )
 
     def _before_evaluation(self):
+        assert (
+            self._sample_names is not None
+        ), "ERR: no samples yet. load them before evaluation"
         assert osp.exists(
             self.dataset_root
         ), f"ERR: {self.dataset_root} does not exist"
-        assert osp.exists(self.CLS_root), f"ERR: {self.CLS_root} does not exist"
         assert osp.exists(
-            self.INST_root
-        ), f"ERR: {self.INST_root} does not exist"
+            self.gtEval_root
+        ), f"ERR: {self.gtEval_root} does not exist"
         assert osp.exists(
             self.pred_root
         ), f"ERR: {self.pred_root} does not exist"
 
     def evaluate_category(
         self,
         category,
@@ -191,24 +220,30 @@
         # populate data (samples)
         data = []
         for sample_name in self.sample_names:
             # FIXME: naming scheme differs sometimes
             category_dir = f"class_{str(category).zfill(3)}"
 
             # GT file paths
-            cls_path = osp.join(self.CLS_root, f"{sample_name}{self.GT_SUFFIX}")
             if self.instance_sensitive:
-                inst_path = osp.join(
-                    self.INST_root, f"{sample_name}{self.GT_SUFFIX}"
+                edge_path = osp.join(
+                    self.gtEval_root,
+                    f"{sample_name}{self.ISEDGE_SUFFIX}",
                 )
-                assert osp.exists(inst_path), f"ERR: {inst_path} is not valid"
             else:
-                inst_path = None
-
-            assert osp.exists(cls_path), f"ERR: {cls_path} is not valid"
+                edge_path = osp.join(
+                    self.gtEval_root,
+                    f"{sample_name}{self.EDGE_SUFFIX}",
+                )
+            seg_path = osp.join(
+                self.gtEval_root,
+                f"{sample_name}{self.SEG_SUFFIX}",
+            )
+            assert osp.exists(edge_path), f"ERR: {edge_path} is not valid"
+            assert osp.exists(seg_path), f"ERR: {seg_path} is not valid"
 
             # prediction file path
             # sample_name = sample_name.split("/")[1]  # assert city/img
             pred_path = osp.join(
                 self.pred_root,
                 category_dir,
                 f"{sample_name}{self.PRED_SUFFIX}",
@@ -216,16 +251,16 @@
 
             data.append(
                 dict(
                     name=sample_name,
                     category=category,
                     thresholds=thresholds,
                     # file paths
-                    cls_path=cls_path,
-                    inst_path=inst_path,
+                    edge_path=edge_path,
+                    seg_path=seg_path,
                     pred_path=pred_path,
                     **self.eval_params,
                 )
             )
 
         assert len(data) > 0, "ERR: no evaluation data"
 
@@ -245,7 +280,102 @@
                 category=category,
                 sample_metrics=sample_metrics,
                 threshold_metrics=threshold_metrics,
                 overall_metric=overall_metric,
             )
 
         return overall_metric
+
+
+class ReannoSBDEvaluator(SBDEvaluator):
+    """Reannotated SBD validation split evaluator."""
+
+    RAW_EDGE_SUFFIX = "_reanno_raw_edge.png"
+    THIN_EDGE_SUFFIX = "_reanno_thin_edge.png"
+    RAW_ISEDGE_SUFFIX = "_reanno_raw_isedge.png"
+    THIN_ISEDGE_SUFFIX = "_reanno_thin_isedge.png"
+
+    def __init__(
+        self,
+        dataset_root: str,
+        pred_root: str,
+        split: str = "val",
+        thin: bool = False,
+        gt_dir=None,
+        pred_suffix=None,
+        **kwargs,
+    ):
+        self.dataset_root = dataset_root
+        self.pred_root = pred_root
+
+        assert split in ("val", "test")
+        self.split = split
+        self.thin = thin
+        if self.thin:
+            print_log(
+                "Using `thin` mode; setting the suffix respectively",
+                logger=self._logger,
+            )
+            self.EDGE_SUFFIX = self.THIN_EDGE_SUFFIX
+            self.ISEDGE_SUFFIX = self.THIN_ISEDGE_SUFFIX
+        else:
+            print_log(
+                "Using `raw` mode; setting the suffix respectively",
+                logger=self._logger,
+            )
+            self.EDGE_SUFFIX = self.RAW_EDGE_SUFFIX
+            self.ISEDGE_SUFFIX = self.RAW_ISEDGE_SUFFIX
+
+        # change dataset directory and suffix
+        if gt_dir:
+            print_log(f"changing GT_DIR to {gt_dir}", logger=self._logger)
+            self.GT_DIR = gt_dir
+        if pred_suffix:
+            print_log(
+                f"changing PRED_SUFFIX to {pred_suffix}", logger=self._logger
+            )
+            self.PRED_SUFFIX = pred_suffix
+
+        # set parameters
+        self.gtEval_root = osp.join(self.dataset_root, self.GT_DIR)
+
+        if pred_suffix is not None:
+            print_log(f"changed suffix to {pred_suffix}")
+            self.PRED_SUFFIX = pred_suffix
+
+        # we can try to load some sample names
+        try:
+            self.set_sample_names()
+        except Exception:
+            print_log(
+                "Tried to set sample_names, but couldn't",
+                logger=self._logger,
+            )
+
+    def set_eval_params(
+        self,
+        eval_mode=None,
+        scale: float = 1.0,
+        apply_thinning: bool = False,
+        apply_nms: bool = False,
+        instance_sensitive: bool = True,
+        max_dist: float = 0.0075,
+        **kwargs,
+    ) -> None:
+        print_log(
+            "Using params for re-annotated test split", logger=self._logger
+        )
+        assert 0 < scale <= 1, f"ERR: scale ({scale}) is not valid"
+        self.scale = scale
+        self.apply_thinning = apply_thinning
+        self.apply_nms = apply_nms
+
+        self.max_dist = max_dist
+        self.kill_internal = False
+        self.skip_if_nonexistent = False
+        self.instance_sensitive = instance_sensitive
+
+        if self.kill_internal and self.instance_sensitive:
+            print_log(
+                "kill_internal and instance_sensitive are both True which will conflict with each either",
+                logger=self._logger,
+            )
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/helpers/convert_cityscapes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/helpers/convert_cityscapes.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/helpers/evaluate_bsds500.py` & `pyEdgeEval-0.2.7/pyEdgeEval/helpers/evaluate_bsds500.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import argparse
 import os.path as osp
 import time
 
+import pyEdgeEval
 from pyEdgeEval.evaluators.bsds import BSDS500Evaluator
 from pyEdgeEval.utils import get_root_logger, mkdir_or_exist
 
 __all__ = ["evaluate_bsds500"]
 
 
 def parse_args():
@@ -109,14 +110,15 @@
     split = "val" if use_val else "test"
 
     # setup logger
     timestamp = time.strftime("%Y%m%d_%H%M%S", time.localtime())
     log_file = osp.join(output_path, f"{timestamp}.log")
     logger = get_root_logger(log_file=log_file, log_level="INFO")
     logger.info("Running BSDS5000 Evaluation")
+    logger.info(f"pyEdgeEval version: {pyEdgeEval.__version__}")
     logger.info(f"split:                  \t{split}")
     logger.info(f"thresholds:             \t{thresholds}")
     logger.info(f"max_dist:               \t{max_dist}")
     logger.info(f"thinning + thinned gts: \t{apply_thinning}")
     logger.info(f"nms:                    \t{apply_nms}")
     print("\n\n")
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/helpers/evaluate_cityscapes.py` & `pyEdgeEval-0.2.7/pyEdgeEval/helpers/evaluate_cityscapes.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 
 import argparse
 import os.path as osp
 import time
 import warnings
 
+import pyEdgeEval
 from pyEdgeEval.evaluators import CityscapesEvaluator, HalfCityscapesEvaluator
 from pyEdgeEval.utils import get_root_logger, mkdir_or_exist
 
 __all__ = ["evaluate_cityscapes_thin", "evaluate_cityscapes_raw"]
 
 
 def _common_parser_args(
@@ -198,14 +199,15 @@
     mkdir_or_exist(output_path)
 
     # setup logger
     timestamp = time.strftime("%Y%m%d_%H%M%S", time.localtime())
     log_file = osp.join(output_path, f"{timestamp}.log")
     logger = get_root_logger(log_file=log_file, log_level="INFO")
     logger.info("Running Cityscapes Evaluation")
+    logger.info(f"pyEdgeEval version: {pyEdgeEval.__version__}")
     logger.info(f"categories:         \t{categories}")
     logger.info(f"thresholds:         \t{thresholds}")
     logger.info(f"scale:              \t{scale}")
     logger.info(f"pre-seal:           \t{pre_seal}")
     logger.info(f"thinned GTs:        \t{thin}")
     logger.info(f"thinning:           \t{apply_thinning}")
     logger.info(f"nms:                \t{apply_nms}")
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/helpers/evaluate_sbd.py` & `pyEdgeEval-0.2.7/pyEdgeEval/helpers/evaluate_sbd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import argparse
 import os.path as osp
 import time
 
-from pyEdgeEval.evaluators.sbd import SBDEvaluator
+import pyEdgeEval
+from pyEdgeEval.evaluators.sbd import SBDEvaluator, ReannoSBDEvaluator
 from pyEdgeEval.utils import get_root_logger, mkdir_or_exist
 
 __all__ = ["evaluate_sbd"]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Evaluate SBD output")
@@ -19,26 +20,14 @@
     )
     parser.add_argument(
         "pred_path",
         type=str,
         help="the root path of the predictions",
     )
     parser.add_argument(
-        "--cls-dir",
-        type=str,
-        default="cls_orig",
-        help="directory name for class labels",
-    )
-    parser.add_argument(
-        "--inst-dir",
-        type=str,
-        default="inst_orig",
-        help="directory name for instance labels",
-    )
-    parser.add_argument(
         "--pred-suffix",
         type=str,
         default=".png",
         help="suffix for predicted images",
     )
     parser.add_argument(
         "--output-path",
@@ -89,18 +78,17 @@
         help="the number of parallel threads",
     )
 
     return parser.parse_args()
 
 
 def evaluate(
+    gt_dir: str,
     sbd_path: str,
     pred_path: str,
-    cls_dir: str,
-    inst_dir: str,
     pred_suffix: str,
     output_path: str,
     categories: str,
     pre_seal: bool,
     apply_thinning: bool,
     apply_nms: bool,
     nonIS: bool,
@@ -170,33 +158,32 @@
 
     mkdir_or_exist(output_path)
 
     timestamp = time.strftime("%Y%m%d_%H%M%S", time.localtime())
     log_file = osp.join(output_path, f"{timestamp}.log")
     logger = get_root_logger(log_file=log_file, log_level="INFO")
     logger.info("Running SBD Evaluation")
-    logger.info(f"cls_dir:    \t{cls_dir}")
-    logger.info(f"inst_dir:   \t{inst_dir}")
+    logger.info(f"pyEdgeEval version: {pyEdgeEval.__version__}")
+    logger.info(f"GT dir:     \t{gt_dir}")
     logger.info(f"pred_suffix:\t{pred_suffix}")
     logger.info(f"categories: \t{categories}")
     logger.info(f"thresholds: \t{thresholds}")
     logger.info(f"pre-seal:   \t{pre_seal}")
     logger.info(f"thin:       \t{apply_thinning}")
     logger.info(f"nms:        \t{apply_nms}")
     logger.info(f"nonIS:      \t{nonIS}")
     logger.info(f"max_dist    \t{max_dist}")
     print("\n\n")
 
     # initialize evaluator
     evaluator = SBDEvaluator(
         dataset_root=sbd_path,
         pred_root=pred_path,
-        cls_dir=cls_dir,
-        inst_dir=inst_dir,
-        pred_suffix=pred_suffix,
+        thin=apply_thinning,
+        gt_dir=gt_dir,  # NOTE: we can change the directory where the preprocessed GTs are located
     )
     if evaluator.sample_names is None:
         # load custom sample names
         # SAMPLE_NAMES = ["2008_000051", "2008_000195"]
         evaluator.set_sample_names()
 
     # set parameters
@@ -216,57 +203,55 @@
         categories=categories,
         thresholds=thresholds,
         nproc=nproc,
         save_dir=output_path,
     )
 
 
-def evaluate_sbd():
+def evaluate_sbd(gt_dir: str = "gtEval"):
     args = parse_args()
 
     # by default, we apply thinning
     apply_thinning = not args.raw
 
     evaluate(
+        gt_dir=gt_dir,
         sbd_path=args.sbd_path,
         pred_path=args.pred_path,
-        cls_dir=args.cls_dir,
-        inst_dir=args.inst_dir,
         pred_suffix=args.pred_suffix,
         output_path=args.output_path,
         categories=args.categories,
         pre_seal=args.pre_seal,
         apply_thinning=apply_thinning,
         apply_nms=args.apply_nms,
         nonIS=args.nonIS,
         max_dist=args.max_dist,
         thresholds=args.thresholds,
         nproc=args.nproc,
     )
 
 
 def evaluate_reanno(
+    gt_dir: str,
     sbd_path: str,
     pred_path: str,
-    cls_dir: str,
-    inst_dir: str,
     pred_suffix: str,
     output_path: str,
     categories: str,
     apply_thinning: bool,
     apply_nms: bool,
     nonIS: bool,
     thresholds: str,
     nproc: int,
 ):
     """Evaluate Re-annotated SBD"""
 
     if categories is None:
         print("use all categories")
-        categories = list(range(1, len(SBDEvaluator.CLASSES) + 1))
+        categories = list(range(1, len(ReannoSBDEvaluator.CLASSES) + 1))
     else:
         # string evaluation for categories
         categories = categories.strip()
         try:
             categories = [int(categories)]
         except ValueError:
             try:
@@ -320,41 +305,40 @@
 
     mkdir_or_exist(output_path)
 
     timestamp = time.strftime("%Y%m%d_%H%M%S", time.localtime())
     log_file = osp.join(output_path, f"{timestamp}.log")
     logger = get_root_logger(log_file=log_file, log_level="INFO")
     logger.info("Running Re-Annotated SBD Evaluation")
-    logger.info(f"cls_dir:    \t{cls_dir}")
-    logger.info(f"inst_dir:   \t{inst_dir}")
+    logger.info(f"pyEdgeEval version: {pyEdgeEval.__version__}")
+    logger.info(f"GT dir:     \t{gt_dir}")
     logger.info(f"pred_suffix:\t{pred_suffix}")
     logger.info(f"categories: \t{categories}")
     logger.info(f"thresholds: \t{thresholds}")
     logger.info(f"thin:       \t{apply_thinning}")
     logger.info(f"nms:        \t{apply_nms}")
     logger.info(f"nonIS:      \t{nonIS}")
     print("\n\n")
 
     # initialize evaluator
-    evaluator = SBDEvaluator(
+    evaluator = ReannoSBDEvaluator(
         dataset_root=sbd_path,
         pred_root=pred_path,
-        cls_dir=cls_dir,
-        inst_dir=inst_dir,
         pred_suffix=pred_suffix,
+        thin=apply_thinning,
+        gt_dir=gt_dir,
     )
     if evaluator.sample_names is None:
         # load custom sample names
         # SAMPLE_NAMES = ["2008_000051", "2008_000195"]
         evaluator.set_sample_names()
 
     # set parameters
     instance_sensitive = not nonIS
     evaluator.set_eval_params(
-        eval_mode="reanno",  # fixed to "reanno" mode
         scale=1.0,
         apply_thinning=apply_thinning,
         apply_nms=apply_nms,
         max_dist=0.0075,  # fixed
         instance_sensitive=instance_sensitive,
     )
 
@@ -363,25 +347,24 @@
         categories=categories,
         thresholds=thresholds,
         nproc=nproc,
         save_dir=output_path,
     )
 
 
-def evaluate_reanno_sbd():
+def evaluate_reanno_sbd(gt_dir: str = "gtEval"):
     args = parse_args()
 
     # by default, we apply thinning
     apply_thinning = not args.raw
 
     evaluate_reanno(
+        gt_dir=gt_dir,
         sbd_path=args.sbd_path,
         pred_path=args.pred_path,
-        cls_dir=args.cls_dir,
-        inst_dir=args.inst_dir,
         pred_suffix=args.pred_suffix,
         output_path=args.output_path,
         categories=args.categories,
         apply_thinning=apply_thinning,
         apply_nms=args.apply_nms,
         nonIS=args.nonIS,
         max_dist=args.max_dist,
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/preprocess/nms/fast_nms.py` & `pyEdgeEval-0.2.7/pyEdgeEval/preprocess/nms/fast_nms.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/preprocess/nms/toolbox.py` & `pyEdgeEval-0.2.7/pyEdgeEval/preprocess/nms/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/preprocess/thin/bwmorph_thin.py` & `pyEdgeEval-0.2.7/pyEdgeEval/preprocess/thin/bwmorph_thin.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/preprocess/thin/thin.py` & `pyEdgeEval-0.2.7/pyEdgeEval/preprocess/thin/thin.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,15 @@
     thin1_mut = _lut_mutate_mask(thin1)
     thin2_mut = _lut_mutate_mask(thin2)
 
     iter_count = 0
     while max_iter is None or iter_count < max_iter:
         # Iter 1
         lut_indices = binary_image_to_lut_indices(x)
+        # FIXME: index "" is out of bounds for axis 0 with size 512
         x_mut = thin1_mut[lut_indices]
         if x_mut.sum() == 0:
             break
 
         x = thin1[lut_indices]
 
         # Iter 2
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/utils/__init__.py` & `pyEdgeEval-0.2.7/pyEdgeEval/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/utils/convert_formats.py` & `pyEdgeEval-0.2.7/pyEdgeEval/utils/convert_formats.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/utils/distance_transforms.py` & `pyEdgeEval-0.2.7/pyEdgeEval/utils/distance_transforms.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/utils/logger.py` & `pyEdgeEval-0.2.7/pyEdgeEval/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/utils/mat_utils.py` & `pyEdgeEval-0.2.7/pyEdgeEval/utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/utils/path.py` & `pyEdgeEval-0.2.7/pyEdgeEval/utils/path.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/utils/progressbar.py` & `pyEdgeEval-0.2.7/pyEdgeEval/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/utils/timer.py` & `pyEdgeEval-0.2.7/pyEdgeEval/utils/timer.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval/visualization/pr_curve.py` & `pyEdgeEval-0.2.7/pyEdgeEval/visualization/pr_curve.py`

 * *Files identical despite different names*

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval.egg-info/PKG-INFO` & `pyEdgeEval-0.2.7/pyEdgeEval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEdgeEval
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python Edge Evaluation Tools
 Home-page: https://github.com/haruishi43/py-edge-eval
 Author: haruishi43
 Author-email: haruyaishikawa@keio.jp
 License: MIT
 Keywords: Edge Detection,Semantic Boundary Detection,Computer Vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyEdgeEval-0.2.6/pyEdgeEval.egg-info/SOURCES.txt` & `pyEdgeEval-0.2.7/pyEdgeEval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 pyEdgeEval/common/multi_label/__init__.py
 pyEdgeEval/common/multi_label/calculate_metrics.py
 pyEdgeEval/common/multi_label/edge_decoding.py
 pyEdgeEval/common/multi_label/edge_encoding.py
 pyEdgeEval/common/multi_label/evaluate_boundaries.py
 pyEdgeEval/common/multi_label/io.py
 pyEdgeEval/common/multi_label/options.py
+pyEdgeEval/common/multi_label/utils.py
 pyEdgeEval/datasets/__init__.py
 pyEdgeEval/datasets/bsds.py
 pyEdgeEval/datasets/cityscapes.py
 pyEdgeEval/datasets/cityscapes_attributes.py
 pyEdgeEval/datasets/generic_binary.py
 pyEdgeEval/datasets/otf_cityscapes.py
 pyEdgeEval/datasets/sbd.py
@@ -94,8 +95,10 @@
 pyEdgeEval/utils/distance_transforms.py
 pyEdgeEval/utils/logger.py
 pyEdgeEval/utils/mat_utils.py
 pyEdgeEval/utils/path.py
 pyEdgeEval/utils/progressbar.py
 pyEdgeEval/utils/timer.py
 pyEdgeEval/visualization/__init__.py
-pyEdgeEval/visualization/pr_curve.py
+pyEdgeEval/visualization/pr_curve.py
+tests/test_bsds500.py
+tests/test_sbd.py
```

### Comparing `pyEdgeEval-0.2.6/setup.py` & `pyEdgeEval-0.2.7/setup.py`

 * *Files identical despite different names*

