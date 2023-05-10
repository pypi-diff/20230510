# Comparing `tmp/unstructured-0.6.4.tar.gz` & `tmp/unstructured-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.4.tar", last modified: Mon May  8 17:58:20 2023, max compression
+gzip compressed data, was "unstructured-0.6.5.tar", last modified: Wed May 10 04:48:50 2023, max compression
```

## Comparing `unstructured-0.6.4.tar` & `unstructured-0.6.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.158476 unstructured-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-08 17:58:11.000000 unstructured-0.6.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-08 17:58:20.158476 unstructured-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-05-08 17:58:11.000000 unstructured-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-08 17:58:20.158476 unstructured-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-08 17:58:12.000000 unstructured-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-08 17:58:12.000000 unstructured-0.6.4/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.150476 unstructured-0.6.4/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.154476 unstructured-0.6.4/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.158476 unstructured-0.6.4/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.158476 unstructured-0.6.4/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-08 17:58:12.000000 unstructured-0.6.4/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 17:58:20.146476 unstructured-0.6.4/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 17:58:20.000000 unstructured-0.6.4/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.161395 unstructured-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-10 04:48:39.000000 unstructured-0.6.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-10 04:48:50.161395 unstructured-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-05-10 04:48:39.000000 unstructured-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-10 04:48:50.161395 unstructured-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-10 04:48:39.000000 unstructured-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.141395 unstructured-0.6.5/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.141395 unstructured-0.6.5/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-10 04:48:39.000000 unstructured-0.6.5/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.141395 unstructured-0.6.5/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.149395 unstructured-0.6.5/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.149395 unstructured-0.6.5/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.149395 unstructured-0.6.5/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.157395 unstructured-0.6.5/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.161395 unstructured-0.6.5/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/partition/text_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.161395 unstructured-0.6.5/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-10 04:48:39.000000 unstructured-0.6.5/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 04:48:50.145395 unstructured-0.6.5/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-10 04:48:50.000000 unstructured-0.6.5/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 04:48:49.000000 unstructured-0.6.5/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.4/LICENSE.md` & `unstructured-0.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/PKG-INFO` & `unstructured-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.4
+Version: 0.6.5
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.4 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.5 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.4/README.md` & `unstructured-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/setup.py` & `unstructured-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             "langdetect",
             "sacremoses",
             "sentencepiece",
             "torch",
             "transformers",
         ],
         "local-inference": [
-            "unstructured-inference>=0.4.2",
+            "unstructured-inference==0.4.4",
         ],
         "s3": ["s3fs", "fsspec"],
         "azure": ["adlfs", "fsspec"],
         "github": [
             # NOTE - pygithub==1.58.0 fails due to https://github.com/PyGithub/PyGithub/issues/2436
             # In the future, we can update this to pygithub>1.58.0
             "pygithub==1.57.0",
```

### Comparing `unstructured-0.6.4/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.5/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.5/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/test_unstructured/test_utils.py` & `unstructured-0.6.5/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/cleaners/core.py` & `unstructured-0.6.5/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/cleaners/extract.py` & `unstructured-0.6.5/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/cleaners/translate.py` & `unstructured-0.6.5/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/documents/base.py` & `unstructured-0.6.5/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/documents/elements.py` & `unstructured-0.6.5/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/documents/email_elements.py` & `unstructured-0.6.5/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/documents/html.py` & `unstructured-0.6.5/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/documents/xml.py` & `unstructured-0.6.5/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/file_utils/exploration.py` & `unstructured-0.6.5/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.5/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/file_utils/filetype.py` & `unstructured-0.6.5/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/file_utils/metadata.py` & `unstructured-0.6.5/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/azure.py` & `unstructured-0.6.5/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.5/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.5/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/git.py` & `unstructured-0.6.5/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/github.py` & `unstructured-0.6.5/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.5/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.5/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/local.py` & `unstructured-0.6.5/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.5/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/s3.py` & `unstructured-0.6.5/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/slack.py` & `unstructured-0.6.5/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.5/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.5/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/interfaces.py` & `unstructured-0.6.5/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/ingest/main.py` & `unstructured-0.6.5/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/nlp/english-words.txt` & `unstructured-0.6.5/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/nlp/english_words.py` & `unstructured-0.6.5/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/nlp/patterns.py` & `unstructured-0.6.5/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/nlp/tokenize.py` & `unstructured-0.6.5/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/__init__.py` & `unstructured-0.6.5/unstructured/partition/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests  # type: ignore
 
 from unstructured.documents.elements import Element
 
 
 def _partition_via_api(
     filename: str = "",
-    file: Optional[bytes] = None,
+    file: Optional[Union[BinaryIO, bytes]] = None,
     url: str = "https://ml.unstructured.io/layout/pdf",
     token: Optional[str] = None,
     data: Optional[dict] = None,  # NOTE(alan): Remove after different models are handled by routing
     include_page_breaks: bool = False,
 ) -> List[Element]:
     """Use API for partitioning."""
     if not filename and not file:
```

### Comparing `unstructured-0.6.4/unstructured/partition/api.py` & `unstructured-0.6.5/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/auto.py` & `unstructured-0.6.5/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/common.py` & `unstructured-0.6.5/unstructured/partition/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import subprocess
-from typing import List, Optional, Tuple, Union
+from io import BytesIO
+from tempfile import SpooledTemporaryFile
+from typing import BinaryIO, List, Optional, Tuple, Union
 
 from unstructured.documents.elements import (
     TYPE_TO_TEXT_ELEMENT_MAP,
     CheckBox,
     Element,
     ElementMetadata,
     ListItem,
@@ -153,7 +155,19 @@
     if sum([(arg is not None and arg != "") for arg in kwargs.values()]) != 1:
         names = list(kwargs.keys())
         if len(names) > 1:
             message = f"Exactly one of {', '.join(names[:-1])} and {names[-1]} must be specified."
         else:
             message = f"{names[0]} must be specified."
         raise ValueError(message)
+
+
+def spooled_to_bytes_io_if_needed(
+    file_obj: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]],
+) -> Optional[Union[bytes, BinaryIO]]:
+    if isinstance(file_obj, SpooledTemporaryFile):
+        file_obj.seek(0)
+        contents = file_obj.read()
+        return BytesIO(contents)
+    else:
+        # Return the original file object if it's not a SpooledTemporaryFile
+        return file_obj
```

### Comparing `unstructured-0.6.4/unstructured/partition/doc.py` & `unstructured-0.6.5/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/docx.py` & `unstructured-0.6.5/unstructured/partition/docx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 import tempfile
-from typing import IO, List, Optional
+from tempfile import SpooledTemporaryFile
+from typing import IO, BinaryIO, List, Optional, Union, cast
 
 import docx
 import pypandoc
 
 from unstructured.cleaners.core import clean_bullets
 from unstructured.documents.elements import (
     Address,
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     Text,
     Title,
 )
