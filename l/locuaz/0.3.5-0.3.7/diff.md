# Comparing `tmp/locuaz-0.3.5.tar.gz` & `tmp/locuaz-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locuaz-0.3.5.tar", last modified: Wed May 10 11:17:35 2023, max compression
+gzip compressed data, was "locuaz-0.3.7.tar", last modified: Wed May 10 13:38:28 2023, max compression
```

## Comparing `locuaz-0.3.5.tar` & `locuaz-0.3.7.tar`

### file list

```diff
@@ -1,82 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.260194 locuaz-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:20.000000 locuaz-0.3.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 11:17:20.000000 locuaz-0.3.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 11:17:20.000000 locuaz-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 11:17:35.260194 locuaz-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 11:17:20.000000 locuaz-0.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.260194 locuaz-0.3.5/locuaz/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/abstractmutationgenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/abstractpruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/abstractscoringfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/amberutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/autodockvina.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/bach.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/basemutator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/basestatistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/bluues.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/bluuesbmf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/epochinitializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/evoef2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/fixbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/gmxmmpbsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/gromacsutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/haddock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/moleculesutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/molutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/mutationgenerators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/mutatorbiobb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/mutatordlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/mutatordlpr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/mutatorevoef2.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/piepisa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/pisa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/projectutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/prunerconsensus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/prunermetropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/pruners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/pruning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/rosetta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/runutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.244194 locuaz-0.3.5/locuaz/sample_bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.260194 locuaz-0.3.5/locuaz/sample_bin/aux_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/sample_bin/aux_scripts/reorder_pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.260194 locuaz-0.3.5/locuaz/sample_bin/dlpacker/
--rwxr-xr-x   0 runner    (1001) docker     (123)    70622 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/sample_bin/dlpacker/charges.rtp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.260194 locuaz-0.3.5/locuaz/sample_bin/gmxmmpbsa/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/sample_bin/gmxmmpbsa/gmxmmpbsa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.260194 locuaz-0.3.5/locuaz/sample_bin/haddock/
--rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/sample_bin/haddock/template_scoring.inp
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/scoringfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/spm4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/spm4i.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/spm4mmpbsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/statisticcmdistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/statisticinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/utils_scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-10 11:17:20.000000 locuaz-0.3.5/locuaz/validatore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.260194 locuaz-0.3.5/locuaz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 11:17:35.000000 locuaz-0.3.5/locuaz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-10 11:17:35.000000 locuaz-0.3.5/locuaz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:17:35.000000 locuaz-0.3.5/locuaz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 11:17:35.000000 locuaz-0.3.5/locuaz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 11:17:35.000000 locuaz-0.3.5/locuaz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 11:17:35.000000 locuaz-0.3.5/locuaz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 11:17:20.000000 locuaz-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-10 11:17:35.260194 locuaz-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:17:35.260194 locuaz-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 11:17:20.000000 locuaz-0.3.5/tests/test_locuaz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.640088 locuaz-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:17.000000 locuaz-0.3.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 13:38:17.000000 locuaz-0.3.7/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 13:38:17.000000 locuaz-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 13:38:28.640088 locuaz-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 13:38:17.000000 locuaz-0.3.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.636088 locuaz-0.3.7/locuaz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.636088 locuaz-0.3.7/locuaz/DLPacker/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/DLPacker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/DLPacker/dlpacker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19402 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/DLPacker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/abstractmutationgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/abstractpruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/abstractscoringfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/amberutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/autodockvina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/bach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/basemutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/basestatistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/bluues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/bluuesbmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/epochinitializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/evoef2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/fixbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/gmxmmpbsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15809 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/gromacsutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/haddock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/moleculesutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/molutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/mutationgenerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/mutatorbiobb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/mutatordlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/mutatordlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/mutatorevoef2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/piepisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/pisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/projectutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/prunerconsensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/prunermetropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/pruners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/rosetta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/runutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.616088 locuaz-0.3.7/locuaz/sample_bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.636088 locuaz-0.3.7/locuaz/sample_bin/aux_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/sample_bin/aux_scripts/reorder_pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.636088 locuaz-0.3.7/locuaz/sample_bin/dlpacker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70622 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/sample_bin/dlpacker/charges.rtp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.636088 locuaz-0.3.7/locuaz/sample_bin/gmxmmpbsa/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/sample_bin/gmxmmpbsa/gmxmmpbsa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.640088 locuaz-0.3.7/locuaz/sample_bin/haddock/
+-rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/sample_bin/haddock/template_scoring.inp
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/scoringfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/spm4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/spm4i.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/spm4mmpbsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/statisticcmdistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/statisticinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/utils_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-10 13:38:17.000000 locuaz-0.3.7/locuaz/validatore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.636088 locuaz-0.3.7/locuaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 13:38:28.000000 locuaz-0.3.7/locuaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-10 13:38:28.000000 locuaz-0.3.7/locuaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:38:28.000000 locuaz-0.3.7/locuaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 13:38:28.000000 locuaz-0.3.7/locuaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 13:38:28.000000 locuaz-0.3.7/locuaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 13:38:28.000000 locuaz-0.3.7/locuaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 13:38:17.000000 locuaz-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-10 13:38:28.640088 locuaz-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:38:28.640088 locuaz-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 13:38:17.000000 locuaz-0.3.7/tests/test_locuaz.py
```

### Comparing `locuaz-0.3.5/LICENSE.rst` & `locuaz-0.3.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/PKG-INFO` & `locuaz-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locuaz
-Version: 0.3.5
+Version: 0.3.7
 Summary: Antibody optimization protocol
 Author: Patricio Barletta
 Author-email: pbarletta@gmail.com
 Keywords: molecular,dynamics,antibody,antibodies
 Requires-Python: >=3.9.15
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
```

### Comparing `locuaz-0.3.5/README.rst` & `locuaz-0.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/abstractmutationgenerator.py` & `locuaz-0.3.7/locuaz/abstractmutationgenerator.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/abstractscoringfunction.py` & `locuaz-0.3.7/locuaz/abstractscoringfunction.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/amberutils.py` & `locuaz-0.3.7/locuaz/amberutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/autodockvina.py` & `locuaz-0.3.7/locuaz/autodockvina.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/bach.py` & `locuaz-0.3.7/locuaz/bach.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/basemutator.py` & `locuaz-0.3.7/locuaz/basemutator.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/basestatistic.py` & `locuaz-0.3.7/locuaz/basestatistic.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/bluues.py` & `locuaz-0.3.7/locuaz/bluues.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/bluuesbmf.py` & `locuaz-0.3.7/locuaz/bluuesbmf.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/cli.py` & `locuaz-0.3.7/locuaz/cli.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/complex.py` & `locuaz-0.3.7/locuaz/complex.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/epochinitializer.py` & `locuaz-0.3.7/locuaz/epochinitializer.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/evoef2.py` & `locuaz-0.3.7/locuaz/evoef2.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/fileutils.py` & `locuaz-0.3.7/locuaz/fileutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/fixbox.py` & `locuaz-0.3.7/locuaz/fixbox.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/gmxmmpbsa.py` & `locuaz-0.3.7/locuaz/gmxmmpbsa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/gromacsutils.py` & `locuaz-0.3.7/locuaz/gromacsutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/haddock.py` & `locuaz-0.3.7/locuaz/haddock.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/interface.py` & `locuaz-0.3.7/locuaz/interface.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/molecules.py` & `locuaz-0.3.7/locuaz/molecules.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/moleculesutils.py` & `locuaz-0.3.7/locuaz/moleculesutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/molutils.py` & `locuaz-0.3.7/locuaz/molutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/mutation.py` & `locuaz-0.3.7/locuaz/mutation.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/mutatorbiobb.py` & `locuaz-0.3.7/locuaz/mutatorbiobb.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/mutatordlp.py` & `locuaz-0.3.7/locuaz/mutatordlp.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/mutatordlpr.py` & `locuaz-0.3.7/locuaz/mutatordlpr.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/mutatorevoef2.py` & `locuaz-0.3.7/locuaz/mutatorevoef2.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/mutators.py` & `locuaz-0.3.7/locuaz/mutators.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/piepisa.py` & `locuaz-0.3.7/locuaz/piepisa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/pisa.py` & `locuaz-0.3.7/locuaz/pisa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/primitives.py` & `locuaz-0.3.7/locuaz/primitives.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/projectutils.py` & `locuaz-0.3.7/locuaz/projectutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/protocol.py` & `locuaz-0.3.7/locuaz/protocol.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/pruner.py` & `locuaz-0.3.7/locuaz/pruner.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/prunerconsensus.py` & `locuaz-0.3.7/locuaz/prunerconsensus.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/prunermetropolis.py` & `locuaz-0.3.7/locuaz/prunermetropolis.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/pruning.py` & `locuaz-0.3.7/locuaz/pruning.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/rosetta.py` & `locuaz-0.3.7/locuaz/rosetta.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/run.py` & `locuaz-0.3.7/locuaz/run.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/runutils.py` & `locuaz-0.3.7/locuaz/runutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/sample_bin/aux_scripts/reorder_pdb.py` & `locuaz-0.3.7/locuaz/sample_bin/aux_scripts/reorder_pdb.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/sample_bin/dlpacker/charges.rtp` & `locuaz-0.3.7/locuaz/sample_bin/dlpacker/charges.rtp`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/sample_bin/haddock/template_scoring.inp` & `locuaz-0.3.7/locuaz/sample_bin/haddock/template_scoring.inp`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/schema.yaml` & `locuaz-0.3.7/locuaz/schema.yaml`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/scoring.py` & `locuaz-0.3.7/locuaz/scoring.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/scoringfunctions.py` & `locuaz-0.3.7/locuaz/scoringfunctions.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/spm4.py` & `locuaz-0.3.7/locuaz/spm4.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/spm4i.py` & `locuaz-0.3.7/locuaz/spm4i.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/spm4mmpbsa.py` & `locuaz-0.3.7/locuaz/spm4mmpbsa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/statisticcmdistance.py` & `locuaz-0.3.7/locuaz/statisticcmdistance.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/statisticinterface.py` & `locuaz-0.3.7/locuaz/statisticinterface.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/statistics.py` & `locuaz-0.3.7/locuaz/statistics.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/utils_scoring.py` & `locuaz-0.3.7/locuaz/utils_scoring.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz/validatore.py` & `locuaz-0.3.7/locuaz/validatore.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.3.5/locuaz.egg-info/PKG-INFO` & `locuaz-0.3.7/locuaz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: locuaz
-Version: 0.3.5
+Version: 0.3.7
 Summary: Antibody optimization protocol
 Author: Patricio Barletta
 Author-email: pbarletta@gmail.com
 Keywords: molecular,dynamics,antibody,antibodies
 Requires-Python: >=3.9.15
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
```

