# Comparing `tmp/ogc_na-0.1.6.tar.gz` & `tmp/ogc_na-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.1.6.tar", last modified: Sun May  7 18:04:12 2023, max compression
+gzip compressed data, was "ogc_na-0.2.0.tar", last modified: Wed May 10 08:29:50 2023, max compression
```

## Comparing `ogc_na-0.1.6.tar` & `ogc_na-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.602810 ogc_na-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.594810 ogc_na-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 18:03:58.000000 ogc_na-0.1.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-07 18:03:58.000000 ogc_na-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-07 18:03:58.000000 ogc_na-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-07 18:04:12.602810 ogc_na-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-07 18:03:58.000000 ogc_na-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-07 18:03:58.000000 ogc_na-0.1.6/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-07 18:03:58.000000 ogc_na-0.1.6/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-07 18:03:58.000000 ogc_na-0.1.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-07 18:03:58.000000 ogc_na-0.1.6/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-07 18:03:58.000000 ogc_na-0.1.6/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.594810 ogc_na-0.1.6/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    31680 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/ingest_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/ogc/na/input_filters/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/input_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/input_filters/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-07 18:03:58.000000 ogc_na-0.1.6/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-07 18:04:12.000000 ogc_na-0.1.6/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-07 18:03:58.000000 ogc_na-0.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.598810 ogc_na-0.1.6/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-07 18:03:58.000000 ogc_na-0.1.6/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-07 18:03:58.000000 ogc_na-0.1.6/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-07 18:03:58.000000 ogc_na-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:04:12.602810 ogc_na-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-07 18:03:58.000000 ogc_na-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.602810 ogc_na-0.1.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:04:12.602810 ogc_na-0.1.6/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/test_input_filters_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-07 18:03:58.000000 ogc_na-0.1.6/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.467215 ogc_na-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.459215 ogc_na-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.459215 ogc_na-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 08:29:38.000000 ogc_na-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-10 08:29:38.000000 ogc_na-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 08:29:38.000000 ogc_na-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-10 08:29:50.463215 ogc_na-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-10 08:29:38.000000 ogc_na-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.459215 ogc_na-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-05-10 08:29:38.000000 ogc_na-0.2.0/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-10 08:29:38.000000 ogc_na-0.2.0/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-10 08:29:38.000000 ogc_na-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-10 08:29:38.000000 ogc_na-0.2.0/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-10 08:29:38.000000 ogc_na-0.2.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.459215 ogc_na-0.2.0/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.463215 ogc_na-0.2.0/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12532 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31936 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.463215 ogc_na-0.2.0/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-10 08:29:38.000000 ogc_na-0.2.0/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.463215 ogc_na-0.2.0/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-10 08:29:50.000000 ogc_na-0.2.0/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-10 08:29:50.000000 ogc_na-0.2.0/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:29:50.000000 ogc_na-0.2.0/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 08:29:50.000000 ogc_na-0.2.0/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 08:29:50.000000 ogc_na-0.2.0/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-10 08:29:38.000000 ogc_na-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.463215 ogc_na-0.2.0/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-10 08:29:38.000000 ogc_na-0.2.0/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-10 08:29:38.000000 ogc_na-0.2.0/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-10 08:29:38.000000 ogc_na-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:29:50.467215 ogc_na-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-10 08:29:38.000000 ogc_na-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.463215 ogc_na-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:50.463215 ogc_na-0.2.0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-10 08:29:38.000000 ogc_na-0.2.0/test/test_profile.py
```

### Comparing `ogc_na-0.1.6/.github/workflows/python-publish.yml` & `ogc_na-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/.gitignore` & `ogc_na-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/PKG-INFO` & `ogc_na-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.1.6
+Version: 0.2.0
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.6/README.md` & `ogc_na-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/docs/examples.md` & `ogc_na-0.2.0/docs/examples.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
   dcat:dataset _:conceptSchemes, _:semanticUplift ;
 
   dcfg:hasProfileSource
     "sparql:https://example.org/sparql",
     "path/to/profile.ttl" ;
 .
 
