# Comparing `tmp/concordia-harmony-0.1.5.tar.gz` & `tmp/concordia-harmony-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concordia-harmony-0.1.5.tar", last modified: Tue May  9 00:27:16 2023, max compression
+gzip compressed data, was "concordia-harmony-1.0.0.tar", last modified: Tue May  9 22:00:37 2023, max compression
```

## Comparing `concordia-harmony-0.1.5.tar` & `concordia-harmony-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:27:16.649794 concordia-harmony-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 00:27:07.000000 concordia-harmony-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-09 00:27:16.649794 concordia-harmony-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-09 00:27:07.000000 concordia-harmony-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-09 00:27:07.000000 concordia-harmony-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:27:16.649794 concordia-harmony-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:27:16.649794 concordia-harmony-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:27:16.649794 concordia-harmony-0.1.5/src/concordia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:27:07.000000 concordia-harmony-0.1.5/src/concordia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-09 00:27:07.000000 concordia-harmony-0.1.5/src/concordia/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-09 00:27:07.000000 concordia-harmony-0.1.5/src/concordia/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-09 00:27:07.000000 concordia-harmony-0.1.5/src/concordia/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:27:16.649794 concordia-harmony-0.1.5/src/concordia_harmony.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-09 00:27:16.000000 concordia-harmony-0.1.5/src/concordia_harmony.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-09 00:27:16.000000 concordia-harmony-0.1.5/src/concordia_harmony.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:27:16.000000 concordia-harmony-0.1.5/src/concordia_harmony.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 00:27:16.000000 concordia-harmony-0.1.5/src/concordia_harmony.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 00:27:16.000000 concordia-harmony-0.1.5/src/concordia_harmony.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:00:37.664795 concordia-harmony-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 22:00:29.000000 concordia-harmony-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-09 22:00:37.664795 concordia-harmony-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-09 22:00:29.000000 concordia-harmony-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-09 22:00:29.000000 concordia-harmony-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:00:37.664795 concordia-harmony-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:00:37.664795 concordia-harmony-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:00:37.664795 concordia-harmony-1.0.0/src/concordia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 22:00:29.000000 concordia-harmony-1.0.0/src/concordia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-09 22:00:29.000000 concordia-harmony-1.0.0/src/concordia/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-09 22:00:29.000000 concordia-harmony-1.0.0/src/concordia/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-09 22:00:29.000000 concordia-harmony-1.0.0/src/concordia/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:00:37.664795 concordia-harmony-1.0.0/src/concordia_harmony.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-09 22:00:37.000000 concordia-harmony-1.0.0/src/concordia_harmony.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-09 22:00:37.000000 concordia-harmony-1.0.0/src/concordia_harmony.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:00:37.000000 concordia-harmony-1.0.0/src/concordia_harmony.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 22:00:37.000000 concordia-harmony-1.0.0/src/concordia_harmony.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 22:00:37.000000 concordia-harmony-1.0.0/src/concordia_harmony.egg-info/top_level.txt
```

### Comparing `concordia-harmony-0.1.5/LICENSE` & `concordia-harmony-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `concordia-harmony-0.1.5/PKG-INFO` & `concordia-harmony-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concordia-harmony
-Version: 0.1.5
+Version: 1.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Concordia: Music Generation Using An SMT-based Harmony Solver
 <div style="text-align: center;">
 <img class="img-fluid" width=500 src="./concordia.png" alt="img-verification">
 </div>
@@ -13,23 +13,23 @@
 Suppose you are composing some music. You have a beautiful melody, but you don’t know what chord progression to use. We propose _Concordia_, an SMT-Based harmony-solving framework that helps composers and songwriters brainstorm musical ideas and test them out right away. Given some constraints ahead of time (e.g. baseline, melody, which chord to use), _Concordia_ will generate a harmony that satisfies the constraints. In the following sections, we will discuss the implementation of the harmony solver in more detail. This project made the following contributions:
 
 - *Describe how musical elements can be expressed* as variables that an SMT-solver can understand.
 - *Provide an extensible framework* for constructing constraints around musical constructs.
 - *Provide An open-source and easy-to-install implementation* of the harmony solver, available on here on Github and as a package on [PyPI]("https://pypi.org/project/concordia-harmony/"). An quick demo can be found in `example.ipynb`.
 
 ## Supported Constraints
-| Constraint          | Description |
-|---------------------| --- |
-| Note specification  | Use specific notes at a certain point in the harmony. |
-| Chord specification | Use a specific chord/chord type at a certain position in the progression. |
-| Chord set           | Only use chords specified to compose the harmony. |
+| Constraint          | Description                                                                                   |
+|---------------------|-----------------------------------------------------------------------------------------------|
+| Note specification  | Use specific notes at a certain point in the harmony.                                         |
+| Chord specification | Use a specific chord/chord type at a certain position in the progression.                     |
+| Chord set           | Only use chords specified to compose the harmony.                                             |
 | Voice range         | Soprano cannot sing a really low note; some instruments can only play a small range of notes. |
-| Voice leading       | You might want to restrict the max interval of a jump in the melody. |
-| Chord progression   | Some chords typically do not proceed to some other chords. |
-| Idiomatic uses | Some music events happen with others (e.g. cadences, voice exchange). |
+| Voice leading       | You might want to restrict the max interval of a jump in the melody.                          |
+| Chord progression   | Some chords typically do not proceed to some other chords.                                    |
+| Idiomatic uses      | Some music events happen with others (e.g. cadences, voice exchange).                         |
 
 ## Architecture
 <div style="text-align: center;">
 <img class="img-fluid" width=500 src="./concordia-architecture.jpeg" alt="img-verification">
 </div>
```

