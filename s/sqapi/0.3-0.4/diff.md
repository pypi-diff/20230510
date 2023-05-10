# Comparing `tmp/sqapi-0.3.tar.gz` & `tmp/sqapi-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqapi-0.3.tar", last modified: Tue Apr 18 02:01:41 2023, max compression
+gzip compressed data, was "sqapi-0.4.tar", last modified: Wed May 10 02:47:17 2023, max compression
```

## Comparing `sqapi-0.3.tar` & `sqapi-0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 02:01:41.982992 sqapi-0.3/
--rw-r--r--   0 ariell     (501) staff       (20)     1061 2023-04-17 06:42:47.000000 sqapi-0.3/LICENSE.txt
--rw-r--r--   0 ariell     (501) staff       (20)     9086 2023-04-18 02:01:41.983075 sqapi-0.3/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)     8059 2023-04-18 01:38:47.000000 sqapi-0.3/README.md
--rw-r--r--   0 ariell     (501) staff       (20)       79 2023-04-18 02:01:41.983360 sqapi-0.3/setup.cfg
--rw-r--r--   0 ariell     (501) staff       (20)     1786 2023-04-18 02:00:20.000000 sqapi-0.3/setup.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 02:01:41.982159 sqapi-0.3/sqapi/
--rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.3/sqapi/__init__.py
--rw-r--r--   0 ariell     (501) staff       (20)    12681 2023-04-18 01:48:28.000000 sqapi-0.3/sqapi/annotate.py
--rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.3/sqapi/api.py
--rw-r--r--   0 ariell     (501) staff       (20)     4902 2023-04-18 01:29:24.000000 sqapi-0.3/sqapi/helpers.py
--rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.3/sqapi/media.py
--rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.3/sqapi/request.py
-drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-04-18 02:01:41.982895 sqapi-0.3/sqapi.egg-info/
--rw-r--r--   0 ariell     (501) staff       (20)     9086 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/PKG-INFO
--rw-r--r--   0 ariell     (501) staff       (20)      282 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/SOURCES.txt
--rw-r--r--   0 ariell     (501) staff       (20)        1 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/dependency_links.txt
--rw-r--r--   0 ariell     (501) staff       (20)       29 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/requires.txt
--rw-r--r--   0 ariell     (501) staff       (20)        6 2023-04-18 02:01:41.000000 sqapi-0.3/sqapi.egg-info/top_level.txt
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-10 02:47:17.233500 sqapi-0.4/
+-rw-r--r--   0 ariell     (501) staff       (20)     1061 2023-05-10 02:42:34.000000 sqapi-0.4/LICENSE.txt
+-rw-r--r--   0 ariell     (501) staff       (20)    10851 2023-05-10 02:47:17.233583 sqapi-0.4/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)     9824 2023-04-21 06:07:59.000000 sqapi-0.4/README.md
+-rw-r--r--   0 ariell     (501) staff       (20)       79 2023-05-10 02:47:17.233832 sqapi-0.4/setup.cfg
+-rw-r--r--   0 ariell     (501) staff       (20)     1786 2023-05-10 02:42:22.000000 sqapi-0.4/setup.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-10 02:47:17.232721 sqapi-0.4/sqapi/
+-rw-r--r--   0 ariell     (501) staff       (20)        0 2023-04-06 00:14:19.000000 sqapi-0.4/sqapi/__init__.py
+-rw-r--r--   0 ariell     (501) staff       (20)    12728 2023-05-10 02:42:22.000000 sqapi-0.4/sqapi/annotate.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4202 2023-04-07 04:44:10.000000 sqapi-0.4/sqapi/api.py
+-rw-r--r--   0 ariell     (501) staff       (20)     4902 2023-04-18 01:29:24.000000 sqapi-0.4/sqapi/helpers.py
+-rw-r--r--   0 ariell     (501) staff       (20)     1632 2022-05-09 04:38:36.000000 sqapi-0.4/sqapi/media.py
+-rw-r--r--   0 ariell     (501) staff       (20)     7454 2023-04-06 07:30:14.000000 sqapi-0.4/sqapi/request.py
+drwxr-xr-x   0 ariell     (501) staff       (20)        0 2023-05-10 02:47:17.233399 sqapi-0.4/sqapi.egg-info/
+-rw-r--r--   0 ariell     (501) staff       (20)    10851 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/PKG-INFO
+-rw-r--r--   0 ariell     (501) staff       (20)      282 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        1 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ariell     (501) staff       (20)       29 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/requires.txt
+-rw-r--r--   0 ariell     (501) staff       (20)        6 2023-05-10 02:47:17.000000 sqapi-0.4/sqapi.egg-info/top_level.txt
```

### Comparing `sqapi-0.3/LICENSE.txt` & `sqapi-0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqapi-0.3/PKG-INFO` & `sqapi-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqapi
-Version: 0.3
+Version: 0.4
 Summary: A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 Home-page: https://bitbucket.org/ariell/pysq
 Download-URL: https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz
 Author: Greybits Engineering
 License: MIT
 Keywords: SQUIDLE+,API,SQ,Machine Learning
 Classifier: Development Status :: 3 - Alpha
