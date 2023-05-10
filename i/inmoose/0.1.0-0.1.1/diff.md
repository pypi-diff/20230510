# Comparing `tmp/inmoose-0.1.0.tar.gz` & `tmp/inmoose-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inmoose-0.1.0.tar", last modified: Wed Apr 12 20:01:53 2023, max compression
+gzip compressed data, was "inmoose-0.1.1.tar", last modified: Wed May 10 12:13:43 2023, max compression
```

## Comparing `inmoose-0.1.0.tar` & `inmoose-0.1.1.tar`

### file list

```diff
@@ -1,99 +1,96 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.339954 inmoose-0.1.0/
--rw-r--r--   0 max        (501) staff       (20)    35149 2023-01-03 16:30:25.000000 inmoose-0.1.0/LICENSE
--rw-r--r--   0 max        (501) staff       (20)     2654 2023-04-12 20:01:53.339824 inmoose-0.1.0/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     2156 2023-04-12 20:01:02.000000 inmoose-0.1.0/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.294882 inmoose-0.1.0/inmoose/
--rw-r--r--   0 max        (501) staff       (20)       98 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/__init__.py
--rw-r--r--   0 max        (501) staff       (20)       22 2023-04-12 20:00:08.000000 inmoose-0.1.0/inmoose/__version__.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.299359 inmoose-0.1.0/inmoose/batch/
--rw-r--r--   0 max        (501) staff       (20)       70 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/batch/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     2261 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/batch/covariates.py
--rw-r--r--   0 max        (501) staff       (20)     3342 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/batch/helper_seq.py
--rw-r--r--   0 max        (501) staff       (20)    25565 2023-01-17 15:54:39.000000 inmoose-0.1.0/inmoose/batch/pycombat.py
--rw-r--r--   0 max        (501) staff       (20)    10011 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/batch/pycombat_seq.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.301031 inmoose-0.1.0/inmoose/common_cpp/
--rw-r--r--   0 max        (501) staff       (20)   228430 2023-04-12 12:58:26.000000 inmoose-0.1.0/inmoose/common_cpp/common_cpp.cpp
--rw-r--r--   0 max        (501) staff       (20)      962 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/common_cpp/common_cpp.pyx
--rw-r--r--   0 max        (501) staff       (20)     2836 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/common_cpp/matrix.cpp
--rw-r--r--   0 max        (501) staff       (20)     9126 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/common_cpp/matrix.h
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.318321 inmoose-0.1.0/inmoose/edgepy/
--rw-r--r--   0 max        (501) staff       (20)     1563 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/DGEGLM.py
--rw-r--r--   0 max        (501) staff       (20)     6668 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/DGEList.py
--rw-r--r--   0 max        (501) staff       (20)      813 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     2188 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/addPriorCount.py
--rw-r--r--   0 max        (501) staff       (20)     2536 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/adjustedProfileLik.py
--rw-r--r--   0 max        (501) staff       (20)     3910 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/aveLogCPM.py
--rw-r--r--   0 max        (501) staff       (20)     3479 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/dispCoxReid.py
--rw-r--r--   0 max        (501) staff       (20)     4438 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/dispCoxReidInterpolateTagwise.py
--rw-r--r--   0 max        (501) staff       (20)     1322 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/dropEmptyLevels.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.333228 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/
--rw-r--r--   0 max        (501) staff       (20)     6098 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/__init__.pxd
--rw-r--r--   0 max        (501) staff       (20)     3085 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/add_prior.cpp
--rw-r--r--   0 max        (501) staff       (20)     1583 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/add_prior.h
--rw-r--r--   0 max        (501) staff       (20)     3110 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp
--rw-r--r--   0 max        (501) staff       (20)      869 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/add_prior_count.h
--rw-r--r--   0 max        (501) staff       (20)     5168 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp
--rw-r--r--   0 max        (501) staff       (20)     2568 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp
--rw-r--r--   0 max        (501) staff       (20)     5065 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/compute_apl.cpp
--rw-r--r--   0 max        (501) staff       (20)     3796 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp
--rw-r--r--   0 max        (501) staff       (20)   841251 2023-04-12 13:15:51.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/edgepy_cpp.cpp
--rw-r--r--   0 max        (501) staff       (20)     2779 2023-04-12 13:15:51.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/edgepy_cpp.h
--rw-r--r--   0 max        (501) staff       (20)     4188 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx
--rw-r--r--   0 max        (501) staff       (20)     3507 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp
--rw-r--r--   0 max        (501) staff       (20)      955 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.h
--rw-r--r--   0 max        (501) staff       (20)     4692 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp
--rw-r--r--   0 max        (501) staff       (20)     2371 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp
--rw-r--r--   0 max        (501) staff       (20)     2273 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/glm.h
--rw-r--r--   0 max        (501) staff       (20)    11007 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp
--rw-r--r--   0 max        (501) staff       (20)     2625 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp
--rw-r--r--   0 max        (501) staff       (20)     6097 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp
--rw-r--r--   0 max        (501) staff       (20)     1137 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h
--rw-r--r--   0 max        (501) staff       (20)     7061 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/interpolator.cpp
--rw-r--r--   0 max        (501) staff       (20)     1308 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/interpolator.h
--rw-r--r--   0 max        (501) staff       (20)     1880 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp
--rw-r--r--   0 max        (501) staff       (20)     2433 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/nbdev.cpp
--rw-r--r--   0 max        (501) staff       (20)     5066 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/objects.cpp
--rw-r--r--   0 max        (501) staff       (20)     1957 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/objects.h
--rw-r--r--   0 max        (501) staff       (20)     1801 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/utils.h
--rw-r--r--   0 max        (501) staff       (20)     3091 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/estimateGLMCommonDisp.py
--rw-r--r--   0 max        (501) staff       (20)     3578 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/estimateGLMTagwiseDisp.py
--rw-r--r--   0 max        (501) staff       (20)     5854 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/glmFit.py
--rw-r--r--   0 max        (501) staff       (20)     5138 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/makeCompressedMatrix.py
--rw-r--r--   0 max        (501) staff       (20)     2057 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/maximizeInterpolant.py
--rw-r--r--   0 max        (501) staff       (20)     2818 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/mglmLevenberg.py
--rw-r--r--   0 max        (501) staff       (20)     2234 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/mglmOneGroup.py
--rw-r--r--   0 max        (501) staff       (20)     4375 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/mglmOneWay.py
--rw-r--r--   0 max        (501) staff       (20)     2168 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/movingAverageByCol.py
--rw-r--r--   0 max        (501) staff       (20)     3371 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/nbinomDeviance.py
--rw-r--r--   0 max        (501) staff       (20)     2222 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/predFC.py
--rw-r--r--   0 max        (501) staff       (20)     1638 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/splitIntoGroups.py
--rw-r--r--   0 max        (501) staff       (20)     5659 2023-04-12 12:53:43.000000 inmoose-0.1.0/inmoose/edgepy/stats.py
--rw-r--r--   0 max        (501) staff       (20)     1543 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/systematicSubset.py
--rw-r--r--   0 max        (501) staff       (20)     1685 2023-01-17 15:52:45.000000 inmoose-0.1.0/inmoose/edgepy/utils.py
--rw-r--r--   0 max        (501) staff       (20)     1713 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/edgepy/validDGEList.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.333702 inmoose-0.1.0/inmoose/utils/
--rw-r--r--   0 max        (501) staff       (20)       68 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/utils/__init__.py
--rw-r--r--   0 max        (501) staff       (20)     1817 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/utils/factor.py
--rw-r--r--   0 max        (501) staff       (20)     1126 2023-04-12 15:21:45.000000 inmoose-0.1.0/inmoose/utils/stats.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.297849 inmoose-0.1.0/inmoose.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     2654 2023-04-12 20:01:53.000000 inmoose-0.1.0/inmoose.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     2823 2023-04-12 20:01:53.000000 inmoose-0.1.0/inmoose.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-04-12 20:01:53.000000 inmoose-0.1.0/inmoose.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       47 2023-04-12 20:01:53.000000 inmoose-0.1.0/inmoose.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)       77 2023-04-12 20:01:53.000000 inmoose-0.1.0/inmoose.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)       89 2023-01-03 16:30:25.000000 inmoose-0.1.0/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)       38 2023-04-12 20:01:53.339988 inmoose-0.1.0/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)     3283 2023-04-12 20:01:02.000000 inmoose-0.1.0/setup.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-12 20:01:53.339642 inmoose-0.1.0/tests/
--rw-r--r--   0 max        (501) staff       (20)     3556 2023-01-17 15:52:45.000000 inmoose-0.1.0/tests/test_DGEList.py
--rw-r--r--   0 max        (501) staff       (20)     1474 2023-04-12 15:21:45.000000 inmoose-0.1.0/tests/test_aveLogCPM.py
--rw-r--r--   0 max        (501) staff       (20)     1583 2023-01-17 15:52:45.000000 inmoose-0.1.0/tests/test_compressMatrix.py
--rw-r--r--   0 max        (501) staff       (20)     7285 2023-04-12 15:21:45.000000 inmoose-0.1.0/tests/test_dispersion.py
--rw-r--r--   0 max        (501) staff       (20)     1827 2023-04-12 15:21:45.000000 inmoose-0.1.0/tests/test_factor.py
--rw-r--r--   0 max        (501) staff       (20)    10270 2023-04-12 15:21:45.000000 inmoose-0.1.0/tests/test_glm.py
--rw-r--r--   0 max        (501) staff       (20)      948 2023-04-12 15:21:45.000000 inmoose-0.1.0/tests/test_lik.py
--rw-r--r--   0 max        (501) staff       (20)     7933 2023-04-12 15:21:45.000000 inmoose-0.1.0/tests/test_mglm.py
--rw-r--r--   0 max        (501) staff       (20)      593 2023-01-17 15:52:45.000000 inmoose-0.1.0/tests/test_objects.py
--rw-r--r--   0 max        (501) staff       (20)     6852 2023-01-17 15:52:45.000000 inmoose-0.1.0/tests/test_pycombat.py
--rw-r--r--   0 max        (501) staff       (20)     2892 2023-04-12 15:21:45.000000 inmoose-0.1.0/tests/test_pycombatseq.py
--rw-r--r--   0 max        (501) staff       (20)     1174 2023-01-17 15:52:45.000000 inmoose-0.1.0/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.962212 inmoose-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 12:13:28.000000 inmoose-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-10 12:13:43.962212 inmoose-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-10 12:13:28.000000 inmoose-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.946212 inmoose-0.1.1/inmoose/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.950212 inmoose-0.1.1/inmoose/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/covariates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/helper_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25565 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/pycombat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/batch/pycombat_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.950212 inmoose-0.1.1/inmoose/common_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/common_cpp/common_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/common_cpp/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/common_cpp/matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.954212 inmoose-0.1.1/inmoose/edgepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/DGEGLM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/DGEList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/addPriorCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/adjustedProfileLik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/aveLogCPM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/dispCoxReid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/dispCoxReidInterpolateTagwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/dropEmptyLevels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.958212 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior_count.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/compute_apl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/interpolator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/interpolator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/nbdev.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/objects.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/objects.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/estimateGLMCommonDisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/estimateGLMTagwiseDisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/glmFit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/makeCompressedMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/maximizeInterpolant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/mglmLevenberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/mglmOneGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/mglmOneWay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/movingAverageByCol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/nbinomDeviance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/predFC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/splitIntoGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/systematicSubset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/edgepy/validDGEList.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.958212 inmoose-0.1.1/inmoose/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/utils/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-10 12:13:28.000000 inmoose-0.1.1/inmoose/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.950212 inmoose-0.1.1/inmoose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 12:13:43.000000 inmoose-0.1.1/inmoose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-10 12:13:28.000000 inmoose-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:13:43.962212 inmoose-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-10 12:13:28.000000 inmoose-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:13:43.962212 inmoose-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_DGEList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_aveLogCPM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_compressMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_glm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_lik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_mglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_pycombat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_pycombatseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-10 12:13:28.000000 inmoose-0.1.1/tests/test_stats.py
```

### Comparing `inmoose-0.1.0/LICENSE` & `inmoose-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/PKG-INFO` & `inmoose-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmoose
-Version: 0.1.0
+Version: 0.1.1
 Summary: InMoose: the Integrated Multi Omic Open Source Environment
 Home-page: https://github.com/epigenelabs/inmoose
 Author: Maximilien Colange
 Author-email: maximilien@epigenelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `inmoose-0.1.0/README.md` & `inmoose-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/batch/covariates.py` & `inmoose-0.1.1/inmoose/batch/covariates.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/batch/helper_seq.py` & `inmoose-0.1.1/inmoose/batch/helper_seq.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/batch/pycombat.py` & `inmoose-0.1.1/inmoose/batch/pycombat.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/batch/pycombat_seq.py` & `inmoose-0.1.1/inmoose/batch/pycombat_seq.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/common_cpp/common_cpp.pyx` & `inmoose-0.1.1/inmoose/common_cpp/common_cpp.pyx`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/common_cpp/matrix.cpp` & `inmoose-0.1.1/inmoose/common_cpp/matrix.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/common_cpp/matrix.h` & `inmoose-0.1.1/inmoose/common_cpp/matrix.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/DGEGLM.py` & `inmoose-0.1.1/inmoose/edgepy/DGEGLM.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/DGEList.py` & `inmoose-0.1.1/inmoose/edgepy/DGEList.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/__init__.py` & `inmoose-0.1.1/inmoose/edgepy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from .. import common_cpp
 from .addPriorCount import addPriorCount
 from .adjustedProfileLik import adjustedProfileLik
 from .aveLogCPM import aveLogCPM
 from .DGEGLM import DGEGLM
 from .DGEList import DGEList
 from .dispCoxReid import dispCoxReid
 from .estimateGLMCommonDisp import estimateGLMCommonDisp
