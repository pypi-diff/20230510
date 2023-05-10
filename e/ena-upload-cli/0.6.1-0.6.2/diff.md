# Comparing `tmp/ena-upload-cli-0.6.1.tar.gz` & `tmp/ena-upload-cli-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ena-upload-cli-0.6.1.tar", last modified: Tue Jul 26 15:47:32 2022, max compression
+gzip compressed data, was "ena-upload-cli-0.6.2.tar", last modified: Wed May 10 12:21:31 2023, max compression
```

## Comparing `ena-upload-cli-0.6.1.tar` & `ena-upload-cli-0.6.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:47:32.534593 ena-upload-cli-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    20884 2022-07-26 15:47:32.534593 ena-upload-cli-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20413 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:47:32.530593 ena-upload-cli-0.6.1/ena_upload/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/check_remote.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    37836 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/ena_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:47:32.534593 ena-upload-cli-0.6.1/ena_upload/templates/
--rw-r--r--   0 runner    (1001) docker     (121)    11094 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA.project.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     5757 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_FILE.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_LIBRARY_SELECTION.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_LIBRARY_SOURCE.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4397 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml
--rw-r--r--   0 runner    (1001) docker     (121)    11114 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_PLATFORM.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)     2577 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_experiments.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)     1352 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_runs.xml
--rw-r--r--   0 runner    (1001) docker     (121)     8670 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000011.xml
--rw-r--r--   0 runner    (1001) docker     (121)    21642 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000012.xml
--rw-r--r--   0 runner    (1001) docker     (121)    24521 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000013.xml
--rw-r--r--   0 runner    (1001) docker     (121)    27548 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000014.xml
--rw-r--r--   0 runner    (1001) docker     (121)    22702 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000015.xml
--rw-r--r--   0 runner    (1001) docker     (121)    22549 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000016.xml
--rw-r--r--   0 runner    (1001) docker     (121)    22729 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000017.xml
--rw-r--r--   0 runner    (1001) docker     (121)    24307 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000018.xml
--rw-r--r--   0 runner    (1001) docker     (121)    31698 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000019.xml
--rw-r--r--   0 runner    (1001) docker     (121)    27887 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000020.xml
--rw-r--r--   0 runner    (1001) docker     (121)    30052 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000021.xml
--rw-r--r--   0 runner    (1001) docker     (121)    29802 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000022.xml
--rw-r--r--   0 runner    (1001) docker     (121)    24767 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000023.xml
--rw-r--r--   0 runner    (1001) docker     (121)    36913 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000024.xml
--rw-r--r--   0 runner    (1001) docker     (121)    26283 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000025.xml
--rw-r--r--   0 runner    (1001) docker     (121)    37057 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000027.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5873 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000028.xml
--rw-r--r--   0 runner    (1001) docker     (121)    12440 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000029.xml
--rw-r--r--   0 runner    (1001) docker     (121)     8000 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000030.xml
--rw-r--r--   0 runner    (1001) docker     (121)    20581 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000031.xml
--rw-r--r--   0 runner    (1001) docker     (121)    16560 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000032.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10224 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000033.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000034.xml
--rw-r--r--   0 runner    (1001) docker     (121)     9615 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000035.xml
--rw-r--r--   0 runner    (1001) docker     (121)     7973 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000036.xml
--rw-r--r--   0 runner    (1001) docker     (121)    27479 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000037.xml
--rw-r--r--   0 runner    (1001) docker     (121)     7622 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000038.xml
--rw-r--r--   0 runner    (1001) docker     (121)     8418 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000039.xml
--rw-r--r--   0 runner    (1001) docker     (121)     6188 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000040.xml
--rw-r--r--   0 runner    (1001) docker     (121)     7805 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000041.xml
--rw-r--r--   0 runner    (1001) docker     (121)     6916 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000043.xml
--rw-r--r--   0 runner    (1001) docker     (121)     5413 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000044.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000045.xml
--rw-r--r--   0 runner    (1001) docker     (121)    15545 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000047.xml
--rw-r--r--   0 runner    (1001) docker     (121)    15826 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000048.xml
--rw-r--r--   0 runner    (1001) docker     (121)    19166 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000049.xml
--rw-r--r--   0 runner    (1001) docker     (121)    14539 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000050.xml
--rw-r--r--   0 runner    (1001) docker     (121)     4263 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000051.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10212 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000052.xml
--rw-r--r--   0 runner    (1001) docker     (121)    10107 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000053.xml
--rwxr-xr-x   0 runner    (1001) docker     (121)     1876 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_studies.xml
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_submission.xml
--rw-r--r--   0 runner    (1001) docker     (121)    55477 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/SRA.common.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    37615 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/SRA.experiment.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    48712 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/SRA.run.xsd
--rw-r--r--   0 runner    (1001) docker     (121)     5404 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/SRA.sample.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    14461 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/SRA.study.xsd
--rw-r--r--   0 runner    (1001) docker     (121)    18180 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/ena_upload/templates/SRA.submission.xsd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 15:47:32.534593 ena-upload-cli-0.6.1/ena_upload_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20884 2022-07-26 15:47:32.000000 ena-upload-cli-0.6.1/ena_upload_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-07-26 15:47:32.000000 ena-upload-cli-0.6.1/ena_upload_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 15:47:32.000000 ena-upload-cli-0.6.1/ena_upload_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-07-26 15:47:32.000000 ena-upload-cli-0.6.1/ena_upload_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-26 15:47:32.000000 ena-upload-cli-0.6.1/ena_upload_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-26 15:47:32.000000 ena-upload-cli-0.6.1/ena_upload_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-26 15:47:32.534593 ena-upload-cli-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-07-26 15:47:23.000000 ena-upload-cli-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:31.914862 ena-upload-cli-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20864 2023-05-10 12:21:31.914862 ena-upload-cli-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20413 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:31.910862 ena-upload-cli-0.6.2/ena_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/check_remote.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37836 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/ena_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:31.914862 ena-upload-cli-0.6.2/ena_upload/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA.project.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_FILE.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_LIBRARY_SELECTION.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_LIBRARY_SOURCE.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_PLATFORM.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2577 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_experiments.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1352 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_runs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000011.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    21730 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000012.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24609 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000013.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    27636 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000014.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    22790 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000015.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    22637 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000016.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000017.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24395 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000018.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31786 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000019.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    27975 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000020.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    30140 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000021.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000022.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24855 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000023.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000024.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    26371 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000025.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    37381 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000027.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000028.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000029.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000030.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000031.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    16560 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000032.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000033.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000034.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000035.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000036.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    27479 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000037.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7946 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000038.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000039.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000040.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000041.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000043.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000044.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000045.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000047.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    16456 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000048.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    19254 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000049.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    14539 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000050.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000051.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000052.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000053.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1876 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_studies.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_submission.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    56636 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/SRA.common.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    38057 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/SRA.experiment.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    48712 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/SRA.run.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/SRA.sample.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/SRA.study.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/ena_upload/templates/SRA.submission.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:21:31.914862 ena-upload-cli-0.6.2/ena_upload_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20864 2023-05-10 12:21:31.000000 ena-upload-cli-0.6.2/ena_upload_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-10 12:21:31.000000 ena-upload-cli-0.6.2/ena_upload_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:21:31.000000 ena-upload-cli-0.6.2/ena_upload_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 12:21:31.000000 ena-upload-cli-0.6.2/ena_upload_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 12:21:31.000000 ena-upload-cli-0.6.2/ena_upload_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 12:21:31.000000 ena-upload-cli-0.6.2/ena_upload_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:21:31.914862 ena-upload-cli-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 12:21:20.000000 ena-upload-cli-0.6.2/setup.py
```

### Comparing `ena-upload-cli-0.6.1/LICENSE` & `ena-upload-cli-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/PKG-INFO` & `ena-upload-cli-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ena-upload-cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: Command Line Interface to upload data to the European Nucleotide Archive
 Home-page: https://github.com/usegalaxy-eu/ena-upload-cli
 Author: Dilmurat Yusuf
 Author-email: bjoern.gruening@gmail.com
 License: MIT
 Keywords: pip,ena-upload-cli,cli,ENA,upload
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python application](https://github.com/usegalaxy-eu/ena-upload-cli/workflows/Python%20application/badge.svg)](https://github.com/usegalaxy-eu/ena-upload-cli/actions?query=workflow%3A%22Python+application%22)
 [![BioConda version](https://anaconda.org/bioconda/ena-upload-cli/badges/version.svg)](https://anaconda.org/bioconda/ena-upload-cli)
@@ -284,9 +283,7 @@
 > **Note for Windows users:** Windows, by default, does not support wildcard expansion in command-line arguments.
 > Because of this the `--data example_data/*gz` argument should be substituted with one containing a list of the data files.
 > For this example, use:
 > 
 > ```
 > --data example_data/ENA_TEST1.R1.fastq.gz example_data/ENA_TEST2.R1.fastq.gz example_data/ENA_TEST2.R2.fastq.gz
 > ```
-
-
```

### Comparing `ena-upload-cli-0.6.1/README.md` & `ena-upload-cli-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/check_remote.py` & `ena-upload-cli-0.6.2/ena_upload/check_remote.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/ena_upload.py` & `ena-upload-cli-0.6.2/ena_upload/ena_upload.py`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA.project.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA.project.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_FILE.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_FILE.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_LIBRARY_SELECTION.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_LIBRARY_SELECTION.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_LIBRARY_SOURCE.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_LIBRARY_SOURCE.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_LIBRARY_STRATEGY.xml`

```diff
@@ -35,9 +35,10 @@
   <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'chia-pet'">ChIA-PET</LIBRARY_STRATEGY>
   <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'synthetic-long-read'">Synthetic-Long-Read</LIBRARY_STRATEGY>
   <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'targeted-capture'">Targeted-Capture</LIBRARY_STRATEGY>
   <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'tethered chromatin conformation capture'">Tethered Chromatin Conformation Capture</LIBRARY_STRATEGY>
   <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'nome-seq'">NOMe-Seq</LIBRARY_STRATEGY>
   <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'chm-seq'">ChM-Seq</LIBRARY_STRATEGY>
   <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'gbs'">GBS</LIBRARY_STRATEGY>
+  <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'ribo-seq'">Ribo-Seq</LIBRARY_STRATEGY>
   <LIBRARY_STRATEGY py:when="row.library_strategy.lower().strip() == 'other'">OTHER</LIBRARY_STRATEGY>
 </py:choose>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_PLATFORM.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_PLATFORM.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_PLATFORM.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_PLATFORM.xml`

```diff
@@ -22,14 +22,15 @@
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina hiseq 2500'">Illumina HiSeq 2500</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina hiseq 3000'">Illumina HiSeq 3000</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina hiseq 4000'">Illumina HiSeq 4000</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina hiseq x'">Illumina HiSeq X</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina iseq 100'">Illumina iSeq 100</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina miseq'">Illumina MiSeq</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina miniseq'">Illumina MiniSeq</INSTRUMENT_MODEL>
+    <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina novaseq x'">Illumina NovaSeq X</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'illumina novaseq 6000'">Illumina NovaSeq 6000</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'nextseq 500'">NextSeq 500</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'nextseq 550'">NextSeq 550</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'nextseq 1000'">NextSeq 1000</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'nextseq 2000'">NextSeq 2000</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'unspecified'">unspecified</INSTRUMENT_MODEL>
   </ILLUMINA>
@@ -97,8 +98,16 @@
   <DNBSEQ py:when="row.platform.lower().strip() == 'dnbseq'" py:choose="">
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'dnbseq-t7'">DNBSEQ-T7</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'dnbseq-g400'">DNBSEQ-G400</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'dnbseq-g50'">DNBSEQ-G50</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'dnbseq-g400 fast'">DNBSEQ-G400 FAST</INSTRUMENT_MODEL>
     <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'unspecified'">unspecified</INSTRUMENT_MODEL>
   </DNBSEQ>
+  <ELEMENT py:when="row.platform.lower().strip() == 'element'" py:choose="">
+    <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'element aviti'">Element AVITI</INSTRUMENT_MODEL>
+    <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'unspecified'">unspecified</INSTRUMENT_MODEL>
+  </ELEMENT>
+  <ULTIMA py:when="row.platform.lower().strip() == 'ultima'" py:choose="">
+    <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'ug 100'">UG 100</INSTRUMENT_MODEL>
+    <INSTRUMENT_MODEL py:when="row.instrument_model.lower().strip() == 'unspecified'">unspecified</INSTRUMENT_MODEL>
+  </ULTIMA>
 </PLATFORM>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_experiments.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_experiments.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_runs.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_runs.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000011.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000011.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000011.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000011.xml`

```diff
@@ -45,20 +45,14 @@
         </py:if>
         <py:if test="attributetest(row, 'tissue_type')">
           <SAMPLE_ATTRIBUTE>
             <TAG>tissue_type</TAG>
             <VALUE>${row['tissue_type']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'collection_date')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>collection_date</TAG>
-            <VALUE>${row['collection_date']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'isolation_source')">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolation_source</TAG>
             <VALUE>${row['isolation_source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'lat_lon')">
@@ -69,14 +63,20 @@
         </py:if>
         <py:if test="attributetest(row, 'collected_by')">
           <SAMPLE_ATTRIBUTE>
             <TAG>collected_by</TAG>
             <VALUE>${row['collected_by']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'collection date')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>collection date</TAG>
+            <VALUE>${row['collection date']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000012.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000012.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000012.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000012.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000013.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000013.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000013.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000013.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000014.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000014.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000014.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000014.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000015.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000015.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000015.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000015.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000016.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000016.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000016.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000016.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000017.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000017.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000017.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000017.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000018.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000018.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000018.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000018.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000019.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000019.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000019.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000019.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000020.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000020.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000020.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000020.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000021.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000021.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000021.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000021.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000022.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000022.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000022.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000022.xml`

```diff
@@ -165,18 +165,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000023.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000023.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000023.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000023.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000024.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000024.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000024.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000024.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000025.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000025.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000025.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000025.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000027.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000027.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000027.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000027.xml`

```diff
@@ -16,18 +16,14 @@
         <py:if test="attributetest(row, 'common_name')">
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       <SAMPLE_ATTRIBUTES>
         <SAMPLE_ATTRIBUTE>
-          <TAG>Event Date/Time</TAG>
-          <VALUE>${row['Event Date/Time']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
           <TAG>Latitude Start</TAG>
           <VALUE>${row['Latitude Start']}</VALUE>
           <UNITS>DD</UNITS>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>Longitude Start</TAG>
           <VALUE>${row['Longitude Start']}</VALUE>
@@ -218,14 +214,24 @@
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>environmental package</TAG>
           <VALUE>${row['environmental package']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
+          <TAG>collection date</TAG>
+          <VALUE>${row['collection date']}</VALUE>
+        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (country and/or sea)</TAG>
+            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <SAMPLE_ATTRIBUTE>
           <TAG>broad-scale environmental context</TAG>
           <VALUE>${row['broad-scale environmental context']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>local environmental context</TAG>
           <VALUE>${row['local environmental context']}</VALUE>
         </SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000028.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000028.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000029.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000029.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000030.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000030.xml`

 * *Files 4% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000030.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000030.xml`

```diff
@@ -21,18 +21,20 @@
       <SAMPLE_ATTRIBUTES>
         <py:if test="attributetest(row, 'Event Label')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Event Label</TAG>
             <VALUE>${row['Event Label']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>Event Date/Time Start</TAG>
-          <VALUE>${row['Event Date/Time Start']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'Event Date/Time Start')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>Event Date/Time Start</TAG>
+            <VALUE>${row['Event Date/Time Start']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'Event Date/Time End')">
           <SAMPLE_ATTRIBUTE>
             <TAG>Event Date/Time End</TAG>
             <VALUE>${row['Event Date/Time End']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
@@ -102,14 +104,26 @@
           <TAG>project name</TAG>
           <VALUE>${row['project name']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>environmental package</TAG>
           <VALUE>${row['environmental package']}</VALUE>
         </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'collection date')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>collection date</TAG>
+            <VALUE>${row['collection date']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (country and/or sea)</TAG>
+            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>broad-scale environmental context</TAG>
           <VALUE>${row['broad-scale environmental context']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>local environmental context</TAG>
           <VALUE>${row['local environmental context']}</VALUE>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000031.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000031.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000031.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000031.xml`

```diff
@@ -146,18 +146,20 @@
         </py:if>
         <py:if test="attributetest(row, 'pcr conditions')">
           <SAMPLE_ATTRIBUTE>
             <TAG>pcr conditions</TAG>
             <VALUE>${row['pcr conditions']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sequence quality check')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sequence quality check</TAG>
             <VALUE>${row['sequence quality check']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'chimera check software')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000032.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000032.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000033.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000033.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000034.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000034.xml`

 * *Files 15% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000034.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000034.xml`

```diff
@@ -19,14 +19,26 @@
       </SAMPLE_NAME>
       <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       <SAMPLE_ATTRIBUTES>
         <SAMPLE_ATTRIBUTE>
           <TAG>tissue_type</TAG>
           <VALUE>${row['tissue_type']}</VALUE>
         </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'collection date')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>collection date</TAG>
+            <VALUE>${row['collection date']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (country and/or sea)</TAG>
+            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>sex</TAG>
           <VALUE>${row['sex']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <py:if test="attributetest(row, 'date of birth')">
           <SAMPLE_ATTRIBUTE>
             <TAG>date of birth</TAG>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000035.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000035.xml`

 * *Files 2% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000035.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000035.xml`

```diff
@@ -51,14 +51,26 @@
         </py:if>
         <py:if test="attributetest(row, 'protocol')">
           <SAMPLE_ATTRIBUTE>
             <TAG>protocol</TAG>
             <VALUE>${row['protocol']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'collection date')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>collection date</TAG>
+            <VALUE>${row['collection date']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (country and/or sea)</TAG>
+            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'sampling time point')">
           <SAMPLE_ATTRIBUTE>
             <TAG>sampling time point</TAG>
             <VALUE>${row['sampling time point']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'initial time point')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000036.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000036.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000037.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000037.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000038.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000038.xml`

 * *Files 5% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000038.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000038.xml`

```diff
@@ -16,18 +16,14 @@
         <py:if test="attributetest(row, 'common_name')">
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       <SAMPLE_ATTRIBUTES>
         <SAMPLE_ATTRIBUTE>
-          <TAG>Event Date/Time</TAG>
-          <VALUE>${row['Event Date/Time']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
           <TAG>Latitude Start</TAG>
           <VALUE>${row['Latitude Start']}</VALUE>
           <UNITS>DD</UNITS>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>Longitude Start</TAG>
           <VALUE>${row['Longitude Start']}</VALUE>
@@ -45,14 +41,24 @@
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>Protocol Label</TAG>
           <VALUE>${row['Protocol Label']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
+          <TAG>collection date</TAG>
+          <VALUE>${row['collection date']}</VALUE>
+        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (country and/or sea)</TAG>
+            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <SAMPLE_ATTRIBUTE>
           <TAG>broad-scale environmental context</TAG>
           <VALUE>${row['broad-scale environmental context']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>local environmental context</TAG>
           <VALUE>${row['local environmental context']}</VALUE>
         </SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000039.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000039.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000040.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000040.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000041.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000041.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000041.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000041.xml`

```diff
@@ -52,26 +52,26 @@
         <py:if test="attributetest(row, 'DNA concentration')">
           <SAMPLE_ATTRIBUTE>
             <TAG>DNA concentration</TAG>
             <VALUE>${row['DNA concentration']}</VALUE>
             <UNITS>ng/µl</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'collection_date')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>collection_date</TAG>
-            <VALUE>${row['collection_date']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'isolation_source')">
           <SAMPLE_ATTRIBUTE>
             <TAG>isolation_source</TAG>
             <VALUE>${row['isolation_source']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'collection date')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>collection date</TAG>
+            <VALUE>${row['collection date']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000043.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000043.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000044.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000044.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000044.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000044.xml`

```diff
@@ -46,22 +46,22 @@
         <py:if test="attributetest(row, 'country of travel')">
           <SAMPLE_ATTRIBUTE>
             <TAG>country of travel</TAG>
             <VALUE>${row['country of travel']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
-          <TAG>collection_date</TAG>
-          <VALUE>${row['collection_date']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
           <TAG>collected_by</TAG>
           <VALUE>${row['collected_by']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
+          <TAG>collection date</TAG>
+          <VALUE>${row['collection date']}</VALUE>
+        </SAMPLE_ATTRIBUTE>
+        <SAMPLE_ATTRIBUTE>
           <TAG>geographic location (country and/or sea)</TAG>
           <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (region and locality)</TAG>
             <VALUE>${row['geographic location (region and locality)']}</VALUE>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000045.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000045.xml`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000045.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000045.xml`

```diff
@@ -16,27 +16,27 @@
         <py:if test="attributetest(row, 'common_name')">
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       <SAMPLE_ATTRIBUTES>
         <SAMPLE_ATTRIBUTE>
-          <TAG>collection_date</TAG>
-          <VALUE>${row['collection_date']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
           <TAG>isolation_source</TAG>
           <VALUE>${row['isolation_source']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <py:if test="attributetest(row, 'collected_by')">
           <SAMPLE_ATTRIBUTE>
             <TAG>collected_by</TAG>
             <VALUE>${row['collected_by']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <SAMPLE_ATTRIBUTE>
+          <TAG>collection date</TAG>
+          <VALUE>${row['collection date']}</VALUE>
+        </SAMPLE_ATTRIBUTE>
         <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
           <SAMPLE_ATTRIBUTE>
             <TAG>geographic location (country and/or sea)</TAG>
             <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'geographic location (region and locality)')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000047.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000047.xml`

 * *Files 2% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000047.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000047.xml`

```diff
@@ -85,18 +85,20 @@
         </py:if>
         <py:if test="attributetest(row, 'adapters')">
           <SAMPLE_ATTRIBUTE>
             <TAG>adapters</TAG>
             <VALUE>${row['adapters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'relevant electronic resources')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant electronic resources</TAG>
             <VALUE>${row['relevant electronic resources']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
@@ -107,18 +109,20 @@
         </py:if>
         <py:if test="attributetest(row, 'number of standard tRNAs extracted')">
           <SAMPLE_ATTRIBUTE>
             <TAG>number of standard tRNAs extracted</TAG>
             <VALUE>${row['number of standard tRNAs extracted']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>assembly software</TAG>
-          <VALUE>${row['assembly software']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'assembly software')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>assembly software</TAG>
+            <VALUE>${row['assembly software']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'feature prediction')">
           <SAMPLE_ATTRIBUTE>
             <TAG>feature prediction</TAG>
             <VALUE>${row['feature prediction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'reference database(s)')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000048.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000048.xml`

 * *Files 2% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000048.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000048.xml`

```diff
@@ -85,18 +85,20 @@
         </py:if>
         <py:if test="attributetest(row, 'adapters')">
           <SAMPLE_ATTRIBUTE>
             <TAG>adapters</TAG>
             <VALUE>${row['adapters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'relevant electronic resources')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant electronic resources</TAG>
             <VALUE>${row['relevant electronic resources']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
@@ -107,18 +109,20 @@
         </py:if>
         <py:if test="attributetest(row, 'number of standard tRNAs extracted')">
           <SAMPLE_ATTRIBUTE>
             <TAG>number of standard tRNAs extracted</TAG>
             <VALUE>${row['number of standard tRNAs extracted']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>assembly software</TAG>
-          <VALUE>${row['assembly software']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'assembly software')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>assembly software</TAG>
+            <VALUE>${row['assembly software']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'feature prediction')">
           <SAMPLE_ATTRIBUTE>
             <TAG>feature prediction</TAG>
             <VALUE>${row['feature prediction']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'reference database(s)')">
@@ -147,34 +151,40 @@
         </py:if>
         <py:if test="attributetest(row, 'tRNA extraction software')">
           <SAMPLE_ATTRIBUTE>
             <TAG>tRNA extraction software</TAG>
             <VALUE>${row['tRNA extraction software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>completeness score</TAG>
-          <VALUE>${row['completeness score']}</VALUE>
-          <UNITS>%</UNITS>
-        </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>completeness software</TAG>
-          <VALUE>${row['completeness software']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'completeness score')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>completeness score</TAG>
+            <VALUE>${row['completeness score']}</VALUE>
+            <UNITS>%</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'completeness software')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>completeness software</TAG>
+            <VALUE>${row['completeness software']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'completeness approach')">
           <SAMPLE_ATTRIBUTE>
             <TAG>completeness approach</TAG>
             <VALUE>${row['completeness approach']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>contamination score</TAG>
-          <VALUE>${row['contamination score']}</VALUE>
-          <UNITS>%</UNITS>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'contamination score')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>contamination score</TAG>
+            <VALUE>${row['contamination score']}</VALUE>
+            <UNITS>%</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'contamination screening input')">
           <SAMPLE_ATTRIBUTE>
             <TAG>contamination screening input</TAG>
             <VALUE>${row['contamination screening input']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'contamination screening parameters')">
@@ -185,22 +195,26 @@
         </py:if>
         <py:if test="attributetest(row, 'decontamination software')">
           <SAMPLE_ATTRIBUTE>
             <TAG>decontamination software</TAG>
             <VALUE>${row['decontamination software']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>assembly quality</TAG>
-          <VALUE>${row['assembly quality']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>taxonomic identity marker</TAG>
-          <VALUE>${row['taxonomic identity marker']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'assembly quality')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>assembly quality</TAG>
+            <VALUE>${row['assembly quality']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'taxonomic identity marker')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>taxonomic identity marker</TAG>
+            <VALUE>${row['taxonomic identity marker']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'taxonomic classification')">
           <SAMPLE_ATTRIBUTE>
             <TAG>taxonomic classification</TAG>
             <VALUE>${row['taxonomic classification']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
@@ -224,21 +238,21 @@
         <py:if test="attributetest(row, 'WGA amplification kit')">
           <SAMPLE_ATTRIBUTE>
             <TAG>WGA amplification kit</TAG>
             <VALUE>${row['WGA amplification kit']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
-          <TAG>collection_date</TAG>
-          <VALUE>${row['collection_date']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
           <TAG>isolation_source</TAG>
           <VALUE>${row['isolation_source']}</VALUE>
         </SAMPLE_ATTRIBUTE>
+        <SAMPLE_ATTRIBUTE>
+          <TAG>collection date</TAG>
+          <VALUE>${row['collection date']}</VALUE>
+        </SAMPLE_ATTRIBUTE>
         <py:if test="attributetest(row, 'altitude')">
           <SAMPLE_ATTRIBUTE>
             <TAG>altitude</TAG>
             <VALUE>${row['altitude']}</VALUE>
             <UNITS>m</UNITS>
           </SAMPLE_ATTRIBUTE>
         </py:if>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000049.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000049.xml`

 * *Files 0% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000049.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000049.xml`

```diff
@@ -91,18 +91,20 @@
         </py:if>
         <py:if test="attributetest(row, 'adapters')">
           <SAMPLE_ATTRIBUTE>
             <TAG>adapters</TAG>
             <VALUE>${row['adapters']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>sequencing method</TAG>
-          <VALUE>${row['sequencing method']}</VALUE>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'sequencing method')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>sequencing method</TAG>
+            <VALUE>${row['sequencing method']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'relevant electronic resources')">
           <SAMPLE_ATTRIBUTE>
             <TAG>relevant electronic resources</TAG>
             <VALUE>${row['relevant electronic resources']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'relevant standard operating procedures')">
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000050.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000050.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000051.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000051.xml`

 * *Files 6% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000051.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000051.xml`

```diff
@@ -15,14 +15,26 @@
         <SCIENTIFIC_NAME>${row.scientific_name}</SCIENTIFIC_NAME>
         <py:if test="attributetest(row, 'common_name')">
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       <SAMPLE_ATTRIBUTES>
+        <py:if test="attributetest(row, 'collection date')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>collection date</TAG>
+            <VALUE>${row['collection date']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'geographic location (country and/or sea)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (country and/or sea)</TAG>
+            <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>sample origin</TAG>
           <VALUE>${row['sample origin']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>sample taxon name</TAG>
           <VALUE>${row['sample taxon name']}</VALUE>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000052.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000052.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000053.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000053.xml`

 * *Files 4% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_samples_ERC000053.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_samples_ERC000053.xml`

```diff
@@ -15,14 +15,42 @@
         <SCIENTIFIC_NAME>${row.scientific_name}</SCIENTIFIC_NAME>
         <py:if test="attributetest(row, 'common_name')">
           <COMMON_NAME>${row.common_name}</COMMON_NAME>
         </py:if>
       </SAMPLE_NAME>
       <DESCRIPTION>${row.sample_description}</DESCRIPTION>
       <SAMPLE_ATTRIBUTES>
+        <py:if test="attributetest(row, 'Latitude Start')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>Latitude Start</TAG>
+            <VALUE>${row['Latitude Start']}</VALUE>
+            <UNITS>DD</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'Longitude Start')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>Longitude Start</TAG>
+            <VALUE>${row['Longitude Start']}</VALUE>
+            <UNITS>DD</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'Latitude End')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>Latitude End</TAG>
+            <VALUE>${row['Latitude End']}</VALUE>
+            <UNITS>DD</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'Longitude End')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>Longitude End</TAG>
+            <VALUE>${row['Longitude End']}</VALUE>
+            <UNITS>DD</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>organism part</TAG>
           <VALUE>${row['organism part']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>lifestage</TAG>
           <VALUE>${row['lifestage']}</VALUE>
@@ -51,24 +79,28 @@
           <TAG>collection date</TAG>
           <VALUE>${row['collection date']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <SAMPLE_ATTRIBUTE>
           <TAG>geographic location (country and/or sea)</TAG>
           <VALUE>${row['geographic location (country and/or sea)']}</VALUE>
         </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>geographic location (latitude)</TAG>
-          <VALUE>${row['geographic location (latitude)']}</VALUE>
-          <UNITS>DD</UNITS>
-        </SAMPLE_ATTRIBUTE>
-        <SAMPLE_ATTRIBUTE>
-          <TAG>geographic location (longitude)</TAG>
-          <VALUE>${row['geographic location (longitude)']}</VALUE>
-          <UNITS>DD</UNITS>
-        </SAMPLE_ATTRIBUTE>
+        <py:if test="attributetest(row, 'geographic location (latitude)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (latitude)</TAG>
+            <VALUE>${row['geographic location (latitude)']}</VALUE>
+            <UNITS>DD</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'geographic location (longitude)')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>geographic location (longitude)</TAG>
+            <VALUE>${row['geographic location (longitude)']}</VALUE>
+            <UNITS>DD</UNITS>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <SAMPLE_ATTRIBUTE>
           <TAG>geographic location (region and locality)</TAG>
           <VALUE>${row['geographic location (region and locality)']}</VALUE>
         </SAMPLE_ATTRIBUTE>
         <py:if test="attributetest(row, 'identified_by')">
           <SAMPLE_ATTRIBUTE>
             <TAG>identified_by</TAG>
@@ -183,26 +215,14 @@
         </SAMPLE_ATTRIBUTE>
         <py:if test="attributetest(row, 'GAL')">
           <SAMPLE_ATTRIBUTE>
             <TAG>GAL</TAG>
             <VALUE>${row['GAL']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
-        <py:if test="attributetest(row, 'bio_material')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>bio_material</TAG>
-            <VALUE>${row['bio_material']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
-        <py:if test="attributetest(row, 'specimen_voucher')">
-          <SAMPLE_ATTRIBUTE>
-            <TAG>specimen_voucher</TAG>
-            <VALUE>${row['specimen_voucher']}</VALUE>
-          </SAMPLE_ATTRIBUTE>
-        </py:if>
         <py:if test="attributetest(row, 'specimen_id')">
           <SAMPLE_ATTRIBUTE>
             <TAG>specimen_id</TAG>
             <VALUE>${row['specimen_id']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <py:if test="attributetest(row, 'GAL_sample_id')">
@@ -213,14 +233,32 @@
         </py:if>
         <py:if test="attributetest(row, 'proxy voucher')">
           <SAMPLE_ATTRIBUTE>
             <TAG>proxy voucher</TAG>
             <VALUE>${row['proxy voucher']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
+        <py:if test="attributetest(row, 'proxy biomaterial')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>proxy biomaterial</TAG>
+            <VALUE>${row['proxy biomaterial']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'bio_material')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>bio_material</TAG>
+            <VALUE>${row['bio_material']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
+        <py:if test="attributetest(row, 'specimen_voucher')">
+          <SAMPLE_ATTRIBUTE>
+            <TAG>specimen_voucher</TAG>
+            <VALUE>${row['specimen_voucher']}</VALUE>
+          </SAMPLE_ATTRIBUTE>
+        </py:if>
         <py:if test="attributetest(row, 'culture_or_strain_id')">
           <SAMPLE_ATTRIBUTE>
             <TAG>culture_or_strain_id</TAG>
             <VALUE>${row['culture_or_strain_id']}</VALUE>
           </SAMPLE_ATTRIBUTE>
         </py:if>
         <SAMPLE_ATTRIBUTE>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_studies.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_studies.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/ENA_template_submission.xml` & `ena-upload-cli-0.6.2/ena_upload/templates/ENA_template_submission.xml`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/SRA.common.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/SRA.common.xsd`

 * *Files 2% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/SRA.common.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/SRA.common.xsd`

```diff
@@ -540,14 +540,28 @@
         </xs:annotation>
         <xs:complexType>
           <xs:sequence>
             <xs:element name="INSTRUMENT_MODEL" maxOccurs="1" minOccurs="1" type="com:typeDnbSeqModel"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
+      <xs:element name="ELEMENT">
+        <xs:complexType>
+          <xs:sequence>
+            <xs:element name="INSTRUMENT_MODEL" maxOccurs="1" minOccurs="1" type="com:typeElementModel"/>
+          </xs:sequence>
+        </xs:complexType>
+      </xs:element>
+      <xs:element name="ULTIMA">
+        <xs:complexType>
+          <xs:sequence>
+            <xs:element name="INSTRUMENT_MODEL" maxOccurs="1" minOccurs="1" type="com:typeUltimaModel"/>
+          </xs:sequence>
+        </xs:complexType>
+      </xs:element>
     </xs:choice>
   </xs:complexType>
   <xs:complexType name="SequencingDirectivesType">
     <xs:all>
       <xs:element name="SAMPLE_DEMUX_DIRECTIVE" minOccurs="0" maxOccurs="1">
         <xs:annotation>
           <xs:documentation>Tells the Archive who will execute the sample demultiplexing operation..</xs:documentation>
@@ -756,14 +770,15 @@
       <xs:enumeration value="Illumina HiSeq 2500"/>
       <xs:enumeration value="Illumina HiSeq 3000"/>
       <xs:enumeration value="Illumina HiSeq 4000"/>
       <xs:enumeration value="Illumina HiSeq X"/>
       <xs:enumeration value="Illumina iSeq 100"/>
       <xs:enumeration value="Illumina MiSeq"/>
       <xs:enumeration value="Illumina MiniSeq"/>
+      <xs:enumeration value="Illumina NovaSeq X"/>
       <xs:enumeration value="Illumina NovaSeq 6000"/>
       <xs:enumeration value="NextSeq 500"/>
       <xs:enumeration value="NextSeq 550"/>
       <xs:enumeration value="NextSeq 1000"/>
       <xs:enumeration value="NextSeq 2000"/>
       <xs:enumeration value="unspecified"/>
     </xs:restriction>
@@ -854,9 +869,21 @@
     <xs:restriction base="xs:string">
       <xs:enumeration value="MinION"/>
       <xs:enumeration value="GridION"/>
       <xs:enumeration value="PromethION"/>
       <xs:enumeration value="unspecified"/>
     </xs:restriction>
   </xs:simpleType>
+  <xs:simpleType name="typeElementModel">
+    <xs:restriction base="xs:string">
+      <xs:enumeration value="Element AVITI"/>
+      <xs:enumeration value="unspecified"/>
+    </xs:restriction>
+  </xs:simpleType>
+  <xs:simpleType name="typeUltimaModel">
+    <xs:restriction base="xs:string">
+      <xs:enumeration value="UG 100"/>
+      <xs:enumeration value="unspecified"/>
+    </xs:restriction>
+  </xs:simpleType>
   <!-- STRING ENUMERATIONS END -->
 </xs:schema>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/SRA.experiment.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/SRA.experiment.xsd`

 * *Files 1% similar despite different names*

#### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/SRA.experiment.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/SRA.experiment.xsd`

```diff
@@ -207,14 +207,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="GBS">
         <xs:annotation>
           <xs:documentation>Genotyping by sequencing is a method to discover single nucleotide polymorphisms for genotyping studies.</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Ribo-Seq">
+        <xs:annotation>
+          <xs:documentation>Ribosome profiling (also named ribosome footprinting) that uses specialized messenger RNA (mRNA) sequencing to determine which mRNAs are being actively translated. It produces a &quot;global snapshot&quot; of all the ribosomes active in a cell at a particular moment, known as a translatome.</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="OTHER">
         <xs:annotation>
           <xs:documentation>Library strategy not listed.</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
     </xs:restriction>
   </xs:simpleType>
```

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/SRA.run.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/SRA.run.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/SRA.sample.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/SRA.sample.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/SRA.study.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/SRA.study.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload/templates/SRA.submission.xsd` & `ena-upload-cli-0.6.2/ena_upload/templates/SRA.submission.xsd`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/ena_upload_cli.egg-info/PKG-INFO` & `ena-upload-cli-0.6.2/ena_upload_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ena-upload-cli
-Version: 0.6.1
+Version: 0.6.2
 Summary: Command Line Interface to upload data to the European Nucleotide Archive
 Home-page: https://github.com/usegalaxy-eu/ena-upload-cli
 Author: Dilmurat Yusuf
 Author-email: bjoern.gruening@gmail.com
 License: MIT
 Keywords: pip,ena-upload-cli,cli,ENA,upload
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python application](https://github.com/usegalaxy-eu/ena-upload-cli/workflows/Python%20application/badge.svg)](https://github.com/usegalaxy-eu/ena-upload-cli/actions?query=workflow%3A%22Python+application%22)
 [![BioConda version](https://anaconda.org/bioconda/ena-upload-cli/badges/version.svg)](https://anaconda.org/bioconda/ena-upload-cli)
@@ -284,9 +283,7 @@
 > **Note for Windows users:** Windows, by default, does not support wildcard expansion in command-line arguments.
 > Because of this the `--data example_data/*gz` argument should be substituted with one containing a list of the data files.
 > For this example, use:
 > 
 > ```
 > --data example_data/ENA_TEST1.R1.fastq.gz example_data/ENA_TEST2.R1.fastq.gz example_data/ENA_TEST2.R2.fastq.gz
 > ```
-
-
```

### Comparing `ena-upload-cli-0.6.1/ena_upload_cli.egg-info/SOURCES.txt` & `ena-upload-cli-0.6.2/ena_upload_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ena-upload-cli-0.6.1/setup.py` & `ena-upload-cli-0.6.2/setup.py`

 * *Files identical despite different names*

