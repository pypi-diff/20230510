# Comparing `tmp/ardilla-0.0.1a0.tar.gz` & `tmp/ardilla-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.0.1a0.tar", last modified: Tue May  9 15:27:39 2023, max compression
+gzip compressed data, was "ardilla-0.0.2a0.tar", last modified: Wed May 10 03:05:52 2023, max compression
```

## Comparing `ardilla-0.0.1a0.tar` & `ardilla-0.0.2a0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 15:27:39.280898 ardilla-0.0.1a0/
--rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.1a0/LICENCE
--rw-rw-rw-   0        0        0     2802 2023-05-09 15:27:39.279612 ardilla-0.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0     2156 2023-05-09 14:51:37.000000 ardilla-0.0.1a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 15:27:39.223513 ardilla-0.0.1a0/ardilla/
--rw-rw-rw-   0        0        0      106 2023-05-08 02:18:14.000000 ardilla-0.0.1a0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     1719 2023-05-09 15:05:34.000000 ardilla-0.0.1a0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:27:39.274611 ardilla-0.0.1a0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.1a0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0     5087 2023-05-09 03:28:06.000000 ardilla-0.0.1a0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0      658 2023-05-09 03:26:46.000000 ardilla-0.0.1a0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     5086 2023-05-09 02:30:46.000000 ardilla-0.0.1a0/ardilla/crud.py
--rw-rw-rw-   0        0        0     1091 2023-05-08 15:23:13.000000 ardilla-0.0.1a0/ardilla/engine.py
--rw-rw-rw-   0        0        0      157 2023-05-08 02:03:09.000000 ardilla-0.0.1a0/ardilla/errors.py
--rw-rw-rw-   0        0        0     1106 2023-05-09 14:59:59.000000 ardilla-0.0.1a0/ardilla/models.py
--rw-rw-rw-   0        0        0     1327 2023-05-09 14:59:10.000000 ardilla-0.0.1a0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:27:39.262387 ardilla-0.0.1a0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     2802 2023-05-09 15:27:39.000000 ardilla-0.0.1a0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-05-09 15:27:39.000000 ardilla-0.0.1a0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 15:27:39.000000 ardilla-0.0.1a0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-09 15:27:39.000000 ardilla-0.0.1a0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-09 15:27:39.000000 ardilla-0.0.1a0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      801 2023-05-09 15:26:46.000000 ardilla-0.0.1a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 15:27:39.281910 ardilla-0.0.1a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.863148 ardilla-0.0.2a0/
+-rw-rw-rw-   0        0        0     1084 2023-05-08 03:28:44.000000 ardilla-0.0.2a0/LICENCE
+-rw-rw-rw-   0        0        0     2893 2023-05-10 03:05:52.863148 ardilla-0.0.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2226 2023-05-10 02:41:02.000000 ardilla-0.0.2a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.755811 ardilla-0.0.2a0/ardilla/
+-rw-rw-rw-   0        0        0      106 2023-05-08 02:18:14.000000 ardilla-0.0.2a0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     2212 2023-05-10 02:30:00.000000 ardilla-0.0.2a0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.845105 ardilla-0.0.2a0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.0.2a0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     6118 2023-05-10 02:39:24.000000 ardilla-0.0.2a0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0      760 2023-05-10 02:34:10.000000 ardilla-0.0.2a0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     5958 2023-05-10 02:39:55.000000 ardilla-0.0.2a0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     1045 2023-05-09 21:05:12.000000 ardilla-0.0.2a0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      212 2023-05-10 02:29:23.000000 ardilla-0.0.2a0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     1106 2023-05-09 14:59:59.000000 ardilla-0.0.2a0/ardilla/models.py
+-rw-rw-rw-   0        0        0     1327 2023-05-09 20:34:49.000000 ardilla-0.0.2a0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.804321 ardilla-0.0.2a0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0     2893 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 03:05:52.000000 ardilla-0.0.2a0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      850 2023-05-10 02:49:34.000000 ardilla-0.0.2a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 03:05:52.863148 ardilla-0.0.2a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 03:05:52.861365 ardilla-0.0.2a0/tests/
+-rw-rw-rw-   0        0        0     4121 2023-05-10 02:48:27.000000 ardilla-0.0.2a0/tests/test_async.py
+-rw-rw-rw-   0        0        0      454 2023-05-09 18:32:20.000000 ardilla-0.0.2a0/tests/test_models.py
+-rw-rw-rw-   0        0        0     3793 2023-05-10 02:47:41.000000 ardilla-0.0.2a0/tests/test_sync.py
```

### Comparing `ardilla-0.0.1a0/LICENCE` & `ardilla-0.0.2a0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.1a0/PKG-INFO` & `ardilla-0.0.2a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: async
+Provides-Extra: dev
 License-File: LICENCE
 
 # ardilla
 
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
 
 A very simple library to quickly add SQLite to your program.