```

### Comparing `inmoose-0.1.0/inmoose/edgepy/addPriorCount.py` & `inmoose-0.1.1/inmoose/edgepy/addPriorCount.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/adjustedProfileLik.py` & `inmoose-0.1.1/inmoose/edgepy/adjustedProfileLik.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/aveLogCPM.py` & `inmoose-0.1.1/inmoose/edgepy/aveLogCPM.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/dispCoxReid.py` & `inmoose-0.1.1/inmoose/edgepy/dispCoxReid.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/dispCoxReidInterpolateTagwise.py` & `inmoose-0.1.1/inmoose/edgepy/dispCoxReidInterpolateTagwise.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/dropEmptyLevels.py` & `inmoose-0.1.1/inmoose/edgepy/dropEmptyLevels.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/__init__.pxd` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/__init__.pxd`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/add_prior.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/add_prior.h` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior_count.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/add_prior_count.h` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/add_prior_count.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/compute_apl.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/compute_apl.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/fit_levenberg.h` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_levenberg.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/fit_one_group.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/glm.h` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/glm_one_group.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 #include "initialize_levenberg.h"
 #include "glm.h"
 #include "numpy/ndarraytypes.h"
 #include "objects.h"
 
 /* Different initialization methods for the Levenberg coefficients */
 
