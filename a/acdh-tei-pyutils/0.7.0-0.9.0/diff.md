# Comparing `tmp/acdh-tei-pyutils-0.7.0.tar.gz` & `tmp/acdh-tei-pyutils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh-tei-pyutils-0.7.0.tar", last modified: Mon Apr  5 06:47:24 2021, max compression
+gzip compressed data, was "acdh-tei-pyutils-0.9.0.tar", last modified: Mon Apr  5 16:53:05 2021, max compression
```

## Comparing `acdh-tei-pyutils-0.7.0.tar` & `acdh-tei-pyutils-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 06:47:24.303550 acdh-tei-pyutils-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-04-05 06:47:24.303550 acdh-tei-pyutils-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 06:47:24.303550 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7249 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7399 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils/tei.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 06:47:24.303550 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-04-05 06:47:24.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      725 2021-04-05 06:47:24.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-05 06:47:24.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-04-05 06:47:24.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-05 06:47:24.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-04-05 06:47:24.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-04-05 06:47:24.000000 acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 06:47:24.303550 acdh-tei-pyutils-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      663 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/acdh_tei_pyutils.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      778 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       85 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-04-05 06:47:24.307550 acdh-tei-pyutils-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 06:47:24.303550 acdh-tei-pyutils-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2021-04-05 06:47:14.000000 acdh-tei-pyutils-0.7.0/tests/test_tei.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 16:53:05.928910 acdh-tei-pyutils-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      289 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-04-05 16:53:05.928910 acdh-tei-pyutils-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 16:53:05.924910 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils/
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7830 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7399 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils/tei.py
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 16:53:05.924910 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-04-05 16:53:05.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2021-04-05 16:53:05.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-05 16:53:05.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2021-04-05 16:53:05.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-05 16:53:05.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-04-05 16:53:05.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-04-05 16:53:05.000000 acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 16:53:05.928910 acdh-tei-pyutils-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/acdh_tei_pyutils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4815 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2021-04-05 16:53:05.928910 acdh-tei-pyutils-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2230 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-05 16:53:05.928910 acdh-tei-pyutils-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2013 2021-04-05 16:52:55.000000 acdh-tei-pyutils-0.9.0/tests/test_tei.py
```

### Comparing `acdh-tei-pyutils-0.7.0/LICENSE` & `acdh-tei-pyutils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/PKG-INFO` & `acdh-tei-pyutils-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: acdh-tei-pyutils
-Version: 0.7.0
+Version: 0.9.0
 Summary: Utilty functions to work with TEI Documents
 Home-page: https://github.com/csae8092/acdh-tei-pyutils
 Author: Peter Andorfer
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT
 Description: ================
         acdh-tei-pyutils
```

### Comparing `acdh-tei-pyutils-0.7.0/README.rst` & `acdh-tei-pyutils-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/acdh_tei_pyutils/cli.py` & `acdh-tei-pyutils-0.9.0/acdh_tei_pyutils/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,15 +98,16 @@
     )
 
 
 @click.command()  # pragma: no cover
 @click.option('-f', '--files', default='./editions/*.xml', show_default=True)  # pragma: no cover
 @click.option('-i', '--indices', default='./indices/list*.xml', show_default=True)  # pragma: no cover
 @click.option('-t', '--event-title', default='erwähnt in ', show_default=True)  # pragma: no cover
-def denormalize_indices(files, indices, event_title):  # pragma: no cover
+@click.option('-x', '--title-xpath', default='.//tei:title/text()', show_default=True)  # pragma: no cover
+def denormalize_indices(files, indices, event_title, title_xpath):  # pragma: no cover
     """Write pointers to mentions in index-docs and copy index entries into docs"""
     files = sorted(glob.glob(files))
     index_files = sorted(glob.glob(indices))
     ref_doc_dict = defaultdict(list)
     doc_ref_dict = defaultdict(list)
     click.echo(
         click.style(
@@ -116,15 +117,15 @@
     )
     for x in tqdm.tqdm(files):
         filename = os.path.split(x)[1]
         doc = TeiEnricher(x)
         doc_base = doc.any_xpath('./@xml:base')[0]
         doc_id = doc.any_xpath('./@xml:id')[0]
         doc_uri = f"{doc_base}/{doc_id}"
-        doc_title = doc.any_xpath('.//tei:title[@type="main"]/text()')[0]
+        doc_title = doc.any_xpath(title_xpath)[0]
         refs = doc.any_xpath('.//tei:rs[@ref]/@ref')
         for ref in refs:
             ref_doc_dict[ref[1:]].append({
                 "doc_uri": doc_uri,
                 "doc_path": x,
                 "doc_title": doc_title
             })
@@ -183,14 +184,24 @@
                 for ent in ent_dict[key]:
                     list_person.append(ent)
             if key.endswith('place'):
                 list_place = ET.Element("{http://www.tei-c.org/ns/1.0}listPlace")
                 back_node.append(list_place)
                 for ent in ent_dict[key]:
                     list_place.append(ent)
+            if key.endswith('org'):
+                list_org = ET.Element("{http://www.tei-c.org/ns/1.0}listOrg")
+                back_node.append(list_org)
+                for ent in ent_dict[key]:
+                    list_org.append(ent)
+            if key.endswith('bibl'):
+                list_bibl = ET.Element("{http://www.tei-c.org/ns/1.0}listBibl")
+                back_node.append(list_bibl)
+                for ent in ent_dict[key]:
+                    list_bibl.append(ent)
         root_node.append(back_node)
         doc.tree_to_file(file=x)
     click.echo(
         click.style(
             "DONE",
             fg='green'
         )
```

### Comparing `acdh-tei-pyutils-0.7.0/acdh_tei_pyutils/tei.py` & `acdh-tei-pyutils-0.9.0/acdh_tei_pyutils/tei.py`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/PKG-INFO` & `acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: acdh-tei-pyutils
-Version: 0.7.0
+Version: 0.9.0
 Summary: Utilty functions to work with TEI Documents
 Home-page: https://github.com/csae8092/acdh-tei-pyutils
 Author: Peter Andorfer
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT
 Description: ================
         acdh-tei-pyutils
```

### Comparing `acdh-tei-pyutils-0.7.0/acdh_tei_pyutils.egg-info/SOURCES.txt` & `acdh-tei-pyutils-0.9.0/acdh_tei_pyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/docs/Makefile` & `acdh-tei-pyutils-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/docs/acdh_tei_pyutils.rst` & `acdh-tei-pyutils-0.9.0/docs/acdh_tei_pyutils.rst`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/docs/conf.py` & `acdh-tei-pyutils-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/docs/installation.rst` & `acdh-tei-pyutils-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/docs/make.bat` & `acdh-tei-pyutils-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-0.7.0/setup.py` & `acdh-tei-pyutils-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,10 +70,10 @@
             'files'
         ),
     },
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/csae8092/acdh-tei-pyutils',
-    version='0.7.0',
+    version='0.9.0',
     zip_safe=False,
 )
```

### Comparing `acdh-tei-pyutils-0.7.0/tests/test_tei.py` & `acdh-tei-pyutils-0.9.0/tests/test_tei.py`

 * *Files identical despite different names*

