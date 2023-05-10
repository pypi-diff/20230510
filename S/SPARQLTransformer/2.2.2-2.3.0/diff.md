# Comparing `tmp/SPARQLTransformer-2.2.2.tar.gz` & `tmp/SPARQLTransformer-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPARQLTransformer-2.2.2.tar", last modified: Wed Feb 22 13:34:49 2023, max compression
+gzip compressed data, was "SPARQLTransformer-2.3.0.tar", last modified: Wed May 10 10:14:03 2023, max compression
```

## Comparing `SPARQLTransformer-2.2.2.tar` & `SPARQLTransformer-2.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pasquale   (501) staff       (20)        0 2023-02-22 13:34:49.201355 SPARQLTransformer-2.2.2/
--rw-r--r--   0 pasquale   (501) staff       (20)    11357 2023-01-19 14:36:05.000000 SPARQLTransformer-2.2.2/LICENSE
--rw-r--r--   0 pasquale   (501) staff       (20)     4089 2023-02-22 13:34:49.201222 SPARQLTransformer-2.2.2/PKG-INFO
--rw-r--r--   0 pasquale   (501) staff       (20)     3461 2023-02-08 11:00:43.000000 SPARQLTransformer-2.2.2/README.md
-drwxr-xr-x   0 pasquale   (501) staff       (20)        0 2023-02-22 13:34:49.201039 SPARQLTransformer-2.2.2/SPARQLTransformer.egg-info/
--rw-r--r--   0 pasquale   (501) staff       (20)     4089 2023-02-22 13:34:49.000000 SPARQLTransformer-2.2.2/SPARQLTransformer.egg-info/PKG-INFO
--rw-r--r--   0 pasquale   (501) staff       (20)      268 2023-02-22 13:34:49.000000 SPARQLTransformer-2.2.2/SPARQLTransformer.egg-info/SOURCES.txt
--rw-r--r--   0 pasquale   (501) staff       (20)        1 2023-02-22 13:34:49.000000 SPARQLTransformer-2.2.2/SPARQLTransformer.egg-info/dependency_links.txt
--rw-r--r--   0 pasquale   (501) staff       (20)       25 2023-02-22 13:34:49.000000 SPARQLTransformer-2.2.2/SPARQLTransformer.egg-info/requires.txt
--rw-r--r--   0 pasquale   (501) staff       (20)       18 2023-02-22 13:34:49.000000 SPARQLTransformer-2.2.2/SPARQLTransformer.egg-info/top_level.txt
--rw-r--r--   0 pasquale   (501) staff       (20)    19304 2023-02-22 13:33:52.000000 SPARQLTransformer-2.2.2/SPARQLTransformer.py
--rw-r--r--   0 pasquale   (501) staff       (20)       24 2023-01-19 14:36:05.000000 SPARQLTransformer-2.2.2/requirements.txt
--rw-r--r--   0 pasquale   (501) staff       (20)       38 2023-02-22 13:34:49.201393 SPARQLTransformer-2.2.2/setup.cfg
--rw-r--r--   0 pasquale   (501) staff       (20)     1247 2023-02-22 10:42:34.000000 SPARQLTransformer-2.2.2/setup.py
+drwxr-xr-x   0 pasquale   (501) staff       (20)        0 2023-05-10 10:14:03.303196 SPARQLTransformer-2.3.0/
+-rw-r--r--   0 pasquale   (501) staff       (20)    11357 2023-01-19 14:36:05.000000 SPARQLTransformer-2.3.0/LICENSE
+-rw-r--r--   0 pasquale   (501) staff       (20)     4089 2023-05-10 10:14:03.303083 SPARQLTransformer-2.3.0/PKG-INFO
+-rw-r--r--   0 pasquale   (501) staff       (20)     3461 2023-02-08 11:00:43.000000 SPARQLTransformer-2.3.0/README.md
+drwxr-xr-x   0 pasquale   (501) staff       (20)        0 2023-05-10 10:14:03.302904 SPARQLTransformer-2.3.0/SPARQLTransformer.egg-info/
+-rw-r--r--   0 pasquale   (501) staff       (20)     4089 2023-05-10 10:14:03.000000 SPARQLTransformer-2.3.0/SPARQLTransformer.egg-info/PKG-INFO
+-rw-r--r--   0 pasquale   (501) staff       (20)      268 2023-05-10 10:14:03.000000 SPARQLTransformer-2.3.0/SPARQLTransformer.egg-info/SOURCES.txt
+-rw-r--r--   0 pasquale   (501) staff       (20)        1 2023-05-10 10:14:03.000000 SPARQLTransformer-2.3.0/SPARQLTransformer.egg-info/dependency_links.txt
+-rw-r--r--   0 pasquale   (501) staff       (20)       25 2023-05-10 10:14:03.000000 SPARQLTransformer-2.3.0/SPARQLTransformer.egg-info/requires.txt
+-rw-r--r--   0 pasquale   (501) staff       (20)       18 2023-05-10 10:14:03.000000 SPARQLTransformer-2.3.0/SPARQLTransformer.egg-info/top_level.txt
+-rw-r--r--   0 pasquale   (501) staff       (20)    19675 2023-05-10 10:13:36.000000 SPARQLTransformer-2.3.0/SPARQLTransformer.py
+-rw-r--r--   0 pasquale   (501) staff       (20)       24 2023-01-19 14:36:05.000000 SPARQLTransformer-2.3.0/requirements.txt
+-rw-r--r--   0 pasquale   (501) staff       (20)       38 2023-05-10 10:14:03.303238 SPARQLTransformer-2.3.0/setup.cfg
+-rw-r--r--   0 pasquale   (501) staff       (20)     1247 2023-05-10 10:13:54.000000 SPARQLTransformer-2.3.0/setup.py
```

### Comparing `SPARQLTransformer-2.2.2/LICENSE` & `SPARQLTransformer-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SPARQLTransformer-2.2.2/PKG-INFO` & `SPARQLTransformer-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPARQLTransformer
-Version: 2.2.2
+Version: 2.3.0
 Summary: Write your SPARQL query directly in the JSON-LD you would like to have in output
 Home-page: https://github.com/D2KLab/py-sparql-transformer
 Author: Pasquale Lisena
 Author-email: pasquale.lisena@eurecom.fr
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/D2KLab/py-sparql-transformer/issues
 Project-URL: Documentation, https://github.com/D2KLab/py-sparql-transformer
