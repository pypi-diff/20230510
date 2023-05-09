# Comparing `tmp/fastlmi-0.0.1.tar.gz` & `tmp/fastlmi-0.1.0.tar.gz`

## Comparing `fastlmi-0.0.1.tar` & `fastlmi-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,18 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastlmi-0.0.1/.gitattributes
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fastlmi-0.0.1/MANIFEST.in
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastlmi-0.0.1/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fastlmi-0.0.1/lmi/__init__.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 fastlmi-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 fastlmi-0.0.1/LICENSE
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastlmi-0.0.1/README.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastlmi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 fastlmi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastlmi-0.1.0/.gitattributes
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastlmi-0.1.0/CITATION.cff
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastlmi-0.1.0/requirements.txt
+-rw-r--r--   0        0        0   145438 2020-02-02 00:00:00.000000 fastlmi-0.1.0/assets/oai_dice_roller.png
+-rw-r--r--   0        0        0    22019 2020-02-02 00:00:00.000000 fastlmi-0.1.0/assets/oai_found_plugin.png
+-rw-r--r--   0        0        0    35758 2020-02-02 00:00:00.000000 fastlmi-0.1.0/assets/oai_manifest.png
+-rw-r--r--   0        0        0    33188 2020-02-02 00:00:00.000000 fastlmi-0.1.0/assets/oai_select_plugins.png
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 fastlmi-0.1.0/examples/dice_roller.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/__init__.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/application.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/openai/__init__.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 fastlmi-0.1.0/fastlmi/openai/models.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 fastlmi-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 fastlmi-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 fastlmi-0.1.0/README.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 fastlmi-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 fastlmi-0.1.0/PKG-INFO
```

### Comparing `fastlmi-0.0.1/.gitignore` & `fastlmi-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastlmi-0.0.1/LICENSE` & `fastlmi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastlmi-0.0.1/pyproject.toml` & `fastlmi-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastlmi"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
     { name = "Andrew Zhu", email = "andrew@zhu.codes" },
 ]
 description = "A FastAPI-based framework for quickly building and iterating on language model interfaces."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     # https://pypi.org/classifiers/
-    "Development Status :: 1 - Planning",
+    "Development Status :: 2 - Pre-Alpha",
     "Framework :: FastAPI",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
```