+# A dcfg:DomainConfiguration will be used for semantic entailment and validation (update_vocabs)
 _:conceptSchemes a dcat:Dataset, dcfg:DomainConfiguration ;
   dct:identifier "conceptSchemes" ;
   dct:description "Set of terms registered with OGC NA not covered by specialised domains" ;
   
   # Which files to include
   dcfg:glob "definitions/conceptSchemes/*.ttl" ;
                  
@@ -42,37 +43,49 @@
   dcfg:uriRootFilter "/def/" ;
                  
   # Profile conformance can optionally be declared in the DomainConfiguration
   # as well as in the source data itself
   dct:conformsTo profiles:vocprez_ogc, profiles:skos_conceptscheme ;
 .
 
+# A dcfg:UpliftConfiguration will be used for semantic uplift (ingest_json)
 _:semanticUplift a dcat:Dataset, dcfg:UpliftConfiguration;
   dct:identifier "semanticUplift" ;
   dct:description "Semantic uplift configuration" ;
   
   # Which files to include
   dcfg:glob "domain1/*.json", "domain2/*.json" ;
 
   # List of profiles (with semantic uplift artifacts) and/or files to 
   # use as uplift definitions
   dcfg:hasUpliftDefinition
-    [ dcfg:order 1; dcfg:file "path/to/file.yaml" ],             # Local file
+    [ dcfg:order 1; dcfg:file "path/to/file.yaml" ],             # Local file, from working directory
     [ dcfg:order 2; dcfg:profile profiles:vocprez_ogc ],         # Profile
-    [ dcfg:order 3; dcfg:file "path/to/another/definition.yaml"] # Local file
+    [ dcfg:order 3; dcfg:file "path/to/another/definition.yaml"] # Local file, from working directory
   ;
 .
 ```
 
 ## Sample JSON-LD uplift context
 
 ```yaml
 # Sample single-file JSON-LD context
 # Processing order is transform -> types -> context
 
+# Input filters allow reading files with a format other than JSON/JSON-LD.
+# Every filter has its own configuration options.
+# When using input filters, the output will be an object with two entries, "metadata" 
+# (with metadata about the original file, the filter configuration, etc.), and "data"
+# (with the data read from the input document). 
+input-filter:
+  csv:
+    skip-rows: 2
+    trim-values: true
+    
+
 # `path-scope` affects how ingest_json treats JSON-LD documents (e.g. when chaining uplifts).
 # It can be `graph` (transformations and paths act on `@graph`, if any, instead of on the
 # whole file) or `document` (do not treat JSON-LD files differently, process "as is").
 # Default is `graph`.
 path-scope: graph
 
 # `transform` uses jq expressions for light data transformations
@@ -123,58 +136,11 @@
   # scoped context for elements with "type" = "IS"
   '$[?type="IS"]': {
     "@vocab": "http://example.org/vocab3#"
   }
 
 # `context-position` dictates where the new context will be added if `@context` is already present
 # at any of the specified paths. Can be `before` (a new entry, with lower precedence, will be preprended