-from unstructured.partition.common import exactly_one
+from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 from unstructured.partition.text_type import (
     is_bulleted_text,
     is_possible_narrative_text,
     is_possible_title,
     is_us_city_state_zip,
 )
 
@@ -58,15 +59,15 @@
     "TOCHeading": Title,
     "Title": Title,
 }
 
 
 def partition_docx(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     metadata_filename: Optional[str] = None,
 ) -> List[Element]:
     """Partitions Microsoft Word Documents in .docx format into its document elements.
 
     Parameters
     ----------
      filename
@@ -81,15 +82,17 @@
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file)
 
     if filename is not None:
         document = docx.Document(filename)
     elif file is not None:
-        document = docx.Document(file)
+        document = docx.Document(
+            spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file)),
+        )
 
     metadata_filename = metadata_filename or filename
     elements: List[Element] = []
     for paragraph in document.paragraphs:
         element = _paragraph_to_element(paragraph)
         if element is not None:
             element.metadata = ElementMetadata(filename=metadata_filename)
```

### Comparing `unstructured-0.6.4/unstructured/partition/email.py` & `unstructured-0.6.5/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/epub.py` & `unstructured-0.6.5/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/html.py` & `unstructured-0.6.5/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/image.py` & `unstructured-0.6.5/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/json.py` & `unstructured-0.6.5/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/md.py` & `unstructured-0.6.5/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/msg.py` & `unstructured-0.6.5/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/odt.py` & `unstructured-0.6.5/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/pdf.py` & `unstructured-0.6.5/unstructured/partition/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import warnings
-from typing import BinaryIO, List, Optional, cast
+from tempfile import SpooledTemporaryFile
+from typing import BinaryIO, List, Optional, Union, cast
 
 import pdf2image
 import pytesseract
 from pdfminer.high_level import extract_pages
 from pdfminer.utils import open_filename
 from PIL import Image
 
@@ -12,23 +13,24 @@
 from unstructured.documents.elements import Element, ElementMetadata, PageBreak
 from unstructured.nlp.patterns import PARAGRAPH_PATTERN
 from unstructured.partition import _partition_via_api
 from unstructured.partition.common import (
     add_element_metadata,
     document_to_element_list,
     exactly_one,
+    spooled_to_bytes_io_if_needed,
 )
 from unstructured.partition.strategies import determine_pdf_or_image_strategy
 from unstructured.partition.text import partition_text
 from unstructured.utils import requires_dependencies
 
 
 def partition_pdf(
     filename: str = "",
-    file: Optional[bytes] = None,
+    file: Optional[Union[BinaryIO, SpooledTemporaryFile]] = None,
     url: Optional[str] = None,
     template: str = "layout/pdf",
     token: Optional[str] = None,
     include_page_breaks: bool = False,
     strategy: str = "hi_res",
     infer_table_structure: bool = False,
     encoding: str = "utf-8",
@@ -82,15 +84,15 @@
         encoding=encoding,
         ocr_languages=ocr_languages,
     )
 
 
 def partition_pdf_or_image(
     filename: str = "",
-    file: Optional[bytes] = None,
+    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     url: Optional[str] = "https://ml.unstructured.io/",
     template: str = "layout/pdf",
     token: Optional[str] = None,
     is_image: bool = False,
     include_page_breaks: bool = False,
     strategy: str = "hi_res",
     infer_table_structure: bool = False,
@@ -118,26 +120,26 @@
 
         if strategy == "hi_res":
             # NOTE(robinson): Catches a UserWarning that occurs when detectron is called
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 layout_elements = _partition_pdf_or_image_local(
                     filename=filename,
-                    file=file,
+                    file=spooled_to_bytes_io_if_needed(file),
                     template=out_template,
                     is_image=is_image,
                     infer_table_structure=infer_table_structure,
                     include_page_breaks=True,
                     ocr_languages=ocr_languages,
                 )
 
         elif strategy == "fast":
             return _partition_pdf_with_pdfminer(
                 filename=filename,
-                file=file,
+                file=spooled_to_bytes_io_if_needed(file),
                 include_page_breaks=include_page_breaks,
                 encoding=encoding,
             )
 
         elif strategy == "ocr_only":
             # NOTE(robinson): Catches file conversion warnings when running with PDFs
             with warnings.catch_warnings():
@@ -155,15 +157,15 @@
             template = "layout/pdf"
         # NOTE(alan): Remove after different models are handled by routing
         data = {"model": "checkbox"} if (template == "checkbox") else None
         url = f"{url.rstrip('/')}/{template.lstrip('/')}"
         # NOTE(alan): Remove "data=data" after different models are handled by routing
         layout_elements = _partition_via_api(
             filename=filename,
-            file=file,
+            file=cast(BinaryIO, file),
             url=url,
             token=token,
             data=data,
             include_page_breaks=True,
         )
 
     return add_element_metadata(
@@ -171,15 +173,15 @@
         include_page_breaks=include_page_breaks,
         filename=filename,
     )
 
 
 def _partition_pdf_or_image_local(
     filename: str = "",
-    file: Optional[bytes] = None,
+    file: Optional[Union[bytes, BinaryIO]] = None,
     template: Optional[str] = None,
     is_image: bool = False,
     infer_table_structure: bool = False,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
 ) -> List[Element]:
     """Partition using package installed locally."""
@@ -222,15 +224,15 @@
 
     return document_to_element_list(layout, include_page_breaks=include_page_breaks)
 
 
 @requires_dependencies("pdfminer", "local-inference")
 def _partition_pdf_with_pdfminer(
     filename: str = "",
-    file: Optional[bytes] = None,
+    file: Optional[BinaryIO] = None,
     include_page_breaks: bool = False,
     encoding: str = "utf-8",
 ) -> List[Element]:
     """Partitions a PDF using PDFMiner instead of using a layoutmodel. Used for faster
     processing or detectron2 is not available.
 
     Implementation is based on the `extract_text` implemenation in pdfminer.six, but
