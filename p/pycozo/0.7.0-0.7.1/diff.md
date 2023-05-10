# Comparing `tmp/pycozo-0.7.0.tar.gz` & `tmp/pycozo-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycozo-0.7.0.tar", last modified: Tue May  2 15:48:58 2023, max compression
+gzip compressed data, was "pycozo-0.7.1.tar", last modified: Wed May 10 07:48:33 2023, max compression
```

## Comparing `pycozo-0.7.0.tar` & `pycozo-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-02 15:48:58.860654 pycozo-0.7.0/
--rw-r--r--   0 zh217      (501) staff       (20)    16724 2022-11-30 04:19:19.000000 pycozo-0.7.0/LICENSE.txt
--rw-r--r--   0 zh217      (501) staff       (20)      469 2023-05-02 15:48:58.860538 pycozo-0.7.0/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)     7974 2023-01-21 11:49:23.000000 pycozo-0.7.0/README.md
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-02 15:48:58.859782 pycozo-0.7.0/pycozo/
--rw-r--r--   0 zh217      (501) staff       (20)      284 2022-11-30 04:32:35.000000 pycozo-0.7.0/pycozo/__init__.py
--rw-r--r--   0 zh217      (501) staff       (20)     9665 2023-01-21 11:49:23.000000 pycozo-0.7.0/pycozo/client.py
--rw-r--r--   0 zh217      (501) staff       (20)     4619 2022-12-28 04:03:29.000000 pycozo-0.7.0/pycozo/ext_impl.py
--rw-r--r--   0 zh217      (501) staff       (20)      378 2022-11-30 04:32:35.000000 pycozo-0.7.0/pycozo/ipyext.py
--rw-r--r--   0 zh217      (501) staff       (20)      677 2022-11-30 04:32:35.000000 pycozo-0.7.0/pycozo/ipyext_direct.py
--rw-r--r--   0 zh217      (501) staff       (20)     2046 2023-01-21 11:49:23.000000 pycozo-0.7.0/pycozo/test_client.py
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-02 15:48:58.860372 pycozo-0.7.0/pycozo.egg-info/
--rw-r--r--   0 zh217      (501) staff       (20)      469 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)      297 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/SOURCES.txt
--rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/dependency_links.txt
--rw-r--r--   0 zh217      (501) staff       (20)       77 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/requires.txt
--rw-r--r--   0 zh217      (501) staff       (20)        7 2023-05-02 15:48:58.000000 pycozo-0.7.0/pycozo.egg-info/top_level.txt
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-02 15:48:58.860695 pycozo-0.7.0/setup.cfg
--rw-r--r--   0 zh217      (501) staff       (20)      920 2023-05-02 15:29:42.000000 pycozo-0.7.0/setup.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-10 07:48:33.908328 pycozo-0.7.1/
+-rw-r--r--   0 zh217      (501) staff       (20)    16724 2022-11-30 04:19:19.000000 pycozo-0.7.1/LICENSE.txt
+-rw-r--r--   0 zh217      (501) staff       (20)      469 2023-05-10 07:48:33.908214 pycozo-0.7.1/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)     8781 2023-05-08 07:24:36.000000 pycozo-0.7.1/README.md
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-10 07:48:33.907387 pycozo-0.7.1/pycozo/
+-rw-r--r--   0 zh217      (501) staff       (20)      284 2022-11-30 04:32:35.000000 pycozo-0.7.1/pycozo/__init__.py
+-rw-r--r--   0 zh217      (501) staff       (20)     6676 2023-05-08 10:26:40.000000 pycozo-0.7.1/pycozo/builder.py
+-rw-r--r--   0 zh217      (501) staff       (20)    13343 2023-05-08 07:55:16.000000 pycozo-0.7.1/pycozo/client.py
+-rw-r--r--   0 zh217      (501) staff       (20)     4619 2022-12-28 04:03:29.000000 pycozo-0.7.1/pycozo/ext_impl.py
+-rw-r--r--   0 zh217      (501) staff       (20)      378 2022-11-30 04:32:35.000000 pycozo-0.7.1/pycozo/ipyext.py
+-rw-r--r--   0 zh217      (501) staff       (20)      677 2022-11-30 04:32:35.000000 pycozo-0.7.1/pycozo/ipyext_direct.py
+-rw-r--r--   0 zh217      (501) staff       (20)     2363 2023-05-08 05:14:33.000000 pycozo-0.7.1/pycozo/test_builder.py
+-rw-r--r--   0 zh217      (501) staff       (20)     2046 2023-01-21 11:49:23.000000 pycozo-0.7.1/pycozo/test_client.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-10 07:48:33.908049 pycozo-0.7.1/pycozo.egg-info/
+-rw-r--r--   0 zh217      (501) staff       (20)      469 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)      338 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/SOURCES.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/dependency_links.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       77 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/requires.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        7 2023-05-10 07:48:33.000000 pycozo-0.7.1/pycozo.egg-info/top_level.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-10 07:48:33.908367 pycozo-0.7.1/setup.cfg
+-rw-r--r--   0 zh217      (501) staff       (20)      920 2023-05-10 07:14:53.000000 pycozo-0.7.1/setup.py
```

### Comparing `pycozo-0.7.0/LICENSE.txt` & `pycozo-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.0/README.md` & `pycozo-0.7.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PyCozo
 
 [![pypi](https://img.shields.io/pypi/v/pycozo)](https://pypi.org/project/pycozo/)
 
 Python client and Jupyter helper for [CozoDB](https://www.cozodb.org).
 
-This document describes how to set up Cozo in Python.
+This document describes how to set up CozoDB in Python.
 To learn how to use CozoDB (CozoScript), read the [docs](https://docs.cozodb.org/en/latest/index.html).
 
 ## Install
 
 ```bash
 pip install "pycozo[embedded,requests,pandas]"
 ```
@@ -39,14 +39,18 @@
 
 ```python
 client = Client('sqlite', 'file.db')
 ```
 
 RocksDB-backed (highly concurrent persistent storage):
 
+```python
+client = Client('rocksdb', 'file.db')
+```
+
 Connecting to a standalone server:
 
 ```python
 client = Client('http', options={'host': 'http://127.0.0.1:9070'})
 ```
 
 If the address is not a loopback address, you also need to provide the auth string:
@@ -101,38 +105,52 @@
 In the embedded mode, `Client` will release the [GIL](https://wiki.python.org/moin/GlobalInterpreterLock)
 when executing queries so that multiple queries in different threads can proceed concurrently.
 
 The embedded database exchanges data with the Python runtime directly, without going through JSON.
 Hence you can pass Python bytes directly in named parameters, and bytes returned by the
 database does not need any decoding.
 
+#### Convenience methods
+
+`Client` has convenience methods for common operations:
+
+```python
+client.put('test_rel', {'a': 1, 'b': 2, 'c': 3})
+client.put('test_rel', [{'a': 3, 'b': 4, 'c': 2}, {'a': 5, 'b': 6, 'c': 7}])
+client.put('test_rel', pandas.DataFrame({'a': [7, 8, 9], 'b': [9, 10, 11], 'c': [12, 13, 14]}))
+# for update, only specify the keys and the values you want to update
+client.update('test_rel', {'a': 7, 'b': 8})
+# for rm, only the keys are needed
+client.rm('test_rel', [{'a': 9}, {'a': 11}])
+```
+
 ### Other operations
 
 `Client` has other methods on it: `export_relations`, `import_relations`, `backup`,
 `restore` and `import_from_backup`. See the [doc](https://docs.cozodb.org/en/latest/nonscript.html) for more details.
 
 ### Multi-statement transaction
 
-You can intersperse Cozo statements within a single transaction with
+You can intersperse CozoDB statements within a single transaction with
 Python computations by using a multi-statement transaction.
 
 ```python
-tx = client.multi_transact(True) # Pass False or nothing for read-only transaction
+tx = client.multi_transact(True)  # Pass False or nothing for read-only transaction
 
 tx.run(':create a {a}')
 tx.run('?[a] <- [[1]] :put a {a}')
 try:
     tx.run(':create a {a}')
 except:
     pass
 
 tx.run('?[a] <- [[2]] :put a {a}')
 tx.run('?[a] <- [[3]] :put a {a}')
-tx.commit() # `tx.abort()` abandons the changes so far 
-            # and deletes resources associated with the transaction.
+tx.commit()  # `tx.abort()` abandons the changes so far 
+# and deletes resources associated with the transaction.
 
 r = client.run('?[a] := *a[a]')
 assert r['rows'] == [[1], [2], [3]]
 ```
 
 You **must** run either `tx.commit()` or `tx.abort()` at the end, otherwise
 you will have a resource leak.
@@ -146,39 +164,41 @@
 def cb(op_name, new_rows, old_rows):
     # op_name is 'Put' or 'Rm'
     # new_rows is a list of lists containing the new rows (i.e., requested puts or deletes)
     # old_rows is a list of lists containing the changed rows (i.e., the old rows in the case of puts, 
     # or the rows actually deleted in the case of deletes)
     pass
 
+
 # this registers the callback to run when the stored relation `test_rel` changes
 cb_id = client.register_callback('test_rel', cb)
 
 # your application logic here
 
 # use the returned id for unregistration
 # client.unregister_callback(cb_id)
 ```
 
 ### User-defined fixed rules
 
-You can define your own fixed rules in Python to be used inside Cozo queries. As an example:
+You can define your own fixed rules in Python to be used inside CozoDB queries. As an example:
 
 ```python
 # custom rule implementation, must accept two arguments
 def rule_impl(inputs, options):
     # inputs is a list of lists of lists, representing the input relations to the rule
     # option is a dict with string keys, representing the options passed in when the rule is called
-    
+
     # You should return a list of tuples (or lists) to represent the return relation of the rule.
     # Here the returned relation has arity one.
     # If you cannot perform the computation due to any reason (wrong parameters, etc.),
     # simply raise an exception.
     return [('Nicely',), ('Done!',)]
 
+
 # Actually registering the rule, the second argument is the arity, must match the actual arity
 # of the relation returned by the implementation.
 client.register_fixed_rule('Custom', 1, rule_impl)
 
 r = client.run("""
     rel[u, v, w] <- [[1,2,3],[4,5,6]]
     ?[] <~ Custom(rel[], x: 1, y: null)
@@ -241,11 +261,17 @@
 * `%cozo_set <KEY> <VALUE>` sets a parameter with the name `<KEY>` to the expression `<VALUE>`. The updated parameters will
   be used by subsequent queries.
 * `%cozo_set_params <PARAM_MAP>` replace all parameters by the given expression, which must evaluate to a dictionary
   with string keys.
 * `%cozo_clear` clears all set parameters.
 * `%cozo_params` returns the parameters currently set.
 
+## Programmatically constructing queries
+
+You can use builders in `pycozo.builder` to construct queries programmatically.
+This is both safer and more convenient than concatenating strings.
+See [here](./pycozo/test_builder.py) for how to use it.
+
 ## Building
 
 This library is pure Python, but the `embedded` option depends on
 `cozo-embedded` native package described [here](https://github.com/cozodb/cozo/tree/main/cozo-lib-python).
```

### Comparing `pycozo-0.7.0/pycozo/ext_impl.py` & `pycozo-0.7.1/pycozo/ext_impl.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.0/pycozo/ipyext_direct.py` & `pycozo-0.7.1/pycozo/ipyext_direct.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.0/pycozo/test_client.py` & `pycozo-0.7.1/pycozo/test_client.py`

 * *Files identical despite different names*

### Comparing `pycozo-0.7.0/setup.py` & `pycozo-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #  This Source Code Form is subject to the terms of the Mozilla Public License, v. 2.0.
 #  If a copy of the MPL was not distributed with this file,
 #  You can obtain one at https://mozilla.org/MPL/2.0/.
 
 from setuptools import setup
 
-VERSION = '0.7.0'
+VERSION = '0.7.1'
 
 setup(
     name='pycozo',
     version=VERSION,
     packages=['pycozo'],
     url='',
     license='MPL-2.0',
```