-extern "C" void build_QRdecomposition(QRdecomposition*);
-extern "C" void decompose_QRdecomposition(QRdecomposition*);
-extern "C" void solve_QRdecomposition(QRdecomposition*);
+void build_QRdecomposition(QRdecomposition*);
+void decompose_QRdecomposition(QRdecomposition*);
+void solve_QRdecomposition(QRdecomposition*);
 
 QRdecomposition::QRdecomposition(int nrows, int ncoefs, const double* curX) : NR(nrows), NC(ncoefs),
         X(curX), Xcopy(NR*NC), tau(NC), effects(NR), weights(NR),
         lwork_geqrf(-1), lwork_ormqr(-1) {
 
     build_QRdecomposition(this);
 }
```

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/initialize_levenberg.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/interpolator.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/interpolator.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/interpolator.h` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/interpolator.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/maximize_interpolant.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/nbdev.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/nbdev.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/objects.cpp` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/objects.cpp`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/objects.h` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/objects.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/edgepy_cpp/utils.h` & `inmoose-0.1.1/inmoose/edgepy/edgepy_cpp/utils.h`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/estimateGLMCommonDisp.py` & `inmoose-0.1.1/inmoose/edgepy/estimateGLMCommonDisp.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/estimateGLMTagwiseDisp.py` & `inmoose-0.1.1/inmoose/edgepy/estimateGLMTagwiseDisp.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/glmFit.py` & `inmoose-0.1.1/inmoose/edgepy/glmFit.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/makeCompressedMatrix.py` & `inmoose-0.1.1/inmoose/edgepy/makeCompressedMatrix.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/maximizeInterpolant.py` & `inmoose-0.1.1/inmoose/edgepy/maximizeInterpolant.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/mglmLevenberg.py` & `inmoose-0.1.1/inmoose/edgepy/mglmLevenberg.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/mglmOneGroup.py` & `inmoose-0.1.1/inmoose/edgepy/mglmOneGroup.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/mglmOneWay.py` & `inmoose-0.1.1/inmoose/edgepy/mglmOneWay.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/movingAverageByCol.py` & `inmoose-0.1.1/inmoose/edgepy/movingAverageByCol.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/nbinomDeviance.py` & `inmoose-0.1.1/inmoose/edgepy/nbinomDeviance.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/predFC.py` & `inmoose-0.1.1/inmoose/edgepy/predFC.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/splitIntoGroups.py` & `inmoose-0.1.1/inmoose/edgepy/splitIntoGroups.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/stats.py` & `inmoose-0.1.1/inmoose/edgepy/stats.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/systematicSubset.py` & `inmoose-0.1.1/inmoose/edgepy/systematicSubset.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/utils.py` & `inmoose-0.1.1/inmoose/edgepy/utils.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/edgepy/validDGEList.py` & `inmoose-0.1.1/inmoose/edgepy/validDGEList.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/utils/factor.py` & `inmoose-0.1.1/inmoose/utils/factor.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose/utils/stats.py` & `inmoose-0.1.1/inmoose/utils/stats.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/inmoose.egg-info/PKG-INFO` & `inmoose-0.1.1/inmoose.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inmoose
-Version: 0.1.0
+Version: 0.1.1
 Summary: InMoose: the Integrated Multi Omic Open Source Environment
 Home-page: https://github.com/epigenelabs/inmoose
 Author: Maximilien Colange
 Author-email: maximilien@epigenelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `inmoose-0.1.0/inmoose.egg-info/SOURCES.txt` & `inmoose-0.1.1/inmoose.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 inmoose.egg-info/requires.txt
 inmoose.egg-info/top_level.txt
 inmoose/batch/__init__.py
 inmoose/batch/covariates.py
 inmoose/batch/helper_seq.py
 inmoose/batch/pycombat.py
 inmoose/batch/pycombat_seq.py
-inmoose/common_cpp/common_cpp.cpp
 inmoose/common_cpp/common_cpp.pyx
 inmoose/common_cpp/matrix.cpp
 inmoose/common_cpp/matrix.h
 inmoose/edgepy/DGEGLM.py
 inmoose/edgepy/DGEList.py
 inmoose/edgepy/__init__.py
 inmoose/edgepy/addPriorCount.py
@@ -48,16 +47,14 @@
 inmoose/edgepy/edgepy_cpp/add_prior.h
 inmoose/edgepy/edgepy_cpp/add_prior_count.cpp
 inmoose/edgepy/edgepy_cpp/add_prior_count.h
 inmoose/edgepy/edgepy_cpp/adj_coxreid.cpp
 inmoose/edgepy/edgepy_cpp/ave_log_cpm.cpp
 inmoose/edgepy/edgepy_cpp/compute_apl.cpp
 inmoose/edgepy/edgepy_cpp/compute_nbdev.cpp
-inmoose/edgepy/edgepy_cpp/edgepy_cpp.cpp
-inmoose/edgepy/edgepy_cpp/edgepy_cpp.h
 inmoose/edgepy/edgepy_cpp/edgepy_cpp.pyx
 inmoose/edgepy/edgepy_cpp/fit_levenberg.cpp
 inmoose/edgepy/edgepy_cpp/fit_levenberg.h
 inmoose/edgepy/edgepy_cpp/fit_one_group.cpp
 inmoose/edgepy/edgepy_cpp/get_one_way_fitted.cpp
 inmoose/edgepy/edgepy_cpp/glm.h
 inmoose/edgepy/edgepy_cpp/glm_levenberg.cpp
```

