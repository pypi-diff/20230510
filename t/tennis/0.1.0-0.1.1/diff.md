# Comparing `tmp/tennis-0.1.0.tar.gz` & `tmp/tennis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tennis-0.1.0.tar", last modified: Tue May  9 03:30:28 2023, max compression
+gzip compressed data, was "tennis-0.1.1.tar", last modified: Wed May 10 21:43:05 2023, max compression
```

## Comparing `tennis-0.1.0.tar` & `tennis-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 03:30:28.409463 tennis-0.1.0/
--rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      439 2023-05-09 03:30:28.408489 tennis-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-06 20:11:07.000000 tennis-0.1.0/README.md
--rw-rw-rw-   0        0        0      516 2023-05-09 03:28:57.000000 tennis-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-09 03:30:28.409463 tennis-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      284 2023-05-09 03:27:27.000000 tennis-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:30:28.388970 tennis-0.1.0/tennis/
--rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.0/tennis/__init__.py
--rw-rw-rw-   0        0        0    30932 2023-05-09 03:05:50.000000 tennis-0.1.0/tennis/match.py
--rw-rw-rw-   0        0        0    17035 2023-05-09 03:03:26.000000 tennis-0.1.0/tennis/tiebreak.py
-drwxrwxrwx   0        0        0        0 2023-05-09 03:30:28.407513 tennis-0.1.0/tennis.egg-info/
--rw-rw-rw-   0        0        0      439 2023-05-09 03:30:28.000000 tennis-0.1.0/tennis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-05-09 03:30:28.000000 tennis-0.1.0/tennis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 03:30:28.000000 tennis-0.1.0/tennis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 03:30:28.000000 tennis-0.1.0/tennis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 21:43:05.326835 tennis-0.1.1/
+-rw-rw-rw-   0        0        0     1083 2023-05-09 03:08:15.000000 tennis-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5443 2023-05-10 21:43:05.325837 tennis-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5002 2023-05-10 21:40:09.000000 tennis-0.1.1/README.md
+-rw-rw-rw-   0        0        0      516 2023-05-10 21:42:49.000000 tennis-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 21:43:05.326835 tennis-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      284 2023-05-10 21:42:53.000000 tennis-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:43:05.315358 tennis-0.1.1/tennis/
+-rw-rw-rw-   0        0        0        0 2023-05-06 20:11:19.000000 tennis-0.1.1/tennis/__init__.py
+-rw-rw-rw-   0        0        0    30932 2023-05-09 03:05:50.000000 tennis-0.1.1/tennis/match.py
+-rw-rw-rw-   0        0        0    17036 2023-05-10 21:30:40.000000 tennis-0.1.1/tennis/tiebreak.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:43:05.324839 tennis-0.1.1/tennis.egg-info/
+-rw-rw-rw-   0        0        0     5443 2023-05-10 21:43:05.000000 tennis-0.1.1/tennis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-05-10 21:43:05.000000 tennis-0.1.1/tennis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 21:43:05.000000 tennis-0.1.1/tennis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 21:43:05.000000 tennis-0.1.1/tennis.egg-info/top_level.txt
```

### Comparing `tennis-0.1.0/LICENSE` & `tennis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tennis-0.1.0/pyproject.toml` & `tennis-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tennis"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="bear102" },
 ]
 description = "A library for tracking tennis matches and scoring"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tennis-0.1.0/tennis/match.py` & `tennis-0.1.1/tennis/match.py`

 * *Files identical despite different names*

### Comparing `tennis-0.1.0/tennis/tiebreak.py` & `tennis-0.1.1/tennis/tiebreak.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 
         else:
             st2="*"
             st1=" "
     
         return (f"""
 ╔═════════════════════════════════════╗
-              Match Score
+            Tiebreak Score
 
      T
      {tb1}  {st1}                {player}
      {tb2}  {st2}                {self.get_other_player(player)}
 
 ╚═════════════════════════════════════╝
 """)
```

