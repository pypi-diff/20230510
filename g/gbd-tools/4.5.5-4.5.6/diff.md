# Comparing `tmp/gbd_tools-4.5.5.tar.gz` & `tmp/gbd_tools-4.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_tools-4.5.5.tar", last modified: Wed May 10 11:26:14 2023, max compression
+gzip compressed data, was "gbd_tools-4.5.6.tar", last modified: Wed May 10 12:17:25 2023, max compression
```

## Comparing `gbd_tools-4.5.5.tar` & `gbd_tools-4.5.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.570997 gbd_tools-4.5.5/
--rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.5/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-10 11:26:14.570997 gbd_tools-4.5.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.5/README.md
--rwxrwxr-x   0 root         (0) root         (0)    12008 2023-05-10 10:58:05.000000 gbd_tools-4.5.5/gbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.562997 gbd_tools-4.5.5/gbd_core/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.5/gbd_core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9416 2023-05-10 10:57:14.000000 gbd_tools-4.5.5/gbd_core/api.py
--rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_core/contexts.py
--rw-rw-r--   0 root         (0) root         (0)    10587 2023-05-08 06:51:06.000000 gbd_tools-4.5.5/gbd_core/database.py
--rw-rw-r--   0 root         (0) root         (0)     6095 2023-05-10 11:22:47.000000 gbd_tools-4.5.5/gbd_core/grammar.py
--rw-rw-r--   0 root         (0) root         (0)     5453 2023-05-10 11:20:19.000000 gbd_tools-4.5.5/gbd_core/query.py
--rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.5/gbd_core/schema.py
--rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_core/util.py
--rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.5/gbd_core/util_argparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.562997 gbd_tools-4.5.5/gbd_init/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.5/gbd_init/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7756 2023-05-10 08:09:50.000000 gbd_tools-4.5.5/gbd_init/cnf_extractors.py
--rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_init/cnf_transformers.py
--rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_init/gbdhash.py
--rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.5/gbd_init/initializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.562997 gbd_tools-4.5.5/gbd_server/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.5/gbd_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.562997 gbd_tools-4.5.5/gbd_server/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.566997 gbd_tools-4.5.5/gbd_server/static/img/
--rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.5/gbd_server/static/img/gbd_logo.jpg
--rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.5/gbd_server/static/img/gbd_logo.png
--rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.5/gbd_server/static/img/gbd_logo_small.png
--rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.5/gbd_server/static/main.css
--rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.5/gbd_server/static/w3.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.566997 gbd_tools-4.5.5/gbd_server/templates/
--rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.5/gbd_server/templates/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 11:26:14.570997 gbd_tools-4.5.5/gbd_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3757 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      772 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-10 11:26:14.000000 gbd_tools-4.5.5/gbd_tools.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.5.5/server.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 11:26:14.570997 gbd_tools-4.5.5/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-10 11:24:44.000000 gbd_tools-4.5.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:17:25.227201 gbd_tools-4.5.6/
+-rw-rw-r--   0 root         (0) root         (0)     1109 2023-01-02 08:34:51.000000 gbd_tools-4.5.6/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      206 2022-12-15 15:28:20.000000 gbd_tools-4.5.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-10 12:17:25.227201 gbd_tools-4.5.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3248 2023-02-07 16:30:01.000000 gbd_tools-4.5.6/README.md
+-rwxrwxr-x   0 root         (0) root         (0)    12008 2023-05-10 10:58:05.000000 gbd_tools-4.5.6/gbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:17:25.211201 gbd_tools-4.5.6/gbd_core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:03:01.000000 gbd_tools-4.5.6/gbd_core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9416 2023-05-10 10:57:14.000000 gbd_tools-4.5.6/gbd_core/api.py
+-rw-rw-r--   0 root         (0) root         (0)     1937 2023-04-20 08:28:49.000000 gbd_tools-4.5.6/gbd_core/contexts.py
+-rw-rw-r--   0 root         (0) root         (0)    10587 2023-05-08 06:51:06.000000 gbd_tools-4.5.6/gbd_core/database.py
+-rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-10 11:45:07.000000 gbd_tools-4.5.6/gbd_core/grammar.py
+-rw-rw-r--   0 root         (0) root         (0)     5452 2023-05-10 12:13:23.000000 gbd_tools-4.5.6/gbd_core/query.py
+-rw-rw-r--   0 root         (0) root         (0)    12359 2023-04-25 15:02:02.000000 gbd_tools-4.5.6/gbd_core/schema.py
+-rw-rw-r--   0 root         (0) root         (0)     4015 2023-04-20 08:28:49.000000 gbd_tools-4.5.6/gbd_core/util.py
+-rw-rw-r--   0 root         (0) root         (0)     3486 2023-05-05 18:48:49.000000 gbd_tools-4.5.6/gbd_core/util_argparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:17:25.215201 gbd_tools-4.5.6/gbd_init/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-12-12 14:00:05.000000 gbd_tools-4.5.6/gbd_init/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7756 2023-05-10 08:09:50.000000 gbd_tools-4.5.6/gbd_init/cnf_extractors.py
+-rw-rw-r--   0 root         (0) root         (0)     3853 2023-04-20 08:28:49.000000 gbd_tools-4.5.6/gbd_init/cnf_transformers.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-04-20 08:28:49.000000 gbd_tools-4.5.6/gbd_init/gbdhash.py
+-rw-rw-r--   0 root         (0) root         (0)     3513 2023-04-20 08:28:49.000000 gbd_tools-4.5.6/gbd_init/initializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:17:25.215201 gbd_tools-4.5.6/gbd_server/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-09-06 14:45:24.000000 gbd_tools-4.5.6/gbd_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:17:25.215201 gbd_tools-4.5.6/gbd_server/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:17:25.223201 gbd_tools-4.5.6/gbd_server/static/img/
+-rw-rw-r--   0 root         (0) root         (0)   125407 2022-09-06 14:45:24.000000 gbd_tools-4.5.6/gbd_server/static/img/gbd_logo.jpg
+-rw-rw-r--   0 root         (0) root         (0)   835988 2022-09-06 14:45:24.000000 gbd_tools-4.5.6/gbd_server/static/img/gbd_logo.png
+-rw-rw-r--   0 root         (0) root         (0)    32090 2022-09-06 14:45:24.000000 gbd_tools-4.5.6/gbd_server/static/img/gbd_logo_small.png
+-rw-rw-r--   0 root         (0) root         (0)     1773 2023-04-16 15:10:50.000000 gbd_tools-4.5.6/gbd_server/static/main.css
+-rw-rw-r--   0 root         (0) root         (0)    11975 2022-09-08 11:53:31.000000 gbd_tools-4.5.6/gbd_server/static/w3.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:17:25.223201 gbd_tools-4.5.6/gbd_server/templates/
+-rw-rw-r--   0 root         (0) root         (0)     5016 2023-04-16 15:24:02.000000 gbd_tools-4.5.6/gbd_server/templates/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:17:25.227201 gbd_tools-4.5.6/gbd_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-05-10 12:17:24.000000 gbd_tools-4.5.6/gbd_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-10 12:17:24.000000 gbd_tools-4.5.6/gbd_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:17:24.000000 gbd_tools-4.5.6/gbd_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-10 12:17:24.000000 gbd_tools-4.5.6/gbd_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-10 12:17:24.000000 gbd_tools-4.5.6/gbd_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-10 12:17:24.000000 gbd_tools-4.5.6/gbd_tools.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)    11989 2023-04-20 15:30:11.000000 gbd_tools-4.5.6/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 12:17:25.227201 gbd_tools-4.5.6/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1034 2023-05-10 12:16:18.000000 gbd_tools-4.5.6/setup.py
```

### Comparing `gbd_tools-4.5.5/LICENSE` & `gbd_tools-4.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/PKG-INFO` & `gbd_tools-4.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd_tools
-Version: 4.5.5
+Version: 4.5.6
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.5/README.md` & `gbd_tools-4.5.6/README.md`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd.py` & `gbd_tools-4.5.6/gbd.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_core/api.py` & `gbd_tools-4.5.6/gbd_core/api.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_core/contexts.py` & `gbd_tools-4.5.6/gbd_core/contexts.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_core/database.py` & `gbd_tools-4.5.6/gbd_core/database.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_core/grammar.py` & `gbd_tools-4.5.6/gbd_core/grammar.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,30 +118,34 @@
                 left = self.get_sql(db, ast["left"])
                 right = self.get_sql(db, ast["right"])
                 return "{} {} {}".format(left, operator, right)
             elif "cop" in ast: # constraint operator
                 operator = "not like" if ast["cop"] == "unlike" else ast["cop"]
                 feat = db.faddr(ast["col"])
                 feat_is_1_n = db.finfo(ast["col"]).default is None
-                if "str" in ast:
-                    if feat_is_1_n and ast["cop"] == "!=":
+                if "str" in ast: # cop:("=" | "!=")
+                    if feat_is_1_n:
                         table = db.faddr_table(ast["col"])
-                        return "{t}.hash NOT IN (SELECT {t}.hash FROM {t} WHERE {f} = '{s}')".format(t=table, f=feat, s=ast["str"])
+                        setop = "IN" if ast["cop"] == "=" else "NOT IN"
+                        return "{t}.hash {o} (SELECT {t}.hash FROM {t} WHERE {f} = '{s}')".format(o=setop, t=table, f=feat, s=ast["str"])
                     else:
                         return "{} {} '{}'".format(feat, operator, ast["str"])
-                elif "lik" in ast:
-                    if feat_is_1_n and ast["cop"] == "unlike":
+                elif "lik" in ast: # cop:("like" | "unlike")
+                    if feat_is_1_n:
                         table = db.faddr_table(ast["col"])
-                        return "{t}.hash NOT IN (SELECT {t}.hash FROM {t} WHERE {f} like '{s}')".format(t=table, f=feat, s="".join([ t for t in ast["lik"] if t ]))
+                        setop = "IN" if ast["cop"] == "like" else "NOT IN"
+                        return "{t}.hash {o} (SELECT {t}.hash FROM {t} WHERE {f} like '{s}')".format(o=setop, t=table, f=feat, s="".join([ t for t in ast["lik"] if t ]))
                     else:
                         return "{} {} '{}'".format(feat, operator, "".join([ t for t in ast["lik"] if t ]))
-                elif "ter" in ast:
+                elif "ter" in ast: # cop:("=" | "!=" | "<=" | ">=" | "<" | ">" )
                     if feat_is_1_n and ast["cop"] == "!=":
                         table = db.faddr_table(ast["col"])
-                        return "{t}.hash NOT IN (SELECT {t}.hash FROM {t} WHERE CAST({f} AS FLOAT) = {s})".format(t=table, f=feat, s=self.get_sql(db, ast["ter"]))
+                        setop = "NOT IN" if ast["cop"] == "!=" else "IN"
+                        cop = "=" if ast["cop"] == "!=" else ast["cop"]
+                        return "{t}.hash {o} (SELECT {t}.hash FROM {t} WHERE CAST({f} AS FLOAT) {c} {s})".format(o=setop, c=cop, t=table, f=feat, s=self.get_sql(db, ast["ter"]))
                     else:
                         return "CAST({} AS FLOAT) {} {}".format(feat, operator, self.get_sql(db, ast["ter"]))
                 raise ParserException("Missing right-hand side of constraint")
             elif "col" in ast:
                 feature = db.faddr(ast["col"])
                 return "CAST({} AS FLOAT)".format(feature)
             elif "constant" in ast:
```