@@ -64,27 +65,28 @@
     user_crud.save_many(user, user2, user3)
     # get many
     users = user_crud.get_many(age=35)
 ```
 
 ## Supported CRUD methods:
  - `crud.get_or_none` Returns an object or None
+ - `crud.insert` Inserts a record, rises errors if there's a conflict
  - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
  - `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
  - `crud.get_all` equivalent to `SELECT * FROM tablename`
  - `crud.get_many` returns all the objects that meet criteria
  - `crud.save_one` upserts an object
  - `crud.save_many` upserts many objects
  - `crud.delete_one` deletes one object
  - `crud.delete_many` deletes many objects
 
 
 ## To-dos
 
 - [ ] Docstring everything using Google format
+- [ ] Add testing
 - [ ] Add proper documentation
   - propper as in a site with how to use
 - [x] Add a schema generator 
   - There should be a method to generate a table's schema off the pydantic model. 
 - [ ] Add a method somewhere to fetch relationships. 
-- [ ] Add examples
 - [ ] Improve this readme
```

### Comparing `ardilla-0.0.1a0/README.md` & `ardilla-0.0.2a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -48,27 +48,28 @@
     user_crud.save_many(user, user2, user3)
     # get many
     users = user_crud.get_many(age=35)
 ```
 
 ## Supported CRUD methods:
  - `crud.get_or_none` Returns an object or None
+ - `crud.insert` Inserts a record, rises errors if there's a conflict
  - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
  - `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
  - `crud.get_all` equivalent to `SELECT * FROM tablename`
  - `crud.get_many` returns all the objects that meet criteria
  - `crud.save_one` upserts an object
  - `crud.save_many` upserts many objects
  - `crud.delete_one` deletes one object
  - `crud.delete_many` deletes many objects
 
 
 ## To-dos
 
 - [ ] Docstring everything using Google format
+- [ ] Add testing
 - [ ] Add proper documentation
   - propper as in a site with how to use
 - [x] Add a schema generator 
   - There should be a method to generate a table's schema off the pydantic model. 
 - [ ] Add a method somewhere to fetch relationships. 
-- [ ] Add examples
 - [ ] Improve this readme
```

### Comparing `ardilla-0.0.1a0/ardilla/abc.py` & `ardilla-0.0.2a0/ardilla/abc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,75 @@
-from typing import Generic, Self
+from typing import Generic, Self, Literal
 from abc import abstractmethod, ABC
 
 from .errors import MissingEngine
 from .engine import Engine
 from .models import M, Model as BaseModel
 
 
 class CrudABC(ABC):
-    engine: Engine = None
+    engine: Engine
     
-    def __init__(self, Model: M, engine: Engine | None = None) -> None:
+    def __init__(self, Model: type[M], engine: Engine | None = None) -> None:
         if engine:
             self.engine = engine
+        
         self.Model = Model
         if Model.__schema__:
             self.engine.schemas.add(Model.__schema__)
         self.tablename = Model.__tablename__
         self.columns = tuple(Model.__fields__)
     
-    def __new__(cls, Model: M, engine: Engine | None = None) -> Self:
+    def __new__(cls, Model: type[M], engine: Engine | None = None) -> Self:
         if not issubclass(Model, BaseModel):
             raise TypeError('Model param has to be a subclass of model')
         
