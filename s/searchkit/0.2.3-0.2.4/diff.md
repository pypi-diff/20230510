# Comparing `tmp/searchkit-0.2.3.tar.gz` & `tmp/searchkit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.3.tar", last modified: Thu Apr 20 14:49:42 2023, max compression
+gzip compressed data, was "searchkit-0.2.4.tar", last modified: Wed May 10 09:52:05 2023, max compression
```

## Comparing `searchkit-0.2.3.tar` & `searchkit-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-20 14:49:42.931016 searchkit-0.2.3/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.3/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-04-20 14:49:42.931016 searchkit-0.2.3/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.3/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-04-17 12:11:23.000000 searchkit-0.2.3/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-20 14:49:42.931016 searchkit-0.2.3/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-04-18 13:47:52.000000 searchkit-0.2.3/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-04-11 08:53:59.000000 searchkit-0.2.3/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.3/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    44374 2023-04-18 16:13:04.000000 searchkit-0.2.3/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4743 2023-04-13 20:08:39.000000 searchkit-0.2.3/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-20 14:49:42.931016 searchkit-0.2.3/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-04-20 14:49:42.000000 searchkit-0.2.3/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-04-20 14:49:42.931016 searchkit-0.2.3/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.3/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-10 09:52:05.554224 searchkit-0.2.4/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.4/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-05-10 09:52:05.554224 searchkit-0.2.4/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.4/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-04-17 12:11:23.000000 searchkit-0.2.4/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-10 09:52:05.554224 searchkit-0.2.4/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-04-18 13:47:52.000000 searchkit-0.2.4/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-05-10 08:57:33.000000 searchkit-0.2.4/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.4/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    49277 2023-05-10 09:51:27.000000 searchkit-0.2.4/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3981 2023-05-10 09:51:27.000000 searchkit-0.2.4/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-10 09:52:05.554224 searchkit-0.2.4/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-10 09:52:05.554224 searchkit-0.2.4/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.4/setup.py
```

### Comparing `searchkit-0.2.3/LICENSE` & `searchkit-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.3/PKG-INFO` & `searchkit-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.3/README.md` & `searchkit-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.3/pyproject.toml` & `searchkit-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.3/searchkit/constraints.py` & `searchkit-0.2.4/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.3/searchkit/search.py` & `searchkit-0.2.4/searchkit/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 from functools import cached_property
 from collections import UserDict, UserList
 
 from searchkit.log import log
 
 RESULTS_QUEUE_TIMEOUT = 60
 MAX_QUEUE_RETRIES = 10
+RS_LOCK = multiprocessing.Lock()
+
+
+def rs_locked(f):
+    def _rs_locked_inner(*args, **kwargs):
+        with RS_LOCK:
+            return f(*args, **kwargs)
+
+    return _rs_locked_inner
 
 
 class FileSearchException(Exception):
     def __init__(self, msg):
         self.msg = msg
 
 
@@ -205,40 +214,104 @@
 
 class SequenceSearchResults(UserDict):
 
     def __init__(self):
         self.data = {}
 
     def add(self, result):
-        id = result.sequence_def.id
+        id = result.sequence_id
         if id in self.data:
             self.data[id].append(result)
         else:
             self.data[id] = [result]
 
     def remove(self, id):
         if id in self.data:
             del self.data[id]
 
 
-class SearchResultPart(object):
+class ResultStoreBase(UserDict):
 