```

### Comparing `SPARQLTransformer-2.2.2/README.md` & `SPARQLTransformer-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SPARQLTransformer-2.2.2/SPARQLTransformer.egg-info/PKG-INFO` & `SPARQLTransformer-2.3.0/SPARQLTransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPARQLTransformer
-Version: 2.2.2
+Version: 2.3.0
 Summary: Write your SPARQL query directly in the JSON-LD you would like to have in output
 Home-page: https://github.com/D2KLab/py-sparql-transformer
 Author: Pasquale Lisena
 Author-email: pasquale.lisena@eurecom.fr
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/D2KLab/py-sparql-transformer/issues
 Project-URL: Documentation, https://github.com/D2KLab/py-sparql-transformer
```

### Comparing `SPARQLTransformer-2.2.2/SPARQLTransformer.py` & `SPARQLTransformer-2.3.0/SPARQLTransformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,22 @@
                 fii_fun(key)
             if _is_empty_obj(variable):
                 instance.pop(k)
             elif obj_as_list:
                 instance[k] = [instance[k]]
             return
 
+        if isinstance(variable, list):
+            fii_fun = _fit_in(variable, line, options)
+            for i in range(len(variable)):
+                fii_fun(i)
+            if all(item is None for item in variable):
+                instance.pop(k)
+            return
+
         if not isinstance(variable, str):
             return
 
         if not variable.startswith('?'):
             return
 
         variable = variable[1:]
@@ -287,15 +295,18 @@
         if "$langTag:" in variable:
             temp = variable.split('$langTag:')
             variable = temp[0]
             langTag = temp[1]
 
         # variable not in result, delete from
         if variable not in line:
-            instance.pop(k)
+            if isinstance(instance, list):
+                instance[k] = None
+            else:
+                instance.pop(k)
         else:
             opt = options.copy()
             opt['accept'] = accept
             opt['langTag'] = langTag
             opt['list'] = asList
             instance[k] = _to_jsonld_value(line[variable], opt)
```

### Comparing `SPARQLTransformer-2.2.2/setup.py` & `SPARQLTransformer-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name="SPARQLTransformer",
-      version="2.2.2",
+      version="2.3.0",
       install_requires=requirements,
       data_files=[('txt', ['requirements.txt'])],
       py_modules=["SPARQLTransformer"],
 
       # metadata to display on PyPI
       author="Pasquale Lisena",
       author_email="pasquale.lisena@eurecom.fr",
```