-        if not isinstance(engine, Engine) and not isinstance(cls.engine, Engine):
+        cls_engine = getattr(cls, 'engine', None)
+        
+        if not isinstance(engine, Engine) and not isinstance(cls_engine, Engine):
             raise MissingEngine(
                 "You must either set the engine at class level (Crud.engine = Engine(...))"
                 "or pass it as an argument."
             )
         return super().__new__(cls)
         
     # Create
+    @abstractmethod        
+    def _do_insert(self, ignore: bool = False, returning: bool = True, / , **kws): pass
+    
+    @abstractmethod    
+    def insert(self, **kws): pass
+    
     @abstractmethod
     def insert_or_ignore(self): pass
 
     # Read
     @abstractmethod
-    def get_all(self): pass
+    def get_all(self) -> list[M]: pass
 
     @abstractmethod
-    def get_many(self): pass
+    def get_many(self, **kws) -> list[M]: pass
 
     @abstractmethod
-    def get_or_create(self): pass
+    def get_or_create(self, **kws) -> tuple[M, bool]: pass
 
     @abstractmethod
-    def get_or_none(self): pass
+    def get_or_none(self, **kws) -> M | None: pass
     
     @abstractmethod
-    def _get_or_none_any(self): pass
+    def _get_or_none_any(self, many: bool, **kws) -> list[M] | M | None: pass
 
     # Update
     @abstractmethod
-    def save_one(self): pass
+    def save_one(self, obj: M) -> Literal[True]: pass
     
     @abstractmethod
-    def save_many(self): pass
+    def save_many(self, *objs: M) -> Literal[True]: pass
 
     # Delete
     @abstractmethod
-    def delete_one(self): pass
+    def delete_one(self, obj: M) -> Literal[True]: pass
 
     @abstractmethod
-    def delete_many(self): pass
+    def delete_many(self, *objs: M) -> Literal[True]: pass
```

### Comparing `ardilla-0.0.1a0/ardilla/asyncio/crud.py` & `ardilla-0.0.2a0/ardilla/asyncio/crud.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from typing import Literal, Generic, Self
 
+import aiosqlite
+
 from .engine import AsyncEngine
 
+from ..errors import QueryExecutionError
 from ..models import M
 from ..abc import CrudABC
 
 
 class AsyncCrud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
     engine: AsyncEngine
@@ -32,27 +35,53 @@
                     if result:
                         return self.Model(**result)
 
     async def get_or_none(self, **kws) -> M | None:
         """Gets an object from a database or None if not found"""
         return await self._get_or_none_any(many=False, **kws)
 
-    async def insert_or_ignore(self, **kws) -> M | None:
-        """inserts a the object of a row or ignores it if it already exists"""
+    async def _do_insert(self, ignore: bool = False, returning: bool = True, / , **kws):
         keys, vals = zip(*kws.items())
         placeholders = ", ".join("?" * len(keys))
         cols = ", ".join(keys)
-        q = f"INSERT OR IGNORE INTO {self.tablename} ({cols}) VALUES ({placeholders}) RETURNING *;"
-
+        
+        q = "INSERT OR IGNORE " if ignore else "INSERT "
+        q += f"INTO {self.tablename} ({cols}) VALUES ({placeholders})"
+        q += " RETURNING *;" if returning else ";"
+        
         async with self.engine as con:
-            async with con.execute(q, vals) as cur:
+            con = await self.engine.connect()
+            cur = None
+            try:
+                cur = await con.execute(q, vals)
+            except aiosqlite.IntegrityError as e:
+                raise QueryExecutionError(str(e))
+            else:
                 result = await cur.fetchone()
                 await con.commit()
-                if result:
+                if returning and result:
                     return self.Model(**result)
+            finally:
+                if cur is not None:
+                    await cur.close()
+                await con.close()
+    
+    async def insert(self, **kws):
+        """
+        Inserts a record into the database.
+        Returns:
+            Model | None: Returns a model only if newly created
+        Rises: 
+            ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
+        """
+        return await self._do_insert(False, True, **kws)
+
+    async def insert_or_ignore(self, **kws) -> M | None:
+        """inserts a the object of a row or ignores it if it already exists"""
+        return await self._do_insert(True, True, **kws)
 
     async def get_or_create(self, **kws) -> tuple[M, bool]:
         """Returns object and bool indicated if it was created or not"""
         created = False
         result = await self.get_or_none(**kws)
         if not result:
             result = await self.insert_or_ignore(**kws)
