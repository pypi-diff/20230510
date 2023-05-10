# Comparing `tmp/diffgram-0.9.6.tar.gz` & `tmp/diffgram-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffgram-0.9.6.tar", last modified: Thu Oct  6 16:45:02 2022, max compression
+gzip compressed data, was "diffgram-0.9.7.tar", last modified: Fri Oct  7 14:14:10 2022, max compression
```

## Comparing `diffgram-0.9.6.tar` & `diffgram-0.9.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.084670 diffgram-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-10-06 16:45:02.084670 diffgram-0.9.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.072669 diffgram-0.9.6/diffgram/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.072669 diffgram-0.9.6/diffgram/brain/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15445 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/brain/brain.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/brain/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/brain/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/brain/train.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.072669 diffgram-0.9.6/diffgram/convert/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/convert/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.076670 diffgram-0.9.6/diffgram/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/core/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    10335 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/core/diffgram_dataset_iterator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12441 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/core/directory.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/core/directory_samples.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/core/sliced_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.076670 diffgram-0.9.6/diffgram/export/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/export/export.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.076670 diffgram-0.9.6/diffgram/file/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/file/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     3826 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/file/file_3d.py
--rw-r--r--   0 runner    (1001) docker     (121)    18439 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/file/file_constructor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/file/test_existing_instances.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/file/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/file/view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.080670 diffgram-0.9.6/diffgram/job/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/job/guide.py
--rw-r--r--   0 runner    (1001) docker     (121)    13708 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/job/job.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.080670 diffgram-0.9.6/diffgram/label/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/label/label_new.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/label/test_label.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.080670 diffgram-0.9.6/diffgram/member/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/member/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.080670 diffgram-0.9.6/diffgram/pytorch_diffgram/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/pytorch_diffgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/pytorch_diffgram/diffgram_pytorch_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.080670 diffgram-0.9.6/diffgram/regular/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/regular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/regular/regular.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.080670 diffgram-0.9.6/diffgram/role/
--rw-r--r--   0 runner    (1001) docker     (121)     5417 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/role/Role.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.080670 diffgram-0.9.6/diffgram/task/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/task/task.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/task/test_task.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.080670 diffgram-0.9.6/diffgram/tensorflow_diffgram/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/tensorflow_diffgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3859 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/tensorflow_diffgram/diffgram_tensorflow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/tensorflow_diffgram/pytorch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.084670 diffgram-0.9.6/diffgram/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20268 2022-10-06 16:42:18.000000 diffgram-0.9.6/diffgram/utils/visualization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.072669 diffgram-0.9.6/diffgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-10-06 16:45:01.000000 diffgram-0.9.6/diffgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-10-06 16:45:01.000000 diffgram-0.9.6/diffgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 16:45:01.000000 diffgram-0.9.6/diffgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-06 16:45:01.000000 diffgram-0.9.6/diffgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-06 16:45:01.000000 diffgram-0.9.6/diffgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-06 16:45:02.084670 diffgram-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-10-06 16:42:18.000000 diffgram-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 16:45:02.084670 diffgram-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-06 16:42:18.000000 diffgram-0.9.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-10-07 14:14:10.210629 diffgram-0.9.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.202629 diffgram-0.9.7/diffgram/
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.202629 diffgram-0.9.7/diffgram/brain/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15445 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/brain/brain.py
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/brain/inference.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/brain/instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1031 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/brain/train.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.202629 diffgram-0.9.7/diffgram/convert/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/convert/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.206629 diffgram-0.9.7/diffgram/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/core/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10886 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/core/diffgram_dataset_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12441 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/core/directory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/core/directory_samples.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2034 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/core/sliced_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.206629 diffgram-0.9.7/diffgram/export/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/export/export.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.206629 diffgram-0.9.7/diffgram/file/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/file/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3826 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/file/file_3d.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18439 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/file/file_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/file/test_existing_instances.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/file/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/file/view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.206629 diffgram-0.9.7/diffgram/job/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/job/guide.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13708 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/job/job.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/diffgram/label/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      941 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/label/label_new.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/label/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/diffgram/member/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/member/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/diffgram/pytorch_diffgram/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/pytorch_diffgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/pytorch_diffgram/diffgram_pytorch_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/diffgram/regular/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/regular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/regular/regular.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/diffgram/role/
+-rw-r--r--   0 runner    (1001) docker     (121)     5417 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/role/Role.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/diffgram/task/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/task/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/diffgram/tensorflow_diffgram/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/tensorflow_diffgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3859 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/tensorflow_diffgram/diffgram_tensorflow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/tensorflow_diffgram/pytorch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/diffgram/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20268 2022-10-07 14:11:53.000000 diffgram-0.9.7/diffgram/utils/visualization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.202629 diffgram-0.9.7/diffgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2852 2022-10-07 14:14:10.000000 diffgram-0.9.7/diffgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-10-07 14:14:10.000000 diffgram-0.9.7/diffgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 14:14:10.000000 diffgram-0.9.7/diffgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-07 14:14:10.000000 diffgram-0.9.7/diffgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-07 14:14:10.000000 diffgram-0.9.7/diffgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-07 14:14:10.210629 diffgram-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-10-07 14:11:53.000000 diffgram-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 14:14:10.210629 diffgram-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 14:11:53.000000 diffgram-0.9.7/tests/__init__.py
```

### Comparing `diffgram-0.9.6/PKG-INFO` & `diffgram-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffgram
-Version: 0.9.6
+Version: 0.9.7
 Summary: SDK for Diffgram
 Home-page: https://github.com/diffgram/python-sdk
 Author: Diffgram
 Author-email: support@diffgram.com
 License: UNKNOWN
 Description: 
         # SDK for Diffgram