-    def __init__(self, index, value, field_info=None):
-        """
-        @param index: index of this result
-        @param value: value of this result
-        @param field_info: ResultFieldInfo object
-        """
-        self.index = index
-        self.value = value
-        if field_info and value is not None:
-            self.name = field_info.index_to_name(index - 1)
-            self.value = field_info.ensure_type(self.name, value)
-        else:
-            self.name = None
+    def __init__(self):
+        self.head = 0
+        self.index = {}
+        self.meta = {}
+        self.data = {}
+
+    def __getitem__(self, result_id):
+        return self.data.get(result_id)
+
+    def increment_head(self):
+        """ Incrementing differs for proxied vs. raw types so we leave this to
+        implementations to figure out. """
+        self.head += 1
+
+    @property
+    def num_deduped(self):
+        counters = self.meta.values()
+        return sum(counters) - len(counters)
+
+    def add(self, value):
+        _id = self.index.get(value)
+        if _id is not None:
+            self.meta[_id] += 1
+            return _id
+
+        _id = self.head
+        self.data[_id] = value
+        self.meta[_id] = 1
+        self.index[value] = _id
+        self.increment_head()
+        return _id
+
+
+class ResultStoreSimple(ResultStoreBase):
+    """ Store for use when sharing between processes is not needed. """
+
+
+class ResultStoreParallel(ResultStoreBase):
+    """ Store for use when sharing between processes is required. """
+
+    def __init__(self, mgr):
+        self._head = mgr.Value('i', 0)
+        self.meta = mgr.dict()
+        self.index = mgr.dict()
+        self.data = mgr.dict()
+
+    @rs_locked
+    def __getitem__(self, result_id):
+        return super().__getitem__(result_id)
+
+    @property
+    def head(self):
+        return self._head.value
+
+    def increment_head(self):
+        self._head.value = self.head + 1
+
+    @rs_locked
+    def add(self, value):
+        return super().add(value)
+
+    @property
+    @rs_locked
+    def num_deduped(self):
+        return super().num_deduped
+
+    @rs_locked
+    def unproxy_results(self):
+        """
+        Converts internal stores to unproxied types so they can be accessed
+        once their manager is gone.
+        """
+        log.debug("unproxying results store (data=%s)", len(self.data))
+        self._head = self._head.value
+        self.data = self.data.copy()
+        self.meta = self.meta.copy()
+        self.index = self.index.copy()
 
 
 class ResultFieldInfo(UserDict):
 
     def __init__(self, fields):
         """
         @param fields: list or dictionary of field names. If a dictionary is
@@ -267,126 +340,193 @@
             if index == i:
                 return _field
 
         raise FileSearchException("field with index {} not found in mapping".
                                   format(index))
 
 
-class SearchResult(UserList):
+class SearchResultBase(UserList):
+
+    def get(self, field):
+        """
+        Retrieve result part value by index or name.
+
+        @param field: integer index of string field name.
+        """
+        for part in self.data:
+            store_id = None
+            if type(field) == str:
+                if part['name'] == field:
+                    store_id = part['store_id']
+            elif part['idx'] == field:
+                store_id = part['store_id']
+
+            if store_id is not None:
+                return self.results_store.get(store_id)
+
+    def __getattr__(self, name):
+        if name != 'field_info':
+            if self.field_info and name in self.field_info:
+                return self.get(name)
+
+        raise AttributeError("'{}' object has no attribute '{}'".
+                             format(self.__class__.__name__, name))
+
+    def __iter__(self):
+        """ Only return part values when iterating over this object. """
+        for part in self.data:
+            yield self.results_store.get(part['store_id'])
+
+    def __repr__(self):
+        r_list = ["{}='{}'".format(rp['idx'],
+                                   self.results_store.get(rp['store_id']))
+                  for rp in self.data]
+        return ("ln:{} {} (section={})".
+                format(self.linenumber, ", ".join(r_list),
+                       self.section_id))
+
+
+class SearchResultMinimal(SearchResultBase):
+
+    def __init__(self, id, data, linenumber, source_id, tag,
+                 sequence_id, sequence_section_id, field_info):
+        """
+        This is a minimised representation of a SearchResult object so as to
+        reduce its size as much as possible before putting on the results
+        queue.
+        """
+        self.id = id
+        self.data = data
+        self.linenumber = linenumber
+        self.source_id = source_id
+        self.tag = tag
+        self.sequence_id = sequence_id
+        self.section_id = sequence_section_id
+        self.field_info = field_info
+        self.results_store = None
+
+    def register_results_store(self, store):
+        """
+        Register a ResultsStore with this result. This is used to re-register
+        the store once the result has been received by the main process.
+
+        @param store: ResultsStore object
+        """
+        self.results_store = store
+
+
+class SearchResult(SearchResultBase):
 
     def __init__(self, linenumber, source_id, result, search_def,
-                 sequence_section_id=None):
+                 results_store, sequence_section_id=None):
         """
         @param linenumber: line number that produced a match.
         @param source_id: data source id - resolves to a path in the
                           SearchCatalog.
         @param result: python.re.match object.
         @param search_def: SearchDef object.