### Comparing `inmoose-0.1.0/setup.py` & `inmoose-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     packages = [
         "inmoose",
         "inmoose/batch",
+        "inmoose/common_cpp",
         "inmoose/edgepy",
         "inmoose/edgepy/edgepy_cpp",
         "inmoose/utils",
     ],
     package_data = {
         "inmoose/edgepy/edgepy_cpp": [
             'edgepy_cpp.pyx',
```

### Comparing `inmoose-0.1.0/tests/test_DGEList.py` & `inmoose-0.1.1/tests/test_DGEList.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_aveLogCPM.py` & `inmoose-0.1.1/tests/test_aveLogCPM.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_compressMatrix.py` & `inmoose-0.1.1/tests/test_compressMatrix.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_dispersion.py` & `inmoose-0.1.1/tests/test_dispersion.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_factor.py` & `inmoose-0.1.1/tests/test_factor.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_glm.py` & `inmoose-0.1.1/tests/test_glm.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_lik.py` & `inmoose-0.1.1/tests/test_lik.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_mglm.py` & `inmoose-0.1.1/tests/test_mglm.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_objects.py` & `inmoose-0.1.1/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_pycombat.py` & `inmoose-0.1.1/tests/test_pycombat.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_pycombatseq.py` & `inmoose-0.1.1/tests/test_pycombatseq.py`

 * *Files identical despite different names*

### Comparing `inmoose-0.1.0/tests/test_stats.py` & `inmoose-0.1.1/tests/test_stats.py`

 * *Files identical despite different names*