@@ -63,14 +63,63 @@
 html = r.execute().text              # perform the request & return result as text (eg: for html)
 ```
 
 > **IMPORTANT:** in order to proceed, you will need a user account on [SQUIDLE+](https://squidle.org). You will also 
 > need to activate your API key.
 
 ## Examples
+### Creating queries
+This is by no means an extensive list of possible API queries. The API is extensive and the models are documented
+[here](https://squidle.org/api/help?template=api_help_page.html) and the creation of queries is documented 
+[here](https://squidle.org/api/help?template=api_help_page.html#api_query). `SQAPI` enables a convenient mechanism 
+for creating these queries inside of Python. For example, a basic API query to list the 
+
+`# /api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}`
+```json
+{
+   "filters": [
+      {
+         "name": "point",
+         "op": "has",
+         "val": {
+            "name": "has_xy",
+            "op": "eq",
+            "val": true
+         }
+      },
+      {
+         "name": "point",
+         "op": "has",
+         "val": {
+            "name": "media",
+            "op": "has",
+            "val": {
+               "name": "poses",
+               "op": "any",
+               "val": {
+                  "name": "geom",
+                  "op": "geo_in_bbox",
+                  "val": [
+                     {
+                        "lat": -32.020013585799155,
+                        "lon": 115.49980113118502
+                     },
+                     {
+                        "lat": -32.01995006531625,
+                        "lon": 115.49987604949759
+                     }
+                  ]
+               }
+            }
+         }
+      }
+   ]
+}
+```
+
 ### Random annotation BOT
 This is an example of an automated labelling bot that selects random class labels to assign to points.
 It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
 Machine Learning algorithm for label suggestions.
 
 Set up the environment and a mini project
 ```shell
```

### Comparing `sqapi-0.3/README.md` & `sqapi-0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -41,14 +41,63 @@
 html = r.execute().text              # perform the request & return result as text (eg: for html)
 ```
 
 > **IMPORTANT:** in order to proceed, you will need a user account on [SQUIDLE+](https://squidle.org). You will also 
 > need to activate your API key.
 
 ## Examples
+### Creating queries
+This is by no means an extensive list of possible API queries. The API is extensive and the models are documented
+[here](https://squidle.org/api/help?template=api_help_page.html) and the creation of queries is documented 
+[here](https://squidle.org/api/help?template=api_help_page.html#api_query). `SQAPI` enables a convenient mechanism 
+for creating these queries inside of Python. For example, a basic API query to list the 
+
+`# /api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}`
+```json
+{
+   "filters": [
+      {
+         "name": "point",
+         "op": "has",
+         "val": {
+            "name": "has_xy",
+            "op": "eq",
+            "val": true
+         }
+      },
+      {
+         "name": "point",
+         "op": "has",
+         "val": {
+            "name": "media",
+            "op": "has",
+            "val": {
+               "name": "poses",
+               "op": "any",
+               "val": {
+                  "name": "geom",
+                  "op": "geo_in_bbox",
+                  "val": [
+                     {
+                        "lat": -32.020013585799155,
+                        "lon": 115.49980113118502
+                     },
+                     {
+                        "lat": -32.01995006531625,
+                        "lon": 115.49987604949759
+                     }
+                  ]
+               }
+            }
+         }
+      }
+   ]
+}
+```
+
 ### Random annotation BOT
 This is an example of an automated labelling bot that selects random class labels to assign to points.
 It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
 Machine Learning algorithm for label suggestions.
 
 Set up the environment and a mini project
 ```shell
```

