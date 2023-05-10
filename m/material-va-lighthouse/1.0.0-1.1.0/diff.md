# Comparing `tmp/material-va-lighthouse-1.0.0.tar.gz` & `tmp/material-va-lighthouse-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material-va-lighthouse-1.0.0.tar", last modified: Mon Apr 17 21:22:11 2023, max compression
+gzip compressed data, was "material-va-lighthouse-1.1.0.tar", last modified: Wed May 10 19:27:22 2023, max compression
```

## Comparing `material-va-lighthouse-1.0.0.tar` & `material-va-lighthouse-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-04-17 21:22:11.447237 material-va-lighthouse-1.0.0/
--rw-r--r--   0 alastairdawson   (501) staff       (20)     1327 2023-04-17 16:55:34.000000 material-va-lighthouse-1.0.0/LICENSE
--rw-r--r--   0 alastairdawson   (501) staff       (20)      267 2023-04-17 21:22:11.447104 material-va-lighthouse-1.0.0/PKG-INFO
--rw-r--r--   0 alastairdawson   (501) staff       (20)      802 2023-04-17 20:26:59.000000 material-va-lighthouse-1.0.0/README.md
-drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-04-17 21:22:11.445473 material-va-lighthouse-1.0.0/material_va_lighthouse/
--rw-r--r--   0 alastairdawson   (501) staff       (20)        0 2023-04-17 18:42:27.000000 material-va-lighthouse-1.0.0/material_va_lighthouse/__init__.py
--rw-r--r--   0 alastairdawson   (501) staff       (20)      915 2023-04-17 20:01:49.000000 material-va-lighthouse-1.0.0/material_va_lighthouse/plugin.py
--rw-r--r--   0 alastairdawson   (501) staff       (20)     1099 2023-04-17 00:21:55.000000 material-va-lighthouse-1.0.0/material_va_lighthouse/va_lighthouse.css
--rw-r--r--   0 alastairdawson   (501) staff       (20)     3180 2023-04-17 00:24:19.000000 material-va-lighthouse-1.0.0/material_va_lighthouse/va_lighthouse_logo.png
-drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-04-17 21:22:11.446902 material-va-lighthouse-1.0.0/material_va_lighthouse.egg-info/
--rw-r--r--   0 alastairdawson   (501) staff       (20)      267 2023-04-17 21:22:11.000000 material-va-lighthouse-1.0.0/material_va_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 alastairdawson   (501) staff       (20)      459 2023-04-17 21:22:11.000000 material-va-lighthouse-1.0.0/material_va_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)        1 2023-04-17 21:22:11.000000 material-va-lighthouse-1.0.0/material_va_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)       99 2023-04-17 21:22:11.000000 material-va-lighthouse-1.0.0/material_va_lighthouse.egg-info/entry_points.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)       23 2023-04-17 21:22:11.000000 material-va-lighthouse-1.0.0/material_va_lighthouse.egg-info/requires.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)       23 2023-04-17 21:22:11.000000 material-va-lighthouse-1.0.0/material_va_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 alastairdawson   (501) staff       (20)       38 2023-04-17 21:22:11.447290 material-va-lighthouse-1.0.0/setup.cfg
--rw-r--r--   0 alastairdawson   (501) staff       (20)      708 2023-04-17 20:15:31.000000 material-va-lighthouse-1.0.0/setup.py
+drwxr-xr-x   0 alastair   (501) staff       (20)        0 2023-05-10 19:27:22.430939 material-va-lighthouse-1.1.0/
+-rw-r--r--   0 alastair   (501) staff       (20)     1327 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/LICENSE
+-rw-r--r--   0 alastair   (501) staff       (20)      267 2023-05-10 19:27:22.430666 material-va-lighthouse-1.1.0/PKG-INFO
+-rw-r--r--   0 alastair   (501) staff       (20)      877 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/README.md
+drwxr-xr-x   0 alastair   (501) staff       (20)        0 2023-05-10 19:27:22.399261 material-va-lighthouse-1.1.0/material_va_lighthouse/
+-rw-r--r--   0 alastair   (501) staff       (20)        0 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/material_va_lighthouse/__init__.py
+-rw-r--r--   0 alastair   (501) staff       (20)      915 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/material_va_lighthouse/plugin.py
+-rw-r--r--   0 alastair   (501) staff       (20)     1099 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/material_va_lighthouse/va_lighthouse.css
+-rw-r--r--   0 alastair   (501) staff       (20)     3180 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/material_va_lighthouse/va_lighthouse_logo.png
+drwxr-xr-x   0 alastair   (501) staff       (20)        0 2023-05-10 19:27:22.430154 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/
+-rw-r--r--   0 alastair   (501) staff       (20)      267 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 alastair   (501) staff       (20)      459 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 alastair   (501) staff       (20)        1 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 alastair   (501) staff       (20)       99 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/entry_points.txt
+-rw-r--r--   0 alastair   (501) staff       (20)       44 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/requires.txt
+-rw-r--r--   0 alastair   (501) staff       (20)       23 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 alastair   (501) staff       (20)       38 2023-05-10 19:27:22.431022 material-va-lighthouse-1.1.0/setup.cfg
+-rw-r--r--   0 alastair   (501) staff       (20)      740 2023-05-10 19:26:33.000000 material-va-lighthouse-1.1.0/setup.py
```

### Comparing `material-va-lighthouse-1.0.0/LICENSE` & `material-va-lighthouse-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.0.0/README.md` & `material-va-lighthouse-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 ## Installation
 Open a terminal and run the following command:
 
 ```bash
 pip install material-va-lighthouse
 ```
 
-Update your `mkdocs.yml` under the `theme` section set `material` as your theme (if you're not already) 
+Update your `mkdocs.yml` to include the plugin:
+
+```yaml
+plugins:
+  - material-va-lighthouse
+```
+
+Update the `theme` section. Set `material` as your theme (if you're not already) 
 and point the logo to the Lighthouse logo from this plugin:
 
 
 ```yaml
 theme:
   name: material
   logo: 'assets/images/va_lighthouse_logo.png'
```

### Comparing `material-va-lighthouse-1.0.0/material_va_lighthouse/plugin.py` & `material-va-lighthouse-1.1.0/material_va_lighthouse/plugin.py`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.0.0/material_va_lighthouse/va_lighthouse.css` & `material-va-lighthouse-1.1.0/material_va_lighthouse/va_lighthouse.css`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.0.0/material_va_lighthouse/va_lighthouse_logo.png` & `material-va-lighthouse-1.1.0/material_va_lighthouse/va_lighthouse_logo.png`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.0.0/setup.py` & `material-va-lighthouse-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="material-va-lighthouse",
-    version="1.0.0",
+    version="1.1.0",
     description="A MKDocs plugin which extends the material theme with styles from the VA design system",
     author="Alastair Dawson",
     author_email="alastair.j.dawson@gmail.com",
     license="CC0 1.0",
     packages=find_packages(),
     include_package_data=True,
     package_data={"material_va_lighthouse": ["va_lighthouse.css", "va_lighthouse_logo.png"]},
     install_requires=[
         "mkdocs",
         "mkdocs-material",
+        "mkdocs-techdocs-core",
     ],
     entry_points={
         "mkdocs.plugins": [
             "material-va-lighthouse = material_va_lighthouse.plugin:MaterialVALighthousePlugin"
         ],
     },
 )
```

