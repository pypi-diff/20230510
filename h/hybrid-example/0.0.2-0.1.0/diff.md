# Comparing `tmp/hybrid_example-0.0.2.tar.gz` & `tmp/hybrid_example-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybrid_example-0.0.2.tar", last modified: Tue May  9 05:36:33 2023, max compression
+gzip compressed data, was "hybrid_example-0.1.0.tar", last modified: Wed May 10 03:25:41 2023, max compression
```

## Comparing `hybrid_example-0.0.2.tar` & `hybrid_example-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/.vscode/c_cpp_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/docs/source/github_actions.md
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/docs/source/scbuild.md
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/docs/source/vscode.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/src/example_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/src/example_lib/example.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/src/hybrid_example/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/src/hybrid_example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/src/hybrid_example.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-09 05:36:33.000000 hybrid_example-0.0.2/src/hybrid_example.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-09 05:36:33.000000 hybrid_example-0.0.2/src/hybrid_example.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:36:33.000000 hybrid_example-0.0.2/src/hybrid_example.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 05:36:33.000000 hybrid_example-0.0.2/src/hybrid_example.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 05:36:33.000000 hybrid_example-0.0.2/src/hybrid_example.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:33.292559 hybrid_example-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-09 05:36:24.000000 hybrid_example-0.0.2/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.740960 hybrid_example-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.728961 hybrid_example-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.732961 hybrid_example-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.732961 hybrid_example-0.1.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/.vscode/c_cpp_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-10 03:25:41.736961 hybrid_example-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.732961 hybrid_example-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.736961 hybrid_example-0.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/source/github_actions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/source/pypi.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/source/scbuild.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/docs/source/vscode.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:25:41.740960 hybrid_example-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.728961 hybrid_example-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.736961 hybrid_example-0.1.0/src/example_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/src/example_lib/example.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.736961 hybrid_example-0.1.0/src/hybrid_example/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/src/hybrid_example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.736961 hybrid_example-0.1.0/src/hybrid_example.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-10 03:25:41.000000 hybrid_example-0.1.0/src/hybrid_example.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-10 03:25:41.000000 hybrid_example-0.1.0/src/hybrid_example.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:25:41.000000 hybrid_example-0.1.0/src/hybrid_example.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:25:41.000000 hybrid_example-0.1.0/src/hybrid_example.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:25:41.000000 hybrid_example-0.1.0/src/hybrid_example.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:41.736961 hybrid_example-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-10 03:25:32.000000 hybrid_example-0.1.0/test/test.py
```

### Comparing `hybrid_example-0.0.2/.github/workflows/CI.yml` & `hybrid_example-0.1.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/.github/workflows/python-publish.yml` & `hybrid_example-0.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/.gitignore` & `hybrid_example-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/.readthedocs.yaml` & `hybrid_example-0.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/.vscode/c_cpp_properties.json` & `hybrid_example-0.1.0/.vscode/c_cpp_properties.json`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/CMakeLists.txt` & `hybrid_example-0.1.0/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # project
 cmake_minimum_required(VERSION 3.13.0)
-project(hybrid_programming VERSION "0.0.2")
+project(hybrid_programming)
 set(CMAKE_CXX_STANDARD 17)
 
 if(SKBUILD)
   # Scikit-Build does not add your site-packages to the search path
   # automatically, so we need to add it _or_ the pybind11 specific directory
   # here.
   execute_process(
```