-# to any existing `@context`) or `after` (a new entry, with higher precedence, will be appended to any
-# existing `@context`). It has no effect for plan JSON documents. 
+# to any existing `@context`; this is the default behavior) or `after` (a new entry, with higher 
+# precedence, will be appended to any existing `@context`). It has no effect for plain JSON documents. 
 context-position: before
 ```
-
-## Sample JSON-LD context registry
-
-The following example defines 3 profile sources (two from local files and one from a SPARQL endpoint),
-and 3 domain configurations for semantic uplifts:
-
-* One for JSON documents inside `domain1` and all its subdirectories, using a definition from a profile (`profileY`)
-  and then another from a file. 
-* Another one for JSON documents inside `domain2` (but not its subdirectories), using only a definition from a file
-  (`profileZ`).
-* A third one for JSON documents inside `domain3`, using two profile definitions sequentially (first from `profileQ`
-and then from `profileR`).
-
-Additionally, 2 local artifact mappings are declared, telling the profile artifact resolver to map
-the `http://example.com/base/1` URL to the `artifacts/base/1` directory, and `http://example.com/another/base/`
-to `artifacts/another/base`.
-
-```json
-{
-  "contexts": {
-    "domain1/**/*.json": [
-      { "profile": "http://example.com/profileY" },
-      { "file": "domain1/common.yml" }
-    ],
-    "domain2/*.json": { "profile": "http://example.com/profileZ" },
-    "domain3/*.json": [
-      { "profile": "http://example.com/profileQ" },
-      { "profile": "http://example.com/profileR" }
-    ]
-  },
-  
-  "profileSources": [
-    { "file": "profiles/my-profile.ttl" },
-    { "file": "also-supports-globs/*.ttl" },
-    { "sparql":  "http://example.com/sparql" }
-  ],
-  
-  "localArtifactMappings": [
-      { "http://example.com/base/1": "artifacts/base/1" },
-      { "http://example.com/another/base/": "artifacts/another/base" }
-  ]
-}
-```
-
-YAML syntax is also supported.
-
-**Note**: The use of profiles is optional for context registries and can be omitted.
```

### Comparing `ogc_na-0.1.6/docs/gen_ref_pages.py` & `ogc_na-0.2.0/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/docs/index.md` & `ogc_na-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/docs/tutorials.md` & `ogc_na-0.2.0/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/mkdocs.yml` & `ogc_na-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/ogc/na/annotate_schema.py` & `ogc_na-0.2.0/ogc/na/annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/ogc/na/domain_config.py` & `ogc_na-0.2.0/ogc/na/domain_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from __future__ import annotations
 import logging
 import os
 from pathlib import Path
 from typing import Union, Optional, Sequence, cast, IO, TypeVar
 
+import wcmatch.glob
 from rdflib import Graph, Namespace, URIRef, DCTERMS, DCAT, Literal
 from wcmatch.glob import globmatch
 
 from ogc.na.profile import ProfileRegistry
 
 DCFG = Namespace('http://www.example.org/ogc/domain-cfg#')
 
@@ -208,15 +209,15 @@
         logger.info("Found %d domain configurations and %d uplift configurations",
                     len(self.entries),
                     len(self.uplift_entries))
 
         return self
 
     def __len__(self):
