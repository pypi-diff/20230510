# Comparing `tmp/PoissonFuncaoCorrente-1.0.0.tar.gz` & `tmp/PoissonFuncaoCorrente-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PoissonFuncaoCorrente-1.0.0.tar", last modified: Wed Feb  8 22:15:09 2023, max compression
+gzip compressed data, was "PoissonFuncaoCorrente-1.1.0.tar", last modified: Wed May 10 14:54:40 2023, max compression
```

## Comparing `PoissonFuncaoCorrente-1.0.0.tar` & `PoissonFuncaoCorrente-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-08 22:15:09.244161 PoissonFuncaoCorrente-1.0.0/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1074 2023-01-31 01:18:37.000000 PoissonFuncaoCorrente-1.0.0/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      450 2023-02-08 22:15:09.244161 PoissonFuncaoCorrente-1.0.0/PKG-INFO
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-08 22:15:09.244161 PoissonFuncaoCorrente-1.0.0/PoissonFuncaoCorrente.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      450 2023-02-08 22:15:09.000000 PoissonFuncaoCorrente-1.0.0/PoissonFuncaoCorrente.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      250 2023-02-08 22:15:09.000000 PoissonFuncaoCorrente-1.0.0/PoissonFuncaoCorrente.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-02-08 22:15:09.000000 PoissonFuncaoCorrente-1.0.0/PoissonFuncaoCorrente.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        6 2023-02-08 22:15:09.000000 PoissonFuncaoCorrente-1.0.0/PoissonFuncaoCorrente.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-02-08 22:15:09.000000 PoissonFuncaoCorrente-1.0.0/PoissonFuncaoCorrente.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      428 2023-02-08 22:11:34.000000 PoissonFuncaoCorrente-1.0.0/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-02-08 22:15:09.244161 PoissonFuncaoCorrente-1.0.0/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      630 2023-02-08 22:10:03.000000 PoissonFuncaoCorrente-1.0.0/setup.py
+drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1074 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/LICENSE
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      412 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/PKG-INFO
+drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      412 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/PKG-INFO
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      349 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/SOURCES.txt
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)        1 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/dependency_links.txt
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)        6 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/requires.txt
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)        4 2023-05-10 14:54:40.000000 PoissonFuncaoCorrente-1.1.0/PoissonFuncaoCorrente.egg-info/top_level.txt
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      856 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/README.md
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)       38 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/setup.cfg
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      630 2023-05-10 14:47:03.000000 PoissonFuncaoCorrente-1.1.0/setup.py
+drwxrwxr-x   0 aluno001  (1000) aluno001  (1000)        0 2023-05-10 14:54:40.885699 PoissonFuncaoCorrente-1.1.0/src/
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1969 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/FCDirichlet.py
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      916 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/FCsemomega.py
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1096 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/FuncaoCorrente.py
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)     1002 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/FuncaoCorrenteCC.py
+-rw-rw-r--   0 aluno001  (1000) aluno001  (1000)      276 2023-03-10 19:23:22.000000 PoissonFuncaoCorrente-1.1.0/src/__init__.py
```

### Comparing `PoissonFuncaoCorrente-1.0.0/LICENSE` & `PoissonFuncaoCorrente-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PoissonFuncaoCorrente-1.0.0/setup.py` & `PoissonFuncaoCorrente-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages  
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="PoissonFuncaoCorrente",
-    version="1.0.0",
+    version="1.1.0",
     author="Lucas Salimene",
     author_email="lucassalimene@protonmail.com",
     packages=find_packages(),
     description="Um pacote para o calculo da funcao corrente",
     long_description="Esse pacote utiliza métodos númericos iterativos para resolver a equação que relaciona a Função Corrente com a vorticidade",
     license='MIT',
     long_description_content_type="text/markdown",
```

