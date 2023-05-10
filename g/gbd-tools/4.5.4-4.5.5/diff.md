# Comparing `tmp/gbd_tools-4.5.4.tar.gz` & `tmp/gbd_tools-4.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.5.4.tar", last modified: Mon May  8 06:55:27 2023, max compression
+gzip compressed data, was "gbd_tools-4.5.5.tar", last modified: Wed May 10 11:26:14 2023, max compression
```

## Comparing `gbd_tools-4.5.4.tar` & `gbd_tools-4.5.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.4/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.4/README.md
--rwxrwxr-x   0 root         (0) root         (0)    12120 2023-05-08 06:53:24.000000 gbd_tools-4.5.4/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.188179 gbd_tools-4.5.4/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.4/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9444 2023-05-08 06:50:54.000000 gbd_tools-4.5.4/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10587 2023-05-08 06:51:06.000000 gbd_tools-4.5.4/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     5065 2023-04-28 06:51:42.000000 gbd_tools-4.5.4/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5790 2023-04-25 15:20:20.000000 gbd_tools-4.5.4/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.4/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.4/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.192179 gbd_tools-4.5.4/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.4/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7647 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.4/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.192179 gbd_tools-4.5.4/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.4/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.192179 gbd_tools-4.5.4/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.4/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.4/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.4/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.4/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.4/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.4/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-08 06:55:27.000000 gbd_tools-4.5.4/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.5.4/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 06:55:27.196179 gbd_tools-4.5.4/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-08 06:54:19.000000 gbd_tools-4.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.570997 gbd_tools-4.5.5/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.5/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-10 11:26:14.570997 gbd_tools-4.5.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.5/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    12008 2023-05-10 10:58:05.000000 gbd_tools-4.5.5/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.562997 gbd_tools-4.5.5/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.5/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9416 2023-05-10 10:57:14.000000 gbd_tools-4.5.5/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10587 2023-05-08 06:51:06.000000 gbd_tools-4.5.5/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     6095 2023-05-10 11:22:47.000000 gbd_tools-4.5.5/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5453 2023-05-10 11:20:19.000000 gbd_tools-4.5.5/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.5/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.5/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.562997 gbd_tools-4.5.5/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.5/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7756 2023-05-10 08:09:50.000000 gbd_tools-4.5.5/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.562997 gbd_tools-4.5.5/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.5/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.562997 gbd_tools-4.5.5/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.566997 gbd_tools-4.5.5/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.5/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.5/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.5/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.5/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.5/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.566997 gbd_tools-4.5.5/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.5/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.570997 gbd_tools-4.5.5/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.5.5/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 11:26:14.570997 gbd_tools-4.5.5/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-10 11:24:44.000000 gbd_tools-4.5.5/setup.py
```

### Comparing `gbd_tools-4.5.4/LICENSE` & `gbd_tools-4.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/PKG-INFO` & `gbd_tools-4.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.5.4
+Version: 4.5.5
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.4/README.md` & `gbd_tools-4.5.5/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd.py` & `gbd_tools-4.5.5/gbd.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     api.rename_feature(args.old_name, args.new_name)
 
 def cli_copy(api: GBD, args):
     api.copy_feature(args.old_name, args.new_name, args.target_db, args.query, args.hashes)
 
 
 def cli_get(api: GBD, args):
-    df = api.query(args.query, args.hashes, args.resolve, args.collapse, args.group_by, args.join_type, args.subselect)
+    df = api.query(args.query, args.hashes, args.resolve, args.collapse, args.group_by, args.join_type)
     for index, row in df.iterrows():
         print(" ".join([ item or "[None]" for item in row.to_list() ]))
 
 def cli_set(api: GBD, args):
     hashes = api.query(args.query, args.hashes)['hash'].tolist()
     if args.create:
         hashes = list(set(hashes + args.hashes))
@@ -158,15 +158,14 @@
     parser_get = subparsers.add_parser('get', help='Get data by query (or hash-list via stdin)')
     add_query_and_hashes_arguments(parser_get)
     parser_get.add_argument('-r', '--resolve', help='List of features to resolve against', nargs='+')
     parser_get.add_argument('-c', '--collapse', default='group_concat', 
                             choices=['group_concat', 'min', 'max', 'avg', 'count', 'sum', 'none'], 
                             help='Treatment of multiple values per hash (or grouping value resp.)')
     parser_get.add_argument('-g', '--group_by', default='hash', help='Group by specified attribute value')
