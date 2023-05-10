# Comparing `tmp/linglit-1.2.0.tar.gz` & `tmp/linglit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linglit-1.2.0.tar", last modified: Mon Nov 28 12:12:28 2022, max compression
+gzip compressed data, was "linglit-1.3.0.tar", last modified: Tue Jan 10 08:19:52 2023, max compression
```

## Comparing `linglit-1.2.0.tar` & `linglit-1.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.803228 linglit-1.2.0/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11357 2022-05-05 05:55:45.000000 linglit-1.2.0/LICENSE
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      692 2022-11-28 12:12:28.803228 linglit-1.2.0/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6441 2022-07-12 07:32:40.000000 linglit-1.2.0/README.md
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       81 2022-05-05 05:57:12.000000 linglit-1.2.0/pyproject.toml
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1447 2022-11-28 12:12:28.803228 linglit-1.2.0/setup.cfg
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       38 2022-05-05 05:57:26.000000 linglit-1.2.0/setup.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.799229 linglit-1.2.0/src/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.799229 linglit-1.2.0/src/linglit/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3240 2022-07-12 06:30:16.000000 linglit-1.2.0/src/linglit/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1189 2022-05-11 09:18:26.000000 linglit-1.2.0/src/linglit/__main__.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.803228 linglit-1.2.0/src/linglit/base/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7682 2022-07-12 13:59:49.000000 linglit-1.2.0/src/linglit/base/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5758 2022-05-18 07:24:15.000000 linglit-1.2.0/src/linglit/bibtex.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.799229 linglit-1.2.0/src/linglit/cfg/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.803228 linglit-1.2.0/src/linglit/cfg/glossa/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    53096 2022-05-09 11:17:47.000000 linglit-1.2.0/src/linglit/cfg/glossa/glossa.csv
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.803228 linglit-1.2.0/src/linglit/cfg/langsci/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      970 2022-05-06 12:06:05.000000 linglit-1.2.0/src/linglit/cfg/langsci/bibtool.rsc
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    82635 2022-05-09 08:51:41.000000 linglit-1.2.0/src/linglit/cfg/langsci/texfile_titles.tsv
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      455 2022-05-11 07:46:30.000000 linglit-1.2.0/src/linglit/cli_util.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.803228 linglit-1.2.0/src/linglit/commands/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-05-10 19:03:22.000000 linglit-1.2.0/src/linglit/commands/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      375 2022-05-11 08:23:30.000000 linglit-1.2.0/src/linglit/commands/bib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      260 2022-05-11 07:58:30.000000 linglit-1.2.0/src/linglit/commands/igt.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      808 2022-05-17 09:11:24.000000 linglit-1.2.0/src/linglit/commands/mergedbib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      243 2022-05-11 11:14:06.000000 linglit-1.2.0/src/linglit/commands/update.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.803228 linglit-1.2.0/src/linglit/glossa/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       54 2022-05-10 16:00:32.000000 linglit-1.2.0/src/linglit/glossa/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1766 2022-05-11 12:58:07.000000 linglit-1.2.0/src/linglit/glossa/cfg.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2247 2022-05-10 17:24:14.000000 linglit-1.2.0/src/linglit/glossa/publication.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2855 2022-11-28 08:53:12.000000 linglit-1.2.0/src/linglit/glossa/repository.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    12659 2022-07-13 08:37:08.000000 linglit-1.2.0/src/linglit/glossa/xml.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.803228 linglit-1.2.0/src/linglit/langsci/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       54 2022-05-16 07:08:56.000000 linglit-1.2.0/src/linglit/langsci/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    17070 2022-05-17 08:39:24.000000 linglit-1.2.0/src/linglit/langsci/bibtex.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2280 2022-05-16 13:32:01.000000 linglit-1.2.0/src/linglit/langsci/catalog.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2468 2022-05-11 12:58:07.000000 linglit-1.2.0/src/linglit/langsci/cfg.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    12921 2022-07-12 12:53:30.000000 linglit-1.2.0/src/linglit/langsci/examples.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    33317 2022-05-10 16:08:07.000000 linglit-1.2.0/src/linglit/langsci/latex.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9510 2022-05-16 07:58:21.000000 linglit-1.2.0/src/linglit/langsci/publication.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4737 2022-05-16 07:09:14.000000 linglit-1.2.0/src/linglit/langsci/repository.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2762 2022-05-16 07:09:55.000000 linglit-1.2.0/src/linglit/langsci/texfixes.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      725 2022-05-16 07:29:16.000000 linglit-1.2.0/src/linglit/langsci/texsoup.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      614 2022-05-11 12:02:49.000000 linglit-1.2.0/src/linglit/util.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-28 12:12:28.803228 linglit-1.2.0/src/linglit.egg-info/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      692 2022-11-28 12:12:28.000000 linglit-1.2.0/src/linglit.egg-info/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1136 2022-11-28 12:12:28.000000 linglit-1.2.0/src/linglit.egg-info/SOURCES.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2022-11-28 12:12:28.000000 linglit-1.2.0/src/linglit.egg-info/dependency_links.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       51 2022-11-28 12:12:28.000000 linglit-1.2.0/src/linglit.egg-info/entry_points.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      206 2022-11-28 12:12:28.000000 linglit-1.2.0/src/linglit.egg-info/requires.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        8 2022-11-28 12:12:28.000000 linglit-1.2.0/src/linglit.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-22 13:51:46.000000 linglit-1.3.0/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)      703 2023-01-10 08:19:52.263935 linglit-1.3.0/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     6442 2023-01-09 17:26:18.000000 linglit-1.3.0/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-22 13:51:46.000000 linglit-1.3.0/pyproject.toml
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1447 2023-01-10 08:19:52.263935 linglit-1.3.0/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)       38 2022-12-22 13:51:46.000000 linglit-1.3.0/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3268 2023-01-09 17:04:03.000000 linglit-1.3.0/src/linglit/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1189 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/__main__.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit/base/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     7682 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/base/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5815 2023-01-10 07:52:41.000000 linglit-1.3.0/src/linglit/bibtex.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit/cfg/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit/cfg/glossa/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    53096 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/cfg/glossa/glossa.csv
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit/cfg/langsci/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      970 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/cfg/langsci/bibtool.rsc
+-rw-rw-r--   0 robert    (1000) robert    (1000)    82635 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/cfg/langsci/texfile_titles.tsv
+-rw-rw-r--   0 robert    (1000) robert    (1000)      455 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/cli_util.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit/commands/
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/commands/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      375 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/commands/bib.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      260 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/commands/igt.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      808 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/commands/mergedbib.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      243 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/commands/update.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit/glossa/
+-rw-rw-r--   0 robert    (1000) robert    (1000)       54 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/glossa/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1766 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/glossa/cfg.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2247 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/glossa/publication.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2892 2023-01-09 17:04:03.000000 linglit-1.3.0/src/linglit/glossa/repository.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    12659 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/glossa/xml.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit/langsci/
+-rw-rw-r--   0 robert    (1000) robert    (1000)       54 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    17070 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/bibtex.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2280 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/catalog.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2468 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/cfg.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    12921 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/examples.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    33317 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/latex.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     9510 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/publication.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4737 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/repository.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2762 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/texfixes.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      725 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/langsci/texsoup.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      614 2022-12-22 13:51:46.000000 linglit-1.3.0/src/linglit/util.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-01-10 08:19:52.263935 linglit-1.3.0/src/linglit.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      703 2023-01-10 08:19:52.000000 linglit-1.3.0/src/linglit.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1136 2023-01-10 08:19:52.000000 linglit-1.3.0/src/linglit.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-01-10 08:19:52.000000 linglit-1.3.0/src/linglit.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       51 2023-01-10 08:19:52.000000 linglit-1.3.0/src/linglit.egg-info/entry_points.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)      206 2023-01-10 08:19:52.000000 linglit-1.3.0/src/linglit.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        8 2023-01-10 08:19:52.000000 linglit-1.3.0/src/linglit.egg-info/top_level.txt
```

### Comparing `linglit-1.2.0/LICENSE` & `linglit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/README.md` & `linglit-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 $ linglit bib glossa ../../cldf_datasets/imtvault/raw/glossa/ 6371 
 Aissen, Judith. 2003. Differential object marking: Iconicity vs. economy. Natural Language and Linguistic Theory 21. 435-483.
 
 Ameka, Felix and de Witte, Carlien and Wilkins, David and Wilkins, David. 1999. Picture series for positional verbs: Eliciting the verbal component in locative descriptions. In Manual for the 1999 field season, 48-54. Nijmegen: Max Planck Institute for Psycholinguistics.
 ...
 ```
 
-Using the `--bibtex` optin will print out the bibliography formatted in BibTeX:
+Using the `--bibtex` option will print out the bibliography formatted in BibTeX:
 ```shell
 $ linglit bib glossa ../../cldf_datasets/imtvault/raw/glossa/ 6371 --bibtex
 @article{glossa6371:B1,
   author  = {Aissen, Judith},
   year    = {2003},
   pages   = {435-483},
   doi     = {10.1023/A:1024109008573},
```

### Comparing `linglit-1.2.0/setup.cfg` & `linglit-1.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = linglit
-version = 1.2.0
+version = 1.3.0
 author = Robert Forkel
 author_email = robert_forkel@eva.mpg.de
 description = Programmatic access to linguistic literature
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

### Comparing `linglit-1.2.0/src/linglit/__init__.py` & `linglit-1.3.0/src/linglit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 assert langsci and glossa
 PROVIDERS = {r.id: r for r in Repository.__subclasses__() if r.id}
 
 
 def iter_publications(d='.', glottolog='glottolog', with_examples=False, exclude=None, **dirs):
     d = pathlib.Path(d)
     glottolog = Glottolog(glottolog)
-    for rid, cls in PROVIDERS.items():
+    for rid, cls in sorted(PROVIDERS.items(), key=lambda i: i[0]):
         if exclude and rid in exclude:
             continue  # pragma: no cover
         sd = dirs.get(rid, d / rid)
         if sd.exists():
             repos = cls(sd)
             glottolog.register_names(repos.lname_map)
             for pub in cls(sd).iter_publications():
```

### Comparing `linglit-1.2.0/src/linglit/__main__.py` & `linglit-1.3.0/src/linglit/__main__.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/base/__init__.py` & `linglit-1.3.0/src/linglit/base/__init__.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/bibtex.py` & `linglit-1.3.0/src/linglit/bibtex.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     by_key = collections.defaultdict(list)
 
     def norm_title(e):
         return e.fields.get('title', '').lower()
 
     for h, v in sorted(aggr.items()):
         t, y, a = h
-        if t and (y or a):  # A meaningful has. So we assume all entries in v to be identical.
+        if t and (y or a):  # A meaningful hash. So we assume all entries in v to be identical.
             k = make_key(v[0])
             if k in keys:  # The same key has already been computed for a batch of entries.
                 (_, y2, a2), title2 = keys[k]
                 title = norm_title(v[0])
 
                 sim = 0
                 if y == y2 and a == a2 and title and title2:
@@ -169,11 +169,11 @@
         year = year.groups()[0][2:]
     else:
         year = 'nd'
     s = s.replace("ä", "ae")
     s = s.replace("ö", "oe")
     s = s.replace("ü", "ue")
     s = s.replace('"=', '-')
-    creators = unidecode(s)
+    creators = unidecode(s).replace(',', '')  # unidecode converts ogonek to comma!
     for c in "/.'()= ":
         creators = creators.replace(c, '')
     return creators.lower() + ed + ':' + year
```

### Comparing `linglit-1.2.0/src/linglit/cfg/glossa/glossa.csv` & `linglit-1.3.0/src/linglit/cfg/glossa/glossa.csv`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/cfg/langsci/bibtool.rsc` & `linglit-1.3.0/src/linglit/cfg/langsci/bibtool.rsc`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/cfg/langsci/texfile_titles.tsv` & `linglit-1.3.0/src/linglit/cfg/langsci/texfile_titles.tsv`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/commands/mergedbib.py` & `linglit-1.3.0/src/linglit/commands/mergedbib.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/glossa/cfg.py` & `linglit-1.3.0/src/linglit/glossa/cfg.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/glossa/publication.py` & `linglit-1.3.0/src/linglit/glossa/publication.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/glossa/repository.py` & `linglit-1.3.0/src/linglit/glossa/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if not p.exists():
             raise KeyError(item)
         lspecs = cfg.language_specs()
         return Publication(lspecs.get(int(item)), p, repos=self)
 
     def iter_publications(self):
         lspecs = cfg.language_specs()
-        for p in self.dir.glob('*.xml'):
+        for p in sorted(self.dir.glob('*.xml'), key=lambda p_: int(p_.stem)):
             yield Publication(lspecs.get(int(p.stem)), p, repos=self)
 
 
 def download(url, verbose=False):
     if verbose:
         print('retrieving {}'.format(url))
     return urllib.request.urlopen(url).read().decode('utf8')
```

### Comparing `linglit-1.2.0/src/linglit/glossa/xml.py` & `linglit-1.3.0/src/linglit/glossa/xml.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/bibtex.py` & `linglit-1.3.0/src/linglit/langsci/bibtex.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/catalog.py` & `linglit-1.3.0/src/linglit/langsci/catalog.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/cfg.py` & `linglit-1.3.0/src/linglit/langsci/cfg.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/examples.py` & `linglit-1.3.0/src/linglit/langsci/examples.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/latex.py` & `linglit-1.3.0/src/linglit/langsci/latex.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/publication.py` & `linglit-1.3.0/src/linglit/langsci/publication.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/repository.py` & `linglit-1.3.0/src/linglit/langsci/repository.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/texfixes.py` & `linglit-1.3.0/src/linglit/langsci/texfixes.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/langsci/texsoup.py` & `linglit-1.3.0/src/linglit/langsci/texsoup.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit/util.py` & `linglit-1.3.0/src/linglit/util.py`

 * *Files identical despite different names*

### Comparing `linglit-1.2.0/src/linglit.egg-info/SOURCES.txt` & `linglit-1.3.0/src/linglit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

