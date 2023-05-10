# Comparing `tmp/esper-2.4.1.zip` & `tmp/esper-2.5.zip`

## zipinfo {}

```diff
@@ -1,47 +1,46 @@
-Zip file size: 47631 bytes, number of entries: 45
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/esper/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/esper.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/tests/
--rw-r--r--  2.0 unx      835 b- defN 19-Jun-13 20:00 esper-2.4.1/.gitignore
--rw-r--r--  2.0 unx      155 b- defN 22-Mar-15 18:31 esper-2.4.1/.travis.yml
--rw-r--r--  2.0 unx     1076 b- defN 21-Oct-01 18:10 esper-2.4.1/LICENSE.rst
--rw-r--r--  2.0 unx       35 b- defN 18-May-28 22:41 esper-2.4.1/MANIFEST.in
--rw-r--r--  2.0 unx    15376 b- defN 22-Oct-06 17:08 esper-2.4.1/README.md
--rw-r--r--  2.0 unx     3526 b- defN 22-Oct-23 13:33 esper-2.4.1/RELEASE_NOTES
--rwxr-xr-x  2.0 unx     1444 b- defN 22-Oct-06 17:12 esper-2.4.1/make.py
--rw-r--r--  2.0 unx     1221 b- defN 22-Oct-06 17:09 esper-2.4.1/setup.py
--rw-r--r--  2.0 unx    16170 b- defN 22-Oct-23 13:35 esper-2.4.1/PKG-INFO
--rw-r--r--  2.0 unx       38 b- defN 22-Oct-23 13:35 esper-2.4.1/setup.cfg
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/.github/ISSUE_TEMPLATE/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Oct-23 13:35 esper-2.4.1/.github/workflows/
--rw-r--r--  2.0 unx      487 b- defN 22-Oct-01 21:58 esper-2.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--  2.0 unx      472 b- defN 22-Oct-01 21:58 esper-2.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--  2.0 unx      121 b- defN 22-Oct-05 17:42 esper-2.4.1/.github/ISSUE_TEMPLATE/question-or-comment.md
--rw-r--r--  2.0 unx      602 b- defN 22-Oct-23 13:31 esper-2.4.1/.github/workflows/python-package.yml
--rw-r--r--  2.0 unx      634 b- defN 19-Aug-24 20:00 esper-2.4.1/docs/Makefile
--rw-r--r--  2.0 unx     1962 b- defN 22-Mar-15 18:31 esper-2.4.1/docs/conf.py
--rw-r--r--  2.0 unx      775 b- defN 22-Oct-01 23:19 esper-2.4.1/docs/index.rst
--rw-r--r--  2.0 unx      795 b- defN 19-Aug-24 20:00 esper-2.4.1/docs/make.bat
--rw-r--r--  2.0 unx    16342 b- defN 22-Oct-23 13:35 esper-2.4.1/esper/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-01 18:10 esper-2.4.1/esper/py.typed
--rw-r--r--  2.0 unx    16170 b- defN 22-Oct-23 13:35 esper-2.4.1/esper.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      767 b- defN 22-Oct-23 13:35 esper-2.4.1/esper.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Oct-23 13:35 esper-2.4.1/esper.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Oct-23 13:35 esper-2.4.1/esper.egg-info/top_level.txt
--rw-r--r--  2.0 unx     4805 b- defN 21-Jun-28 21:40 esper-2.4.1/examples/benchmark.py
--rw-r--r--  2.0 unx     3589 b- defN 21-Jun-28 21:59 esper-2.4.1/examples/benchmark_cache.py
--rw-r--r--  2.0 unx      215 b- defN 16-Jan-02 20:48 esper-2.4.1/examples/bluesquare.png
--rw-r--r--  2.0 unx     1669 b- defN 21-Jun-28 21:59 esper-2.4.1/examples/headless_example.py
--rw-r--r--  2.0 unx     4890 b- defN 21-Jun-28 21:59 esper-2.4.1/examples/pygame_example.py
--rw-r--r--  2.0 unx     4434 b- defN 22-Oct-23 13:05 esper-2.4.1/examples/pyglet_example.py
--rwxr-xr-x  2.0 unx     8370 b- defN 22-Oct-23 13:05 esper-2.4.1/examples/pyglet_example_batch.py
--rw-r--r--  2.0 unx     5874 b- defN 16-Jan-09 12:16 esper-2.4.1/examples/pysdl2_example.py
--rw-r--r--  2.0 unx     2042 b- defN 16-Apr-19 21:26 esper-2.4.1/examples/pythonista_ios_example.py
--rw-r--r--  2.0 unx      218 b- defN 16-Jan-02 20:48 esper-2.4.1/examples/redsquare.png
--rw-r--r--  2.0 unx        0 b- defN 16-Feb-15 21:16 esper-2.4.1/tests/__init__.py
--rw-r--r--  2.0 unx    13052 b- defN 22-Jun-10 11:15 esper-2.4.1/tests/test_world.py
-45 files, 128168 bytes uncompressed, 41427 bytes compressed:  67.7%
+Zip file size: 47896 bytes, number of entries: 44
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/esper/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/esper.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/tests/
+-rw-r--r--  2.0 unx      835 b- defN 19-Jun-13 20:00 esper-2.5/.gitignore
+-rw-r--r--  2.0 unx     1081 b- defN 22-Dec-20 15:53 esper-2.5/LICENSE.rst
+-rw-r--r--  2.0 unx       35 b- defN 18-May-28 22:41 esper-2.5/MANIFEST.in
+-rw-r--r--  2.0 unx    15487 b- defN 22-Dec-20 16:10 esper-2.5/README.md
+-rw-r--r--  2.0 unx     3800 b- defN 23-May-10 17:48 esper-2.5/RELEASE_NOTES
+-rwxr-xr-x  2.0 unx     1444 b- defN 22-Oct-06 17:12 esper-2.5/make.py
+-rw-r--r--  2.0 unx     1221 b- defN 22-Oct-06 17:09 esper-2.5/setup.py
+-rw-r--r--  2.0 unx    16279 b- defN 23-May-10 18:02 esper-2.5/PKG-INFO
+-rw-r--r--  2.0 unx       38 b- defN 23-May-10 18:02 esper-2.5/setup.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/.github/ISSUE_TEMPLATE/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-10 18:02 esper-2.5/.github/workflows/
+-rw-r--r--  2.0 unx      487 b- defN 22-Oct-01 21:58 esper-2.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--  2.0 unx      472 b- defN 22-Oct-01 21:58 esper-2.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--  2.0 unx      121 b- defN 22-Oct-05 17:42 esper-2.5/.github/ISSUE_TEMPLATE/question-or-comment.md
+-rw-r--r--  2.0 unx      693 b- defN 23-May-09 17:11 esper-2.5/.github/workflows/unit-tests.yml
+-rw-r--r--  2.0 unx      634 b- defN 19-Aug-24 20:00 esper-2.5/docs/Makefile
+-rw-r--r--  2.0 unx     1962 b- defN 22-Mar-15 18:31 esper-2.5/docs/conf.py
+-rw-r--r--  2.0 unx      775 b- defN 22-Oct-01 23:19 esper-2.5/docs/index.rst
+-rw-r--r--  2.0 unx      795 b- defN 19-Aug-24 20:00 esper-2.5/docs/make.bat
+-rw-r--r--  2.0 unx    16776 b- defN 23-May-10 17:48 esper-2.5/esper/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 21-Oct-01 18:10 esper-2.5/esper/py.typed
+-rw-r--r--  2.0 unx    16279 b- defN 23-May-10 18:02 esper-2.5/esper.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      751 b- defN 23-May-10 18:02 esper-2.5/esper.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-10 18:02 esper-2.5/esper.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-10 18:02 esper-2.5/esper.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     4805 b- defN 21-Jun-28 21:40 esper-2.5/examples/benchmark.py
+-rw-r--r--  2.0 unx     3589 b- defN 21-Jun-28 21:59 esper-2.5/examples/benchmark_cache.py
+-rw-r--r--  2.0 unx      215 b- defN 16-Jan-02 20:48 esper-2.5/examples/bluesquare.png
+-rw-r--r--  2.0 unx     1669 b- defN 21-Jun-28 21:59 esper-2.5/examples/headless_example.py
+-rw-r--r--  2.0 unx     4890 b- defN 21-Jun-28 21:59 esper-2.5/examples/pygame_example.py
+-rw-r--r--  2.0 unx     4434 b- defN 22-Oct-23 13:05 esper-2.5/examples/pyglet_example.py
+-rwxr-xr-x  2.0 unx     8370 b- defN 22-Oct-23 13:05 esper-2.5/examples/pyglet_example_batch.py
+-rw-r--r--  2.0 unx     5874 b- defN 16-Jan-09 12:16 esper-2.5/examples/pysdl2_example.py
+-rw-r--r--  2.0 unx     2042 b- defN 16-Apr-19 21:26 esper-2.5/examples/pythonista_ios_example.py
+-rw-r--r--  2.0 unx      218 b- defN 16-Jan-02 20:48 esper-2.5/examples/redsquare.png
+-rw-r--r--  2.0 unx        0 b- defN 16-Feb-15 21:16 esper-2.5/tests/__init__.py
+-rw-r--r--  2.0 unx    15224 b- defN 23-May-10 17:54 esper-2.5/tests/test_world.py
+44 files, 131302 bytes uncompressed, 41998 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -1,136 +1,133 @@
-Filename: esper-2.4.1/
+Filename: esper-2.5/
 Comment: 
 
-Filename: esper-2.4.1/.github/
+Filename: esper-2.5/.github/
 Comment: 
 
-Filename: esper-2.4.1/docs/
+Filename: esper-2.5/docs/
 Comment: 
 
-Filename: esper-2.4.1/esper/
+Filename: esper-2.5/esper/
 Comment: 
 
-Filename: esper-2.4.1/esper.egg-info/
+Filename: esper-2.5/esper.egg-info/
 Comment: 
 
-Filename: esper-2.4.1/examples/
+Filename: esper-2.5/examples/
 Comment: 
 
-Filename: esper-2.4.1/tests/
+Filename: esper-2.5/tests/
 Comment: 
 
-Filename: esper-2.4.1/.gitignore
+Filename: esper-2.5/.gitignore
 Comment: 
 
-Filename: esper-2.4.1/.travis.yml
+Filename: esper-2.5/LICENSE.rst
 Comment: 
 
-Filename: esper-2.4.1/LICENSE.rst
+Filename: esper-2.5/MANIFEST.in
 Comment: 
 
-Filename: esper-2.4.1/MANIFEST.in
+Filename: esper-2.5/README.md
 Comment: 
 
-Filename: esper-2.4.1/README.md
+Filename: esper-2.5/RELEASE_NOTES
 Comment: 
 
-Filename: esper-2.4.1/RELEASE_NOTES
+Filename: esper-2.5/make.py
 Comment: 
 
-Filename: esper-2.4.1/make.py
+Filename: esper-2.5/setup.py
 Comment: 
 
-Filename: esper-2.4.1/setup.py
+Filename: esper-2.5/PKG-INFO
 Comment: 
 
-Filename: esper-2.4.1/PKG-INFO
+Filename: esper-2.5/setup.cfg
 Comment: 
 
-Filename: esper-2.4.1/setup.cfg
+Filename: esper-2.5/.github/ISSUE_TEMPLATE/
 Comment: 
 
-Filename: esper-2.4.1/.github/ISSUE_TEMPLATE/
+Filename: esper-2.5/.github/workflows/
 Comment: 
 
-Filename: esper-2.4.1/.github/workflows/
+Filename: esper-2.5/.github/ISSUE_TEMPLATE/bug_report.md
 Comment: 
 
-Filename: esper-2.4.1/.github/ISSUE_TEMPLATE/bug_report.md
+Filename: esper-2.5/.github/ISSUE_TEMPLATE/feature_request.md
 Comment: 
 
-Filename: esper-2.4.1/.github/ISSUE_TEMPLATE/feature_request.md
+Filename: esper-2.5/.github/ISSUE_TEMPLATE/question-or-comment.md
 Comment: 
 
-Filename: esper-2.4.1/.github/ISSUE_TEMPLATE/question-or-comment.md
+Filename: esper-2.5/.github/workflows/unit-tests.yml
 Comment: 
 
-Filename: esper-2.4.1/.github/workflows/python-package.yml
+Filename: esper-2.5/docs/Makefile
 Comment: 
 
-Filename: esper-2.4.1/docs/Makefile
+Filename: esper-2.5/docs/conf.py
 Comment: 
 
-Filename: esper-2.4.1/docs/conf.py
+Filename: esper-2.5/docs/index.rst
 Comment: 
 
-Filename: esper-2.4.1/docs/index.rst
+Filename: esper-2.5/docs/make.bat
 Comment: 
 
-Filename: esper-2.4.1/docs/make.bat
+Filename: esper-2.5/esper/__init__.py
 Comment: 
 
-Filename: esper-2.4.1/esper/__init__.py
+Filename: esper-2.5/esper/py.typed
 Comment: 
 
-Filename: esper-2.4.1/esper/py.typed
+Filename: esper-2.5/esper.egg-info/PKG-INFO
 Comment: 
 
-Filename: esper-2.4.1/esper.egg-info/PKG-INFO
+Filename: esper-2.5/esper.egg-info/SOURCES.txt
 Comment: 
 
-Filename: esper-2.4.1/esper.egg-info/SOURCES.txt
+Filename: esper-2.5/esper.egg-info/dependency_links.txt
 Comment: 
 
-Filename: esper-2.4.1/esper.egg-info/dependency_links.txt
+Filename: esper-2.5/esper.egg-info/top_level.txt
 Comment: 
 
-Filename: esper-2.4.1/esper.egg-info/top_level.txt
+Filename: esper-2.5/examples/benchmark.py
 Comment: 
 
-Filename: esper-2.4.1/examples/benchmark.py
+Filename: esper-2.5/examples/benchmark_cache.py
 Comment: 
 
-Filename: esper-2.4.1/examples/benchmark_cache.py
+Filename: esper-2.5/examples/bluesquare.png
 Comment: 
 
-Filename: esper-2.4.1/examples/bluesquare.png
+Filename: esper-2.5/examples/headless_example.py
 Comment: 
 
-Filename: esper-2.4.1/examples/headless_example.py
+Filename: esper-2.5/examples/pygame_example.py
 Comment: 
 
-Filename: esper-2.4.1/examples/pygame_example.py
+Filename: esper-2.5/examples/pyglet_example.py
 Comment: 
 
-Filename: esper-2.4.1/examples/pyglet_example.py
+Filename: esper-2.5/examples/pyglet_example_batch.py
 Comment: 
 
-Filename: esper-2.4.1/examples/pyglet_example_batch.py
+Filename: esper-2.5/examples/pysdl2_example.py
 Comment: 
 
-Filename: esper-2.4.1/examples/pysdl2_example.py
+Filename: esper-2.5/examples/pythonista_ios_example.py
 Comment: 
 
-Filename: esper-2.4.1/examples/pythonista_ios_example.py
+Filename: esper-2.5/examples/redsquare.png
 Comment: 
 
-Filename: esper-2.4.1/examples/redsquare.png
+Filename: esper-2.5/tests/__init__.py
 Comment: 
 
-Filename: esper-2.4.1/tests/__init__.py
-Comment: 
-
-Filename: esper-2.4.1/tests/test_world.py
+Filename: esper-2.5/tests/test_world.py
 Comment: 
 
 Zip file comment:
```

