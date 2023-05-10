# Comparing `tmp/raisetool-0.1.14.tar.gz` & `tmp/raisetool-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raisetool-0.1.14.tar", max compression
+gzip compressed data, was "raisetool-0.1.15.tar", max compression
```

## Comparing `raisetool-0.1.14.tar` & `raisetool-0.1.15.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-05-08 19:33:42.976724 raisetool-0.1.14/LICENSE
--rw-r--r--   0        0        0      710 2023-05-08 22:41:03.006476 raisetool-0.1.14/README.md
--rw-r--r--   0        0        0      650 2023-05-08 22:42:30.706600 raisetool-0.1.14/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 09:06:36.254156 raisetool-0.1.14/raisetool/__init__.py
--rw-r--r--   0        0        0     5239 2023-05-08 22:18:38.497028 raisetool-0.1.14/raisetool/formatter.py
--rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 raisetool-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-09 11:26:38.487906 raisetool-0.1.15/LICENSE
+-rw-r--r--   0        0        0     1968 2023-05-10 09:55:07.537199 raisetool-0.1.15/README.md
+-rw-r--r--   0        0        0      646 2023-05-10 09:56:31.065175 raisetool-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 11:26:38.487906 raisetool-0.1.15/raisetool/__init__.py
+-rw-r--r--   0        0        0     5239 2023-05-09 11:26:38.487906 raisetool-0.1.15/raisetool/formatter.py
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 raisetool-0.1.15/PKG-INFO
```

### Comparing `raisetool-0.1.14/LICENSE` & `raisetool-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `raisetool-0.1.14/pyproject.toml` & `raisetool-0.1.15/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "raisetool"
-version = "0.1.14"
+version = "0.1.15"
 description = "Rise class for formatting thrown exception messages."
 authors = ["Jacek Kotlarski <szumak@virthost.pl>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Szumak75/RaiseTool"
 classifiers = [
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-attribtool = "^1.0.1"
+attribtool = "^1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.1"
 nose = "^1.3.7"
 typing-extensions = "^4.5.0"
```

### Comparing `raisetool-0.1.14/raisetool/formatter.py` & `raisetool-0.1.15/raisetool/formatter.py`

 * *Files identical despite different names*

