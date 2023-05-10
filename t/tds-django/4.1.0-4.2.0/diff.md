# Comparing `tmp/tds-django-4.1.0.tar.gz` & `tmp/tds-django-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tds-django-4.1.0.tar", last modified: Tue Aug 16 02:59:48 2022, max compression
+gzip compressed data, was "tds-django-4.2.0.tar", last modified: Wed May 10 12:30:54 2023, max compression
```

## Comparing `tds-django-4.1.0.tar` & `tds-django-4.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 02:59:48.516051 tds-django-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-08-16 02:59:39.000000 tds-django-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-08-16 02:59:48.516051 tds-django-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-08-16 02:59:39.000000 tds-django-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 02:59:48.516051 tds-django-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-08-16 02:59:39.000000 tds-django-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 02:59:48.512050 tds-django-4.1.0/tds_django/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5805 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7082 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/creation.py
--rw-r--r--   0 runner    (1001) docker     (121)    13082 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/features.py
--rw-r--r--   0 runner    (1001) docker     (121)     8373 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6708 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/introspection.py
--rw-r--r--   0 runner    (1001) docker     (121)    12859 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/patches.py
--rw-r--r--   0 runner    (1001) docker     (121)    21625 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 02:59:48.516051 tds-django-4.1.0/tds_django/sql/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7800 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/sql/clr.sql
--rw-r--r--   0 runner    (1001) docker     (121)     4961 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/sql/init.sql
--rw-r--r--   0 runner    (1001) docker     (121)     6236 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/sql/queries.py
--rw-r--r--   0 runner    (1001) docker     (121)    21250 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/tz.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-08-16 02:59:39.000000 tds-django-4.1.0/tds_django/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 02:59:48.516051 tds-django-4.1.0/tds_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-08-16 02:59:48.000000 tds-django-4.1.0/tds_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-08-16 02:59:48.000000 tds-django-4.1.0/tds_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 02:59:48.000000 tds-django-4.1.0/tds_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-16 02:59:48.000000 tds-django-4.1.0/tds_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:54.394771 tds-django-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-10 12:30:41.000000 tds-django-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-10 12:30:54.394771 tds-django-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-10 12:30:41.000000 tds-django-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:30:54.394771 tds-django-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-05-10 12:30:41.000000 tds-django-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:54.390771 tds-django-4.2.0/tds_django/
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5805 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7431 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/creation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14532 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8818 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6969 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12859 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2081 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/patches.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21732 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:54.394771 tds-django-4.2.0/tds_django/sql/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7800 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/sql/clr.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/sql/init.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/sql/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21250 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/tz.py
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-05-10 12:30:41.000000 tds-django-4.2.0/tds_django/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:30:54.394771 tds-django-4.2.0/tds_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-10 12:30:54.000000 tds-django-4.2.0/tds_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-10 12:30:54.000000 tds-django-4.2.0/tds_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:30:54.000000 tds-django-4.2.0/tds_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-10 12:30:54.000000 tds-django-4.2.0/tds_django.egg-info/top_level.txt
```

### Comparing `tds-django-4.1.0/LICENSE` & `tds-django-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tds-django-4.1.0/PKG-INFO` & `tds-django-4.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 Metadata-Version: 2.1
 Name: tds-django
-Version: 4.1.0
+Version: 4.2.0
 Summary: Django backend for SQL Server using tds
 Home-page: https://github.com/ecogels/tds-django
 Author: Etienne Cogels
 Author-email: ecogels@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ecogels/tds-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQL Server backend for Django >=3.2
 - django 4
 - django 3.2 (pypi package version 0.1)
-- tested and used with SQL Server 2017
+- tested and used with SQL Server 2017 and for version 4.2 with python 3.11 only
 
 ## Warning
 - There is an official package supported by microsoft, microsoft/mssql-django.
 - This package does not need pyodbc nor the microsoft odbc driver, only pytds.