-        return len(self.entries)
+        return len(self.entries) + len(self.uplift_entries)
 
 
 class ConfigurationEntry:
 
     def __init__(self,
                  working_directory: Path,
                  glob: Sequence[str],
@@ -230,15 +231,15 @@
     def find_all(self) -> set[Path]:
         return set(item for g in self.globs for item in self.working_directory.glob(g))
 
     def matches(self, fn: str | Path) -> bool:
         if not isinstance(fn, Path):
             fn = Path(fn)
         fn = os.path.relpath(fn.resolve(), self.working_directory)
-        return globmatch(fn, self.globs)
+        return globmatch(fn, self.globs, flags=wcmatch.glob.G)
 
 
 class DomainConfigurationEntry(ConfigurationEntry):
 
     def __init__(self,
                  working_directory: Path,
                  glob: Sequence[str],
@@ -277,15 +278,15 @@
         for entry in self:
             if entry.matches(fn):
                 return entry
 
     def find_entries_for_files(self, fns: list[str | Path]) -> 'dict[Path, ConfigurationEntry]':
         """
         Find the configuration entries associated to a list of files. Similar
-        to [find_file()][ogc.na.domain_config.ConfigurationEntryList.find_file]
+        to [find_entry_for_file()][ogc.na.domain_config.ConfigurationEntryList.find_entry_for_file]
         but with a list of files.
 
         :param fns: a list of files to find
         :return: a path \u2192 DomainConfigurationEntry dict for each file that is found
         """
         result: dict[Path, ConfigurationEntry] = {}
         for fn in fns:
```

### Comparing `ogc_na-0.1.6/ogc/na/download.py` & `ogc_na-0.2.0/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/ogc/na/ingest_json.py` & `ogc_na-0.2.0/ogc/na/ingest_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
 """
 This module contains classes to perform JSON-LD uplifting operations, facilitating
 the conversion of standard JSON into JSON-LD.
 
-JSON-LD uplifting is done in 3 steps:
+JSON-LD uplifting is done in 4 steps:
 
+* Input filter pre-processing (e.g., csv). This step is *optional*.
 * Initial transformation using [jq](https://stedolan.github.io/jq/manual/) expressions (`transform`).
 * Class annotation (adding `@type` to the root object and/or to specific nodes, using
   [jsonpath-ng](https://pypi.org/project/jsonpath-ng/) expressions) (`types`).
 * Injecting custom JSON-LD `@context` either globally or inside specific nodes (using
   [jsonpath-ng](https://pypi.org/project/jsonpath-ng/) expressions (`context`).
 
 The details for each of these operations are declared inside context definition files,
 which are YAML documents containing specifications for the uplift workflow. For each input
 JSON file, its corresponding YAML context definition is detected at runtime:
 
-1. A [context definition registry][ogc.na.ingest_json.ContextRegistry] can be used,
+1. A [domain configuration][ogc.na.domain_config.DomainConfiguration] can be used,
 which is a JSON (or YAML) document that defines JSON file to context definition mappings.
 2. If no registry is used or the input file is not in the registry, a file with the same
 name but `.yml` extension will be used, if it exists.
 3. Otherwise, a `_json-context.yml` file in the same directory will be used, if it exists.
 
 If no context definition file is found after performing the previous 3 steps, then the file will
 be skipped.
@@ -34,15 +35,15 @@
 import sys
 import uuid
 from collections import deque
 from dataclasses import dataclass, field
 from datetime import datetime
 from os import scandir
 from pathlib import Path
-from typing import Union, Optional, Sequence, cast, Iterable
+from typing import Union, Optional, Sequence, cast, Iterable, Any
 
 import jq
 from jsonpath_ng.ext import parse as json_path_parse
 from jsonschema import validate as json_validate
 from pyld import jsonld
 from rdflib import Graph, DC, DCTERMS, SKOS, OWL, RDF, RDFS, XSD, DCAT
 from rdflib.namespace import Namespace, DefinedNamespace
@@ -134,15 +135,14 @@
 
 
 @dataclass
 class UpliftResult:
     input_file: Path = None
     uplifted_json: dict | list = None
     graph: Graph = None
-    expanded_jsonld: dict | list = None
     output_files: list[Path] = field(default_factory=list)
 
 
 def _document_loader(secure: bool = False,
                      url_whitelist: Optional[Union[Sequence, bool]] = None,
                      **kwargs):
     if url_whitelist is False:
@@ -241,16 +241,19 @@
 
     # Check if pre-transform necessary
     transform = context.get('transform')
     if transform:
         # Allow for transform lists to do sequential transformations
         if isinstance(transform, str):
             transform = (transform,)
-        for t in transform:
-            data_graph = json.loads(jq.compile(t).input(data_graph).text())
+        for i, t in enumerate(transform):
+            tranformed_txt = jq.compile(t).input(data_graph).text()
+            if logger.isEnabledFor(logging.DEBUG):
+                logger.debug('After transform %d:\n%s', i + 1, tranformed_txt)
+            data_graph = json.loads(tranformed_txt)
 
     # Add types
     types = context.get('types', {})
     for loc, type_list in types.items():
         items = json_path_parse(loc).find(data_graph)
         if isinstance(type_list, str):
             type_list = [type_list]
@@ -268,20 +271,22 @@
         if not loc or loc in ['.', '$']:
             global_context = val
         else:
             items = json_path_parse(loc).find(data_graph)
             for item in items:
                 item.value['@context'] = _get_injected_context(item.value, val, context_position)
 
-    if global_context or scoped_graph:
+    if (global_context and not isinstance(data_graph, dict)) or scoped_graph:
         return {
             '@context': _get_injected_context(data, global_context, context_position),
             '@graph': data_graph,
         }
     else:
+        if global_context:
+            data_graph['@context'] = _get_injected_context(data, global_context, context_position)
         return data_graph
 
 
 def _get_injected_context(node: dict, ctx: Union[dict, list] = None, position: str = 'before') -> Union[dict, list]:
     if not ctx:
         return node.get('@context')
 
@@ -308,15 +313,15 @@
     else:
         result = ctx
 
     return result
 
 
 def generate_graph(input_data: dict | list,
-                   context: dict | Sequence[dict] = None,
+                   context: dict[str, Any] | Sequence[dict] = None,
                    base: str | None = None,
                    fetch_timeout: int = 5,
                    fetch_url_whitelist: Sequence[str] | bool | None = None) -> UpliftResult:
     """
     Create a graph from an input JSON document and a YAML context definition file.
 
     :param input_data: input JSON data in dict or list format
@@ -364,18 +369,19 @@
                     if base:
                         break
             else:
                 # If not a list, just look @base up
                 base = jdoc_ld['@context'].get('@base')
     if base:
         options['base'] = base
+    if logger.isEnabledFor(logging.DEBUG):
+        logger.debug('Uplifted JSON:\n%s', json.dumps(jdoc_ld, indent=2))
     g.parse(data=json.dumps(jdoc_ld), format='json-ld')
-    expanded = jsonld.expand(jdoc_ld, options)
 
-    return UpliftResult(graph=g, expanded_jsonld=expanded, uplifted_json=jdoc_ld)
+    return UpliftResult(graph=g, uplifted_json=jdoc_ld)
 
 
 def process_file(input_fn: str | Path,
                  jsonld_fn: str | Path | bool | None = False,
                  ttl_fn: str | Path | bool | None = False,
                  context_fn: str | Path | Sequence[str | Path] | None = None,
                  domain_cfg: DomainConfiguration | None = None,
@@ -444,14 +450,17 @@
         if not isinstance(input_filters, dict):
             raise ValueError('input-filter must be an object')
         input_data = apply_input_filter(input_fn, input_filters)
     else:
         with open(input_fn, 'r') as j:
             input_data = json.load(j)
 
+    if logger.isEnabledFor(logging.DEBUG):
+        logger.debug('Input data:\n%s', json.dumps(input_data, indent=2))
+
     provenance_metadata: ProvenanceMetadata | None = None
     if provenance_base_uri is not False:
         used = [FileProvenanceMetadata(filename=input_fn, mime_type='application/json')]
         used.extend(FileProvenanceMetadata(filename=c, mime_type='application/yaml') for c in provenance_contexts)
         provenance_metadata = ProvenanceMetadata(
             used=used,
             batch_activity_id=provenance_process_id,
@@ -468,15 +477,15 @@
                                    fetch_url_whitelist=fetch_url_whitelist)
 
     uplift_result.input_file = input_fn
 
     # False = do not generate
     # None = auto filename
     # - = stdout
-    if ttl_fn or ttl_fn is None:
+    if ttl_fn is not False:
         if ttl_fn == '-':
             if provenance_metadata:
                 provenance_metadata.output = FileProvenanceMetadata(mime_type='text/turtle', use_bnode=False)
                 generate_provenance(uplift_result.graph, provenance_metadata)
             print(uplift_result.graph.serialize(format='ttl'))
         else:
             if not ttl_fn:
@@ -490,36 +499,25 @@
                 generate_provenance(uplift_result.graph, provenance_metadata)
             uplift_result.graph.serialize(destination=ttl_fn, format='ttl')
             uplift_result.output_files.append(ttl_fn)
 
     # False = do not generate
     # None = auto filename
     # "-" = stdout
-    if jsonld_fn or jsonld_fn is None:
+    if jsonld_fn is not False:
         if jsonld_fn == '-':
-            if provenance_metadata:
-                provenance_metadata.generated = FileProvenanceMetadata(mime_type='application/ld+json', use_bnode=False)
-                uplift_result.expanded_jsonld = add_jsonld_provenance(uplift_result.expanded_jsonld,
-                                                                      provenance_metadata)
-            print(uplift_result.expanded_jsonld)
+            print(json.dumps(uplift_result.uplifted_json, indent=2))
         else:
             if not jsonld_fn:
                 jsonld_fn = input_fn.with_suffix('.jsonld') \
                     if input_fn.suffix != '.jsonld' \
                     else input_fn.with_suffix(input_fn.suffix + '.jsonld')
-            if provenance_metadata:
-                provenance_metadata.generated = FileProvenanceMetadata(
-                    filename=jsonld_fn,
-                    mime_type='application/ld+json',
-                    use_bnode=False,
-                )
-                uplift_result.expanded_jsonld = add_jsonld_provenance(uplift_result.expanded_jsonld,
-                                                                      provenance_metadata)
+
             with open(jsonld_fn, 'w') as f:
-                json.dump(uplift_result.expanded_jsonld, f, indent=2)
+                json.dump(uplift_result.uplifted_json, f, indent=2)
             uplift_result.output_files.append(jsonld_fn)
 
     return uplift_result
 
 
 def find_contexts(filename: Path | str,
                   domain_config: DomainConfiguration | None = None) -> list[Path | str] | None:
@@ -668,14 +666,15 @@
                     ttl_fn=False if ttl_fn is False else None,
                     context_fn=None,
                     base=base,
                     provenance_base_uri=provenance_base_uri,
                     provenance_process_id=process_id,
                     fetch_timeout=fetch_timeout,
                     fetch_url_whitelist=fetch_url_whitelist,
+                    domain_cfg=domain_cfg,
                 ))
             except Exception as e:
                 if skip_on_missing_context:
                     logger.warning("Error processing JSON/JSON-LD file, skipping: %s", getattr(e, 'msg', str(e)))
                 else:
                     raise
     else:
@@ -687,14 +686,15 @@
                     ttl_fn=ttl_fn if ttl_fn is not None else '-',
                     context_fn=context_fn,
                     base=base,
                     provenance_base_uri=provenance_base_uri,
                     provenance_process_id=process_id,
                     fetch_timeout=fetch_timeout,
                     fetch_url_whitelist=fetch_url_whitelist,
+                    domain_cfg=domain_cfg,
                 ))
             except Exception as e:
                 if skip_on_missing_context:
                     logger.warning("Error processing JSON/JSON-LD file, skipping: %s", getattr(e, 'msg', str(e)))
                 else:
                     raise
 