### Comparing `concordia-harmony-0.1.5/README.md` & `concordia-harmony-1.0.0/src/concordia_harmony.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,37 @@
+Metadata-Version: 2.1
+Name: concordia-harmony
+Version: 1.0.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Concordia: Music Generation Using An SMT-based Harmony Solver
 <div style="text-align: center;">
 <img class="img-fluid" width=500 src="./concordia.png" alt="img-verification">
 </div>
 
 ## Overview
 Suppose you are composing some music. You have a beautiful melody, but you don’t know what chord progression to use. We propose _Concordia_, an SMT-Based harmony-solving framework that helps composers and songwriters brainstorm musical ideas and test them out right away. Given some constraints ahead of time (e.g. baseline, melody, which chord to use), _Concordia_ will generate a harmony that satisfies the constraints. In the following sections, we will discuss the implementation of the harmony solver in more detail. This project made the following contributions:
 
 - *Describe how musical elements can be expressed* as variables that an SMT-solver can understand.
 - *Provide an extensible framework* for constructing constraints around musical constructs.
 - *Provide An open-source and easy-to-install implementation* of the harmony solver, available on here on Github and as a package on [PyPI]("https://pypi.org/project/concordia-harmony/"). An quick demo can be found in `example.ipynb`.
 
 ## Supported Constraints
-| Constraint          | Description |
-|---------------------| --- |
-| Note specification  | Use specific notes at a certain point in the harmony. |
-| Chord specification | Use a specific chord/chord type at a certain position in the progression. |
-| Chord set           | Only use chords specified to compose the harmony. |
+| Constraint          | Description                                                                                   |
+|---------------------|-----------------------------------------------------------------------------------------------|
+| Note specification  | Use specific notes at a certain point in the harmony.                                         |
+| Chord specification | Use a specific chord/chord type at a certain position in the progression.                     |
+| Chord set           | Only use chords specified to compose the harmony.                                             |
 | Voice range         | Soprano cannot sing a really low note; some instruments can only play a small range of notes. |
