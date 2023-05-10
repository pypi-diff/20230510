# Comparing `tmp/PoissonFuncaoCorrente-1.1.0.tar.gz` & `tmp/PoissonFuncaoCorrente-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PoissonFuncaoCorrente-1.1.0.tar", last modified: Wed May 10 14:54:40 2023, max compression
+gzip compressed data, was "PoissonFuncaoCorrente-1.1.1.tar", last modified: Wed May 10 15:09:06 2023, max compression
```

## Comparing `PoissonFuncaoCorrente-1.1.0.tar` & `PoissonFuncaoCorrente-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1074 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/LICENSE
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      412 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/PKG-INFO
-drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      412 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/PKG-INFO
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      349 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/SOURCES.txt
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)        1 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/dependency_links.txt
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)        6 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/requires.txt
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)        4 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/top_level.txt
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      856 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/README.md
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)       38 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/setup.cfg
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      630 2023-05-10 14:47:03.000000 PoissonFuncaoCorrente-1.1.0/setup.py
-drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/src/
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1969 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/FCDirichlet.py
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      916 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/FCsemomega.py
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1096 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/FuncaoCorrente.py
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1002 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/FuncaoCorrenteCC.py
--rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      276 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/__init__.py
+drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 15:09:06.178442 PoissonFuncaoCorrente-1.1.1/
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1074 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.1/LICENSE
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      607 2023-05-10 15:09:06.178442 PoissonFuncaoCorrente-1.1.1/PKG-INFO
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      856 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.1/README.md
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)       38 2023-05-10 15:09:06.178442 PoissonFuncaoCorrente-1.1.1/setup.cfg
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      925 2023-05-10 15:08:46.000000 PoissonFuncaoCorrente-1.1.1/setup.py
+drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 15:09:06.174442 PoissonFuncaoCorrente-1.1.1/src/
+drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 15:09:06.178442 PoissonFuncaoCorrente-1.1.1/src/PoissonFuncaoCorrente.egg-info/
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      607 2023-05-10 15:09:06.000000 PoissonFuncaoCorrente-1.1.1/src/PoissonFuncaoCorrente.egg-info/PKG-INFO
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      222 2023-05-10 15:09:06.000000 PoissonFuncaoCorrente-1.1.1/src/PoissonFuncaoCorrente.egg-info/SOURCES.txt
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)        1 2023-05-10 15:09:06.000000 PoissonFuncaoCorrente-1.1.1/src/PoissonFuncaoCorrente.egg-info/dependency_links.txt
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)        1 2023-05-10 15:09:06.000000 PoissonFuncaoCorrente-1.1.1/src/PoissonFuncaoCorrente.egg-info/top_level.txt
```

### Comparing `PoissonFuncaoCorrente-1.1.0/LICENSE` & `PoissonFuncaoCorrente-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PoissonFuncaoCorrente-1.1.0/README.md` & `PoissonFuncaoCorrente-1.1.1/README.md`

 * *Files identical despite different names*

