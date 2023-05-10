# Comparing `tmp/codefast-23.5.5.11.tar.gz` & `tmp/codefast-23.5.7.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codefast-23.5.5.11.tar", last modified: Fri May  5 03:21:24 2023, max compression
+gzip compressed data, was "dist/codefast-23.5.7.16.tar", last modified: Sun May  7 08:47:17 2023, max compression
```

## Comparing `codefast-23.5.5.11.tar` & `codefast-23.5.7.16.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.904297 codefast-23.5.5.11/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1074 2021-08-14 02:45:04.000000 codefast-23.5.5.11/LICENSE
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1485 2023-05-05 03:21:24.904297 codefast-23.5.5.11/PKG-INFO
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1115 2021-08-14 02:45:04.000000 codefast-23.5.5.11/README.md
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.896297 codefast-23.5.5.11/codefast/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1605 2023-04-08 02:18:46.000000 codefast-23.5.5.11/codefast/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6075 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/argparser.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/asyncio/
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1368 2023-04-19 05:45:01.000000 codefast-23.5.5.11/codefast/asyncio/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1777 2023-05-04 16:26:49.000000 codefast-23.5.5.11/codefast/asyncio/rabbitmq.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/axe/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       34 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/axe/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2232 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/axe/axe.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1029 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/axe.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/base/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       31 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/base/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3880 2022-12-25 13:22:03.000000 codefast-23.5.5.11/codefast/base/format_print.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/betterargs/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       71 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/betterargs/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4719 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/betterargs/abstractclient.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      692 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/cn.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2646 2022-11-19 16:15:49.000000 codefast-23.5.5.11/codefast/concurrency.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/concurrent/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/concurrent/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2891 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/concurrent/fastapi_demo.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4328 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/concurrent/scheduler.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2108 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/constants.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      592 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/core.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/decorators/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3105 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/decorators/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)      440 2022-12-15 06:35:33.000000 codefast-23.5.5.11/codefast/decorators/log.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2886 2023-04-28 12:37:33.000000 codefast-23.5.5.11/codefast/decorators/retry.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    11928 2023-01-09 08:00:38.000000 codefast-23.5.5.11/codefast/ds.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      112 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/exception.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/experimental/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2023-01-10 00:15:53.000000 codefast-23.5.5.11/codefast/experimental/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)      581 2023-01-10 02:42:34.000000 codefast-23.5.5.11/codefast/experimental/nsq.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/fio/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       23 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/fio/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     5951 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/fio/ffpb.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/frameworks/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1103 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/frameworks/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/functools/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       75 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/functools/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      485 2023-01-02 02:54:54.000000 codefast-23.5.5.11/codefast/functools/random.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1042 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/functools/subroutine.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/io/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      174 2023-02-05 03:01:40.000000 codefast-23.5.5.11/codefast/io/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3773 2023-03-29 03:50:19.000000 codefast-23.5.5.11/codefast/io/_json.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3328 2022-12-04 12:10:17.000000 codefast-23.5.5.11/codefast/io/dblite.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     7818 2023-03-29 13:37:50.000000 codefast-23.5.5.11/codefast/io/file.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     4411 2023-04-12 12:05:54.000000 codefast-23.5.5.11/codefast/io/osdb.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3857 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/io/sqlite.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3310 2022-12-28 09:45:27.000000 codefast-23.5.5.11/codefast/logger.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      716 2023-04-07 06:17:01.000000 codefast-23.5.5.11/codefast/math.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/network/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      135 2023-04-07 06:18:56.000000 codefast-23.5.5.11/codefast/network/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1213 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/network/curl.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      587 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/network/factory.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2681 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/network/richdownloader.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3778 2023-04-07 06:18:28.000000 codefast-23.5.5.11/codefast/network/tools.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/patterns/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       70 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/patterns/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1223 2022-12-10 01:39:19.000000 codefast-23.5.5.11/codefast/patterns/factory_method.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3320 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/patterns/observer.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1844 2023-04-12 13:39:31.000000 codefast-23.5.5.11/codefast/patterns/pipeline.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      773 2022-12-27 13:57:07.000000 codefast-23.5.5.11/codefast/patterns/responsibility_chain.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      395 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/patterns/singleton.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1303 2022-12-15 06:38:07.000000 codefast-23.5.5.11/codefast/reader.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/supercell/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       21 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/supercell/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      124 2022-11-19 13:54:17.000000 codefast-23.5.5.11/codefast/tmp.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast/types/
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1064 2022-11-23 05:27:16.000000 codefast-23.5.5.11/codefast/types/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    11921 2023-04-13 00:21:26.000000 codefast-23.5.5.11/codefast/utils.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/codefast.egg-info/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1485 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1676 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/SOURCES.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/dependency_links.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       96 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/requires.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       15 2023-05-05 03:21:24.000000 codefast-23.5.5.11/codefast.egg-info/top_level.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-05-05 03:21:24.904297 codefast-23.5.5.11/setup.cfg
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      878 2023-04-07 08:56:08.000000 codefast-23.5.5.11/setup.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:21:24.900297 codefast-23.5.5.11/tests/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-18 12:52:35.000000 codefast-23.5.5.11/tests/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      825 2023-04-18 13:01:02.000000 codefast-23.5.5.11/tests/test_unique_session.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.261715 codefast-23.5.7.16/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1074 2021-08-14 02:45:04.000000 codefast-23.5.7.16/LICENSE
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)     1485 2023-05-07 08:47:17.261715 codefast-23.5.7.16/PKG-INFO
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1115 2021-08-14 02:45:04.000000 codefast-23.5.7.16/README.md
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.245715 codefast-23.5.7.16/codefast/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1605 2023-04-08 02:18:46.000000 codefast-23.5.7.16/codefast/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6075 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/argparser.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast/asyncio/
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1368 2023-04-19 05:45:01.000000 codefast-23.5.7.16/codefast/asyncio/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1777 2023-05-04 16:26:49.000000 codefast-23.5.7.16/codefast/asyncio/rabbitmq.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast/axe/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       34 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/axe/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2232 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/axe/axe.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1029 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/axe.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast/base/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       31 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/base/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3880 2022-12-25 13:22:03.000000 codefast-23.5.7.16/codefast/base/format_print.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast/betterargs/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       71 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/betterargs/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4719 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/betterargs/abstractclient.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      692 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/cn.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2646 2022-11-19 16:15:49.000000 codefast-23.5.7.16/codefast/concurrency.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast/concurrent/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/concurrent/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2891 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/concurrent/fastapi_demo.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4328 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/concurrent/scheduler.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2108 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/constants.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      592 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/core.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast/decorators/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3105 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/decorators/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)      440 2022-12-15 06:35:33.000000 codefast-23.5.7.16/codefast/decorators/log.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2886 2023-04-28 12:37:33.000000 codefast-23.5.7.16/codefast/decorators/retry.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    11928 2023-01-09 08:00:38.000000 codefast-23.5.7.16/codefast/ds.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      112 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/exception.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast/experimental/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-01-10 00:15:53.000000 codefast-23.5.7.16/codefast/experimental/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)      581 2023-01-10 02:42:34.000000 codefast-23.5.7.16/codefast/experimental/nsq.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast/fio/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       23 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/fio/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     5951 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/fio/ffpb.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.253714 codefast-23.5.7.16/codefast/frameworks/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1103 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/frameworks/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.253714 codefast-23.5.7.16/codefast/functools/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       75 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/functools/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      485 2023-01-02 02:54:54.000000 codefast-23.5.7.16/codefast/functools/random.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1042 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/functools/subroutine.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.253714 codefast-23.5.7.16/codefast/io/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      174 2023-02-05 03:01:40.000000 codefast-23.5.7.16/codefast/io/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3912 2023-05-07 07:55:23.000000 codefast-23.5.7.16/codefast/io/_json.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     3328 2022-12-04 12:10:17.000000 codefast-23.5.7.16/codefast/io/dblite.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     7818 2023-03-29 13:37:50.000000 codefast-23.5.7.16/codefast/io/file.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     4411 2023-04-12 12:05:54.000000 codefast-23.5.7.16/codefast/io/osdb.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     3857 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/io/sqlite.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3310 2022-12-28 09:45:27.000000 codefast-23.5.7.16/codefast/logger.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      716 2023-04-07 06:17:01.000000 codefast-23.5.7.16/codefast/math.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.257715 codefast-23.5.7.16/codefast/network/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      135 2023-04-07 06:18:56.000000 codefast-23.5.7.16/codefast/network/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1213 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/network/curl.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      587 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/network/factory.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2681 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/network/richdownloader.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3778 2023-04-07 06:18:28.000000 codefast-23.5.7.16/codefast/network/tools.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.261715 codefast-23.5.7.16/codefast/patterns/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       70 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/patterns/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1223 2022-12-10 01:39:19.000000 codefast-23.5.7.16/codefast/patterns/factory_method.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     3320 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/patterns/observer.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1844 2023-04-12 13:39:31.000000 codefast-23.5.7.16/codefast/patterns/pipeline.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      773 2022-12-27 13:57:07.000000 codefast-23.5.7.16/codefast/patterns/responsibility_chain.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      395 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/patterns/singleton.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1303 2022-12-15 06:38:07.000000 codefast-23.5.7.16/codefast/reader.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.261715 codefast-23.5.7.16/codefast/supercell/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       21 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/supercell/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      124 2022-11-19 13:54:17.000000 codefast-23.5.7.16/codefast/tmp.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.261715 codefast-23.5.7.16/codefast/types/
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1064 2022-11-23 05:27:16.000000 codefast-23.5.7.16/codefast/types/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    12126 2023-05-05 12:49:16.000000 codefast-23.5.7.16/codefast/utils.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.249714 codefast-23.5.7.16/codefast.egg-info/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)     1485 2023-05-07 08:47:17.000000 codefast-23.5.7.16/codefast.egg-info/PKG-INFO
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)     1676 2023-05-07 08:47:17.000000 codefast-23.5.7.16/codefast.egg-info/SOURCES.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-05-07 08:47:17.000000 codefast-23.5.7.16/codefast.egg-info/dependency_links.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       96 2023-05-07 08:47:17.000000 codefast-23.5.7.16/codefast.egg-info/requires.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       15 2023-05-07 08:47:17.000000 codefast-23.5.7.16/codefast.egg-info/top_level.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-05-07 08:47:17.261715 codefast-23.5.7.16/setup.cfg
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      878 2023-04-07 08:56:08.000000 codefast-23.5.7.16/setup.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 08:47:17.261715 codefast-23.5.7.16/tests/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-04-18 12:52:35.000000 codefast-23.5.7.16/tests/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      825 2023-04-18 13:01:02.000000 codefast-23.5.7.16/tests/test_unique_session.py
```

### Comparing `codefast-23.5.5.11/LICENSE` & `codefast-23.5.7.16/LICENSE`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/PKG-INFO` & `codefast-23.5.7.16/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefast
-Version: 23.5.5.11
+Version: 23.5.7.16
 Summary: A package for faster coding.
 Home-page: https://github.com/
 Author: Tommy
 Author-email: i@pm.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codefast-23.5.5.11/README.md` & `codefast-23.5.7.16/README.md`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/__init__.py` & `codefast-23.5.7.16/codefast/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/argparser.py` & `codefast-23.5.7.16/codefast/argparser.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/asyncio/__init__.py` & `codefast-23.5.7.16/codefast/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/asyncio/rabbitmq.py` & `codefast-23.5.7.16/codefast/asyncio/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/axe/axe.py` & `codefast-23.5.7.16/codefast/axe/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/axe.py` & `codefast-23.5.7.16/codefast/axe.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/base/format_print.py` & `codefast-23.5.7.16/codefast/base/format_print.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/betterargs/abstractclient.py` & `codefast-23.5.7.16/codefast/betterargs/abstractclient.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/cn.py` & `codefast-23.5.7.16/codefast/cn.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/concurrency.py` & `codefast-23.5.7.16/codefast/concurrency.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/concurrent/fastapi_demo.py` & `codefast-23.5.7.16/codefast/concurrent/fastapi_demo.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/concurrent/scheduler.py` & `codefast-23.5.7.16/codefast/concurrent/scheduler.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/constants.py` & `codefast-23.5.7.16/codefast/constants.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/core.py` & `codefast-23.5.7.16/codefast/core.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/decorators/__init__.py` & `codefast-23.5.7.16/codefast/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/decorators/retry.py` & `codefast-23.5.7.16/codefast/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/ds.py` & `codefast-23.5.7.16/codefast/ds.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/experimental/nsq.py` & `codefast-23.5.7.16/codefast/experimental/nsq.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/fio/ffpb.py` & `codefast-23.5.7.16/codefast/fio/ffpb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/frameworks/__init__.py` & `codefast-23.5.7.16/codefast/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/functools/subroutine.py` & `codefast-23.5.7.16/codefast/functools/subroutine.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/io/_json.py` & `codefast-23.5.7.16/codefast/io/_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,19 @@
         if len(path_or_str) < 255:
             try:
                 return json.loads(open(path_or_str, 'r').read())
             except FileNotFoundError as e:
                 warning("input is not a file, {}".format(e))
 
         try:
-            return ast.literal_eval(path_or_str)
+            obj = ast.literal_eval(path_or_str)
+            if isinstance(obj, dict):
+                return obj
+            else:
+                return json.loads(obj.replace("'", '"'))
         except SyntaxError as e:
             error("input is not a valid json string, {}".format(e))
 
         return {}
 
     def write(self, d: dict, file_name: str):
         json.dump(d, open(file_name, 'w'), ensure_ascii=False, indent=2)
```

### Comparing `codefast-23.5.5.11/codefast/io/dblite.py` & `codefast-23.5.7.16/codefast/io/dblite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/io/file.py` & `codefast-23.5.7.16/codefast/io/file.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/io/osdb.py` & `codefast-23.5.7.16/codefast/io/osdb.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/io/sqlite.py` & `codefast-23.5.7.16/codefast/io/sqlite.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/logger.py` & `codefast-23.5.7.16/codefast/logger.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/math.py` & `codefast-23.5.7.16/codefast/math.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/network/curl.py` & `codefast-23.5.7.16/codefast/network/curl.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/network/factory.py` & `codefast-23.5.7.16/codefast/network/factory.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/network/richdownloader.py` & `codefast-23.5.7.16/codefast/network/richdownloader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/network/tools.py` & `codefast-23.5.7.16/codefast/network/tools.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/patterns/factory_method.py` & `codefast-23.5.7.16/codefast/patterns/factory_method.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/patterns/observer.py` & `codefast-23.5.7.16/codefast/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/patterns/pipeline.py` & `codefast-23.5.7.16/codefast/patterns/pipeline.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/patterns/responsibility_chain.py` & `codefast-23.5.7.16/codefast/patterns/responsibility_chain.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/reader.py` & `codefast-23.5.7.16/codefast/reader.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/types/__init__.py` & `codefast-23.5.7.16/codefast/types/__init__.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/codefast/utils.py` & `codefast-23.5.7.16/codefast/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,19 +102,19 @@
 
 def underline(text: str) -> str:
     '''Print underlined text in terminal.'''
     return f"\033[4m{text}\033[0m"
 
 
 def b64decode(text_str: str) -> str:
