# Comparing `tmp/locuaz-0.2.1.tar.gz` & `tmp/locuaz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locuaz-0.2.1.tar", last modified: Thu Apr 20 13:30:57 2023, max compression
+gzip compressed data, was "locuaz-0.3.1.tar", last modified: Wed May 10 09:59:29 2023, max compression
```

## Comparing `locuaz-0.2.1.tar` & `locuaz-0.3.1.tar`

### file list

```diff
@@ -1,70 +1,82 @@
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-11 13:53:32.000000 locuaz-0.2.1/CHANGELOG.rst
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1069 2023-04-11 13:54:09.000000 locuaz-0.2.1/LICENSE.rst
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8856 2023-04-20 13:30:57.951101 locuaz-0.2.1/PKG-INFO
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7475 2023-04-20 13:30:34.000000 locuaz-0.2.1/README.rst
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/locuaz/
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/locuaz/DLPacker/
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    26845 2023-04-19 14:49:18.000000 locuaz-0.2.1/locuaz/DLPacker/dlpacker.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    19402 2023-03-24 13:12:43.000000 locuaz-0.2.1/locuaz/DLPacker/utils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       22 2023-04-07 11:50:26.000000 locuaz-0.2.1/locuaz/__init__.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      849 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/abstractmutationgenerator.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1807 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/abstractscoringfunction.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    13051 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/amberutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4466 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/autodockvina.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3692 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/bach.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6734 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/basemutator.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3096 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/basestatistic.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5809 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/bluues.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7170 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/bluuesbmf.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    18852 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/cli.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7929 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/complex.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5298 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/epochinitializer.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3072 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/evoef2.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5733 2023-04-19 13:31:58.000000 locuaz-0.2.1/locuaz/fileutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6890 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/fixbox.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4317 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/gmxmmpbsa.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    15143 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/gromacsutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7700 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/haddock.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5441 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/interface.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    12472 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/molecules.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     6159 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/moleculesutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1641 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/molutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1548 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutation.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      351 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutationgenerators.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1284 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutatorbiobb.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3916 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutatordlp.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4722 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutatordlpr.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3709 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutatorevoef2.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      634 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/mutators.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4199 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/piepisa.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3069 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/pisa.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2668 2023-04-20 10:23:58.000000 locuaz-0.2.1/locuaz/primitives.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    31268 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/projectutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2383 2023-04-19 14:37:41.000000 locuaz-0.2.1/locuaz/protocol.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3943 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/pruner.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1951 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/pruners.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     3892 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/rosetta.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4656 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/run.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8927 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/runutils.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     5816 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/scoring.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      758 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/scoringfunctions.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     7125 2023-04-20 11:10:24.000000 locuaz-0.2.1/locuaz/spm4.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4608 2023-04-20 11:35:59.000000 locuaz-0.2.1/locuaz/spm4i.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8177 2023-04-20 11:35:01.000000 locuaz-0.2.1/locuaz/spm4mmpbsa.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1384 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/statisticcmdistance.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     2074 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/statisticinterface.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      984 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/stats.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     4820 2023-04-19 14:38:28.000000 locuaz-0.2.1/locuaz/utils_scoring.py
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)    10044 2023-04-19 13:23:22.000000 locuaz-0.2.1/locuaz/validatore.py
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/locuaz.egg-info/
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     8856 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/PKG-INFO
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)     1362 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/SOURCES.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        1 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/dependency_links.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       57 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/entry_points.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      208 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/requires.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)        7 2023-04-20 13:30:57.000000 locuaz-0.2.1/locuaz.egg-info/top_level.txt
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)       95 2023-04-12 11:27:33.000000 locuaz-0.2.1/pyproject.toml
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      866 2023-04-20 13:30:57.951101 locuaz-0.2.1/setup.cfg
-drwxrwxr-x   0 pbarletta  (1000) pbarletta  (1001)        0 2023-04-20 13:30:57.951101 locuaz-0.2.1/tests/
--rw-rw-r--   0 pbarletta  (1000) pbarletta  (1001)      536 2023-02-21 12:12:48.000000 locuaz-0.2.1/tests/test_locuaz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:18.000000 locuaz-0.3.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 09:59:18.000000 locuaz-0.3.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 09:59:18.000000 locuaz-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 09:59:29.936362 locuaz-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-10 09:59:18.000000 locuaz-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/abstractmutationgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/abstractpruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/abstractscoringfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/amberutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/autodockvina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/bach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/basemutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/basestatistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/bluues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/bluuesbmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/epochinitializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/evoef2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/fixbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/gmxmmpbsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/gromacsutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/haddock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/moleculesutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/molutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutationgenerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutatorbiobb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutatordlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutatordlpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutatorevoef2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/piepisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/pisa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/projectutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/prunerconsensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/prunermetropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/pruners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/rosetta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/runutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.924362 locuaz-0.3.1/locuaz/sample_bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/sample_bin/aux_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/sample_bin/aux_scripts/reorder_pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/sample_bin/dlpacker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70622 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/sample_bin/dlpacker/charges.rtp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/sample_bin/gmxmmpbsa/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/sample_bin/gmxmmpbsa/gmxmmpbsa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz/sample_bin/haddock/
+-rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/sample_bin/haddock/template_scoring.inp
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/scoringfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/spm4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/spm4i.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/spm4mmpbsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/statisticcmdistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/statisticinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/utils_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-10 09:59:19.000000 locuaz-0.3.1/locuaz/validatore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/locuaz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 09:59:29.000000 locuaz-0.3.1/locuaz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-10 09:59:19.000000 locuaz-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-10 09:59:29.936362 locuaz-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:59:29.932362 locuaz-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 09:59:19.000000 locuaz-0.3.1/tests/test_locuaz.py
```

### Comparing `locuaz-0.2.1/LICENSE.rst` & `locuaz-0.3.1/LICENSE.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) [2023] [Patricio Barletta]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `locuaz-0.2.1/locuaz/abstractmutationgenerator.py` & `locuaz-0.3.1/locuaz/abstractmutationgenerator.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/abstractscoringfunction.py` & `locuaz-0.3.1/locuaz/abstractscoringfunction.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/amberutils.py` & `locuaz-0.3.1/locuaz/amberutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,29 +85,32 @@
 
     return PDBStructure(FileHandle(out_pdb_path))
 
 
 def run_tleap(
     tleap_script: Union[FileHandle, Path], name: str
 ) -> Tuple[PDBStructure, FileHandle, FileHandle]:
-    """run_tleap(): runs tleap script and then uses a local PDB to add chainID info
+    """runs tleap script and then uses a local PDB to add chainID info
     to the .prmtop and box info to the .rst7. Then it uses both to overwrite the
     PDB to keep everything in sync (in case, for example, that the tleap script
     added ions)
 
-
-    Args:
-        tleap_script (Union[FileHandle, Path]): script that loads a local PDB and
-        outputs a .prmtop and a .rst7 file
-        name (str): name of the system
-
-    Returns:
-        Tuple[PDBStructure, FileHandle, FileHandle]: PDB, .prmtop and .rst7
+    Parameters
+    ----------
+    tleap_script : Union[FileHandle, Path]
+        script that loads a local PDB and outputs a .prmtop and a .rst7 file
+    name : str
+        name of the system
+
+    Returns
+    -------
+    .pdb, .prmtop and .rst7: Tuple[PDBStructure, FileHandle, FileHandle]
+        The ``.prmtop`` and the ``.rst7`` are the output of the tleap script,
+        and both are read by parmed to generate the ``.pdb``.
     """
-
     local_dir = Path(tleap_script).parent
 
     p = sp.run(
         f"tleap -f {Path(tleap_script)}",
         stdout=sp.PIPE,
         stderr=sp.PIPE,
         cwd=local_dir,
```

### Comparing `locuaz-0.2.1/locuaz/autodockvina.py` & `locuaz-0.3.1/locuaz/autodockvina.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,64 +23,45 @@
         # Get PDBQT file for target
         target_pdb = f"../target-{i}.pdb"
         target_pdbqt = f"target-{i}.pdbqt"
 
         comando_ob_target = \
             f"{self.openbabel_bin} -ipdb {target_pdb} -O {target_pdbqt} --partialcharge gasteiger  ---errorlevel 0"
 
-        p = sp.run(
-            comando_ob_target,
-            stdout=sp.PIPE,
-            stderr=sp.PIPE,
-            cwd=self.results_dir,
-            shell=True,
-            text=True,
-        )
+        p = sp.run(comando_ob_target, stdout=sp.PIPE, stderr=sp.PIPE, cwd=self.results_dir, shell=True,text=True)
+
         self.__assert_scoring_function_outfile__(Path(self.results_dir, target_pdbqt), stdout=p.stdout, stderr=p.stderr,
                                                  command=comando_ob_target)
         # Get PDBQT file for binder
         binder_pdb = f"../binder-{i}.pdb"
         binder_pdbqt = f"binder-{i}.pdbqt"
 
         comando_ob_binder = \
             f"{self.openbabel_bin} -ipdb {binder_pdb} -O {binder_pdbqt} --partialcharge gasteiger -xr ---errorlevel 0"
 
-        p = sp.run(
-            comando_ob_binder,
-            stdout=sp.PIPE,
-            stderr=sp.PIPE,
-            cwd=self.results_dir,
-            shell=True,
-            text=True,
-        )
+        p = sp.run(comando_ob_binder, stdout=sp.PIPE, stderr=sp.PIPE, cwd=self.results_dir, shell=True, text=True)
+
         self.__assert_scoring_function_outfile__(Path(self.results_dir, binder_pdbqt), stdout=p.stdout, stderr=p.stderr,
                                                  command=comando_ob_binder)
 
         comando_vina = f"{self.bin_path} --score_only --ligand {target_pdbqt} --receptor {binder_pdbqt} --autobox"
 
