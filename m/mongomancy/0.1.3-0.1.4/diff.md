# Comparing `tmp/mongomancy-0.1.3.tar.gz` & `tmp/mongomancy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomancy-0.1.3.tar", last modified: Tue May  9 14:23:46 2023, max compression
+gzip compressed data, was "mongomancy-0.1.4.tar", last modified: Tue May  9 14:59:17 2023, max compression
```

## Comparing `mongomancy-0.1.3.tar` & `mongomancy-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 14:23:46.455578 mongomancy-0.1.3/
--rw-r--r--   0 trval     (1000) trval     (1000)     1572 2023-05-09 14:22:36.000000 mongomancy-0.1.3/CHANGELOG.md
--rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.3/LICENSE
--rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.3/MANIFEST.in
--rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 14:23:46.455578 mongomancy-0.1.3/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.1.3/README.md
--rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.3/pyproject.toml
--rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.3/requirements.txt
--rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-09 14:23:46.455578 mongomancy-0.1.3/setup.cfg
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 14:23:46.452244 mongomancy-0.1.3/src/
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 14:23:46.452244 mongomancy-0.1.3/src/mongomancy/
--rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-09 14:23:28.000000 mongomancy-0.1.3/src/mongomancy/__init__.py
--rw-r--r--   0 trval     (1000) trval     (1000)    13920 2023-05-09 13:03:25.000000 mongomancy-0.1.3/src/mongomancy/engine.py
--rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.3/src/mongomancy/mongo_errors.py
--rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.3/src/mongomancy/py.typed
--rw-r--r--   0 trval     (1000) trval     (1000)    15269 2023-05-09 14:19:12.000000 mongomancy-0.1.3/src/mongomancy/schema.py
--rw-r--r--   0 trval     (1000) trval     (1000)     5944 2023-05-09 13:03:25.000000 mongomancy-0.1.3/src/mongomancy/types.py
-drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 14:23:46.455578 mongomancy-0.1.3/src/mongomancy.egg-info/
--rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 14:23:46.000000 mongomancy-0.1.3/src/mongomancy.egg-info/PKG-INFO
--rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-09 14:23:46.000000 mongomancy-0.1.3/src/mongomancy.egg-info/SOURCES.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-09 14:23:46.000000 mongomancy-0.1.3/src/mongomancy.egg-info/dependency_links.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-09 14:23:46.000000 mongomancy-0.1.3/src/mongomancy.egg-info/requires.txt
--rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-09 14:23:46.000000 mongomancy-0.1.3/src/mongomancy.egg-info/top_level.txt
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 14:59:17.593975 mongomancy-0.1.4/
+-rw-r--r--   0 trval     (1000) trval     (1000)     1672 2023-05-09 14:58:54.000000 mongomancy-0.1.4/CHANGELOG.md
+-rw-rw-r--   0 trval     (1000) trval     (1000)     1329 2022-09-02 09:33:19.000000 mongomancy-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1516 2023-04-04 08:06:59.000000 mongomancy-0.1.4/LICENSE
+-rw-r--r--   0 trval     (1000) trval     (1000)       42 2023-04-12 12:30:41.000000 mongomancy-0.1.4/MANIFEST.in
+-rw-r--r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 14:59:17.593975 mongomancy-0.1.4/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)     3677 2022-09-06 10:07:16.000000 mongomancy-0.1.4/README.md
+-rw-r--r--   0 trval     (1000) trval     (1000)     1368 2023-04-12 12:30:41.000000 mongomancy-0.1.4/pyproject.toml
+-rw-rw-r--   0 trval     (1000) trval     (1000)       68 2022-09-02 09:38:35.000000 mongomancy-0.1.4/requirements.txt
+-rw-r--r--   0 trval     (1000) trval     (1000)       38 2023-05-09 14:59:17.593975 mongomancy-0.1.4/setup.cfg
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 14:59:17.590642 mongomancy-0.1.4/src/
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 14:59:17.590642 mongomancy-0.1.4/src/mongomancy/
+-rw-r--r--   0 trval     (1000) trval     (1000)      431 2023-05-09 14:58:54.000000 mongomancy-0.1.4/src/mongomancy/__init__.py
+-rw-r--r--   0 trval     (1000) trval     (1000)    14133 2023-05-09 14:58:54.000000 mongomancy-0.1.4/src/mongomancy/engine.py
+-rw-rw-r--   0 trval     (1000) trval     (1000)      924 2022-08-29 12:44:42.000000 mongomancy-0.1.4/src/mongomancy/mongo_errors.py
+-rw-r--r--   0 trval     (1000) trval     (1000)        0 2023-04-12 12:30:41.000000 mongomancy-0.1.4/src/mongomancy/py.typed
+-rw-r--r--   0 trval     (1000) trval     (1000)    15269 2023-05-09 14:58:54.000000 mongomancy-0.1.4/src/mongomancy/schema.py
+-rw-r--r--   0 trval     (1000) trval     (1000)     5944 2023-05-09 13:03:25.000000 mongomancy-0.1.4/src/mongomancy/types.py
+drwxr-xr-x   0 trval     (1000) trval     (1000)        0 2023-05-09 14:59:17.593975 mongomancy-0.1.4/src/mongomancy.egg-info/
+-rw-rw-r--   0 trval     (1000) trval     (1000)     4468 2023-05-09 14:59:17.000000 mongomancy-0.1.4/src/mongomancy.egg-info/PKG-INFO
+-rw-rw-r--   0 trval     (1000) trval     (1000)      435 2023-05-09 14:59:17.000000 mongomancy-0.1.4/src/mongomancy.egg-info/SOURCES.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)        1 2023-05-09 14:59:17.000000 mongomancy-0.1.4/src/mongomancy.egg-info/dependency_links.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       13 2023-05-09 14:59:17.000000 mongomancy-0.1.4/src/mongomancy.egg-info/requires.txt
+-rw-rw-r--   0 trval     (1000) trval     (1000)       11 2023-05-09 14:59:17.000000 mongomancy-0.1.4/src/mongomancy.egg-info/top_level.txt
```

### Comparing `mongomancy-0.1.3/CHANGELOG.md` & `mongomancy-0.1.4/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.4] - 2023-05-09
+
+### Fixed
+
+- tracing if engine dispose to prevent closed connection error
+
 ## [0.1.3] - 2023-05-09
 
 ### Fixed
 
 - ignore double init on collection
 
 ## [0.1.2] - 2023-05-09
