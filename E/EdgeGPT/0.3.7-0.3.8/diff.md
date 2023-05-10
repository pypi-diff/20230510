# Comparing `tmp/EdgeGPT-0.3.7.tar.gz` & `tmp/EdgeGPT-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.3.7.tar", last modified: Tue May  9 15:17:39 2023, max compression
+gzip compressed data, was "EdgeGPT-0.3.8.tar", last modified: Wed May 10 05:53:50 2023, max compression
```

## Comparing `EdgeGPT-0.3.7.tar` & `EdgeGPT-0.3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-09 15:17:01.000000 EdgeGPT-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-09 15:17:01.000000 EdgeGPT-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 15:17:39.477652 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-09 15:17:39.000000 EdgeGPT-0.3.7/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30099 2023-05-09 15:17:01.000000 EdgeGPT-0.3.7/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 15:17:01.000000 EdgeGPT-0.3.7/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:50.322965 EdgeGPT-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-10 05:53:19.000000 EdgeGPT-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-10 05:53:50.322965 EdgeGPT-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-10 05:53:50.000000 EdgeGPT-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 05:53:50.322965 EdgeGPT-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-10 05:53:19.000000 EdgeGPT-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:50.318965 EdgeGPT-0.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 05:53:50.318965 EdgeGPT-0.3.8/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-10 05:53:50.000000 EdgeGPT-0.3.8/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 05:53:50.000000 EdgeGPT-0.3.8/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 05:53:50.000000 EdgeGPT-0.3.8/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 05:53:50.000000 EdgeGPT-0.3.8/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 05:53:50.000000 EdgeGPT-0.3.8/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 05:53:50.000000 EdgeGPT-0.3.8/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29675 2023-05-10 05:53:19.000000 EdgeGPT-0.3.8/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-10 05:53:19.000000 EdgeGPT-0.3.8/src/ImageGen.py
```

### Comparing `EdgeGPT-0.3.7/LICENSE` & `EdgeGPT-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.7/PKG-INFO` & `EdgeGPT-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.7
+Version: 0.3.8
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.7 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.8 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.7/README.md` & `EdgeGPT-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.3.7/setup.py` & `EdgeGPT-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT",
-    version="0.3.7",
+    version="0.3.8",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
```

### Comparing `EdgeGPT-0.3.7/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.3.8/src/EdgeGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.3.7
+Version: 0.3.8
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.7 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.3.8 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `EdgeGPT-0.3.7/src/EdgeGPT.py` & `EdgeGPT-0.3.8/src/EdgeGPT.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,27 +507,16 @@
                             for item in cookies:
                                 if item["name"] == "_U":
                                     U = item["value"]
                             async with ImageGenAsync(U, True) as image_generator:
                                 images = await image_generator.get_images(
                                     response["arguments"][0]["messages"][0]["text"],
                                 )
-                            cache = resp_txt
-                            resp_txt = (
-                                cache
-                                + "\n![image0]("
-                                + images[0]
-                                + ")\n![image1]("
-                                + images[1]
-                                + ")\n![image0]("
-                                + images[2]
-                                + ")\n![image3]("
-                                + images[3]
-                                + ")"
-                            )
+                            for i, image in enumerate(images):
+                                resp_txt = resp_txt + f"\n![image{i}]({image})"
                             draw = True
                         if (
                             response["arguments"][0]["messages"][0]["contentOrigin"]
                             != "Apology"
                         ) and not draw:
                             resp_txt = result_text + response["arguments"][0][
                                 "messages"
```

