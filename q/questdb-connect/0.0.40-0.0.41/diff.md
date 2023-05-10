# Comparing `tmp/questdb-connect-0.0.40.tar.gz` & `tmp/questdb-connect-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.40.tar", last modified: Mon May  8 10:52:16 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.41.tar", last modified: Wed May 10 09:18:08 2023, max compression
```

## Comparing `questdb-connect-0.0.40.tar` & `questdb-connect-0.0.41.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.089220 questdb-connect-0.0.40/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.40/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     3377 2023-05-08 10:52:16.088519 questdb-connect-0.0.40/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     2670 2023-05-08 10:47:52.000000 questdb-connect-0.0.40/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2520 2023-05-08 10:43:19.000000 questdb-connect-0.0.40/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-08 10:52:16.089396 questdb-connect-0.0.40/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.080563 questdb-connect-0.0.40/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.083524 questdb-connect-0.0.40/src/examples/
--rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.40/src/examples/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.40/src/examples/hello_world.py
--rw-r--r--   0 marregui   (501) staff       (20)     2433 2023-05-08 09:10:08.000000 questdb-connect-0.0.40/src/examples/psycopg2_connect.py
--rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.40/src/examples/sqlalchemy_orm.py
--rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.40/src/examples/sqlalchemy_raw.py
--rw-r--r--   0 marregui   (501) staff       (20)     2668 2023-05-08 09:30:05.000000 questdb-connect-0.0.40/src/examples/trigonometry.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.085248 questdb-connect-0.0.40/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-07 15:01:28.000000 questdb-connect-0.0.40/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.40/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.40/src/questdb_connect/function_names.py
--rw-r--r--   0 marregui   (501) staff       (20)    10535 2023-05-04 07:43:58.000000 questdb-connect-0.0.40/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.40/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.086397 questdb-connect-0.0.40/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     3377 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      703 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-08 10:52:16.000000 questdb-connect-0.0.40/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-08 10:52:16.087710 questdb-connect-0.0.40/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.40/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.40/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.40/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.344699 questdb-connect-0.0.41/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.41/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     3377 2023-05-10 09:18:08.344554 questdb-connect-0.0.41/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     2670 2023-05-08 10:47:52.000000 questdb-connect-0.0.41/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2520 2023-05-10 09:17:08.000000 questdb-connect-0.0.41/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-05-10 09:18:08.344733 questdb-connect-0.0.41/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.338707 questdb-connect-0.0.41/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.341460 questdb-connect-0.0.41/src/examples/
+-rw-r--r--   0 marregui   (501) staff       (20)     1140 2023-05-08 09:15:23.000000 questdb-connect-0.0.41/src/examples/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     1862 2023-05-08 09:22:31.000000 questdb-connect-0.0.41/src/examples/hello_world.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2433 2023-05-08 09:10:08.000000 questdb-connect-0.0.41/src/examples/psycopg2_connect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3879 2023-05-08 09:20:14.000000 questdb-connect-0.0.41/src/examples/sqlalchemy_orm.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2006 2023-05-08 09:20:14.000000 questdb-connect-0.0.41/src/examples/sqlalchemy_raw.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2668 2023-05-08 09:30:05.000000 questdb-connect-0.0.41/src/examples/trigonometry.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.342597 questdb-connect-0.0.41/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1938 2023-05-07 15:01:28.000000 questdb-connect-0.0.41/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)    11459 2023-05-07 15:04:17.000000 questdb-connect-0.0.41/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5160 2023-05-02 10:54:34.000000 questdb-connect-0.0.41/src/questdb_connect/function_names.py
+-rw-r--r--   0 marregui   (501) staff       (20)    10946 2023-05-10 09:15:20.000000 questdb-connect-0.0.41/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5787 2023-05-03 12:21:25.000000 questdb-connect-0.0.41/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.343609 questdb-connect-0.0.41/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     3377 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      703 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       25 2023-05-10 09:18:08.000000 questdb-connect-0.0.41/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-05-10 09:18:08.344265 questdb-connect-0.0.41/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-05-02 10:42:47.000000 questdb-connect-0.0.41/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     4325 2023-05-10 09:15:13.000000 questdb-connect-0.0.41/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.41/tests/test_types.py
```

### Comparing `questdb-connect-0.0.40/LICENSE` & `questdb-connect-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/PKG-INFO` & `questdb-connect-0.0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.40
+Version: 0.0.41
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.40/README.md` & `questdb-connect-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/pyproject.toml` & `questdb-connect-0.0.41/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.40"
+version = "0.0.41"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.40/src/examples/__init__.py` & `questdb-connect-0.0.41/src/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/examples/hello_world.py` & `questdb-connect-0.0.41/src/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/examples/psycopg2_connect.py` & `questdb-connect-0.0.41/src/examples/psycopg2_connect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/examples/sqlalchemy_orm.py` & `questdb-connect-0.0.41/src/examples/sqlalchemy_orm.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/examples/sqlalchemy_raw.py` & `questdb-connect-0.0.41/src/examples/sqlalchemy_raw.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/examples/trigonometry.py` & `questdb-connect-0.0.41/src/examples/trigonometry.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/questdb_connect/__init__.py` & `questdb-connect-0.0.41/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/questdb_connect/dialect.py` & `questdb-connect-0.0.41/src/questdb_connect/dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/questdb_connect/function_names.py` & `questdb-connect-0.0.41/src/questdb_connect/function_names.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.41/src/questdb_connect/superset_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 import re
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Tuple
 
 from sqlalchemy.sql import text
 from sqlalchemy.types import TypeEngine