## Comparing `esper-2.4.1/.gitignore` & `esper-2.5/.gitignore`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/LICENSE.rst` & `esper-2.5/LICENSE.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License
 
-Copyright (c) 2020 Benjamin Moran
+Copyright (c) 2015-2023 Benjamin Moran
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `esper-2.4.1/README.md` & `esper-2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-[![CI Status](https://readthedocs.org/projects/esper/badge/?version=latest)](https://travis-ci.org/benmoran56/esper)
-[![Documentation Status](https://readthedocs.org/projects/esper/badge/?version=latest)](https://esper.readthedocs.io/?badge=latest)
+[![pypi](https://badge.fury.io/py/esper.svg)](https://pypi.python.org/pypi/esper)
+[![rtd](https://readthedocs.org/projects/esper/badge/?version=latest)](https://esper.readthedocs.io)
+[![PyTest](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml)
 
 Esper is a lightweight Entity System module for Python, with a focus on performance
 ===================================================================================
 
 Esper is an MIT licensed Entity System, or, Entity Component System (ECS).
 The design is based on the Entity System concepts outlined by Adam Martin in his blog at
 http://t-machine.org/, and others. The primary focus is on keeping it as lightweight and
@@ -367,8 +368,10 @@
 Contributions to Esper are always welcome, but there are some specific project goals to keep in mind:
 
 - Pure Python code only - no binary extensions, Cython, etc.
 - Try to target all currently supported Python versions. Exceptions can be made if there is a compelling reason.
 - Avoid bloat as much as possible. New features will be considered if they are commonly useful. Generally speaking, we don't want to add functionality that is better handled in another module or library. 
 - Performance is preferrable to readability.
 
-If you have any questions before contributing, feel free to `open an issue <https://github.com/benmoran56/esper/issues>`_.
+If you have any questions before contributing, feel free to [open an issue].
+
+[open an issue]: https://github.com/benmoran56/esper/issues
```

## Comparing `esper-2.4.1/RELEASE_NOTES` & `esper-2.5/RELEASE_NOTES`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+esper 2.5
+=========
+Maintenance release
+
+Changes
+-------
+- Removing all Components from an Entity will no longer automatically delete the Entity.
+- Typing fixes and additions.
+- Entity DB check and creation is done once when Entity is created, not when adding Components.
+
+
 esper 2.4
 =========
 Maintenance release
 
 Changes
 -------
 - Minor typing changes, and docstring improvement.
```