@@ -785,25 +785,42 @@
 
     parser.add_argument(
         '--use-git-status',
         action='store_true',
         help='Use git status for obtaining batch filenames'
     )
 
+    parser.add_argument(
+        '--debug',
+        action='store_true',
+        help='Enable debug mode'
+    )
+
+    parser.add_argument(
+        '--work-dir',
+        help='Set root directory for globs in domain configurations'
+    )
+
     args = parser.parse_args()
 
     if args.domain_config:
-        domain_cfg = DomainConfiguration(args.domain_config)
+        domain_cfg = DomainConfiguration(args.domain_config, args.work_dir)
     else:
         domain_cfg = None
 
     input_files = args.input
     if args.batch and args.use_git_status:
         git_status = util.git_status()
         input_files = git_status['added'] + git_status['modified'] + [r[1] for r in git_status['renamed']]
+    elif not input_files:
+        print("Error: no input files provided")
+        sys.exit(1)
+
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
 
     result = process(input_files,
                      context_fn=args.context,
                      domain_cfg=domain_cfg,
                      jsonld_fn=args.json_ld_file if args.json_ld else False,
                      ttl_fn=args.ttl_file if args.ttl else False,
                      batch=args.batch,
```

### Comparing `ogc_na-0.1.6/ogc/na/input_filters/csv.py` & `ogc_na-0.2.0/ogc/na/input_filters/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,29 +32,36 @@
     'delimiter': ',',
     'quotechar': '"',
     'skip-empty-rows': True,
     'trim-values': False,
 }
 
 