@@ -296,15 +298,15 @@
             elements.append(PageBreak())
 
     return elements
 
 
 def _partition_pdf_or_image_with_ocr(
     filename: str = "",
-    file: Optional[bytes] = None,
+    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = False,
     ocr_languages: str = "eng",
     is_image: bool = False,
 ):
     """Partitions and image or PDF using Tesseract OCR. For PDFs, each page is converted
     to an image prior to processing."""
     if is_image:
```

### Comparing `unstructured-0.6.4/unstructured/partition/ppt.py` & `unstructured-0.6.5/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/pptx.py` & `unstructured-0.6.5/unstructured/partition/pptx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from typing import IO, List, Optional
+from tempfile import SpooledTemporaryFile
+from typing import IO, BinaryIO, List, Optional, Union, cast
 
 import pptx
 
 from unstructured.documents.elements import (
     Element,
     ElementMetadata,
     ListItem,
     NarrativeText,
     PageBreak,
     Text,
     Title,
 )
-from unstructured.partition.common import exactly_one
+from unstructured.partition.common import exactly_one, spooled_to_bytes_io_if_needed
 from unstructured.partition.text_type import (
     is_possible_narrative_text,
     is_possible_title,
 )
 
 OPENXML_SCHEMA_NAME = "{http://schemas.openxmlformats.org/drawingml/2006/main}"
 
 
 def partition_pptx(
     filename: Optional[str] = None,
-    file: Optional[IO] = None,
+    file: Optional[Union[IO, SpooledTemporaryFile]] = None,
     include_page_breaks: bool = True,
     metadata_filename: Optional[str] = None,
 ) -> List[Element]:
     """Partitions Microsoft PowerPoint Documents in .pptx format into its document elements.
 
     Parameters
     ----------
@@ -44,15 +45,17 @@
 
     # Verify that only one of the arguments was provided
     exactly_one(filename=filename, file=file)
 
     if filename is not None:
         presentation = pptx.Presentation(filename)
     elif file is not None:
-        presentation = pptx.Presentation(file)
+        presentation = pptx.Presentation(
+            spooled_to_bytes_io_if_needed(cast(Union[BinaryIO, SpooledTemporaryFile], file)),
+        )
 
     elements: List[Element] = []
     metadata_filename = metadata_filename or filename
     metadata = ElementMetadata(filename=metadata_filename)
     num_slides = len(presentation.slides)
     for i, slide in enumerate(presentation.slides):
         metadata.page_number = i + 1
```

### Comparing `unstructured-0.6.4/unstructured/partition/rtf.py` & `unstructured-0.6.5/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/strategies.py` & `unstructured-0.6.5/unstructured/partition/strategies.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import BinaryIO, Dict, List, Optional, cast
+from tempfile import SpooledTemporaryFile
+from typing import BinaryIO, Dict, List, Optional, Union, cast
 
 from pdfminer.pdfpage import PDFPage, PDFTextExtractionNotAllowed
 from pdfminer.utils import open_filename
 
 from unstructured.logger import logger
 from unstructured.partition.common import exactly_one
 from unstructured.utils import dependency_exists
@@ -27,15 +28,18 @@
     valid_filetypes = VALID_STRATEGIES.get(strategy, None)
     if valid_filetypes is None:
         raise ValueError(f"{strategy} is not a valid strategy.")
     if filetype not in valid_filetypes:
         raise ValueError(f"{strategy} is not a valid strategy for filetype {filetype}.")
 
 
-def is_pdf_text_extractable(filename: str = "", file: Optional[bytes] = None):
+def is_pdf_text_extractable(
+    filename: str = "",
+    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
+):
     """Checks to see if the text from a PDF document is extractable. Sometimes the
     text is not extractable due to PDF security settings."""
     exactly_one(filename=filename, file=file)
 
     def _fp_is_extractable(fp):
         try:
             next(PDFPage.get_pages(fp, check_extractable=True))
@@ -52,15 +56,15 @@
         fp = cast(BinaryIO, file)
         return _fp_is_extractable(fp)
 
 
 def determine_pdf_or_image_strategy(
     strategy: str,
     filename: str = "",
-    file: Optional[bytes] = None,
+    file: Optional[Union[bytes, BinaryIO, SpooledTemporaryFile]] = None,
     is_image: bool = False,
 ):
     """Determines what strategy to use for processing PDFs or images, accounting for fallback
     logic if some dependencies are not available."""
     pytesseract_installed = dependency_exists("pytesseract")
     detectron2_installed = dependency_exists("detectron2")
```

### Comparing `unstructured-0.6.4/unstructured/partition/text.py` & `unstructured-0.6.5/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/partition/text_type.py` & `unstructured-0.6.5/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/staging/argilla.py` & `unstructured-0.6.5/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/staging/base.py` & `unstructured-0.6.5/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/staging/baseplate.py` & `unstructured-0.6.5/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/staging/datasaur.py` & `unstructured-0.6.5/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/staging/huggingface.py` & `unstructured-0.6.5/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/staging/label_box.py` & `unstructured-0.6.5/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/staging/label_studio.py` & `unstructured-0.6.5/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/staging/prodigy.py` & `unstructured-0.6.5/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured/utils.py` & `unstructured-0.6.5/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.4/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.5/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.4
+Version: 0.6.5
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.4 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.5 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.4/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.5/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

