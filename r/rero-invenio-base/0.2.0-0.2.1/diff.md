# Comparing `tmp/rero_invenio_base-0.2.0.tar.gz` & `tmp/rero_invenio_base-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rero_invenio_base-0.2.0.tar", max compression
+gzip compressed data, was "rero_invenio_base-0.2.1.tar", max compression
```

## Comparing `rero_invenio_base-0.2.0.tar` & `rero_invenio_base-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1062 2022-09-02 07:16:03.900445 rero_invenio_base-0.2.0/LICENSE
--rw-r--r--   0        0        0     1462 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/README.rst
--rw-r--r--   0        0        0     1365 2023-01-31 15:38:38.473736 rero_invenio_base-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      854 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/__init__.py
--rw-r--r--   0        0        0      965 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/__init__.py
--rw-r--r--   0        0        0     1031 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/es/__init__.py
--rw-r--r--   0        0        0     2184 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/es/alias.py
--rw-r--r--   0        0        0     5900 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/es/index.py
--rw-r--r--   0        0        0      792 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/es/slm/__init__.py
--rw-r--r--   0        0        0     5164 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/es/slm/cli.py
--rw-r--r--   0        0        0      768 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/es/snapshot/__init__.py
--rw-r--r--   0        0        0     4543 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/es/snapshot/cli.py
--rw-r--r--   0        0        0     2729 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/es/snapshot/repository.py
--rw-r--r--   0        0        0      850 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/shared.py
--rw-r--r--   0        0        0    10089 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/cli/utils.py
--rw-r--r--   0        0        0      741 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/config.py
--rw-r--r--   0        0        0     1576 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/ext.py
--rw-r--r--   0        0        0      756 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/modules/__init__.py
--rw-r--r--   0        0        0      862 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/modules/export/__init__.py
--rw-r--r--   0        0        0     2353 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/modules/export/config.py
--rw-r--r--   0        0        0     1397 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/modules/export/ext.py
--rw-r--r--   0        0        0      975 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/modules/export/proxies.py
--rw-r--r--   0        0        0     5413 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/modules/export/views.py
--rw-r--r--   0        0        0     2521 2023-01-31 15:38:38.473736 rero_invenio_base-0.2.0/rero_invenio_base/modules/tasks.py
--rw-r--r--   0        0        0     1138 2023-01-31 15:38:38.473736 rero_invenio_base-0.2.0/rero_invenio_base/modules/utils.py
--rw-r--r--   0        0        0      893 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.0/rero_invenio_base/version.py
--rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 rero_invenio_base-0.2.0/setup.py
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 rero_invenio_base-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-09-02 07:16:03.900445 rero_invenio_base-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1462 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/README.rst
+-rw-r--r--   0        0        0     1502 2023-05-10 08:51:39.093434 rero_invenio_base-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      854 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/__init__.py
+-rw-r--r--   0        0        0      965 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/__init__.py
+-rw-r--r--   0        0        0     1075 2023-05-10 08:51:39.093434 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/__init__.py
+-rw-r--r--   0        0        0     2184 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/alias.py
+-rw-r--r--   0        0        0    10712 2023-05-10 08:51:39.093434 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/index.py
+-rw-r--r--   0        0        0      792 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/slm/__init__.py
+-rw-r--r--   0        0        0     5164 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/slm/cli.py
+-rw-r--r--   0        0        0      768 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/snapshot/__init__.py
+-rw-r--r--   0        0        0     4543 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/snapshot/cli.py
+-rw-r--r--   0        0        0     2729 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/snapshot/repository.py
+-rw-r--r--   0        0        0     3888 2023-05-10 08:51:39.093434 rero_invenio_base-0.2.1/rero_invenio_base/cli/es/task.py
+-rw-r--r--   0        0        0      850 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/shared.py
+-rw-r--r--   0        0        0    10089 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/cli/utils.py
+-rw-r--r--   0        0        0      741 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/config.py
+-rw-r--r--   0        0        0     1576 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/ext.py
+-rw-r--r--   0        0        0      756 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/modules/__init__.py
+-rw-r--r--   0        0        0      862 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/modules/export/__init__.py
+-rw-r--r--   0        0        0     2353 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/modules/export/config.py
+-rw-r--r--   0        0        0     1397 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/modules/export/ext.py
+-rw-r--r--   0        0        0      975 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/modules/export/proxies.py
+-rw-r--r--   0        0        0     5413 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/modules/export/views.py
+-rw-r--r--   0        0        0     2521 2023-01-31 15:38:38.473736 rero_invenio_base-0.2.1/rero_invenio_base/modules/tasks.py
+-rw-r--r--   0        0        0     1138 2023-01-31 15:38:38.473736 rero_invenio_base-0.2.1/rero_invenio_base/modules/utils.py
+-rw-r--r--   0        0        0      893 2022-09-02 07:39:15.910445 rero_invenio_base-0.2.1/rero_invenio_base/version.py
+-rw-r--r--   0        0        0     3319 1970-01-01 00:00:00.000000 rero_invenio_base-0.2.1/setup.py
+-rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 rero_invenio_base-0.2.1/PKG-INFO
```

### Comparing `rero_invenio_base-0.2.0/LICENSE` & `rero_invenio_base-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/README.rst` & `rero_invenio_base-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/pyproject.toml` & `rero_invenio_base-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [tool.poetry]
 name = "rero-invenio-base"