+        @param results_store: ResultsStore object
         @param sequence_section_id: if this result is part of a sequence the
                                     section ID must be provided.
         """
+        self.results_store = results_store
         self.data = []
         self.linenumber = linenumber
         self.source_id = source_id
         self.tag = search_def.tag
         self.section_id = sequence_section_id
-        self.sequence_def = search_def.sequence_def
-        if self.sequence_def and sequence_section_id is None:
-            raise FileSearchException("sequence section result saved "
-                                      "but no section id provided")
+        self.sequence_id = None
+        if search_def.sequence_def:
+            if sequence_section_id is None:
+                raise FileSearchException("sequence section result saved "
+                                          "but no section id provided")
+
+            self.sequence_id = search_def.sequence_def.id
+
         self.field_info = search_def.field_info
 
         if not search_def.store_result_contents:
             log.debug("store_contents is False - skipping save")
             return
 
+        self.store_result(result)
+
+    def store_result(self, result):
         num_groups = len(result.groups())
         # NOTE: this does not include group(0)
         if num_groups:
             # To reduce memory footprint, don't store group(0) i.e. the whole
             # line, if there are actual groups in the result.
             for i in range(1, num_groups + 1):
-                self._add(i, result.group(i))
+                self._save_part(i, result.group(i))
         else:
             log.debug("saving full search result which can lead to high "
                       "memory usage")
-            self._add(0, result.group(0))
+            self._save_part(0, result.group(0))
 
     @cached_property
     def id(self):
         """ Unique Result ID """
         id_string = "{}-{}-{}".format(uuid.uuid4(), self.source_id,
                                       self.linenumber)
-        if self.sequence_def:
+        if self.sequence_id:
             id_string = "{}-{}-{}".format(id_string,
-                                          self.sequence_def.id,
+                                          self.sequence_id,
                                           self.section_id)
         return id_string
 
-    def _add(self, index, value):
-        self.data.append(SearchResultPart(index, value, self.field_info))
-
-    def get(self, field):
-        """
-        Retrieve result part value by index or name.
-
-        @param field: integer index of string field name.
-        """
-        for group in self.data:
-            if type(field) == str:
-                if group.name == field:
-                    return group.value
-            else:
-                if group.index == field:
-                    return group.value
+    def _save_part(self, part_index, value):
+        name = None
+        if value is not None and self.field_info:
+            name = self.field_info.index_to_name(part_index - 1)
+            value = self.field_info.ensure_type(name, value)
+
+        store_id = self.results_store.add(value)
+        self.data.append({'idx': part_index, 'store_id': store_id,
+                          'name': name})
 
-    def __getattr__(self, name):
-        if name != 'field_info':
-            if self.field_info and name in self.field_info:
-                return self.get(name)
-
-        raise AttributeError("'{}' object has no attribute '{}'".
-                             format(self.__class__.__name__, name))
-
-    def __iter__(self):
-        """ Only return part values when iterating over this object. """
-        for part in self.data:
-            yield part.value
-
-    def __repr__(self):
-        r_list = ["{}='{}'".format(rp.index, rp.value) for rp in self.data]
-        return ("ln:{} {} (section={})".
-                format(self.linenumber, ", ".join(r_list),
-                       self.section_id))
+    @cached_property
+    def export(self):
+        """ Export the smallest possible representation of this object. """
+        return SearchResultMinimal(self.id, self.data, self.linenumber,
+                                   self.source_id, self.tag,
+                                   self.sequence_id, self.section_id,
+                                   self.field_info)
 
 
 class SearchResultsCollection(UserDict):
 
-    def __init__(self, search_catalog):
+    def __init__(self, search_catalog, results_store):
         self.search_catalog = search_catalog
+        self.results_store = results_store
         self.reset()
 
     @property
     def data(self):
         results = {}
         for path, ids in self._results_by_path.items():
             results[path] = [self._results_by_id[id] for id in ids]
 
         return results
 
+    @property
+    def all(self):
+        for r in self._results_by_id.values():
+            yield r
+
     def reset(self):
-        self._iter_idx = 0
         self._results_by_path = {}
         self._results_by_id = {}
 
     @property
     def files(self):
         return list(self._results_by_path.keys())
 
     def add(self, result):
+        result.register_results_store(self.results_store)
         # resolve
         path = self.search_catalog.source_id_to_path(result.source_id)
         self._results_by_id[result.id] = result
         if path not in self._results_by_path:
             self._results_by_path[path] = [result.id]
         else:
             self._results_by_path[path].append(result.id)
@@ -427,15 +567,15 @@
             paths = [path]
         else:
             paths = list(self._results_by_path.keys())
 
         sequences = []
         for path in paths:
             for result in self.find_by_path(path):
-                if result.sequence_def is None:
+                if result.sequence_id is None:
                     continue
 
                 sequences.append(result.id)
 
         return sequences
 
     def find_sequence_by_tag(self, tag, path=None):
@@ -463,15 +603,15 @@
 
         @param sequence_obj: SequenceSearch object
         @param path: optionally filter results for a given path.
         """
         _results = {}
         for r in self._get_all_sequence_results(path=path):
             result = self._results_by_id[r]