### Comparing `hybrid_example-0.0.2/LICENSE` & `hybrid_example-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/README.md` & `hybrid_example-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # hybrid_programming
 
 [![Build Status](https://github.com/YaozhenghangMa/hybrid_programming/actions/workflows/CI.yml/badge.svg?branch=)](https://github.com/YaozhenghangMa/hybrid_programming/actions/workflows/CI.yml?query=branch%3A)
 [![Coverage](https://codecov.io/gh/YaozhenghangMa/hybrid_programming/branch/main/graph/badge.svg)](https://codecov.io/gh/YaozhenghangMa/hybrid_programming)
-[![PyPI](https://img.shields.io/pypi/v/hybrid_programming)](https://pypi.org/project/hybrid_programming/)
+[![PyPI](https://img.shields.io/pypi/v/hybrid_example)](https://pypi.org/project/hybrid_example/)
+[![Documentation Status](https://readthedocs.org/projects/hybrid-programming/badge/?version=latest)](https://hybrid-programming.readthedocs.io/en/latest/?badge=latest)
 ![License](https://img.shields.io/github/license/yaozhenghangma/hybrid_programming)
 
 This package aims to offer tutorials on hybrid programming using C++ and Python. The tutorials cover the following topics:
 
 * Set up programming environment on [VSCode](https://code.visualstudio.com)
 * Compilation with [scikit-build](https://github.com/scikit-build/scikit-build)
 * Hybrid programming via [pybind11](https://github.com/pybind/pybind11)
```

### Comparing `hybrid_example-0.0.2/docs/make.bat` & `hybrid_example-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/docs/source/conf.py` & `hybrid_example-0.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/docs/source/github_actions.md` & `hybrid_example-0.1.0/docs/source/github_actions.md`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/docs/source/index.md` & `hybrid_example-0.1.0/docs/source/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 **hybrid_programming**  is a package aiming to offer tutorials on hybrid programming using C++ and Python. The tutorials cover the following topics:
 * Set up programming environment on [VSCode](https://code.visualstudio.com)
 * Compilation with [scikit-build](https://github.com/scikit-build/scikit-build)
 * Hybrid programming via [pybind11](https://github.com/pybind/pybind11)
 * Multiprocessing via [mpi4py](https://github.com/mpi4py/mpi4py)
 * Continuous integration with [Github Actions](https://github.com/features/actions)
 * Testing with [pytest](https://docs.pytest.org/en/7.3.x/)
-* Register package on [pypi](https://pypi.org)
+* Register package on [PyPI](https://pypi.org)
 * Publish documents on [Read the Docs](https://readthedocs.org)
 
 ## Contents
 
 ```{eval-rst}
 .. toctree::
    vscode
    scbuild
    github_actions
+   pypi
    api
 ```
```

### Comparing `hybrid_example-0.0.2/docs/source/scbuild.md` & `hybrid_example-0.1.0/docs/source/scbuild.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 `setup.py` is config file used by Python's setuptools. It consists of basic information about the project. To activate Sckikit-Build tools, the `setup` function must be overloaded by function provided by Scikit-Build in `setup.py`:
 ```python
 from skbuild import setup
 ```
 An example of `setup.py` can be found [here](https://github.com/yaozhenghangma/hybrid_programming/blob/main/setup.py). The additional options in `setup.py` are listed on [Scikit-Build's website](https://scikit-build.readthedocs.io/en/latest/usage.html#setup-options) and [Python's document](https://docs.python.org/3/distutils/setupscript.html).
 
 ## `pyproject.toml`
-`pyproject.toml` is the specified file format of [PEP 518](https://peps.python.org/pep-0518/), which contains the building system requirements of the project. A detailed description of `pyproject.toml` can be found in [pip's document](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/). Here, we only utilize a simplified yet practical version that is suitable for most scenarios:
+`pyproject.toml` is the specified file format of [PEP 518](https://peps.python.org/pep-0518/), which contains the dependencies of the project. A detailed description of `pyproject.toml` can be found in [pip's document](https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/). Here, we only utilize a simplified yet practical version that is suitable for most scenarios:
 ```toml
 [build-system]
 requires = [
     "setuptools>=42",
     "cmake>=3.13",
     "scikit-build>=0.14.1",
+    "pybind11>=2.9.2",
 ]
 
 build-backend = "setuptools.build_meta"
 ```
 
 ## `CMakeLists.txt`
 `CMakeLists.txt` file contains building options of CMake. To correctly build a pybind11 project, the location of pybind11 must be provided to CMake:
```

### Comparing `hybrid_example-0.0.2/docs/source/vscode.md` & `hybrid_example-0.1.0/docs/source/vscode.md`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/setup.py` & `hybrid_example-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     )
     raise
 
 from setuptools import find_packages
 
 setup(
     name="hybrid_example",
-    version="0.0.2",
-    description="Dynamical mean field theory package for material research.",
+    version="0.1.0",
+    description="Tutorials about hybrid programming using C++ and Python",
     author="Yaozhenghang Ma",
     author_email="Yaozhenghang.Ma@gmail.com",
     license="MIT",
     url="https://github.com/yaozhenghangma/hybrid_programming/",
     project_urls={
         "Bug Tracker": "https://github.com/yaozhenghangma/hybrid_programming/issues/",
         "Documentation": "https://hybrid_programming.readthedocs.io/",
```

### Comparing `hybrid_example-0.0.2/src/example_lib/example.cpp` & `hybrid_example-0.1.0/src/example_lib/example.cpp`

 * *Files identical despite different names*

### Comparing `hybrid_example-0.0.2/src/hybrid_example.egg-info/SOURCES.txt` & `hybrid_example-0.1.0/src/hybrid_example.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .vscode/c_cpp_properties.json
 docs/make.bat
 docs/requirements.txt
 docs/source/api.rst
 docs/source/conf.py
 docs/source/github_actions.md
 docs/source/index.md
+docs/source/pypi.md
 docs/source/scbuild.md
 docs/source/vscode.md
 src/example_lib/example.cpp
 src/hybrid_example/__init__.py
 src/hybrid_example.egg-info/PKG-INFO
 src/hybrid_example.egg-info/SOURCES.txt
 src/hybrid_example.egg-info/dependency_links.txt
```