-version = "0.2.0"
+version = "0.2.1"
 description = "Generic backend libraries for RERO Invenio instances."
 readme = "README.rst"
 authors = ["RERO <software@rero.ch>"]
 license = "GNU Affero General Public License v3.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.10"
-PyYAML = "^6.0"
-invenio-search = {version = "^1.4.2", extras = ["elasticsearch7"]}
-jsonpatch = "^1.32"
-invenio-db = "^1.0.14"
-invenio-records-rest = "*"
+PyYAML = "<=7.0"
+jsonpatch = "<=2.0"
 Mako = ">=1.2.2"
 dparse = ">=0.5.2"
-invenio-indexer = "<2.0.0"
-pydocstyle = "<6.2.0"
+invenio-search = {version = ">=1.4.2,<3.0.0", extras = ["elasticsearch7"]}
+invenio-db = {version = ">=1.0.14,<1.1.0", extras = ["postgresql"]}
+invenio-indexer = "<2.2.0"
+invenio-records-rest = "<2.3.0"
+pydocstyle = ">=6.1.1, <6.2.0"
+docker-services-cli = "^0.6.1"
 
 [tool.poetry.dev-dependencies]
-safety = "^1.10.3"
-pytest-invenio = "^1.4.11"
-ipython = "^8.3.0"
-autoflake = "^1.4"
-Sphinx = "^4.5.0"
+safety = ">=1.8"
+ipython = "*"
+autoflake = ">=1.3.1"
+Sphinx = ">=4.5.0"
+pytest-invenio = ">=1.4.11, <3.0.0"
+docker-services-cli = "<=1.0.0"
 
 [tool.poetry.scripts]
 check_license = "rero_invenio_base.cli.utils:check_license"
 check_json = "rero_invenio_base.cli.utils:check_json"
 rero = "rero_invenio_base.cli:rero"
 
 [build-system]
