# Comparing `tmp/ezq-2.0.2.tar.gz` & `tmp/ezq-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezq-2.0.2.tar", last modified: Tue Aug 24 17:46:02 2021, max compression
+gzip compressed data, was "ezq-2.0.3.tar", last modified: Wed May 10 04:14:00 2023, max compression
```

## Comparing `ezq-2.0.2.tar` & `ezq-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 17:46:02.921580 ezq-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-08-24 17:45:48.000000 ezq-2.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     7046 2021-08-24 17:46:02.921580 ezq-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6407 2021-08-24 17:45:48.000000 ezq-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-08-24 17:45:48.000000 ezq-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-08-24 17:46:02.921580 ezq-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2021-08-24 17:45:48.000000 ezq-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 17:46:02.917580 ezq-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 17:46:02.917580 ezq-2.0.2/src/ezq/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2021-08-24 17:45:48.000000 ezq-2.0.2/src/ezq/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5695 2021-08-24 17:45:48.000000 ezq-2.0.2/src/ezq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 17:46:02.917580 ezq-2.0.2/src/ezq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7046 2021-08-24 17:46:02.000000 ezq-2.0.2/src/ezq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-08-24 17:46:02.000000 ezq-2.0.2/src/ezq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-24 17:46:02.000000 ezq-2.0.2/src/ezq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-24 17:46:02.000000 ezq-2.0.2/src/ezq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-08-24 17:46:02.000000 ezq-2.0.2/src/ezq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-24 17:46:02.921580 ezq-2.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3316 2021-08-24 17:45:48.000000 ezq-2.0.2/test/test_ezq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.229999 ezq-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-10 04:13:34.000000 ezq-2.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-10 04:14:00.229999 ezq-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9080 2023-05-10 04:13:34.000000 ezq-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 04:13:34.000000 ezq-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-10 04:14:00.229999 ezq-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-10 04:13:34.000000 ezq-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.225999 ezq-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.229999 ezq-2.0.3/src/ezq/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 04:13:34.000000 ezq-2.0.3/src/ezq/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-10 04:13:34.000000 ezq-2.0.3/src/ezq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.229999 ezq-2.0.3/src/ezq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 04:14:00.000000 ezq-2.0.3/src/ezq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:14:00.229999 ezq-2.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-10 04:13:34.000000 ezq-2.0.3/test/test_ezq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-10 04:13:34.000000 ezq-2.0.3/test/test_iter.py
```

### Comparing `ezq-2.0.2/LICENSE.md` & `ezq-2.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ezq-2.0.2/setup.py` & `ezq-2.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 
 """Install library package."""
 
 # native
 from pathlib import Path
 import site
 import sys
+from typing import Dict
 
 # lib
 from setuptools import setup, find_namespace_packages
 
 # pkg
-pkg = {}
+pkg: Dict[str, str] = {}
 here = Path(__file__).parent.resolve()
-top = here / "src" / "ezq"
-exec((top / "__about__.py").open().read(), pkg)  # pylint: disable=exec-used
+exec(  # pylint: disable=exec-used
+    (here / "src" / "ezq" / "__about__.py").open(encoding="utf-8").read(), pkg
+)
 
 # See: https://github.com/pypa/pip/issues/7953
 site.ENABLE_USER_SITE = "--user" in sys.argv[1:]
 
 # See: https://github.com/pypa/pipenv/issues/1911
 # See: https://caremad.io/posts/2013/07/setup-vs-requirement/
 
 setup(
     python_requires=">=3.8",
     name="ezq",
     version=pkg["__version__"],
     description=pkg["__doc__"].split("\n")[0],
-    long_description=(here / "README.md").read_text(),
+    long_description=(here / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     license=pkg["__license__"],
     author=pkg["__author__"],
     author_email=pkg["__email__"],
     url=pkg["__url__"],
     download_url=pkg["__url__"],
     package_dir={"": "src"},
```

