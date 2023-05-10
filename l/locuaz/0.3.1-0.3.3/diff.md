# Comparing `tmp/locuaz-0.3.1.tar.gz` & `tmp/locuaz-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locuaz-0.3.1.tar", last modified: Wed May 10 09:59:29 2023, max compression
+gzip compressed data, was "locuaz-0.3.3.tar", last modified: Wed May 10 10:13:03 2023, max compression
```

## Comparing `locuaz-0.3.1.tar` & `locuaz-0.3.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:18.000000 locuaz-0.3.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 09:59:18.000000 locuaz-0.3.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 09:59:18.000000 locuaz-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 09:59:29.936362 locuaz-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 09:59:18.000000 locuaz-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/abstractmutationgenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/abstractpruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/abstractscoringfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/amberutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/autodockvina.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/bach.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/basemutator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/basestatistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/bluues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/bluuesbmf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/epochinitializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/evoef2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/fixbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/gmxmmpbsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/gromacsutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/haddock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/moleculesutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/molutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutationgenerators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutatorbiobb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutatordlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutatordlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutatorevoef2.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/piepisa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/pisa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/projectutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/prunerconsensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/prunermetropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/pruners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/rosetta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/runutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.924362 locuaz-0.3.1/locuaz/sample_bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/sample_bin/aux_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/sample_bin/aux_scripts/reorder_pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/sample_bin/dlpacker/
--rwxr-xr-x   0 runner    (1001) docker     (123)    70622 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/sample_bin/dlpacker/charges.rtp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/sample_bin/gmxmmpbsa/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/sample_bin/gmxmmpbsa/gmxmmpbsa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/sample_bin/haddock/
--rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/sample_bin/haddock/template_scoring.inp
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/scoringfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/spm4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/spm4i.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/spm4mmpbsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/statisticcmdistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/statisticinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/utils_scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/validatore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 09:59:19.000000 locuaz-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-10 09:59:29.936362 locuaz-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 09:59:19.000000 locuaz-0.3.1/tests/test_locuaz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.676916 locuaz-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 10:12:50.000000 locuaz-0.3.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 10:12:50.000000 locuaz-0.3.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 10:12:50.000000 locuaz-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 10:13:03.676916 locuaz-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 10:12:50.000000 locuaz-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.676916 locuaz-0.3.3/locuaz/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/abstractmutationgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/abstractpruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/abstractscoringfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/amberutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/autodockvina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/bach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/basemutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/basestatistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/bluues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/bluuesbmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/epochinitializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/evoef2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/fixbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/gmxmmpbsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/gromacsutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/haddock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/moleculesutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/molutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/mutationgenerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/mutatorbiobb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/mutatordlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/mutatordlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/mutatorevoef2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/piepisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/pisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/projectutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/prunerconsensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/prunermetropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/pruners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/rosetta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/runutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.664916 locuaz-0.3.3/locuaz/sample_bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.676916 locuaz-0.3.3/locuaz/sample_bin/aux_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/sample_bin/aux_scripts/reorder_pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.676916 locuaz-0.3.3/locuaz/sample_bin/dlpacker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70622 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/sample_bin/dlpacker/charges.rtp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.676916 locuaz-0.3.3/locuaz/sample_bin/gmxmmpbsa/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/sample_bin/gmxmmpbsa/gmxmmpbsa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.676916 locuaz-0.3.3/locuaz/sample_bin/haddock/
+-rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/sample_bin/haddock/template_scoring.inp
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/scoringfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/spm4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/spm4i.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/spm4mmpbsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/statisticcmdistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/statisticinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/utils_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-10 10:12:50.000000 locuaz-0.3.3/locuaz/validatore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.676916 locuaz-0.3.3/locuaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 10:13:03.000000 locuaz-0.3.3/locuaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-10 10:13:03.000000 locuaz-0.3.3/locuaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 10:13:03.000000 locuaz-0.3.3/locuaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 10:13:03.000000 locuaz-0.3.3/locuaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 10:13:03.000000 locuaz-0.3.3/locuaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 10:13:03.000000 locuaz-0.3.3/locuaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 10:12:50.000000 locuaz-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-10 10:13:03.676916 locuaz-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 10:13:03.676916 locuaz-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 10:12:50.000000 locuaz-0.3.3/tests/test_locuaz.py
```

### Comparing `locuaz-0.3.1/LICENSE.rst` & `locuaz-0.3.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/PKG-INFO` & `locuaz-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locuaz
-Version: 0.3.1
+Version: 0.3.3
 Summary: Antibody optimization protocol
 Author: Patricio Barletta
 Author-email: pbarletta@gmail.com
 Keywords: molecular,dynamics,antibody,antibodies
 Requires-Python: >=3.9.15
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
```

### Comparing `locuaz-0.3.1/README.rst` & `locuaz-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/abstractmutationgenerator.py` & `locuaz-0.3.3/locuaz/abstractmutationgenerator.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/abstractscoringfunction.py` & `locuaz-0.3.3/locuaz/abstractscoringfunction.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/amberutils.py` & `locuaz-0.3.3/locuaz/amberutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/autodockvina.py` & `locuaz-0.3.3/locuaz/autodockvina.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/bach.py` & `locuaz-0.3.3/locuaz/bach.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/basemutator.py` & `locuaz-0.3.3/locuaz/basemutator.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/basestatistic.py` & `locuaz-0.3.3/locuaz/basestatistic.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/bluues.py` & `locuaz-0.3.3/locuaz/bluues.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/bluuesbmf.py` & `locuaz-0.3.3/locuaz/bluuesbmf.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/cli.py` & `locuaz-0.3.3/locuaz/cli.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/complex.py` & `locuaz-0.3.3/locuaz/complex.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/epochinitializer.py` & `locuaz-0.3.3/locuaz/epochinitializer.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/evoef2.py` & `locuaz-0.3.3/locuaz/evoef2.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/fileutils.py` & `locuaz-0.3.3/locuaz/fileutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/fixbox.py` & `locuaz-0.3.3/locuaz/fixbox.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/gmxmmpbsa.py` & `locuaz-0.3.3/locuaz/gmxmmpbsa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/gromacsutils.py` & `locuaz-0.3.3/locuaz/gromacsutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/haddock.py` & `locuaz-0.3.3/locuaz/haddock.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/interface.py` & `locuaz-0.3.3/locuaz/interface.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/molecules.py` & `locuaz-0.3.3/locuaz/molecules.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/moleculesutils.py` & `locuaz-0.3.3/locuaz/moleculesutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/molutils.py` & `locuaz-0.3.3/locuaz/molutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/mutation.py` & `locuaz-0.3.3/locuaz/mutation.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/mutatorbiobb.py` & `locuaz-0.3.3/locuaz/mutatorbiobb.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/mutatordlp.py` & `locuaz-0.3.3/locuaz/mutatordlp.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/mutatordlpr.py` & `locuaz-0.3.3/locuaz/mutatordlpr.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/mutatorevoef2.py` & `locuaz-0.3.3/locuaz/mutatorevoef2.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/mutators.py` & `locuaz-0.3.3/locuaz/mutators.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/piepisa.py` & `locuaz-0.3.3/locuaz/piepisa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/pisa.py` & `locuaz-0.3.3/locuaz/pisa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/primitives.py` & `locuaz-0.3.3/locuaz/primitives.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/projectutils.py` & `locuaz-0.3.3/locuaz/projectutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/protocol.py` & `locuaz-0.3.3/locuaz/protocol.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/pruner.py` & `locuaz-0.3.3/locuaz/pruner.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/prunerconsensus.py` & `locuaz-0.3.3/locuaz/prunerconsensus.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/prunermetropolis.py` & `locuaz-0.3.3/locuaz/prunermetropolis.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/pruning.py` & `locuaz-0.3.3/locuaz/pruning.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/rosetta.py` & `locuaz-0.3.3/locuaz/rosetta.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/run.py` & `locuaz-0.3.3/locuaz/run.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/runutils.py` & `locuaz-0.3.3/locuaz/runutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/sample_bin/aux_scripts/reorder_pdb.py` & `locuaz-0.3.3/locuaz/sample_bin/aux_scripts/reorder_pdb.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/sample_bin/dlpacker/charges.rtp` & `locuaz-0.3.3/locuaz/sample_bin/dlpacker/charges.rtp`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/sample_bin/haddock/template_scoring.inp` & `locuaz-0.3.3/locuaz/sample_bin/haddock/template_scoring.inp`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/schema.yaml` & `locuaz-0.3.3/locuaz/schema.yaml`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/scoring.py` & `locuaz-0.3.3/locuaz/scoring.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/scoringfunctions.py` & `locuaz-0.3.3/locuaz/scoringfunctions.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/spm4.py` & `locuaz-0.3.3/locuaz/spm4.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/spm4i.py` & `locuaz-0.3.3/locuaz/spm4i.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/spm4mmpbsa.py` & `locuaz-0.3.3/locuaz/spm4mmpbsa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/statisticcmdistance.py` & `locuaz-0.3.3/locuaz/statisticcmdistance.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/statisticinterface.py` & `locuaz-0.3.3/locuaz/statisticinterface.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/statistics.py` & `locuaz-0.3.3/locuaz/statistics.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/utils_scoring.py` & `locuaz-0.3.3/locuaz/utils_scoring.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz/validatore.py` & `locuaz-0.3.3/locuaz/validatore.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/locuaz.egg-info/PKG-INFO` & `locuaz-0.3.3/locuaz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locuaz
-Version: 0.3.1
+Version: 0.3.3
 Summary: Antibody optimization protocol
 Author: Patricio Barletta
 Author-email: pbarletta@gmail.com
 Keywords: molecular,dynamics,antibody,antibodies
 Requires-Python: >=3.9.15
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
```

### Comparing `locuaz-0.3.1/locuaz.egg-info/SOURCES.txt` & `locuaz-0.3.3/locuaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.1/setup.cfg` & `locuaz-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = locuaz
-version = 0.3.1
+version = 0.3.3
 author = Patricio Barletta
 author_email = pbarletta@gmail.com
 description = Antibody optimization protocol
 long_description = file: README.rst, CHANGELOG.rst, LICENSE.rst
 long_description_content_type = text/x-rst
 keywords = molecular, dynamics, antibody, antibodies
```

### Comparing `locuaz-0.3.1/tests/test_locuaz.py` & `locuaz-0.3.3/tests/test_locuaz.py`

 * *Files identical despite different names*