-    return base64.urlsafe_b64decode(text_str.encode()).decode()
+    return base64.urlsafe_b64decode(text_str.encode()).decode().rstrip()
 
 
 def b64encode(text_str: str) -> str:
-    return base64.urlsafe_b64encode(text_str.encode()).decode()
+    return base64.urlsafe_b64encode(text_str.encode()).decode().rstrip()
 
 
 def uuid():
     import uuid
     return str(uuid.uuid4())
 
 
@@ -148,26 +148,30 @@
           surpress_error: bool = False,
           ignore_result: bool = False) -> str:
 
     if ignore_result:
         os.system(cmd)
         return
 
-    ret_str = ''
     try:
         ret_str = subprocess.check_output(cmd,
                                           stderr=subprocess.DEVNULL,
                                           shell=True).decode('utf8').rstrip()
-    except Exception as e:
-        if not surpress_error:
-            print(e)
-    finally:
         if print_str:
-            p(ret_str)
+            print(ret_str)
         return ret_str
+    except Exception as e:
+        if not surpress_error:
+            import traceback
+            import pprint
+            pprint.pprint({
+                'cmd': cmd,
+                'error': str(e),
+                'traceback': '\n'.join(traceback.format_exc().split('\n'))
+            })
 
 
 class CSVIO:
     '''CSV manager'''
 
     @classmethod
     def read(cls, filename: str, delimiter: str = ',') -> List[List]:
```

### Comparing `codefast-23.5.5.11/codefast.egg-info/PKG-INFO` & `codefast-23.5.7.16/codefast.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefast
-Version: 23.5.5.11
+Version: 23.5.7.16
 Summary: A package for faster coding.
 Home-page: https://github.com/
 Author: Tommy
 Author-email: i@pm.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codefast-23.5.5.11/codefast.egg-info/SOURCES.txt` & `codefast-23.5.7.16/codefast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/setup.py` & `codefast-23.5.7.16/setup.py`

 * *Files identical despite different names*

### Comparing `codefast-23.5.5.11/tests/test_unique_session.py` & `codefast-23.5.7.16/tests/test_unique_session.py`

 * *Files identical despite different names*