-    parser_get.add_argument('--subselect', help='Move where to subselect', action='store_true')
     parser_get.add_argument('--join-type', help='Join Type: treatment of missing values in queries', choices=['INNER', 'OUTER', 'LEFT'], default="LEFT")
     parser_get.set_defaults(func=cli_get)
 
     # GBD SET
     parser_set = subparsers.add_parser('set', help='Set specified attribute-value for query result')
     parser_set.add_argument('assign', type=key_value_type, help='key=value')
     parser_set.add_argument('-c', '--create', help='Create given hashes if they do not exist yet (otherwise intersect with existing hashes)', action='store_true')
```

### Comparing `gbd_tools-4.5.4/gbd_core/api.py` & `gbd_tools-4.5.5/gbd_core/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,18 +57,18 @@
             Returns:
                 str: GBD hash
         """
         from gbd_init.gbdhash import identify
         return identify(path)
 
 
-    def query(self, gbd_query=None, hashes=[], resolve=[], collapse="group_concat", group_by="hash", join_type="LEFT", subselect=False):
+    def query(self, gbd_query=None, hashes=[], resolve=[], collapse="group_concat", group_by="hash", join_type="LEFT"):
         query_builder = GBDQuery(self.database, gbd_query)
         try:
-            sql = query_builder.build_query(hashes, resolve or [], group_by or "hash", join_type, collapse, subselect)
+            sql = query_builder.build_query(hashes, resolve or [], group_by or "hash", join_type, collapse)
         except tatsu.exceptions.FailedParse as err:
             if self.verbose:
                 util.eprint(traceback.format_exc())
             raise GBDException("Parser Error with Query '{}': {}".format(gbd_query, str(err)))
         try:
             result = self.database.query(sql)
         except sqlite3.OperationalError as err:
```

### Comparing `gbd_tools-4.5.4/gbd_core/contexts.py` & `gbd_tools-4.5.5/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_core/database.py` & `gbd_tools-4.5.5/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_core/grammar.py` & `gbd_tools-4.5.5/gbd_core/grammar.py`

 * *Files 15% similar despite different names*

```diff
@@ -109,28 +109,41 @@
     def get_sql(self, db: Database, ast=None):
         try:
             ast = ast if ast else self.ast
             if "q" in ast:
                 return "(" + self.get_sql(db, ast["q"]) + ")"
             elif "t" in ast:
                 return "(" + self.get_sql(db, ast["t"]) + ")"
-            elif "qop" in ast or "top" in ast:
+            elif "qop" in ast or "top" in ast: # query operator or term operator
                 operator = ast["qop"] if ast["qop"] else ast["top"]
                 left = self.get_sql(db, ast["left"])
                 right = self.get_sql(db, ast["right"])
                 return "{} {} {}".format(left, operator, right)
-            elif "cop" in ast:
+            elif "cop" in ast: # constraint operator
                 operator = "not like" if ast["cop"] == "unlike" else ast["cop"]
                 feat = db.faddr(ast["col"])
+                feat_is_1_n = db.finfo(ast["col"]).default is None
                 if "str" in ast:
-                    return "{} {} '{}'".format(feat, operator, ast["str"])
+                    if feat_is_1_n and ast["cop"] == "!=":
+                        table = db.faddr_table(ast["col"])
+                        return "{t}.hash NOT IN (SELECT {t}.hash FROM {t} WHERE {f} = '{s}')".format(t=table, f=feat, s=ast["str"])
+                    else:
+                        return "{} {} '{}'".format(feat, operator, ast["str"])
                 elif "lik" in ast:
-                    return "{} {} '{}'".format(feat, operator, "".join([ t for t in ast["lik"] if t ]))
+                    if feat_is_1_n and ast["cop"] == "unlike":
+                        table = db.faddr_table(ast["col"])
+                        return "{t}.hash NOT IN (SELECT {t}.hash FROM {t} WHERE {f} like '{s}')".format(t=table, f=feat, s="".join([ t for t in ast["lik"] if t ]))
+                    else:
+                        return "{} {} '{}'".format(feat, operator, "".join([ t for t in ast["lik"] if t ]))
                 elif "ter" in ast:
-                    return "CAST({} AS FLOAT) {} {}".format(feat, operator, self.get_sql(db, ast["ter"]))
+                    if feat_is_1_n and ast["cop"] == "!=":
+                        table = db.faddr_table(ast["col"])
+                        return "{t}.hash NOT IN (SELECT {t}.hash FROM {t} WHERE CAST({f} AS FLOAT) = {s})".format(t=table, f=feat, s=self.get_sql(db, ast["ter"]))
+                    else:
+                        return "CAST({} AS FLOAT) {} {}".format(feat, operator, self.get_sql(db, ast["ter"]))
                 raise ParserException("Missing right-hand side of constraint")
             elif "col" in ast:
                 feature = db.faddr(ast["col"])
                 return "CAST({} AS FLOAT)".format(feature)
             elif "constant" in ast:
                 return ast["constant"]
             else:
```

### Comparing `gbd_tools-4.5.4/gbd_core/query.py` & `gbd_tools-4.5.5/gbd_core/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,22 +30,22 @@
     def features_exist_or_throw(self, features):
         for feature in features:
             if not feature in self.db.get_features():
                 raise DatabaseException("Unknown feature '{}'".format(feature))
 
 
     # Generate SQL Query from given GBD Query 
-    def build_query(self, hashes=[], resolve=[], group_by="hash", join_type="LEFT", collapse=None, where_in_subselect=False):
+    def build_query(self, hashes=[], resolve=[], group_by="hash", join_type="LEFT", collapse=None):
         self.features_exist_or_throw(resolve + [group_by] + list(self.features))
 
         sql_select = self.build_select(group_by, resolve, collapse)
 
         sql_from = self.build_from(group_by, set(resolve) | self.features, join_type)
         
-        sql_where = self.build_where(hashes, group_by, where_in_subselect)
+        sql_where = self.build_where(hashes, group_by)
 
         sql_groupby = "GROUP BY {}".format(self.db.faddr(group_by)) if collapse else ""
         sql_orderby = "ORDER BY {}".format(self.db.faddr(group_by))
         
         return "{} {} WHERE {} {} {}".format(sql_select, sql_from, sql_where, sql_groupby, sql_orderby)
 
 
@@ -101,18 +101,14 @@
                         result[taddress] = "INNER JOIN {trans} ON {group}.hash = {trans}.{dir0}".format(trans=taddress, group=gaddress, dir0=direction[0])
                         
                     result[faddress] = "INNER JOIN {feat} ON {trans}.{dir1} = {feat}.hash".format(feat=faddress, trans=taddress, dir1=direction[1])
 
         return " ".join(result.values())
 
 
-    def build_where(self, hashes, group_by, subselect=False):
-        result = "{} != 'None'".format(self.db.faddr(group_by))
-        if subselect:
-            fro = self.build_from(group_by, self.features)
-            whe = self.parser.get_sql(self.db)
-            result = result + " AND {}.hash in (SELECT {}.hash FROM {} WHERE {})".format(self.db.faddr_table(group_by), self.db.faddr_table(group_by), fro, whe)
-        else:
-            result = result + " AND " + self.parser.get_sql(self.db)
+    def build_where(self, hashes, group_by):
+        group_column = self.db.faddr(group_by)
+        group_table = self.db.faddr_table(group_by)
+        result = group_column + " != 'None' AND " + self.parser.get_sql(self.db)
         if len(hashes):
-            result = result + " AND {}.hash in ('{}')".format(self.db.faddr_table(group_by), "', '".join(hashes))
+            result = result + " AND {}.hash in ('{}')".format(group_table, "', '".join(hashes))
         return result
```

### Comparing `gbd_tools-4.5.4/gbd_core/schema.py` & `gbd_tools-4.5.5/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_core/util.py` & `gbd_tools-4.5.5/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_core/util_argparse.py` & `gbd_tools-4.5.5/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_init/cnf_extractors.py` & `gbd_tools-4.5.5/gbd_init/cnf_extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     extractor = Initializer([ context ], [ context ], api, context, rlimits, target_db, features, compute_hash)
     extractor.create_features()
 
     df = api.query(group_by="local")
     
     dfilter = df["local"].apply(lambda x: not x or not os.path.isfile(x))
     missing = df[dfilter]
+    if len(missing) and api.verbose:
+        for path in missing["local"].tolist():
+            eprint(path)
     if len(missing) and confirm("{} files not found. Remove stale entries from local table?".format(len(missing))):
         api.reset_values("local", values=missing["local"].tolist())
 
     paths = [ path for suffix in suffix_list(context) for path in glob.iglob(root + "/**/*" + suffix, recursive=True) ]
     df2 = pd.DataFrame([(None, path) for path in paths if not path in df["local"].to_list()], columns=["hash", "local"])
     
     extractor.run(df2)
```

### Comparing `gbd_tools-4.5.4/gbd_init/cnf_transformers.py` & `gbd_tools-4.5.5/gbd_init/cnf_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_init/gbdhash.py` & `gbd_tools-4.5.5/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_init/initializer.py` & `gbd_tools-4.5.5/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.5.5/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.5.5/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.5.5/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_server/static/main.css` & `gbd_tools-4.5.5/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_server/static/w3.js` & `gbd_tools-4.5.5/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_server/templates/index.html` & `gbd_tools-4.5.5/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.5.5/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.5.4
+Version: 4.5.5
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.4/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.5.5/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/server.py` & `gbd_tools-4.5.5/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.4/setup.py` & `gbd_tools-4.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.5.4',
+  version='4.5.5',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

