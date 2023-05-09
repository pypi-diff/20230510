# Comparing `tmp/formic_opcua-1.3.3.tar.gz` & `tmp/formic_opcua-1.3.4.tar.gz`

## Comparing `formic_opcua-1.3.3.tar` & `formic_opcua-1.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/examples/opcua_client.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/examples/example_configs/opcua_config.yaml
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/examples/example_configs/opcua_config_1.yaml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/examples/example_configs/opcua_config_2.yaml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/examples/example_configs/opcua_config_3.yaml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/examples/example_configs/opcua_config_4.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/examples/example_configs/opcua_config_5.yaml
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/client/__init__.py
--rw-r--r--   0        0        0    11780 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/client/async_opcua_client.py
--rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/client/opcua_client.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/core/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/core/exceptions.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/core/parse.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/core/type_conversions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/scripts/__init__.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/scripts/formic_opcua_client.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/scripts/formic_opcua_server.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/server/__init__.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/formic_opcua/server/opcua_server.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/hooks/add_issue_prefix.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/tests/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/tests/test_server_config.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/examples/opcua_client.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/examples/example_configs/opcua_config.yaml
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/examples/example_configs/opcua_config_1.yaml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/examples/example_configs/opcua_config_2.yaml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/examples/example_configs/opcua_config_3.yaml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/examples/example_configs/opcua_config_4.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/examples/example_configs/opcua_config_5.yaml
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/client/__init__.py
+-rw-r--r--   0        0        0    11780 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/client/async_opcua_client.py
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/client/opcua_client.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/core/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/core/exceptions.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/core/parse.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/core/type_conversions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/scripts/__init__.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/scripts/formic_opcua_client.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/scripts/formic_opcua_server.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/server/__init__.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/formic_opcua/server/opcua_server.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/hooks/add_issue_prefix.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/tests/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/tests/test_server_config.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 formic_opcua-1.3.4/PKG-INFO
```

### Comparing `formic_opcua-1.3.3/.pre-commit-config.yaml` & `formic_opcua-1.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/examples/opcua_client.py` & `formic_opcua-1.3.4/examples/opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/examples/example_configs/opcua_config.yaml` & `formic_opcua-1.3.4/examples/example_configs/opcua_config.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/examples/example_configs/opcua_config_1.yaml` & `formic_opcua-1.3.4/examples/example_configs/opcua_config_1.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/examples/example_configs/opcua_config_2.yaml` & `formic_opcua-1.3.4/examples/example_configs/opcua_config_2.yaml`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/formic_opcua/client/async_opcua_client.py` & `formic_opcua-1.3.4/formic_opcua/client/async_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/formic_opcua/client/opcua_client.py` & `formic_opcua-1.3.4/formic_opcua/client/opcua_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,56 +166,56 @@
             return True
         else:
             logger.warning('Write attempt failed')
             self._has_connected = False
 
         return False
 
-    def _read_helper(self, path: str) -> Any:
+    def _read_helper(self, path: str, return_datavalue: bool = False) -> Any:
         if self._has_connected:
             try:
                 node = self._node_map[path][0]
             except (KeyError, IndexError):
                 logger.warning(f'Unable to get node {path} from client map {self._node_map}')
                 return None
             try:
-                value = node.read_value()
+                value = node.read_value() if not return_datavalue else node.read_data_value()
                 logger.info(f'Read value {value} from path {path}')
                 return value
             except (ConnectionError, ThreadLoopNotRunning) as e:
                 logger.warning(f'{e}')
                 logger.warning(f'Unable to read node at {path}')
         else:
             logger.warning(f'No connection has been made to server. Cannot read node at path {path}')
         return None
 
-    def read(self, path: str) -> Any:
+    def read(self, path: str, return_datavalue: bool = False) -> Any:
         logger.info(f'Attempting to read path {path}.')
         if not self._has_connected:  # Read attempt has failed or client never connected.
             logger.info('Client has not connected to server. Attempting to connect.')
             self.__enter__()
-        value = self._read_helper(path=path)
+        value = self._read_helper(path=path, return_datavalue=return_datavalue)
         if value is not None:
             logger.info('Read attempt succeeded')
             logger.info(f'Value: {value}')
             return value
         else:
             logger.warning('Read attempt failed')
             self._has_connected = False
         return None
 
-    def read_all(self) -> Dict[str, Any]:
+    def read_all(self, return_datavalue: bool = False) -> Dict[str, Any]:
         logger.info(f'Attempting to read all variables on server at uri: {self._uri} and url: {self._url}.')
         results = {}
         if not self._has_connected:  # Client has never successfully connected to the server
             logger.info('Client may not be connected to server. Attempting to connect.')
             self.__enter__()  # Creates a new client object and adjusts self._has_connected() appropriately
         if self._has_connected:  # In case self.__enter__() changed value to true by establishing a connection
             for path in self._node_path_list:
-                value = self._read_helper(path)
+                value = self._read_helper(path, return_datavalue=return_datavalue)
                 if value is not None:
                     logger.info(f'Successfully read value: {value} for path: {path}')
                     results[path] = value
                 else:
                     # This could happens if there is a disconnect during reading
                     logger.warning(f'Unsuccessful read attempt for path {path}')
                     self._has_connected = False
```

### Comparing `formic_opcua-1.3.3/formic_opcua/core/parse.py` & `formic_opcua-1.3.4/formic_opcua/core/parse.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/formic_opcua/core/type_conversions.py` & `formic_opcua-1.3.4/formic_opcua/core/type_conversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def positive_sha256_hash(obj):
     sha256_hash = hashlib.sha256()
     sha256_hash.update(str(obj).encode('utf-8'))
-    return int(sha256_hash.hexdigest()[:8], 16)  # Make sure there are not too many bytes for UInt32
+    return int(sha256_hash.hexdigest()[:6], 16)  # Make sure there are not too many bytes for UInt32
 
 
 type_map = {
     VariantType.SByte: int,
     VariantType.Byte: int,
     VariantType.ByteString: bytes,
     VariantType.Int32: int,
```

### Comparing `formic_opcua-1.3.3/formic_opcua/scripts/formic_opcua_client.py` & `formic_opcua-1.3.4/formic_opcua/scripts/formic_opcua_client.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/formic_opcua/scripts/formic_opcua_server.py` & `formic_opcua-1.3.4/formic_opcua/scripts/formic_opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/formic_opcua/server/opcua_server.py` & `formic_opcua-1.3.4/formic_opcua/server/opcua_server.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/hooks/add_issue_prefix.py` & `formic_opcua-1.3.4/hooks/add_issue_prefix.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/tests/test_server_config.py` & `formic_opcua-1.3.4/tests/test_server_config.py`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/.gitignore` & `formic_opcua-1.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `formic_opcua-1.3.3/pyproject.toml` & `formic_opcua-1.3.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
 
 [project]
 name = 'formic_opcua'
 requires-python = ">=3.8"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
     {name = "Spencer White", email = "swhite@formic.co"},
     {name = "Damian Stempel"},
     {name = "Viachaslau Zakharchuk"}
 
 ]
 dependencies = [
```