-| Voice leading       | You might want to restrict the max interval of a jump in the melody. |
-| Chord progression   | Some chords typically do not proceed to some other chords. |
-| Idiomatic uses | Some music events happen with others (e.g. cadences, voice exchange). |
+| Voice leading       | You might want to restrict the max interval of a jump in the melody.                          |
+| Chord progression   | Some chords typically do not proceed to some other chords.                                    |
+| Idiomatic uses      | Some music events happen with others (e.g. cadences, voice exchange).                         |
 
 ## Architecture
 <div style="text-align: center;">
 <img class="img-fluid" width=500 src="./concordia-architecture.jpeg" alt="img-verification">
 </div>
 
 
 ## Changes
-To push an update to PyPI, first update the version number in `pyproject.toml`, then push to GitHub.
+To push an update to PyPI, first update the version number in `pyproject.toml`, then push to GitHub.
```

### Comparing `concordia-harmony-0.1.5/src/concordia/constraints.py` & `concordia-harmony-1.0.0/src/concordia/constraints.py`

 * *Files identical despite different names*

### Comparing `concordia-harmony-0.1.5/src/concordia/library.py` & `concordia-harmony-1.0.0/src/concordia/library.py`

 * *Files identical despite different names*

### Comparing `concordia-harmony-0.1.5/src/concordia/solver.py` & `concordia-harmony-1.0.0/src/concordia/solver.py`

 * *Files identical despite different names*

### Comparing `concordia-harmony-0.1.5/src/concordia_harmony.egg-info/PKG-INFO` & `concordia-harmony-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-Metadata-Version: 2.1
-Name: concordia-harmony
-Version: 0.1.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Concordia: Music Generation Using An SMT-based Harmony Solver
 <div style="text-align: center;">
 <img class="img-fluid" width=500 src="./concordia.png" alt="img-verification">
 </div>
 
 ## Overview
 Suppose you are composing some music. You have a beautiful melody, but you don’t know what chord progression to use. We propose _Concordia_, an SMT-Based harmony-solving framework that helps composers and songwriters brainstorm musical ideas and test them out right away. Given some constraints ahead of time (e.g. baseline, melody, which chord to use), _Concordia_ will generate a harmony that satisfies the constraints. In the following sections, we will discuss the implementation of the harmony solver in more detail. This project made the following contributions:
 
 - *Describe how musical elements can be expressed* as variables that an SMT-solver can understand.
 - *Provide an extensible framework* for constructing constraints around musical constructs.
 - *Provide An open-source and easy-to-install implementation* of the harmony solver, available on here on Github and as a package on [PyPI]("https://pypi.org/project/concordia-harmony/"). An quick demo can be found in `example.ipynb`.
 
 ## Supported Constraints
-| Constraint          | Description |
-|---------------------| --- |
-| Note specification  | Use specific notes at a certain point in the harmony. |
-| Chord specification | Use a specific chord/chord type at a certain position in the progression. |
-| Chord set           | Only use chords specified to compose the harmony. |
+| Constraint          | Description                                                                                   |
+|---------------------|-----------------------------------------------------------------------------------------------|
+| Note specification  | Use specific notes at a certain point in the harmony.                                         |
+| Chord specification | Use a specific chord/chord type at a certain position in the progression.                     |
+| Chord set           | Only use chords specified to compose the harmony.                                             |
 | Voice range         | Soprano cannot sing a really low note; some instruments can only play a small range of notes. |
-| Voice leading       | You might want to restrict the max interval of a jump in the melody. |
-| Chord progression   | Some chords typically do not proceed to some other chords. |
-| Idiomatic uses | Some music events happen with others (e.g. cadences, voice exchange). |
+| Voice leading       | You might want to restrict the max interval of a jump in the melody.                          |
+| Chord progression   | Some chords typically do not proceed to some other chords.                                    |
+| Idiomatic uses      | Some music events happen with others (e.g. cadences, voice exchange).                         |
 
 ## Architecture
 <div style="text-align: center;">
 <img class="img-fluid" width=500 src="./concordia-architecture.jpeg" alt="img-verification">
 </div>
 
 
 ## Changes
-To push an update to PyPI, first update the version number in `pyproject.toml`, then push to GitHub.
+To push an update to PyPI, first update the version number in `pyproject.toml`, then push to GitHub.
```

