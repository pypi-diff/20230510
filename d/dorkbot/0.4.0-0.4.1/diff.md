# Comparing `tmp/dorkbot-0.4.0.tar.gz` & `tmp/dorkbot-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorkbot-0.4.0.tar", last modified: Wed May 10 00:12:43 2023, max compression
+gzip compressed data, was "dorkbot-0.4.1.tar", last modified: Wed May 10 01:00:13 2023, max compression
```

## Comparing `dorkbot-0.4.0.tar` & `dorkbot-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.852147 dorkbot-0.4.0/
--rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.4.0/LICENSE
--rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.4.0/MANIFEST.in
--rw-r--r--   0 jgor       (501) staff       (20)    11006 2023-05-10 00:12:43.852231 dorkbot-0.4.0/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)    10604 2023-05-09 23:21:26.000000 dorkbot-0.4.0/README.md
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.797481 dorkbot-0.4.0/dorkbot/
--rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.4.0/dorkbot/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)       22 2023-05-10 00:12:10.000000 dorkbot-0.4.0/dorkbot/_version.py
--rwxr-xr-x   0 jgor       (501) staff       (20)    32189 2023-05-09 22:36:28.000000 dorkbot-0.4.0/dorkbot/dorkbot.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.839483 dorkbot-0.4.0/dorkbot/indexers/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.0/dorkbot/indexers/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     1870 2023-05-09 22:35:43.000000 dorkbot-0.4.0/dorkbot/indexers/bing_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     6022 2023-05-09 19:41:07.000000 dorkbot-0.4.0/dorkbot/indexers/commoncrawl.py
--rw-r--r--   0 jgor       (501) staff       (20)      479 2023-05-09 19:40:01.000000 dorkbot-0.4.0/dorkbot/indexers/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-27 19:42:53.000000 dorkbot-0.4.0/dorkbot/indexers/google.js
--rw-r--r--   0 jgor       (501) staff       (20)     2221 2023-05-09 19:40:36.000000 dorkbot-0.4.0/dorkbot/indexers/google.py
--rw-r--r--   0 jgor       (501) staff       (20)     3008 2023-05-09 19:40:46.000000 dorkbot-0.4.0/dorkbot/indexers/google_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     6279 2023-05-09 19:41:26.000000 dorkbot-0.4.0/dorkbot/indexers/pywb.py
--rw-r--r--   0 jgor       (501) staff       (20)      562 2023-05-09 19:40:11.000000 dorkbot-0.4.0/dorkbot/indexers/stdin.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     4674 2023-05-09 21:01:22.000000 dorkbot-0.4.0/dorkbot/indexers/wayback.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.851677 dorkbot-0.4.0/dorkbot/scanners/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.0/dorkbot/scanners/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     3397 2023-05-09 21:38:35.000000 dorkbot-0.4.0/dorkbot/scanners/arachni.py
--rw-r--r--   0 jgor       (501) staff       (20)      913 2023-05-08 20:47:36.000000 dorkbot-0.4.0/dorkbot/scanners/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     3160 2023-05-09 21:38:21.000000 dorkbot-0.4.0/dorkbot/scanners/wapiti.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.807522 dorkbot-0.4.0/dorkbot.egg-info/
--rw-r--r--   0 jgor       (501) staff       (20)    11006 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)      659 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/SOURCES.txt
--rw-r--r--   0 jgor       (501) staff       (20)        1 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/dependency_links.txt
--rw-r--r--   0 jgor       (501) staff       (20)       49 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/entry_points.txt
--rw-r--r--   0 jgor       (501) staff       (20)        8 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/top_level.txt
--rw-r--r--   0 jgor       (501) staff       (20)       74 2023-05-10 00:12:43.852897 dorkbot-0.4.0/setup.cfg
--rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.4.0/setup.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.088159 dorkbot-0.4.1/
+-rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.4.1/LICENSE
+-rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.4.1/MANIFEST.in
+-rw-r--r--   0 jgor       (501) staff       (20)    11006 2023-05-10 01:00:13.088254 dorkbot-0.4.1/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)    10604 2023-05-10 00:18:30.000000 dorkbot-0.4.1/README.md
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.041996 dorkbot-0.4.1/dorkbot/
+-rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.4.1/dorkbot/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)       22 2023-05-10 00:59:53.000000 dorkbot-0.4.1/dorkbot/_version.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)    32189 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/dorkbot.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.074958 dorkbot-0.4.1/dorkbot/indexers/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.1/dorkbot/indexers/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     1870 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/bing_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     6022 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/commoncrawl.py
+-rw-r--r--   0 jgor       (501) staff       (20)      479 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-27 19:42:53.000000 dorkbot-0.4.1/dorkbot/indexers/google.js
+-rw-r--r--   0 jgor       (501) staff       (20)     2221 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/google.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3008 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/google_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     6285 2023-05-10 00:57:38.000000 dorkbot-0.4.1/dorkbot/indexers/pywb.py
+-rw-r--r--   0 jgor       (501) staff       (20)      562 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/stdin.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     4674 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/indexers/wayback.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.087746 dorkbot-0.4.1/dorkbot/scanners/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.1/dorkbot/scanners/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3397 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/scanners/arachni.py
+-rw-r--r--   0 jgor       (501) staff       (20)      913 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/scanners/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3160 2023-05-10 00:18:30.000000 dorkbot-0.4.1/dorkbot/scanners/wapiti.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 01:00:13.044706 dorkbot-0.4.1/dorkbot.egg-info/
+-rw-r--r--   0 jgor       (501) staff       (20)    11006 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)      659 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        1 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       49 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/entry_points.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        8 2023-05-10 01:00:13.000000 dorkbot-0.4.1/dorkbot.egg-info/top_level.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       74 2023-05-10 01:00:13.089142 dorkbot-0.4.1/setup.cfg
+-rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.4.1/setup.py
```

### Comparing `dorkbot-0.4.0/LICENSE` & `dorkbot-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/PKG-INFO` & `dorkbot-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.4.0
+Version: 0.4.1
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