```

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/__init__.py` & `rero_invenio_base-0.2.1/rero_invenio_base/__init__.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/__init__.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/es/__init__.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/es/snapshot/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,28 +11,12 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""Click elasticsearch command-line utilities."""
+"""Click command-line utilities."""
 
-import click
+from .cli import snapshot
 
-from .alias import alias
-from .index import index
-from .slm import slm
-from .snapshot import snapshot
-
-
-@click.group()
-def es():
-    """Elasticsarch management commands."""
-
-
-es.add_command(index)
-es.add_command(alias)
-es.add_command(slm)
-es.add_command(snapshot)
-
-__all__ = ('index')
+__all__ = ('snapshot')
```

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/es/alias.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/es/alias.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/es/slm/__init__.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/es/slm/__init__.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/es/slm/cli.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/es/slm/cli.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/es/snapshot/__init__.py` & `rero_invenio_base-0.2.1/rero_invenio_base/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,12 +11,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""Click command-line utilities."""
-
-from .cli import snapshot
-
-__all__ = ('snapshot')
+"""Generic backend libraries for RERO Invenio instances."""
```

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/es/snapshot/cli.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/es/snapshot/cli.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/es/snapshot/repository.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/es/snapshot/repository.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/shared.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/shared.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/cli/utils.py` & `rero_invenio_base-0.2.1/rero_invenio_base/cli/utils.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/config.py` & `rero_invenio_base-0.2.1/rero_invenio_base/modules/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 #
 # RERO Invenio Base
 # Copyright (C) 2022 RERO.
+# Copyright (C) 2022 UCLouvain.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, version 3 of the License.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""Generic backend libraries for RERO Invenio instances."""
+"""RERO Invenio Base Modules extension."""
```

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/ext.py` & `rero_invenio_base-0.2.1/rero_invenio_base/ext.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/modules/__init__.py` & `rero_invenio_base-0.2.1/rero_invenio_base/modules/export/proxies.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,8 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""RERO Invenio Base Modules extension."""
+"""Helper proxy."""
+
+from flask import current_app
+from werkzeug.local import LocalProxy
+
+current_export = LocalProxy(
+    lambda: current_app.extensions["rero_invenio_base_exports"]
+)
+"""Helper proxy to get the current 'RERO Invenio base' exports extension."""
```

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/modules/export/__init__.py` & `rero_invenio_base-0.2.1/rero_invenio_base/modules/export/__init__.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/modules/export/config.py` & `rero_invenio_base-0.2.1/rero_invenio_base/modules/export/config.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/modules/export/ext.py` & `rero_invenio_base-0.2.1/rero_invenio_base/modules/export/ext.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/modules/export/proxies.py` & `rero_invenio_base-0.2.1/rero_invenio_base/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # -*- coding: utf-8 -*-
 #
 # RERO Invenio Base
 # Copyright (C) 2022 RERO.
-# Copyright (C) 2022 UCLouvain.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as published by
 # the Free Software Foundation, version 3 of the License.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""Helper proxy."""
+"""Version information for RERO Invenio Base.
 
-from flask import current_app
-from werkzeug.local import LocalProxy
+This file is imported by ``rero_invenio_base.__init__``,
+and parsed by ``setup.py``.
+"""
+from importlib import metadata
 
-current_export = LocalProxy(
-    lambda: current_app.extensions["rero_invenio_base_exports"]
-)
-"""Helper proxy to get the current 'RERO Invenio base' exports extension."""
+__version__ = metadata.version(__package__)
```

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/modules/export/views.py` & `rero_invenio_base-0.2.1/rero_invenio_base/modules/export/views.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/modules/tasks.py` & `rero_invenio_base-0.2.1/rero_invenio_base/modules/tasks.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/rero_invenio_base/modules/utils.py` & `rero_invenio_base-0.2.1/rero_invenio_base/modules/utils.py`

 * *Files identical despite different names*

### Comparing `rero_invenio_base-0.2.0/setup.py` & `rero_invenio_base-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,23 @@
  'rero_invenio_base.modules.export']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Mako>=1.2.2',
- 'PyYAML>=6.0,<7.0',
+ 'PyYAML<=7.0',
+ 'docker-services-cli>=0.6.1,<0.7.0',
  'dparse>=0.5.2',