### Comparing `locuaz-0.3.5/locuaz.egg-info/SOURCES.txt` & `locuaz-0.3.7/locuaz.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -61,12 +61,15 @@
 locuaz/validatore.py
 locuaz.egg-info/PKG-INFO
 locuaz.egg-info/SOURCES.txt
 locuaz.egg-info/dependency_links.txt
 locuaz.egg-info/entry_points.txt
 locuaz.egg-info/requires.txt
 locuaz.egg-info/top_level.txt
+locuaz/DLPacker/__init__.py
+locuaz/DLPacker/dlpacker.py
+locuaz/DLPacker/utils.py
 locuaz/sample_bin/aux_scripts/reorder_pdb.py
 locuaz/sample_bin/dlpacker/charges.rtp
 locuaz/sample_bin/gmxmmpbsa/gmxmmpbsa
 locuaz/sample_bin/haddock/template_scoring.inp
 tests/test_locuaz.py
```

### Comparing `locuaz-0.3.5/setup.cfg` & `locuaz-0.3.7/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [metadata]
 name = locuaz
-version = 0.3.5
+version = 0.3.7
 author = Patricio Barletta
 author_email = pbarletta@gmail.com
 description = Antibody optimization protocol
 long_description = file: README.rst, CHANGELOG.rst, LICENSE.rst
 long_description_content_type = text/x-rst
 keywords = molecular, dynamics, antibody, antibodies
 
 [options]
 python_requires = >=3.9.15
-packages = locuaz
+packages = 
+	locuaz
+	locuaz.DLPacker
 install_requires = 
 	py
 	scipy
 	numpy >=1.21.0,<2.0.0
 	attrs
 	chemfiles
 	mdanalysis >= 2.3.0
```

### Comparing `locuaz-0.3.5/tests/test_locuaz.py` & `locuaz-0.3.7/tests/test_locuaz.py`

 * *Files identical despite different names*