### Comparing `dorkbot-0.4.0/README.md` & `dorkbot-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/dorkbot.py` & `dorkbot-0.4.1/dorkbot/dorkbot.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/indexers/bing_api.py` & `dorkbot-0.4.1/dorkbot/indexers/bing_api.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/indexers/commoncrawl.py` & `dorkbot-0.4.1/dorkbot/indexers/commoncrawl.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/indexers/google.js` & `dorkbot-0.4.1/dorkbot/indexers/google.js`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/indexers/google.py` & `dorkbot-0.4.1/dorkbot/indexers/google.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/indexers/google_api.py` & `dorkbot-0.4.1/dorkbot/indexers/google_api.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/indexers/pywb.py` & `dorkbot-0.4.1/dorkbot/indexers/pywb.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,28 @@
                           help="suffix after index for index api")
     module_group.add_argument("--index", \
                           help="search a specific index")
     module_group.add_argument("--filter", \
                           help="query filter to apply to the search")
     module_group.add_argument("--retries", type=int, default=10, \
                           help="number of times to retry fetching results on error")
-    module_group.add_argument("--threads", type=int, default=1, \
+    module_group.add_argument("--threads", type=int, default=10, \
                           help="number of concurrent requests to wayback.org")
 
 
 def run(args):
     source = __name__.split(".")[-1]
     data = {}
     data["url"] = "*.%s" % args.domain
     data["output"] = "json"
     if args.filter:
         data["filter"] = args.filter
 
     if not args.index:
-        index = get_latest_index(args.server, int(args.retries))
+        args.index = get_latest_index(args.server, int(args.retries))
     base_url = f"{args.server}/{args.index}{args.cdx_api_suffix}"
     num_pages = get_num_pages(base_url, data, int(args.retries))
 
     source += f",index:{args.index}"
 
     results = get_results(base_url, data, args.retries, num_pages, args.threads, args.domain)
     for result in results:
```

### Comparing `dorkbot-0.4.0/dorkbot/indexers/stdin.py` & `dorkbot-0.4.1/dorkbot/indexers/stdin.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/indexers/wayback.py` & `dorkbot-0.4.1/dorkbot/indexers/wayback.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/scanners/arachni.py` & `dorkbot-0.4.1/dorkbot/scanners/arachni.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/scanners/example.py` & `dorkbot-0.4.1/dorkbot/scanners/example.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot/scanners/wapiti.py` & `dorkbot-0.4.1/dorkbot/scanners/wapiti.py`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/dorkbot.egg-info/PKG-INFO` & `dorkbot-0.4.1/dorkbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.4.0
+Version: 0.4.1
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
```

### Comparing `dorkbot-0.4.0/dorkbot.egg-info/SOURCES.txt` & `dorkbot-0.4.1/dorkbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorkbot-0.4.0/setup.py` & `dorkbot-0.4.1/setup.py`

 * *Files identical despite different names*