- 'invenio-db>=1.0.14,<2.0.0',
- 'invenio-indexer<2.0.0',
- 'invenio-records-rest',
- 'invenio-search[elasticsearch7]>=1.4.2,<2.0.0',
- 'jsonpatch>=1.32,<2.0',
- 'pydocstyle<6.2.0']
+ 'invenio-db[postgresql]>=1.0.14,<1.1.0',
+ 'invenio-indexer<2.2.0',
+ 'invenio-records-rest<2.3.0',
+ 'invenio-search[elasticsearch7]>=1.4.2,<3.0.0',
+ 'jsonpatch<=2.0',
+ 'pydocstyle>=6.1.1,<6.2.0']
 
 entry_points = \
 {'console_scripts': ['check_json = rero_invenio_base.cli.utils:check_json',
                      'check_license = '
                      'rero_invenio_base.cli.utils:check_license',
                      'rero = rero_invenio_base.cli:rero'],
  'flask.commands': ['rero = rero_invenio_base.cli:rero'],
@@ -34,15 +35,15 @@
                                  'rero_invenio_base.modules.export.views:create_blueprint_from_app'],
  'invenio_base.apps': ['rero-invenio-base-export = '
                        'rero_invenio_base.modules.export.ext:ReroInvenioBaseExportApp'],
  'invenio_celery.tasks': ['rero = rero_invenio_base.modules.tasks']}
 
 setup_kwargs = {
     'name': 'rero-invenio-base',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Generic backend libraries for RERO Invenio instances.',
     'long_description': '..\n    RERO Invenio Base\n    Copyright (C) 2022 RERO.\n\n    This program is free software: you can redistribute it and/or modify\n    it under the terms of the GNU Affero General Public License as published by\n    the Free Software Foundation, version 3 of the License.\n\n    This program is distributed in the hope that it will be useful,\n    but WITHOUT ANY WARRANTY; without even the implied warranty of\n    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the\n    GNU Affero General Public License for more details.\n\n    You should have received a copy of the GNU Affero General Public License\n    along with this program. If not, see <http://www.gnu.org/licenses/>.\n\n===================\n RERO Invenio Base\n===================\n\n.. image:: https://github.com/rero/rero-invenio-base/workflows/CI/badge.svg\n        :target: https://github.com/rero/rero-invenio-base/actions?query=workflow%3ACI\n\n.. image:: https://img.shields.io/github/tag/rero/rero-invenio-base.svg\n        :target: https://github.com/rero/rero-invenio-base/releases\n\n.. image:: https://img.shields.io/pypi/dm/rero-invenio-base.svg\n        :target: https://pypi.python.org/pypi/rero-invenio-base\n\n.. image:: https://img.shields.io/github/license/rero/rero-invenio-base.svg\n        :target: https://github.com/rero/rero-invenio-base/blob/master/LICENSE\n\nGeneric backend libraries for RERO Invenio instances.\n\nFurther documentation is available on\nhttps://rero-invenio-base.readthedocs.io/\n',
     'author': 'RERO',
     'author_email': 'software@rero.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `rero_invenio_base-0.2.0/PKG-INFO` & `rero_invenio_base-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: rero-invenio-base
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generic backend libraries for RERO Invenio instances.
 License: AGPL-3.0
 Author: RERO
 Author-email: software@rero.ch
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Mako (>=1.2.2)
-Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: PyYAML (<=7.0)
+Requires-Dist: docker-services-cli (>=0.6.1,<0.7.0)
 Requires-Dist: dparse (>=0.5.2)
-Requires-Dist: invenio-db (>=1.0.14,<2.0.0)
-Requires-Dist: invenio-indexer (<2.0.0)
-Requires-Dist: invenio-records-rest
-Requires-Dist: invenio-search[elasticsearch7] (>=1.4.2,<2.0.0)
-Requires-Dist: jsonpatch (>=1.32,<2.0)
-Requires-Dist: pydocstyle (<6.2.0)
+Requires-Dist: invenio-db[postgresql] (>=1.0.14,<1.1.0)
+Requires-Dist: invenio-indexer (<2.2.0)
+Requires-Dist: invenio-records-rest (<2.3.0)
+Requires-Dist: invenio-search[elasticsearch7] (>=1.4.2,<3.0.0)
+Requires-Dist: jsonpatch (<=2.0)
+Requires-Dist: pydocstyle (>=6.1.1,<6.2.0)
 Description-Content-Type: text/x-rst
 
 ..
     RERO Invenio Base
     Copyright (C) 2022 RERO.
 
     This program is free software: you can redistribute it and/or modify
```