```

### Comparing `mongomancy-0.1.3/CONTRIBUTING.md` & `mongomancy-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.3/LICENSE` & `mongomancy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.3/PKG-INFO` & `mongomancy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `mongomancy-0.1.3/README.md` & `mongomancy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.3/pyproject.toml` & `mongomancy-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.3/src/mongomancy/engine.py` & `mongomancy-0.1.4/src/mongomancy/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 
 class Engine(types.Executor):
     """
     Client of Mongo Database storage. All DB communication should be handled through this class.
     """
 
-    CONNECTION_ERRORS: ClassVar[Type[pymongo.errors.PyMongoError]] = (
+    CONNECTION_ERRORS: ClassVar[Type[pymongo.errors.PyMongoError]] = [
         pymongo.errors.AutoReconnect,
         pymongo.errors.ConnectionFailure,
-    )
-
+    ]
+    disposed: bool
     client: pymongo.MongoClient
     logger: LoggerType
     retry_codes: Set[int]
     write_retry: int
     write_retry_delay: Union[float, int]
     read_retry: int
     read_retry_delay: Union[float, int]
@@ -53,14 +53,15 @@
         "read_retry_delay",
         "retry_codes",
         "_address",
         "_connection_params",
         "reconnect_hooks",
         "mp_semaphore",
         "th_semaphore",
+        "disposed",
     )
 
     def __init__(
         self,
         host: str = "localhost",
         port: int = 27017,
         max_pool_size: int = 1,
@@ -92,14 +93,15 @@
         :param password: password of used user
         :param connect_timeout: [ms]Controls how long the mongo_driver will wait during server monitoring when connecting a
             new socket to a server before concluding the server is unavailable. `0` or `None` means no timeout.
         :param kwargs: other named parameters for db
         :exception pymongo.errors.PyMongoError: if database connection could not be established
         """
         super(Engine, self).__init__()
+        self.disposed = True
         self.reconnect_hooks = []
         self._address = f"{host}:{port}"
         self.logger = logger or logging.getLogger(type(self).__qualname__)
         self.retry_codes = set(retry_codes or mongo_errors.DEFAULT_RETRY)
         # how many times to retry write on error 10107 (switched master)
         self.write_retry = max(0, write_retry or 0)
         # how much time to sleep between retry write on error 10107 (switched master)
@@ -119,14 +121,15 @@
             maxPoolSize=max_pool_size,
             waitQueueTimeoutMS=queue_timeout,
             connectTimeoutMS=connect_timeout,
             **authentication,
             **kwargs,
         )
         self.client = self._new_client()
+        self.disposed = False
         atexit.register(self.dispose)
 
     def __repr__(self) -> str:
         return f"{type(self).__qualname__}(server={self.address!r})"
 
     def __str__(self) -> str:
         return f"{type(self).__name__}(server={self.address!r})"
@@ -165,14 +168,15 @@
 
     def dispose(self) -> None:
         """
         Cleanup client resources and disconnect from MongoDB.
         """
         try:
             self.client.close()
+            self.disposed = True
         except PyMongoError as e:
             self.logger.debug(f"Cannot close mongo client because: {e}")
         self.logger.debug(f"{self} - disconnect from MongoDB")
 
     def ping(self, database: Optional[str] = None) -> bool:
         """
         Is database server reachable?
@@ -198,14 +202,15 @@
         return bool(is_ok)
 
     def reconnect(self):
         """Close existing MongoClient and create new one"""
         self.logger.debug(f"{type(self).__qualname__} - reconnecting client")
         try:
             self.client = self._new_client()
+            self.disposed = False
         except (IOError, pymongo.errors.PyMongoError) as e:
             self.logger.error(f"{type(self).__qualname__} - cannot reconnect to mongo server because: {e}")
         for hook in self.reconnect_hooks:
             _ = hook(self)
         self.logger.info(f"{type(self).__qualname__} - reconnected client")
 
     def _retry_command(
@@ -223,23 +228,25 @@
         :param collection: collection of method used; f.e.: `game` in `game.find_one`
         :param command: method to execute; f.e.: `game.find_one`
         :param args: arguments for command
         :param command_name_: use this as command name for logging
         :param kwargs: key word arguments for command
         :return: return same as command returns
         """
+        if self.disposed:
+            self.reconnect()
         result = None
         _error = False
         attempt = 0
         while attempt <= self.write_retry and _error is not None:
             attempt += 1
             try:
                 result = command(*args, **kwargs)
                 _error = None
-            except pymongo.errors.AutoReconnect as e:
+            except self.CONNECTION_ERRORS as e:
                 command_name_ = command_name_ or getattr(command, "__qualname__", "<unknown_command>")
                 self.logger.info(
                     f"fail {attempt}/{self.write_retry} - {command_name_} " f"args={args}, kwargs={kwargs} e={e}"
                 )
                 _error = e
                 time.sleep(self.write_retry_delay)
                 self.reconnect()
```

### Comparing `mongomancy-0.1.3/src/mongomancy/mongo_errors.py` & `mongomancy-0.1.4/src/mongomancy/mongo_errors.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.3/src/mongomancy/schema.py` & `mongomancy-0.1.4/src/mongomancy/schema.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.3/src/mongomancy/types.py` & `mongomancy-0.1.4/src/mongomancy/types.py`

 * *Files identical despite different names*

### Comparing `mongomancy-0.1.3/src/mongomancy.egg-info/PKG-INFO` & `mongomancy-0.1.4/src/mongomancy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomancy
-Version: 0.1.3
+Version: 0.1.4
 Summary: Pymongo based python client with data definition layer.
 Author-email: Tom Trval <thandeus@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Ryu-CZ/mongomancy
 Project-URL: Bug Tracker, https://github.com/Ryu-CZ/mongomancy/issues
 Keywords: mongo,python,pymongo,database,nosql
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