-            s_id = result.sequence_def.id
+            s_id = result.sequence_id
             if s_id != sequence_obj.id:
                 continue
 
             section_id = result.section_id
             if section_id not in _results:
                 _results[section_id] = []
 
@@ -650,19 +790,21 @@
                        'source_id': self._get_source_id(path),
                        'searches': [self.resolve_from_id(id)
                                     for id in searches]}
 
 
 class SearchTask(object):
 
-    def __init__(self, info, constraints_manager, results_queue):
+    def __init__(self, info, constraints_manager, results_queue,
+                 results_store):
         self.info = info
         self.stats = SearchTaskStats()
         self.constraints_manager = constraints_manager
         self.results_queue = results_queue
+        self.results_store = results_store
 
     @cached_property
     def id(self):
         return str(uuid.uuid4())
 
     @cached_property
     def search_defs_conditional(self):
@@ -680,17 +822,17 @@
 
     def put_result(self, result):
         self.stats['results'] += 1
         max_tries = MAX_QUEUE_RETRIES
         while max_tries > 0:
             try:
                 if max_tries == MAX_QUEUE_RETRIES:
-                    self.results_queue.put_nowait(result)
+                    self.results_queue.put_nowait(result.export)
                 else:
-                    self.results_queue.put(result,
+                    self.results_queue.put(result.export,
                                            timeout=RESULTS_QUEUE_TIMEOUT)
 
                 break
             except queue.Full:
                 if max_tries == MAX_QUEUE_RETRIES:
                     msg = ("search task queue for '%s' is full - switching "
                            "to using blocking put with timeout")
@@ -715,15 +857,15 @@
         @param ln: current line number
         """
         ret = search_def.run(line)
         if not ret:
             return
 
         self.put_result(SearchResult(ln, self.info['source_id'], ret,
-                                     search_def))
+                                     search_def, self.results_store))
 
     def _sequence_search(self, seq_def, line, ln, sequence_results):
         """ Perform a sequence search on line.
 
         @param seq_def: SequenceSearchDef object
         @param line: current line (string)
         @param ln: current line number
@@ -754,23 +896,24 @@
                 # the next.
                 if seq_def.s_end is None:
                     s_term = seq_def.s_start
                     seq_def.start()
                     section_id = seq_def.current_section_id
 
             sequence_results.add(SearchResult(ln, self.info['source_id'], ret,
-                                              s_term,
+                                              s_term, self.results_store,
                                               sequence_section_id=section_id))
         elif seq_def.started and seq_def.s_body:
             section_id = seq_def.current_section_id
             ret = seq_def.s_body.run(line)
             if ret:
                 sequence_results.add(SearchResult(
                                             ln, self.info['source_id'],
                                             ret, seq_def.s_body,
+                                            self.results_store,
                                             sequence_section_id=section_id))
 
     def _process_sequence_results(self, sequence_results, current_ln):
         """
         Perform post processing to sequence search results.
 
         @param sequence_results: SequenceSearchResults object
@@ -792,15 +935,17 @@
             if seq_def.s_end is None:
                 continue
 
             ret = seq_def.s_end.run('')
             if ret:
                 section_id = seq_def.current_section_id
                 r = SearchResult(current_ln + 1, self.info['source_id'], ret,
-                                 seq_def.s_end, sequence_section_id=section_id)
+                                 seq_def.s_end,
+                                 self.results_store,
+                                 sequence_section_id=section_id)
                 sequence_results.add(r)
             else:
                 if seq_def.id not in filter_section_id:
                     filter_section_id[seq_def.id] = []
 
                 filter_section_id[seq_def.id].append(
                     seq_def.current_section_id)
@@ -811,18 +956,18 @@
 
         log.debug("filtering sections: %s", filter_section_id)
         # Now add sequence results to main results list, excluding any
         # incomplete sections.
         for s_results in sequence_results.values():
             for r in s_results:
                 if filter_section_id:
-                    if r.sequence_def is None:
+                    if r.sequence_id is None:
                         continue
 
-                    seq_id = r.sequence_def.id
+                    seq_id = r.sequence_id
                     if seq_id in filter_section_id:
                         if r.section_id in filter_section_id[seq_id]:
                             continue
 
                 self.put_result(r)
 
     def _run_search(self, fd):
@@ -1167,29 +1312,30 @@
 
             try:
                 log.debug('sending SIGKILL to worker process %s', wpid)
                 os.kill(wpid, signal.SIGILL)
             except Exception:
                 log.debug('worker process %s already killed', wpid)
 
-    def _run_single(self, results):
+    def _run_single(self, results, results_store):
         """ Run a single search using this process.
 
         @param results: SearchResultsCollection object
         """
         queue = multiprocessing.Queue()
         for info in self.catalog:
             task = SearchTask(info,
                               constraints_manager=self.constraints_manager,
-                              results_queue=queue)
+                              results_queue=queue,
+                              results_store=results_store)
             self.stats.update(task.execute())
 
         self._purge_results(results, queue, self.stats['results'])
 
-    def _run_mp(self, mgr, results):
+    def _run_mp(self, mgr, results, results_store):
         """ Run searches in parallel.
 
         @param mgr: multiprocessing.Manager object
         @param results: SearchResultsCollection object
         """
         queue = mgr.Queue()
         results_thread, event = self._create_results_thread(results, queue,
@@ -1200,15 +1346,16 @@
             with concurrent.futures.ProcessPoolExecutor(
                                     max_workers=num_workers) as executor:
                 jobs = {}
                 for info in self.catalog:
                     c_mgr = self.constraints_manager
                     task = SearchTask(info,
                                       constraints_manager=c_mgr,
-                                      results_queue=queue)
+                                      results_queue=queue,
+                                      results_store=results_store)
                     job = executor.submit(task.execute)
                     jobs[job] = info['path']
                     self.stats['total_jobs'] += 1
 
                 log.debug("filesearcher: syncing %s job(s)", len(jobs))
                 results_thread.start()
                 results_thread_started = True
@@ -1239,31 +1386,37 @@
 
                 self._ensure_worker_processes_killed()
                 log.debug("terminating pool")
         finally:
             if results_thread is not None and results_thread_started:
                 self._stop_results_thread(results_thread, event)
 
-        log.debug("filesearcher: stats=%s", self.stats)
-        log.debug("filesearcher: completed (results=%s)", len(results))
-
     def run(self):
         """ Run all searches.
 
         @return: SearchResultsCollection object
         """
         log.debug("filesearcher: starting")
         self.stats.reset()
-        results = SearchResultsCollection(self.catalog)
         if len(self.catalog) == 0:
             log.debug("catalog is empty - nothing to run")
-            return results
+            return SearchResultsCollection(self.catalog, ResultStoreSimple())
 
         if len(self.files) > 1:
             log.debug("running searches (parallel=True)")
             with multiprocessing.Manager() as mgr:
-                self._run_mp(mgr, results)
+                rs = ResultStoreParallel(mgr)
+                results = SearchResultsCollection(self.catalog, rs)
+                self._run_mp(mgr, results, rs)
+                self.stats['num_deduped'] = rs.num_deduped
+                rs.unproxy_results()
         else:
             log.debug("running searches (parallel=False)")
-            self._run_single(results)
+            rs = ResultStoreSimple()
+            results = SearchResultsCollection(self.catalog, rs)
+            self._run_single(results, rs)
+            self.stats['num_deduped'] = rs.num_deduped
 
+        log.debug("filesearcher: stats=%s", self.stats)
+        log.debug("filesearcher: completed (results=%s, dedup=%s)",
+                  len(results), self.stats['num_deduped'])
         return results
```

### Comparing `searchkit-0.2.3/searchkit/utils.py` & `searchkit-0.2.4/searchkit/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import fasteners
 import os
-import pickle
+import shelve
 
 from functools import cached_property
 
 from searchkit.log import log
 
 
 class MPCache(object):
@@ -62,52 +62,49 @@
                 _dir = os.path.dirname(path)
 
             if not os.path.isdir(_dir):
                 os.makedirs(_dir)
 
         return path
 
-    def _get_unsafe(self, path):
+    def _get_unsafe(self, key, path):
         """
         Unlocked get not to be used without having first acquired the lock.
 
         @param path: path to cache contents file.
         """
         if not path or not os.path.exists(path):
             log.debug("no cache found at '%s'", path)
             return
 
-        with open(path, 'rb') as fd:
-            try:
-                contents = pickle.load(fd)
-            except Exception:
-                log.exception("failed to load contents from cache '%s'", path)
-                contents = None
-
-            if not contents:
-                return
-
-            return contents
+        with shelve.open(path) as db:
+            return db.get(key)
 
     def get(self, key):
         """
         Get value for key
 
         @param key: key to lookup in cache.
         @return: value or None.
         """
         path = self._cache_path
         with self._cache_lock:
             log.debug("load from cache '%s' (key='%s')", path, key)
             if self.file_per_key:
-                return self._get_unsafe(os.path.join(path, key))
+                return self._get_unsafe('0', os.path.join(path, key))
+
+            return self._get_unsafe(key, path)
 
-            contents = self._get_unsafe(path)
-            if contents:
-                return contents.get(key)
+    def _set_unsafe(self, path, key, value):
+        if self.file_per_key:
+            path = os.path.join(path, key)
+            key = '0'
+
+        with shelve.open(path) as db:
+            db[key] = value
 
     def set(self, key, value):
         """
         Set value for key.
 
         Cache contents are update as read-modify-write of entire contents.
 
@@ -116,30 +113,12 @@
         """
         path = self._cache_path
         if not path:
             log.warning("invalid path '%s' - cannot save to cache", path)
             return
 
         with self._cache_lock:
-            if self.file_per_key:
-                path = os.path.join(path, key)
-                log.debug("saving to cache '%s' (key=%s)", path, key)
-                contents = value
-            else:
-                contents = self._get_unsafe(path)
-                if contents:
-                    contents[key] = value
-                else:
-                    contents = {key: value}
-
-                log.debug("saving to cache '%s' (key=%s, items=%s)", path, key,
-                          len(contents))
-
-            with open(path, 'wb') as fd:
-                try:
-                    pickle.dump(contents, fd)
-                except Exception:
-                    log.exception("failed to save contents to cache '%s'",
-                                  path)
+            log.debug("saving to cache '%s' (key=%s)", path, key)
+            self._set_unsafe(path, key, value)
 
-            log.debug("cache id=%s size=%s", self.cache_id,
-                      os.path.getsize(path))
+        log.debug("cache id=%s size=%s", self.cache_id,
+                  os.path.getsize(path))
```

### Comparing `searchkit-0.2.3/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.4/searchkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