### Comparing `gbd_tools-4.5.5/gbd_core/query.py` & `gbd_tools-4.5.6/gbd_core/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         
         return "{} {} WHERE {} {} {}".format(sql_select, sql_from, sql_where, sql_groupby, sql_orderby)
 
 
     def build_select(self, group_by, resolve, collapse=None):
         result = [ self.db.faddr(f) for f in [group_by] + resolve ]
         if collapse and collapse != "none":
-            result = [ "{}(DISTINCT({}))".format(collapse, r) for r in result ]
-        return "SELECT " + ", ".join(result)
+            result = [ "{}({})".format(collapse, r) for r in result ]
+        return "SELECT DISTINCT " + ", ".join(result)
 
 
     def find_translator_feature(self, source_context, target_context):
         for dbname in self.db.get_databases(source_context):
             #eprint("Checking database {} for translator".format(dbname))
             if "to_"+target_context in self.db.get_features([ dbname ]):
                 return self.db.finfo("to_"+target_context, dbname)
```

### Comparing `gbd_tools-4.5.5/gbd_core/schema.py` & `gbd_tools-4.5.6/gbd_core/schema.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_core/util.py` & `gbd_tools-4.5.6/gbd_core/util.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_core/util_argparse.py` & `gbd_tools-4.5.6/gbd_core/util_argparse.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_init/cnf_extractors.py` & `gbd_tools-4.5.6/gbd_init/cnf_extractors.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_init/cnf_transformers.py` & `gbd_tools-4.5.6/gbd_init/cnf_transformers.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_init/gbdhash.py` & `gbd_tools-4.5.6/gbd_init/gbdhash.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_init/initializer.py` & `gbd_tools-4.5.6/gbd_init/initializer.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_server/static/img/gbd_logo.jpg` & `gbd_tools-4.5.6/gbd_server/static/img/gbd_logo.jpg`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_server/static/img/gbd_logo.png` & `gbd_tools-4.5.6/gbd_server/static/img/gbd_logo.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_server/static/img/gbd_logo_small.png` & `gbd_tools-4.5.6/gbd_server/static/img/gbd_logo_small.png`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_server/static/main.css` & `gbd_tools-4.5.6/gbd_server/static/main.css`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_server/static/w3.js` & `gbd_tools-4.5.6/gbd_server/static/w3.js`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_server/templates/index.html` & `gbd_tools-4.5.6/gbd_server/templates/index.html`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/gbd_tools.egg-info/PKG-INFO` & `gbd_tools-4.5.6/gbd_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbd-tools
-Version: 4.5.5
+Version: 4.5.6
 Summary: GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes
 Home-page: https://github.com/Udopia/gbd
 Author: Markus Iser, Karlsruhe Institute of Technology (KIT)
 Author-email: markus.iser@kit.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `gbd_tools-4.5.5/gbd_tools.egg-info/SOURCES.txt` & `gbd_tools-4.5.6/gbd_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/server.py` & `gbd_tools-4.5.6/server.py`

 * *Files identical despite different names*

### Comparing `gbd_tools-4.5.5/setup.py` & `gbd_tools-4.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='gbd_tools',
-  version='4.5.5',
+  version='4.5.6',
   description='GBD Benchmark Database Tools: Maintenance of Benchmark Instances and their Attributes',
   long_description=open('README.md', 'rt').read(),
   long_description_content_type="text/markdown",
   url='https://github.com/Udopia/gbd',
   author='Markus Iser, Karlsruhe Institute of Technology (KIT)',
   author_email='markus.iser@kit.edu',
   packages=[
```

