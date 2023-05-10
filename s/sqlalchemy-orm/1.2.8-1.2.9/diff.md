# Comparing `tmp/sqlalchemy-orm-1.2.8.tar.gz` & `tmp/sqlalchemy-orm-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-orm-1.2.8.tar", last modified: Thu May  4 23:55:50 2023, max compression
+gzip compressed data, was "sqlalchemy-orm-1.2.9.tar", last modified: Wed May 10 12:54:00 2023, max compression
```

## Comparing `sqlalchemy-orm-1.2.8.tar` & `sqlalchemy-orm-1.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:55:50.772112 sqlalchemy-orm-1.2.8/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-04 23:55:50.772112 sqlalchemy-orm-1.2.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1036 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-04 23:55:50.000000 sqlalchemy-orm-1.2.8/VERSION
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-04 23:55:50.773113 sqlalchemy-orm-1.2.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1257 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:55:50.766112 sqlalchemy-orm-1.2.8/sqlalchemy_orm/
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:55:50.769112 sqlalchemy-orm-1.2.8/sqlalchemy_orm/base/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/base/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      855 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/base/base.py
--rwxrwxrwx   0 root         (0) root         (0)    14522 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/base/helper.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/base/mapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/custom_types.py
--rw-rw-rw-   0 root         (0) root         (0)     6265 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/database.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:55:50.771113 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/cst.py
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    10155 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/main.py
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/models.py
--rw-rw-rw-   0 root         (0) root         (0)     5089 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/version.py
--rwxrwxrwx   0 root         (0) root         (0)     1401 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/filter.py
--rwxrwxrwx   0 root         (0) root         (0)     1264 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/order_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:55:50.772112 sqlalchemy-orm-1.2.8/sqlalchemy_orm/patterns/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/patterns/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3635 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/patterns/tag.py
--rwxrwxrwx   0 root         (0) root         (0)     1718 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/patterns/tag_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      143 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/patterns/taggable.py
--rw-rw-rw-   0 root         (0) root         (0)     4983 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/query.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/session.py
--rw-rw-rw-   0 root         (0) root         (0)     3161 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/typemapper.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-05-04 23:55:41.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:55:50.767112 sqlalchemy-orm-1.2.8/sqlalchemy_orm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-04 23:55:50.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-05-04 23:55:50.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 23:55:50.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-04 23:55:50.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-04 23:55:50.000000 sqlalchemy-orm-1.2.8/sqlalchemy_orm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:54:00.657504 sqlalchemy-orm-1.2.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-10 12:54:00.657504 sqlalchemy-orm-1.2.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-10 12:54:00.000000 sqlalchemy-orm-1.2.9/VERSION
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-10 12:54:00.658504 sqlalchemy-orm-1.2.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1257 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:54:00.651504 sqlalchemy-orm-1.2.9/sqlalchemy_orm/
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:54:00.654504 sqlalchemy-orm-1.2.9/sqlalchemy_orm/base/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/base/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      855 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/base/base.py
+-rwxrwxrwx   0 root         (0) root         (0)    15051 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/base/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/base/mapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/custom_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6265 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:54:00.656504 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/cst.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10155 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     5089 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/version.py
+-rwxrwxrwx   0 root         (0) root         (0)     1401 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1264 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/order_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:54:00.657504 sqlalchemy-orm-1.2.9/sqlalchemy_orm/patterns/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/patterns/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3635 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/patterns/tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     1718 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/patterns/tag_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      143 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/patterns/taggable.py
+-rw-rw-rw-   0 root         (0) root         (0)     4983 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/query.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     3187 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/typemapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2023-05-10 12:53:50.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:54:00.652504 sqlalchemy-orm-1.2.9/sqlalchemy_orm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-10 12:54:00.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-05-10 12:54:00.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:54:00.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-10 12:54:00.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-10 12:54:00.000000 sqlalchemy-orm-1.2.9/sqlalchemy_orm.egg-info/top_level.txt
```

### Comparing `sqlalchemy-orm-1.2.8/LICENSE` & `sqlalchemy-orm-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/PKG-INFO` & `sqlalchemy-orm-1.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-orm
-Version: 1.2.8
+Version: 1.2.9
 Summary: Data Relation Mapping framework for Python.
 Home-page: https://gitlab.com/parob/sqlalchemy-orm
-Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.8/sqlalchemy-orm-v1.2.8.tar.gz
+Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.9/sqlalchemy-orm-v1.2.9.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: SQLAlchemy,ORM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlalchemy-orm-1.2.8/README.md` & `sqlalchemy-orm-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/setup.py` & `sqlalchemy-orm-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/base/base.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/base/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/base/helper.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/base/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Set
+from typing import Set, Dict
 
 from sqlalchemy.orm import class_mapper, RelationshipProperty
 from sqlalchemy.orm.base import manager_of_class
 from sqlalchemy import String
 from sqlalchemy.orm.decl_api import declared_attr
 
 from sqlalchemy_orm.query import Query