-def apply_filter(content: bytes, conf: dict[str, Any] | None) -> dict[str, Any] | list:
+def apply_filter(content: bytes, conf: dict[str, Any] | None) -> tuple[dict[str, Any] | list, dict[str, Any] | None]:
     conf = util.deep_update(DEFAULT_CONF, conf) if conf else DEFAULT_CONF
 
+    metadata = {
+        'filter': {
+            'conf': conf,
+        },
+    }
+
     textio = StringIO(content.decode('utf-8'))
     reader = csv.reader(textio, delimiter=conf['delimiter'], quotechar=conf['quotechar'])
 
     headers = None
     if conf['rows'] == 'dict':
         header_row = max(conf['header-row'], 0)
         # Skip to header row
         for i in range(header_row):
             next(reader, None)
         headers = next(reader, [])
         if not headers:
-            return []
+            return [], None
+        metadata['headers'] = headers
 
     # Skip requested rows
     for i in range(conf['skip-rows']):
         next(reader, None)
 
     result = []
     for row in reader:
@@ -64,8 +71,8 @@
         if conf['trim-values']:
             row = [v.strip() for v in row]
         if conf['rows'] == 'list':
             result.append(row)
         else:
             result.append(dict(zip(headers, row)))
 
-    return result
+    return result, metadata
```

### Comparing `ogc_na-0.1.6/ogc/na/profile.py` & `ogc_na-0.2.0/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/ogc/na/provenance.py` & `ogc_na-0.2.0/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/ogc/na/update_vocabs.py` & `ogc_na-0.2.0/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/ogc/na/util.py` & `ogc_na-0.2.0/ogc/na/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,19 +228,21 @@
             key_to_remove = min(self._last_access, key=self._last_access.get)
             del self._cache[key_to_remove]
             del self._last_access[key_to_remove]
         self._cache[key] = value
         self._last_access[key] = time()
 
 
