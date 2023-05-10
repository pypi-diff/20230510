# Comparing `tmp/vgd_counterfactuals-0.1.0.tar.gz` & `tmp/vgd_counterfactuals-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgd_counterfactuals-0.1.0.tar", max compression
+gzip compressed data, was "vgd_counterfactuals-0.1.1.tar", max compression
```

## Comparing `vgd_counterfactuals-0.1.0.tar` & `vgd_counterfactuals-0.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     6577 2023-05-02 06:41:58.633779 vgd_counterfactuals-0.1.0/README.rst
--rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.0/banner.png
--rwxr-xr-x   0        0        0     1514 2023-05-02 06:24:10.198569 vgd_counterfactuals-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        5 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.0/vgd_counterfactuals/VERSION
--rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.0/vgd_counterfactuals/__init__.py
--rw-r--r--   0        0        0     6867 2023-05-01 16:03:23.965909 vgd_counterfactuals-0.1.0/vgd_counterfactuals/base.py
--rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.0/vgd_counterfactuals/cli.py
--rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/00_quickstart.py
--rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/01_visualization.py
--rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/__init__.py
--rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
--rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
--rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
--rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
--rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
--rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
--rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
--rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
--rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
--rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
--rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
--rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
--rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
--rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
--rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
--rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
--rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
--rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
--rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
--rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
--rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
--rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
--rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
--rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
--rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
--rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
--rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.0/vgd_counterfactuals/experiments/README.rst
--rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.0/vgd_counterfactuals/experiments/results/README.rst
--rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.0/vgd_counterfactuals/experiments/template_experiment.py
--rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.0/vgd_counterfactuals/experiments/template_experiment_sub.py
--rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.0/vgd_counterfactuals/generate/__init__.py
--rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.0/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3633 2023-04-30 08:18:38.839977 vgd_counterfactuals-0.1.0/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
--rw-r--r--   0        0        0     5345 2023-04-30 08:18:38.171972 vgd_counterfactuals-0.1.0/vgd_counterfactuals/generate/molecules.py
--rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.0/vgd_counterfactuals/generate/smiles_one_step_changes.py
--rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.0/vgd_counterfactuals/templates/article.tex.j2
--rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.0/vgd_counterfactuals/testing.py
--rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.0/vgd_counterfactuals/utils.py
--rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.0/vgd_counterfactuals/visualization.py
--rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     6577 2023-05-10 10:47:16.579832 vgd_counterfactuals-0.1.1/README.rst
+-rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.1/banner.png
+-rwxr-xr-x   0        0        0     1514 2023-05-10 10:47:16.571832 vgd_counterfactuals-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2023-05-10 10:47:16.579832 vgd_counterfactuals-0.1.1/vgd_counterfactuals/VERSION
+-rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.1/vgd_counterfactuals/__init__.py
+-rw-r--r--   0        0        0     6867 2023-05-01 16:03:23.965909 vgd_counterfactuals-0.1.1/vgd_counterfactuals/base.py
+-rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/cli.py
+-rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/00_quickstart.py
+-rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/01_visualization.py
+-rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
+-rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
+-rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
+-rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
+-rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
+-rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
+-rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
+-rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
+-rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
+-rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
+-rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
+-rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
+-rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
+-rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
+-rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
+-rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
+-rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
+-rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
+-rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
+-rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
+-rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
+-rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
+-rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
+-rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
+-rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
+-rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
+-rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/README.rst
+-rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/results/README.rst
+-rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/template_experiment.py
+-rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/template_experiment_sub.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3752 2023-05-10 10:46:22.791428 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
+-rw-r--r--   0        0        0     6040 2023-05-10 10:46:22.147423 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/molecules.py
+-rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/smiles_one_step_changes.py
+-rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.1/vgd_counterfactuals/templates/article.tex.j2
+-rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.1/vgd_counterfactuals/testing.py
+-rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.1/vgd_counterfactuals/utils.py
+-rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.1/vgd_counterfactuals/visualization.py
+-rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.1/PKG-INFO
```

### Comparing `vgd_counterfactuals-0.1.0/LICENSE` & `vgd_counterfactuals-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/README.rst` & `vgd_counterfactuals-0.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.0-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.1-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