### Comparing `sqapi-0.3/setup.py` & `sqapi-0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sqapi',
-    version='0.3',
+    version='0.4',
     packages=['sqapi'],
     install_requires=['requests', 'numpy', 'opencv-python'],
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.',   # Give a short description about your library
     author='Greybits Engineering',                   # Type in your name
```

### Comparing `sqapi-0.3/sqapi/annotate.py` & `sqapi-0.4/sqapi/annotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 if self.email_results if email_results is None else email_results:
                     self.email_annotation_set_user(a, media_count, point_count, annotation_count)
             except Exception as e:
                 print(traceback.format_exc())
 
         # paginate annotation_sets, if more than one page returned
         if annotation_sets.get("page") < annotation_sets.get("total_pages"):
-            self.run(page=page+1, results_per_page=results_per_page, email_results=email_results)
+            self.run(annotation_set_request=annotation_set_request, page=page+1, results_per_page=results_per_page, email_results=email_results)
 
     def process_annotation_set(self, annotation_set_data):
         """
 
         :param annotation_set_data:
         :return:
         """
```

### Comparing `sqapi-0.3/sqapi/api.py` & `sqapi-0.4/sqapi/api.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.3/sqapi/helpers.py` & `sqapi-0.4/sqapi/helpers.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.3/sqapi/media.py` & `sqapi-0.4/sqapi/media.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.3/sqapi/request.py` & `sqapi-0.4/sqapi/request.py`

 * *Files identical despite different names*

### Comparing `sqapi-0.3/sqapi.egg-info/PKG-INFO` & `sqapi-0.4/sqapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqapi
-Version: 0.3
+Version: 0.4
 Summary: A python package that simplifies interactions with the SQUIDLE+ API. It can be used to integrate automated labelling from machine learning algorithms and plenty other cool things.
 Home-page: https://bitbucket.org/ariell/pysq
 Download-URL: https://bitbucket.org/ariell/pysq/get/bede6badfc1ea09cd45b3ae3d4bc3551daa0b3e0.tar.gz
 Author: Greybits Engineering
 License: MIT
 Keywords: SQUIDLE+,API,SQ,Machine Learning
 Classifier: Development Status :: 3 - Alpha
@@ -63,14 +63,63 @@
 html = r.execute().text              # perform the request & return result as text (eg: for html)
 ```
 
 > **IMPORTANT:** in order to proceed, you will need a user account on [SQUIDLE+](https://squidle.org). You will also 
 > need to activate your API key.
 
 ## Examples
+### Creating queries
+This is by no means an extensive list of possible API queries. The API is extensive and the models are documented
+[here](https://squidle.org/api/help?template=api_help_page.html) and the creation of queries is documented 
+[here](https://squidle.org/api/help?template=api_help_page.html#api_query). `SQAPI` enables a convenient mechanism 
+for creating these queries inside of Python. For example, a basic API query to list the 
+
+`# /api/annotation?template=models/annotation/list_thumbnails.html&q={"filters":[{"name":"point","op":"has","val":{"name":"has_xy","op":"eq","val":true}},{"name":"point","op":"has","val":{"name":"media","op":"has","val":{"name":"poses","op":"any","val":{"name":"geom","op":"geo_in_bbox","val":[{"lat":-32.020013585799155,"lon":115.49980113118502},{"lat":-32.01995006531625,"lon":115.49987604949759}]}}}}]}`
+```json
+{
+   "filters": [
+      {
+         "name": "point",
+         "op": "has",
+         "val": {
+            "name": "has_xy",
+            "op": "eq",
+            "val": true
+         }
+      },
+      {
+         "name": "point",
+         "op": "has",
+         "val": {
+            "name": "media",
+            "op": "has",
+            "val": {
+               "name": "poses",
+               "op": "any",
+               "val": {
+                  "name": "geom",
+                  "op": "geo_in_bbox",
+                  "val": [
+                     {
+                        "lat": -32.020013585799155,
+                        "lon": 115.49980113118502
+                     },
+                     {
+                        "lat": -32.01995006531625,
+                        "lon": 115.49987604949759
+                     }
+                  ]
+               }
+            }
+         }
+      }
+   ]
+}
+```
+
 ### Random annotation BOT
 This is an example of an automated labelling bot that selects random class labels to assign to points.
 It provides terrible suggestions, however it provides a simple boiler-plate example of how to integrate a
 Machine Learning algorithm for label suggestions.
 
 Set up the environment and a mini project
 ```shell
```