-- This passes about 15000 tests from the django test suite but I personally use the django ORM mostly in a basic way and
+- This passes about 15000 tests from the django test suite, but I personally use the django ORM in a basic way and
 don't use most of the features.
 
 ## Requirements
 - [python-tds](https://github.com/denisenkom/pytds)
 
 - optional:
   - bitarray, recommended by python-tds for performance
-  - for regex support you need to compile `clr/django_clr.cs` and install the resulting assembly or read and then run the `tds_django/sql/clr.sql` script.
-  - for date "math" as well as bitshift operations you need to read and run the `tds_django/sql/init.sql` script.
+  - for regex support you need to compile `clr/django_clr.cs` and install the resulting assembly or read and then run
+the `tds_django/sql/clr.sql` script.
+  - for date "math" as well as bit-shift operations you need to read and run the `tds_django/sql/init.sql` script.
     
 ## Unsupported
 - JSON
 - foreign keys to a nullable field (limitation of SQL Server)
 - feel free to read `tds_django/features.py` for more details.
 - queryset iterator with chunk size
 
 ## Warning If you have used another backend before
 - this one uses `uniqueidentifier` field for UUIDField while others may have used nvarchar.
 
 # Installation
+For django 4.2
+`pip install bitarray python-tds tds_django==4.2.0`
+
 For django 4.1
 `pip install bitarray python-tds tds_django==4.1.0`
 
 For django 4.0
 `pip install bitarray python-tds tds_django==4.0.0`
 
 For django 3.2
```

### Comparing `tds-django-4.1.0/README.md` & `tds-django-4.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # SQL Server backend for Django >=3.2
 - django 4
 - django 3.2 (pypi package version 0.1)
-- tested and used with SQL Server 2017
+- tested and used with SQL Server 2017 and for version 4.2 with python 3.11 only
 
 ## Warning
 - There is an official package supported by microsoft, microsoft/mssql-django.
 - This package does not need pyodbc nor the microsoft odbc driver, only pytds.
-- This passes about 15000 tests from the django test suite but I personally use the django ORM mostly in a basic way and
+- This passes about 15000 tests from the django test suite, but I personally use the django ORM in a basic way and
 don't use most of the features.
 
 ## Requirements
 - [python-tds](https://github.com/denisenkom/pytds)
 
 - optional:
   - bitarray, recommended by python-tds for performance
-  - for regex support you need to compile `clr/django_clr.cs` and install the resulting assembly or read and then run the `tds_django/sql/clr.sql` script.
-  - for date "math" as well as bitshift operations you need to read and run the `tds_django/sql/init.sql` script.
+  - for regex support you need to compile `clr/django_clr.cs` and install the resulting assembly or read and then run
+the `tds_django/sql/clr.sql` script.
+  - for date "math" as well as bit-shift operations you need to read and run the `tds_django/sql/init.sql` script.
     
 ## Unsupported
 - JSON
 - foreign keys to a nullable field (limitation of SQL Server)
 - feel free to read `tds_django/features.py` for more details.
 - queryset iterator with chunk size
 
 ## Warning If you have used another backend before
 - this one uses `uniqueidentifier` field for UUIDField while others may have used nvarchar.
 
 # Installation
+For django 4.2
+`pip install bitarray python-tds tds_django==4.2.0`
+
 For django 4.1
 `pip install bitarray python-tds tds_django==4.1.0`
 
 For django 4.0
 `pip install bitarray python-tds tds_django==4.0.0`
 
 For django 3.2
```

### Comparing `tds-django-4.1.0/setup.py` & `tds-django-4.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tds-django",
-    version="4.1.0",
+    version="4.2.0",
     author="Etienne Cogels",
     author_email="ecogels@users.noreply.github.com",
     description="Django backend for SQL Server using tds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ecogels/tds-django",
     project_urls={
@@ -19,14 +19,16 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Programming Language :: Python",
         "Topic :: Database",
         "Topic :: Software Development :: Libraries",
     ],
     packages=find_packages(),
     include_package_data=True,
     package_data={'': ['sql/*.sql']},
```

### Comparing `tds-django-4.1.0/tds_django/base.py` & `tds-django-4.2.0/tds_django/base.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.1.0/tds_django/compiler.py` & `tds-django-4.2.0/tds_django/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,25 @@
 from django.db.models.sql import compiler
 
 
 class SQLCompiler(compiler.SQLCompiler):
     _re_constant = re.compile(r'^\s*\(?\s*\d+\s*\)?\s*')
 
     def as_sql(self, with_limits=True, with_col_aliases=False):
+        if self.query.subquery and not with_limits:
+            self.query.clear_ordering(force=True)
+
         sql, params = super().as_sql(with_limits=with_limits, with_col_aliases=with_col_aliases)
         if with_limits and not self.query.low_mark and self.query.high_mark is not None:
             if self.query.combinator == 'union':
-                sql = f'SELECT TOP {self.query.high_mark} * FROM ({sql}) t'
+                try:
+                    idx = sql.index('ORDER BY')
+                    sql = f'SELECT TOP {self.query.high_mark} * FROM ({sql[:idx]}) t {sql[idx:]}'
+                except ValueError:
+                    sql = f'SELECT TOP {self.query.high_mark} * FROM ({sql}) t'
             else:
                 needle = 'SELECT DISTINCT' if self.query.distinct else 'SELECT'
                 sql = sql.replace(needle, needle + ' TOP %d' % self.query.high_mark, 1)
         if not params and hasattr(self, 'escape_if_noparams'):
             sql = sql % ()
         return sql, params
 
@@ -102,16 +109,16 @@
         )
 
         placeholder_rows, param_rows = self.assemble_as_sql(fields, value_rows)
 
         on_conflict_suffix_sql = self.connection.ops.on_conflict_suffix_sql(
             fields,
             self.query.on_conflict,
-            self.query.update_fields,
-            self.query.unique_fields,
+            (f.column for f in self.query.update_fields),
+            (f.column for f in self.query.unique_fields),
         )
         if (
             self.returning_fields
             and self.connection.features.can_return_columns_from_insert
         ):
             if self.connection.features.can_return_rows_from_bulk_insert:
                 result.append(
```

### Comparing `tds-django-4.1.0/tds_django/creation.py` & `tds-django-4.2.0/tds_django/creation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.db.backends.base.creation import BaseDatabaseCreation
 
 
 class DatabaseCreation(BaseDatabaseCreation):
 
     def create_test_db(self, *args, **kwargs):
         import os
-        db_name = super().create_test_db()
+        db_name = super().create_test_db(*args, **kwargs)
 
         here = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
         with self.connection.cursor() as cursor:
             for f in ['init.sql', 'clr.sql']:
                 with open(f'{here}/sql/{f}', 'r') as file:
                     sql = file.read()
                     for s in sql.split('\nGO\n'):
```

### Comparing `tds-django-4.1.0/tds_django/features.py` & `tds-django-4.2.0/tds_django/features.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     # json
     supports_json_field = False
     can_introspect_json_field = False  # ISJSON only validates json objects, not literals
     has_json_object_function = False
     supports_json_field_contains = False
     
     allow_sliced_subqueries_with_in = False  # TODO CHECK
+    allows_group_by_select_index = False
+
     can_create_inline_fk = False
 
     can_return_columns_from_insert = True
     can_return_id_from_insert = True
     can_rollback_ddl = True
     # can_use_chunked_reads = False
     greatest_least_ignores_nulls = True
@@ -29,17 +31,19 @@
     implied_column_null = True
     max_query_params = 1000
     requires_literal_defaults = True
 
     # supported_explain_formats = {'XML', }
     supports_boolean_expr_in_select_clause = False
     supports_covering_indexes = True
+    supports_comparing_boolean_expr = False
     supports_expression_indexes = False  # would need to manage computed column
     supports_ignore_conflicts = False
     supports_index_on_text_field = False
+    supports_order_by_nulls_modifier = False
     supports_over_clause = True
     supports_paramstyle_pyformat = False  # TODO
     supports_partially_nullable_unique_constraints = False
     supports_sequence_reset = False  # TODO
     supports_subqueries_in_group_by = False
     supports_temporal_subtraction = True
     supports_transactions = True
@@ -78,34 +82,38 @@
         },
         "test uses cursor directly and we don't fix the query, the query should set (SET IDENTITY_INSERT off)": {
             'migrations.test_operations.OperationTests.test_create_model_with_constraint',
             'migrations.test_operations.OperationTests.test_create_model_with_boolean_expression_in_check_constraint'
         },
         "unsupported by SQL Server": {
             # subquery in agg function
-            'aggregation.tests.AggregateTestCase.test_aggregation_subquery_annotation_values_collision',
             'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_on_exists',
-            'db_functions.math.test_mod.ModTests.test_float',
-            # subquery in avg
             'expressions_case.tests.CaseExpressionTests.test_annotate_with_in_clause',
-            # ORDER BY LOB in window function
-            'expressions_window.tests.WindowFunctionTests.test_key_transform',
+            'expressions.tests.BasicExpressionsTests.test_aggregate_subquery_annotation',
             # NTH_RESULT: could be done
             'expressions_window.tests.WindowFunctionTests.test_nth_returns_null',
             'expressions_window.tests.WindowFunctionTests.test_nthvalue',
             # order by constant
             'ordering.tests.OrderingTests.test_order_by_constant_value',
             # distinct + subquery, could work if rewrite distinct with group by
             'ordering.tests.OrderingTests.test_orders_nulls_first_on_filtered_subquery',
-            # sql server does not allow like predicates index
+            # sql server does not allow LIKE predicates index
             'indexes.tests.PartialIndexTests.test_multiple_conditions',
+            # alias in order by expression
+            'queries.test_qs_combinators.QuerySetSetOperationTests.test_ordering_by_f_expression_and_alias',
+            'tests.queries.test_qs_combinators.QuerySetSetOperationTests.test_union_order_with_null_first_last',
+            'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_order_with_null_first_last',
         },
         "Test is using hardcoded values that are different for sql server": {
             'aggregation.tests.AggregateTestCase.test_count_star',
             'cache.tests.CreateCacheTableForDBCacheTests.test_createcachetable_observes_database_router',
+            # assumes string starts with UPDATE when we do a SET NOCOUNT
+            'get_or_create.tests.UpdateOrCreateTests.test_update_only_defaults_and_pre_save_fields_when_local_fields',
+            # bug in test? we don't "supports_expression_indexes" but test assumes so
+            'schema.tests.SchemaTests.test_remove_ignored_unique_constraint_not_create_fk_index',
         },
         "Avg are cast as float, with can cause issues with decimals": {
             'aggregation_regress.tests.AggregationTests.test_values_list_annotation_args_ordering',
         },
         "client unsupported": {
             "dbshell.tests.DbshellCommandTestCase.test_command_missing",
         },
@@ -196,14 +204,24 @@
             "many_to_one_null.tests.ManyToOneNullTests.test_created_without_related",
             "many_to_one_null.tests.ManyToOneNullTests.test_get_related",
             "many_to_one_null.tests.ManyToOneNullTests.test_related_null_to_field",
             "many_to_one_null.tests.ManyToOneNullTests.test_related_set",
             "many_to_one_null.tests.ManyToOneNullTests.test_remove_from_wrong_set",
             "many_to_one_null.tests.ManyToOneNullTests.test_set",
             "many_to_one_null.tests.ManyToOneNullTests.test_set_clear_non_bulk",
+            "constraints.tests.UniqueConstraintTests.test_model_validation_with_condition",
+        },
+        "To look at when time is available? We don't use these features": {
+            'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_empty_condition',
+            'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_ref_multiple_subquery_annotation',
+            'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_ref_subquery_annotation',
+            'aggregation.tests.AggregateTestCase.test_aggregation_exists_multivalued_outeref',
+            'aggregation.tests.AggregateTestCase.test_group_by_nested_expression_with_params',
+            #
+            'schema.tests.SchemaTests.test_autofield_to_o2o',
         }
     }
 
     # Collation names for use by the Django test suite.
     test_collations = {
         'ci': 'Latin1_General_CI_AS',  # Case-insensitive.
         'cs': 'Latin1_General_BIN2',  # Case-sensitive.
```

### Comparing `tds-django-4.1.0/tds_django/functions.py` & `tds-django-4.2.0/tds_django/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.db.models import BooleanField, IntegerField, Lookup
 from django.db.models.aggregates import Avg, Count, StdDev, Variance
 from django.db.models.expressions import Value, OrderBy, OrderByList, Exists, RawSQL, Window, ExpressionList, Case, When, \
     DurationExpression, CombinedExpression
+from django.db.models.fields import DecimalField, FloatField
 from django.db.models.fields.json import HasKeyLookup
-from django.db.models.functions import Now, ATan2, Chr, Collate, Greatest, Least, Length, LPad, Random, \
+from django.db.models.functions import Now, ATan2, Cast, Chr, Collate, Greatest, Least, Length, LPad, Random, \
     Repeat, RPad, StrIndex, Substr, Log, Ln, Mod, Round, Degrees, Power, Radians, RowNumber
 from django.db.models.lookups import BuiltinLookup
 
 
 def as_sqlserver(expression):
     def decorator(func):
         setattr(expression, 'as_sqlserver', func)
@@ -156,15 +157,26 @@
 def ln(self, compiler, connection, **extra_context):
     return self.as_sql(compiler, connection, function='LOG', **extra_context)
 
 
 @as_sqlserver(Mod)
 def sqlserver_mod(self, compiler, connection, **extra_context):
     compiler.escape_if_noparams = True
-    return self.as_sql(compiler, connection, template='%(expressions)s', arg_joiner=' %% ', **extra_context)
+    # cast floatfield as decimal
+    output_field = DecimalField(decimal_places=12, max_digits=20)
+    clone = self.copy()
+    clone.set_source_expressions(
+        [
+            Cast(expression, output_field)
+            if isinstance(expression.output_field, FloatField)
+            else expression
+            for expression in self.get_source_expressions()
+        ]
+    )
+    return clone.as_sql(compiler, connection, template='%(expressions)s', arg_joiner=' %% ', **extra_context)
 
 
 @as_sqlserver(Power)
 def sqlserver_pow(self, compiler, connection, **extra_context):
     template = '%(function)s(CAST(%(expressions)s)'
     return self.as_sql(compiler, connection, **extra_context, template=template, arg_joiner=' AS FLOAT),')
```

### Comparing `tds-django-4.1.0/tds_django/introspection.py` & `tds-django-4.2.0/tds_django/introspection.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,19 @@
         """ As of django 3.2 django still does not take defaults into account
             Ignores collation if it is the server default
         """
         cursor.execute(Introspection.table_description, (table_name, ))
         extras = {line[0]: line[1:] for line in cursor.fetchall()}
 
         cursor.execute('SELECT TOP 1 * FROM %s' % self.connection.ops.quote_name(table_name, ))
-        return [FieldInfo(*column, *extras[column[0]]) for column in cursor.description]
+        return [FieldInfo(name, type_code,
+                          internal_size if display_size is None else display_size,
+                          internal_size, precision, scale, null_ok,
+                          *extras[name])
+                for name, type_code, display_size, internal_size, precision, scale, null_ok in cursor.description]
 
     def get_sequences(self, cursor, table_name, table_fields=()):
         cursor.execute(Introspection.sequences, (table_name, ))
         # SQL Server allows only one identity column per table
         # https://docs.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql-identity-property
         row = cursor.fetchone()
         return [{'table': table_name, 'column': row[0]}] if row else []
```

### Comparing `tds-django-4.1.0/tds_django/operations.py` & `tds-django-4.2.0/tds_django/operations.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.1.0/tds_django/patches.py` & `tds-django-4.2.0/tds_django/patches.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 _bulk = QuerySet.bulk_update
 
 
 def bulk_update(self, objs, fields, batch_size=None):
     affected = 0
     if connections[self.db].vendor == 'sqlserver':
-        if batch_size is not None and batch_size < 0:
+        if batch_size is not None and batch_size <= 0:
             raise ValueError('Batch size must be a positive integer.')
         if not fields:
             raise ValueError('Field names must be given to bulk_update().')
         objs = tuple(objs)
         if any(obj.pk is None for obj in objs):
             raise ValueError('All bulk_update() objects must have a primary key set.')
         field_names = {self.model._meta.get_field(name): name for name in fields}
```

### Comparing `tds-django-4.1.0/tds_django/schema.py` & `tds-django-4.2.0/tds_django/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 
 class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
     sql_create_column = 'ALTER TABLE %(table)s ADD %(column)s %(definition)s'
     sql_alter_column_default = 'ADD DEFAULT %(default)s FOR %(column)s'
     sql_delete_column = 'ALTER TABLE %(table)s DROP COLUMN %(column)s'
     sql_alter_column_no_default = 'DROP CONSTRAINT IF EXISTS %(column)s'
-    sql_alter_column_type = 'ALTER COLUMN %(column)s %(type)s'
-    sql_alter_column_collate = 'ALTER COLUMN %(column)s %(type)s %(collation)s'
+    sql_alter_column_type = 'ALTER COLUMN %(column)s %(type)s %(collation)s'
     sql_delete_index = 'DROP INDEX %(name)s ON %(table)s'
     sql_delete_table = Misc.delete_table
     sql_rename_column = "EXEC sp_rename '%(table)s.%(old_column)s', %(new_column)s, 'COLUMN'"
     sql_rename_table = 'EXEC sp_rename %(old_table)s, %(new_table)s'
 
     sql_alter_column_not_null = 'ALTER COLUMN %(column)s %(type)s NOT NULL'
     sql_alter_column_null = 'ALTER COLUMN %(column)s %(type)s NULL'
@@ -53,15 +52,15 @@
         else:
             return str(value)
 
     def _alter_column_default_sql(self, model, old_field, new_field, drop=False):
         if drop:
             with self.connection.cursor() as cursor:
                 defaults = self.connection.introspection.get_table_defaults(cursor, model._meta.db_table)
-                constraint_name = defaults.get(new_field.column, ['DEF_DOES_NOT_EXISTS'])[0]
+                constraint_name = defaults.get(new_field.column, ['DEF_DOES_NOT_EXIST'])[0]
             return (self.sql_alter_column_no_default % {
                 'column': constraint_name,
             }, [])
         return super()._alter_column_default_sql(model, old_field, new_field)
 
     def _is_identity_column(self, table_name, column_name):
         with self.connection.cursor() as cursor:
@@ -396,26 +395,27 @@
                 if sql:
                     self.execute(sql % {
                         'table': self.quote_name(table_name),
                         'name': self.quote_name(name),
                     })
         return reverse if new_field else None
 
-    def _alter_column_type_sql(self, model, old_field, new_field, new_type):
-        fragment, more = super()._alter_column_type_sql(model, old_field, new_field, new_type)
+    def _alter_column_type_sql(self, model, old_field, new_field, new_type, old_collation, new_collation):
+        fragment, more = super()._alter_column_type_sql(model, old_field, new_field, new_type, old_collation,
+                                                        new_collation)
         if not new_field.null:
             (sql, params) = fragment
             fragment = (sql + ' NOT NULL', params)
         # at this point the field would have already be renamed
         todo = self._remove_constraints(model, new_field.column, new_field)
         more += [(sql, []) for sql in todo]
         return fragment, more
 
-    def _collate_sql(self, collation):
-        return ' COLLATE ' + collation
+    def _collate_sql(self, collation, old_collation=None, table_name=None):
+        return ' COLLATE ' + collation if collation else ''
 
     def _field_should_be_indexed(self, model, field):
         """ we prevent the nullable unique constraint at table creation so we need to do it now """
         create_index = super()._field_should_be_indexed(model, field) or (field.unique and field.null)
         if create_index:
             db_type = field.db_type(self.connection)
             if db_type is not None and db_type.lower() in 'nvarchar(max)':
```

### Comparing `tds-django-4.1.0/tds_django/sql/clr.sql` & `tds-django-4.2.0/tds_django/sql/clr.sql`

 * *Files identical despite different names*

### Comparing `tds-django-4.1.0/tds_django/sql/init.sql` & `tds-django-4.2.0/tds_django/sql/init.sql`

 * *Files identical despite different names*

### Comparing `tds-django-4.1.0/tds_django/sql/queries.py` & `tds-django-4.2.0/tds_django/sql/queries.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.1.0/tds_django/tz.py` & `tds-django-4.2.0/tds_django/tz.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.1.0/tds_django/validation.py` & `tds-django-4.2.0/tds_django/validation.py`

 * *Files identical despite different names*

### Comparing `tds-django-4.1.0/tds_django.egg-info/PKG-INFO` & `tds-django-4.2.0/tds_django.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 Metadata-Version: 2.1
 Name: tds-django
-Version: 4.1.0
+Version: 4.2.0
 Summary: Django backend for SQL Server using tds
 Home-page: https://github.com/ecogels/tds-django
 Author: Etienne Cogels
 Author-email: ecogels@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ecogels/tds-django/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SQL Server backend for Django >=3.2
 - django 4
 - django 3.2 (pypi package version 0.1)
-- tested and used with SQL Server 2017
+- tested and used with SQL Server 2017 and for version 4.2 with python 3.11 only
 
 ## Warning
 - There is an official package supported by microsoft, microsoft/mssql-django.
 - This package does not need pyodbc nor the microsoft odbc driver, only pytds.
-- This passes about 15000 tests from the django test suite but I personally use the django ORM mostly in a basic way and
+- This passes about 15000 tests from the django test suite, but I personally use the django ORM in a basic way and
 don't use most of the features.
 
 ## Requirements
 - [python-tds](https://github.com/denisenkom/pytds)
 
 - optional:
   - bitarray, recommended by python-tds for performance
-  - for regex support you need to compile `clr/django_clr.cs` and install the resulting assembly or read and then run the `tds_django/sql/clr.sql` script.
-  - for date "math" as well as bitshift operations you need to read and run the `tds_django/sql/init.sql` script.
+  - for regex support you need to compile `clr/django_clr.cs` and install the resulting assembly or read and then run
+the `tds_django/sql/clr.sql` script.
+  - for date "math" as well as bit-shift operations you need to read and run the `tds_django/sql/init.sql` script.
     
 ## Unsupported
 - JSON
 - foreign keys to a nullable field (limitation of SQL Server)
 - feel free to read `tds_django/features.py` for more details.
 - queryset iterator with chunk size
 
 ## Warning If you have used another backend before
 - this one uses `uniqueidentifier` field for UUIDField while others may have used nvarchar.
 
 # Installation
+For django 4.2
+`pip install bitarray python-tds tds_django==4.2.0`
+
 For django 4.1
 `pip install bitarray python-tds tds_django==4.1.0`
 
 For django 4.0
 `pip install bitarray python-tds tds_django==4.0.0`
 
 For django 3.2
```

### Comparing `tds-django-4.1.0/tds_django.egg-info/SOURCES.txt` & `tds-django-4.2.0/tds_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