```

### Comparing `diffgram-0.9.6/diffgram/brain/brain.py` & `diffgram-0.9.7/diffgram/brain/brain.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/brain/inference.py` & `diffgram-0.9.7/diffgram/brain/inference.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/brain/train.py` & `diffgram-0.9.7/diffgram/brain/train.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/convert/convert.py` & `diffgram-0.9.7/diffgram/convert/convert.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/core/core.py` & `diffgram-0.9.7/diffgram/core/core.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/core/diffgram_dataset_iterator.py` & `diffgram-0.9.7/diffgram/core/diffgram_dataset_iterator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 from PIL import Image, ImageDraw
 from imageio import imread
 import numpy as np
 import traceback
 import sys
 from threading import Thread
 from concurrent.futures import ThreadPoolExecutor
+from typing import Callable
 
 
 class DiffgramDatasetIterator:
     diffgram_file_id_list: list
     max_size_cache: int = 1073741824
     pool: ThreadPoolExecutor
     project: 'Project'
     file_cache: dict
     _internal_file_list: list
     current_file_index: int
+    custom_signer_fn: Callable
 
     def __init__(self,
                  project,
                  diffgram_file_id_list,
                  validate_ids = True,
                  max_size_cache = 1073741824,
-                 max_num_concurrent_fetches = 25):
+                 max_num_concurrent_fetches = 25,
+                 custom_signer_fn = None):
         """
 
         :param project (sdk.core.core.Project): A Project object from the Diffgram SDK
         :param diffgram_file_list (list): An arbitrary number of file ID's from Diffgram.
         """
         self.diffgram_file_id_list = []
         self.max_size_cache = 1073741824
         self.pool = None
+        self.custom_signer_fn = custom_signer_fn
         self.file_cache = {}
         self._internal_file_list = []
         self.current_file_index = 0
         self.start_iterator(
             project = project,
             diffgram_file_id_list = diffgram_file_id_list,
             validate_ids = validate_ids,
@@ -114,24 +118,32 @@
         result = self.project.file.file_list_exists(
             self.diffgram_file_id_list,
             use_session = False)
         if not result:
             raise Exception(
                 'Some file IDs do not belong to the project. Please provide only files from the same project.')
 
+    def set_custom_url_signer(self, signer_fn: Callable):
+        self.custom_signer_fn = signer_fn
+
     def get_image_data(self, diffgram_file):
         MAX_RETRIES = 10
         image = None
         if hasattr(diffgram_file, 'image'):
             for i in range(0, MAX_RETRIES):
                 try:
+                    url = None
                     if diffgram_file.image:
                         url = diffgram_file.image.get('url_signed')
-                        if url:
-                            image = imread(diffgram_file.image.get('url_signed'))
+                    if diffgram_file.image and self.custom_signer_fn is not None:
+                        blob_path = diffgram_file.image['url_signed_blob_path']
+                        bucket_name = diffgram_file.image['bucket_name']
+                        url = self.custom_signer_fn(blob_path, bucket_name)
+                    if url:
+                        image = imread(url)
                     break
                 except Exception as e:
                     if i < MAX_RETRIES - 1:
                         continue
                     else:
                         print('Fetch Image Failed: Diffgram File ID: {}'.format(diffgram_file.id))
                         print(traceback.format_exc())
```

### Comparing `diffgram-0.9.6/diffgram/core/directory.py` & `diffgram-0.9.7/diffgram/core/directory.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/core/sliced_directory.py` & `diffgram-0.9.7/diffgram/core/sliced_directory.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/export/export.py` & `diffgram-0.9.7/diffgram/export/export.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/file/file.py` & `diffgram-0.9.7/diffgram/file/file.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/file/file_3d.py` & `diffgram-0.9.7/diffgram/file/file_3d.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/file/file_constructor.py` & `diffgram-0.9.7/diffgram/file/file_constructor.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/file/test_existing_instances.py` & `diffgram-0.9.7/diffgram/file/test_existing_instances.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/file/view.py` & `diffgram-0.9.7/diffgram/file/view.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/job/guide.py` & `diffgram-0.9.7/diffgram/job/guide.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/job/job.py` & `diffgram-0.9.7/diffgram/job/job.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/label/label_new.py` & `diffgram-0.9.7/diffgram/label/label_new.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/pytorch_diffgram/diffgram_pytorch_dataset.py` & `diffgram-0.9.7/diffgram/pytorch_diffgram/diffgram_pytorch_dataset.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/role/Role.py` & `diffgram-0.9.7/diffgram/role/Role.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/task/task.py` & `diffgram-0.9.7/diffgram/task/task.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/tensorflow_diffgram/diffgram_tensorflow_dataset.py` & `diffgram-0.9.7/diffgram/tensorflow_diffgram/diffgram_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/tensorflow_diffgram/pytorch_test.py` & `diffgram-0.9.7/diffgram/tensorflow_diffgram/pytorch_test.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram/utils/visualization_utils.py` & `diffgram-0.9.7/diffgram/utils/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/diffgram.egg-info/PKG-INFO` & `diffgram-0.9.7/diffgram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffgram
-Version: 0.9.6
+Version: 0.9.7
 Summary: SDK for Diffgram
 Home-page: https://github.com/diffgram/python-sdk
 Author: Diffgram
 Author-email: support@diffgram.com
 License: UNKNOWN
 Description: 
         # SDK for Diffgram
```

### Comparing `diffgram-0.9.6/diffgram.egg-info/SOURCES.txt` & `diffgram-0.9.7/diffgram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diffgram-0.9.6/setup.py` & `diffgram-0.9.7/setup.py`

 * *Files identical despite different names*

