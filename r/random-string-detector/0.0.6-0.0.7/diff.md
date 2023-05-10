# Comparing `tmp/random_string_detector-0.0.6.tar.gz` & `tmp/random_string_detector-0.0.7.tar.gz`

## Comparing `random_string_detector-0.0.6.tar` & `random_string_detector-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/setup.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.idea/.gitignore
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.idea/modules.xml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.idea/random-string-detector.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.idea/vcs.xml
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.idea/workspace.xml
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/random_string_detector/__init__.py
--rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/random_string_detector/random_string_detector.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/LICENSE
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 random_string_detector-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/setup.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.idea/.gitignore
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.idea/modules.xml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.idea/random-string-detector.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.idea/vcs.xml
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.idea/workspace.xml
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/random_string_detector/__init__.py
+-rw-r--r--   0        0        0    24145 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/random_string_detector/random_string_detector.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/README.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 random_string_detector-0.0.7/PKG-INFO
```

### Comparing `random_string_detector-0.0.6/.DS_Store` & `random_string_detector-0.0.7/.DS_Store`

 * *Files identical despite different names*

### Comparing `random_string_detector-0.0.6/.idea/workspace.xml` & `random_string_detector-0.0.7/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `random_string_detector-0.0.6/.idea/workspace.xml` & `random_string_detector-0.0.7/.idea/workspace.xml`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="f5ecef9d-00fa-4204-9c00-c6d0a944b6c1" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
```

### Comparing `random_string_detector-0.0.6/.idea/inspectionProfiles/Project_Default.xml` & `random_string_detector-0.0.7/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `random_string_detector-0.0.6/random_string_detector/random_string_detector.py` & `random_string_detector-0.0.7/random_string_detector/random_string_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,15 +673,15 @@
         "qk": 0.0,
         "qy": 0.0,
         "qz": 0.0,
         "wq": 0.0,
         "wz": 0.0
     }
 
-def is_random_string(word, threshold):
+def is_random_string(word, threshold=0.1):
     # Allow only words longer than 3 characters which contains only English alphabetic characters
     if len(word) < 4 or not word.isalpha():
         return False
 
     # Turn word into lowercase
     word = word.lower()
 
@@ -696,11 +696,8 @@
     num_common_bigrams = sum(1 for bigram in bigrams if en_bigrams_dict.get(bigram, 0) > threshold)
     num_uncommon_bigrams = len(bigrams) - num_common_bigrams
 
     # Higher number wins
     if num_common_bigrams > num_uncommon_bigrams:
         return False
     else:
-        return True
-
-def is_random_string(word):
-    return is_random_string(word, 0.1)
+        return True
```

### Comparing `random_string_detector-0.0.6/.gitignore` & `random_string_detector-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `random_string_detector-0.0.6/LICENSE` & `random_string_detector-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `random_string_detector-0.0.6/README.md` & `random_string_detector-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `random_string_detector-0.0.6/pyproject.toml` & `random_string_detector-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "random-string-detector"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Mehmed Kadric", email="kadricze@gmail.com" },
 ]
 description = "A package for random string detection"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `random_string_detector-0.0.6/PKG-INFO` & `random_string_detector-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random-string-detector
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for random string detection
 Project-URL: Homepage, https://github.com/mehmedkadric/random-string-detector
 Project-URL: Bug Tracker, https://github.com/mehmedkadric/random-string-detector/issues
 Author-email: Mehmed Kadric <kadricze@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