-from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType
+from superset.db_engine_specs.base import BaseEngineSpec, BasicParametersMixin, BasicParametersType, TimeGrain
 from superset.utils import core as utils
 from superset.utils.core import GenericDataType
 
 import questdb_connect.dialect as qdbcd
 
 from . import remove_public_schema, types
 from .function_names import FUNCTION_NAMES
@@ -43,14 +43,15 @@
 class QDBEngineSpec(BaseEngineSpec, BasicParametersMixin):
     engine = 'questdb'
     engine_name = 'QuestDB Connect'
     default_driver = "psycopg2"
     encryption_parameters = {"sslmode": "prefer"}
     sqlalchemy_uri_placeholder = "questdb://user:password@host:port/dbname[?key=value&key=value...]"
     time_groupby_inline = True
+    allows_hidden_cc_in_orderby=True
     time_secondary_columns = True
     max_column_name_length = 120
     try_remove_schema_from_table_name = True
     supports_dynamic_schema = False
     allow_dml = True
     _time_grain_expressions = {
         None: '{col}',
@@ -121,14 +122,24 @@
         """
         if cls.allows_escaped_colons:
             clause = clause.replace(":", "\\:")
             remove_public_schema(clause)
         return text(remove_public_schema(clause))
 
     @classmethod
+    def get_time_grains(cls) -> Tuple[TimeGrain, ...]:
+        """Generate a tuple of supported time grains.
+        :return: All time grains supported by the engine
+        """
+        return tuple(
+            TimeGrain(duration, duration, func, duration)
+            for duration, func in cls._time_grain_expressions.copy().items()
+        )
+
+    @classmethod
     def epoch_to_dttm(cls) -> str:
         """SQL expression that converts epoch (seconds) to datetime that can be used in a
         query. The reference column should be denoted as `{col}` in the return
         expression, e.g. "FROM_UNIXTIME({col})"
         :return: SQL Expression
         """
         return '{col} * 1000000'
```

### Comparing `questdb-connect-0.0.40/src/questdb_connect/types.py` & `questdb-connect-0.0.41/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.41/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.40
+Version: 0.0.41
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.40/src/questdb_connect.egg-info/SOURCES.txt` & `questdb-connect-0.0.41/src/questdb_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/tests/test_dialect.py` & `questdb-connect-0.0.41/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.40/tests/test_types.py` & `questdb-connect-0.0.41/tests/test_types.py`

 * *Files identical despite different names*

