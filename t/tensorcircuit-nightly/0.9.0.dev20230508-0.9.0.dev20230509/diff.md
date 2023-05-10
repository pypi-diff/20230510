# Comparing `tmp/tensorcircuit-nightly-0.9.0.dev20230508.tar.gz` & `tmp/tensorcircuit-nightly-0.9.0.dev20230509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.0.dev20230508.tar", last modified: Mon May  8 12:39:36 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.0.dev20230509.tar", last modified: Tue May  9 13:19:37 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.0.dev20230508.tar` & `tensorcircuit-nightly-0.9.0.dev20230509.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/
--rw-r--r--   0 runner    (1001) docker     (122)    23884 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18300 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.047514 tensorcircuit-nightly-0.9.0.dev20230508/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.051514 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6397 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2985 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8695 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-08 12:39:30.000000 tensorcircuit-nightly-0.9.0.dev20230508/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.051514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-08 12:39:29.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.055514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3519 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-08 12:39:35.000000 tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-08 12:39:36.059514 tensorcircuit-nightly-0.9.0.dev20230508/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-08 12:17:34.000000 tensorcircuit-nightly-0.9.0.dev20230508/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/
+-rw-r--r--   0 runner    (1001) docker     (122)    24079 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18300 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.254651 tensorcircuit-nightly-0.9.0.dev20230509/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.258651 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6397 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2985 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8695 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-09 13:19:30.000000 tensorcircuit-nightly-0.9.0.dev20230509/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.258651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-09 13:19:30.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14212 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7968 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2945 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7791 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5030 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.262651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    20682 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-09 13:19:36.000000 tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 13:19:37.266651 tensorcircuit-nightly-0.9.0.dev20230509/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33394 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46467 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4204 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-09 12:55:12.000000 tensorcircuit-nightly-0.9.0.dev20230509/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/CHANGELOG.md` & `tensorcircuit-nightly-0.9.0.dev20230509/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 
 ### Added
 
 - Add `tc.TorchHardwarLayer` for shortcut layer construction of quantum hardware experiments
 
 - Add cotengra contractor setup shortcut
 
+- Add simplecompiler module to assite qiskit compile for better performance when targeting rz native basis
+
 ### Changed
 
 - Add compiler and cloud namespace to the global tensorcircuit namespace
 