## Comparing `esper-2.4.1/make.py` & `esper-2.5/make.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/setup.py` & `esper-2.5/setup.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/PKG-INFO` & `esper-2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esper
-Version: 2.4.1
+Version: 2.5
 Summary: esper is a lightweight Entity System (ECS) for Python, with a focus on performance.
 Home-page: https://github.com/benmoran56/esper
 Download-URL: https://github.com/benmoran56/esper/releases
 Author: Benjamin Moran
 Author-email: benmoran@protonmail.com
 License: MIT
 Keywords: ecs,entity component system,game
@@ -16,16 +16,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE.rst
 
-[![CI Status](https://readthedocs.org/projects/esper/badge/?version=latest)](https://travis-ci.org/benmoran56/esper)
-[![Documentation Status](https://readthedocs.org/projects/esper/badge/?version=latest)](https://esper.readthedocs.io/?badge=latest)
+[![pypi](https://badge.fury.io/py/esper.svg)](https://pypi.python.org/pypi/esper)
+[![rtd](https://readthedocs.org/projects/esper/badge/?version=latest)](https://esper.readthedocs.io)
+[![PyTest](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml)
 
 Esper is a lightweight Entity System module for Python, with a focus on performance
 ===================================================================================
 
 Esper is an MIT licensed Entity System, or, Entity Component System (ECS).
 The design is based on the Entity System concepts outlined by Adam Martin in his blog at
 http://t-machine.org/, and others. The primary focus is on keeping it as lightweight and
@@ -389,8 +390,10 @@
 Contributions to Esper are always welcome, but there are some specific project goals to keep in mind:
 
 - Pure Python code only - no binary extensions, Cython, etc.
 - Try to target all currently supported Python versions. Exceptions can be made if there is a compelling reason.
 - Avoid bloat as much as possible. New features will be considered if they are commonly useful. Generally speaking, we don't want to add functionality that is better handled in another module or library. 
 - Performance is preferrable to readability.
 
-If you have any questions before contributing, feel free to `open an issue <https://github.com/benmoran56/esper/issues>`_.
+If you have any questions before contributing, feel free to [open an issue].
+
+[open an issue]: https://github.com/benmoran56/esper/issues
```

## Comparing `esper-2.4.1/docs/Makefile` & `esper-2.5/docs/Makefile`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/docs/conf.py` & `esper-2.5/docs/conf.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/docs/index.rst` & `esper-2.5/docs/index.rst`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/docs/make.bat` & `esper-2.5/docs/make.bat`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/esper/__init__.py` & `esper-2.5/esper/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import time as _time
 
 from types import MethodType as _MethodType
 
-from typing import Iterable as _Iterable
+from typing import Any as _Any
 from typing import List as _List
-from typing import Optional as _Optional
-from typing import Tuple as _Tuple
 from typing import Type as _Type
+from typing import Tuple as _Tuple
 from typing import TypeVar as _TypeVar
+from typing import Iterable as _Iterable
+from typing import Optional as _Optional
+from typing import overload as _overload
 
 from weakref import ref as _ref
 from weakref import WeakMethod as _WeakMethod
 
 
-version = '2.4.1'
+version = '2.5'
 
 
 ###################
 #  Event system
 ###################
 
 event_registry: dict = {}
@@ -82,14 +84,17 @@
 
 ###################
 #   ECS Classes
 ###################
 
 
 _C = _TypeVar('_C')
+_C2 = _TypeVar('_C2')
+_C3 = _TypeVar('_C3')
+_C4 = _TypeVar('_C4')
 
 
 class Processor:
     """Base class for all Processors to inherit from.
 
     Processor instances must contain a `process` method, but you are otherwise
     free to define the class any way you wish. Processors should be instantiated,
@@ -206,26 +211,26 @@
         assigned to the Entity on creation. Components can be also be
         added later with the :py:meth:`esper.World.add_component` method.
         """
         self._next_entity_id += 1
 
         entity = self._next_entity_id
 
+        if entity not in self._entities:
+            self._entities[entity] = {}
+
         for component_instance in components:
 
             component_type = type(component_instance)
 
             if component_type not in self._components:
                 self._components[component_type] = set()
 
             self._components[component_type].add(entity)
 
-            if entity not in self._entities:
-                self._entities[entity] = {}
-
             self._entities[entity][component_type] = component_instance
             self.clear_cache()
 
         return entity
 
     def delete_entity(self, entity: int, immediate: bool = False) -> None:
         """Delete an Entity from the World.
@@ -305,42 +310,34 @@
         component_type = type_alias or type(component_instance)
 
         if component_type not in self._components:
             self._components[component_type] = set()
 
         self._components[component_type].add(entity)
 
-        if entity not in self._entities:
-            self._entities[entity] = {}
-
         self._entities[entity][component_type] = component_instance
         self.clear_cache()
 
-    def remove_component(self, entity: int, component_type: _Type[_C]) -> int:
+    def remove_component(self, entity: int, component_type: _Type[_C]) -> _C:
         """Remove a Component instance from an Entity, by type.
 
-        A Component instance can be removed by providing its type.
+        A Component instance can only be removed by providing its type.
         For example: world.delete_component(enemy_a, Velocity) will remove
         the Velocity instance from the Entity enemy_a.
 
         Raises a KeyError if either the given entity or Component type does
         not exist in the database.
         """
         self._components[component_type].discard(entity)
 
         if not self._components[component_type]:
             del self._components[component_type]
 
-        del self._entities[entity][component_type]
-
-        if not self._entities[entity]:
-            del self._entities[entity]
-
         self.clear_cache()
-        return entity
+        return self._entities[entity].pop(component_type)
 
     def _get_component(self, component_type: _Type[_C]) -> _Iterable[_Tuple[int, _C]]:
         entity_db = self._entities
 
         for entity in self._components.get(component_type, []):
             yield entity, entity_db[entity][component_type]
 
@@ -359,15 +356,27 @@
         try:
             return self._get_component_cache[component_type]
         except KeyError:
             return self._get_component_cache.setdefault(
                 component_type, list(self._get_component(component_type))
             )
 
-    def get_components(self, *component_types: _Type[_C]) -> _List[_Tuple[int, _List[_C]]]:
+    @_overload
+    def get_components(self, __c1: _Type[_C], __c2: _Type[_C2]) -> _List[_Tuple[int, _Tuple[_C, _C2]]]:
+        ...
+
+    @_overload
+    def get_components(self, __c1: _Type[_C], __c2: _Type[_C2], __c3: _Type[_C3]) -> _List[_Tuple[int, _Tuple[_C, _C2, _C3]]]:
+        ...
+
+    @_overload
+    def get_components(self, __c1: _Type[_C], __c2: _Type[_C2], __c3: _Type[_C3], __c4: _Type[_C4]) -> _List[_Tuple[int, _Tuple[_C, _C2, _C3, _C4]]]:
+        ...
+
+    def get_components(self, *component_types: _Type[_Any]) -> _Iterable[_Tuple[int, _Tuple[_Any, ...]]]:
         """Get an iterator for Entity and multiple Component sets."""
         try:
             return self._get_components_cache[component_types]
         except KeyError:
             return self._get_components_cache.setdefault(
                 component_types, list(self._get_components(*component_types))
             )
```

## Comparing `esper-2.4.1/esper.egg-info/PKG-INFO` & `esper-2.5/esper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esper
-Version: 2.4.1
+Version: 2.5
 Summary: esper is a lightweight Entity System (ECS) for Python, with a focus on performance.
 Home-page: https://github.com/benmoran56/esper
 Download-URL: https://github.com/benmoran56/esper/releases
 Author: Benjamin Moran
 Author-email: benmoran@protonmail.com
 License: MIT
 Keywords: ecs,entity component system,game
@@ -16,16 +16,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE.rst
 
-[![CI Status](https://readthedocs.org/projects/esper/badge/?version=latest)](https://travis-ci.org/benmoran56/esper)
-[![Documentation Status](https://readthedocs.org/projects/esper/badge/?version=latest)](https://esper.readthedocs.io/?badge=latest)
+[![pypi](https://badge.fury.io/py/esper.svg)](https://pypi.python.org/pypi/esper)
+[![rtd](https://readthedocs.org/projects/esper/badge/?version=latest)](https://esper.readthedocs.io)
+[![PyTest](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml)
 
 Esper is a lightweight Entity System module for Python, with a focus on performance
 ===================================================================================
 
 Esper is an MIT licensed Entity System, or, Entity Component System (ECS).
 The design is based on the Entity System concepts outlined by Adam Martin in his blog at
 http://t-machine.org/, and others. The primary focus is on keeping it as lightweight and
@@ -389,8 +390,10 @@
 Contributions to Esper are always welcome, but there are some specific project goals to keep in mind:
 
 - Pure Python code only - no binary extensions, Cython, etc.
 - Try to target all currently supported Python versions. Exceptions can be made if there is a compelling reason.
 - Avoid bloat as much as possible. New features will be considered if they are commonly useful. Generally speaking, we don't want to add functionality that is better handled in another module or library. 
 - Performance is preferrable to readability.
 
-If you have any questions before contributing, feel free to `open an issue <https://github.com/benmoran56/esper/issues>`_.
+If you have any questions before contributing, feel free to [open an issue].
+
+[open an issue]: https://github.com/benmoran56/esper/issues
```

## Comparing `esper-2.4.1/esper.egg-info/SOURCES.txt` & `esper-2.5/esper.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 .gitignore
-.travis.yml
 LICENSE.rst
 MANIFEST.in
 README.md
 RELEASE_NOTES
 make.py
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question-or-comment.md
-.github/workflows/python-package.yml
+.github/workflows/unit-tests.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 esper/__init__.py
 esper/py.typed
 esper.egg-info/PKG-INFO
```

## Comparing `esper-2.4.1/examples/benchmark.py` & `esper-2.5/examples/benchmark.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/examples/benchmark_cache.py` & `esper-2.5/examples/benchmark_cache.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/examples/headless_example.py` & `esper-2.5/examples/headless_example.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/examples/pygame_example.py` & `esper-2.5/examples/pygame_example.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/examples/pyglet_example.py` & `esper-2.5/examples/pyglet_example.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/examples/pyglet_example_batch.py` & `esper-2.5/examples/pyglet_example_batch.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/examples/pysdl2_example.py` & `esper-2.5/examples/pysdl2_example.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/examples/pythonista_ios_example.py` & `esper-2.5/examples/pythonista_ios_example.py`

 * *Files identical despite different names*

## Comparing `esper-2.4.1/tests/test_world.py` & `esper-2.5/tests/test_world.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,19 @@
     entity2 = world.create_entity(ComponentB())
     assert world.has_component(entity1, ComponentA) is True
     assert world.has_component(entity1, ComponentB) is False
     assert world.has_component(entity2, ComponentA) is False
     assert world.has_component(entity2, ComponentB) is True
 
 
+def test_adding_component_to_not_existing_entity_raises_error(world):
+    with pytest.raises(KeyError):
+        world.add_component(123, ComponentA())
+
+
 def test_create_entity_and_add_components(world):
     entity1 = world.create_entity()
     world.add_component(entity1, ComponentA())
     world.add_component(entity1, ComponentB())
     assert world.has_component(entity1, ComponentA) is True
     assert world.has_component(entity1, ComponentC) is False
 
@@ -55,26 +60,25 @@
 
 
 def test_delete_entity(world):
     entity1 = world.create_entity()
     world.add_component(entity1, ComponentC())
     entity2 = world.create_entity()
     world.add_component(entity2, ComponentD())
-    entity3 = world.create_entity()
-    world.add_component(entity3, ComponentE())
-    entity4 = world.create_entity()
+    entity_with_component = world.create_entity()
+    world.add_component(entity_with_component, ComponentE())
+    empty_entity = world.create_entity()
 
-    assert entity3 == 3
-    world.delete_entity(entity3, immediate=True)
+    assert entity_with_component == 3
+    world.delete_entity(entity_with_component, immediate=True)
     with pytest.raises(KeyError):
-        world.components_for_entity(entity3)
+        world.components_for_entity(entity_with_component)
     with pytest.raises(KeyError):
         world.delete_entity(999, immediate=True)
-    with pytest.raises(KeyError):
-        world.delete_entity(entity4, immediate=True)
+    world.delete_entity(empty_entity, immediate=True)
 
 
 def test_component_for_entity(world):
     entity = world.create_entity()
     world.add_component(entity, ComponentC())
     assert isinstance(world.component_for_entity(entity, ComponentC), ComponentC)
     with pytest.raises(KeyError):
@@ -252,25 +256,79 @@
     entity2 = world.create_entity(ComponentB(), ComponentC(), ComponentD())
     assert len(list(query for query in world.get_components(ComponentB, ComponentC))) == 2
 
     world.delete_entity(entity2, immediate=True)
     assert len(list(query for query in world.get_components(ComponentB, ComponentC))) == 1
 
 
-def test_entity_exists(world):
-    dead_entity = world.create_entity(ComponentB())
-    world.delete_entity(dead_entity)
-    empty_entity = world.create_entity()
-    existent_entity = world.create_entity(ComponentA())
-    future_entity = existent_entity + 1
+class TestEntityExists:
+    def test_dead_entity(self, world):
+        dead_entity = world.create_entity(ComponentB())
+        world.delete_entity(dead_entity)
+        assert not world.entity_exists(dead_entity)
+
+    def test_not_created_entity(self, world):
+        assert not world.entity_exists(123)
+
+    def test_empty_entity(self, world):
+        empty_entity = world.create_entity()
+        assert world.entity_exists(empty_entity)
+
+    def test_entity_with_component(self, world):
+        entity_with_component = world.create_entity(ComponentA())
+        assert world.entity_exists(entity_with_component)
+
+
+class TestRemoveComponent:
+    def test_remove_from_not_existing_entity_raises_key_error(self, world):
+        with pytest.raises(KeyError):
+            world.remove_component(123, ComponentA)
+
+    def test_remove_not_existing_component_raises_key_error(self, world):
+        entity = world.create_entity(ComponentB())
+
+        with pytest.raises(KeyError):
+            world.remove_component(entity, ComponentA)
 
-    assert world.entity_exists(existent_entity)
-    assert not world.entity_exists(dead_entity)
-    assert not world.entity_exists(empty_entity)
-    assert not world.entity_exists(future_entity)
+    def test_remove_component_with_object_raises_key_error(self, populated_world):
+        entity = 2
+        component = ComponentD()
+
+        assert populated_world.has_component(entity, type(component))
+        with pytest.raises(KeyError):
+            populated_world.remove_component(entity, component)
+
+    def test_remove_component_returns_removed_instance(self, world):
+        component = ComponentA()
+        entity = world.create_entity(component)
+
+        result = world.remove_component(entity, type(component))
+
+        assert result is component
+
+    def test_remove_last_component_leaves_empty_entity(self, world):
+        entity = world.create_entity()
+        world.add_component(entity, ComponentA())
+
+        world.remove_component(entity, ComponentA)
+
+        assert not world.has_component(entity, ComponentA)
+        assert world.entity_exists(entity)
+
+    def test_removing_one_component_leaves_other_intact(self, world):
+        component_a = ComponentA()
+        component_b = ComponentB()
+        component_c = ComponentC()
+        entity = world.create_entity(component_a, component_b, component_c)
+
+        world.remove_component(entity, ComponentB)
+
+        assert world.component_for_entity(entity, ComponentA) is component_a
+        assert not world.has_component(entity, ComponentB)
+        assert world.component_for_entity(entity, ComponentC) is component_c
 
 
 def test_event_dispatch_no_handlers():
     esper.dispatch_event("foo")
     esper.dispatch_event("foo", 1)
     esper.dispatch_event("foo", 1, 2)
     esper.event_registry.clear()
@@ -297,29 +355,31 @@
 def test_set_methoad_as_handler_in_init():
 
     class MyClass(esper.Processor):
 
         def __init__(self):
             esper.set_handler("foo", self._my_handler)
 
-        def _my_handler(self):
+        @staticmethod
+        def _my_handler():
             print("OK")
 
         def process(self, dt):
             pass
 
-    myclass = MyClass()
+    _myclass = MyClass()
     esper.dispatch_event("foo")
     esper.event_registry.clear()
 
 
 def test_set_instance_methoad_as_handler():
     class MyClass(esper.Processor):
 
-        def my_handler(self):
+        @staticmethod
+        def my_handler():
             print("OK")
 
         def process(self, dt):
             pass
 
     myclass = MyClass()
     esper.set_handler("foo", myclass.my_handler)
@@ -373,16 +433,15 @@
 class ComponentE:
     def __init__(self):
         self.items = {"itema": None, "itemb": 1000}
         self.points = [a + 2 for a in list(range(44))]
 
 
 class ComponentF:
-    def __init__(self):
-        pass
+    pass
 
 
 class CorrectProcessorA(esper.Processor):
 
     def process(self):
         pass
```

