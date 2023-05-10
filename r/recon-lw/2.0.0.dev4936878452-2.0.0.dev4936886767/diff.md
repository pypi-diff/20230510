# Comparing `tmp/recon_lw-2.0.0.dev4936878452.tar.gz` & `tmp/recon_lw-2.0.0.dev4936886767.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4936878452.tar", last modified: Wed May 10 12:18:04 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4936886767.tar", last modified: Wed May 10 12:19:00 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4936878452.tar` & `recon_lw-2.0.0.dev4936886767.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-10 12:17:44.000000 recon_lw-2.0.0.dev4936878452/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13016 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    21366 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    13987 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:18:04.000000 recon_lw-2.0.0.dev4936878452/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-10 12:17:36.000000 recon_lw-2.0.0.dev4936878452/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-10 12:18:38.000000 recon_lw-2.0.0.dev4936886767/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21366 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13987 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 12:19:00.000000 recon_lw-2.0.0.dev4936886767/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-10 12:18:30.000000 recon_lw-2.0.0.dev4936886767/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev4936878452/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev4936886767/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936878452/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev4936886767/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936878452/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4936886767/recon_lw/recon_lw.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,24 +124,24 @@
             n += 1
     return result
 
 
 # match_compare_func takes m1, m2  returns e
 # end_events_func tekes iterable of events
 def rule_flush(current_ts, horizon_delay, match_index, time_index, message_cache,
-               interpret_func, event_sequence, send_events_func, parent_event):
+               interpret_func, event_sequence, send_events_func, parent_event, live_orders_cache):
     old_keys = flush_old(current_ts, horizon_delay, time_index)
     events = []
     for k in old_keys:
         elem = match_index.pop(k)
         if elem[0] is not None and elem[0] not in message_cache:
             #request already processed through different key
             continue
 
-        results = interpret_func([message_cache_pop(item, message_cache) for item in elem], event_sequence)
+        results = interpret_func([message_cache_pop(item, message_cache) for item in elem],live_orders_cache,event_sequence)
 #       result = interpret_func(message_cache_pop(elem[0], message_cache),
 #                                message_cache_pop(elem[1], message_cache), event_sequence)
         if results is not None:
             for r in results:
                 r["parentEventId"] = parent_event["eventId"]
                 events.append(r)
 
@@ -219,26 +219,29 @@
     rule_settings["time_index"] = SortedKeyList(key=lambda t: time_stamp_key(t[0]))
     rule_settings["message_cache"] = {}
 
 
 def collect_matcher(batch, rule_settings):
     rule_match_func = rule_settings["rule_match_func"]
     rule_match_func(batch, rule_settings)
+    if "live_orders_cache" in rule_settings:
+        rule_settings["live_orders_cache"].process_objects_batch(batch)
 
 
 def flush_matcher(ts,rule_settings,event_sequence, save_events_func):
     rule_flush(ts,
                rule_settings["horizon_delay"],
                rule_settings["match_index"],
                rule_settings["time_index"],
                rule_settings["message_cache"],
                rule_settings["interpret_func"],
                event_sequence,
                save_events_func,
-               rule_settings["rule_root_event"])
+               rule_settings["rule_root_event"],
+               rule_settings["live_orders_cache"] if "live_orders_cache" in rule_settings else None)
 
 
 def simplify_message(m):
     mm = m.copy()
     if len(m["body"]) > 0:
         mm["simpleBody"] = message_utils.message_to_dict(m)  #.message2dict(m)
         mm["protocol"] = protocol(m)
```

### Comparing `recon_lw-2.0.0.dev4936878452/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4936886767/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936878452/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev4936886767/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936878452/setup.py` & `recon_lw-2.0.0.dev4936886767/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4936878452/test/test_recon_ob.py` & `recon_lw-2.0.0.dev4936886767/test/test_recon_ob.py`

 * *Files identical despite different names*