-def deep_update(orig_dict: dict, with_dict: dict, replace: bool = False) -> dict:
+def deep_update(orig_dict: dict, with_dict: Mapping, replace: bool = False) -> dict:
+    if not isinstance(orig_dict, Mapping):
+        return with_dict
     dest = orig_dict if replace else {**orig_dict}
     for k, v in with_dict.items():
         if isinstance(v, Mapping):
-            dest[k] = deep_update(orig_dict.get(k, {}), with_dict, replace)
+            dest[k] = deep_update(orig_dict.get(k, {}), v, replace)
         else:
             dest[k] = v
     return dest
 
 
 def git_status(repo_path: str | Path = '.'):
     repo = git.Repo(repo_path)
@@ -249,15 +251,15 @@
     deleted = []
     renamed = []
     for diff in repo.head.commit.diff(None):
         if diff.change_type == 'D':
             deleted.append(diff.a_path)
         elif diff.change_type == 'M':
             modified.append(diff.a_path)
-        elif diff.chhange_type == 'R':
+        elif diff.change_type == 'R':
             renamed.append((diff.a_path, diff.b_path))
     return {
         'added': added,
         'modified': modified,
         'deleted': deleted,
         'renamed': renamed,
     }
```

### Comparing `ogc_na-0.1.6/ogc/na/validation.py` & `ogc_na-0.2.0/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.2.0/ogc_na.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.1.6
+Version: 0.2.0
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.6/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.2.0/ogc_na.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/pyproject.toml` & `ogc_na-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/rdf/domaincfg.vocab.ttl` & `ogc_na-0.2.0/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/test/data/headers.csv` & `ogc_na-0.2.0/test/data/headers.csv`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/test/data/uplift_context_valid.yml` & `ogc_na-0.2.0/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/test/test_annotate_schema.py` & `ogc_na-0.2.0/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/test/test_ingest_json.py` & `ogc_na-0.2.0/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/test/test_input_filters_csv.py` & `ogc_na-0.2.0/test/test_input_filters_csv.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.6/test/test_profile.py` & `ogc_na-0.2.0/test/test_profile.py`

 * *Files identical despite different names*