-        p = sp.run(
-            comando_vina,
-            stdout=sp.PIPE,
-            stderr=sp.PIPE,
-            cwd=self.results_dir,
-            shell=True,
-            text=True,
-        )
+        p = sp.run(comando_vina, stdout=sp.PIPE, stderr=sp.PIPE, cwd=self.results_dir, shell=True, text=True)
 
         autodockvina_score = self.__parse_stdout__(
             score_stdout=p.stdout, original_command=comando_vina
         )
 
         return i, autodockvina_score
 
     def __parse_stdout__(self, score_stdout: str, original_command: str) -> float:
 
         try:
             autodockvina_score = float(self.rgx.search(score_stdout).group(1))
-        except (ValueError, IndexError) as e:
+        except (ValueError, IndexError, Exception) as e:
             raise ValueError(
                 f"{self} couldn't parse {score_stdout}\nfrom: \n{original_command}"
             ) from e
 
         return autodockvina_score
 
     def __call__(
```

### Comparing `locuaz-0.2.1/locuaz/bach.py` & `locuaz-0.3.1/locuaz/bach.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/basemutator.py` & `locuaz-0.3.1/locuaz/basemutator.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/basestatistic.py` & `locuaz-0.3.1/locuaz/basestatistic.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/bluues.py` & `locuaz-0.3.1/locuaz/bluues.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/bluuesbmf.py` & `locuaz-0.3.1/locuaz/bluuesbmf.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/cli.py` & `locuaz-0.3.1/locuaz/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import argparse
 import glob
 import os
 import pickle
 import shutil as sh
 import sys
-import warnings
+from warnings import warn, simplefilter
 from collections import defaultdict
 from itertools import product
 from pathlib import Path
 from queue import PriorityQueue
 from typing import Dict, List, Final, Set, Tuple, Union, Any
 
 import yaml
+import networkx as nx
 
 from locuaz.validatore import Validatore
 from locuaz.primitives import UserInputError
 
 
 def get_dir_size(folder: Path) -> float:
     B_TO_MB: Final = 1048576
@@ -50,18 +51,15 @@
     if not validator.validate(raw_config):  # type: ignore
         raise ValueError(validator.errors)  # type: ignore
     else:
         config = validator.normalized(raw_config)  # type: ignore
 
     # Check mode
     if mode != config["main"]["mode"]:
-        warnings.warn(
-            f"Warning, CLI input {mode} doesn't match {config['main']['mode']}."
-            f"Overwriting option."
-        )
+        warn(f"Warning, CLI input {mode} doesn't match {config['main']['mode']}. Overwriting option.")
         config["main"]["mode"] = mode
 
     config["main"]["debug"] = debug
 
     # Check input work dir
     if Path(config["paths"]["work"]).is_dir():
         start = False
@@ -76,35 +74,44 @@
 
     # Check use of tleap
     if config["md"].get("use_tleap", False):
         assert "tleap" in config["paths"], f"Specify path to tleap files."
         assert (
                 get_dir_size(config["paths"]["tleap"]) < 10
         ), f"tleap dir is heavier than 10Mb. Choose a dir with only the necessary tleap files."
-        warnings.warn(
+        warn(
             "tleap script will be used. Options: 'water_type' and 'force_field' will be ignored.")
 
     # Check matching lengths of mutating_resSeq and mutating_resname.
     for resnames, resSeqs in zip(config["binder"]["mutating_resname"], config["binder"]["mutating_resSeq"]):
         assert len(resnames) == len(resSeqs), f"mutating_resname({resnames}) and mutating_resSeq ({resSeqs}) have " \
                                               f"different lengths: {len(resnames)} and {len(resSeqs)}, respectively."
 
     # Check 'branches' and 'generator'
     if ("SPM4" in config["generation"]["generator"]) and (config["protocol"]["branches"] > 19):
         raise UserInputError(f"SPM4 mutation generators cannot generate more than 19 branches")
 
     check_gmxmmpbsa(config)
 
+    # Check consensus threshold and scoring functions
+    if config["pruning"]["pruner"] == "consensus":
+        assert "consensus_threshold" in config["pruning"], "Set 'consensus_threshold' when using 'consensus' pruner."
+        t = config["pruning"]["consensus_threshold"]
+        n = len(config["scoring"]["functions"])
+        assert t <= n, f"Threshold ({t}) should be equal or lower than the number of scoring functions ({n})"
+    elif config["pruning"]["pruner"] == "metropolis":
+        assert len(config["scoring"]["functions"]) == 1, f"Can only use 1 scoring function when pruner is 'metropolis'."
+
     return config, start
 
 
 def backup_iteration(it_fn: Union[str, Path]) -> None:
     it_path = Path(it_fn)
     new_path = Path(it_path.parent, "bu_" + it_path.name)
-    warnings.warn(f"Found incomplete epoch. Will backup {it_path} to {new_path}")
+    warn(f"Found incomplete epoch. Will backup {it_path} to {new_path}")
     sh.move(it_path, new_path)
 
 
 def append_iterations(
         sorted_iters: PriorityQueue, iterations: List, prev_epoch: int
 ) -> str:
     if sorted_iters.empty():
@@ -172,91 +179,89 @@
     for it_fn in iterations:
         it_path = Path(it_fn)
         if int(it_path.name.split("-")[0]) == starting_epoch:
             return False
     return True
 
 
-def lacks_branches(
-        current_iterations: Union[List[str], List[Path]],
-        *,
-        branches: int,
-        starting_epoch: int,
-        prevent_fewer_branches: bool,
-) -> bool:
-    if prevent_fewer_branches:
-        # Check that the epoch wasn't cut short during its initialization. This may
-        # happen if last run was cut during initialize_new_epoch().
+def lacks_branches(current_iterations: Union[List[str], List[Path]],
+                   top_iterations: Union[List[str], List[Path]], config: Dict[str, Any]) -> bool:
+    if config["protocol"]["prevent_fewer_branches"]:
+        if config["protocol"]["constant_width"]:
+            branches = config["protocol"]["branches"]
+        else:
+            n_top_iters = 1 if len(top_iterations) == 0 else len(top_iterations)
+            branches = config["protocol"]["branches"] * n_top_iters
         nbr_branches = len(current_iterations)
+        starting_epoch = config["main"]["starting_epoch"]
+
+        # Check that the epoch wasn't cut short during its initialization.
+        # This may happen if last run was cut during initialize_new_epoch().
         if nbr_branches < branches and is_not_epoch_0(current_iterations, starting_epoch):
             for it_fn in current_iterations:
                 backup_iteration(it_fn)
             return True
     return False
 
 
+def read_key_from_tracking_file(config: Dict[str, Any], tracking: Dict[str, Any], attr: str) -> Dict[str, Any]:
+    try:
+        config[attr] = tracking[attr]
+    except (Exception,):
+        warn(f"Could not read {attr} tree from tracking file.")
+    return config
+
+
 def get_tracking_files(config: Dict) -> bool:
     tracking_pkl = Path(config["paths"]["work"], "tracking.pkl")
 
     try:
         with open(tracking_pkl, "rb") as file:
             tracking: Dict[str, Any] = pickle.load(file)
     except (Exception,):
-        warnings.warn("Could not read tracking file.")
+        warn("Could not read tracking file.")
         return False
     try:
-        previous_iterations = get_valid_iter_dirs(
-            tracking["previous_iterations"], config
-        )
+        previous_iterations = get_valid_iter_dirs(tracking["previous_iterations"], config)
         current_iterations = get_valid_iter_dirs(tracking["current_iterations"], config)
         top_iterations = get_valid_iter_dirs(tracking["top_iterations"], config)
 
-        if lacks_branches(
-                current_iterations,
-                branches=config["protocol"]["branches"],
-                starting_epoch=config["main"]["starting_epoch"],
-                prevent_fewer_branches=config["protocol"]["prevent_fewer_branches"],
-        ):
-            warnings.warn("Will ignore the tracking file. The current iterations field is invalid.")
+        if lacks_branches(current_iterations, top_iterations, config):
+            warn("Will ignore the tracking file. The current iterations field is invalid.")
             return False
 
         config["paths"]["previous_iterations"] = previous_iterations
         config["paths"]["current_iterations"] = current_iterations
         config["paths"]["top_iterations"] = top_iterations
-        config["misc"]["epoch_mutated_positions"] = set(
-            tracking["epoch_mutated_positions"]
-        )
+        config["misc"]["epoch_mutated_positions"] = set(tracking["epoch_mutated_positions"])
+
         if "memory_positions" in config["protocol"]:
-            warnings.warn(
-                f"Tracking file memory_positions ignored: "
-                f'{tracking["memory_positions"]}.\n'
-                f"Using input config memory_positions instead: "
-                f'{config["protocol"]["memory_positions"]}'
-            )
+            warn(f"Tracking file's 'memory_positions' ignored: {tracking['memory_positions']}.\n"
+                 f"Using input config 'memory_positions' instead: {config['protocol']['memory_positions']}")
         else:
             config["protocol"]["memory_positions"] = tracking["memory_positions"]
 
         if "failed_memory_positions" in config["protocol"]:
-            warnings.warn(
-                f"Tracking file failed_memory_positions ignored: "
-                f'{tracking["failed_memory_positions"]}.\n'
-                f"Using input config failed_memory_positions instead: "
-                f'{config["protocol"]["failed_memory_positions"]}'
-            )
+            warn(f"Tracking file's 'failed_memory_positions' ignored: {tracking['failed_memory_positions']}.\n"
+                 "Using input config 'failed_memory_positions' instead: "
+                 f"{config['protocol']['failed_memory_positions']}")
         else:
-            config["protocol"]["failed_memory_positions"] = tracking[
-                "failed_memory_positions"
-            ]
-        return True
+            config["protocol"]["failed_memory_positions"] = tracking["failed_memory_positions"]
+
+        # Read options related to the DAGs
+        for key in ("project_dag", "project_mut_dag", "mutations"):
+            config = read_key_from_tracking_file(config, tracking, key)
+
     except (Exception,):
-        warnings.warn("Will ignore the tracking file. It is in an invalid state with respect to the working dir.")
+        warn("Will ignore the tracking file. It is in an invalid state with respect to the working dir.")
         return False
 
+    return True
 
-def set_iterations(config: Dict) -> None:
+def set_iterations(config: Dict) -> Dict:
     """set_iterations Set config["paths"]["current_iterations"],
     config["paths"]["previous_iterations"] and possibly config["paths"]["top_iterations"].
 
     Args:
         config (Dict): dictionary with input config
 
     Raises:
@@ -270,27 +275,22 @@
         nbr, *_ = iter_path.name.split("-")
         iters.put((-int(nbr), iter_path))
     # Iterations are sorted by epoch number now
     while not iters.empty():
         config["paths"]["current_iterations"] = []
         iter_str = append_iterations(iters, config["paths"]["current_iterations"], 1)
 
-        if lacks_branches(
-                config["paths"]["current_iterations"],
-                branches=config["protocol"]["branches"],
-                starting_epoch=config["main"]["starting_epoch"],
-                prevent_fewer_branches=config["protocol"]["prevent_fewer_branches"],
-        ):
+        if lacks_branches(config["paths"]["current_iterations"], [], config):
             # Start over, this time, the incomplete epoch will not be in `iters`.
             continue
 
         if iter_str != "":
             config["paths"]["previous_iterations"] = []
             append_iterations(iters, config["paths"]["previous_iterations"], 1)
-        return
+        return config
     raise ValueError("No valid iterations in work_dir. Aborting.")
 
 
 def check_gmxmmpbsa(config: Dict) -> None:
     if config["generation"]["generator"] == "SPM4gmxmmpbsa":
         if "gmxmmpbsa" not in config["scoring"]["functions"]:
             print(f"'gmxmmbpsa' function is necessary to use the 'SPM4mmpbsa' mutator",
@@ -375,22 +375,22 @@
         # Reformat the paths
         epoch_iternames = [
             Path(iter_str).name.split("-")[1:] for iter_str in epoch_iters_paths
         ]
         # Check in case the mutating chains/residues have changed:
         for iterchains in epoch_iternames:
             if len(iterchains) != input_n_chains:
-                warnings.warn(
+                warn(
                     f"Can't fill requested memory since input 'mutating_chainID' does not "
                     f" match the 'mutating_chainID' previously used on this workspace."
                 )
                 return set(), [[]]
             old_n_resSeqs = [len(itername[2:]) for itername in iterchains]
             if old_n_resSeqs != input_n_resSeqs:
-                warnings.warn(
+                warn(
                     f"Can't fill requested memory since input 'mutating_resSeq' does not "
                     f" match the 'mutating_resSeq' previously used on this workspace."
                 )
                 return set(), [[]]
 
         # Find the positions and chains that were mutated in this epoch
         memory_positions = set()
@@ -412,17 +412,23 @@
         f'{config["protocol"]["memory_size"]} previous epochs.',
         flush=True,
     )
     # Get the mutated positions on the last epoch
     return set(all_memory_positions[0]), all_memory_positions
 
 
+def set_empty_dags(config: Dict) -> Dict:
+    config["project_dag"] = nx.DiGraph()
+    config["project_mut_dag"] = nx.DiGraph()
+    return config
+
+
 def main() -> Tuple[Dict, bool]:
     """Console script for locuaz."""
-    warnings.simplefilter("default")
+    simplefilter("default")
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "config_file",
         help="File containing all the necessary parameters to run the protocol",
     )
     parser.add_argument(
         "-m",
@@ -455,15 +461,16 @@
         if get_tracking_files(config):
             print("Read tracking file from work dir.", flush=True)
         else:
             print(
                 "Will try to get the previous iterations, the current iterations and the memory of the "
                 "last mutated positions from the work dir. Memory of failed mutations won't be loaded.",
                 flush=True)
-            set_iterations(config)
+            config = set_iterations(config)
+            config = set_empty_dags(config)
             # Set up the memory
             requested_memory = "memory_size" in config["protocol"]
             if requested_memory:
                 epoch_mutated_positions, memory_positions = get_memory(config)
                 config["misc"]["epoch_mutated_positions"] = epoch_mutated_positions
                 has_no_memory = not ("memory_positions" in config["protocol"])
                 if has_no_memory:
@@ -471,11 +478,11 @@
             else:
                 config["misc"]["epoch_mutated_positions"] = set()
 
     # Set up environment
     os.environ["OMP_PLACES"] = "threads"
     omp_procs_str = str(config["md"]["omp_procs"])
     if os.environ.get("OMP_NUM_THREADS", "") != omp_procs_str:
-        warnings.warn(f"Setting 'OMP_NUM_THREADS' environment variable to input 'omp_procs' {omp_procs_str}")
+        warn(f"Setting 'OMP_NUM_THREADS' environment variable to input 'omp_procs' {omp_procs_str}")
         os.environ["OMP_NUM_THREADS"] = omp_procs_str
 
     return config, starts
```

### Comparing `locuaz-0.2.1/locuaz/complex.py` & `locuaz-0.3.1/locuaz/complex.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/epochinitializer.py` & `locuaz-0.3.1/locuaz/epochinitializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,68 +30,75 @@
     # Create required mutator
     mutator = mutators[work_pjct.config["mutation"]["mutator"]](
         work_pjct.config["paths"]["mutator"], work_pjct.config["mutation"]["reconstruct_radius"]
     )
     # Create required mutation generator and generate mutation.
     generator = mutation_generators[work_pjct.config["generation"]["generator"]]
     successful_mutations = 0
-    while successful_mutations < work_pjct.config["protocol"]["branches"]:
+
+    if work_pjct.config["protocol"]["constant_width"]:
+        branches = work_pjct.config["protocol"]["branches"]
+    else:
+        branches = work_pjct.config["protocol"]["branches"] * len(old_epoch.top_iterations)
+
+    # Usually, this `while` would only be executed once, unless the Mutator program fails to perform a mutation.
+    while successful_mutations < branches:
         mutation_generator = generator(
             old_epoch,
-            work_pjct.config["protocol"]["branches"] - successful_mutations,
+            branches - successful_mutations,
             excluded_aas=work_pjct.get_mem_aminoacids(),
             excluded_pos=work_pjct.get_mem_positions(),
             use_tleap=work_pjct.config["md"]["use_tleap"],
             logger=log,
-            probe_radius=work_pjct.config["generation"]["probe_radius"]
-        )
+            probe_radius=work_pjct.config["generation"]["probe_radius"])
 
         for old_iter_name, mutations in mutation_generator.items():
             old_iter = old_epoch.top_iterations[old_iter_name]
 
-            # GROMACS renumbers resSeqs to strided numbering. If using Amber's continuous
-            # numbering, this will result in the wrong mutating_resSeq.
             if work_pjct.config["md"]["use_tleap"]:
-                # Backup the PDB before runing pdb4amber
+                # GROMACS renumbers resSeqs to strided numbering. If using Amber's continuous
+                # numbering, this will result in the wrong mutating_resSeq.
+                # Backup the PDB before running pdb4amber
                 pdb_path = Path(old_iter.complex.pdb)
                 pre_fix_pdb = Path(old_iter.dir_handle, f"preAmberPDBFixer_{pdb_path.stem}.pdb")
                 sh.move(pdb_path, pre_fix_pdb)
 
                 old_pdb = fix_pdb(pre_fix_pdb, pdb_path)
             else:
                 old_pdb = old_iter.complex.pdb
 
             for mutation in mutations:
-                iter_name, iter_resnames = mutation.new_name_resname(old_iter)
+                iter_name, iter_resnames = old_iter.generate_name_resname(mutation)
                 iter_path = Path(work_pjct.dir_handle, f"{epoch_id}-{iter_name}")
 
                 this_iter = Iteration(
                     DirHandle(iter_path, make=True),
                     iter_name=iter_name,
                     chainIDs=old_iter.chainIDs,
                     resnames=iter_resnames,
-                    resSeqs=old_iter.resSeqs)
+                    resSeqs=old_iter.resSeqs,
+                    parent=old_iter,
+                    mutation=mutation)
 
                 init_wt = Path(iter_path, "init_wt.pdb")
                 sh.copy(old_pdb, init_wt)
                 log.info(f"New mutation: {mutation} on Epoch-Iteration: {epoch_id}-{iter_name}")
 
                 # Mutate the PDB
                 with warnings.catch_warnings():
                     warnings.simplefilter("ignore")
                     try:
                         overlapped_pdb = mutator.on_pdb(
                             PDBStructure.from_path(init_wt),
                             iter_path,
                             mutation=mutation,
                             selection_complex=old_iter.complex.top.selection_complex,
-                            selection_wations=old_iter.complex.top.selection_not_complex,
-                        )
+                            selection_wations=old_iter.complex.top.selection_not_complex)
                     except AssertionError as e:
-                        # Mutator failed
+                        # Mutator failed. This position will still be memorized.
                         log.info(f"Mutation of {iter_name} failed. Will try with another one. Backing-up {iter_path} .")
                         print(e, file=sys.stderr)
                         failed_iter_path = Path(work_pjct.dir_handle, f"failed_{epoch_id}-{iter_name}")
                         sh.move(iter_path, failed_iter_path)
                         continue
                 remove_overlapping_solvent(
                     overlapped_pdb,
```

### Comparing `locuaz-0.2.1/locuaz/evoef2.py` & `locuaz-0.3.1/locuaz/evoef2.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/fileutils.py` & `locuaz-0.3.1/locuaz/fileutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/fixbox.py` & `locuaz-0.3.1/locuaz/fixbox.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/gmxmmpbsa.py` & `locuaz-0.3.1/locuaz/gmxmmpbsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from locuaz.abstractscoringfunction import AbstractScoringFunction
 from locuaz.complex import GROComplex
 from locuaz.fileutils import DirHandle, FileHandle
 from locuaz.molecules import ZipTopology
 
 
 class GmxMmpbsa(AbstractScoringFunction):
-    bin_name = "gmx_MMPBSA"
+    bin_name = "gmxmmpbsa"
     TIMEOUT_PER_FRAME: int = 20
 
     def __init__(self, sf_dir, *, nthreads=2, mpiprocs=2) -> None:
         super().__init__(sf_dir, nthreads=nthreads, mpiprocs=mpiprocs)
         # `gmxmmpbsa` isn't actually the binary, but the config file
         # This happens because gmx_MMPBSA is the only SF that comes with the protocol instead of
         # being an external binary.
```

### Comparing `locuaz-0.2.1/locuaz/gromacsutils.py` & `locuaz-0.3.1/locuaz/gromacsutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     # First, get a PDB with the same topology as `cluster_trj`.
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         orig_pdb = Path(wrk_dir, "orig.pdb")
         # Selection
         orig_u.select_atoms(cpx.top.selection_complex).write(str(orig_pdb))
     u = mda.Universe(str(orig_pdb), str(cluster_trj))
+    # noinspection all
     u.trajectory[2]  # type: ignore
     cluster_gro = Path(wrk_dir, "clustered.gro")
     u.atoms.write(str(cluster_gro))  # type: ignore
 
     nojump_trj = Path(wrk_dir, "nojump.xtc")
     fix_jump = GMXImage(
         input_traj_path=str(cluster_trj),
@@ -116,14 +117,15 @@
         },
     )
     launch_biobb(center)
 
     # Finally, get the last frame of the trajectory and leave it in case the user wants to check it.
     out_pdb_fn = Path(out_trj_fn.parent, out_trj_fn.stem + ".pdb")
     u = mda.Universe(str(orig_pdb), str(out_trj_fn))
+    # noinspection all
     u.trajectory[-1]
     if not use_tleap:
         # Staggered resSeq
         for s in u.segments:
             if s.segid in {'', 'X'}:
                 break
             s.residues.resids = np.array(range(1, len(s.residues) + 1))
@@ -198,14 +200,15 @@
     ndx = FileHandle(ndx_fn_out)
     update_header(ndx, f"[ non_overlapping ]\n")
 
     wat_count = wat_atoms // 3
 
     return ndx, wat_count
 
+
 def remove_overlapping_waters(complex: GROComplex, config: Dict, overlapped_resSeq: int) -> GROComplex:
     """DEPRECATED remove_overlapping_waters takes a complex and removes all the waters that
     are within a certain cutoff from `overlapped_resSeq`. Then it replaces them.
     It does a lot of gymnastics to deal with Gromacs weirdness.
 
     Args:
         config (Dict): work project's config file
@@ -318,23 +321,34 @@
     return new_complex
 
 
 def fix_gromacs_pdb(
         pdb_in_fn: Path, pdb_out_fn: Path, *, new_chainID: Optional[str] = None,
         allowed_nonstandard_residues: Optional[Set] = None,
 ) -> Path:
-    """fix_gromacs_pdb uses Bio to add TER between chains, END at the end,
-    and manually make the resSeq numbers continuous.
-    Since this changes the PBD numbering it should only be used for structures
-    to be used for scoring.
-    Specifically, Haddock, that requires chains to have unique resSeq numbers.
-
-    Args:
-        pdb_in_fn (Path): Path to input PDB.
-        pdb_out_fn (Path): Path to output PDB.
+    """
+    uses Bio to add TER between chains, END at the end, and manually make the resSeq numbers continuous.
+    Since this changes the PBD numbering it should only be used for structures to be used for scoring.
+    For ex., Haddock requires chains to have unique resSeq numbers.
+
+    Parameters
+    ----------
+    pdb_in_fn : Path
+        input PDB
+    pdb_out_fn : Path
+        output PDB
+    new_chainID : Optional[str]
+        For assigning a new chain ID to all atoms in the output PDB
+    allowed_nonstandard_residues : Optional[set]
+        Any residue not present in AA_MAP or in this set will be discarded from the output PDB.
+        Useful when scoring complexes with ligands.
+    Returns
+    -------
+    the output PDB : Path
+        the PDB will be written with Biopython's PDB tools.
     """
     if not allowed_nonstandard_residues:
         allowed_nonstandard_residues = set()
     parsero = PDBParser(QUIET=True)
     pdb = parsero.get_structure("foo", file=pdb_in_fn)
 
     # Modifying resSeq, chainID and mapping resnames to standard resnames.
```

### Comparing `locuaz-0.2.1/locuaz/haddock.py` & `locuaz-0.3.1/locuaz/haddock.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/interface.py` & `locuaz-0.3.1/locuaz/interface.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/molecules.py` & `locuaz-0.3.1/locuaz/molecules.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/moleculesutils.py` & `locuaz-0.3.1/locuaz/moleculesutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/molutils.py` & `locuaz-0.3.1/locuaz/molutils.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/mutatorbiobb.py` & `locuaz-0.3.1/locuaz/mutatorbiobb.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/mutatordlp.py` & `locuaz-0.3.1/locuaz/mutatordlp.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/mutatordlpr.py` & `locuaz-0.3.1/locuaz/mutatordlpr.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/mutatorevoef2.py` & `locuaz-0.3.1/locuaz/mutatorevoef2.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/mutators.py` & `locuaz-0.3.1/locuaz/mutators.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/piepisa.py` & `locuaz-0.3.1/locuaz/piepisa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/pisa.py` & `locuaz-0.3.1/locuaz/pisa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/primitives.py` & `locuaz-0.3.1/locuaz/primitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from typing import Dict, Optional
 from pathlib import Path
 import shutil as sh
+from warnings import warn
+
+from Bio.SeqUtils import seq1
 
 # This will be used to map non-conventional AAs to conventional ones, so the
 # scoring functions don't fail.
 AA_MAP: Dict[str, str] = {
     "ALA": "ALA",
     "ARG": "ARG",
     "ASN": "ASN",
@@ -86,7 +89,17 @@
         name (str): filename with or without the extension.
         suffix (str): desired extension.
 
     Returns:
         str: filename with the extension.
     """
     return f"{name.split('.')[0]}.{suffix}"
+
+def my_seq1(resn_3: str) -> str:
+    resn_1 = seq1(resn_3)
+    if resn_1 == 'X':
+        try:
+            resn_1 = seq1(AA_MAP[resn_3])
+            warn(f"Converted non-standard residue {resn_3} from 3-letter code to 1-letter: {resn_1}.")
+        except KeyError:
+            warn(f"Could not convert non-standard residue {resn_3} from 3-letter code to 1-letter. Setting it to 'X'.")
+    return resn_1
```

### Comparing `locuaz-0.2.1/locuaz/projectutils.py` & `locuaz-0.3.1/locuaz/projectutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from collections import deque
 from collections.abc import MutableMapping
 # TODO: replace own pairwise with itertools' on 3.10
 # from itertools import pairwise
 from itertools import tee, zip_longest
 from pathlib import Path
 from queue import PriorityQueue
-from statistics import mean, stdev
 from typing import (
     Iterable,
     Iterator,
     List,
     Set,
     Dict,
     Tuple,
@@ -25,21 +24,24 @@
 from warnings import warn
 from numpy.typing import NDArray
 
 import MDAnalysis as mda
 import numpy as np
 from Bio.SeqUtils import seq1
 from attrs import define, field, validators
+import matplotlib.pyplot as plt
+import networkx as nx
 
 from locuaz.abstractscoringfunction import AbstractScoringFunction
 from locuaz.complex import AbstractComplex, GROComplex
 from locuaz.fileutils import FileHandle, DirHandle, copy_to
-from locuaz.primitives import AA_MAP
+from locuaz.primitives import AA_MAP, my_seq1
 from locuaz.scoringfunctions import scoringfunctions
 from locuaz.interface import get_freesasa_residues
+from locuaz.mutation import Mutation
 
 
 # TODO: replace own pairwise with itertools' on 3.10
 def pairwise(iterable):
     # pairwise('ABCDEFG') --> AB BC CD DE EF FG
     a, b = tee(iterable)
     next(b, None)
@@ -51,14 +53,16 @@
     dir_handle: DirHandle = field(converter=DirHandle)  # type: ignore
     iter_name: str = field(converter=str, kw_only=True)
     chainIDs: List[str] = field(kw_only=True, validator=validators.instance_of(list))
     resnames: List[str] = field(kw_only=True, validator=validators.instance_of(list))
     resSeqs: List[List[int]] = field(
         kw_only=True, validator=validators.instance_of(list)
     )  # Had to use validators.instance_of() instead of converter because mypy complains
+    parent: Optional["Iteration"] = field(kw_only=True, default=None)
+    mutation: Optional[Mutation] = field(kw_only=True, default=None)
     epoch_id: int = field(converter=int, init=False)
     complex: Union[AbstractComplex, GROComplex] = field(init=False)
     score_dir: DirHandle = field(converter=DirHandle, init=False)  # type: ignore
     scores: Dict[str, tuple] = field(init=False)
     mean_scores: Dict[str, float] = field(init=False)
     stats: Dict[str, NDArray] = field(init=False)
     outside_box: bool = field(init=False, default=False)
@@ -74,18 +78,18 @@
 
     def set_score(
             self, sf_name: str, scores: Iterable, log: Optional[logging.Logger] = None
     ) -> float:
         if not log:
             log = logging.getLogger("root")
         self.scores[sf_name] = tuple(scores)
-        avg_score = mean(scores)
+        avg_score: float = np.mean(scores)
         self.mean_scores[sf_name] = avg_score
 
-        std_score = stdev(scores)
+        std_score = np.std(scores)
         if abs(avg_score) < std_score:
             log.warning(
                 f"{sf_name} score has a mean of {avg_score:.5f} and a std dev of {std_score:.5f}. "
                 f"This is too much variance. You might want to check {self.epoch_id}-{self.iter_name}"
             )
         return self.mean_scores[sf_name]
 
@@ -130,14 +134,23 @@
                 with open(scores_fn, "r") as f:
                     self.set_score(SF, [float(linea.strip()) for linea in f], log)
             except FileNotFoundError as e:
                 log.warning(f"{self.epoch_id}-{self.iter_name} was not scored with {SF}.")
                 return False
         return True
 
+    def mutation_str(self) -> Optional[str]:
+        if self.mutation:
+            return self.mutation.to_str()
+        else:
+            return None
+
+    def full_name(self) -> str:
+        return f"{self.epoch_id}-{self.iter_name}"
+
     def __str__(self) -> str:
         return str(self.dir_handle)
 
     def __fspath__(self) -> str:
         return str(self.dir_handle)
 
     def __truediv__(self, key) -> Union[FileHandle, "DirHandle"]:
@@ -152,14 +165,42 @@
         Args:
             other (Iteration): another iteration object.
         Returns:
             bool: first iteration in alphabetical order according to its name.
         """
         return self.iter_name < other.iter_name
 
+    def generate_name_resname(self, mutation: Mutation) -> Tuple[str, List[str]]:
+        """
+        returns the name of the iteration that would be generated by the input mutation.
+        It also returns a list with the resnames (1-letter names) of each mutated sequence (CDR),
+        also including the one that would be mutated.
+        Parameters
+        ----------
+        mutation : Mutation
+
+        Returns
+        -------
+        iteration_name and resnames: Tuple[str, List[str]]
+        """
+        iter_name = ""
+        new_iteration_resnames = []
+        for idx, (chainID, resname) in enumerate(zip(self.chainIDs, self.resnames)):
+            if idx == mutation.chainID_idx:
+                # This is the mutated chainID
+                new_resname = resname[: mutation.resSeq_idx] + mutation.new_aa + resname[mutation.resSeq_idx + 1:]
+            else:
+                # This one remains the same
+                new_resname = "".join([residue for residue in resname])
+            iter_name += f"-{chainID}_{new_resname}"
+            new_iteration_resnames.append(new_resname)
+
+        # Drop the leading '-'
+        return iter_name[1:], new_iteration_resnames
+
 
 @define
 class Epoch(MutableMapping):
     id: int = field(converter=int)
     iterations: Dict[str, Iteration] = field(kw_only=True)
     nvt_done: bool = field(converter=bool, default=False, kw_only=True)
     npt_done: bool = field(converter=bool, default=False, kw_only=True)
@@ -241,14 +282,16 @@
 class WorkProject:
     config: Dict
     name: str
     dir_handle: DirHandle
     epochs: List[Epoch]
     mdps: Dict[str, FileHandle]
     scorers: Dict[str, AbstractScoringFunction] = {}
+    project_dag: nx.DiGraph = nx.DiGraph()
+    project_mut_dag: nx.DiGraph = nx.DiGraph()
     mutated_positions: Deque[Set[int]] = deque(set())
     mutated_aminoacids: Deque[Set[str]] = deque(set())
     failed_mutated_positions: Deque[Set[int]] = deque(set())
     has_memory: bool = False
     has_failed_memory: bool = False
     tleap_dir: Optional[DirHandle] = None
 
@@ -279,18 +322,21 @@
     def __start_work__(self, log: logging.Logger):
         starting_epoch = self.config["main"]["starting_epoch"]
         zero_epoch = Epoch(starting_epoch, iterations={}, nvt_done=False, npt_done=False)
         for data_str in self.config["paths"]["input"]:
 
             # Check input PDB to create name and attributes for the starting iteration.
             input_path = Path(data_str)
-            self.__check_input_pdb__(input_path)
-            iter_name, chainIDs, resSeqs, resnames = self.__generate_iteration_ID__(
-                input_path
-            )
+            try:
+                self.__check_input_pdb__(input_path)
+            except (Exception,) as e:
+                # Remove the working dir, so it can restart easily again.
+                sh.rmtree(Path(self.config["paths"]["work"]))
+                raise e
+            iter_name, chainIDs, resSeqs, resnames = self.__generate_iteration_ID__(input_path)
 
             iter_path = Path(self.dir_handle, f"{starting_epoch}-{iter_name}")
             assert not (iter_path.is_dir() or iter_path.is_file()), f"{iter_path} exists. Wrong input path."
             this_iter = Iteration(
                 DirHandle(iter_path, make=True),
                 iter_name=iter_name,
                 chainIDs=chainIDs,
@@ -323,22 +369,18 @@
 
         zero_epoch.mutated_positions = set()
         # Finally, add the initial epoch.
         self.new_epoch(zero_epoch)
 
     def __restart_work__(self, log: logging.Logger):
         # Restart from input iterations, they should all have the same epoch number
-        epoch_nbr = int(
-            Path(self.config["paths"]["current_iterations"][0]).name.split("-")[0]
-        )
+        epoch_nbr = int(Path(self.config["paths"]["current_iterations"][0]).name.split("-")[0])
 
         if "previous_iterations" in self.config["paths"]:
-            prev_epoch = Epoch(
-                epoch_nbr - 1, iterations={}, nvt_done=True, npt_done=True
-            )
+            prev_epoch = Epoch(epoch_nbr - 1, iterations={}, nvt_done=True, npt_done=True)
             prev_epoch.top_iterations = {}
             for iter_str in self.config["paths"]["previous_iterations"]:
                 # Get `iter_name` from the input iteration dir
                 iter_name, iter_path, this_iter = self.iteration_from_str(iter_str)
                 try:
                     # Previous iterations should be fully ran.
                     this_iter.complex = GROComplex.from_complex(
@@ -356,14 +398,21 @@
 
                 # Previous iterations should be fully scored.
                 try:
                     this_iter.read_scores(self.config["scoring"]["functions"])
                 except Exception as e_score:
                     log.error(f"Previous epoch not fully scored. Run in --score mode.")
                     raise e_score
+
+                # Finally, add its mutation, if present.
+                try:
+                    this_iter.mutation = self.config["mutations"][iter_name]
+                except KeyError:
+                    this_iter.mutation = None
+                # Store it in the epoch.
                 prev_epoch[iter_name] = this_iter
 
             try:
                 prev_epoch.set_top_iter(self.config["paths"])
             except Exception as e_top_iter:
                 log.error(f"Failed to set top iteration from: {prev_epoch.keys()}")
                 raise e_top_iter
@@ -421,21 +470,27 @@
                             ignore_cpt=True,
                         )
                     except Exception as e_restart_cpx:
                         log.error(
                             f"{iter_path} is in an invalid state. Cannot build complex from it."
                         )
                         raise e_restart_cpx
-
+            # Finally, add its mutation, if present.
+            try:
+                this_iter.mutation = self.config["mutations"][iter_name]
+            except KeyError:
+                this_iter.mutation = None
+            # Store it in the epoch.
             current_epoch[iter_name] = this_iter
 
-        current_epoch.mutated_positions = set(
-            self.config["misc"]["epoch_mutated_positions"]
-        )
+        current_epoch.mutated_positions = set(self.config["misc"]["epoch_mutated_positions"])
+
         self.new_epoch(current_epoch)
+        self.project_dag = self.config["project_dag"]
+        self.project_mut_dag = self.config["project_mut_dag"]
 
     def iteration_from_str(self, iter_str: str) -> Tuple[str, Path, Iteration]:
         iter_path = Path(iter_str)
         _, *name_by_chain = iter_path.name.split("-")
         iter_name = "-".join(name_by_chain)
         # `iter_name` comes from the input iteration.
         _, chainIDs, resSeqs, resnames = self.__generate_iteration_ID__(
@@ -465,29 +520,21 @@
 
         u = mda.Universe(str(pdb_path))
         resnames = []
         for chainID, list_resSeq in zip(chainIDs, resSeqs):
             ch_resnames = []
             ch_resids = []
             cadena = u.select_atoms(f"segid {chainID}")
-            for resn, resi in {
-                (atm.resname, atm.resnum)
-                for atm in cadena.select_atoms(
-                    " or ".join([f"resid {res}" for res in list_resSeq])
-                )
-            }:
-                ch_resnames.append(resn)
+            for resn, resi in {(atm.resname, atm.resnum)
+                               for atm in cadena.select_atoms(" or ".join([f"resid {res}" for res in list_resSeq]))}:
+                ch_resnames.append(my_seq1(resn))
                 ch_resids.append(resi)
+
             resnames.append(
-                "".join(
-                    [
-                        seq1(resn_3)
-                        for resn_3 in np.array(ch_resnames)[np.argsort(ch_resids)]
-                    ]
-                )
+                "".join([resn_1 for resn_1 in np.array(ch_resnames)[np.argsort(ch_resids)]])
             )
         return resnames
 
     def __generate_iteration_ID__(
             self, input_path: Path
     ) -> Tuple[str, List[str], List[List[int]], List[str]]:
         chainIDs = self.config["binder"]["mutating_chainID"]
@@ -515,31 +562,37 @@
         segids = [s.segid for s in u.segments]  # type: ignore
         assert len(segids) > 2, "Too few segments in the input PDB. " \
                                 "There should be at least 3 (target+binder+solvent)."
 
         chainIDs = self.config["target"]["chainID"] + self.config["binder"]["chainID"]
         for segid, chainID in zip_longest(segids, chainIDs):
             if chainID:
-                assert (segid == chainID), f"PDBs chainIDs ({segids}) and input target-binder chainIDs "\
-                f"({chainIDs}) from the config should have the same ordering and the target chains should go first."
+                assert (segid == chainID), f"PDBs chainIDs ({segids}) and input target-binder chainIDs " \
+                                           f"({chainIDs}) from the config should have the same ordering and the target chains should go first."
             else:
                 assert (segid == '' or segid == 'X'), f"There're unaccounted segments. {segid} has to either be, " \
                                                       f"target or binder. If it's solvent or ions, then its segid " \
                                                       "and chainID should be empty ('') or 'X'."
 
         # Check amino acids
         all_residues = "protein or " + " or ".join(
             [f"segid {chainID}" for chainID in (self.config["target"]["chainID"] + self.config["binder"]["chainID"])])
         prot = u.atoms.select_atoms(all_residues)  # type: ignore
         aas = {res.resname for res in prot.residues}
         all_aas = set(AA_MAP.keys())
-        if not aas.issubset(all_aas):
-            warn(f"Unrecognized residues: {aas - all_aas}. Make sure you can build "
+        nonstandard_residues = aas - all_aas
+        if len(nonstandard_residues) != 0:
+            warn(f"Unrecognized residues: {nonstandard_residues}. Make sure you can build "
                  "a topology for them and that they are not necessary for scoring.")
 
+            allowed_nonstandard_residues = set(self.config["scoring"]["allowed_nonstandard_residues"])
+            if not nonstandard_residues.issubset(allowed_nonstandard_residues):
+                warn(f"Watch out, {nonstandard_residues - allowed_nonstandard_residues} were not included as "
+                     "'allowed_nonstandard_residues', make sure you don't need them for scoring.")
+
         # Check solvent
         solvent_sel = "resname WAT" if self.config["md"]["use_tleap"] else "resname SOL"
         wat = u.select_atoms(solvent_sel)
         assert len(wat), f"Input PDB lacks solvent: {solvent_sel}."
 
         # Make sure mutating residues are present.
         mutating_chainID = self.config["binder"]["mutating_chainID"]
@@ -677,61 +730,138 @@
                 self.mdps[mdp_name] = FileHandle(mdp_path)
             except Exception as e:
                 print(f"Could not get mdp file from: {mdp_path}.", flush=True)
                 raise e
 
     def new_epoch(self, epoch: Epoch, log: Optional[logging.Logger] = None) -> None:
         self.epochs.append(epoch)
+        self.update_dags()
         self.__track_project__(log)
 
+    def update_dags(self) -> None:
+
+        for iteration in self.epochs[-1].values():
+            # Iteration DAG:
+            try:
+                self.project_dag.add_edge(iteration.parent.full_name(), iteration.full_name())
+            except AttributeError:
+                # This iteration is on the 0 epoch, it has no parent.
+                self.project_dag.add_node(iteration.full_name())
+
+            # Mutational DAG:
+            try:
+                self.project_mut_dag.add_edge(iteration.parent.mutation_str(), iteration.mutation_str())
+            except ValueError:
+                # The parent iteration is on the 0 epoch and has no mutation.
+                self.project_mut_dag.add_edge("None", iteration.mutation_str())
+            except AttributeError:
+                # This iteration is on the 0 epoch, it has no parent and no mutation.
+                self.project_mut_dag.add_node("None")
+
     def __track_project__(self, log: Optional[logging.Logger] = None) -> None:
         try:
-            previous_iterations = [
-                str(pre_it.dir_handle) for pre_it in self.epochs[-2].values()
-            ]
-            current_iterations = [
-                str(cur_it.dir_handle) for cur_it in self.epochs[-1].values()
-            ]
-            top_iterations = [
-                str(cur_it.dir_handle)
-                for cur_it in self.epochs[-2].top_iterations.values()
-            ]
+            previous_iterations: List[str] = []
+            mutations: Dict[str, str] = {}
+            for iter_name, iteration in self.epochs[-2].items():
+                previous_iterations.append(str(iteration.dir_handle))
+                mutations[iter_name] = iteration.mutation
+
+            current_iterations: List[str] = []
+            for iter_name, iteration in self.epochs[-1].items():
+                current_iterations.append(str(iteration.dir_handle))
+                mutations[iter_name] = iteration.mutation
+
+            top_iterations: List[str] = []
+            for iter_name, iteration in self.epochs[-2].top_iterations.items():
+                top_iterations.append(str(iteration.dir_handle))
+                mutations[iter_name] = iteration.mutation
 
             tracking = {
                 "previous_iterations": previous_iterations,
                 "current_iterations": current_iterations,
                 "top_iterations": top_iterations,
+                "mutations": mutations,
                 "epoch_mutated_positions": self.epochs[-1].mutated_positions,
                 "memory_positions": self.mutated_positions,
                 "failed_memory_positions": self.failed_mutated_positions,
+                "project_dag": self.project_dag,
+                "project_mut_dag": self.project_mut_dag,
             }
-            assert (
-                    len(previous_iterations) > 0
-                    and len(current_iterations) > 0
-                    and len(top_iterations) > 0
-            )
+            assert (len(previous_iterations) > 0 and len(current_iterations) > 0 and len(top_iterations) > 0)
 
             # Back up tracking.pkl before writing.
             track = Path(self.dir_handle, "tracking.pkl")
             try:
                 unique_str = "_".join(time.ctime().split()).replace(":", "_")
                 sh.move(track, Path(self.dir_handle, f"{unique_str}_tracking.pkl"))
             except (FileNotFoundError, OSError):
                 pass
 
             with open(track, "wb") as cur_file:
                 pickle.dump(tracking, cur_file)
 
+            self.__draw_dags__(Path(self.dir_handle, "dags.png"))
         except Exception as e:
             if log:
                 log.warning(f"Not a full WorkProject yet, could not track it.")
 
     def get_first_iter(self) -> Tuple[str, Iteration]:
         return next(iter(self.epochs[0].items()))
 
+    def __draw_dags__(self, out_path: Path) -> None:
+        # Try to set a nice plot size
+        w = max(dict(self.project_dag.degree()).values()) * 2 + 4
+        h = (nx.dag_longest_path_length(self.project_dag) + 1) * 4 + 2
+        _, axes = plt.subplots(1, 2, figsize=(w, h))
+        # _, axes = plt.subplots(1, 2)
+
+        ##### Iterations graph
+        plt.sca(axes[0])
+        # For a better display of the iterations names.
+        label_remap = {node: node.replace('-', '\n') for node in self.project_dag.nodes}
+        dag = nx.relabel_nodes(self.project_dag, label_remap)
+        # Adjuste node and plot sizes, so it fits nicely, hopefully.
+        one_label = next(iter(label_remap.keys()))
+        node_size = max([len(piece) for piece in one_label.split('\n')]) * 400
+        # Plot
+        pos = nx.drawing.nx_agraph.graphviz_layout(dag, prog="dot")
+        nx.draw(dag, pos, with_labels=True, node_size=node_size, node_color="lightblue", font_size=10)
+
+        ##### Mutations graph
+        plt.sca(axes[1])
+        # Plot
+        pos = nx.drawing.nx_agraph.graphviz_layout(self.project_mut_dag, prog="dot")
+        nx.draw(self.project_mut_dag, pos, with_labels=True, node_size=4000, node_color="pink", font_size=10)
+
+        # Remove axes and save.
+        axes[0].set_axis_off()
+        axes[1].set_axis_off()
+        plt.savefig(out_path)
+
+    @staticmethod
+    def draw_dag(dag: nx.Graph, out_path: Path, *, reformat: bool = False) -> None:
+        node_size = 4000
+        w = max(dict(dag.degree()).values()) * 2 + 2
+        h = (nx.dag_longest_path_length(dag) + 1) * 4 + 2
+        plt.figure(figsize=(w, h))
+
+        if reformat:
+            # For a better display of the iterations names.
+            label_remap = {node: node.replace('-', '\n') for node in dag.nodes}
+            dag = nx.relabel_nodes(dag, label_remap)
+
+            # Adjuste node and plot sizes, so it fits nicely, hopefully.
+            one_label = next(iter(label_remap.keys()))
+            node_size = max([len(piece) for piece in one_label.split('\n')]) * 500
+
+        # Plot and save
+        pos = nx.drawing.nx_agraph.graphviz_layout(dag, prog="dot")
+        nx.draw(dag, pos, with_labels=True, node_size=node_size, node_color="lightblue", font_size=10)
+        plt.savefig(out_path)
+
 
 def set_logger(name: str, dir_path: Path) -> logging.Logger:
     logger = logging.getLogger(f"{name}")
     logger.setLevel(logging.INFO)
 
     stream_handler = logging.StreamHandler()
     stream_handler.setLevel(logging.WARNING)
```

### Comparing `locuaz-0.2.1/locuaz/protocol.py` & `locuaz-0.3.1/locuaz/protocol.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import logging
 import sys
 from pathlib import Path
 
 import locuaz.cli
 from locuaz.projectutils import set_logger, WorkProject
 from locuaz.epochinitializer import initialize_new_epoch
-from locuaz.pruners import prune
-from locuaz.run import run_epoch, run_npt_epoch
+from locuaz.pruning import prune
+from locuaz.run import run_epoch
 from locuaz.scoring import score
 
-def main() -> int:
 
+def main() -> int:
     config, start = locuaz.cli.main()
     log = set_logger(config["main"]["name"], Path(config["paths"]["work"]))
     log.info("-----------------------------")
     log.info("Setting up work project.")
     work_pjct = WorkProject(config, start)
     log = logging.getLogger(work_pjct.name)
     log.info("Launching.")
 
     if config["main"]["mode"] == "run":
         run_epoch(work_pjct)
         return 0
-    elif config["main"]["mode"] == "run_npt":
-        run_npt_epoch(work_pjct)
-        return 0
     elif config["main"]["mode"] == "score":
         try:
             prev_id = work_pjct.epochs[-2].id
             prev_epoch = work_pjct.epochs[-2]
             for iter_name, iteration in prev_epoch.items():
                 log.info(f"Scoring NPT run from iteration: {prev_id}-{iter_name}")
                 score(work_pjct, iteration)
```

### Comparing `locuaz-0.2.1/locuaz/pruner.py` & `locuaz-0.3.1/locuaz/prunerconsensus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,91 @@
-from typing import Tuple, Dict
 from queue import PriorityQueue
+from typing import Dict, Tuple
 import logging
 
+from locuaz.abstractpruner import AbstractPruner
 from locuaz.projectutils import Epoch, Iteration
 
 
-def beats_old_iter(
-    old_iter: Iteration, new_iter: Iteration, threshold: int, log: logging.Logger
-) -> Tuple[bool, int]:
-
-    # Allow the user to change scoring functions mid-run and only use
-    # the subset present in both iterations.
-    old_SFs = set(old_iter.scores.keys())
-    new_SFs = set(new_iter.scores.keys())
-    scoring_functions = old_SFs & new_SFs
-    if len(scoring_functions) == 0:
-        raise RuntimeError(f"No common scoring functions between the ones from the old iteration ({old_SFs}) "
-                           f"and those from the new one ({new_SFs}). Cannot prune.")
-    log.info(f"Scoring functions: {scoring_functions}")
-    count = sum(
-        [
-            old_iter.mean_scores[SF] >= new_iter.mean_scores[SF]
-            for SF in scoring_functions
-        ]
-    )
-    log.info(
-        f"{new_iter.epoch_id}-{new_iter.iter_name} vs. {old_iter.epoch_id}-{old_iter.iter_name} "
-        f"improves on {count} of {len(scoring_functions)} scoring functions."
-    )
-
-    return count >= threshold, count
-
-
-def choose_top_iters(
-    prev_epoch: Epoch, this_epoch: Epoch, threshold: int, log: logging.Logger
-) -> PriorityQueue:
-    better_iters: PriorityQueue = PriorityQueue()
-
-    for iter in this_epoch.values():
-        better_overall: bool = True
-        rank_overall: int = 0
-        for prev_iter in prev_epoch.top_iterations.values():
-            better, rank = beats_old_iter(prev_iter, iter, threshold, log)
-            better_overall &= better
-            rank_overall += rank
-        if better_overall:
-            better_iters.put((-rank_overall, iter))
-
-    return better_iters
-
-
-def top_pruner(better_iters: PriorityQueue, prune: int) -> Dict[str, Iteration]:
-    """top_pruner select, at least, the first `prun` iterations above the threshold
-
-    Args:
-        better_iters (PriorityQueue[Tuple[int, Iteration]]): iterations above the threshold,
-            sorted by approved SFs
-        prune (int): minimum number of iterations returned
-
-    Returns:
-        Dict[str, Iteration]: map of top `iter_name:Iteration` for the next epoch.
+class PrunerConsensus(AbstractPruner):
+    """PrunerConsensus select all iterations that satisfy the threshold of approved SFs
     """
 
-    top_iterations: Dict[str, Iteration] = {}
-    for i in range(prune):
-        iter = better_iters.get()[1]
-        top_iterations[iter.iter_name] = iter
-    return top_iterations
-
-
-def adaptive_pruner(better_iters: PriorityQueue, prune: int) -> Dict[str, Iteration]:
-    """adaptive_pruner select all iterations that have the maximum number of approved SFs
-
-    Args:
-        better_iters (PriorityQueue[Tuple[int, Iteration]]): iterations above the threshold,
-            sorted by approved SFs
-        prune (int): unused
-
-    Returns:
-        Dict[str, Iteration]: map of top `iter_name:Iteration` for the next epoch.
-    """
-    top_iterations: Dict[str, Iteration] = {}
-    prev_count = 1
-    while not better_iters.empty():
-        # Remember, `count`, the priority, is negative.
-        count, iter = better_iters.get()
-        if count > prev_count:
-            assert len(top_iterations) > 0, f"Logical error. This can't happen."
-            break
-        prev_count = count
-        top_iterations[iter.iter_name] = iter
-    return top_iterations
-
-
-def threshold_pruner(better_iters: PriorityQueue, prune: int) -> Dict[str, Iteration]:
-    """threshold_pruner select all iterations that satisfy the threshold of approved SFs
-
-    Args:
-        better_iters (PriorityQueue[Tuple[int, Iteration]]): iterations above the threshold,
-            sorted by approved SFs
-        prune (int): unused
+    def __init__(self, prev_epoch: Epoch, this_epoch: Epoch, log: logging.Logger):
+        self.prev_epoch = prev_epoch
+        self.this_epoch = this_epoch
+        self.log = log
+
+    def prune(self, config: Dict) -> PriorityQueue:
+        """
+        The only public method from the Pruner.
+        Parameters
+        ----------
+        config : Dict
+            User input config file
+        Returns
+        -------
+        passing_iters: PriorityQueue
+            ordered queue with the iterations from the new epoch that are better than all the
+            iterations from the old epoch. It may be empty.
+        """
+        return self.__get_passing_iters__(config["pruning"]["consensus_threshold"])
+
+    def __get_passing_iters__(self, threshold: int) -> PriorityQueue:
+        """
+
+        Parameters
+        ----------
+        threshold : int
+            number of scoring functions that have to improve for an iteration to be
+            considered better than another one.
+
+        Returns
+        -------
+        passing_iters: PriorityQueue
+            ordered queue with the iterations from the new epoch that are better than all the
+            iterations from the old epoch. It may be empty.
+        """
+        better_iters: PriorityQueue = PriorityQueue()
+
+        for iteration in self.this_epoch.values():
+            better_overall: bool = True
+            rank_overall: int = 0
+            for prev_iter in self.prev_epoch.top_iterations.values():
+                better, rank = self.__beats_old_iter__(prev_iter, iteration, threshold)
+                better_overall &= better
+                rank_overall += rank
+            if better_overall:
+                better_iters.put((-rank_overall, iteration))
+
+        return better_iters
+
+    def __beats_old_iter__(self, old_iter: Iteration, new_iter: Iteration, threshold: int) -> Tuple[bool, int]:
+        """
+        Parameters
+        ----------
+        old_iter: Iteration
+        new_iter : Iteration
+        threshold : int
+            number of scoring functions that have to improve for the new_iter to be
+            considered better than the old_iter.
+
+        Returns
+        -------
+        beats and count: Tuple[bool, int]
+            whether if it does beat the old iter and the number of improved SFs.
+        """
+        # Allow the user to change scoring functions mid-run and only use
+        # the subset present in both iterations.
+        old_SFs = set(old_iter.scores.keys())
+        new_SFs = set(new_iter.scores.keys())
+        scoring_functions = old_SFs & new_SFs
+        if len(scoring_functions) == 0:
+            raise RuntimeError(f"No common scoring functions between the ones from the old iteration ({old_SFs}) "
+                               f"and those from the new one ({new_SFs}). Cannot prune.")
+        self.log.info(f"Scoring functions: {scoring_functions}")
+        count = sum([old_iter.mean_scores[SF] >= new_iter.mean_scores[SF]
+                     for SF in scoring_functions])
+        self.log.info(f"{new_iter.epoch_id}-{new_iter.iter_name} vs. {old_iter.epoch_id}-{old_iter.iter_name} "
+                      f"improves on {count} of {len(scoring_functions)} scoring functions.")
 
-    Returns:
-        Dict[str, Iteration]: map of top `iter_name:Iteration` for the next epoch.
-    """
-    top_iterations: Dict[str, Iteration] = {}
-    prev_count = 1
-    while not better_iters.empty():
-        _, iter = better_iters.get()
-        top_iterations[iter.iter_name] = iter
-    return top_iterations
+        return count >= threshold, count
```

### Comparing `locuaz-0.2.1/locuaz/pruners.py` & `locuaz-0.3.1/locuaz/pruning.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,45 @@
-from typing import Dict, Callable, Set
+from typing import Set, Dict
 import logging
 
-from locuaz.projectutils import WorkProject
-from locuaz.pruner import choose_top_iters, adaptive_pruner, top_pruner, threshold_pruner
-
-
-pruners: Dict[str, Callable] = {
-    "adaptive": adaptive_pruner,
-    "top": top_pruner,
-    "threshold": threshold_pruner,
-}
+from locuaz.projectutils import WorkProject, Iteration
+from locuaz.pruners import pruners
 
 
 def prune(work_pjct: WorkProject) -> None:
     this_epoch = work_pjct.epochs[-1]
     try:
         prev_epoch = work_pjct.epochs[-2]
-    except IndexError as e:
+    except IndexError:
         # Initial epoch.
         this_epoch.top_iterations = this_epoch.iterations
         return
 
     log = logging.getLogger(work_pjct.name)
-    threshold = work_pjct.config["scoring"]["consensus_threshold"]
+    # Use chosen pruner to prune.
+    pruner_func = pruners[work_pjct.config["pruning"]["pruner"]](prev_epoch, this_epoch, log)
+    better_iters_queue = pruner_func.prune(work_pjct.config)
 
-    better_iters_queue = choose_top_iters(prev_epoch, this_epoch, threshold, log)
     failed_pos: Set[int] = set()
     if better_iters_queue.empty():
-        # All new iterations are worse than the old ones or they all failed during MD.
-        log.info(
-            f"Failed epoch after mutating resSeqs: {this_epoch.mutated_positions}. "
-            f"Backing up epoch {this_epoch.id}."
-        )
+        # All new iterations are worse than the old ones, or they all failed during MD.
+        log.info(f"Unsuccessful epoch after mutating resSeqs: {this_epoch.mutated_positions}. "
+                 f"Backing up epoch {this_epoch.id}.")
         failed_pos = this_epoch.mutated_positions
         this_epoch.backup()
         work_pjct.epochs[-1] = prev_epoch
     else:
-        log.info(
-            f"Successful epoch after mutating resSeqs: {this_epoch.mutated_positions} ."
-        )
-        pruner_func = pruners[work_pjct.config["protocol"]["pruner"]]
-        prune = work_pjct.config["protocol"].get("prune")
-        # Prune as many branches as requested, using the required pruner.
-        this_epoch.top_iterations = pruner_func(better_iters_queue, prune)
+        log.info(f"Successful epoch after mutating resSeqs: {this_epoch.mutated_positions} .")
+        this_epoch.top_iterations: Dict[str, Iteration] = {}
+        while not better_iters_queue.empty():
+            _, iteration = better_iters_queue.get()
+            this_epoch.top_iterations[iteration.iter_name] = iteration
 
     if work_pjct.has_failed_memory:
+        # If epoch was successful, we're appending an empty set, just to move the queue along.
         work_pjct.failed_mutated_positions.appendleft(failed_pos)
 
-    top_itrs_str = " ; ".join(
-        [
-            f"{iter.epoch_id}-{iter.iter_name}"
-            for iter in work_pjct.epochs[-1].top_iterations.values()
-        ]
-    )
+    top_itrs_str = " ; ".join([f"{iteration.epoch_id}-{iteration.iter_name}"
+                               for iteration in work_pjct.epochs[-1].top_iterations.values()])
     log.info(f"Top iterations: {top_itrs_str}")
 
     return
```

### Comparing `locuaz-0.2.1/locuaz/rosetta.py` & `locuaz-0.3.1/locuaz/rosetta.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/run.py` & `locuaz-0.3.1/locuaz/run.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/runutils.py` & `locuaz-0.3.1/locuaz/runutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             gpu_id: int = 0,
             pinoffset: int = 0,
             out_name="min",
     ) -> "MDrun":
 
         obj = cls(
             DirHandle(root_dir),
-            binary_path=work_pjct.config["md"]["gmx_bin"],
+            binary_path=work_pjct.config["md"]["gmx_mdrun"],
             mdp=FileHandle(Path(work_pjct.mdps["min_mdp"])),
             gpu_id=gpu_id,
             pinoffset=pinoffset,
             num_threads_omp=work_pjct.config["md"]["omp_procs"],
             num_threads_mpi=work_pjct.config["md"]["mpi_procs"],
             dev=f"-nb gpu -pin on -pinoffset {pinoffset}",
             out_name=out_name,
@@ -63,21 +63,21 @@
             gpu_id: int = 0,
             pinoffset: int = 0,
             out_name="nvt",
     ) -> "MDrun":
 
         obj = cls(
             DirHandle(root_dir),
-            binary_path=work_pjct.config["md"]["gmx_bin"],
+            binary_path=work_pjct.config["md"]["gmx_mdrun"],
             mdp=FileHandle(Path(work_pjct.mdps["nvt_mdp"])),
             gpu_id=gpu_id,
             pinoffset=pinoffset,
             num_threads_omp=work_pjct.config["md"]["omp_procs"],
             num_threads_mpi=work_pjct.config["md"]["mpi_procs"],
-            dev=f"-nb gpu -pme gpu -bonded gpu -pmefft gpu -pin on -pinoffset {pinoffset}",
+            dev=f"-nb gpu -pme gpu -pin on -pinoffset {pinoffset}",
             out_name=out_name,
             maxwarn=work_pjct.config["md"]["maxwarn"],
         )
 
         return obj
 
     @classmethod
@@ -90,21 +90,21 @@
             pinoffset: int = 0,
             out_name="npt",
             image_after=True,
     ) -> "MDrun":
 
         obj = cls(
             DirHandle(root_dir),
-            binary_path=work_pjct.config["md"]["gmx_bin"],
+            binary_path=work_pjct.config["md"]["gmx_mdrun"],
             mdp=FileHandle(Path(work_pjct.mdps["npt_mdp"])),
             gpu_id=gpu_id,
             pinoffset=pinoffset,
             num_threads_omp=work_pjct.config["md"]["omp_procs"],
             num_threads_mpi=work_pjct.config["md"]["mpi_procs"],
-            dev=f"-nb gpu -pme gpu -bonded gpu -pmefft gpu -pin on -pinoffset {pinoffset}",
+            dev=f"-nb gpu -pme gpu -pin on -pinoffset {pinoffset}",
             out_name=out_name,
             image_after=image_after,
             maxwarn=work_pjct.config["md"]["maxwarn"],
         )
 
         return obj
```

### Comparing `locuaz-0.2.1/locuaz/scoring.py` & `locuaz-0.3.1/locuaz/scoring.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from biobb_analysis.gromacs.gmx_trjconv_str_ens import GMXTrjConvStrEns
 
 from locuaz.fileutils import DirHandle
 from locuaz.gromacsutils import image_traj
 from locuaz.primitives import launch_biobb
 from locuaz.projectutils import WorkProject, Iteration
 from locuaz.utils_scoring import extract_pdbs, join_target_binder, rm_aux_scoring_files
-from locuaz.stats import run_stats
+from locuaz.statistics import run_stats
 
 
 def initialize_scoring_folder(
         iteration: Iteration, config: dict, *, log: Optional[logging.Logger] = None
 ) -> Tuple[int, int]:
     """
     Creates scoring folder inside the iteration dir, fixes PBC issues with the original NPT trajectory
```

### Comparing `locuaz-0.2.1/locuaz/scoringfunctions.py` & `locuaz-0.3.1/locuaz/scoringfunctions.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/spm4.py` & `locuaz-0.3.1/locuaz/spm4.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,26 +55,26 @@
         mut_idx_chain, mut_chainID, mut_idx_residue, mut_resSeq = self.__generate_position__(epoch, use_tleap, logger)
         self.__fill_mutations__(epoch, branches, mut_idx_chain, mut_chainID, mut_idx_residue, mut_resSeq)
 
     def __fill_mutations__(self, epoch: Epoch, branches: int, mut_idx_chain: int, mut_chainID: str,
                            mut_idx_residue: int, mut_resSeq: int):
         """
         generates up to `branches` different mutations
-        :param epoch:
-        :type epoch:
-        :param branches:
-        :type branches:
-        :param mut_idx_chain:
-        :type mut_idx_chain:
-        :param mut_chainID:
-        :type mut_chainID:
-        :param mut_idx_residue:
-        :type mut_idx_residue:
-        :param mut_resSeq:
-        :type mut_resSeq:
+        Parameters
+        ----------
+        epoch :
+        branches :
+        mut_idx_chain :
+        mut_chainID :
+        mut_idx_residue :
+        mut_resSeq :
+
+        Returns
+        -------
+
         """
         remaining_branches = branches
         remaining_iterations = set(epoch.top_iterations.keys())
         while remaining_branches != 0:
             iteration = epoch.top_iterations[remaining_iterations.pop()]
             old_aa, new_aa = self.__get_random_aa__(iteration, mut_idx_chain, mut_idx_residue)
             # Build the mutation object for this iteration.
@@ -96,24 +96,22 @@
 
     def __generate_position__(self, epoch: Epoch, use_tleap: bool = False,
                               logger: Logger = None) -> Tuple[int, str, int, int]:
         # Get an iteration to read the chainIDs and the resSeqs.
         try:
             any_iteration = next(iter(epoch.top_iterations.values()))
         except Exception:
-            raise RuntimeError(
-                f"No available iterations on Epoch {epoch.id}. "
-                "It's likely that all of them failed during MD."
-            )
+            raise RuntimeError(f"No available iterations on Epoch {epoch.id}. "
+                               "It's likely that all of them failed during MD.")
 
         # Now, filter the mutating resSeqs.
         candidates_resSeq = [resSeq for cdr in any_iteration.resSeqs for resSeq in cdr if
-                                     resSeq not in self.excluded_pos]
+                             resSeq not in self.excluded_pos]
         if len(candidates_resSeq) == 0:
-            raise RuntimeError(f"Cannot mutate. No CDR residue on the interface that isn't excluded.")
+            raise RuntimeError(f"Cannot mutate. No CDR residue that isn't excluded.")
 
         logger.info(f"Generating mutations with: {self}.\n"
                     f"'mutating_resSeq': {any_iteration.resSeqs}.\n"
                     f"excluded resSeq: {self.excluded_pos}.\n"
                     f"'mutating_resSeq' that may be mutated: {candidates_resSeq}.")
 
         # Choose the position to mutate. This will be the same for all iterations.
```

### Comparing `locuaz-0.2.1/locuaz/spm4i.py` & `locuaz-0.3.1/locuaz/spm4i.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/spm4mmpbsa.py` & `locuaz-0.3.1/locuaz/spm4mmpbsa.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/statisticcmdistance.py` & `locuaz-0.3.1/locuaz/statisticcmdistance.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/statisticinterface.py` & `locuaz-0.3.1/locuaz/statisticinterface.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/stats.py` & `locuaz-0.3.1/locuaz/statistics.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/utils_scoring.py` & `locuaz-0.3.1/locuaz/utils_scoring.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz/validatore.py` & `locuaz-0.3.1/locuaz/validatore.py`

 * *Files identical despite different names*

### Comparing `locuaz-0.2.1/locuaz.egg-info/SOURCES.txt` & `locuaz-0.3.1/locuaz.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 CHANGELOG.rst
 LICENSE.rst
+MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 locuaz/__init__.py
 locuaz/abstractmutationgenerator.py
+locuaz/abstractpruner.py
 locuaz/abstractscoringfunction.py
 locuaz/amberutils.py
 locuaz/autodockvina.py
 locuaz/bach.py
 locuaz/basemutator.py
 locuaz/basestatistic.py
 locuaz/bluues.py
@@ -35,30 +37,36 @@
 locuaz/mutators.py
 locuaz/piepisa.py
 locuaz/pisa.py
 locuaz/primitives.py
 locuaz/projectutils.py
 locuaz/protocol.py
 locuaz/pruner.py
+locuaz/prunerconsensus.py
+locuaz/prunermetropolis.py
 locuaz/pruners.py
+locuaz/pruning.py
 locuaz/rosetta.py
 locuaz/run.py
 locuaz/runutils.py
+locuaz/schema.yaml
 locuaz/scoring.py
 locuaz/scoringfunctions.py
 locuaz/spm4.py
 locuaz/spm4i.py
 locuaz/spm4mmpbsa.py
 locuaz/statisticcmdistance.py
 locuaz/statisticinterface.py
-locuaz/stats.py
+locuaz/statistics.py
 locuaz/utils_scoring.py
 locuaz/validatore.py
 locuaz.egg-info/PKG-INFO
 locuaz.egg-info/SOURCES.txt
 locuaz.egg-info/dependency_links.txt
 locuaz.egg-info/entry_points.txt
 locuaz.egg-info/requires.txt
 locuaz.egg-info/top_level.txt
-locuaz/DLPacker/dlpacker.py
-locuaz/DLPacker/utils.py
+locuaz/sample_bin/aux_scripts/reorder_pdb.py
+locuaz/sample_bin/dlpacker/charges.rtp
+locuaz/sample_bin/gmxmmpbsa/gmxmmpbsa
+locuaz/sample_bin/haddock/template_scoring.inp
 tests/test_locuaz.py
```

### Comparing `locuaz-0.2.1/tests/test_locuaz.py` & `locuaz-0.3.1/tests/test_locuaz.py`

 * *Files identical despite different names*