### Comparing `vgd_counterfactuals-0.1.0/banner.png` & `vgd_counterfactuals-0.1.1/banner.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/pyproject.toml` & `vgd_counterfactuals-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vgd_counterfactuals"
-version = "0.1.0"
+version = "0.1.1"
 description = "Counterfactual explanations for GNNs based on the visual graph dataset format"
 license = "MIT license"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "counterfactuals", "explainable AI"]
 packages = [
```

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/base.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/base.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/cli.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/cli.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/00_quickstart.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/00_quickstart.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/01_visualization.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/01_visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/code.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/code.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/experiments/README.rst` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/experiments/template_experiment.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/template_experiment.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/experiments/template_experiment_sub.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/experiments/template_experiment_sub.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 30 08:18:38 2023 UTC, .py size: 5345 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,228 +1,235 @@
-00000000: 6f0d 0d0a 0000 0000 5e24 4e64 e114 0000  o.......^$Nd....
+00000000: 6f0d 0d0a 0000 0000 fe75 5b64 9817 0000  o........u[d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 f800 0000 6400  .....@...s....d.
+00000020: 0009 0000 0040 0000 0073 fa00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6405 6406 6407  m.Z...d.d.d.d.d.
-00000060: 6407 6408 9c06 5a07 6507 6601 6409 6508  d.d...Z.e.f.d.e.
-00000070: 640a 6502 6a09 6508 1900 6604 640b 640c  d.e.j.e...f.d.d.
-00000080: 8405 5a0a 641a 640e 6504 6a0b 640f 650c  ..Z.d.d.e.j.d.e.
-00000090: 640a 650d 6606 6410 6411 8405 5a0e 640e  d.e.f.d.d...Z.d.
-000000a0: 6504 6a0b 6412 6502 6a0f 6508 650c 6602  e.j.d.e.j.e.e.f.
-000000b0: 1900 6413 6502 6a0f 650c 6502 6a09 650c  ..d.e.j.e.e.j.e.
-000000c0: 1900 6602 1900 640a 6502 6a10 6508 1900  ..f...d.e.j.e...
-000000d0: 6608 6414 6415 8404 5a11 640e 6504 6a0b  f.d.d...Z.d.e.j.
-000000e0: 6413 6502 6a0f 650c 6502 6a09 650c 1900  d.e.j.e.e.j.e...
-000000f0: 6602 1900 640a 6502 6a10 6508 1900 6606  f...d.e.j.e...f.
-00000100: 6416 6417 8404 5a12 640e 6504 6a0b 640a  d.d...Z.d.e.j.d.
-00000110: 6502 6a10 6508 1900 6604 6418 6419 8404  e.j.e...f.d.d...
-00000120: 5a13 6401 5300 291b e900 0000 004e 2901  Z.d.S.)......N).
-00000130: da04 4368 656d 2901 da0b 696e 7665 7274  ..Chem)...invert
-00000140: 5f64 6963 74e9 0400 0000 e905 0000 00e9  _dict...........
-00000150: 0600 0000 e907 0000 0029 06da 0143 da01  .........)...C..
-00000160: 4eda 0150 da01 4fda 0146 da02 436c da06  N..P..O..F..Cl..
-00000170: 736d 696c 6573 da06 7265 7475 726e 6302  smiles..returnc.
-00000180: 0000 0000 0000 0000 0000 0005 0000 0007  ................
-00000190: 0000 0043 0000 0073 5600 0000 7400 8300  ...C...sV...t...
-000001a0: 7d02 7401 a002 7c00 a101 7d03 7403 7c03  }.t...|...}.t.|.
-000001b0: 8301 7d04 7c02 a004 7405 7c03 7c01 7c04  ..}.|...t.|.|.|.
-000001c0: 6401 8d03 a101 0100 7c02 a004 7406 7c03  d.......|...t.|.
-000001d0: 7c04 6402 8d02 a101 0100 7c02 a004 7407  |.d.......|...t.
-000001e0: 7c03 6403 8d01 a101 0100 7408 7c02 8301  |.d.......t.|...
-000001f0: 5300 2904 4e29 03da 036d 6f6c da10 6174  S.).N)...mol..at
-00000200: 6f6d 5f76 616c 656e 6365 5f6d 6170 da18  om_valence_map..
-00000210: 6672 6565 5f76 616c 656e 6365 5f69 6e64  free_valence_ind
-00000220: 6963 6573 5f6d 6170 2902 7210 0000 0072  ices_map).r....r
-00000230: 1200 0000 2901 7210 0000 0029 09da 0373  ....).r....)...s
-00000240: 6574 7202 0000 00da 0d4d 6f6c 4672 6f6d  etr......MolFrom
-00000250: 536d 696c 6573 da14 6765 745f 6672 6565  Smiles..get_free
-00000260: 5f76 616c 656e 6365 5f6d 6170 da06 7570  _valence_map..up
-00000270: 6461 7465 da18 6765 745f 7661 6c69 645f  date..get_valid_
-00000280: 6174 6f6d 5f61 6464 6974 696f 6e73 da18  atom_additions..
-00000290: 6765 745f 7661 6c69 645f 626f 6e64 5f61  get_valid_bond_a
-000002a0: 6464 6974 696f 6e73 da17 6765 745f 7661  dditions..get_va
-000002b0: 6c69 645f 626f 6e64 5f72 656d 6f76 616c  lid_bond_removal
-000002c0: 73da 046c 6973 7429 0572 0e00 0000 7211  s..list).r....r.
-000002d0: 0000 00da 0d6e 6569 6768 626f 7273 5f73  .....neighbors_s
-000002e0: 6574 7210 0000 0072 1200 0000 a900 721c  etr....r......r.
-000002f0: 0000 00fa 542f 6d65 6469 612f 7373 642f  ....T/media/ssd/
-00000300: 5072 6f67 7261 6d6d 696e 672f 7667 645f  Programming/vgd_
-00000310: 636f 756e 7465 7266 6163 7475 616c 732f  counterfactuals/
-00000320: 7667 645f 636f 756e 7465 7266 6163 7475  vgd_counterfactu
-00000330: 616c 732f 6765 6e65 7261 7465 2f6d 6f6c  als/generate/mol
-00000340: 6563 756c 6573 2e70 79da 1067 6574 5f6e  ecules.py..get_n
-00000350: 6569 6768 626f 7268 6f6f 6412 0000 0073  eighborhood....s
-00000360: 2000 0000 0603 0a02 0801 0602 0201 0201   ...............
-00000370: 0201 08fd 0606 0201 0201 08fe 0605 0201  ................
-00000380: 08ff 0804 721e 0000 00e9 0800 0000 7210  ....r.........r.
-00000390: 0000 00da 0b6d 6178 5f76 616c 656e 6365  .....max_valence
-000003a0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
-000003b0: 0004 0000 0003 0000 0073 3200 0000 6900  .........s2...i.
-000003c0: 7d02 7400 6401 7c01 8302 4400 5d0f 8900  }.t.d.|...D.]...
-000003d0: 8700 6601 6402 6403 8408 7c00 a001 a100  ..f.d.d...|.....
-000003e0: 4400 8301 7c02 8800 3c00 7107 7c02 5300  D...|...<.q.|.S.
-000003f0: 2904 4ee9 0100 0000 6301 0000 0000 0000  ).N.....c.......
-00000400: 0000 0000 0002 0000 0004 0000 0013 0000  ................
-00000410: 0073 2000 0000 6700 7c00 5d0c 7d01 7c01  .s ...g.|.].}.|.
-00000420: a000 a100 8800 6b05 7202 7c01 a001 a100  ......k.r.|.....
-00000430: 9102 7102 5300 721c 0000 0029 02da 1047  ..q.S.r....)...G
-00000440: 6574 4e75 6d49 6d70 6c69 6369 7448 73da  etNumImplicitHs.
-00000450: 0647 6574 4964 7829 02da 022e 30da 0461  .GetIdx)....0..a
-00000460: 746f 6da9 01da 0169 721c 0000 0072 1d00  tom....ir....r..
-00000470: 0000 da0a 3c6c 6973 7463 6f6d 703e 2f00  ....<listcomp>/.
-00000480: 0000 730c 0000 0006 0002 020a 0102 fd06  ..s.............
-00000490: 0106 ff7a 2867 6574 5f66 7265 655f 7661  ...z(get_free_va
-000004a0: 6c65 6e63 655f 6d61 702e 3c6c 6f63 616c  lence_map.<local
-000004b0: 733e 2e3c 6c69 7374 636f 6d70 3e29 02da  s>.<listcomp>)..
-000004c0: 0572 616e 6765 da08 4765 7441 746f 6d73  .range..GetAtoms
-000004d0: 2903 7210 0000 0072 2000 0000 da06 7265  ).r....r .....re
-000004e0: 7375 6c74 721c 0000 0072 2600 0000 721d  sultr....r&...r.
-000004f0: 0000 0072 1500 0000 2c00 0000 730c 0000  ...r....,...s...
-00000500: 0004 010e 010a 0106 020c fe04 0672 1500  .............r..
-00000510: 0000 7211 0000 0072 1200 0000 6303 0000  ..r....r....c...
-00000520: 0000 0000 0000 0000 000e 0000 0008 0000  ................
-00000530: 0043 0000 0073 a400 0000 7400 8300 7d03  .C...s....t...}.
-00000540: 7401 6a02 6a03 7401 6a02 6a04 7401 6a02  t.j.j.t.j.j.t.j.
-00000550: 6a05 6401 9c03 7d04 7c04 a006 a100 4400  j.d...}.|.....D.
-00000560: 5d3c 5c02 7d05 7d06 7c02 7c05 1900 4400  ]<\.}.}.|.|...D.
-00000570: 5d33 7d07 7c01 a006 a100 4400 5d2c 5c02  ]3}.|.....D.],\.
-00000580: 7d08 7d09 7401 a007 7c00 a101 7d0a 7c0a  }.}.t...|...}.|.
-00000590: a008 7401 a009 7c08 a101 a101 7d0b 7c0a  ..t...|.....}.|.
-000005a0: a00a 7c07 7c0b 7c06 a103 0100 7401 6a0b  ..|.|.|.....t.j.
-000005b0: 7c0a 6402 6403 8d02 7d0c 7c0c 7243 7121  |.d.d...}.|.rCq!
-000005c0: 7401 a00c 7c0a a101 7d0d 7c03 a00d 7c0d  t...|...}.|...|.
-000005d0: a101 0100 7121 711b 7113 7c03 5300 2904  ....q!q.q.|.S.).
-000005e0: 4ea9 0372 2100 0000 e902 0000 00e9 0300  N..r!...........
-000005f0: 0000 54a9 01da 0b63 6174 6368 4572 726f  ..T....catchErro
-00000600: 7273 290e 7213 0000 0072 0200 0000 da08  rs).r....r......
-00000610: 426f 6e64 5479 7065 da06 5349 4e47 4c45  BondType..SINGLE
-00000620: da06 444f 5542 4c45 da06 5452 4950 4c45  ..DOUBLE..TRIPLE
-00000630: da05 6974 656d 73da 0552 574d 6f6c da07  ..items..RWMol..
-00000640: 4164 6441 746f 6dda 0441 746f 6dda 0741  AddAtom..Atom..A
-00000650: 6464 426f 6e64 da0b 5361 6e69 7469 7a65  ddBond..Sanitize
-00000660: 4d6f 6cda 0b4d 6f6c 546f 536d 696c 6573  Mol..MolToSmiles
-00000670: da03 6164 6429 0e72 1000 0000 7211 0000  ..add).r....r...
-00000680: 0072 1200 0000 da07 7265 7375 6c74 73da  .r......results.
-00000690: 1376 616c 7565 5f62 6f6e 645f 7479 7065  .value_bond_type
-000006a0: 5f6d 6170 7227 0000 00da 0962 6f6e 645f  _mapr'.....bond_
-000006b0: 7479 7065 7225 0000 00da 0765 6c65 6d65  typer%.....eleme
-000006c0: 6e74 da07 7661 6c65 6e63 65da 076e 6577  nt..valence..new
-000006d0: 5f6d 6f6c da03 6964 78da 1373 616e 6974  _mol..idx..sanit
-000006e0: 697a 6174 696f 6e5f 7265 7375 6c74 720e  ization_resultr.
-000006f0: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000700: 0000 7217 0000 0038 0000 0073 2600 0000  ..r....8...s&...
-00000710: 0604 0603 0601 0601 06fd 1005 0c02 1001  ................
-00000720: 0a01 1001 0e01 0e01 0401 0201 0a02 0c01  ................
-00000730: 02f7 02ff 040c 7217 0000 0063 0200 0000  ......r....c....
-00000740: 0000 0000 0000 0000 1000 0000 0700 0000  ................
-00000750: 4300 0000 7318 0100 0074 0083 007d 0264  C...s....t...}.d
-00000760: 0074 016a 026a 0374 016a 026a 0474 016a  .t.j.j.t.j.j.t.j
-00000770: 026a 0564 019c 047d 0374 067c 0383 017d  .j.d...}.t.|...}
-00000780: 047c 01a0 07a1 0044 005d 715c 027d 057d  .|.....D.]q\.}.}
-00000790: 0674 08a0 097c 0664 02a1 0244 005d 665c  .t...|.d...D.]f\
-000007a0: 027d 077d 0874 01a0 0a7c 00a1 01a0 0b7c  .}.}.t...|.....|
-000007b0: 077c 08a1 027d 0974 01a0 0c7c 00a1 017d  .|...}.t...|...}
-000007c0: 0a74 016a 0d7c 0a64 0364 048d 0201 007c  .t.j.|.d.d.....|
-000007d0: 0964 0075 0172 697c 09a0 0ea1 007d 0b7c  .d.u.ri|.....}.|
-000007e0: 0b7c 03a0 0fa1 0076 0172 4a71 227c 047c  .|.....v.rJq"|.|
-000007f0: 0b19 007d 0c7c 0c7c 0537 007d 0c7c 0c64  ...}.|.|.7.}.|.d
-00000800: 056b 0472 5771 227c 09a0 10a1 007d 0d7c  .k.rWq"|.....}.|
-00000810: 09a0 117c 037c 0c19 00a1 0101 007c 0aa0  ...|.|.......|..
-00000820: 127c 0d7c 09a1 0201 006e 0b7c 037c 0519  .|.|.....n.|.|..
-00000830: 007d 0b7c 0aa0 137c 077c 087c 0ba1 0301  .}.|...|.|.|....
-00000840: 0074 016a 147c 0a64 0364 068d 027d 0e7c  .t.j.|.d.d...}.|
-00000850: 0e72 7e71 2274 01a0 157c 0aa1 017d 0f7c  .r~q"t...|...}.|
-00000860: 02a0 167c 0fa1 0101 0071 2271 187c 0253  ...|.....q"q.|.S
-00000870: 0029 074e a904 7201 0000 0072 2100 0000  .).N..r....r!...
-00000880: 722d 0000 0072 2e00 0000 722d 0000 0054  r-...r....r-...T
-00000890: a901 da12 636c 6561 7241 726f 6d61 7469  ....clearAromati
-000008a0: 6346 6c61 6773 722e 0000 0072 2f00 0000  cFlagsr....r/...
-000008b0: 2917 7213 0000 0072 0200 0000 7231 0000  ).r....r....r1..
-000008c0: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
-000008d0: 7203 0000 0072 3500 0000 da09 6974 6572  r....r5.....iter
-000008e0: 746f 6f6c 73da 0c63 6f6d 6269 6e61 7469  tools..combinati
-000008f0: 6f6e 73da 034d 6f6c da13 4765 7442 6f6e  ons..Mol..GetBon
-00000900: 6442 6574 7765 656e 4174 6f6d 7372 3600  dBetweenAtomsr6.
-00000910: 0000 da08 4b65 6b75 6c69 7a65 da0b 4765  ....Kekulize..Ge
-00000920: 7442 6f6e 6454 7970 65da 0676 616c 7565  tBondType..value
-00000930: 7372 2300 0000 da0b 5365 7442 6f6e 6454  sr#.....SetBondT
-00000940: 7970 65da 0b52 6570 6c61 6365 426f 6e64  ype..ReplaceBond
-00000950: 7239 0000 0072 3a00 0000 723b 0000 0072  r9...r:...r;...r
-00000960: 3c00 0000 2910 7210 0000 0072 1200 0000  <...).r....r....
-00000970: 723d 0000 0072 3e00 0000 da13 626f 6e64  r=...r>.....bond
-00000980: 5f74 7970 655f 7661 6c75 655f 6d61 7072  _type_value_mapr
-00000990: 4100 0000 da05 6174 6f6d 73da 0561 746f  A.....atoms..ato
-000009a0: 6d31 da05 6174 6f6d 32da 0462 6f6e 6472  m1..atom2..bondr
-000009b0: 4200 0000 723f 0000 00da 0a62 6f6e 645f  B...r?.....bond_
-000009c0: 7661 6c75 65da 0569 6e64 6578 7244 0000  value..indexrD..
-000009d0: 0072 0e00 0000 721c 0000 0072 1c00 0000  .r....r....r....
-000009e0: 721d 0000 0072 1800 0000 5400 0000 7340  r....r....T...s@
-000009f0: 0000 0006 0302 0306 0106 0106 0106 fc08  ................
-00000a00: 0610 0214 0112 010a 010e 0208 0108 010c  ................
-00000a10: 0102 0108 0208 0108 0102 0108 020e 010e  ................
-00000a20: 0108 030e 010e 0204 0102 010a 020c 0102  ................
-00000a30: e404 1e72 1800 0000 6301 0000 0000 0000  ...r....c.......
-00000a40: 0000 0000 000f 0000 0006 0000 0043 0000  .............C..
-00000a50: 0073 4601 0000 7400 8300 7d01 6400 7401  .sF...t...}.d.t.
-00000a60: 6a02 6a03 7401 6a02 6a04 7401 6a02 6a05  j.j.t.j.j.t.j.j.
-00000a70: 6401 9c04 7d02 7406 7c02 8301 7d03 6402  d...}.t.|...}.d.
-00000a80: 4400 5d8a 7d04 7c00 a007 a100 4400 5d83  D.].}.|.....D.].
-00000a90: 7d05 7c05 a008 a100 7c05 a009 a100 0202  }.|.....|.......
-00000aa0: 7d06 7d07 7401 a00a 7c00 a101 a00b 7c06  }.}.t...|.....|.
-00000ab0: 7c07 a102 7d05 7c05 a00c a100 7d08 7c08  |...}.|.....}.|.
-00000ac0: 7c02 a00d a100 7601 723b 711c 7401 a00e  |.....v.r;q.t...
-00000ad0: 7c00 a101 7d09 7401 6a0f 7c09 6403 6404  |...}.t.j.|.d.d.
-00000ae0: 8d02 0100 7c03 7c08 1900 7d0a 7c0a 7c04  ....|.|...}.|.|.
-00000af0: 3800 7d0a 7c0a 6405 6b02 725a 7c09 a010  8.}.|.d.k.rZ|...
-00000b00: 7c06 7c07 a102 0100 6e17 7c0a 6405 6b04  |.|.....n.|.d.k.
-00000b10: 7270 7c05 a011 7c02 7c0a 1900 a101 0100  rp|...|.|.......
-00000b20: 7c05 a012 a100 7d0b 7c09 a013 7c0b 7c05  |.....}.|...|.|.
-00000b30: a102 0100 6e01 711c 7401 6a14 7c09 6403  ....n.q.t.j.|.d.
-00000b40: 6406 8d02 7d0c 7c0c 727b 711c 7401 a015  d...}.|.r{q.t...
-00000b50: 7c09 a101 7d0d 6407 7c0d 7600 729a 7416  |...}.d.|.v.r.t.
-00000b60: 7c0d a017 6407 a101 7418 6408 8d02 7d0e  |...d...t.d...}.
-00000b70: 7418 7c0e 6405 1900 8301 6409 6b04 7296  t.|.d.....d.k.r.
-00000b80: 711c 7c0e 6409 1900 7d0d 7c01 a019 7c0d  q.|.d...}.|...|.
-00000b90: a101 0100 711c 7116 7c01 5300 290a 4e72  ....q.q.|.S.).Nr
-00000ba0: 4500 0000 722c 0000 0054 7246 0000 0072  E...r,...TrF...r
-00000bb0: 0100 0000 722f 0000 00da 012e 2901 da03  ....r/......)...
-00000bc0: 6b65 7972 2100 0000 291a 7213 0000 0072  keyr!...).r....r
-00000bd0: 0200 0000 7231 0000 0072 3200 0000 7233  ....r1...r2...r3
-00000be0: 0000 0072 3400 0000 7203 0000 00da 0847  ...r4...r......G
-00000bf0: 6574 426f 6e64 73da 0f47 6574 4265 6769  etBonds..GetBegi
-00000c00: 6e41 746f 6d49 6478 da0d 4765 7445 6e64  nAtomIdx..GetEnd
-00000c10: 4174 6f6d 4964 7872 4a00 0000 724b 0000  AtomIdxrJ...rK..
-00000c20: 0072 4d00 0000 724e 0000 0072 3600 0000  .rM...rN...r6...
-00000c30: 724c 0000 00da 0a52 656d 6f76 6542 6f6e  rL.....RemoveBon
-00000c40: 6472 4f00 0000 7223 0000 0072 5000 0000  drO...r#...rP...
-00000c50: 723a 0000 0072 3b00 0000 da06 736f 7274  r:...r;.....sort
-00000c60: 6564 da05 7370 6c69 74da 036c 656e 723c  ed..split..lenr<
-00000c70: 0000 0029 0f72 1000 0000 723d 0000 0072  ...).r....r=...r
-00000c80: 3e00 0000 7251 0000 0072 4100 0000 7255  >...rQ...rA...rU
-00000c90: 0000 0072 5300 0000 7254 0000 0072 3f00  ...rS...rT...r?.
-00000ca0: 0000 7242 0000 0072 5600 0000 7257 0000  ..rB...rV...rW..
-00000cb0: 0072 4400 0000 720e 0000 00da 0570 6172  .rD...r......par
-00000cc0: 7473 721c 0000 0072 1c00 0000 721d 0000  tsr....r....r...
-00000cd0: 0072 1900 0000 8300 0000 734a 0000 0006  .r........sJ....
-00000ce0: 0202 0306 0106 0106 0106 fc08 0608 020c  ................
-00000cf0: 0112 0112 0108 020c 0102 010a 020e 0108  ................
-00000d00: 0208 0108 020e 0108 020e 0108 010e 0102  ................
-00000d10: 030e 0204 0102 010a 0208 0112 0110 0102  ................
-00000d20: 0108 020c 0202 db04 2772 1900 0000 2901  ........'r....).
-00000d30: 721f 0000 0029 1472 4800 0000 da06 7479  r....).rH.....ty
-00000d40: 7069 6e67 da01 74da 0572 646b 6974 7202  ping..t..rdkitr.
-00000d50: 0000 00da 1976 6764 5f63 6f75 6e74 6572  .....vgd_counter
-00000d60: 6661 6374 7561 6c73 2e75 7469 6c73 7203  factuals.utilsr.
-00000d70: 0000 00da 1844 4546 4155 4c54 5f41 544f  .....DEFAULT_ATO
-00000d80: 4d5f 5641 4c45 4e43 455f 4d41 50da 0373  M_VALENCE_MAP..s
-00000d90: 7472 da04 4c69 7374 721e 0000 0072 4a00  tr..Listr....rJ.
-00000da0: 0000 da03 696e 74da 0464 6963 7472 1500  ....int..dictr..
-00000db0: 0000 da04 4469 6374 da03 5365 7472 1700  ....Dict..Setr..
-00000dc0: 0000 7218 0000 0072 1900 0000 721c 0000  ..r....r....r...
-00000dd0: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000de0: da08 3c6d 6f64 756c 653e 0100 0000 733e  ..<module>....s>
-00000df0: 0000 0008 0008 010c 010c 0202 0402 0102  ................
-00000e00: 0102 0102 0102 0106 fa02 0b08 ff08 020a  ................
-00000e10: fe1a 1a08 0c0c 0102 ff12 0202 fe08 030a  ................
-00000e20: fd08 1c12 0102 ff08 020a fe08 2f08 010e  ............/...
-00000e30: ff                                       .
+00000060: 6408 6406 6409 9c07 5a07 6507 6601 640a  d.d.d...Z.e.f.d.
+00000070: 6508 640b 6502 6a09 6508 1900 6604 640c  e.d.e.j.e...f.d.
+00000080: 640d 8405 5a0a 641b 640f 6504 6a0b 6410  d...Z.d.d.e.j.d.
+00000090: 650c 640b 650d 6606 6411 6412 8405 5a0e  e.d.e.f.d.d...Z.
+000000a0: 640f 6504 6a0b 6413 6502 6a0f 6508 650c  d.e.j.d.e.j.e.e.
+000000b0: 6602 1900 6414 6502 6a0f 650c 6502 6a09  f...d.e.j.e.e.j.
+000000c0: 650c 1900 6602 1900 640b 6502 6a10 6508  e...f...d.e.j.e.
+000000d0: 1900 6608 6415 6416 8404 5a11 640f 6504  ..f.d.d...Z.d.e.
+000000e0: 6a0b 6414 6502 6a0f 650c 6502 6a09 650c  j.d.e.j.e.e.j.e.
+000000f0: 1900 6602 1900 640b 6502 6a10 6508 1900  ..f...d.e.j.e...
+00000100: 6606 6417 6418 8404 5a12 640f 6504 6a0b  f.d.d...Z.d.e.j.
+00000110: 640b 6502 6a10 6508 1900 6604 6419 641a  d.e.j.e...f.d.d.
+00000120: 8404 5a13 6401 5300 291c e900 0000 004e  ..Z.d.S.)......N
+00000130: 2901 da04 4368 656d 2901 da0b 696e 7665  )...Chem)...inve
+00000140: 7274 5f64 6963 74e9 0400 0000 e905 0000  rt_dict.........
+00000150: 00e9 0600 0000 e901 0000 00e9 0700 0000  ................
+00000160: 2907 da01 43da 014e da01 50da 014f da01  )...C..N..P..O..
+00000170: 46da 0243 6cda 0153 da06 736d 696c 6573  F..Cl..S..smiles
+00000180: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
+00000190: 0000 0000 0005 0000 0007 0000 0043 0000  .............C..
+000001a0: 0073 5600 0000 7400 8300 7d02 7401 a002  .sV...t...}.t...
+000001b0: 7c00 a101 7d03 7403 7c03 8301 7d04 7c02  |...}.t.|...}.|.
+000001c0: a004 7405 7c03 7c01 7c04 6401 8d03 a101  ..t.|.|.|.d.....
+000001d0: 0100 7c02 a004 7406 7c03 7c04 6402 8d02  ..|...t.|.|.d...
+000001e0: a101 0100 7c02 a004 7407 7c03 6403 8d01  ....|...t.|.d...
+000001f0: a101 0100 7408 7c02 8301 5300 2904 4e29  ....t.|...S.).N)
+00000200: 03da 036d 6f6c da10 6174 6f6d 5f76 616c  ...mol..atom_val
+00000210: 656e 6365 5f6d 6170 da18 6672 6565 5f76  ence_map..free_v
+00000220: 616c 656e 6365 5f69 6e64 6963 6573 5f6d  alence_indices_m
+00000230: 6170 2902 7212 0000 0072 1400 0000 2901  ap).r....r....).
+00000240: 7212 0000 0029 09da 0373 6574 7202 0000  r....)...setr...
+00000250: 00da 0d4d 6f6c 4672 6f6d 536d 696c 6573  ...MolFromSmiles
+00000260: da14 6765 745f 6672 6565 5f76 616c 656e  ..get_free_valen
+00000270: 6365 5f6d 6170 da06 7570 6461 7465 da18  ce_map..update..
+00000280: 6765 745f 7661 6c69 645f 6174 6f6d 5f61  get_valid_atom_a
+00000290: 6464 6974 696f 6e73 da18 6765 745f 7661  dditions..get_va
+000002a0: 6c69 645f 626f 6e64 5f61 6464 6974 696f  lid_bond_additio
+000002b0: 6e73 da17 6765 745f 7661 6c69 645f 626f  ns..get_valid_bo
+000002c0: 6e64 5f72 656d 6f76 616c 73da 046c 6973  nd_removals..lis
+000002d0: 7429 0572 1000 0000 7213 0000 00da 0d6e  t).r....r......n
+000002e0: 6569 6768 626f 7273 5f73 6574 7212 0000  eighbors_setr...
+000002f0: 0072 1400 0000 a900 721e 0000 00fa 542f  .r......r.....T/
+00000300: 6d65 6469 612f 7373 642f 5072 6f67 7261  media/ssd/Progra
+00000310: 6d6d 696e 672f 7667 645f 636f 756e 7465  mming/vgd_counte
+00000320: 7266 6163 7475 616c 732f 7667 645f 636f  rfactuals/vgd_co
+00000330: 756e 7465 7266 6163 7475 616c 732f 6765  unterfactuals/ge
+00000340: 6e65 7261 7465 2f6d 6f6c 6563 756c 6573  nerate/molecules
+00000350: 2e70 79da 1067 6574 5f6e 6569 6768 626f  .py..get_neighbo
+00000360: 7268 6f6f 6414 0000 0073 2000 0000 0603  rhood....s .....
+00000370: 0a02 0801 0602 0201 0201 0201 08fd 0606  ................
+00000380: 0201 0201 08fe 0605 0201 08ff 0804 7220  ..............r 
+00000390: 0000 00e9 0800 0000 7212 0000 00da 0b6d  ........r......m
+000003a0: 6178 5f76 616c 656e 6365 6302 0000 0000  ax_valencec.....
+000003b0: 0000 0000 0000 0003 0000 0004 0000 0003  ................
+000003c0: 0000 0073 3200 0000 6900 7d02 7400 6401  ...s2...i.}.t.d.
+000003d0: 7c01 8302 4400 5d0f 8900 8700 6601 6402  |...D.].....f.d.
+000003e0: 6403 8408 7c00 a001 a100 4400 8301 7c02  d...|.....D...|.
+000003f0: 8800 3c00 7107 7c02 5300 2904 4e72 0700  ..<.q.|.S.).Nr..
+00000400: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00000410: 0000 0004 0000 0013 0000 0073 2000 0000  ...........s ...
+00000420: 6700 7c00 5d0c 7d01 7c01 a000 a100 8800  g.|.].}.|.......
+00000430: 6b05 7202 7c01 a001 a100 9102 7102 5300  k.r.|.......q.S.
+00000440: 721e 0000 0029 02da 1047 6574 4e75 6d49  r....)...GetNumI
+00000450: 6d70 6c69 6369 7448 73da 0647 6574 4964  mplicitHs..GetId
+00000460: 7829 02da 022e 30da 0461 746f 6da9 01da  x)....0..atom...
+00000470: 0169 721e 0000 0072 1f00 0000 da0a 3c6c  .ir....r......<l
+00000480: 6973 7463 6f6d 703e 3100 0000 730c 0000  istcomp>1...s...
+00000490: 0006 0002 020a 0102 fd06 0106 ff7a 2867  .............z(g
+000004a0: 6574 5f66 7265 655f 7661 6c65 6e63 655f  et_free_valence_
+000004b0: 6d61 702e 3c6c 6f63 616c 733e 2e3c 6c69  map.<locals>.<li
+000004c0: 7374 636f 6d70 3e29 02da 0572 616e 6765  stcomp>)...range
+000004d0: da08 4765 7441 746f 6d73 2903 7212 0000  ..GetAtoms).r...
+000004e0: 0072 2200 0000 da06 7265 7375 6c74 721e  .r".....resultr.
+000004f0: 0000 0072 2700 0000 721f 0000 0072 1700  ...r'...r....r..
+00000500: 0000 2e00 0000 730c 0000 0004 010e 010a  ......s.........
+00000510: 0106 020c fe04 0672 1700 0000 7213 0000  .......r....r...
+00000520: 0072 1400 0000 6303 0000 0000 0000 0000  .r....c.........
+00000530: 0000 000e 0000 0008 0000 0043 0000 0073  ...........C...s
+00000540: a400 0000 7400 8300 7d03 7401 6a02 6a03  ....t...}.t.j.j.
+00000550: 7401 6a02 6a04 7401 6a02 6a05 6401 9c03  t.j.j.t.j.j.d...
+00000560: 7d04 7c04 a006 a100 4400 5d3c 5c02 7d05  }.|.....D.]<\.}.
+00000570: 7d06 7c02 7c05 1900 4400 5d33 7d07 7c01  }.|.|...D.]3}.|.
+00000580: a006 a100 4400 5d2c 5c02 7d08 7d09 7401  ....D.],\.}.}.t.
+00000590: a007 7c00 a101 7d0a 7c0a a008 7401 a009  ..|...}.|...t...
+000005a0: 7c08 a101 a101 7d0b 7c0a a00a 7c07 7c0b  |.....}.|...|.|.
+000005b0: 7c06 a103 0100 7401 6a0b 7c0a 6402 6403  |.....t.j.|.d.d.
+000005c0: 8d02 7d0c 7c0c 7243 7121 7401 a00c 7c0a  ..}.|.rCq!t...|.
+000005d0: a101 7d0d 7c03 a00d 7c0d a101 0100 7121  ..}.|...|.....q!
+000005e0: 711b 7113 7c03 5300 2904 4ea9 0372 0700  q.q.|.S.).N..r..
+000005f0: 0000 e902 0000 00e9 0300 0000 54a9 01da  ............T...
+00000600: 0b63 6174 6368 4572 726f 7273 290e 7215  .catchErrors).r.
+00000610: 0000 0072 0200 0000 da08 426f 6e64 5479  ...r......BondTy
+00000620: 7065 da06 5349 4e47 4c45 da06 444f 5542  pe..SINGLE..DOUB
+00000630: 4c45 da06 5452 4950 4c45 da05 6974 656d  LE..TRIPLE..item
+00000640: 73da 0552 574d 6f6c da07 4164 6441 746f  s..RWMol..AddAto
+00000650: 6dda 0441 746f 6dda 0741 6464 426f 6e64  m..Atom..AddBond
+00000660: da0b 5361 6e69 7469 7a65 4d6f 6cda 0b4d  ..SanitizeMol..M
+00000670: 6f6c 546f 536d 696c 6573 da03 6164 6429  olToSmiles..add)
+00000680: 0e72 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000690: da07 7265 7375 6c74 73da 1376 616c 7565  ..results..value
+000006a0: 5f62 6f6e 645f 7479 7065 5f6d 6170 7228  _bond_type_mapr(
+000006b0: 0000 00da 0962 6f6e 645f 7479 7065 7226  .....bond_typer&
+000006c0: 0000 00da 0765 6c65 6d65 6e74 da07 7661  .....element..va
+000006d0: 6c65 6e63 65da 076e 6577 5f6d 6f6c da03  lence..new_mol..
+000006e0: 6964 78da 1373 616e 6974 697a 6174 696f  idx..sanitizatio
+000006f0: 6e5f 7265 7375 6c74 7210 0000 0072 1e00  n_resultr....r..
+00000700: 0000 721e 0000 0072 1f00 0000 7219 0000  ..r....r....r...
+00000710: 003a 0000 0073 2600 0000 0604 0603 0601  .:...s&.........
+00000720: 0601 06fd 1005 0c02 1001 0a01 1001 0e01  ................
+00000730: 0e01 0401 0201 0a02 0c01 02f7 02ff 040c  ................
+00000740: 7219 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00000750: 0000 1000 0000 0700 0000 4300 0000 7336  ..........C...s6
+00000760: 0100 0074 0083 007d 0264 0074 016a 026a  ...t...}.d.t.j.j
+00000770: 0374 016a 026a 0474 016a 026a 0564 019c  .t.j.j.t.j.j.d..
+00000780: 047d 0374 067c 0383 017d 047c 01a0 07a1  .}.t.|...}.|....
+00000790: 0044 005d 805c 027d 057d 0674 08a0 097c  .D.].\.}.}.t...|
+000007a0: 0664 02a1 0244 005d 755c 027d 077d 087c  .d...D.]u\.}.}.|
+000007b0: 00a0 0a7c 07a1 01a0 0ba1 0072 357c 00a0  ...|.......r5|..
+000007c0: 0a7c 08a1 01a0 0ba1 0072 3571 2274 01a0  .|.......r5q"t..
+000007d0: 0c7c 00a1 01a0 0d7c 077c 08a1 027d 0974  .|.....|.|...}.t
+000007e0: 01a0 0e7c 00a1 017d 0a74 016a 0f7c 0a64  ...|...}.t.j.|.d
+000007f0: 0364 048d 0201 007c 0964 0075 0172 787c  .d.....|.d.u.rx|
+00000800: 09a0 10a1 007d 0b7c 0b7c 03a0 11a1 0076  .....}.|.|.....v
+00000810: 0172 5971 227c 047c 0b19 007d 0c7c 0c7c  .rYq"|.|...}.|.|
+00000820: 0537 007d 0c7c 0c64 056b 0472 6671 227c  .7.}.|.d.k.rfq"|
+00000830: 09a0 12a1 007d 0d7c 09a0 137c 037c 0c19  .....}.|...|.|..
+00000840: 00a1 0101 007c 0aa0 147c 0d7c 09a1 0201  .....|...|.|....
+00000850: 006e 0b7c 037c 0519 007d 0b7c 0aa0 157c  .n.|.|...}.|...|
+00000860: 077c 087c 0ba1 0301 0074 016a 167c 0a64  .|.|.....t.j.|.d
+00000870: 0364 068d 027d 0e7c 0e72 8d71 2274 01a0  .d...}.|.r.q"t..
+00000880: 177c 0aa1 017d 0f7c 02a0 187c 0fa1 0101  .|...}.|...|....
+00000890: 0071 2271 187c 0253 0029 074e a904 7201  .q"q.|.S.).N..r.
+000008a0: 0000 0072 0700 0000 722e 0000 0072 2f00  ...r....r....r/.
+000008b0: 0000 722e 0000 0054 a901 da12 636c 6561  ..r....T....clea
+000008c0: 7241 726f 6d61 7469 6346 6c61 6773 722f  rAromaticFlagsr/
+000008d0: 0000 0072 3000 0000 2919 7215 0000 0072  ...r0...).r....r
+000008e0: 0200 0000 7232 0000 0072 3300 0000 7234  ....r2...r3...r4
+000008f0: 0000 0072 3500 0000 7203 0000 0072 3600  ...r5...r....r6.
+00000900: 0000 da09 6974 6572 746f 6f6c 73da 0c63  ....itertools..c
+00000910: 6f6d 6269 6e61 7469 6f6e 73da 0e47 6574  ombinations..Get
+00000920: 4174 6f6d 5769 7468 4964 78da 0849 7349  AtomWithIdx..IsI
+00000930: 6e52 696e 67da 034d 6f6c da13 4765 7442  nRing..Mol..GetB
+00000940: 6f6e 6442 6574 7765 656e 4174 6f6d 7372  ondBetweenAtomsr
+00000950: 3700 0000 da08 4b65 6b75 6c69 7a65 da0b  7.....Kekulize..
+00000960: 4765 7442 6f6e 6454 7970 65da 0676 616c  GetBondType..val
+00000970: 7565 7372 2400 0000 da0b 5365 7442 6f6e  uesr$.....SetBon
+00000980: 6454 7970 65da 0b52 6570 6c61 6365 426f  dType..ReplaceBo
+00000990: 6e64 723a 0000 0072 3b00 0000 723c 0000  ndr:...r;...r<..
+000009a0: 0072 3d00 0000 2910 7212 0000 0072 1400  .r=...).r....r..
+000009b0: 0000 723e 0000 0072 3f00 0000 da13 626f  ..r>...r?.....bo
+000009c0: 6e64 5f74 7970 655f 7661 6c75 655f 6d61  nd_type_value_ma
+000009d0: 7072 4200 0000 da05 6174 6f6d 73da 0561  prB.....atoms..a
+000009e0: 746f 6d31 da05 6174 6f6d 32da 0462 6f6e  tom1..atom2..bon
+000009f0: 6472 4300 0000 7240 0000 00da 0a62 6f6e  drC...r@.....bon
+00000a00: 645f 7661 6c75 65da 0569 6e64 6578 7245  d_value..indexrE
+00000a10: 0000 0072 1000 0000 721e 0000 0072 1e00  ...r....r....r..
+00000a20: 0000 721f 0000 0072 1a00 0000 5600 0000  ..r....r....V...
+00000a30: 7344 0000 0006 0302 0306 0106 0106 0106  sD..............
+00000a40: fc08 0610 0214 011c 0302 0112 020a 010e  ................
+00000a50: 0208 0108 010c 0102 0108 0208 0108 0102  ................
+00000a60: 0108 020e 010e 0108 030e 010e 0204 0102  ................
+00000a70: 010a 020c 0102 df04 2372 1a00 0000 6301  ........#r....c.
+00000a80: 0000 0000 0000 0000 0000 000f 0000 0007  ................
+00000a90: 0000 0043 0000 0073 6201 0000 7400 8300  ...C...sb...t...
+00000aa0: 7d01 6400 7401 6a02 6a03 7401 6a02 6a04  }.d.t.j.j.t.j.j.
+00000ab0: 7401 6a02 6a05 6401 9c04 7d02 7406 7c02  t.j.j.d...}.t.|.
+00000ac0: 8301 7d03 6402 4400 5d98 7d04 7c00 a007  ..}.d.D.].}.|...
+00000ad0: a100 4400 5d91 7d05 7c05 a008 a100 7c05  ..D.].}.|.....|.
+00000ae0: a009 a100 0202 7d06 7d07 7401 a00a 7c00  ......}.}.t...|.
+00000af0: a101 a00b 7c06 7c07 a102 7d05 7c05 a00c  ....|.|...}.|...
+00000b00: a100 7d08 7c08 7c02 a00d a100 7601 723b  ..}.|.|.....v.r;
+00000b10: 711c 7401 a00e 7c00 a101 7d09 7401 6a0f  q.t...|...}.t.j.
+00000b20: 7c09 6403 6404 8d02 0100 7c03 7c08 1900  |.d.d.....|.|...
+00000b30: 7d0a 7c0a 7c04 3800 7d0a 7c0a 6405 6b02  }.|.|.8.}.|.d.k.
+00000b40: 725a 7c09 a010 7c06 7c07 a102 0100 6e17  rZ|...|.|.....n.
+00000b50: 7c0a 6405 6b04 7270 7c05 a011 7c02 7c0a  |.d.k.rp|...|.|.
+00000b60: 1900 a101 0100 7c05 a012 a100 7d0b 7c09  ......|.....}.|.
+00000b70: a013 7c0b 7c05 a102 0100 6e01 711c 7401  ..|.|.....n.q.t.
+00000b80: 6a14 7c09 6403 6406 8d02 7d0c 7c0c 727b  j.|.d.d...}.|.r{
+00000b90: 711c 7401 a015 7c09 a101 7d0d 6407 7c0d  q.t...|...}.d.|.
+00000ba0: 7600 72a8 7416 7c0d a017 6407 a101 7418  v.r.t.|...d...t.
+00000bb0: 6408 8d02 7d0e 7418 7c0e 6405 1900 8301  d...}.t.|.d.....
+00000bc0: 6409 6b04 7296 711c 7418 7401 a019 7c0e  d.k.r.q.t.t...|.
+00000bd0: 6409 1900 a101 a01a a100 8301 640a 6b00  d...........d.k.
+00000be0: 72a4 711c 7c0e 6409 1900 7d0d 7c01 a01b  r.q.|.d...}.|...
+00000bf0: 7c0d a101 0100 711c 7116 7c01 5300 290b  |.....q.q.|.S.).
+00000c00: 4e72 4600 0000 722d 0000 0054 7247 0000  NrF...r-...TrG..
+00000c10: 0072 0100 0000 7230 0000 00da 012e 2901  .r....r0......).
+00000c20: da03 6b65 7972 0700 0000 722e 0000 0029  ..keyr....r....)
+00000c30: 1c72 1500 0000 7202 0000 0072 3200 0000  .r....r....r2...
+00000c40: 7233 0000 0072 3400 0000 7235 0000 0072  r3...r4...r5...r
+00000c50: 0300 0000 da08 4765 7442 6f6e 6473 da0f  ......GetBonds..
+00000c60: 4765 7442 6567 696e 4174 6f6d 4964 78da  GetBeginAtomIdx.
+00000c70: 0d47 6574 456e 6441 746f 6d49 6478 724d  .GetEndAtomIdxrM
+00000c80: 0000 0072 4e00 0000 7250 0000 0072 5100  ...rN...rP...rQ.
+00000c90: 0000 7237 0000 0072 4f00 0000 da0a 5265  ..r7...rO.....Re
+00000ca0: 6d6f 7665 426f 6e64 7252 0000 0072 2400  moveBondrR...r$.
+00000cb0: 0000 7253 0000 0072 3b00 0000 723c 0000  ..rS...r;...r<..
+00000cc0: 00da 0673 6f72 7465 64da 0573 706c 6974  ...sorted..split
+00000cd0: da03 6c65 6e72 1600 0000 722b 0000 0072  ..lenr....r+...r
+00000ce0: 3d00 0000 290f 7212 0000 0072 3e00 0000  =...).r....r>...
+00000cf0: 723f 0000 0072 5400 0000 7242 0000 0072  r?...rT...rB...r
+00000d00: 5800 0000 7256 0000 0072 5700 0000 7240  X...rV...rW...r@
+00000d10: 0000 0072 4300 0000 7259 0000 0072 5a00  ...rC...rY...rZ.
+00000d20: 0000 7245 0000 0072 1000 0000 da05 7061  ..rE...r......pa
+00000d30: 7274 7372 1e00 0000 721e 0000 0072 1f00  rtsr....r....r..
+00000d40: 0000 721b 0000 008a 0000 0073 4e00 0000  ..r........sN...
+00000d50: 0602 0203 0601 0601 0601 06fc 0806 0802  ................
+00000d60: 0c01 1201 1201 0802 0c01 0201 0a02 0e01  ................
+00000d70: 0802 0801 0802 0e01 0802 0e01 0801 0e01  ................
+00000d80: 0203 0e02 0401 0201 0a02 0801 1201 1001  ................
+00000d90: 0201 1a06 0201 0802 0c02 02d4 042e 721b  ..............r.
+00000da0: 0000 0029 0172 2100 0000 2914 7249 0000  ...).r!...).rI..
+00000db0: 00da 0674 7970 696e 67da 0174 da05 7264  ...typing..t..rd
+00000dc0: 6b69 7472 0200 0000 da19 7667 645f 636f  kitr......vgd_co
+00000dd0: 756e 7465 7266 6163 7475 616c 732e 7574  unterfactuals.ut
+00000de0: 696c 7372 0300 0000 da18 4445 4641 554c  ilsr......DEFAUL
+00000df0: 545f 4154 4f4d 5f56 414c 454e 4345 5f4d  T_ATOM_VALENCE_M
+00000e00: 4150 da03 7374 72da 044c 6973 7472 2000  AP..str..Listr .
+00000e10: 0000 724d 0000 00da 0369 6e74 da04 6469  ..rM.....int..di
+00000e20: 6374 7217 0000 00da 0444 6963 74da 0353  ctr......Dict..S
+00000e30: 6574 7219 0000 0072 1a00 0000 721b 0000  etr....r....r...
+00000e40: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00000e50: 721f 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000e60: 0000 0073 4000 0000 0800 0801 0c01 0c02  ...s@...........
+00000e70: 0204 0201 0201 0201 0201 0201 0201 06f9  ................
+00000e80: 020d 08ff 0802 0afe 1a1a 080c 0c01 02ff  ................
+00000e90: 1202 02fe 0803 0afd 081c 1201 02ff 0802  ................
+00000ea0: 0afe 0834 0801 0eff                      ...4....
```

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/generate/molecules.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/molecules.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 
 DEFAULT_ATOM_VALENCE_MAP = {
     'C': 4,
     'N': 5,
     'P': 5,
     'O': 6,
-    'F': 7,
+    'F': 1,
     'Cl': 7,
+    'S': 6,
+
 }
 
 
 def get_neighborhood(smiles: str,
                      atom_valence_map=DEFAULT_ATOM_VALENCE_MAP
                      ) -> t.List[str]:
     neighbors_set = set()
@@ -92,14 +94,19 @@
         2: Chem.BondType.DOUBLE,
         3: Chem.BondType.TRIPLE,
     }
     bond_type_value_map = invert_dict(value_bond_type_map)
 
     for valence, atoms in free_valence_indices_map.items():
         for atom1, atom2 in itertools.combinations(atoms, 2):
+
+            # We don't even want to entertain bonds between two atoms which are already part of rings
+            if mol.GetAtomWithIdx(atom1).IsInRing() and mol.GetAtomWithIdx(atom2).IsInRing():
+                continue
+
             bond = Chem.Mol(mol).GetBondBetweenAtoms(atom1, atom2)
             new_mol = Chem.RWMol(mol)
 
             Chem.Kekulize(new_mol, clearAromaticFlags=True)
             if bond is not None:
                 bond_type = bond.GetBondType()
                 if bond_type not in value_bond_type_map.values():
@@ -172,13 +179,20 @@
 
             smiles = Chem.MolToSmiles(new_mol)
             if '.' in smiles:
                 parts = sorted(smiles.split('.'), key=len)
                 if len(parts[0]) > 1:
                     continue
 
+                # 10.05.23 - Not filtering this has caused a bug in the down stream machine learning because
+                # we would have essentially allowed "molecules" only consisting of a single atom and those
+                # "graphs" would have no edges at all, which is a case that graph neural networks are not
+                # prepared to handle.
+                if len(Chem.MolFromSmiles(parts[1]).GetAtoms()) < 2:
+                    continue
+
                 smiles = parts[1]
 
             results.add(smiles)
 
     return results
```

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/generate/smiles_one_step_changes.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/generate/smiles_one_step_changes.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/templates/article.tex.j2` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/utils.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/utils.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/vgd_counterfactuals/visualization.py` & `vgd_counterfactuals-0.1.1/vgd_counterfactuals/visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.0/PKG-INFO` & `vgd_counterfactuals-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgd-counterfactuals
-Version: 0.1.0
+Version: 0.1.1
 Summary: Counterfactual explanations for GNNs based on the visual graph dataset format
 License: MIT
 Keywords: graph neural networks,counterfactuals,explainable AI
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
@@ -32,15 +32,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.0-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.1.1-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

