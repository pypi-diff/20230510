# Comparing `tmp/pokepastes-scraper-0.2.1.tar.gz` & `tmp/pokepastes-scraper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokepastes-scraper-0.2.1.tar", last modified: Sat Apr 22 01:29:16 2023, max compression
+gzip compressed data, was "pokepastes-scraper-0.2.2.tar", last modified: Tue May  9 23:28:17 2023, max compression
```

## Comparing `pokepastes-scraper-0.2.1.tar` & `pokepastes-scraper-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.295613 pokepastes-scraper-0.2.1/
--rw-rw-rw-   0        0        0     1088 2023-04-05 18:08:47.000000 pokepastes-scraper-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3003 2023-04-22 01:29:16.292603 pokepastes-scraper-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1196 2023-04-19 01:33:09.000000 pokepastes-scraper-0.2.1/README.md
--rw-rw-rw-   0        0        0      718 2023-04-22 01:28:04.000000 pokepastes-scraper-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 01:29:16.296593 pokepastes-scraper-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.221791 pokepastes-scraper-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.239764 pokepastes-scraper-0.2.1/src/pokepastes_scraper/
--rw-rw-rw-   0        0        0     8070 2023-04-22 01:25:04.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.284629 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/
--rw-rw-rw-   0        0        0     3003 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-22 01:29:16.000000 pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-22 01:29:16.287638 pokepastes-scraper-0.2.1/test/
--rw-rw-rw-   0        0        0      745 2023-04-18 07:13:19.000000 pokepastes-scraper-0.2.1/test/test_json_conversion.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:28:17.569510 pokepastes-scraper-0.2.2/
+-rw-rw-rw-   0        0        0     1088 2023-04-05 18:08:47.000000 pokepastes-scraper-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3003 2023-05-09 23:28:17.567521 pokepastes-scraper-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2023-04-19 01:33:09.000000 pokepastes-scraper-0.2.2/README.md
+-rw-rw-rw-   0        0        0      718 2023-05-09 23:27:08.000000 pokepastes-scraper-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 23:28:17.569510 pokepastes-scraper-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 23:28:17.491521 pokepastes-scraper-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 23:28:17.512522 pokepastes-scraper-0.2.2/src/pokepastes_scraper/
+-rw-rw-rw-   0        0        0     8038 2023-05-09 11:53:31.000000 pokepastes-scraper-0.2.2/src/pokepastes_scraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 23:28:17.559510 pokepastes-scraper-0.2.2/src/pokepastes_scraper.egg-info/
+-rw-rw-rw-   0        0        0     3003 2023-05-09 23:28:17.000000 pokepastes-scraper-0.2.2/src/pokepastes_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-05-09 23:28:17.000000 pokepastes-scraper-0.2.2/src/pokepastes_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 23:28:17.000000 pokepastes-scraper-0.2.2/src/pokepastes_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-09 23:28:17.000000 pokepastes-scraper-0.2.2/src/pokepastes_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-09 23:28:17.000000 pokepastes-scraper-0.2.2/src/pokepastes_scraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 23:28:17.563563 pokepastes-scraper-0.2.2/test/
+-rw-rw-rw-   0        0        0      745 2023-04-18 07:13:19.000000 pokepastes-scraper-0.2.2/test/test_json_conversion.py
```

### Comparing `pokepastes-scraper-0.2.1/LICENSE` & `pokepastes-scraper-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pokepastes-scraper-0.2.1/PKG-INFO` & `pokepastes-scraper-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokepastes-scraper
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object.
 Author-email: MyApaulogies <myapaulogies@tuta.io>
 License: MIT License
         
         Copyright (c) 2023 MyApaulogies
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pokepastes-scraper-0.2.1/README.md` & `pokepastes-scraper-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pokepastes-scraper-0.2.1/pyproject.toml` & `pokepastes-scraper-0.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pokepastes-scraper"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="MyApaulogies", email="myapaulogies@tuta.io" },
 ]
 description = "Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pokepastes-scraper-0.2.1/src/pokepastes_scraper/__init__.py` & `pokepastes-scraper-0.2.2/src/pokepastes_scraper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         return res
 
     @staticmethod
     def _from_pre(tag: Tag):
         # rule of thumb for this function: n = next(tags_iter) whenever you are done with n's current value
         tags_iter = iter(tag.children)
-        res = PokepastesMon('asdfasdf')
+        res = PokepastesMon()
 
         firstline = ''
         while True:
             n = next(tags_iter)
             firstline += n.text
 
             if '\n' in n.text:
@@ -132,17 +132,17 @@
                 case 'Gigantamax:':
                     n = next(tags_iter)
                     res.gigantamax = True
                 case 'Tera Type:':
                     n = next(tags_iter)
                     res.tera_type = n.text.strip()
                 # see below match statement for evs: ivs: case
-                case '-':
-                    break
                 case other:
+                    if curr.startswith('-'):
+                        break
                     if curr.strip().endswith('Nature'):
                         res.nature, _ = curr.split()
 
             if curr and curr in 'EVs:IVs:':
                 if curr == 'IVs:':
                     stats = res.ivs = Stats()
                 else:
@@ -156,28 +156,27 @@
                     if n.text != ' / ':
                         break
             
             else:
                 n = next(tags_iter)
         
     
-        # n is on a '-' before the first move
         res.moveset = []
 
-        # skip '-'
-        n = next(tags_iter)
-
-        for _ in range(3):
-            res.moveset.append(n.text.strip())
-            n = next(tags_iter)
-            # skip '-'
-            n = next(tags_iter)
+        # n is on a '-' before the first move
+        moveset_str = n.text
+        for n in tags_iter:
+            moveset_str += n.text
+        
+        for move in moveset_str.split('\n'):
+            if not move.strip():
+                continue
+            # shave off '-' and whitespace
+            res.moveset.append(move[1:].strip())
 
-        # don't `n = next(tags_iter)` on the last iteration to not raise StopIteration
-        res.moveset.append(n.text.strip())
         return res
 
 
 @dataclass
 class PokepastesTeam:
     # IF YOU RENAME THIS FIELD THEN CHECK: to_dict, team_from_json 
     members: list[PokepastesMon] = None
```

### Comparing `pokepastes-scraper-0.2.1/src/pokepastes_scraper.egg-info/PKG-INFO` & `pokepastes-scraper-0.2.2/src/pokepastes_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokepastes-scraper
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extracts Pokémon team information from a https://pokepast.es/ URL to a JSON-serializable Python object.
 Author-email: MyApaulogies <myapaulogies@tuta.io>
 License: MIT License
         
         Copyright (c) 2023 MyApaulogies
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pokepastes-scraper-0.2.1/test/test_json_conversion.py` & `pokepastes-scraper-0.2.2/test/test_json_conversion.py`

 * *Files identical despite different names*