+- Refactor composed compiler pipeline interface to include simple_compiler (breaking)
+
 ## 0.9.0
 
 ### Added
 
 - Cloud module for Tencent QCloud is now merged into the master branch and ready to release
 
 - Add `tc.about()` to print related software versions and configs
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/HISTORY.md` & `tensorcircuit-nightly-0.9.0.dev20230509/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/LICENSE` & `tensorcircuit-nightly-0.9.0.dev20230509/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/PKG-INFO` & `tensorcircuit-nightly-0.9.0.dev20230509/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.0.dev20230508
+Version: 0.9.0.dev20230509
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/README.md` & `tensorcircuit-nightly-0.9.0.dev20230509/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/README_cn.md` & `tensorcircuit-nightly-0.9.0.dev20230509/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/conf.py` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/index.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.0.dev20230509/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/setup.py` & `tensorcircuit-nightly-0.9.0.dev20230509/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.0.dev20230508"
+__version__ = "0.9.0.dev20230509"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cloud/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,20 +150,21 @@
                 c1.rx(j, theta=np.pi / 2)  # type: ignore
                 exp.append(j)
             elif i == 3:
                 exp.append(j)
         c1, info = qiskit_compile(
             c1,
             compiled_options={
-                "basis_gates": device.native_gates(),
+                "basis_gates": device.native_gates() + ["cx"],
                 # whether + "cx" here?
-                "optimization_level": 3,
+                "optimization_level": 2,
                 "coupling_map": device.topology(),
             },
         )
+        # change the compiler to DefaultCompiler when it matures
         cs.append(c1)
         infos.append(info)
         exps.append(exp)
 
     reduced_cs = []
     reduced_dict = {}
     recover_dict = {}
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/composed_compiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from ..utils import is_sequence
 from ..abstractcircuit import AbstractCircuit
 from .qiskit_compiler import qiskit_compile
+from .simple_compiler import simple_compile
 
 
 class Compiler:
     def __init__(
         self,
         compile_funcs: Union[Callable[..., Any], List[Callable[..., Any]]],
         compiled_options: Optional[List[Dict[str, Any]]] = None,
@@ -20,24 +21,54 @@
         else:
             self.compile_funcs = list(compile_funcs)  # type: ignore
         self.add_options(compiled_options)
 
     def add_options(
         self, compiled_options: Optional[List[Dict[str, Any]]] = None
     ) -> None:
-        if not is_sequence(compiled_options):
-            self.compiled_options = [compiled_options for _ in self.compile_funcs]
+        if compiled_options is None:
+            self.compiled_options = [{} for _ in range(len(self.compile_funcs))]  # type: ignore
+        elif not is_sequence(compiled_options):
+            self.compiled_options = [compiled_options for _ in self.compile_funcs]  # type: ignore
         else:
             assert len(compiled_options) == len(  # type: ignore
                 self.compile_funcs
             ), "`compiled_options` must have the same list length as `compile_funcs`"
             self.compiled_options = list(compiled_options)  # type: ignore
+            for i, c in enumerate(self.compiled_options):
+                if c is None:
+                    self.compiled_options[i] = {}
 
     def __call__(
         self, circuit: AbstractCircuit, info: Optional[Dict[str, Any]] = None
     ) -> Any:
         for f, d in zip(self.compile_funcs, self.compiled_options):
-            circuit, info = f(circuit, info, compiled_options=d)  # type: ignore
+            result = f(circuit, info, compiled_options=d)  # type: ignore
+            if not isinstance(result, tuple):
+                result = (result, info)
+            circuit, info = result
         return circuit, info
 
 
-default_compiler = Compiler(qiskit_compile)
+class DefaultCompiler(Compiler):
+    def __init__(self, qiskit_compiled_options: Optional[Dict[str, Any]] = None):
+        """
+        A fallback choice to compile circuit running on tencent quantum cloud with rz as native gate
+
+        :param qiskit_compiled_options: qiskit compiled options to be added
+            options documented in `qiskit.transpile` method,
+            to use tencent quantum cloud, `{"coupling_map": d.topology()}` is in general enough,
+            where d is a device object,
+            defaults to None, i.e. no qubit mapping is applied
+        :type qiskit_compiled_options: Optional[Dict[str, Any]], optional
+        """
+        compiled_options = {
+            "optimization_level": 3,
+            "basis_gates": ["u3", "h", "cx", "cz"],
+        }
+        # rz target is bad for qiskit
+        if qiskit_compiled_options:
+            compiled_options.update(qiskit_compiled_options)
+        super().__init__(
+            [qiskit_compile, simple_compile],
+            [compiled_options, None],  # type: ignore
+        )
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     for r in s.split("\n"):
         inc = re.search(r"\(.*\)", r)
         if inc is None:
             rs.append(r)
         else:
             v = r[inc.start() : inc.end()]
             v = eval(v)
-            r = r[: inc.start()] + "(" + str(v) + ")" + r[inc.end() :]
+            if not isinstance(v, tuple):
+                r = r[: inc.start()] + "(" + str(v) + ")" + r[inc.end() :]
+            else:  # u gate case
+                r = r[: inc.start()] + str(v) + r[inc.end() :]
             rs.append(r)
     return "\n".join(rs)
 
 
 def _comment_qasm(s: str) -> str:
     """
     return the qasm str in comment format
@@ -116,27 +119,41 @@
 
 def qiskit_compile(
     circuit: Any,
     info: Optional[Dict[str, Any]] = None,
     output: str = "tc",
     compiled_options: Optional[Dict[str, Any]] = None,
 ) -> Any:
+    """
+    compile the circuit using ``qiskit.transpile`` method with some tricks and hacks
+
+    :param circuit: circuit in ``tc.Circuit`` or ``qiskit.QuantumCircuit`` form
+    :type circuit: Any
+    :param info: info for qubit mappings, defaults to None
+    :type info: Optional[Dict[str, Any]], optional
+    :param output: output circuit format, defaults to "tc"
+    :type output: str, optional
+    :param compiled_options: ``qiskit.transpile`` options in a dict, defaults to None
+    :type compiled_options: Optional[Dict[str, Any]], optional
+    :return: Tuple containing the output circuit and the qubit mapping info dict
+    :rtype: Any
+    """
     from qiskit.compiler import transpile
     from qiskit.transpiler.passes import RemoveBarriers
 
     if isinstance(circuit, AbstractCircuit):
         circuit = circuit.to_qiskit(enable_instruction=True)
     elif isinstance(circuit, str):
         circuit = qiskit_from_qasm_str_ordered_measure(circuit)
     # else qiskit circuit
     circuit = _add_measure_all_if_none(circuit)
     if compiled_options is None:
         compiled_options = {
             "basis_gates": ["h", "rz", "cx"],
-            "optimization_level": 2,
+            "optimization_level": 2,  # 3 can induce bugs...
         }
     ncircuit = transpile(circuit, **compiled_options)
     ncircuit = RemoveBarriers()(ncircuit)
 
     if output.lower() in ["qasm", "openqasm"]:
         r0 = ncircuit.qasm()
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.0.dev20230508
+Version: 0.9.0.dev20230509
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.0.dev20230509/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 tensorcircuit/cloud/quafu_provider.py
 tensorcircuit/cloud/tencent.py
 tensorcircuit/cloud/utils.py
 tensorcircuit/cloud/wrapper.py
 tensorcircuit/compiler/__init__.py
 tensorcircuit/compiler/composed_compiler.py
 tensorcircuit/compiler/qiskit_compiler.py
+tensorcircuit/compiler/simple_compiler.py
 tensorcircuit/interfaces/__init__.py
 tensorcircuit/interfaces/numpy.py
 tensorcircuit/interfaces/scipy.py
 tensorcircuit/interfaces/tensorflow.py
 tensorcircuit/interfaces/tensortrans.py
 tensorcircuit/interfaces/torch.py
 tensorcircuit/results/__init__.py
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/conftest.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_backends.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_channels.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_compiler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import os
 import pytest
+import numpy as np
 
 # from pytest_lazyfixture import lazy_fixture as lf
 
 
 thisfile = os.path.abspath(__file__)
 modulepath = os.path.dirname(os.path.dirname(thisfile))
 
@@ -69,31 +70,78 @@
         },
     )
     assert info2["positional_logical_mapping"] == {0: 1}
     print(c2.draw())
 
 
 def test_composed_compiler():
-    from tensorcircuit.compiler import default_compiler
+    from tensorcircuit.compiler import DefaultCompiler
 
     c = tc.Circuit(3)
     c.rx(0)
     c.cx(0, 1)
     c.cz(1, 0)
     c.rxx(0, 2, theta=0.2)
     c.measure_instruction(2)
     c.measure_instruction(0)
+    default_compiler = DefaultCompiler()
     c1, info = default_compiler(c)
     print(c1.draw())
-    assert c1.gate_count_by_condition(lambda qir: qir["name"] == "cnot") == 4
+    assert c1.gate_count_by_condition(lambda qir: qir["name"] == "cnot") == 3
     assert info["positional_logical_mapping"][0] == 2
 
-    default_compiler.add_options(
+    default_compiler = DefaultCompiler(
         {
             "basis_gates": ["h", "rz", "cz"],
             "optimization_level": 2,
             "coupling_map": [[0, 1], [1, 2]],
         }
     )
+
     c1, info = default_compiler(c)
     assert c1.gate_count_by_condition(lambda qir: qir["name"] == "cnot") == 0
     print(info)
+
+
+def test_replace_r():
+    c = tc.Circuit(3)
+    c.rz(0, theta=0.1)
+    c.cx(0, 2)
+    c.ry(1)
+    c.rxx(1, 0, theta=0.2)
+    c.rx(0, theta=3.9)
+    c.ry(1, theta=-0.2)
+    c.rzz(1, 0, theta=-0.3)
+    c.ryy(1, 0, theta=-0.6)
+    c.rx(2)
+
+    print(c.draw())
+    c1 = tc.compiler.simple_compiler.replace_r(c)
+    print(c1.draw())
+    np.testing.assert_allclose(c.matrix(), c1.matrix(), atol=1e-5)
+
+
+def test_default_compiler():
+    c = tc.Circuit(3)
+    c.cx(0, 1)
+    c.rx(0, theta=1e-5)
+    c.x(1)
+    c.y(1)
+    c.z(1)
+    c.h(1)
+    c.cz(2, 0)
+    c.h(1)
+    c.cz(2, 0)
+    c.s(2)
+    c.sd(2)
+    c.s(2)
+    c.s(2)
+    c.y(2)
+    c.ry(2, theta=0.1)
+    c.t(2)
+    c.td(2)
+    c.ry(2, theta=-0.1)
+    c.rz(1, theta=0.3)
+
+    c1, _ = tc.compiler.simple_compiler.simple_compile(c)
+    print(c1.draw())
+    assert c1.gate_count() == 3
```

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_gates.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_keras.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_results.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_templates.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.0.dev20230508/tests/test_van.py` & `tensorcircuit-nightly-0.9.0.dev20230509/tests/test_van.py`

 * *Files identical despite different names*