```

### Comparing `ardilla-0.0.1a0/ardilla/asyncio/engine.py` & `ardilla-0.0.2a0/ardilla/asyncio/engine.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from __future__ import annotations
 import aiosqlite
 
 from ..models import M
 from ..engine import Engine
 
 class AsyncEngine(Engine):
-        
-    async def __aenter__(self) -> aiosqlite.Connection:
+    
+    async def connect(self) -> aiosqlite.Connection:
         con = await aiosqlite.connect(self.path)
         con.row_factory = aiosqlite.Row
-        self.con = con
         return con
+        
+    async def __aenter__(self) -> aiosqlite.Connection:
+        self.con = await self.connect()
+        return self.con
 
     async def __aexit__(self, *_):
         await self.con.close()
     
     
     async def setup(self):
         async with self as con:
```

### Comparing `ardilla-0.0.1a0/ardilla/crud.py` & `ardilla-0.0.2a0/ardilla/crud.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,80 @@
+import sqlite3
 from typing import Literal, Generic, Self
 
 from .engine import Engine
 from .abc import CrudABC
 from .models import M, Model as BaseModel
-from .errors import MissingEngine
+from .errors import QueryExecutionError
 
 
 class Crud(CrudABC, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
 
-    def _get_or_none_any(self, many: bool, **kws):
+    def _get_or_none_any(self, many: bool, **kws) -> list[M] | M | None:
         """
         private helper to the get_or_none queries.
         if param "many" is true it will return a list of matches else will return only one record
         """
         keys, vals = zip(*kws.items())
         to_match = f" AND ".join(f"{k} = ?" for k in keys)
 
         limit = 'LIMIT 1;' if not many else ';'
         q = f"SELECT * FROM {self.tablename} WHERE ({to_match}) {limit}"
         with self.engine as con:
             with self.engine.cursor(con) as cur:
                 cur.execute(q, vals)
                 if many:
-                    result = cur.fetchall()
-                    return [self.Model(**entry) for entry in result]
+                    results: list[dict] = cur.fetchall()
+                    return [self.Model(**entry) for entry in results]
                 else:
-                    result = cur.fetchone()
+                    result: dict = cur.fetchone()
                     if result:
                         return self.Model(**result)
+        return
 
 
     def get_or_none(self, **kws) -> M | None:
         """Gets an object from a database or None if not found"""
         return self._get_or_none_any(many=False, **kws)
-
-    def insert_or_ignore(self, **kws) -> M | None:
-        """inserts a the object of a row or ignores it if it already exists"""
+    
+    def _do_insert(self, ignore: bool = False, returning: bool = True, / , **kws):
         keys, vals = zip(*kws.items())
         placeholders = ", ".join("?" * len(keys))
         cols = ", ".join(keys)
-        q = f"INSERT OR IGNORE INTO {self.tablename} ({cols}) VALUES ({placeholders}) RETURNING *;"
+        
+        q = "INSERT OR IGNORE " if ignore else "INSERT "
+        q += f"INTO {self.tablename} ({cols}) VALUES ({placeholders})"
+        q += " RETURNING *;" if returning else ";"
+        
         with self.engine as con:
             with self.engine.cursor(con) as cur:
-                cur.execute(q, vals)
+                try:
+                    cur.execute(q, vals)
+                except sqlite3.IntegrityError as e:
+                    raise QueryExecutionError(str(e)) 
+                    
                 result = cur.fetchone()
                 con.commit()
-                if result:
+                if returning and result:
                     return self.Model(**result)
+    
+    def insert(self, **kws):
+        """
+        Inserts a record into the database.
+        Returns:
+            Model | None: Returns a model only if newly created
+        Rises: 
+            ardilla.error.QueryExecutionError: if there's a conflict when inserting the record
+        """
+        return self._do_insert(False, True, **kws)
+
+    def insert_or_ignore(self, **kws) -> M | None:
+        """inserts a the object of a row or ignores it if it already exists"""
+        return self._do_insert(True, True, **kws)
         
 
     def get_or_create(self, **kws) -> tuple[M, bool]:
         """Returns object and bool indicated if it was created or not"""
         created = False
         result = self.get_or_none(**kws)
         if not result:
@@ -101,15 +124,17 @@
         Deletes the object from the database (won't delete the actual object)
         queries only by the Model id fields (fields suffixed with 'id')
         """
         obj_dict = obj.dict()
         id_cols = tuple([k for k in obj_dict if "id" in k])
         placeholders = ", ".join(f"{k} = ?" for k in id_cols)
         vals = tuple([obj_dict[k] for k in id_cols])
-        q = f"DELETE FROM {self.tablename} WHERE ({placeholders});"
+        q = f"""
+        DELETE FROM {self.tablename} WHERE ({placeholders});
+        """
         with self.engine as con:
             con.execute(q, vals)
             con.commit()
         
         return True
 
     def delete_many(self, *objs: M) -> Literal[True]:
```

### Comparing `ardilla-0.0.1a0/ardilla/engine.py` & `ardilla-0.0.2a0/ardilla/engine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 import sqlite3
-from typing import Generic
 
 from .models import M
 
-Crud = Generic()
 
 class ContextCursor:
     def __init__(self, con: sqlite3.Connection):
         self.con = con
     
     def __enter__(self) -> sqlite3.Cursor:
         self.cur = self.con.cursor()
```

### Comparing `ardilla-0.0.1a0/ardilla/models.py` & `ardilla-0.0.2a0/ardilla/models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.1a0/ardilla/schemas.py` & `ardilla-0.0.2a0/ardilla/schemas.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.0.1a0/ardilla.egg-info/PKG-INFO` & `ardilla-0.0.2a0/ardilla.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ardilla
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic
 Author-email: ChrisDewa <chrisdewa@duck.com>
 Project-URL: Homepage, https://github.com/chrisdewa/ardilla
 Project-URL: Bug Tracker, https://github.com/chrisdewa/ardilla/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: async
+Provides-Extra: dev
 License-File: LICENCE
 
 # ardilla
 
 Ardilla (pronounced *ahr-dee-yah*) means "**SQ**uirre**L**" in spanish.
 
 A very simple library to quickly add SQLite to your program.
@@ -64,27 +65,28 @@
     user_crud.save_many(user, user2, user3)
     # get many
     users = user_crud.get_many(age=35)
 ```
 
 ## Supported CRUD methods:
  - `crud.get_or_none` Returns an object or None
+ - `crud.insert` Inserts a record, rises errors if there's a conflict
  - `crud.insert_or_ignore` Inserts a record or silently ignores if it already exists
  - `crud.get_or_create` returns an tuple of the object and a bool, True if the object was newly created
  - `crud.get_all` equivalent to `SELECT * FROM tablename`
  - `crud.get_many` returns all the objects that meet criteria
  - `crud.save_one` upserts an object
  - `crud.save_many` upserts many objects
  - `crud.delete_one` deletes one object
  - `crud.delete_many` deletes many objects
 
 
 ## To-dos
 
 - [ ] Docstring everything using Google format
+- [ ] Add testing
 - [ ] Add proper documentation
   - propper as in a site with how to use
 - [x] Add a schema generator 
   - There should be a method to generate a table's schema off the pydantic model. 
 - [ ] Add a method somewhere to fetch relationships. 
-- [ ] Add examples
 - [ ] Improve this readme
```

### Comparing `ardilla-0.0.1a0/pyproject.toml` & `ardilla-0.0.2a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.0.1-alpha"
+version = "0.0.2-alpha"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "A small package for performing basic CRUD operations with sqlite via aiosqlite and pydantic"
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Development Status :: 3 - Alpha",
 ]
 dependencies = [
   "pydantic==1.10.7",
 ]
 
 [project.optional-dependencies]
 async = ["aiosqlite==0.19.0",]
-
+dev = ["pytest==7.3.1", "pytest-asyncio==0.21.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/chrisdewa/ardilla"
 "Bug Tracker" = "https://github.com/chrisdewa/ardilla/issues"
```