@@ -98,18 +98,18 @@
             ):
                 key_ = (cls.identifier(), field)
                 Base.unresolved[key_] = flat_type.__name__
 
             else:
                 mappable.append(field)
 
-        cls.map(mappable)
-
         super().__init_subclass__(**kwargs)
 
+        cls.map(mappable)
+
         Base.models[cls.__name__] = cls
         Base.resolve()
 
         @event.listens_for(cls, "mapper_configured")
         def receive_mapper_configured(mapper, class_):
             Base.resolve()
 
@@ -131,24 +131,25 @@
     @classmethod
     def map(cls, fields):
         base = cls.base()
         inheritance = cls.__inheritance__
         is_base = cls.is_base()
         parent = cls.super()
 
+        had_primary_key = False
+
         if base and not is_base and inheritance:
             for pk in parent.primary_keys():
+                had_primary_key = True
                 key = pk.name
                 column = pk._copy()
                 fk = ForeignKey(f"{parent.__tablename__}.{key}")
                 column.append_foreign_key(fk)
                 setattr(cls, key, column)
 
-        had_primary_key = False
-
         # Map the direct fields to columns
         for field in fields:
             key, type_, default = field
 
             nullable = is_nullable(type_)
             primary_key = not had_primary_key and (
                 is_base or not inheritance or not base
@@ -444,23 +445,35 @@
 
 def get_type(field_type) -> Union[Type, str]:
     origin = typing_inspect.get_origin(field_type)
 
     if origin is List or origin is list or origin is Union:
         args = typing_inspect.get_args(field_type, evaluate=True)
         none_type = type(None)
-        args = [arg for arg in args if arg is not none_type]
+        non_none_args = set(arg for arg in args if arg is not none_type)
 
-        if len(args) != 1:
+        scalar_types = [str, float, bool, dict, list, type(None)]
+        non_scalar_args = set(arg for arg in args if arg not in scalar_types)
+
+        if len(non_scalar_args) == 0:
+            python_type = list
+            if len(non_none_args) == 1:
+                # inner_type = non_none_args.pop()
+                python_type = list  # List[inner_type]
+
+        elif len(non_none_args) != 1:
             raise TypeError(
                 f"Field type '{field_type}' origin: '{origin}' "
-                f"contained invalid args: '{args}'."
+                f"contained multiple different types: '{args}'."
             )
+        else:
+            python_type = args[0]
 
-        python_type = args[0]
+    elif origin is Dict or origin is dict:
+        python_type = dict
     elif origin is Mapped:
         python_type = get_type(typing_inspect.get_args(field_type, evaluate=True)[0])
     else:
         python_type = field_type
 
     if hasattr(python_type, "__forward_arg__"):
         python_type = python_type.__forward_arg__
```

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/custom_types.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/custom_types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/database.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/database.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/cst.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/cst.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/helpers.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/main.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/main.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/models.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/models.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/parser.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/parser.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/eralchemy/sqla.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/eralchemy/sqla.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/filter.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/filter.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/order_by.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/order_by.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/patterns/tag.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/patterns/tag.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/patterns/tag_mixin.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/patterns/tag_mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/proxy.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/proxy.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/query.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/query.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/typemapper.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/typemapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             timedelta: DateTime(),
             int: Integer(),
             Decimal: Numeric(),
             float: Float(),
             bytes: LargeBinary(),
             bool: Boolean(),
             dict: JSON(),
+            list: JSON(),
             UUID: Uuid(),
             **type_map,
         }
         self.type_factories: List[TypeFactory] = []
         _types = types + get_all_subclasses(TypeEngine)
 
         for type_ in _types:
```

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm/utils.py` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm/utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm.egg-info/PKG-INFO` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-orm
-Version: 1.2.8
+Version: 1.2.9
 Summary: Data Relation Mapping framework for Python.
 Home-page: https://gitlab.com/parob/sqlalchemy-orm
-Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.8/sqlalchemy-orm-v1.2.8.tar.gz
+Download-URL: https://gitlab.com/parob/sqlalchemy-orm/-/archive/v1.2.9/sqlalchemy-orm-v1.2.9.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: SQLAlchemy,ORM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlalchemy-orm-1.2.8/sqlalchemy_orm.egg-info/SOURCES.txt` & `sqlalchemy-orm-1.2.9/sqlalchemy_orm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

