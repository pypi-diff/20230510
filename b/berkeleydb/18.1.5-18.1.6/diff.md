# Comparing `tmp/berkeleydb-18.1.5.tar.gz` & `tmp/berkeleydb-18.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berkeleydb-18.1.5.tar", last modified: Fri Jan 21 14:03:19 2022, max compression
+gzip compressed data, was "berkeleydb-18.1.6.tar", last modified: Wed May 10 16:32:27 2023, max compression
```

## Comparing `berkeleydb-18.1.5.tar` & `berkeleydb-18.1.6.tar`

### file list

```diff
@@ -1,120 +1,117 @@
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.614752 berkeleydb-18.1.5/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)      149 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/.hgignore
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2079 2022-01-21 13:51:03.000000 berkeleydb-18.1.5/.hgtags
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     1616 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/BerkeleyDB_issues.txt
--rw-rw-r--   0 jcea      (1000) jcea      (1000)      937 2021-05-18 23:52:13.000000 berkeleydb-18.1.5/ChangeLog
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     1756 2022-01-20 23:27:14.000000 berkeleydb-18.1.5/LICENSE.txt
--rw-rw-r--   0 jcea      (1000) jcea      (1000)      601 2021-05-19 16:24:48.000000 berkeleydb-18.1.5/MANIFEST.in
--rw-rw-r--   0 jcea      (1000) jcea      (1000)      319 2022-01-20 23:30:33.000000 berkeleydb-18.1.5/Makefile
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2463 2022-01-21 14:03:19.614752 berkeleydb-18.1.5/PKG-INFO
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     6234 2020-11-25 14:31:28.000000 berkeleydb-18.1.5/README.txt
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     8434 2022-01-21 01:26:53.000000 berkeleydb-18.1.5/TODO.txt
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     1647 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/TODO.txt.old
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.594752 berkeleydb-18.1.5/berkeleydb.egg-info/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2463 2022-01-21 14:03:18.000000 berkeleydb-18.1.5/berkeleydb.egg-info/PKG-INFO
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2393 2022-01-21 14:03:19.000000 berkeleydb-18.1.5/berkeleydb.egg-info/SOURCES.txt
--rw-rw-r--   0 jcea      (1000) jcea      (1000)        1 2022-01-21 14:03:18.000000 berkeleydb-18.1.5/berkeleydb.egg-info/dependency_links.txt
--rw-rw-r--   0 jcea      (1000) jcea      (1000)       11 2022-01-21 14:03:18.000000 berkeleydb-18.1.5/berkeleydb.egg-info/top_level.txt
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.598752 berkeleydb-18.1.5/docs/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     6054 2021-04-24 00:34:38.000000 berkeleydb-18.1.5/docs/Makefile
--rw-r--r--   0 jcea      (1000) jcea      (1000)     1087 2018-07-01 19:33:23.000000 berkeleydb-18.1.5/docs/bitcoin.png
--rw-r--r--   0 jcea      (1000) jcea      (1000)      308 2018-07-01 19:33:23.000000 berkeleydb-18.1.5/docs/bitcoin.png.asc
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    42488 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/docs/changelog-bsddb3.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    15493 2022-01-21 13:57:14.000000 berkeleydb-18.1.5/docs/changelog.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     4264 2022-01-20 23:32:16.000000 berkeleydb-18.1.5/docs/conf.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    32508 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/docs/db.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     6970 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/docs/dbcursor.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    71174 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/docs/dbenv.rst
--rw-r--r--   0 jcea      (1000) jcea      (1000)      254 2018-07-01 19:33:23.000000 berkeleydb-18.1.5/docs/dblock.rst
--rw-r--r--   0 jcea      (1000) jcea      (1000)     2011 2020-02-10 23:58:47.000000 berkeleydb-18.1.5/docs/dblogcursor.rst
--rw-r--r--   0 jcea      (1000) jcea      (1000)     4429 2018-07-01 19:33:23.000000 berkeleydb-18.1.5/docs/dbsequence.rst
--rw-r--r--   0 jcea      (1000) jcea      (1000)     1377 2018-07-01 19:33:24.000000 berkeleydb-18.1.5/docs/dbsite.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2340 2020-11-25 14:31:28.000000 berkeleydb-18.1.5/docs/dbtxn.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2467 2021-04-25 23:37:06.000000 berkeleydb-18.1.5/docs/donate.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)      951 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/docs/history.rst
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.602752 berkeleydb-18.1.5/docs/html/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    71651 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/changelog-bsddb3.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    33832 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/changelog.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    77712 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/db.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    36251 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/dbcursor.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)   130957 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/dbenv.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     4520 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/dblock.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     9492 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/dblogcursor.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    17051 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/dbsequence.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     8496 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/dbsite.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    11236 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/dbtxn.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     8530 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/donate.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    59827 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/genindex.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     5141 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/history.html
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.602752 berkeleydb-18.1.5/docs/html/images/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     1087 2018-07-01 19:33:23.000000 berkeleydb-18.1.5/docs/html/images/bitcoin.png
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    18792 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/index.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    17885 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/introduction.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     9343 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/license.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     4032 2022-01-21 13:54:59.000000 berkeleydb-18.1.5/docs/html/search.html
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    39688 2022-01-21 13:54:48.000000 berkeleydb-18.1.5/docs/html/searchindex.js
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.606752 berkeleydb-18.1.5/docs/html/static/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    11185 2022-01-21 13:54:48.000000 berkeleydb-18.1.5/docs/html/static/alabaster.css
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    14692 2022-01-21 13:54:48.000000 berkeleydb-18.1.5/docs/html/static/basic.css
--rw-rw-r--   0 jcea      (1000) jcea      (1000)       42 2021-10-07 01:27:49.000000 berkeleydb-18.1.5/docs/html/static/custom.css
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     9758 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/doctools.js
--rw-rw-r--   0 jcea      (1000) jcea      (1000)      357 2022-01-21 13:54:48.000000 berkeleydb-18.1.5/docs/html/static/documentation_options.js
--rw-rw-r--   0 jcea      (1000) jcea      (1000)      286 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/file.png
--rw-rw-r--   0 jcea      (1000) jcea      (1000)   287630 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/jquery-3.5.1.js
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    89476 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/jquery.js
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    10854 2022-01-21 13:54:48.000000 berkeleydb-18.1.5/docs/html/static/language_data.js
--rw-rw-r--   0 jcea      (1000) jcea      (1000)       90 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/minus.png
--rw-rw-r--   0 jcea      (1000) jcea      (1000)       90 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/plus.png
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     5249 2022-01-21 13:54:48.000000 berkeleydb-18.1.5/docs/html/static/pygments.css
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    16793 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/searchtools.js
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    68420 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/underscore-1.13.1.js
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    19530 2022-01-16 23:24:09.000000 berkeleydb-18.1.5/docs/html/static/underscore.js
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     1686 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/docs/index.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    11893 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/docs/introduction.rst
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     3494 2022-01-20 23:32:16.000000 berkeleydb-18.1.5/docs/license.rst
--rw-r--r--   0 jcea      (1000) jcea      (1000)     1586 2018-07-01 19:33:23.000000 berkeleydb-18.1.5/licenses.txt
--rw-rw-r--   0 jcea      (1000) jcea      (1000)      100 2021-05-19 16:35:32.000000 berkeleydb-18.1.5/pyproject.toml
--rw-r--r--   0 jcea      (1000) jcea      (1000)       67 2022-01-21 14:03:19.614752 berkeleydb-18.1.5/setup.cfg
--rwxrwxr-x   0 jcea      (1000) jcea      (1000)     2640 2022-01-20 23:52:02.000000 berkeleydb-18.1.5/setup.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    21047 2022-01-21 13:35:57.000000 berkeleydb-18.1.5/setup3.py
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.586752 berkeleydb-18.1.5/src/
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.606752 berkeleydb-18.1.5/src/Module/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)   278965 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/src/Module/berkeleydb.c
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    10499 2021-05-19 17:24:44.000000 berkeleydb-18.1.5/src/Module/berkeleydb.h
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.606752 berkeleydb-18.1.5/src/berkeleydb/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    14240 2020-11-25 14:31:28.000000 berkeleydb-18.1.5/src/berkeleydb/__init__.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2053 2020-11-25 14:31:28.000000 berkeleydb-18.1.5/src/berkeleydb/db.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    10834 2020-11-25 14:31:28.000000 berkeleydb-18.1.5/src/berkeleydb/dbobj.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     5313 2020-11-25 14:31:28.000000 berkeleydb-18.1.5/src/berkeleydb/dbrecio.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    10191 2020-11-25 14:31:28.000000 berkeleydb-18.1.5/src/berkeleydb/dbshelve.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2815 2020-11-25 14:31:28.000000 berkeleydb-18.1.5/src/berkeleydb/dbutils.py
--rwxrwxr-x   0 jcea      (1000) jcea      (1000)     3054 2022-01-20 23:32:16.000000 berkeleydb-18.1.5/test-full_prerelease.py
--rwxrwxr-x   0 jcea      (1000) jcea      (1000)    16938 2022-01-20 23:12:31.000000 berkeleydb-18.1.5/test.py
-drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2022-01-21 14:03:19.614752 berkeleydb-18.1.5/tests/
--rw-rw-r--   0 jcea      (1000) jcea      (1000)        0 2021-04-02 16:40:02.000000 berkeleydb-18.1.5/tests/__init__.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     6129 2022-01-21 02:36:20.000000 berkeleydb-18.1.5/tests/test_all.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    18197 2022-01-21 01:51:20.000000 berkeleydb-18.1.5/tests/test_associate.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    48761 2022-01-21 01:53:46.000000 berkeleydb-18.1.5/tests/test_basics.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    16027 2022-01-21 01:55:33.000000 berkeleydb-18.1.5/tests/test_compare.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     6341 2022-01-21 01:56:24.000000 berkeleydb-18.1.5/tests/test_compat.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     2985 2022-01-21 01:57:50.000000 berkeleydb-18.1.5/tests/test_concurrent_data_store.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     3684 2022-01-21 01:58:36.000000 berkeleydb-18.1.5/tests/test_cursor_pget_bug.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     7553 2022-01-21 02:02:12.000000 berkeleydb-18.1.5/tests/test_db.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    25393 2022-01-21 02:00:49.000000 berkeleydb-18.1.5/tests/test_dbenv.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     4149 2022-01-21 02:01:14.000000 berkeleydb-18.1.5/tests/test_dbobj.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    11955 2022-01-21 02:04:29.000000 berkeleydb-18.1.5/tests/test_dbshelve.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     6251 2022-01-21 02:05:26.000000 berkeleydb-18.1.5/tests/test_distributed_transactions.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     8023 2022-01-21 02:06:07.000000 berkeleydb-18.1.5/tests/test_early_close.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     3726 2022-01-21 02:06:56.000000 berkeleydb-18.1.5/tests/test_fileid.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     5576 2022-01-21 02:07:39.000000 berkeleydb-18.1.5/tests/test_get_none.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     5708 2022-01-21 02:08:12.000000 berkeleydb-18.1.5/tests/test_heap.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     4964 2022-01-21 02:09:30.000000 berkeleydb-18.1.5/tests/test_join.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     7505 2022-01-21 02:10:13.000000 berkeleydb-18.1.5/tests/test_lock.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     6532 2022-01-21 02:10:41.000000 berkeleydb-18.1.5/tests/test_misc.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     3468 2022-01-21 02:11:04.000000 berkeleydb-18.1.5/tests/test_pickle.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     7019 2022-01-21 02:13:19.000000 berkeleydb-18.1.5/tests/test_queue.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    10012 2022-01-21 02:18:31.000000 berkeleydb-18.1.5/tests/test_recno.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    21233 2022-01-21 02:26:47.000000 berkeleydb-18.1.5/tests/test_replication.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     7322 2022-01-21 02:39:14.000000 berkeleydb-18.1.5/tests/test_sequence.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)    15500 2022-01-21 02:30:37.000000 berkeleydb-18.1.5/tests/test_thread.py
--rw-rw-r--   0 jcea      (1000) jcea      (1000)     5325 2022-01-21 02:39:26.000000 berkeleydb-18.1.5/tests/test_weakref.py
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.016946 berkeleydb-18.1.6/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      149 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/.hgignore
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2127 2023-05-10 16:29:48.000000 berkeleydb-18.1.6/.hgtags
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     1616 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/BerkeleyDB_issues.txt
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      937 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/ChangeLog
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     1756 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/LICENSE.txt
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      601 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/MANIFEST.in
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      319 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/Makefile
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2443 2023-05-10 16:32:27.020946 berkeleydb-18.1.6/PKG-INFO
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     6234 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/README.txt
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     8957 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/TODO.txt
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     1647 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/TODO.txt.old
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.004946 berkeleydb-18.1.6/berkeleydb.egg-info/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2443 2023-05-10 16:32:25.000000 berkeleydb-18.1.6/berkeleydb.egg-info/PKG-INFO
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2301 2023-05-10 16:32:26.000000 berkeleydb-18.1.6/berkeleydb.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)        1 2023-05-10 16:32:25.000000 berkeleydb-18.1.6/berkeleydb.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)       11 2023-05-10 16:32:25.000000 berkeleydb-18.1.6/berkeleydb.egg-info/top_level.txt
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.008946 berkeleydb-18.1.6/docs/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     6054 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/Makefile
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     1087 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/bitcoin.png
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      308 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/bitcoin.png.asc
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    42425 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/changelog-bsddb3.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    16053 2023-05-10 16:30:25.000000 berkeleydb-18.1.6/docs/changelog.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4264 2023-05-10 16:10:20.000000 berkeleydb-18.1.6/docs/conf.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    32508 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/db.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     6970 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/dbcursor.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    71174 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/dbenv.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      254 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/dblock.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2011 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/dblogcursor.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4429 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/dbsequence.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     1377 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/dbsite.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2340 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/dbtxn.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2467 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/donate.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      951 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/history.rst
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.012946 berkeleydb-18.1.6/docs/html/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    71521 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/changelog-bsddb3.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    34768 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/changelog.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    89763 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/db.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    40261 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/dbcursor.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)   154214 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/dbenv.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4523 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/dblock.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    10622 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/dblogcursor.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    19633 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/dbsequence.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     9501 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/dbsite.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    12895 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/dbtxn.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     8533 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/donate.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    59833 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/genindex.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     5144 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/history.html
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.012946 berkeleydb-18.1.6/docs/html/images/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     1087 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/html/images/bitcoin.png
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    70156 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/index.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    18151 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/introduction.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     9342 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/license.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4002 2023-05-10 16:28:21.000000 berkeleydb-18.1.6/docs/html/search.html
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    73704 2023-05-10 16:28:16.000000 berkeleydb-18.1.6/docs/html/searchindex.js
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.012946 berkeleydb-18.1.6/docs/html/static/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    11185 2023-05-10 16:28:16.000000 berkeleydb-18.1.6/docs/html/static/alabaster.css
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    14813 2023-05-10 16:28:16.000000 berkeleydb-18.1.6/docs/html/static/basic.css
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)       42 2022-01-08 02:29:31.000000 berkeleydb-18.1.6/docs/html/static/custom.css
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4472 2023-04-30 03:03:59.000000 berkeleydb-18.1.6/docs/html/static/doctools.js
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      422 2023-05-10 16:28:16.000000 berkeleydb-18.1.6/docs/html/static/documentation_options.js
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      286 2023-04-30 03:03:59.000000 berkeleydb-18.1.6/docs/html/static/file.png
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4758 2023-05-10 16:28:16.000000 berkeleydb-18.1.6/docs/html/static/language_data.js
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)       90 2023-04-30 03:03:59.000000 berkeleydb-18.1.6/docs/html/static/minus.png
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)       90 2023-04-30 03:03:59.000000 berkeleydb-18.1.6/docs/html/static/plus.png
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     5327 2023-05-10 16:28:16.000000 berkeleydb-18.1.6/docs/html/static/pygments.css
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    18215 2023-04-30 03:03:59.000000 berkeleydb-18.1.6/docs/html/static/searchtools.js
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4712 2023-04-30 03:03:59.000000 berkeleydb-18.1.6/docs/html/static/sphinx_highlight.js
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     1689 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/index.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    11893 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/introduction.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     3494 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/docs/license.rst
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     1586 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/licenses.txt
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)      100 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/pyproject.toml
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)       67 2023-05-10 16:32:27.020946 berkeleydb-18.1.6/setup.cfg
+-rwxrwxr-x   0 jcea      (1000) jcea      (1000)     2640 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/setup.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    21047 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/setup3.py
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.004946 berkeleydb-18.1.6/src/
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.012946 berkeleydb-18.1.6/src/Module/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)   278310 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/src/Module/berkeleydb.c
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    10499 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/src/Module/berkeleydb.h
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.012946 berkeleydb-18.1.6/src/berkeleydb/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    14240 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/src/berkeleydb/__init__.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2053 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/src/berkeleydb/db.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    10834 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/src/berkeleydb/dbobj.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     5313 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/src/berkeleydb/dbrecio.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    10191 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/src/berkeleydb/dbshelve.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2815 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/src/berkeleydb/dbutils.py
+-rwxrwxr-x   0 jcea      (1000) jcea      (1000)     3062 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/test-full_prerelease.py
+-rwxrwxr-x   0 jcea      (1000) jcea      (1000)    17238 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/test.py
+drwxrwxr-x   0 jcea      (1000) jcea      (1000)        0 2023-05-10 16:32:27.016946 berkeleydb-18.1.6/tests/
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)        0 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/__init__.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     6767 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_all.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    18197 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_associate.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    48761 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_basics.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    16027 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_compare.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     6341 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_compat.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     2985 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_concurrent_data_store.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     3684 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_cursor_pget_bug.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     7553 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_db.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    25393 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_dbenv.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4149 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_dbobj.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    11955 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_dbshelve.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     6251 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_distributed_transactions.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     8023 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_early_close.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     3726 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_fileid.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     5576 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_get_none.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     5708 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_heap.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     4964 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_join.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     7505 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_lock.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     6532 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_misc.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     3468 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_pickle.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     7019 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_queue.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    10012 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_recno.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    21233 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_replication.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     7322 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_sequence.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)    15500 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_thread.py
+-rw-rw-r--   0 jcea      (1000) jcea      (1000)     5325 2023-05-10 15:59:41.000000 berkeleydb-18.1.6/tests/test_weakref.py
```

### Comparing `berkeleydb-18.1.5/.hgtags` & `berkeleydb-18.1.6/.hgtags`

 * *Files 11% similar despite different names*

```diff
@@ -38,7 +38,8 @@
 ad93c3d9907522a784a90d41df24d478355ef132 18.1.0-pre
 5800d489c014bad9fd16b51b371808a05bc9854e 18.1.0
 4b026ef841781f298b9a247b69678e424d022e1e 18.1.1
 470411c6c59c399f39b73fac77ce661a901b7682 18.1.2
 4537900e659aa3a68c96fce27b5a9f486d91ed57 18.1.3
 097aac99c211402d00718fdd6652ac6471ff2665 18.1.4
 1ee800f9490c91e30d3efc7be9a451718feb772c 18.1.5
+b466ea616dcf7a86afa8ff318b4c6959d02478d2 18.1.6
```

### Comparing `berkeleydb-18.1.5/BerkeleyDB_issues.txt` & `berkeleydb-18.1.6/BerkeleyDB_issues.txt`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/ChangeLog` & `berkeleydb-18.1.6/ChangeLog`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/LICENSE.txt` & `berkeleydb-18.1.6/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Except when noted in individual files, this project is distributed
 under BSD 3-Clause License. More details in
 <http://opensource.org/licenses/BSD-3-Clause>.
 
 License Text:
 
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/MANIFEST.in` & `berkeleydb-18.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/PKG-INFO` & `berkeleydb-18.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: berkeleydb
-Version: 18.1.5
+Version: 18.1.6
 Summary: Python bindings for Oracle Berkeley DB
 Home-page: https://www.jcea.es/programacion/pybsddb.htm
 Author: Jesus Cea, Robin Dunn, Gregory P. Smith, Andrew Kuchling, Barry Warsaw
 Author-email: pybsddb@jcea.es
 License: 3-clause BSD License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Spanish
 Classifier: Operating System :: OS Independent
@@ -45,9 +44,7 @@
 
 `Homepage <https://www.jcea.es/programacion/pybsddb.htm>`__ --
 `Releases (changelog)
 <https://docs.jcea.es/berkeleydb/latest/changelog.html>`__ --
 `Documentation <https://docs.jcea.es/berkeleydb/latest/>`__ --
 `Mailing List <https://mailman.jcea.es/listinfo/pybsddb>`__ --
 `Donation <https://docs.jcea.es/berkeleydb/latest/donate.html>`__
-
-
```

### Comparing `berkeleydb-18.1.5/README.txt` & `berkeleydb-18.1.6/README.txt`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/TODO.txt` & `berkeleydb-18.1.6/TODO.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+- 20230410: RECNO databases should accept strings, not only bytes.
+
+- 20230410: Cursors should support iterator protocol.
+
+- 20230410: In currently supported Python releases, we always have threads
+  available.
+
+- 20230410: Encoding and decoding in "dbtables". "__next__", "getattr(...,
+  'next')" and  "bytes(x, 'ascii')" or "bytes(x, 'iso...')". How to be dbtables
+  compatible but being all binary now?
+
+- 20221030: Implement PEP 489 – Multi-phase extension module initialization:
+  https://peps.python.org/pep-0489/
+
 - 20220121: Rewrite all the test suite discovery and test driver.
 
 - 20210615: Add annotated types to the API.
 
 - 20210527: The legacy "bsddb3" library should be upgraded to search for
   new Berkeley DB libraries and raise an error pointing to this project.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `berkeleydb-18.1.5/TODO.txt.old` & `berkeleydb-18.1.6/TODO.txt.old`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/berkeleydb.egg-info/PKG-INFO` & `berkeleydb-18.1.6/berkeleydb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: berkeleydb
-Version: 18.1.5
+Version: 18.1.6
 Summary: Python bindings for Oracle Berkeley DB
 Home-page: https://www.jcea.es/programacion/pybsddb.htm
 Author: Jesus Cea, Robin Dunn, Gregory P. Smith, Andrew Kuchling, Barry Warsaw
 Author-email: pybsddb@jcea.es
 License: 3-clause BSD License
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Spanish
 Classifier: Operating System :: OS Independent
@@ -45,9 +44,7 @@
 
 `Homepage <https://www.jcea.es/programacion/pybsddb.htm>`__ --
 `Releases (changelog)
 <https://docs.jcea.es/berkeleydb/latest/changelog.html>`__ --
 `Documentation <https://docs.jcea.es/berkeleydb/latest/>`__ --
 `Mailing List <https://mailman.jcea.es/listinfo/pybsddb>`__ --
 `Donation <https://docs.jcea.es/berkeleydb/latest/donate.html>`__
-
-
```

### Comparing `berkeleydb-18.1.5/berkeleydb.egg-info/SOURCES.txt` & `berkeleydb-18.1.6/berkeleydb.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -59,23 +59,20 @@
 docs/html/images/bitcoin.png
 docs/html/static/alabaster.css
 docs/html/static/basic.css
 docs/html/static/custom.css
 docs/html/static/doctools.js
 docs/html/static/documentation_options.js
 docs/html/static/file.png
-docs/html/static/jquery-3.5.1.js
-docs/html/static/jquery.js
 docs/html/static/language_data.js
 docs/html/static/minus.png
 docs/html/static/plus.png
 docs/html/static/pygments.css
 docs/html/static/searchtools.js
-docs/html/static/underscore-1.13.1.js
-docs/html/static/underscore.js
+docs/html/static/sphinx_highlight.js
 src/Module/berkeleydb.c
 src/Module/berkeleydb.h
 src/berkeleydb/__init__.py
 src/berkeleydb/db.py
 src/berkeleydb/dbobj.py
 src/berkeleydb/dbrecio.py
 src/berkeleydb/dbshelve.py
```

### Comparing `berkeleydb-18.1.5/docs/Makefile` & `berkeleydb-18.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/bitcoin.png` & `berkeleydb-18.1.6/docs/bitcoin.png`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/changelog-bsddb3.rst` & `berkeleydb-18.1.6/docs/changelog-bsddb3.rst`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     compatibility with those versions, you can keep using old
     releases of these bindings.
   * Drop support for Berkeley DB 4.3, 4.4, 4.5, 4.6. If you need
     compatibility with those versions, you can keep using old
     releases of these bindings.
   * From now on, our support reference is Red Hat Enterprise Linux 6.
   * Drop modules attributes "cvsid".
-  * Drop (hidden) $Id: changelog-bsddb3.rst,v 2a174b277731 2020/12/11 01:35:38 jcea $ keyword in the documentation.
+  * Drop (hidden) $Id$ keyword in the documentation.
 
 6.0.1:
 ------
   * Clarification of license. Thanks to
     Jan Staněk <jstanek@redhat.com> for bringing this issue up.
     This work is now explicitly licensed under 3-clause BSD license.
   * Fixed a long standing bug (August 2008, rev 9fd52748fa59)
```

### Comparing `berkeleydb-18.1.5/docs/changelog.rst` & `berkeleydb-18.1.6/docs/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 Changelog
 =========
 
-18.1.6 -:
----------
+18.1.7
+------
 
-  - x
+  - X.
+
+18.1.6 - 2023-05-10:
+--------------------
+
+  - Initial implementation of PEP 489 – Multi-phase extension
+    module initialization: https://peps.python.org/pep-0489/.
+
+  - Update "setuptools" built-time dependency to version
+    ">=65.5.0". A "pip" modern enough will automatically take care
+    of this.
+
+  - We must be sure we are testing the correct library. Previously
+    we could be testing the installed library instead of
+    development code.
+
+  - Python 3.12 added to the full test matrix.
+
+  - Experimental Python 3.12 support. Tested under 3.12.0a7.
 
 18.1.5 - 2022-01-21:
 --------------------
 
   - **WARNING - BREAKING CHANGE:** Drop support for Python 3.6.
 
     This breaking change should usually require a major and/or minor
```

### Comparing `berkeleydb-18.1.5/docs/conf.py` & `berkeleydb-18.1.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # The contents of this file are pickled, so don't put values in the namespace
 # that aren't pickleable (module imports are okay, they're removed automatically).
 
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
@@ -54,22 +54,22 @@
         "oracle":
             ("https://docs.oracle.com/database/bdb181/html/%s",
             None),
         }
 
 # General substitutions.
 project = 'BerkeleyDB'
-copyright = '2008-2022 Jesús Cea Avión'
+copyright = '2008-2023 Jesús Cea Avión'
 
 # The default replacements for |version| and |release|.
 #
 # The short X.Y version.
-version = '18.1.5'
+version = '18.1.6'
 # The full version, including alpha/beta/rc tags.
-release = '18.1.5'
+release = '18.1.6'
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 today = ''
 # Else, today_fmt is used as the format for a strftime call.
 today_fmt = '%B %d, %Y'
```

### Comparing `berkeleydb-18.1.5/docs/db.rst` & `berkeleydb-18.1.6/docs/db.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/dbcursor.rst` & `berkeleydb-18.1.6/docs/dbcursor.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/dbenv.rst` & `berkeleydb-18.1.6/docs/dbenv.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/dblogcursor.rst` & `berkeleydb-18.1.6/docs/dblogcursor.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/dbsequence.rst` & `berkeleydb-18.1.6/docs/dbsequence.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/dbsite.rst` & `berkeleydb-18.1.6/docs/dbsite.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/dbtxn.rst` & `berkeleydb-18.1.6/docs/dbtxn.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/donate.rst` & `berkeleydb-18.1.6/docs/donate.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/history.rst` & `berkeleydb-18.1.6/docs/history.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/html/changelog-bsddb3.html` & `berkeleydb-18.1.6/docs/html/changelog-bsddb3.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Changelog of legacy “bsddb3” project &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>Changelog of legacy “bsddb3” project &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="LICENSE" href="license.html" />
     <link rel="prev" title="Changelog" href="changelog.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,25 +28,25 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="changelog-of-legacy-bsddb3-project">
-<h1>Changelog of legacy “bsddb3” project<a class="headerlink" href="#changelog-of-legacy-bsddb3-project" title="Permalink to this headline">¶</a></h1>
+<h1>Changelog of legacy “bsddb3” project<a class="headerlink" href="#changelog-of-legacy-bsddb3-project" title="Permalink to this heading">¶</a></h1>
 <section id="id1">
-<h2>6.2.9 - 2020-11-26:<a class="headerlink" href="#id1" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.9 - 2020-11-26:<a class="headerlink" href="#id1" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>For some reason, 6.2.8 release was incomplete. Let’s try again.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id2">
-<h2>6.2.8 - 2020-11-20:<a class="headerlink" href="#id2" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.8 - 2020-11-20:<a class="headerlink" href="#id2" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>In Python 3.9, “find_unused_port” has been moved to
 “test.support.socket_helper”. Reported by Michał Górny.</p></li>
 <li><p>If we use “set_get_returns_none()” in the environment,
 the value could not be correctly inherited by the child
 databases. Reported by Patrick Laimbock and modern GCC
@@ -56,98 +54,98 @@
 <li><p>If you install this library under Python 3 &gt;= 3.6, let
 you know this is a legacy library and urgess you to
 migrate to “berkeleydb” library.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id3">
-<h2>6.2.7:<a class="headerlink" href="#id3" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.7:<a class="headerlink" href="#id3" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Update copyright notices.</p></li>
 <li><p>https links.</p></li>
 <li><p>Fix Python 3 deprecation warning.
 Notified by Arthur Gautier.</p></li>
 <li><p>Fix compilation Python 3.8 deprecation warnings.</p></li>
 <li><p>Fix compilation Python 3.9 deprecation warnings.</p></li>
 <li><p>Python 3.8 and 3.9 are explicitly supported.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id4">
-<h2>6.2.6:<a class="headerlink" href="#id4" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.6:<a class="headerlink" href="#id4" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Correctly detect Berkeley DB when installed via Homebrew on Mac OS X.
 Patch by Matthew Peveler.</p></li>
 <li><p>Python 3.6 and 3.7 are explicitly supported.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id5">
-<h2>6.2.5:<a class="headerlink" href="#id5" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.5:<a class="headerlink" href="#id5" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>We should be able to install inside a PYPY virtualenv.
 Reported by Zhihao Yuan.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id6">
-<h2>6.2.4:<a class="headerlink" href="#id6" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.4:<a class="headerlink" href="#id6" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>More complete fix for pkgsrc.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id7">
-<h2>6.2.3:<a class="headerlink" href="#id7" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.3:<a class="headerlink" href="#id7" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Update copyright notices.</p></li>
 <li><p>Solve a conflict between different installations of Berkeley DB
 on some pkgsrc configurations.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id8">
-<h2>6.2.2:<a class="headerlink" href="#id8" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.2:<a class="headerlink" href="#id8" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Correctly detect Berkeley DB installations in SmartOS native zones.</p></li>
 <li><p>“Probably” (not tested) correctly detect Berkeley DB in pkgsrc systems.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id9">
-<h2>6.2.1:<a class="headerlink" href="#id9" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.1:<a class="headerlink" href="#id9" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Correctly detect Berkeley DB installations in modern 64 bits Debians.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id10">
-<h2>6.2.0:<a class="headerlink" href="#id10" title="Permalink to this headline">¶</a></h2>
+<h2>6.2.0:<a class="headerlink" href="#id10" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support Berkeley DB 6.2.x.</p></li>
 <li><p>Declare Python 3.5 support for PyPI.</p></li>
 <li><p>Drop support for Python 3.2. If you need
 compatibility with that version, you can keep using
 old releases of these bindings.</p></li>
 <li><p>Drop support for Berkeley DB 5.0, 5.2 and 6.0. If you need
 compatibility with those versions, you can keep using old
 releases of these bindings.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id11">
-<h2>6.1.1:<a class="headerlink" href="#id11" title="Permalink to this headline">¶</a></h2>
+<h2>6.1.1:<a class="headerlink" href="#id11" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Compatibility with Python 3.5.</p></li>
 <li><p>Code cleanup after dropping Python 2.4/2.5 support.</p></li>
 <li><p>PGP key changed.</p></li>
 <li><p>Support for DB_FORCESYNCENV flag in “DB_ENV.close()”.</p></li>
 <li><p>Support for DB_LOG_NOSYNC flag in “DB_ENV.log_set_config()”.</p></li>
@@ -156,33 +154,33 @@
 “DB.compact()” method call.</p></li>
 <li><p>Solve a compilation warning when compiling the bindings for
 Python 3.5 and Berkeley DB 4.8, 5.0 or 5.1.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id12">
-<h2>6.1.0:<a class="headerlink" href="#id12" title="Permalink to this headline">¶</a></h2>
+<h2>6.1.0:<a class="headerlink" href="#id12" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support Berkeley DB 6.1.x.</p></li>
 <li><p>Solve a ResourceWarning when compiling.</p></li>
 <li><p>Drop support for Python 2.4, 2.5 and 3.1. If you need
 compatibility with those versions, you can keep using old
 releases of these bindings.</p></li>
 <li><p>Drop support for Berkeley DB 4.3, 4.4, 4.5, 4.6. If you need
 compatibility with those versions, you can keep using old
 releases of these bindings.</p></li>
 <li><p>From now on, our support reference is Red Hat Enterprise Linux 6.</p></li>
 <li><p>Drop modules attributes “cvsid”.</p></li>
-<li><p>Drop (hidden) $Id: changelog-bsddb3.rst,v 2a174b277731 2020/12/11 01:35:38 jcea $ keyword in the documentation.</p></li>
+<li><p>Drop (hidden) $Id$ keyword in the documentation.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id13">
-<h2>6.0.1:<a class="headerlink" href="#id13" title="Permalink to this headline">¶</a></h2>
+<h2>6.0.1:<a class="headerlink" href="#id13" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul>
 <li><p>Clarification of license. Thanks to
 Jan Staněk &lt;<a class="reference external" href="mailto:jstanek&#37;&#52;&#48;redhat&#46;com">jstanek<span>&#64;</span>redhat<span>&#46;</span>com</a>&gt; for bringing this issue up.
 This work is now explicitly licensed under 3-clause BSD license.</p></li>
 <li><p>Fixed a long standing bug (August 2008, rev 9fd52748fa59)
 on “dbtables.py”. Notified by Maxime Labelle.</p></li>
@@ -204,15 +202,15 @@
 <a class="reference external" href="http://lists.debian.org/debian-legal/2013/07/">http://lists.debian.org/debian-legal/2013/07/</a></p>
 </div></blockquote>
 </li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id14">
-<h2>6.0.0:<a class="headerlink" href="#id14" title="Permalink to this headline">¶</a></h2>
+<h2>6.0.0:<a class="headerlink" href="#id14" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support Berkeley DB 6.0.x.</p></li>
 <li><p>HEADS UP: If you are using “bsddb3._bsddb” in your code,
 for example for exceptions, change it to “bsddb3._db”.</p></li>
 <li><p>Print test working directory when running the testsuite.
 You can control it using “TMPDIR” environment variable.
@@ -231,15 +229,15 @@
 anymore, and the version in Python 2.6/2.7 is being
 maintained separately.</p></li>
 <li><p>Improvements to documentation generation.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id15">
-<h2>5.3.0:<a class="headerlink" href="#id15" title="Permalink to this headline">¶</a></h2>
+<h2>5.3.0:<a class="headerlink" href="#id15" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul>
 <li><p>Support Berkeley DB 5.3.x.</p></li>
 <li><p>Drop support for Berkeley DB 4.2 and Python 2.3. Our reference
 is Red Hat Enterprise Linux 5, until march 2014.
 After that, RHEL6 has Python 2.6 and BDB 4.7.
 * According to <a class="reference external" href="http://superuser.com/questions/189931/python-and-berkeley-db-versions-in-redhat-enterprise-linux-3-4-5-and-upcoming-6">http://superuser.com/questions/189931/python-and-berkeley-db-versions-in-redhat-enterprise-linux-3-4-5-and-upcoming-6</a> :</p>
@@ -266,15 +264,15 @@
 in 20110929.</p></li>
 <li><p>When doing the full matrix test for a release, stop the verification
 if any test failed.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id16">
-<h2>5.2.0:<a class="headerlink" href="#id16" title="Permalink to this headline">¶</a></h2>
+<h2>5.2.0:<a class="headerlink" href="#id16" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support for Berkeley DB 5.2.</p></li>
 <li><p>Support for the newly available replication manager events:
 DB_EVENT_REP_SITE_ADDED, DB_EVENT_REP_SITE_REMOVED,
 DB_EVENT_REP_LOCAL_SITE_REMOVED, DB_EVENT_REP_CONNECT_BROKEN,
 DB_EVENT_REP_CONNECT_ESTD, DB_EVENT_REP_CONNECT_TRY_FAILED,
@@ -286,15 +284,15 @@
 DB_MEM_LOCK, DB_MEM_LOCKOBJECT, DB_MEM_LOCKER, DB_MEM_LOGID,
 DB_MEM_TRANSACTION, DB_MEM_THREAD.</p></li>
 <li><p>Add “bytes” to “DBEnv_memp_stat()”. Original patch from Garrett Cooper.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id17">
-<h2>5.1.2:<a class="headerlink" href="#id17" title="Permalink to this headline">¶</a></h2>
+<h2>5.1.2:<a class="headerlink" href="#id17" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>5.1.1 install fails if the bsddb in the standard library is not installed,
 under Python 2.7. Reported by Arfrever Frehtes Taifersar Arahesis.</p></li>
 <li><p>Since 5.0.0, we can’t find 4.x libraries unless we specify a
 “–berkeley-db=/path/to/bsddb” option. Reported by Wen Heping.</p></li>
 <li><p>Support “DB_ENV-&gt;get_open_flags()”, “DB_ENV-&gt;set_intermediate_dir_mode()”,
@@ -307,15 +305,15 @@
 <li><p>‘assertEquals()’ is deprecated in Python 3.2.</p></li>
 <li><p>‘assert_()’ is deprecated in Python 3.2.</p></li>
 <li><p>Solved ‘ResourceWarning’ under Python 3.2.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id18">
-<h2>5.1.1:<a class="headerlink" href="#id18" title="Permalink to this headline">¶</a></h2>
+<h2>5.1.1:<a class="headerlink" href="#id18" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Recent pre-releases of Python 3.2 issue ResourceWarnings about
 fileshandles deallocated without being closed first. Fix testsuite.</p></li>
 <li><p>Current “<em>.pyc” and “</em>.pyo” cleaning is not working in a PEP 3147
 world (“__pycache__”). I don’t think this code is actually
 necessary anymore. Deleted.</p></li>
@@ -337,15 +335,15 @@
 <li><p>Support for “DB_REP_CONF_INMEM”.</p></li>
 <li><p>Support for “DB_TIMEOUT “.</p></li>
 <li><p>Support for “DB_CURSOR_BULK”.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id19">
-<h2>5.1.0:<a class="headerlink" href="#id19" title="Permalink to this headline">¶</a></h2>
+<h2>5.1.0:<a class="headerlink" href="#id19" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul>
 <li><p>Support for Berkeley DB 5.1.</p></li>
 <li><p>Drop support for Berkeley DB 4.1. Our reference
 is Red Hat Enterprise Linux 4, until February 2012.
 After that, RHEL5 has Python 2.4 and BDB 4.3.
 * According to <a class="reference external" href="http://superuser.com/questions/189931/python-and-berkeley-db-versions-in-redhat-enterprise-linux-3-4-5-and-upcoming-6">http://superuser.com/questions/189931/python-and-berkeley-db-versions-in-redhat-enterprise-linux-3-4-5-and-upcoming-6</a> :</p>
@@ -367,15 +365,15 @@
 reference.</p></li>
 <li><p>Support for “DB-&gt;get_transactional()”.</p></li>
 <li><p>Support for “DB_REPMGR_ACKS_ALL_AVAILABLE”.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id20">
-<h2>5.0.0:<a class="headerlink" href="#id20" title="Permalink to this headline">¶</a></h2>
+<h2>5.0.0:<a class="headerlink" href="#id20" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support for Berkeley DB 5.0.</p></li>
 <li><p>Drop support for Python 3.0.</p></li>
 <li><p>Now you can use TMPDIR env variable to override default
 test directory (“/tmp”).</p></li>
 <li><p>Versioning of C API. If you use the code from C, please
@@ -398,15 +396,15 @@
 <li><p>Solve an “Overflow” warning in the testsuite running under python 2.3.</p></li>
 <li><p>When doing a complete full-matrix test, any warning will be considered
 an error.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id21">
-<h2>4.8.4:<a class="headerlink" href="#id21" title="Permalink to this headline">¶</a></h2>
+<h2>4.8.4:<a class="headerlink" href="#id21" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>When doing the full matrix testing with python &gt;=2.6, we
 activate the deprecation warnings (py3k).</p></li>
 <li><p>Split dependencies in the Replication testsuite.</p></li>
 <li><p>Help the Gargabe Collection freeing resources when the
 replication testsuite is completed.</p></li>
@@ -437,15 +435,15 @@
 <li><p>Solved last point, document that DBKeyEmptyError exception derives also
 from KeyError, just like DBNotFoundError exception.</p></li>
 <li><p>Update documentation to describe all exceptions provided by this module.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id22">
-<h2>4.8.3:<a class="headerlink" href="#id22" title="Permalink to this headline">¶</a></h2>
+<h2>4.8.3:<a class="headerlink" href="#id22" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>“bsddb.h” inclusion in PYPI is inconsistent. Solved.</p></li>
 <li><p>Support for “DB_ENV-&gt;mutex_stat()”, “DB_ENV-&gt;mutex_stat_print()”,
 “DB-&gt;stat_print()”, “DB_ENV-&gt;lock_stat_print()”,
 “DB_ENV-&gt;log_stat_print()”, “DB_ENV-&gt;stat_print()”,
 “DB_ENV-&gt;memp_stat()” and “DB_ENV-&gt;memp_stat_print()”.</p></li>
@@ -470,15 +468,15 @@
 will require a database scanning always, not only when there is any
 write. If you need an accurate and fast “len()”, the application must
 keep that information manually in a database register.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id23">
-<h2>4.8.2:<a class="headerlink" href="#id23" title="Permalink to this headline">¶</a></h2>
+<h2>4.8.2:<a class="headerlink" href="#id23" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support for “DB_OVERWRITE_DUP”, “DB_FOREIGN_ABORT”,
 “DB_FOREIGN_CASCADE”, “DB_FOREIGN_NULLIFY”, “DB_PRINTABLE”, “DB_INORDER”
 flags.</p></li>
 <li><p>Support for “DB_FOREIGN_CONFLICT” exception.</p></li>
 <li><p>Support for “DB_ENV-&gt;memp_trickle()”, “DB_ENV-&gt;memp_sync()”,
@@ -503,15 +501,15 @@
 <li><p>Unlock the Python GIL when doing “DB_ENV-&gt;db_home_get()”. This is
 slower, because the function is very fast so we add overhead, but it is
 called very infrequently and we do the change for consistency.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id24">
-<h2>4.8.1:<a class="headerlink" href="#id24" title="Permalink to this headline">¶</a></h2>
+<h2>4.8.1:<a class="headerlink" href="#id24" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support for “DB_ENV-&gt;mutex_set_align()” and
 “DB_ENV-&gt;mutex_get_align()”.</p></li>
 <li><p>Support for “DB_ENV-&gt;mutex_set_increment()” and
 “DB_ENV-&gt;mutex_get_increment()”.</p></li>
 <li><p>Support for “DB_ENV-&gt;mutex_set_tas_spins()” and
@@ -532,15 +530,15 @@
 that API via the new Capsule protocol (see “bsddb.h”).
 If you use the C API and upgrade to Python 3.2 and up,
 you must update the access code (see “bsddb.h”).</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id25">
-<h2>4.8.0:<a class="headerlink" href="#id25" title="Permalink to this headline">¶</a></h2>
+<h2>4.8.0:<a class="headerlink" href="#id25" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support for Berkeley DB 4.8.</p></li>
 <li><p>Compatibility with Python 3.1.</p></li>
 <li><p>The “DB_XIDDATASIZE” constant has been renamed
 to “DB_GID_SIZE”. Update your code!. If linked
 to BDB 4.8, only “DB_GID_SIZE” is defined.
@@ -564,15 +562,15 @@
 <li><p>In recno/queue databases, “set_re_delim()” and “set_re_pad()”
 require a byte instead of a unicode char, under Python3.</p></li>
 <li><p>Support for “DB_ENV-&gt;mutex_set_max()” and “DB_ENV-&gt;mutex_get_max()”.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id26">
-<h2>4.7.6:<a class="headerlink" href="#id26" title="Permalink to this headline">¶</a></h2>
+<h2>4.7.6:<a class="headerlink" href="#id26" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Compatibility with Python 3.0.1.</p></li>
 <li><p>Add support for “DB_ENV-&gt;stat()” and “DB_ENV-&gt;stat_print()”.</p></li>
 <li><p>Add support for “DB_ENV-&gt;rep_set_clockskew()” and
 “DB_ENV-&gt;rep_get_clockskew()”. The binding support
 for base replication is now complete.</p></li>
@@ -597,15 +595,15 @@
 <li><p>Add support for “DBCursor-&gt;set_priority()” and
 “DBCursor-&gt;get_priority()”. The binding support for cursors
 is now complete.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id27">
-<h2>4.7.5:<a class="headerlink" href="#id27" title="Permalink to this headline">¶</a></h2>
+<h2>4.7.5:<a class="headerlink" href="#id27" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Add support for “DB_EID_INVALID” and “DB_EID_BROADCAST” flags.</p></li>
 <li><p>Add support for “DB_SEQUENCE-&gt;stat_print()”. The binding
 support for “DB_SEQUENCE” is now complete.</p></li>
 <li><p>Add support for “DB_ENV-&gt;txn_stat_print()”.</p></li>
 <li><p>Add support for “DB_ENV-&gt;get_timeout()”.</p></li>
@@ -626,15 +624,15 @@
 “DB_REP_CONF_LEASE”, “DB_REPMGR_CONF_2SITE_STRICT”,
 “DB_REP_ANYWHERE”, “DB_REP_NOBUFFER” and “DB_REP_REREQUEST”
 flags.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id28">
-<h2>4.7.4:<a class="headerlink" href="#id28" title="Permalink to this headline">¶</a></h2>
+<h2>4.7.4:<a class="headerlink" href="#id28" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Under Python 3.0, “bsddb.db.DB_VERSION_STRING”,
 “bsddb.db.__version__” and “bsddb.db.cvsid” must
 return (unicode) strings instead of bytes. Solved.</p></li>
 <li><p>Use the new (20081018) trove classifiers in PyPI
 to identify Python supported versions.</p></li>
@@ -658,15 +656,15 @@
 support this function from Berkeley DB 4.7 and newer.
 We also support related flags “DB_FREELIST_ONLY”
 and “DB_FREE_SPACE”.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="python-2-6-release-first-release-with-python-3-0-support">
-<h2>4.7.3: (Python 2.6 release. First release with Python 3.0 support)<a class="headerlink" href="#python-2-6-release-first-release-with-python-3-0-support" title="Permalink to this headline">¶</a></h2>
+<h2>4.7.3: (Python 2.6 release. First release with Python 3.0 support)<a class="headerlink" href="#python-2-6-release-first-release-with-python-3-0-support" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>“private” is a keyword in C++.  (Duncan Grisby)</p></li>
 <li><p>setup.py should install “bsddb.h”.  (Duncan Grisby)</p></li>
 <li><p>“DB_remove” memory corruption &amp; crash.  (Duncan Grisby)</p></li>
 <li><p>Under Python 3.0, you can’t use string keys/values, but
 bytes ones. Print the right error message.</p></li>
@@ -688,15 +686,15 @@
 <li><p>Raising exceptions while doing a garbage collection
 will kill the interpreter.  (Victor Stinner)</p></li>
 <li><p>Crash in “DB.verify()”. Noted by solsTiCe d’Hiver.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id29">
-<h2>4.7.2:<a class="headerlink" href="#id29" title="Permalink to this headline">¶</a></h2>
+<h2>4.7.2:<a class="headerlink" href="#id29" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Solved a race condition in Replication Manager testcode.</p></li>
 <li><p>Changing any python code, automatically regenerates the
 Python3 version. The master version is Python2.</p></li>
 <li><p>Compatibility with Python 3.0.</p></li>
 <li><p>Solved a crash when DB handle creation fails.
@@ -716,15 +714,15 @@
 <li><p>Use ABC (Abstract Base Classes) under Python 2.6 and 3.0.</p></li>
 <li><p>Support for “relative imports”.</p></li>
 <li><p>Replication testcode behaves better in heavily loaded machines.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id30">
-<h2>4.7.1:<a class="headerlink" href="#id30" title="Permalink to this headline">¶</a></h2>
+<h2>4.7.1:<a class="headerlink" href="#id30" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Workaround a problem with un-initialized threads with the
 replication callback.</p></li>
 <li><p>Export “DBRepUnavailError” exception.</p></li>
 <li><p>Get rid of Berkeley DB 3.3 support. Rationale:
 <a class="reference external" href="http://mailman.jcea.es/pipermail/pybsddb/2008-March/000019.html">http://mailman.jcea.es/pipermail/pybsddb/2008-March/000019.html</a></p></li>
@@ -743,30 +741,30 @@
 <li><p>Support more base replication calls:  “DB_ENV-&gt;rep_elect”,
 “DB_ENV-&gt;rep_set_transport” and “DB_ENV-&gt;rep_process_message”.
 Support also related flags.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id31">
-<h2>4.7.0:<a class="headerlink" href="#id31" title="Permalink to this headline">¶</a></h2>
+<h2>4.7.0:<a class="headerlink" href="#id31" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support for Berkeley DB 4.7.</p></li>
 <li><p>Support “DB_ENV-&gt;log_set_config”, and related flags.</p></li>
 <li><p>Complete the Berkeley DB Replication Manager support:
 “DB_ENV-&gt;repmgr_site_list” and related flags.
 “DB_ENV-&gt;repmgr_stat”, “DB_ENV-&gt;repmgr_stat_print” and related flags.</p></li>
 <li><p>Solved an old crash when building with debug python. (Neal Norwitz)</p></li>
 <li><p>Extend the testsuite driver to check also against Python 2.6 (a3).</p></li>
 <li><p>Support for RPC client service.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id32">
-<h2>4.6.4:<a class="headerlink" href="#id32" title="Permalink to this headline">¶</a></h2>
+<h2>4.6.4:<a class="headerlink" href="#id32" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Basic support for Berkeley DB Replication Manager.</p></li>
 <li><p>Support for a few replication calls, for benefice of Berkeley DB
 Replication Manager: “DB_ENV-&gt;rep_set_priority”,
 “DB_ENV-&gt;rep_get_priority”, “DB_ENV-&gt;rep_set_nsites”,
 “DB_ENV-&gt;rep_get_nsites”, “DB_ENV-&gt;rep_set_timeout”,
@@ -781,15 +779,15 @@
 threaded ConcurrentDataStore, threaded simple locks, threaded
 transactions.</p></li>
 <li><p>New exported flags: “DB_LOCK_EXPIRE” and “DB_LOCK_MAXWRITE”.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id33">
-<h2>4.6.3:<a class="headerlink" href="#id33" title="Permalink to this headline">¶</a></h2>
+<h2>4.6.3:<a class="headerlink" href="#id33" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Be sure all DBEnv/DB paths in the TestSuite are generated in a
 way compatible with launching the tests in multiple
 threads/processes.</p></li>
 <li><p>Move all the “assert” in the TestSuite to the version in the
 framework. This is very convenient, for example, to generate the
@@ -813,15 +811,15 @@
 the datatypes are 64 bit width in fact.</p></li>
 <li><p>Solve a compilation warning when including “bsddb.h”
 in other projects. (George Feinberg)</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id34">
-<h2>4.6.2:<a class="headerlink" href="#id34" title="Permalink to this headline">¶</a></h2>
+<h2>4.6.2:<a class="headerlink" href="#id34" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support for MVCC (MultiVersion Concurrency Control).</p></li>
 <li><p>Support for DB_DSYNC_LOG, DB_DSYNC_DB and DB_OVERWRITE flags.</p></li>
 <li><p>Move old documentation to ReST format. This is important for several
 reasons, notably to be able to integrate the documentation “as is”
 in python official docs (from Python 2.6).</p></li>
@@ -849,15 +847,15 @@
 <li><p>Documented the already available DBCursor methods: “pget” (several
 flavours).</p></li>
 <li><p>Completed documentation of DBCursor methods: “consume”, “join_item”.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="first-release-from-jesus-cea-avion">
-<h2>4.6.1: (first release from Jesús Cea Avión)<a class="headerlink" href="#first-release-from-jesus-cea-avion" title="Permalink to this headline">¶</a></h2>
+<h2>4.6.1: (first release from Jesús Cea Avión)<a class="headerlink" href="#first-release-from-jesus-cea-avion" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>‘egg’ (setuptools) support.</p></li>
 <li><p>Environments, database handles and cursors are
 maintained in a logical tree. Closing any element
 of the tree, implicitly closes its children.</p></li>
 <li><p>Transactions are managed in a logical tree. When
@@ -875,15 +873,15 @@
 opening the database in thread safe mode or not.
 In one case the lib gives “” and in the other
 it gives None.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id35">
-<h2>4.6.0:<a class="headerlink" href="#id35" title="Permalink to this headline">¶</a></h2>
+<h2>4.6.0:<a class="headerlink" href="#id35" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Adds support for compiling and linking with BerkeleyDB 4.6.21.</p></li>
 <li><p>Fixes a double free bug with DBCursor.get and friends.  Based on
 submitted pybsddb patch #1708868. (jjjhhhll)</p></li>
 <li><p>Adds a basic C API to the module so that other extensions or
 third party modules can access types directly. Based on pybsddb
@@ -901,255 +899,255 @@
 <li><p>Add the DBEnv.lock_id_free method.</p></li>
 <li><p>Removes any remnants of support for Python older than 2.1.</p></li>
 <li><p>Removes any remnants of support for BerkeleyDB 3.2.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id36">
-<h2>4.5.0:<a class="headerlink" href="#id36" title="Permalink to this headline">¶</a></h2>
+<h2>4.5.0:<a class="headerlink" href="#id36" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Adds supports for compiling and linking with BerkeleyDB 4.5</p></li>
 <li><p>Python Bug #1599782: Fix segfault on bsddb.db.DB().type() due to
 releasing the GIL when it shouldn’t.  (nnorowitz)</p></li>
 <li><p>Fixes a bug with bsddb.DB.stat where the flags and txn keyword
 arguments are transposed.</p></li>
 <li><p>change test cases to use tempfile.gettempdir()</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id37">
-<h2>4.4.5:<a class="headerlink" href="#id37" title="Permalink to this headline">¶</a></h2>
+<h2>4.4.5:<a class="headerlink" href="#id37" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>pybsddb Bug #1527939: bsddb module DBEnv dbremove and dbrename
 methods now allow their database parameter to be None as the
 sleepycat API allows.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id38">
-<h2>4.4.4:<a class="headerlink" href="#id38" title="Permalink to this headline">¶</a></h2>
+<h2>4.4.4:<a class="headerlink" href="#id38" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>fix DBCursor.pget() bug with keyword argument names when no data= is
 supplied [SF pybsddb bug #1477863]</p></li>
 <li><p>add support for DBSequence objects [patch #1466734]</p></li>
 <li><p>support DBEnv.log_stat() method on BerkeleyDB &gt;= 4.0 [patch #1494885]</p></li>
 <li><p>support DBEnv.lsn_reset() method on BerkeleyDB &gt;= 4.4 [patch #1494902]</p></li>
 <li><p>add DB_ARCH_REMOVE flag and fix DBEnv.log_archive() to accept it without
 potentially following an uninitialized pointer.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id39">
-<h2>4.4.3:<a class="headerlink" href="#id39" title="Permalink to this headline">¶</a></h2>
+<h2>4.4.3:<a class="headerlink" href="#id39" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>fix DBEnv.set_tx_timestamp to not crash on Win64 platforms (thomas.wouters)</p></li>
 <li><p>tons of memory leak fixes all over the code (thomas.wouters)</p></li>
 <li><p>fixes ability to unpickle DBError (and children) exceptions</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id40">
-<h2>4.4.2:<a class="headerlink" href="#id40" title="Permalink to this headline">¶</a></h2>
+<h2>4.4.2:<a class="headerlink" href="#id40" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Wrap the DBEnv.set_tx_timeout method</p></li>
 <li><p>fix problem when DBEnv deleted before Txn sf bug #1413192 (Neal Norwitz)</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id41">
-<h2>4.4.1:<a class="headerlink" href="#id41" title="Permalink to this headline">¶</a></h2>
+<h2>4.4.1:<a class="headerlink" href="#id41" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>sf.net patch 1407992 - fixes associate tests on BerkeleyDB 3.3 thru 4.1
 (contributed by Neal Norwitz)</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id42">
-<h2>4.4.0:<a class="headerlink" href="#id42" title="Permalink to this headline">¶</a></h2>
+<h2>4.4.0:<a class="headerlink" href="#id42" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Added support for compiling and linking with BerkeleyDB 4.4.20.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id43">
-<h2>4.3.3:<a class="headerlink" href="#id43" title="Permalink to this headline">¶</a></h2>
+<h2>4.3.3:<a class="headerlink" href="#id43" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>NOTICE: set_bt_compare() callback function arguments CHANGED to only
 require two arguments (left, right) rather than (db, left, right).</p></li>
 <li><p>DB.associate() would crash when a DBError occurred.  fixed.
 [pybsddb SF bug id 1215432].</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id44">
-<h2>4.3.2:<a class="headerlink" href="#id44" title="Permalink to this headline">¶</a></h2>
+<h2>4.3.2:<a class="headerlink" href="#id44" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>the has_key() method was not raising a DBError when a database error
 had occurred. [SF patch id 1212590]</p></li>
 <li><p>added a wrapper for the DBEnv.set_lg_regionmax method [SF patch id 1212590]</p></li>
 <li><p>DBKeyEmptyError now derives from KeyError just like DBNotFoundError.</p></li>
 <li><p>internally everywhere DB_NOTFOUND was checked for has been updated
 to also check for DB_KEYEMPTY.  This fixes the semantics of a couple
 operations on recno and queue databases to be more intuitive and results
 in less unexpected DBKeyEmptyError exceptions being raised.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id45">
-<h2>4.3.1:<a class="headerlink" href="#id45" title="Permalink to this headline">¶</a></h2>
+<h2>4.3.1:<a class="headerlink" href="#id45" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Added support for DB.set_bt_compare() method to use a user
 supplied python comparison function taking (db, left, right)
 args as the database’s B-Tree comparison function.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id46">
-<h2>4.3.0:<a class="headerlink" href="#id46" title="Permalink to this headline">¶</a></h2>
+<h2>4.3.0:<a class="headerlink" href="#id46" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Added support for building properly against BerkeleyDB 4.3.21.</p></li>
 <li><p>fixed bug introduced in 4.2.8 that prevent the module from
 compiling against BerkeleyDB 3.2 (which doesn’t support pget).</p></li>
 <li><p>setup.py was cleaned up a bit to search for and find the latest
 version of the correct combo of db.h and libdb.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id47">
-<h2>4.2.9:<a class="headerlink" href="#id47" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.9:<a class="headerlink" href="#id47" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>DB keys() values() and items() methods were ignoring their optional
 txn parameter.  This would lead to deadlocks in applications
 needing those to be transaction protected.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id48">
-<h2>4.2.8:<a class="headerlink" href="#id48" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.8:<a class="headerlink" href="#id48" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Adds support for DB and DBCursor pget methods.  Based on a patch
 submitted to the mailing list by Ian Ward &lt;<a class="reference external" href="mailto:ian&#37;&#52;&#48;arevco&#46;ca">ian<span>&#64;</span>arevco<span>&#46;</span>ca</a>&gt;</p></li>
 <li><p>Added weakref support to all bsddb.db objects.</p></li>
 <li><p>Make DBTxn objects automatically call abort() in their destructor if
 not yet finalized and raise a RuntimeWarning to that effect.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id49">
-<h2>4.2.7:<a class="headerlink" href="#id49" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.7:<a class="headerlink" href="#id49" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>fix an error with the legacy interface relying on the DB_TRUNCATE
 flag that changed behaviour to not work in a locking environment
 with BerkeleyDB 4.2.52.  [SF bug id 897820]</p></li>
 <li><p>fixed memory leaks in DB.get, DBC.set_range and potentially several
 other methods that would occur primarily when using queue | recno
 format databases with integer keys. [SF patch id 967763]</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id50">
-<h2>4.2.6:<a class="headerlink" href="#id50" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.6:<a class="headerlink" href="#id50" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>the DB.has_key method was not honoring its txn parameter to perform
 its lookup within the specified (optional) transaction.  fixed.
 [SF bug id 914019]</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id51">
-<h2>4.2.5:<a class="headerlink" href="#id51" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.5:<a class="headerlink" href="#id51" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Fixed a bug in the compatibility interface set_location() method
 where it would not properly search to the next nearest key when
 used on BTree databases.  [SF bug id 788421]</p></li>
 <li><p>Fixed a bug in the compatibility interface set_location() method
 where it could crash when looking up keys in a hash or recno
 format database due to an incorrect free().</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id52">
-<h2>4.2.4:<a class="headerlink" href="#id52" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.4:<a class="headerlink" href="#id52" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>changed DB and DBEnv set_get_returns_none() default from 1 to 2.</p></li>
 <li><p>cleaned up compatibility iterator interface.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id53">
-<h2>4.2.3:<a class="headerlink" href="#id53" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.3:<a class="headerlink" href="#id53" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>the legacy compatibility dict-like interface now support iterators
 and generators and allows multithreaded access to the database.</p></li>
 <li><p>fixed a tuple memory leak when raising “object has been closed”
 exceptions for DB, DBEnv and DBCursor objects.  I doubt much
 previous code triggered this.</p></li>
 <li><p>use of a closed DBCursor now raises a DBCursorClosedError exception
 subclass of DBError rather than a boring old DBError.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id54">
-<h2>4.2.2:<a class="headerlink" href="#id54" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.2:<a class="headerlink" href="#id54" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>added DBCursor.get_current_size() method to return the length in bytes
 of the value pointed to by the cursor without reading the actual data.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id55">
-<h2>4.2.1:<a class="headerlink" href="#id55" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.1:<a class="headerlink" href="#id55" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Standalone pybsddb builds now use a _pybsddb dynamic/shared library
 rather than _bsddb.  This allows for pybsddb to be built, installed
 and used on python &gt;= 2.3 which includes an older version of pybsddb
 as its bsddb library.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id56">
-<h2>4.2.0:<a class="headerlink" href="#id56" title="Permalink to this headline">¶</a></h2>
+<h2>4.2.0:<a class="headerlink" href="#id56" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Can now compile and link with BerkeleyDB 4.2.x (when its released).</p></li>
 <li><p>the legacy bsddb module supports the iterator interface on python 2.3.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="x">
-<h2>4.1.x:<a class="headerlink" href="#x" title="Permalink to this headline">¶</a></h2>
+<h2>4.1.x:<a class="headerlink" href="#x" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Support the DBEnv.set_shm_key() method.</p></li>
 <li><p>Fixed setup.py include/{db4,db3} header file searching (SF bug #789740).</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id57">
-<h2>4.1.6:<a class="headerlink" href="#id57" title="Permalink to this headline">¶</a></h2>
+<h2>4.1.6:<a class="headerlink" href="#id57" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Extended DB &amp; DBEnv set_get_returns_none functionality to take a
 “level” instead of a boolean flag.  The boolean 0 and 1 values still
 have the same effect.  A value of 2 extends the “return None instead
 of raising an exception” behaviour to the DBCursor set methods.
 This will become the default behaviour in pybsddb 4.2.</p></li>
@@ -1160,43 +1158,43 @@
 for join and join_item.</p></li>
 <li><p>Added the dbobj wrapper for DBEnv set_timeout method.</p></li>
 <li><p>Updated README.txt</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id58">
-<h2>4.1.5:<a class="headerlink" href="#id58" title="Permalink to this headline">¶</a></h2>
+<h2>4.1.5:<a class="headerlink" href="#id58" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Added the DBEnv.set_timeout method.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id59">
-<h2>4.1.4:<a class="headerlink" href="#id59" title="Permalink to this headline">¶</a></h2>
+<h2>4.1.4:<a class="headerlink" href="#id59" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>rebuilt the windows 4.1.3 package, the original package was corrupt due
 to bad ram on my build host.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id60">
-<h2>4.1.3 - 2003-02-02:<a class="headerlink" href="#id60" title="Permalink to this headline">¶</a></h2>
+<h2>4.1.3 - 2003-02-02:<a class="headerlink" href="#id60" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>code cleanup to use python 2.x features in .py files</p></li>
 <li><p>the standalone pybsddb distribution will install a module
 called bsddb3 while the module included with python &gt;= 2.3
 will be known as bsddb.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id61">
-<h2>4.1.2 - 2003-01-17:<a class="headerlink" href="#id61" title="Permalink to this headline">¶</a></h2>
+<h2>4.1.2 - 2003-01-17:<a class="headerlink" href="#id61" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Shared all .py and .c source with the Python project.</p></li>
 <li><p>Fixed DBTxn objects to raise an exception if they are used after
 the underlying DB_TXN handle becomes invalid. (rather than
 potentially causing a segfault)</p></li>
 <li><p>Fixed module to work when compiled against a python without thread
@@ -1205,25 +1203,25 @@
 has already been closed (fixes a segfault).</p></li>
 <li><p>Close DB objects when DB.open fails to prevent an exception about
 databases still being open when calling DBEnv.close.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id62">
-<h2>4.1.1 - 2002-12-20:<a class="headerlink" href="#id62" title="Permalink to this headline">¶</a></h2>
+<h2>4.1.1 - 2002-12-20:<a class="headerlink" href="#id62" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Fixed a memory leak when raising exceptions from the database
 library.  Debugged and fixed by Josh Hoyt &lt;<a class="reference external" href="mailto:josh&#37;&#52;&#48;janrain&#46;com">josh<span>&#64;</span>janrain<span>&#46;</span>com</a>&gt;.  Thanks!
 (sourceforge patch 656517)</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id63">
-<h2>4.1.0 - 2002-12-13:<a class="headerlink" href="#id63" title="Permalink to this headline">¶</a></h2>
+<h2>4.1.0 - 2002-12-13:<a class="headerlink" href="#id63" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Updated our version number to track the latest BerkeleyDB interface
 version that we support.</p></li>
 <li><p>Simplified the build and test process.  Now you should just be able
 to say “python setup.py build” and “python setup.py install”.  Also
 added a nice test.py harness.  Do “python test.py -h” for details.</p></li>
@@ -1231,52 +1229,52 @@
 eight patches issued by Sleepycat applied.</p></li>
 <li><p>REMINDER: BerkeleyDB 4.1 requires code changes if you use database
 transactions.  See the upgrade docs on <a class="reference external" href="http://www.sleepycat.com/">http://www.sleepycat.com/</a>.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id64">
-<h2>3.4.3 - 2002-10-18:<a class="headerlink" href="#id64" title="Permalink to this headline">¶</a></h2>
+<h2>3.4.3 - 2002-10-18:<a class="headerlink" href="#id64" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>added support for BerkeleyDB 4.1:  DB.open and DB.associate
 will now accept a txn keyword argument when using BerkeleyDB 4.1.
 DBEnv.dbremove, DBEnv.dbrename, DBEnv.set_encrypt and DB.set_encrypt
 methods have been exposed for 4.1.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id65">
-<h2>3.4.2 - 2002-08-14:<a class="headerlink" href="#id65" title="Permalink to this headline">¶</a></h2>
+<h2>3.4.2 - 2002-08-14:<a class="headerlink" href="#id65" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>dbtables.py: serious bug fix.  The Select, Modify and Delete methods could
 all act upon rows that did not match all of the conditions.  (bug # 590449)
 A test case was added.</p></li>
 <li><p>dbutils.py: updated DeadlockWrap</p></li>
 <li><p>test_threads.py: fixed to use dbutils.DeadlockWrap to catch and avoid
 DBLockDeadlockError exceptions during simple threading tests.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id66">
-<h2>3.4.1:<a class="headerlink" href="#id66" title="Permalink to this headline">¶</a></h2>
+<h2>3.4.1:<a class="headerlink" href="#id66" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>fixed typo cut and paste bugs in test_dbsimple.py and test_threads.py</p></li>
 <li><p>fixed bug with cursors where calling DBCursor.close() would cause
 the object’s destructor __del__() method to raise an exception when
 it was called by the gc.</p></li>
 <li><p>fixed a bug in associated callbacks that could cause a null pointer
 dereference when python threading had not yet been initialized.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="id67">
-<h2>3.4.0:<a class="headerlink" href="#id67" title="Permalink to this headline">¶</a></h2>
+<h2>3.4.0:<a class="headerlink" href="#id67" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>many bugfixes, its been a long while since a new package was created.</p></li>
 <li><p>ChangeLog started.</p></li>
 </ul>
 </div></blockquote>
 </section>
@@ -1402,32 +1400,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** Changelog of legacy âbsddb3â projectÂ¶ ******
 ***** 6.2.9 - 2020-11-26:Â¶ *****
          * For some reason, 6.2.8 release was incomplete. Letâs try
            again.
 
 ***** 6.2.8 - 2020-11-20:Â¶ *****
          * In Python 3.9, âfind_unused_portâ has been moved to
@@ -89,16 +88,15 @@
            releases of these bindings.
          * Drop support for Berkeley DB 4.3, 4.4, 4.5, 4.6. If you need
            compatibility with those versions, you can keep using old
            releases of these bindings.
          * From now on, our support reference is Red Hat Enterprise Linux
            6.
          * Drop modules attributes âcvsidâ.
-         * Drop (hidden) $Id: changelog-bsddb3.rst,v 2a174b277731 2020/12/
-           11 01:35:38 jcea $ keyword in the documentation.
+         * Drop (hidden) $Id$ keyword in the documentation.
 
 ***** 6.0.1:Â¶ *****
          * Clarification of license. Thanks to Jan StanÄk
            <jstanek@redhat.com> for bringing this issue up. This work is
            now explicitly licensed under 3-clause BSD license.
          * Fixed a long standing bug (August 2008, rev 9fd52748fa59) on
            âdbtables.pyâ. Notified by Maxime Labelle.
@@ -1059,8 +1057,8 @@
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: Changelog
           o Next: LICENSE
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/changelog.html` & `berkeleydb-18.1.6/docs/html/changelog.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Changelog &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>Changelog &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Changelog of legacy “bsddb3” project" href="changelog-bsddb3.html" />
     <link rel="prev" title="History" href="history.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,17 +28,34 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="changelog">
-<h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this headline">¶</a></h1>
+<h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this heading">¶</a></h1>
 <section id="id1">
-<h2>18.1.5 - 2022-01-21:<a class="headerlink" href="#id1" title="Permalink to this headline">¶</a></h2>
+<h2>18.1.6 - 2023-05-10:<a class="headerlink" href="#id1" title="Permalink to this heading">¶</a></h2>
+<blockquote>
+<div><ul class="simple">
+<li><p>Initial implementation of PEP 489 – Multi-phase extension
+module initialization: <a class="reference external" href="https://peps.python.org/pep-0489/">https://peps.python.org/pep-0489/</a>.</p></li>
+<li><p>Update “setuptools” built-time dependency to version
+“&gt;=65.5.0”. A “pip” modern enough will automatically take care
+of this.</p></li>
+<li><p>We must be sure we are testing the correct library. Previously
+we could be testing the installed library instead of
+development code.</p></li>
+<li><p>Python 3.12 added to the full test matrix.</p></li>
+<li><p>Experimental Python 3.12 support. Tested under 3.12.0a7.</p></li>
+</ul>
+</div></blockquote>
+</section>
+<section id="id2">
+<h2>18.1.5 - 2022-01-21:<a class="headerlink" href="#id2" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul>
 <li><p><strong>WARNING - BREAKING CHANGE:</strong> Drop support for Python 3.6.</p>
 <p>This breaking change should usually require a major and/or minor
 number update. Since <code class="docutils literal notranslate"><span class="pre">berkeleydb</span></code> traditional numbering is
 related to the higher Oracle Berkeley DB supported, I would
 usually wait until Oracle releases a new version to upgrade my
@@ -59,27 +74,27 @@
 <code class="docutils literal notranslate"><span class="pre">unittest.makeSuite()</span></code> and it will be deleted in Python
 3.13. We migrate the tests to
 <code class="docutils literal notranslate"><span class="pre">unittest.TestLoader.loadTestsFromTestCase()</span></code>.</p></li>
 <li><p>Experimental Python 3.11 support. Tested in 3.11.0a4.</p></li>
 </ul>
 </div></blockquote>
 </section>
-<section id="id2">
-<h2>18.1.4 - 2021-05-19:<a class="headerlink" href="#id2" title="Permalink to this headline">¶</a></h2>
+<section id="id3">
+<h2>18.1.4 - 2021-05-19:<a class="headerlink" href="#id3" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul>
 <li><p>If your “pip” is modern enough, “setuptools” is automatically
 added as a built-time dependency.</p>
 <p>If not, you <strong>MUST</strong> install “setuptools” package first.</p>
 </li>
 </ul>
 </div></blockquote>
 </section>
-<section id="id3">
-<h2>18.1.3 - 2021-05-19:<a class="headerlink" href="#id3" title="Permalink to this headline">¶</a></h2>
+<section id="id4">
+<h2>18.1.3 - 2021-05-19:<a class="headerlink" href="#id4" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul>
 <li><p>Docs in <a class="reference external" href="https://docs.jcea.es/berkeleydb/">https://docs.jcea.es/berkeleydb/</a>.</p></li>
 <li><p><code class="docutils literal notranslate"><span class="pre">make</span> <span class="pre">publish</span></code> build and publish the documentation online.</p></li>
 <li><p>Python 3.10 deprecated <code class="docutils literal notranslate"><span class="pre">distutils</span></code>. <code class="docutils literal notranslate"><span class="pre">setuptools</span></code> is now an
 installation dependency.</p></li>
 <li><p><code class="docutils literal notranslate"><span class="pre">make</span> <span class="pre">dist</span></code> will generate the HTML documentation and will
@@ -124,16 +139,16 @@
 available if you are using Oracle Berkeley DB 5.3 or newer.
 These methods allow you to do hot backups without needing to
 follow a careful procedure, and they can be incremental.</p></li>
 <li><p>Changelog moved to Sphinx documentation.</p></li>
 </ul>
 </div></blockquote>
 </section>
-<section id="id4">
-<h2>18.1.2 - 2020-12-07:<a class="headerlink" href="#id4" title="Permalink to this headline">¶</a></h2>
+<section id="id5">
+<h2>18.1.2 - 2020-12-07:<a class="headerlink" href="#id5" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p>Releases 18.1.0 and 18.1.1 were incomplete. Thanks to Mihai.i
 for reporting.</p></li>
 <li><p>Export exception <code class="docutils literal notranslate"><span class="pre">DBMetaChksumFail</span></code> (from error
 <code class="docutils literal notranslate"><span class="pre">DB_META_CHKSUM_FAIL</span></code>) if running Oracle Berkeley DB version
 6.2 or newer.</p></li>
@@ -172,16 +187,16 @@
 Berkeley DB 6.2 or newer).</p></li>
 <li><p>Queue access method: Added <code class="docutils literal notranslate"><span class="pre">metaflags</span></code> (always).</p></li>
 </ul>
 </li>
 </ul>
 </div></blockquote>
 </section>
-<section id="id5">
-<h2>18.1.1 - 2020-12-01:<a class="headerlink" href="#id5" title="Permalink to this headline">¶</a></h2>
+<section id="id6">
+<h2>18.1.1 - 2020-12-01:<a class="headerlink" href="#id6" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul>
 <li><p>If you try to install this library in an unsupported Python
 environment, instruct the user about how to install legacy
 <code class="docutils literal notranslate"><span class="pre">bsddb3</span></code> library.</p></li>
 <li><p>Expose <code class="docutils literal notranslate"><span class="pre">DBSite</span></code> object in the C API. Increase C API version.</p></li>
 <li><p><strong>WARNING - BREAKING CHANGE:</strong> Ancient release 4.2.8 added
@@ -226,26 +241,26 @@
 defined, test will run in <code class="docutils literal notranslate"><span class="pre">/tmp/ram/</span></code> if exists and in
 <code class="docutils literal notranslate"><span class="pre">/tmp</span></code> if <code class="docutils literal notranslate"><span class="pre">/tmp/ram/</span></code> doesn’t exists or it is not a
 directory. The idea is that <code class="docutils literal notranslate"><span class="pre">/tmp/ram/</span></code> is a ramdisk and the
 test will run faster.</p></li>
 </ul>
 </div></blockquote>
 </section>
-<section id="id6">
-<h2>18.1.0 - 2020-11-12:<a class="headerlink" href="#id6" title="Permalink to this headline">¶</a></h2>
+<section id="id7">
+<h2>18.1.0 - 2020-11-12:<a class="headerlink" href="#id7" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul class="simple">
 <li><p><code class="docutils literal notranslate"><span class="pre">bsddb</span></code> name is reserved in PYPI, so we rename the project
 to <code class="docutils literal notranslate"><span class="pre">berkeleydb</span></code>. This has been a long trip:
 <a class="reference external" href="http://mailman.jcea.es/pipermail/pybsddb/2008-March/000019.html">http://mailman.jcea.es/pipermail/pybsddb/2008-March/000019.html</a></p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="pre">
-<h2>18.1.0-pre:<a class="headerlink" href="#pre" title="Permalink to this headline">¶</a></h2>
+<h2>18.1.0-pre:<a class="headerlink" href="#pre" title="Permalink to this heading">¶</a></h2>
 <blockquote>
 <div><ul>
 <li><p>Support Oracle Berkeley DB 18.1.x.</p></li>
 <li><p>Drop support for Oracle Berkeley DB 4.7, 5.1 and 6.1.</p></li>
 <li><p>Drop support for Python 2.6, 2.7, 3.3, 3.4 and 3.5.</p></li>
 <li><p>The library name is migrated from <code class="docutils literal notranslate"><span class="pre">bsddb3</span></code> to <code class="docutils literal notranslate"><span class="pre">bsddb</span></code>. Reasons:</p>
 <ul>
@@ -403,20 +418,21 @@
 <li class="toctree-l1"><a class="reference internal" href="dblogcursor.html">DBLogCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbtxn.html">DBTxn</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblock.html">DBLock</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsequence.html">DBSequence</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsite.html">DBSite</a></li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Changelog</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#id1">18.1.5 - 2022-01-21:</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id2">18.1.4 - 2021-05-19:</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id3">18.1.3 - 2021-05-19:</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id4">18.1.2 - 2020-12-07:</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id5">18.1.1 - 2020-12-01:</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id6">18.1.0 - 2020-11-12:</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id1">18.1.6 - 2023-05-10:</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id2">18.1.5 - 2022-01-21:</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id3">18.1.4 - 2021-05-19:</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id4">18.1.3 - 2021-05-19:</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id5">18.1.2 - 2020-12-07:</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id6">18.1.1 - 2020-12-01:</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id7">18.1.0 - 2020-11-12:</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#pre">18.1.0-pre:</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="changelog-bsddb3.html">Changelog of legacy “bsddb3” project</a></li>
 <li class="toctree-l1"><a class="reference internal" href="license.html">LICENSE</a></li>
 <li class="toctree-l1"><a class="reference internal" href="donate.html">DONATE!</a></li>
 </ul>
@@ -435,32 +451,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,16 +2,27 @@
 
 
 
 
 
 
 
-
 ****** ChangelogÂ¶ ******
+***** 18.1.6 - 2023-05-10:Â¶ *****
+         * Initial implementation of PEP 489 â Multi-phase extension
+           module initialization: https://peps.python.org/pep-0489/.
+         * Update âsetuptoolsâ built-time dependency to version
+           â>=65.5.0â. A âpipâ modern enough will automatically
+           take care of this.
+         * We must be sure we are testing the correct library. Previously
+           we could be testing the installed library instead of
+           development code.
+         * Python 3.12 added to the full test matrix.
+         * Experimental Python 3.12 support. Tested under 3.12.0a7.
+
 ***** 18.1.5 - 2022-01-21:Â¶ *****
          * WARNING - BREAKING CHANGE: Drop support for Python 3.6.
            This breaking change should usually require a major and/or
            minor number update. Since berkeleydb traditional numbering is
            related to the higher Oracle Berkeley DB supported, I would
            usually wait until Oracle releases a new version to upgrade my
            own version and deprecate old Python support at the same time.
@@ -315,14 +326,15 @@
     * DBLogCursor
     * DBTxn
     * DBLock
     * DBSequence
     * DBSite
     * History
     * Changelog
+          o 18.1.6_-_2023-05-10:
           o 18.1.5_-_2022-01-21:
           o 18.1.4_-_2021-05-19:
           o 18.1.3_-_2021-05-19:
           o 18.1.2_-_2020-12-07:
           o 18.1.1_-_2020-12-01:
           o 18.1.0_-_2020-11-12:
           o 18.1.0-pre:
@@ -331,8 +343,8 @@
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: History
           o Next: Changelog_of_legacy_âbsddb3â_project
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/db.html` & `berkeleydb-18.1.6/docs/html/db.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DB &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DB &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DBCursor" href="dbcursor.html" />
     <link rel="prev" title="DBEnv" href="dbenv.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,20 +28,20 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="db">
-<h1>DB<a class="headerlink" href="#db" title="Permalink to this headline">¶</a></h1>
+<h1>DB<a class="headerlink" href="#db" title="Permalink to this heading">¶</a></h1>
 <p>Read <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/programmer_reference/index.html">Oracle documentation</a>
 for better understanding.</p>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/db.html">More info…</a></p>
 <section id="db-methods">
-<h2>DB Methods<a class="headerlink" href="#db-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DB Methods<a class="headerlink" href="#db-methods" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="DB">
 <span class="sig-name descname"><span class="pre">DB</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">dbEnv</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#DB" title="Permalink to this definition">¶</a></dt>
 <dd><p>Constructor.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcreate.html">More info…</a></p>
 </dd></dl>
 
@@ -80,18 +78,14 @@
 <dt class="sig sig-object py" id="compact">
 <span class="sig-name descname"><span class="pre">compact</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">stop</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">compact_fillpercent</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">compact_pages</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">compact_timeout</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#compact" title="Permalink to this definition">¶</a></dt>
 <dd><p>Compacts Btree and Recno access method databases, and optionally
 returns unused Btree, Hash or Recno database pages to the underlying
 filesystem.</p>
 <p>The method returns a dictionary with the following content:</p>
 <table class="docutils align-default">
-<colgroup>
-<col style="width: 28%" />
-<col style="width: 72%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>deadlock</p></td>
 <td><p>If no txnid parameter was specified, the
 number of deadlocks which occurred</p></td>
 </tr>
 <tr class="row-even"><td><p>pages_examine</p></td>
 <td><p>The number of database pages reviewed
@@ -122,24 +116,24 @@
 </tbody>
 </table>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcompact.html">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="consume">
-<span class="sig-name descname"><span class="pre">consume</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#consume" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">consume</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#consume" title="Permalink to this definition">¶</a></dt>
 <dd><p>For a database with the Queue access method, returns the record
 number and data from the first available record and deletes it from
 the queue.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbget.html#dbget_DB_CONSUME">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="consume_wait">
-<span class="sig-name descname"><span class="pre">consume_wait</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#consume_wait" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">consume_wait</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#consume_wait" title="Permalink to this definition">¶</a></dt>
 <dd><p>For a database with the Queue access method, returns the record
 number and data from the first available record and deletes it from
 the queue. If the Queue database is empty, the thread of control
 will wait until there is data in the queue before returning.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbget.html#dbget_DB_CONSUME_WAIT">More info…</a></p>
 </dd></dl>
 
@@ -172,28 +166,28 @@
 <span class="sig-name descname"><span class="pre">fd</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#fd" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns a file descriptor for the database.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbfd.html">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">default</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#get" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">default</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns the data object associated with key. If key is an integer
 then the DB_SET_RECNO flag is automatically set for BTree databases
 and the actual key and the data value are returned as a tuple. If
 default is given then it is returned if the key is not found in the
 database. Partial records can be read using dlen and doff, however be
 sure to not read beyond the end of the actual data or you may get
 garbage.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbget.html">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pget">
-<span class="sig-name descname"><span class="pre">pget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">default</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pget" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">pget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">default</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pget" title="Permalink to this definition">¶</a></dt>
 <dd><p>This method is available only on secondary databases. It will return
 the primary key, given the secondary one, and associated data.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbget.html">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="get_transactional">
@@ -347,15 +341,15 @@
 be shared or preserved on disk may be created by setting both the
 filename and dbname arguments to None.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbopen.html">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="put">
-<span class="sig-name descname"><span class="pre">put</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#put" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">put</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#put" title="Permalink to this definition">¶</a></dt>
 <dd><p>Stores the key/data pair in the database. Partial data objects
 can be written using dlen and doff.</p>
 <p>If the DB_APPEND flag is used and the database is using the
 Recno, Queue or Heap access method then the record number
 (Recno or Queue) or Record ID (RID) (Heap) allocated to the
 data is returned.</p>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbput.html">More info…</a></p>
@@ -661,18 +655,14 @@
 <dt class="sig sig-object py" id="stat">
 <span class="sig-name descname"><span class="pre">stat</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">txn</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#stat" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return a dictionary containing database statistics with the following
 keys.</p>
 <p>For Hash databases:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 18%" />
-<col style="width: 82%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>magic</p></td>
 <td><p>Magic number that identifies the file as a Hash
 database.</p></td>
 </tr>
 <tr class="row-even"><td><p>version</p></td>
 <td><p>Version of the Hash database.</p></td>
@@ -734,18 +724,14 @@
 </tr>
 </tbody>
 </table>
 </div></blockquote>
 <p>For BTree and Recno databases:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 22%" />
-<col style="width: 78%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>magic</p></td>
 <td><p>Magic number that identifies the file as a
 Btree database.</p></td>
 </tr>
 <tr class="row-even"><td><p>version</p></td>
 <td><p>Version of the Btree database.</p></td>
@@ -826,18 +812,14 @@
 </tr>
 </tbody>
 </table>
 </div></blockquote>
 <p>For Queue databases:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 22%" />
-<col style="width: 78%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>magic</p></td>
 <td><p>Magic number that identifies the file as a
 Queue database.</p></td>
 </tr>
 <tr class="row-even"><td><p>version</p></td>
 <td><p>Version of the Queue file type.</p></td>
@@ -877,18 +859,14 @@
 </tr>
 </tbody>
 </table>
 </div></blockquote>
 <p>For Heap databases:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 22%" />
-<col style="width: 78%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>magic</p></td>
 <td><p>Magic number that identifies the file as a
 Heap database.</p></td>
 </tr>
 <tr class="row-even"><td><p>nrecs</p></td>
 <td><p>Reports the number of records in the Heap
@@ -960,15 +938,15 @@
 filename argument, and optionally outputs the databases’ key/data
 pairs to a file.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbverify.html">More info…</a></p>
 </dd></dl>
 
 </section>
 <section id="db-mapping-and-compatibility-methods">
-<h2>DB Mapping and Compatibility Methods<a class="headerlink" href="#db-mapping-and-compatibility-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DB Mapping and Compatibility Methods<a class="headerlink" href="#db-mapping-and-compatibility-methods" title="Permalink to this heading">¶</a></h2>
 <p>These methods of the DB type are for implementing the Mapping Interface,
 as well as others for making a DB behave as much like a dictionary as
 possible. The main downside to using a DB as a dictionary is you are not
 able to specify a transaction object.</p>
 <dl class="py function">
 <dt class="sig sig-object py">
 <span class="sig-name descname"><span class="pre">DB_length()</span> <span class="pre">[</span> <span class="pre">usage:</span> <span class="pre">len(db)</span> <span class="pre">]</span></span></dt>
@@ -1038,16 +1016,95 @@
 
 
 <h3>Navigation</h3>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="introduction.html">Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbenv.html">DBEnv</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">DB</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#db-methods">DB Methods</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#db-mapping-and-compatibility-methods">DB Mapping and Compatibility Methods</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#db-methods">DB Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#DB"><code class="docutils literal notranslate"><span class="pre">DB()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#append"><code class="docutils literal notranslate"><span class="pre">append()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#associate"><code class="docutils literal notranslate"><span class="pre">associate()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#close"><code class="docutils literal notranslate"><span class="pre">close()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#compact"><code class="docutils literal notranslate"><span class="pre">compact()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#consume"><code class="docutils literal notranslate"><span class="pre">consume()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#consume_wait"><code class="docutils literal notranslate"><span class="pre">consume_wait()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#cursor"><code class="docutils literal notranslate"><span class="pre">cursor()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#delete"><code class="docutils literal notranslate"><span class="pre">delete()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#exists"><code class="docutils literal notranslate"><span class="pre">exists()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#fd"><code class="docutils literal notranslate"><span class="pre">fd()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get"><code class="docutils literal notranslate"><span class="pre">get()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#pget"><code class="docutils literal notranslate"><span class="pre">pget()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_transactional"><code class="docutils literal notranslate"><span class="pre">get_transactional()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_priority"><code class="docutils literal notranslate"><span class="pre">get_priority()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_priority"><code class="docutils literal notranslate"><span class="pre">set_priority()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lk_exclusive"><code class="docutils literal notranslate"><span class="pre">get_lk_exclusive()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lk_exclusive"><code class="docutils literal notranslate"><span class="pre">set_lk_exclusive()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_dbname"><code class="docutils literal notranslate"><span class="pre">get_dbname()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_open_flags"><code class="docutils literal notranslate"><span class="pre">get_open_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_private"><code class="docutils literal notranslate"><span class="pre">set_private()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_private"><code class="docutils literal notranslate"><span class="pre">get_private()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_both"><code class="docutils literal notranslate"><span class="pre">get_both()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_byteswapped"><code class="docutils literal notranslate"><span class="pre">get_byteswapped()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_size"><code class="docutils literal notranslate"><span class="pre">get_size()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_type"><code class="docutils literal notranslate"><span class="pre">get_type()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#join"><code class="docutils literal notranslate"><span class="pre">join()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#key_range"><code class="docutils literal notranslate"><span class="pre">key_range()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#open"><code class="docutils literal notranslate"><span class="pre">open()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#put"><code class="docutils literal notranslate"><span class="pre">put()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#remove"><code class="docutils literal notranslate"><span class="pre">remove()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rename"><code class="docutils literal notranslate"><span class="pre">rename()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_encrypt"><code class="docutils literal notranslate"><span class="pre">set_encrypt()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_encrypt_flags"><code class="docutils literal notranslate"><span class="pre">get_encrypt_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_bt_compare"><code class="docutils literal notranslate"><span class="pre">set_bt_compare()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_bt_minkey"><code class="docutils literal notranslate"><span class="pre">get_bt_minkey()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_bt_minkey"><code class="docutils literal notranslate"><span class="pre">set_bt_minkey()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_cachesize"><code class="docutils literal notranslate"><span class="pre">set_cachesize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_cachesize"><code class="docutils literal notranslate"><span class="pre">get_cachesize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_heapsize"><code class="docutils literal notranslate"><span class="pre">set_heapsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_heapsize"><code class="docutils literal notranslate"><span class="pre">get_heapsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_heap_regionsize"><code class="docutils literal notranslate"><span class="pre">set_heap_regionsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_heap_regionsize"><code class="docutils literal notranslate"><span class="pre">get_heap_regionsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_dup_compare"><code class="docutils literal notranslate"><span class="pre">set_dup_compare()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_get_returns_none"><code class="docutils literal notranslate"><span class="pre">set_get_returns_none()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_flags"><code class="docutils literal notranslate"><span class="pre">get_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_flags"><code class="docutils literal notranslate"><span class="pre">set_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_h_ffactor"><code class="docutils literal notranslate"><span class="pre">get_h_ffactor()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_h_ffactor"><code class="docutils literal notranslate"><span class="pre">set_h_ffactor()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_h_nelem"><code class="docutils literal notranslate"><span class="pre">get_h_nelem()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_h_nelem"><code class="docutils literal notranslate"><span class="pre">set_h_nelem()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lorder"><code class="docutils literal notranslate"><span class="pre">get_lorder()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lorder"><code class="docutils literal notranslate"><span class="pre">set_lorder()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_pagesize"><code class="docutils literal notranslate"><span class="pre">get_pagesize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_pagesize"><code class="docutils literal notranslate"><span class="pre">set_pagesize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_re_delim"><code class="docutils literal notranslate"><span class="pre">get_re_delim()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_re_delim"><code class="docutils literal notranslate"><span class="pre">set_re_delim()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_re_len"><code class="docutils literal notranslate"><span class="pre">get_re_len()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_re_len"><code class="docutils literal notranslate"><span class="pre">set_re_len()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_re_pad"><code class="docutils literal notranslate"><span class="pre">get_re_pad()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_re_pad"><code class="docutils literal notranslate"><span class="pre">set_re_pad()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_re_source"><code class="docutils literal notranslate"><span class="pre">get_re_source()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_re_source"><code class="docutils literal notranslate"><span class="pre">set_re_source()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_q_extentsize"><code class="docutils literal notranslate"><span class="pre">get_q_extentsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_q_extentsize"><code class="docutils literal notranslate"><span class="pre">set_q_extentsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#stat"><code class="docutils literal notranslate"><span class="pre">stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#stat_print"><code class="docutils literal notranslate"><span class="pre">stat_print()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#sync"><code class="docutils literal notranslate"><span class="pre">sync()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#truncate"><code class="docutils literal notranslate"><span class="pre">truncate()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#upgrade"><code class="docutils literal notranslate"><span class="pre">upgrade()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#verify"><code class="docutils literal notranslate"><span class="pre">verify()</span></code></a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="#db-mapping-and-compatibility-methods">DB Mapping and Compatibility Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#keys"><code class="docutils literal notranslate"><span class="pre">keys()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#items"><code class="docutils literal notranslate"><span class="pre">items()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#values"><code class="docutils literal notranslate"><span class="pre">values()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#has_key"><code class="docutils literal notranslate"><span class="pre">has_key()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="dbcursor.html">DBCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblogcursor.html">DBLogCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbtxn.html">DBTxn</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblock.html">DBLock</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsequence.html">DBSequence</a></li>
@@ -1073,32 +1130,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** DBÂ¶ ******
 Read Oracle_documentation for better understanding.
 More_infoâ¦
 ***** DB MethodsÂ¶ *****
   DB(dbEnv=None, flags=0)Â¶
       Constructor. More_infoâ¦
   append(data, txn=None)Â¶
@@ -42,19 +41,19 @@
                       phase
       levels          The number of levels removed from the Btree or Recno
                       database during the compaction phase
       pages_truncated The number of database pages returned to the filesystem
       end             Will be filled with the database key/page marking the end
                       of the compaction operation
       More_infoâ¦
-  consume(txn=None, flags=0, dlen=- 1, doff=- 1)Â¶
+  consume(txn=None, flags=0, dlen=-1, doff=-1)Â¶
       For a database with the Queue access method, returns the record number
       and data from the first available record and deletes it from the queue.
       More_infoâ¦
-  consume_wait(txn=None, flags=0, dlen=- 1, doff=- 1)Â¶
+  consume_wait(txn=None, flags=0, dlen=-1, doff=-1)Â¶
       For a database with the Queue access method, returns the record number
       and data from the first available record and deletes it from the queue.
       If the Queue database is empty, the thread of control will wait until
       there is data in the queue before returning. More_infoâ¦
   cursor(txn=None, flags=0)Â¶
       Create a cursor on the DB and returns a DBCursor object. If a transaction
       is passed then the cursor can only be used within that transaction and
@@ -62,23 +61,23 @@
       More_infoâ¦
   delete(key, txn=None, flags=0)Â¶
       Removes a key/data pair from the database. More_infoâ¦
   exists(key, txn=None, flags=0)Â¶
       Test if a key exists in the database. Returns True or False. More_infoâ¦
   fd()Â¶
       Returns a file descriptor for the database. More_infoâ¦
-  get(key, default=None, txn=None, flags=0, dlen=- 1, doff=- 1)Â¶
+  get(key, default=None, txn=None, flags=0, dlen=-1, doff=-1)Â¶
       Returns the data object associated with key. If key is an integer then
       the DB_SET_RECNO flag is automatically set for BTree databases and the
       actual key and the data value are returned as a tuple. If default is
       given then it is returned if the key is not found in the database.
       Partial records can be read using dlen and doff, however be sure to not
       read beyond the end of the actual data or you may get garbage. More
       infoâ¦
-  pget(key, default=None, txn=None, flags=0, dlen=- 1, doff=- 1)Â¶
+  pget(key, default=None, txn=None, flags=0, dlen=-1, doff=-1)Â¶
       This method is available only on secondary databases. It will return the
       primary key, given the secondary one, and associated data. More_infoâ¦
   get_transactional()Â¶
       Returns True if the database is transactional. False if not. More_infoâ¦
   get_priority()Â¶
       Returns the cache priority for pages referenced by the DB handle. This
       priority value is set using the DB->set_priority() method. More_infoâ¦
@@ -147,15 +146,15 @@
       Opens the database named dbname in the file named filename. The dbname
       argument is optional and allows applications to have multiple logical
       databases in a single physical file. It is an error to attempt to open a
       second database in a file that was not initially created using a database
       name. In-memory databases never intended to be shared or preserved on
       disk may be created by setting both the filename and dbname arguments to
       None. More_infoâ¦
-  put(key, data, txn=None, flags=0, dlen=- 1, doff=- 1)Â¶
+  put(key, data, txn=None, flags=0, dlen=-1, doff=-1)Â¶
       Stores the key/data pair in the database. Partial data objects can be
       written using dlen and doff.
       If the DB_APPEND flag is used and the database is using the Recno, Queue
       or Heap access method then the record number (Recno or Queue) or Record
       ID (RID) (Heap) allocated to the data is returned.
       More_infoâ¦
   remove(filename, dbname=None, flags=0)Â¶
@@ -417,15 +416,90 @@
 
 ****** BerkeleyDB ******
 **** Navigation ****
     * Oracle_Berkeley_DB_4.8,_5.3,_6.2_and_18.1_Python_Extension_Package
     * DBEnv
     * DB
           o DB_Methods
+                # DB()
+                # append()
+                # associate()
+                # close()
+                # compact()
+                # consume()
+                # consume_wait()
+                # cursor()
+                # delete()
+                # exists()
+                # fd()
+                # get()
+                # pget()
+                # get_transactional()
+                # get_priority()
+                # set_priority()
+                # get_lk_exclusive()
+                # set_lk_exclusive()
+                # get_dbname()
+                # get_open_flags()
+                # set_private()
+                # get_private()
+                # get_both()
+                # get_byteswapped()
+                # get_size()
+                # get_type()
+                # join()
+                # key_range()
+                # open()
+                # put()
+                # remove()
+                # rename()
+                # set_encrypt()
+                # get_encrypt_flags()
+                # set_bt_compare()
+                # get_bt_minkey()
+                # set_bt_minkey()
+                # set_cachesize()
+                # get_cachesize()
+                # set_heapsize()
+                # get_heapsize()
+                # set_heap_regionsize()
+                # get_heap_regionsize()
+                # set_dup_compare()
+                # set_get_returns_none()
+                # get_flags()
+                # set_flags()
+                # get_h_ffactor()
+                # set_h_ffactor()
+                # get_h_nelem()
+                # set_h_nelem()
+                # get_lorder()
+                # set_lorder()
+                # get_pagesize()
+                # set_pagesize()
+                # get_re_delim()
+                # set_re_delim()
+                # get_re_len()
+                # set_re_len()
+                # get_re_pad()
+                # set_re_pad()
+                # get_re_source()
+                # set_re_source()
+                # get_q_extentsize()
+                # set_q_extentsize()
+                # stat()
+                # stat_print()
+                # sync()
+                # truncate()
+                # upgrade()
+                # verify()
           o DB_Mapping_and_Compatibility_Methods
+                # keys()
+                # items()
+                # values()
+                # has_key()
     * DBCursor
     * DBLogCursor
     * DBTxn
     * DBLock
     * DBSequence
     * DBSite
     * History
@@ -435,8 +509,8 @@
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: DBEnv
           o Next: DBCursor
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/dbcursor.html` & `berkeleydb-18.1.6/docs/html/dbcursor.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DBCursor &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DBCursor &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DBLogCursor" href="dblogcursor.html" />
     <link rel="prev" title="DB" href="db.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,20 +28,20 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="dbcursor">
-<h1>DBCursor<a class="headerlink" href="#dbcursor" title="Permalink to this headline">¶</a></h1>
+<h1>DBCursor<a class="headerlink" href="#dbcursor" title="Permalink to this heading">¶</a></h1>
 <p>Read <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/programmer_reference/index.html">Oracle documentation</a>
 for better understanding.</p>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbc.html">More info…</a></p>
 <section id="dbcursor-methods">
-<h2>DBCursor Methods<a class="headerlink" href="#dbcursor-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBCursor Methods<a class="headerlink" href="#dbcursor-methods" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="close">
 <span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Discards the cursor. If the cursor is created within a transaction
 then you <em>must</em> be sure to close the cursor before commiting the
 transaction.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcclose.html">More info…</a></p>
@@ -83,115 +81,115 @@
 <span class="sig-name descname"><span class="pre">get_priority</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#get_priority" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns the cache priority for pages referenced by the DBC handle.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget_priority.html">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="put">
-<span class="sig-name descname"><span class="pre">put</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#put" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">put</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#put" title="Permalink to this definition">¶</a></dt>
 <dd><p>Stores the key/data pair into the database. Partial data records can
 be written using dlen and doff.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcput.html">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#get" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#get" title="Permalink to this definition">¶</a></dt>
 <dd><p>See get(key, data, flags, dlen=-1, doff=-1) below.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="id0">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id0" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id0" title="Permalink to this definition">¶</a></dt>
 <dd><p>See get(key, data, flags, dlen=-1, doff=-1) below.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="id1">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id1" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id1" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieves key/data pairs from the database using the cursor. All the
 specific functionalities of the get method are actually provided by
 the various methods below, which are the preferred way to fetch data
 using the cursor. These generic interfaces are only provided as an
 inconvenience. Partial data records are returned if dlen and doff
 are used in this method and in many of the specific methods below.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="pget">
-<span class="sig-name descname"><span class="pre">pget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pget" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">pget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#pget" title="Permalink to this definition">¶</a></dt>
 <dd><p>See pget(key, data, flags, dlen=-1, doff=-1) below.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="id2">
-<span class="sig-name descname"><span class="pre">pget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id2" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">pget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id2" title="Permalink to this definition">¶</a></dt>
 <dd><p>See pget(key, data, flags, dlen=-1, doff=-1) below.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="id3">
-<span class="sig-name descname"><span class="pre">pget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id3" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">pget</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">data</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id3" title="Permalink to this definition">¶</a></dt>
 <dd><p>Similar to the already described get(). This method is available only
 on secondary databases. It will return the primary key, given the
 secondary one, and associated data
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html">More info…</a></p>
 </dd></dl>
 
 </section>
 <section id="dbcursor-get-methods">
-<h2>DBCursor Get Methods<a class="headerlink" href="#dbcursor-get-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBCursor Get Methods<a class="headerlink" href="#dbcursor-get-methods" title="Permalink to this heading">¶</a></h2>
 <p>These DBCursor methods are all wrappers around the get() function in the
 C API.</p>
 <dl class="py function">
 <dt class="sig sig-object py" id="current">
-<span class="sig-name descname"><span class="pre">current</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#current" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">current</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#current" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns the key/data pair currently referenced by the cursor.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_CURRENT">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="get_current_size">
 <span class="sig-name descname"><span class="pre">get_current_size</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#get_current_size" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns length of the data for the current entry referenced by the
 cursor.</p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="first">
-<span class="sig-name descname"><span class="pre">first</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#first" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">first</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#first" title="Permalink to this definition">¶</a></dt>
 <dd><p>Position the cursor to the first key/data pair and return it.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_FIRST">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="last">
-<span class="sig-name descname"><span class="pre">last</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#last" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">last</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#last" title="Permalink to this definition">¶</a></dt>
 <dd><p>Position the cursor to the last key/data pair and return it.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_LAST">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="next">
-<span class="sig-name descname"><span class="pre">next</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#next" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">next</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#next" title="Permalink to this definition">¶</a></dt>
 <dd><p>Position the cursor to the next key/data pair and return it.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_NEXT">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="prev">
-<span class="sig-name descname"><span class="pre">prev</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#prev" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">prev</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#prev" title="Permalink to this definition">¶</a></dt>
 <dd><p>Position the cursor to the previous key/data pair and return it.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_PREV">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="consume">
-<span class="sig-name descname"><span class="pre">consume</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#consume" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">consume</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#consume" title="Permalink to this definition">¶</a></dt>
 <dd><p>For a database with the Queue access method, returns the record
 number and data from the first available record and deletes it from
 the queue.</p>
 <p><em>NOTE:</em> This method is deprecated in Oracle Berkeley DB version
 3.2 in favor of the new consume method in the DB class.</p>
 </dd></dl>
 
@@ -219,67 +217,67 @@
 <dd><p>For cursors returned from the DB.join method, returns the combined
 key value from the joined cursors.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_JOIN_ITEM">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="next_dup">
-<span class="sig-name descname"><span class="pre">next_dup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#next_dup" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">next_dup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#next_dup" title="Permalink to this definition">¶</a></dt>
 <dd><p>If the next key/data pair of the database is a duplicate record for
 the current key/data pair, the cursor is moved to the next key/data
 pair of the database, and that pair is returned.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_NEXT_DUP">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="next_nodup">
-<span class="sig-name descname"><span class="pre">next_nodup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#next_nodup" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">next_nodup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#next_nodup" title="Permalink to this definition">¶</a></dt>
 <dd><p>The cursor is moved to the next non-duplicate key/data pair of the
 database, and that pair is returned.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_NEXT_NODUP">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="prev_dup">
-<span class="sig-name descname"><span class="pre">prev_dup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#prev_dup" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">prev_dup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#prev_dup" title="Permalink to this definition">¶</a></dt>
 <dd><p>If the previous key/data pair of the database is a duplicate data
 record for the current key/data pair, the cursor is moved to the
 previous key/data pair of the database, and that pair is returned.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_PREV_DUP">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="prev_nodup">
-<span class="sig-name descname"><span class="pre">prev_nodup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#prev_nodup" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">prev_nodup</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#prev_nodup" title="Permalink to this definition">¶</a></dt>
 <dd><p>The cursor is moved to the previous non-duplicate key/data pair of
 the database, and that pair is returned.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_PREV_NODUP">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="set">
-<span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#set" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#set" title="Permalink to this definition">¶</a></dt>
 <dd><p>Move the cursor to the specified key in the database and return the
 key/data pair found there.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_SET">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="set_range">
-<span class="sig-name descname"><span class="pre">set_range</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#set_range" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">set_range</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#set_range" title="Permalink to this definition">¶</a></dt>
 <dd><p>Identical to set() except that in the case of the BTree access
 method, the returned key/data pair is the smallest key greater than
 or equal to the specified key (as determined by the comparison
 function), permitting partial key matches and range searches.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_SET_RANGE">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="set_recno">
-<span class="sig-name descname"><span class="pre">set_recno</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">recno</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-</span> <span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#set_recno" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">set_recno</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">recno</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dlen</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">doff</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">-1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#set_recno" title="Permalink to this definition">¶</a></dt>
 <dd><p>Move the cursor to the specific numbered record of the database, and
 return the associated key/data pair. The underlying database must be
 of type Btree and it must have been created with the DB_RECNUM flag.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbcget.html#dbcget_DB_SET_RECNO">More info…</a></p>
 </dd></dl>
 
 <dl class="py function">
@@ -311,16 +309,51 @@
 
 <h3>Navigation</h3>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="introduction.html">Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbenv.html">DBEnv</a></li>
 <li class="toctree-l1"><a class="reference internal" href="db.html">DB</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">DBCursor</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#dbcursor-methods">DBCursor Methods</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#dbcursor-get-methods">DBCursor Get Methods</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#dbcursor-methods">DBCursor Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#close"><code class="docutils literal notranslate"><span class="pre">close()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#count"><code class="docutils literal notranslate"><span class="pre">count()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#delete"><code class="docutils literal notranslate"><span class="pre">delete()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#dup"><code class="docutils literal notranslate"><span class="pre">dup()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_priority"><code class="docutils literal notranslate"><span class="pre">set_priority()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_priority"><code class="docutils literal notranslate"><span class="pre">get_priority()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#put"><code class="docutils literal notranslate"><span class="pre">put()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get"><code class="docutils literal notranslate"><span class="pre">get()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#id0"><code class="docutils literal notranslate"><span class="pre">get()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#id1"><code class="docutils literal notranslate"><span class="pre">get()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#pget"><code class="docutils literal notranslate"><span class="pre">pget()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#id2"><code class="docutils literal notranslate"><span class="pre">pget()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#id3"><code class="docutils literal notranslate"><span class="pre">pget()</span></code></a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="#dbcursor-get-methods">DBCursor Get Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#current"><code class="docutils literal notranslate"><span class="pre">current()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_current_size"><code class="docutils literal notranslate"><span class="pre">get_current_size()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#first"><code class="docutils literal notranslate"><span class="pre">first()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#last"><code class="docutils literal notranslate"><span class="pre">last()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#next"><code class="docutils literal notranslate"><span class="pre">next()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#prev"><code class="docutils literal notranslate"><span class="pre">prev()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#consume"><code class="docutils literal notranslate"><span class="pre">consume()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_both"><code class="docutils literal notranslate"><span class="pre">get_both()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_recno"><code class="docutils literal notranslate"><span class="pre">get_recno()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#join_item"><code class="docutils literal notranslate"><span class="pre">join_item()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#next_dup"><code class="docutils literal notranslate"><span class="pre">next_dup()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#next_nodup"><code class="docutils literal notranslate"><span class="pre">next_nodup()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#prev_dup"><code class="docutils literal notranslate"><span class="pre">prev_dup()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#prev_nodup"><code class="docutils literal notranslate"><span class="pre">prev_nodup()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set"><code class="docutils literal notranslate"><span class="pre">set()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_range"><code class="docutils literal notranslate"><span class="pre">set_range()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_recno"><code class="docutils literal notranslate"><span class="pre">set_recno()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_both"><code class="docutils literal notranslate"><span class="pre">set_both()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="dblogcursor.html">DBLogCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbtxn.html">DBTxn</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblock.html">DBLock</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsequence.html">DBSequence</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsite.html">DBSite</a></li>
@@ -345,32 +378,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** DBCursorÂ¶ ******
 Read Oracle_documentation for better understanding.
 More_infoâ¦
 ***** DBCursor MethodsÂ¶ *****
   close()Â¶
       Discards the cursor. If the cursor is created within a transaction then
       you must be sure to close the cursor before commiting the transaction.
@@ -25,57 +24,57 @@
       Create a new cursor. More_infoâ¦
   set_priority(priority)Â¶
       Set the cache priority for pages referenced by the DBC handle. More
       infoâ¦
   get_priority()Â¶
       Returns the cache priority for pages referenced by the DBC handle. More
       infoâ¦
-  put(key, data, flags=0, dlen=- 1, doff=- 1)Â¶
+  put(key, data, flags=0, dlen=-1, doff=-1)Â¶
       Stores the key/data pair into the database. Partial data records can be
       written using dlen and doff. More_infoâ¦
-  get(flags, dlen=- 1, doff=- 1)Â¶
+  get(flags, dlen=-1, doff=-1)Â¶
       See get(key, data, flags, dlen=-1, doff=-1) below.
-  get(key, flags, dlen=- 1, doff=- 1)Â¶
+  get(key, flags, dlen=-1, doff=-1)Â¶
       See get(key, data, flags, dlen=-1, doff=-1) below.
-  get(key, data, flags, dlen=- 1, doff=- 1)Â¶
+  get(key, data, flags, dlen=-1, doff=-1)Â¶
       Retrieves key/data pairs from the database using the cursor. All the
       specific functionalities of the get method are actually provided by the
       various methods below, which are the preferred way to fetch data using
       the cursor. These generic interfaces are only provided as an
       inconvenience. Partial data records are returned if dlen and doff are
       used in this method and in many of the specific methods below. More
       infoâ¦
-  pget(flags, dlen=- 1, doff=- 1)Â¶
+  pget(flags, dlen=-1, doff=-1)Â¶
       See pget(key, data, flags, dlen=-1, doff=-1) below.
-  pget(key, flags, dlen=- 1, doff=- 1)Â¶
+  pget(key, flags, dlen=-1, doff=-1)Â¶
       See pget(key, data, flags, dlen=-1, doff=-1) below.
-  pget(key, data, flags, dlen=- 1, doff=- 1)Â¶
+  pget(key, data, flags, dlen=-1, doff=-1)Â¶
       Similar to the already described get(). This method is available only on
       secondary databases. It will return the primary key, given the secondary
       one, and associated data More_infoâ¦
 
 ***** DBCursor Get MethodsÂ¶ *****
 These DBCursor methods are all wrappers around the get() function in the C API.
-  current(flags=0, dlen=- 1, doff=- 1)Â¶
+  current(flags=0, dlen=-1, doff=-1)Â¶
       Returns the key/data pair currently referenced by the cursor. More
       infoâ¦
   get_current_size()Â¶
       Returns length of the data for the current entry referenced by the
       cursor.
-  first(flags=0, dlen=- 1, doff=- 1)Â¶
+  first(flags=0, dlen=-1, doff=-1)Â¶
       Position the cursor to the first key/data pair and return it. More
       infoâ¦
-  last(flags=0, dlen=- 1, doff=- 1)Â¶
+  last(flags=0, dlen=-1, doff=-1)Â¶
       Position the cursor to the last key/data pair and return it. More_infoâ¦
-  next(flags=0, dlen=- 1, doff=- 1)Â¶
+  next(flags=0, dlen=-1, doff=-1)Â¶
       Position the cursor to the next key/data pair and return it. More_infoâ¦
-  prev(flags=0, dlen=- 1, doff=- 1)Â¶
+  prev(flags=0, dlen=-1, doff=-1)Â¶
       Position the cursor to the previous key/data pair and return it. More
       infoâ¦
-  consume(flags=0, dlen=- 1, doff=- 1)Â¶
+  consume(flags=0, dlen=-1, doff=-1)Â¶
       For a database with the Queue access method, returns the record number
       and data from the first available record and deletes it from the queue.
       NOTE: This method is deprecated in Oracle Berkeley DB version 3.2 in
       favor of the new consume method in the DB class.
   get_both(key, data, flags=0)Â¶
       Like set() but positions the cursor to the record matching both key and
       data. (An alias for this is set_both, which makes more sense to meâ¦)
@@ -83,37 +82,37 @@
   get_recno()Â¶
       Return the record number associated with the cursor. The database must
       use the BTree access method and have been created with the DB_RECNUM
       flag. More_infoâ¦
   join_item(flags=0)Â¶
       For cursors returned from the DB.join method, returns the combined key
       value from the joined cursors. More_infoâ¦
-  next_dup(flags=0, dlen=- 1, doff=- 1)Â¶
+  next_dup(flags=0, dlen=-1, doff=-1)Â¶
       If the next key/data pair of the database is a duplicate record for the
       current key/data pair, the cursor is moved to the next key/data pair of
       the database, and that pair is returned. More_infoâ¦
-  next_nodup(flags=0, dlen=- 1, doff=- 1)Â¶
+  next_nodup(flags=0, dlen=-1, doff=-1)Â¶
       The cursor is moved to the next non-duplicate key/data pair of the
       database, and that pair is returned. More_infoâ¦
-  prev_dup(flags=0, dlen=- 1, doff=- 1)Â¶
+  prev_dup(flags=0, dlen=-1, doff=-1)Â¶
       If the previous key/data pair of the database is a duplicate data record
       for the current key/data pair, the cursor is moved to the previous key/
       data pair of the database, and that pair is returned. More_infoâ¦
-  prev_nodup(flags=0, dlen=- 1, doff=- 1)Â¶
+  prev_nodup(flags=0, dlen=-1, doff=-1)Â¶
       The cursor is moved to the previous non-duplicate key/data pair of the
       database, and that pair is returned. More_infoâ¦
-  set(key, flags=0, dlen=- 1, doff=- 1)Â¶
+  set(key, flags=0, dlen=-1, doff=-1)Â¶
       Move the cursor to the specified key in the database and return the key/
       data pair found there. More_infoâ¦
-  set_range(key, flags=0, dlen=- 1, doff=- 1)Â¶
+  set_range(key, flags=0, dlen=-1, doff=-1)Â¶
       Identical to set() except that in the case of the BTree access method,
       the returned key/data pair is the smallest key greater than or equal to
       the specified key (as determined by the comparison function), permitting
       partial key matches and range searches. More_infoâ¦
-  set_recno(recno, flags=0, dlen=- 1, doff=- 1)Â¶
+  set_recno(recno, flags=0, dlen=-1, doff=-1)Â¶
       Move the cursor to the specific numbered record of the database, and
       return the associated key/data pair. The underlying database must be of
       type Btree and it must have been created with the DB_RECNUM flag. More
       infoâ¦
   set_both(key, data, flags=0)Â¶
       See get_both(). The only difference in behaviour can be disabled using
       set_get_returns_none(2). More_infoâ¦
@@ -121,15 +120,46 @@
 ****** BerkeleyDB ******
 **** Navigation ****
     * Oracle_Berkeley_DB_4.8,_5.3,_6.2_and_18.1_Python_Extension_Package
     * DBEnv
     * DB
     * DBCursor
           o DBCursor_Methods
+                # close()
+                # count()
+                # delete()
+                # dup()
+                # set_priority()
+                # get_priority()
+                # put()
+                # get()
+                # get()
+                # get()
+                # pget()
+                # pget()
+                # pget()
           o DBCursor_Get_Methods
+                # current()
+                # get_current_size()
+                # first()
+                # last()
+                # next()
+                # prev()
+                # consume()
+                # get_both()
+                # get_recno()
+                # join_item()
+                # next_dup()
+                # next_nodup()
+                # prev_dup()
+                # prev_nodup()
+                # set()
+                # set_range()
+                # set_recno()
+                # set_both()
     * DBLogCursor
     * DBTxn
     * DBLock
     * DBSequence
     * DBSite
     * History
     * Changelog
@@ -138,8 +168,8 @@
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: DB
           o Next: DBLogCursor
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/dbenv.html` & `berkeleydb-18.1.6/docs/html/dbenv.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DBEnv &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DBEnv &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DB" href="db.html" />
     <link rel="prev" title="Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package" href="introduction.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,29 +28,29 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="dbenv">
-<h1>DBEnv<a class="headerlink" href="#dbenv" title="Permalink to this headline">¶</a></h1>
+<h1>DBEnv<a class="headerlink" href="#dbenv" title="Permalink to this heading">¶</a></h1>
 <p>Read <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/programmer_reference/index.html">Oracle documentation</a>
 for better understanding.</p>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/env.html">More info…</a></p>
 <section id="dbenv-attributes">
-<h2>DBEnv Attributes<a class="headerlink" href="#dbenv-attributes" title="Permalink to this headline">¶</a></h2>
+<h2>DBEnv Attributes<a class="headerlink" href="#dbenv-attributes" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="DBEnv">
 <span class="sig-name descname"><span class="pre">DBEnv</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#DBEnv" title="Permalink to this definition">¶</a></dt>
 <dd><p>database home directory (read-only)</p>
 </dd></dl>
 
 </section>
 <section id="dbenv-methods">
-<h2>DBEnv Methods<a class="headerlink" href="#dbenv-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBEnv Methods<a class="headerlink" href="#dbenv-methods" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="id0">
 <span class="sig-name descname"><span class="pre">DBEnv</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#id0" title="Permalink to this definition">¶</a></dt>
 <dd><p>Constructor.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/envcreate.html">More info…</a></p>
 </dd></dl>
 
@@ -84,18 +82,14 @@
 statistics.</p>
 <p>The returning value is a tuple. The first element is a dictionary
 with the general stats. The second element is another dictionary,
 keyed by filename, and the values are the stats for each file.</p>
 <p>The first dictionary contains these data:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 30%" />
-<col style="width: 70%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>gbytes</p></td>
 <td><p>Gigabytes of cache (total cache size is
 st_gbytes + st_bytes).</p></td>
 </tr>
 <tr class="row-even"><td><p>bytes</p></td>
 <td><p>Bytes of cache (total cache size is
@@ -250,18 +244,14 @@
 </tr>
 </tbody>
 </table>
 </div></blockquote>
 <p>The second dictionary contains these data:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 30%" />
-<col style="width: 70%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>pagesize</p></td>
 <td><p>Page size in bytes.</p></td>
 </tr>
 <tr class="row-even"><td><p>cache_hit</p></td>
 <td><p>Requested pages found in the cache.</p></td>
 </tr>
@@ -930,18 +920,14 @@
 <dl class="py function">
 <dt class="sig sig-object py" id="lock_stat">
 <span class="sig-name descname"><span class="pre">lock_stat</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#lock_stat" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns a dictionary of locking subsystem statistics with the
 following keys:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 26%" />
-<col style="width: 74%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>id</p></td>
 <td><p>Last allocated lock ID.</p></td>
 </tr>
 <tr class="row-even"><td><p>cur_maxid</p></td>
 <td><p>The current maximum unused locker ID.</p></td>
 </tr>
@@ -1131,18 +1117,14 @@
 <dl class="py function">
 <dt class="sig sig-object py" id="txn_stat">
 <span class="sig-name descname"><span class="pre">txn_stat</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#txn_stat" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return a dictionary of transaction statistics with the following
 keys:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 24%" />
-<col style="width: 76%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>last_ckp</p></td>
 <td><p>The LSN of the last checkpoint.</p></td>
 </tr>
 <tr class="row-even"><td><p>time_ckp</p></td>
 <td><p>Time the last completed checkpoint finished
 (as the number of seconds since the Epoch,
@@ -1223,18 +1205,14 @@
 <dl class="py function">
 <dt class="sig sig-object py" id="log_stat">
 <span class="sig-name descname"><span class="pre">log_stat</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#log_stat" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns a dictionary of logging subsystem statistics with the
 following keys:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 30%" />
-<col style="width: 70%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>magic</p></td>
 <td><p>The magic number that identifies a file as
 a log file.</p></td>
 </tr>
 <tr class="row-even"><td><p>version</p></td>
 <td><p>The version of the log file type.</p></td>
@@ -1373,18 +1351,14 @@
 <dl class="py function">
 <dt class="sig sig-object py" id="mutex_stat">
 <span class="sig-name descname"><span class="pre">mutex_stat</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#mutex_stat" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns a dictionary of mutex subsystem statistics with the following
 keys:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 28%" />
-<col style="width: 72%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>mutex_align</p></td>
 <td><p>The mutex alignment, in bytes.</p></td>
 </tr>
 <tr class="row-even"><td><p>mutex_tas_spins</p></td>
 <td><p>The number of times test-and-set mutexes
 will spin without blocking.</p></td>
@@ -1482,15 +1456,15 @@
 <span class="sig-name descname"><span class="pre">mutex_get_tas_spins</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#mutex_get_tas_spins" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns the test-and-set spin count.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/mutexget_tas_spins.html">More info…</a></p>
 </dd></dl>
 
 </section>
 <section id="dbenv-replication-manager-methods">
-<h2>DBEnv Replication Manager Methods<a class="headerlink" href="#dbenv-replication-manager-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBEnv Replication Manager Methods<a class="headerlink" href="#dbenv-replication-manager-methods" title="Permalink to this heading">¶</a></h2>
 <p>This module automates many of the tasks needed to provide replication
 abilities in a Berkeley DB system. The module is fairly limited, but
 enough in many cases. Users more demanding must use the <strong>full</strong> Base
 Replication API.</p>
 <p>This module requires pthread support (in Unix), so you must compile
 Berkeley DB with it if you want to be able to use the Replication
 Manager.</p>
@@ -1548,18 +1522,14 @@
 
 <dl class="py function">
 <dt class="sig sig-object py" id="repmgr_stat">
 <span class="sig-name descname"><span class="pre">repmgr_stat</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#repmgr_stat" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns a dictionary with the replication manager statistics. Keys
 are:</p>
 <table class="docutils align-default">
-<colgroup>
-<col style="width: 26%" />
-<col style="width: 74%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>perm_failed</p></td>
 <td><p>The number of times a message critical for
 maintaining database integrity (for example, a
 transaction commit), originating at this site,
 did not receive sufficient acknowledgement from
 clients, according to the configured
@@ -1598,15 +1568,15 @@
 <span class="sig-name descname"><span class="pre">repmgr_stat_print</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#repmgr_stat_print" title="Permalink to this definition">¶</a></dt>
 <dd><p>Displays the replication manager statistical information.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/repmgrstat_print.html">More info…</a></p>
 </dd></dl>
 
 </section>
 <section id="dbenv-replication-methods">
-<h2>DBEnv Replication Methods<a class="headerlink" href="#dbenv-replication-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBEnv Replication Methods<a class="headerlink" href="#dbenv-replication-methods" title="Permalink to this heading">¶</a></h2>
 <p>This section provides the raw methods for replication. If possible,
 it is recommended to use the Replication Manager.</p>
 <dl class="py function">
 <dt class="sig sig-object py" id="rep_elect">
 <span class="sig-name descname"><span class="pre">rep_elect</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">nsites</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">nvotes</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#rep_elect" title="Permalink to this definition">¶</a></dt>
 <dd><p>Holds an election for the master of a replication group.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/repelect.html">More info…</a></p>
@@ -1772,18 +1742,14 @@
 
 <dl class="py function">
 <dt class="sig sig-object py" id="rep_stat">
 <span class="sig-name descname"><span class="pre">rep_stat</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#rep_stat" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns a dictionary with the replication subsystem statistics. Keys
 are:</p>
 <table class="docutils align-default">
-<colgroup>
-<col style="width: 32%" />
-<col style="width: 68%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>st_bulk_fills</p></td>
 <td><p>The number of times the bulk buffer filled
 up, forcing the buffer content to be sent.</p></td>
 </tr>
 <tr class="row-even"><td><p>bulk_overflows</p></td>
 <td><p>The number of times a record was bigger
@@ -2048,18 +2014,162 @@
 
 
 
 <h3>Navigation</h3>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="introduction.html">Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">DBEnv</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#dbenv-attributes">DBEnv Attributes</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#dbenv-methods">DBEnv Methods</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#dbenv-replication-manager-methods">DBEnv Replication Manager Methods</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#dbenv-replication-methods">DBEnv Replication Methods</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#dbenv-attributes">DBEnv Attributes</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#DBEnv"><code class="docutils literal notranslate"><span class="pre">DBEnv()</span></code></a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="#dbenv-methods">DBEnv Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#id0"><code class="docutils literal notranslate"><span class="pre">DBEnv()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#close"><code class="docutils literal notranslate"><span class="pre">close()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#open"><code class="docutils literal notranslate"><span class="pre">open()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_cursor"><code class="docutils literal notranslate"><span class="pre">log_cursor()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#memp_stat"><code class="docutils literal notranslate"><span class="pre">memp_stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#memp_stat_print"><code class="docutils literal notranslate"><span class="pre">memp_stat_print()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#memp_sync"><code class="docutils literal notranslate"><span class="pre">memp_sync()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#memp_trickle"><code class="docutils literal notranslate"><span class="pre">memp_trickle()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#remove"><code class="docutils literal notranslate"><span class="pre">remove()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#dbremove"><code class="docutils literal notranslate"><span class="pre">dbremove()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#dbrename"><code class="docutils literal notranslate"><span class="pre">dbrename()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#backup"><code class="docutils literal notranslate"><span class="pre">backup()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#dbbackup"><code class="docutils literal notranslate"><span class="pre">dbbackup()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_backup_config"><code class="docutils literal notranslate"><span class="pre">get_backup_config()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_backup_config"><code class="docutils literal notranslate"><span class="pre">set_backup_config()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#fileid_reset"><code class="docutils literal notranslate"><span class="pre">fileid_reset()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_thread_count"><code class="docutils literal notranslate"><span class="pre">get_thread_count()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_thread_count"><code class="docutils literal notranslate"><span class="pre">set_thread_count()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_encrypt"><code class="docutils literal notranslate"><span class="pre">set_encrypt()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_encrypt_flags"><code class="docutils literal notranslate"><span class="pre">get_encrypt_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_intermediate_dir_mode"><code class="docutils literal notranslate"><span class="pre">get_intermediate_dir_mode()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_intermediate_dir_mode"><code class="docutils literal notranslate"><span class="pre">set_intermediate_dir_mode()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_timeout"><code class="docutils literal notranslate"><span class="pre">get_timeout()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_timeout"><code class="docutils literal notranslate"><span class="pre">set_timeout()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_mp_max_openfd"><code class="docutils literal notranslate"><span class="pre">get_mp_max_openfd()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_mp_max_openfd"><code class="docutils literal notranslate"><span class="pre">set_mp_max_openfd()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_mp_max_write"><code class="docutils literal notranslate"><span class="pre">get_mp_max_write()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_mp_max_write"><code class="docutils literal notranslate"><span class="pre">set_mp_max_write()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_shm_key"><code class="docutils literal notranslate"><span class="pre">set_shm_key()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_shm_key"><code class="docutils literal notranslate"><span class="pre">get_shm_key()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_cache_max"><code class="docutils literal notranslate"><span class="pre">set_cache_max()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_cache_max"><code class="docutils literal notranslate"><span class="pre">get_cache_max()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_cachesize"><code class="docutils literal notranslate"><span class="pre">set_cachesize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_cachesize"><code class="docutils literal notranslate"><span class="pre">get_cachesize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_data_dir"><code class="docutils literal notranslate"><span class="pre">set_data_dir()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_data_dirs"><code class="docutils literal notranslate"><span class="pre">get_data_dirs()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_flags"><code class="docutils literal notranslate"><span class="pre">get_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_flags"><code class="docutils literal notranslate"><span class="pre">set_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_tmp_dir"><code class="docutils literal notranslate"><span class="pre">set_tmp_dir()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_tmp_dir"><code class="docutils literal notranslate"><span class="pre">get_tmp_dir()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_get_returns_none"><code class="docutils literal notranslate"><span class="pre">set_get_returns_none()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_private"><code class="docutils literal notranslate"><span class="pre">set_private()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_private"><code class="docutils literal notranslate"><span class="pre">get_private()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_open_flags"><code class="docutils literal notranslate"><span class="pre">get_open_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lg_filemode"><code class="docutils literal notranslate"><span class="pre">get_lg_filemode()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lg_filemode"><code class="docutils literal notranslate"><span class="pre">set_lg_filemode()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lg_bsize"><code class="docutils literal notranslate"><span class="pre">get_lg_bsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lg_bsize"><code class="docutils literal notranslate"><span class="pre">set_lg_bsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lg_dir"><code class="docutils literal notranslate"><span class="pre">get_lg_dir()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lg_dir"><code class="docutils literal notranslate"><span class="pre">set_lg_dir()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lg_max"><code class="docutils literal notranslate"><span class="pre">set_lg_max()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lg_max"><code class="docutils literal notranslate"><span class="pre">get_lg_max()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lg_regionmax"><code class="docutils literal notranslate"><span class="pre">get_lg_regionmax()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lg_regionmax"><code class="docutils literal notranslate"><span class="pre">set_lg_regionmax()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lk_partitions"><code class="docutils literal notranslate"><span class="pre">get_lk_partitions()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lk_partitions"><code class="docutils literal notranslate"><span class="pre">set_lk_partitions()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lk_detect"><code class="docutils literal notranslate"><span class="pre">get_lk_detect()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lk_detect"><code class="docutils literal notranslate"><span class="pre">set_lk_detect()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lk_max_locks"><code class="docutils literal notranslate"><span class="pre">get_lk_max_locks()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lk_max_locks"><code class="docutils literal notranslate"><span class="pre">set_lk_max_locks()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lk_max_lockers"><code class="docutils literal notranslate"><span class="pre">get_lk_max_lockers()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lk_max_lockers"><code class="docutils literal notranslate"><span class="pre">set_lk_max_lockers()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_lk_max_objects"><code class="docutils literal notranslate"><span class="pre">get_lk_max_objects()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_lk_max_objects"><code class="docutils literal notranslate"><span class="pre">set_lk_max_objects()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_mp_mmapsize"><code class="docutils literal notranslate"><span class="pre">get_mp_mmapsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_mp_mmapsize"><code class="docutils literal notranslate"><span class="pre">set_mp_mmapsize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#stat_print"><code class="docutils literal notranslate"><span class="pre">stat_print()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_file"><code class="docutils literal notranslate"><span class="pre">log_file()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_printf"><code class="docutils literal notranslate"><span class="pre">log_printf()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_archive"><code class="docutils literal notranslate"><span class="pre">log_archive()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_flush"><code class="docutils literal notranslate"><span class="pre">log_flush()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_get_config"><code class="docutils literal notranslate"><span class="pre">log_get_config()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_set_config"><code class="docutils literal notranslate"><span class="pre">log_set_config()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#lock_detect"><code class="docutils literal notranslate"><span class="pre">lock_detect()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#lock_get"><code class="docutils literal notranslate"><span class="pre">lock_get()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#lock_id"><code class="docutils literal notranslate"><span class="pre">lock_id()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#lock_id_free"><code class="docutils literal notranslate"><span class="pre">lock_id_free()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#lock_put"><code class="docutils literal notranslate"><span class="pre">lock_put()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#lock_stat"><code class="docutils literal notranslate"><span class="pre">lock_stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#lock_stat_print"><code class="docutils literal notranslate"><span class="pre">lock_stat_print()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#cdsgroup_begin"><code class="docutils literal notranslate"><span class="pre">cdsgroup_begin()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_tx_max"><code class="docutils literal notranslate"><span class="pre">get_tx_max()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_tx_max"><code class="docutils literal notranslate"><span class="pre">set_tx_max()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_tx_timestamp"><code class="docutils literal notranslate"><span class="pre">get_tx_timestamp()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_tx_timestamp"><code class="docutils literal notranslate"><span class="pre">set_tx_timestamp()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#txn_begin"><code class="docutils literal notranslate"><span class="pre">txn_begin()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#txn_checkpoint"><code class="docutils literal notranslate"><span class="pre">txn_checkpoint()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#txn_stat"><code class="docutils literal notranslate"><span class="pre">txn_stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#txn_stat_print"><code class="docutils literal notranslate"><span class="pre">txn_stat_print()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#lsn_reset"><code class="docutils literal notranslate"><span class="pre">lsn_reset()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_stat"><code class="docutils literal notranslate"><span class="pre">log_stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#log_stat_print"><code class="docutils literal notranslate"><span class="pre">log_stat_print()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#txn_recover"><code class="docutils literal notranslate"><span class="pre">txn_recover()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_verbose"><code class="docutils literal notranslate"><span class="pre">set_verbose()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_verbose"><code class="docutils literal notranslate"><span class="pre">get_verbose()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_event_notify"><code class="docutils literal notranslate"><span class="pre">set_event_notify()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_stat"><code class="docutils literal notranslate"><span class="pre">mutex_stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_stat_print"><code class="docutils literal notranslate"><span class="pre">mutex_stat_print()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_set_max"><code class="docutils literal notranslate"><span class="pre">mutex_set_max()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_get_max"><code class="docutils literal notranslate"><span class="pre">mutex_get_max()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_set_increment"><code class="docutils literal notranslate"><span class="pre">mutex_set_increment()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_get_increment"><code class="docutils literal notranslate"><span class="pre">mutex_get_increment()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_set_align"><code class="docutils literal notranslate"><span class="pre">mutex_set_align()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_get_align"><code class="docutils literal notranslate"><span class="pre">mutex_get_align()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_set_tas_spins"><code class="docutils literal notranslate"><span class="pre">mutex_set_tas_spins()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#mutex_get_tas_spins"><code class="docutils literal notranslate"><span class="pre">mutex_get_tas_spins()</span></code></a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="#dbenv-replication-manager-methods">DBEnv Replication Manager Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#repmgr_start"><code class="docutils literal notranslate"><span class="pre">repmgr_start()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#repmgr_site"><code class="docutils literal notranslate"><span class="pre">repmgr_site()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#repmgr_site_by_eid"><code class="docutils literal notranslate"><span class="pre">repmgr_site_by_eid()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#repmgr_set_ack_policy"><code class="docutils literal notranslate"><span class="pre">repmgr_set_ack_policy()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#repmgr_get_ack_policy"><code class="docutils literal notranslate"><span class="pre">repmgr_get_ack_policy()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#repmgr_site_list"><code class="docutils literal notranslate"><span class="pre">repmgr_site_list()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#repmgr_stat"><code class="docutils literal notranslate"><span class="pre">repmgr_stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#repmgr_stat_print"><code class="docutils literal notranslate"><span class="pre">repmgr_stat_print()</span></code></a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="#dbenv-replication-methods">DBEnv Replication Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#rep_elect"><code class="docutils literal notranslate"><span class="pre">rep_elect()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_set_transport"><code class="docutils literal notranslate"><span class="pre">rep_set_transport()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_process_messsage"><code class="docutils literal notranslate"><span class="pre">rep_process_messsage()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_start"><code class="docutils literal notranslate"><span class="pre">rep_start()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_sync"><code class="docutils literal notranslate"><span class="pre">rep_sync()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_set_config"><code class="docutils literal notranslate"><span class="pre">rep_set_config()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_get_config"><code class="docutils literal notranslate"><span class="pre">rep_get_config()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_set_limit"><code class="docutils literal notranslate"><span class="pre">rep_set_limit()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_get_limit"><code class="docutils literal notranslate"><span class="pre">rep_get_limit()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_set_request"><code class="docutils literal notranslate"><span class="pre">rep_set_request()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_get_request"><code class="docutils literal notranslate"><span class="pre">rep_get_request()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_set_nsites"><code class="docutils literal notranslate"><span class="pre">rep_set_nsites()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_get_nsites"><code class="docutils literal notranslate"><span class="pre">rep_get_nsites()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_set_priority"><code class="docutils literal notranslate"><span class="pre">rep_set_priority()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_get_priority"><code class="docutils literal notranslate"><span class="pre">rep_get_priority()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_set_timeout"><code class="docutils literal notranslate"><span class="pre">rep_set_timeout()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_get_timeout"><code class="docutils literal notranslate"><span class="pre">rep_get_timeout()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_set_clockskew"><code class="docutils literal notranslate"><span class="pre">rep_set_clockskew()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_get_clockskew"><code class="docutils literal notranslate"><span class="pre">rep_get_clockskew()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_stat"><code class="docutils literal notranslate"><span class="pre">rep_stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#rep_stat_print"><code class="docutils literal notranslate"><span class="pre">rep_stat_print()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="db.html">DB</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbcursor.html">DBCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblogcursor.html">DBLogCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbtxn.html">DBTxn</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblock.html">DBLock</a></li>
@@ -2086,32 +2196,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** DBEnvÂ¶ ******
 Read Oracle_documentation for better understanding.
 More_infoâ¦
 ***** DBEnv AttributesÂ¶ *****
   DBEnv(flags=0)Â¶
       database home directory (read-only)
 
@@ -792,17 +791,153 @@
       Displays the replication subsystem statistical information. More_infoâ¦
 
 ****** BerkeleyDB ******
 **** Navigation ****
     * Oracle_Berkeley_DB_4.8,_5.3,_6.2_and_18.1_Python_Extension_Package
     * DBEnv
           o DBEnv_Attributes
+                # DBEnv()
           o DBEnv_Methods
+                # DBEnv()
+                # close()
+                # open()
+                # log_cursor()
+                # memp_stat()
+                # memp_stat_print()
+                # memp_sync()
+                # memp_trickle()
+                # remove()
+                # dbremove()
+                # dbrename()
+                # backup()
+                # dbbackup()
+                # get_backup_config()
+                # set_backup_config()
+                # fileid_reset()
+                # get_thread_count()
+                # set_thread_count()
+                # set_encrypt()
+                # get_encrypt_flags()
+                # get_intermediate_dir_mode()
+                # set_intermediate_dir_mode()
+                # get_timeout()
+                # set_timeout()
+                # get_mp_max_openfd()
+                # set_mp_max_openfd()
+                # get_mp_max_write()
+                # set_mp_max_write()
+                # set_shm_key()
+                # get_shm_key()
+                # set_cache_max()
+                # get_cache_max()
+                # set_cachesize()
+                # get_cachesize()
+                # set_data_dir()
+                # get_data_dirs()
+                # get_flags()
+                # set_flags()
+                # set_tmp_dir()
+                # get_tmp_dir()
+                # set_get_returns_none()
+                # set_private()
+                # get_private()
+                # get_open_flags()
+                # get_lg_filemode()
+                # set_lg_filemode()
+                # get_lg_bsize()
+                # set_lg_bsize()
+                # get_lg_dir()
+                # set_lg_dir()
+                # set_lg_max()
+                # get_lg_max()
+                # get_lg_regionmax()
+                # set_lg_regionmax()
+                # get_lk_partitions()
+                # set_lk_partitions()
+                # get_lk_detect()
+                # set_lk_detect()
+                # get_lk_max_locks()
+                # set_lk_max_locks()
+                # get_lk_max_lockers()
+                # set_lk_max_lockers()
+                # get_lk_max_objects()
+                # set_lk_max_objects()
+                # get_mp_mmapsize()
+                # set_mp_mmapsize()
+                # stat_print()
+                # log_file()
+                # log_printf()
+                # log_archive()
+                # log_flush()
+                # log_get_config()
+                # log_set_config()
+                # lock_detect()
+                # lock_get()
+                # lock_id()
+                # lock_id_free()
+                # lock_put()
+                # lock_stat()
+                # lock_stat_print()
+                # cdsgroup_begin()
+                # get_tx_max()
+                # set_tx_max()
+                # get_tx_timestamp()
+                # set_tx_timestamp()
+                # txn_begin()
+                # txn_checkpoint()
+                # txn_stat()
+                # txn_stat_print()
+                # lsn_reset()
+                # log_stat()
+                # log_stat_print()
+                # txn_recover()
+                # set_verbose()
+                # get_verbose()
+                # set_event_notify()
+                # mutex_stat()
+                # mutex_stat_print()
+                # mutex_set_max()
+                # mutex_get_max()
+                # mutex_set_increment()
+                # mutex_get_increment()
+                # mutex_set_align()
+                # mutex_get_align()
+                # mutex_set_tas_spins()
+                # mutex_get_tas_spins()
           o DBEnv_Replication_Manager_Methods
+                # repmgr_start()
+                # repmgr_site()
+                # repmgr_site_by_eid()
+                # repmgr_set_ack_policy()
+                # repmgr_get_ack_policy()
+                # repmgr_site_list()
+                # repmgr_stat()
+                # repmgr_stat_print()
           o DBEnv_Replication_Methods
+                # rep_elect()
+                # rep_set_transport()
+                # rep_process_messsage()
+                # rep_start()
+                # rep_sync()
+                # rep_set_config()
+                # rep_get_config()
+                # rep_set_limit()
+                # rep_get_limit()
+                # rep_set_request()
+                # rep_get_request()
+                # rep_set_nsites()
+                # rep_get_nsites()
+                # rep_set_priority()
+                # rep_get_priority()
+                # rep_set_timeout()
+                # rep_get_timeout()
+                # rep_set_clockskew()
+                # rep_get_clockskew()
+                # rep_stat()
+                # rep_stat_print()
     * DB
     * DBCursor
     * DBLogCursor
     * DBTxn
     * DBLock
     * DBSequence
     * DBSite
@@ -814,8 +949,8 @@
 **** Related Topics ****
     * Documentation_overview
           o Previous: Oracle_Berkeley_DB_4.8,_5.3,_6.2_and_18.1_Python
             Extension_Package
           o Next: DB
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/dblock.html` & `berkeleydb-18.1.6/docs/html/dblock.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DBLock &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DBLock &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DBSequence" href="dbsequence.html" />
     <link rel="prev" title="DBTxn" href="dbtxn.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,15 +28,15 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="dblock">
-<h1>DBLock<a class="headerlink" href="#dblock" title="Permalink to this headline">¶</a></h1>
+<h1>DBLock<a class="headerlink" href="#dblock" title="Permalink to this heading">¶</a></h1>
 <p>Read <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/programmer_reference/index.html">Oracle documentation</a>
 for better understanding.</p>
 <p>The DBLock objects have no methods or attributes. They are just opaque
 handles to the lock in question.</p>
 <p>They are managed via DBEnv methods.</p>
 </section>
 
@@ -90,32 +88,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** DBLockÂ¶ ******
 Read Oracle_documentation for better understanding.
 The DBLock objects have no methods or attributes. They are just opaque handles
 to the lock in question.
 They are managed via DBEnv methods.
 ****** BerkeleyDB ******
 **** Navigation ****
@@ -30,8 +29,8 @@
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: DBTxn
           o Next: DBSequence
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/dblogcursor.html` & `berkeleydb-18.1.6/docs/html/dblogcursor.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DBLogCursor &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DBLogCursor &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DBTxn" href="dbtxn.html" />
     <link rel="prev" title="DBCursor" href="dbcursor.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,30 +28,30 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="dblogcursor">
-<h1>DBLogCursor<a class="headerlink" href="#dblogcursor" title="Permalink to this headline">¶</a></h1>
+<h1>DBLogCursor<a class="headerlink" href="#dblogcursor" title="Permalink to this heading">¶</a></h1>
 <p>Read <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/programmer_reference/index.html">Oracle documentation</a>
 for better understanding.</p>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/logc.html">More info…</a></p>
 <section id="dblogcursor-methods">
-<h2>DBLogCursor Methods<a class="headerlink" href="#dblogcursor-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBLogCursor Methods<a class="headerlink" href="#dblogcursor-methods" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="close">
 <span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Discards the log cursor.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/logcclose.html">More info…</a></p>
 </dd></dl>
 
 </section>
 <section id="dblogcursor-get-methods">
-<h2>DBLogCursor Get Methods<a class="headerlink" href="#dblogcursor-get-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBLogCursor Get Methods<a class="headerlink" href="#dblogcursor-get-methods" title="Permalink to this heading">¶</a></h2>
 <p>These DBLogCursor methods are all wrappers around the get() function in
 the C API.</p>
 <p>These functions returns a tuple. The first element is a LSN tuple,
 and the second element is a bytes object with the log data.</p>
 <p>If the following methods don’t have log data to return, they return
 None.</p>
 <dl class="py function">
@@ -129,16 +127,27 @@
 <h3>Navigation</h3>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="introduction.html">Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbenv.html">DBEnv</a></li>
 <li class="toctree-l1"><a class="reference internal" href="db.html">DB</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbcursor.html">DBCursor</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">DBLogCursor</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#dblogcursor-methods">DBLogCursor Methods</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#dblogcursor-get-methods">DBLogCursor Get Methods</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#dblogcursor-methods">DBLogCursor Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#close"><code class="docutils literal notranslate"><span class="pre">close()</span></code></a></li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="#dblogcursor-get-methods">DBLogCursor Get Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#current"><code class="docutils literal notranslate"><span class="pre">current()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#first"><code class="docutils literal notranslate"><span class="pre">first()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#last"><code class="docutils literal notranslate"><span class="pre">last()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#next"><code class="docutils literal notranslate"><span class="pre">next()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#prev"><code class="docutils literal notranslate"><span class="pre">prev()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set"><code class="docutils literal notranslate"><span class="pre">set()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="dbtxn.html">DBTxn</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblock.html">DBLock</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsequence.html">DBSequence</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsite.html">DBSite</a></li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a></li>
@@ -162,32 +171,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** DBLogCursorÂ¶ ******
 Read Oracle_documentation for better understanding.
 More_infoâ¦
 ***** DBLogCursor MethodsÂ¶ *****
   close()Â¶
       Discards the log cursor. More_infoâ¦
 
@@ -51,15 +50,22 @@
 **** Navigation ****
     * Oracle_Berkeley_DB_4.8,_5.3,_6.2_and_18.1_Python_Extension_Package
     * DBEnv
     * DB
     * DBCursor
     * DBLogCursor
           o DBLogCursor_Methods
+                # close()
           o DBLogCursor_Get_Methods
+                # current()
+                # first()
+                # last()
+                # next()
+                # prev()
+                # set()
     * DBTxn
     * DBLock
     * DBSequence
     * DBSite
     * History
     * Changelog
     * Changelog_of_legacy_âbsddb3â_project
@@ -67,8 +73,8 @@
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: DBCursor
           o Next: DBTxn
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/dbsequence.html` & `berkeleydb-18.1.6/docs/html/dbsequence.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DBSequence &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DBSequence &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DBSite" href="dbsite.html" />
     <link rel="prev" title="DBLock" href="dblock.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,25 +28,25 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="dbsequence">
-<h1>DBSequence<a class="headerlink" href="#dbsequence" title="Permalink to this headline">¶</a></h1>
+<h1>DBSequence<a class="headerlink" href="#dbsequence" title="Permalink to this heading">¶</a></h1>
 <p>Read <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/programmer_reference/index.html">Oracle documentation</a>
 for better understanding.</p>
 <p>Sequences provide an arbitrary number of persistent objects that return
 an increasing or decreasing sequence of integers. Opening a sequence
 handle associates it with a record in a database. The handle can
 maintain a cache of values from the database so that a database update
 is not needed as the application allocates a value.</p>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/seq.html">More info…</a></p>
 <section id="dbsequence-methods">
-<h2>DBSequence Methods<a class="headerlink" href="#dbsequence-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBSequence Methods<a class="headerlink" href="#dbsequence-methods" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="DBSequence">
 <span class="sig-name descname"><span class="pre">DBSequence</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">db</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#DBSequence" title="Permalink to this definition">¶</a></dt>
 <dd><p>Constructor.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/seqcreate.html">More info…</a></p>
 </dd></dl>
 
@@ -134,18 +132,14 @@
 
 <dl class="py function">
 <dt class="sig sig-object py" id="stat">
 <span class="sig-name descname"><span class="pre">stat</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#stat" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns a dictionary of sequence statistics with the following keys:</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 21%" />
-<col style="width: 79%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p>wait</p></td>
 <td><p>The number of times a thread of control was
 forced to wait on the handle mutex.</p></td>
 </tr>
 <tr class="row-even"><td><p>nowait</p></td>
 <td><p>The number of times that a thread
@@ -227,15 +221,33 @@
 <li class="toctree-l1"><a class="reference internal" href="dbenv.html">DBEnv</a></li>
 <li class="toctree-l1"><a class="reference internal" href="db.html">DB</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbcursor.html">DBCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblogcursor.html">DBLogCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbtxn.html">DBTxn</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblock.html">DBLock</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">DBSequence</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#dbsequence-methods">DBSequence Methods</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#dbsequence-methods">DBSequence Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#DBSequence"><code class="docutils literal notranslate"><span class="pre">DBSequence()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#open"><code class="docutils literal notranslate"><span class="pre">open()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#close"><code class="docutils literal notranslate"><span class="pre">close()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#initial_value"><code class="docutils literal notranslate"><span class="pre">initial_value()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get"><code class="docutils literal notranslate"><span class="pre">get()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_dbp"><code class="docutils literal notranslate"><span class="pre">get_dbp()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_key"><code class="docutils literal notranslate"><span class="pre">get_key()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#remove"><code class="docutils literal notranslate"><span class="pre">remove()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_cachesize"><code class="docutils literal notranslate"><span class="pre">get_cachesize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_cachesize"><code class="docutils literal notranslate"><span class="pre">set_cachesize()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_flags"><code class="docutils literal notranslate"><span class="pre">get_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_flags"><code class="docutils literal notranslate"><span class="pre">set_flags()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#stat"><code class="docutils literal notranslate"><span class="pre">stat()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#stat_print"><code class="docutils literal notranslate"><span class="pre">stat_print()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_range"><code class="docutils literal notranslate"><span class="pre">get_range()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_range"><code class="docutils literal notranslate"><span class="pre">set_range()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="dbsite.html">DBSite</a></li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a></li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a></li>
 <li class="toctree-l1"><a class="reference internal" href="changelog-bsddb3.html">Changelog of legacy “bsddb3” project</a></li>
 <li class="toctree-l1"><a class="reference internal" href="license.html">LICENSE</a></li>
@@ -256,32 +268,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** DBSequenceÂ¶ ******
 Read Oracle_documentation for better understanding.
 Sequences provide an arbitrary number of persistent objects that return an
 increasing or decreasing sequence of integers. Opening a sequence handle
 associates it with a record in a database. The handle can maintain a cache of
 values from the database so that a database update is not needed as the
 application allocates a value.
@@ -74,20 +73,36 @@
     * DB
     * DBCursor
     * DBLogCursor
     * DBTxn
     * DBLock
     * DBSequence
           o DBSequence_Methods
+                # DBSequence()
+                # open()
+                # close()
+                # initial_value()
+                # get()
+                # get_dbp()
+                # get_key()
+                # remove()
+                # get_cachesize()
+                # set_cachesize()
+                # get_flags()
+                # set_flags()
+                # stat()
+                # stat_print()
+                # get_range()
+                # set_range()
     * DBSite
     * History
     * Changelog
     * Changelog_of_legacy_âbsddb3â_project
     * LICENSE
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: DBLock
           o Next: DBSite
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/dbsite.html` & `berkeleydb-18.1.6/docs/html/dbsite.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DBSite &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DBSite &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="History" href="history.html" />
     <link rel="prev" title="DBSequence" href="dbsequence.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,21 +28,21 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="dbsite">
-<h1>DBSite<a class="headerlink" href="#dbsite" title="Permalink to this headline">¶</a></h1>
+<h1>DBSite<a class="headerlink" href="#dbsite" title="Permalink to this heading">¶</a></h1>
 <p>Read <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/programmer_reference/group_membership.html">Oracle documentation</a>
 for better understanding.</p>
 <p>You use the DB_SITE handle to configure and manage replication sites.</p>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/repmgr_site.html">More info…</a></p>
 <section id="dbsite-methods">
-<h2>DBSite Methods<a class="headerlink" href="#dbsite-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBSite Methods<a class="headerlink" href="#dbsite-methods" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="close">
 <span class="sig-name descname"><span class="pre">close</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">flags</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#close" title="Permalink to this definition">¶</a></dt>
 <dd><p>Close a DBSite handle.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/dbsite_close.html">More info…</a></p>
 </dd></dl>
 
@@ -113,15 +111,23 @@
 <li class="toctree-l1"><a class="reference internal" href="db.html">DB</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbcursor.html">DBCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblogcursor.html">DBLogCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbtxn.html">DBTxn</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblock.html">DBLock</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsequence.html">DBSequence</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">DBSite</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#dbsite-methods">DBSite Methods</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#dbsite-methods">DBSite Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#close"><code class="docutils literal notranslate"><span class="pre">close()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_address"><code class="docutils literal notranslate"><span class="pre">get_address()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_config"><code class="docutils literal notranslate"><span class="pre">get_config()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_eid"><code class="docutils literal notranslate"><span class="pre">get_eid()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#remove"><code class="docutils literal notranslate"><span class="pre">remove()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_config"><code class="docutils literal notranslate"><span class="pre">set_config()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a></li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a></li>
 <li class="toctree-l1"><a class="reference internal" href="changelog-bsddb3.html">Changelog of legacy “bsddb3” project</a></li>
 <li class="toctree-l1"><a class="reference internal" href="license.html">LICENSE</a></li>
 <li class="toctree-l1"><a class="reference internal" href="donate.html">DONATE!</a></li>
@@ -141,32 +147,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** DBSiteÂ¶ ******
 Read Oracle_documentation for better understanding.
 You use the DB_SITE handle to configure and manage replication sites.
 More_infoâ¦
 ***** DBSite MethodsÂ¶ *****
   close(flags=0)Â¶
       Close a DBSite handle. More_infoâ¦
@@ -38,19 +37,25 @@
     * DBCursor
     * DBLogCursor
     * DBTxn
     * DBLock
     * DBSequence
     * DBSite
           o DBSite_Methods
+                # close()
+                # get_address()
+                # get_config()
+                # get_eid()
+                # remove()
+                # set_config()
     * History
     * Changelog
     * Changelog_of_legacy_âbsddb3â_project
     * LICENSE
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: DBSequence
           o Next: History
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/dbtxn.html` & `berkeleydb-18.1.6/docs/html/dbtxn.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DBTxn &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DBTxn &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DBLock" href="dblock.html" />
     <link rel="prev" title="DBLogCursor" href="dblogcursor.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,20 +28,20 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="dbtxn">
-<h1>DBTxn<a class="headerlink" href="#dbtxn" title="Permalink to this headline">¶</a></h1>
+<h1>DBTxn<a class="headerlink" href="#dbtxn" title="Permalink to this heading">¶</a></h1>
 <p>Read <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/programmer_reference/index.html">Oracle documentation</a>
 for better understanding.</p>
 <p><a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/txn.html">More info…</a></p>
 <section id="dbtxn-methods">
-<h2>DBTxn Methods<a class="headerlink" href="#dbtxn-methods" title="Permalink to this headline">¶</a></h2>
+<h2>DBTxn Methods<a class="headerlink" href="#dbtxn-methods" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="abort">
 <span class="sig-name descname"><span class="pre">abort</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#abort" title="Permalink to this definition">¶</a></dt>
 <dd><p>Aborts the transaction
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/txnabort.html">More info…</a></p>
 </dd></dl>
 
@@ -147,15 +145,27 @@
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="introduction.html">Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbenv.html">DBEnv</a></li>
 <li class="toctree-l1"><a class="reference internal" href="db.html">DB</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbcursor.html">DBCursor</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dblogcursor.html">DBLogCursor</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">DBTxn</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#dbtxn-methods">DBTxn Methods</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#dbtxn-methods">DBTxn Methods</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#abort"><code class="docutils literal notranslate"><span class="pre">abort()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#commit"><code class="docutils literal notranslate"><span class="pre">commit()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#id"><code class="docutils literal notranslate"><span class="pre">id()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#prepare"><code class="docutils literal notranslate"><span class="pre">prepare()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#discard"><code class="docutils literal notranslate"><span class="pre">discard()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_timeout"><code class="docutils literal notranslate"><span class="pre">set_timeout()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_name"><code class="docutils literal notranslate"><span class="pre">get_name()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_name"><code class="docutils literal notranslate"><span class="pre">set_name()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#get_priority"><code class="docutils literal notranslate"><span class="pre">get_priority()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#set_priority"><code class="docutils literal notranslate"><span class="pre">set_priority()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="dblock.html">DBLock</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsequence.html">DBSequence</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dbsite.html">DBSite</a></li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a></li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a></li>
@@ -178,32 +188,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** DBTxnÂ¶ ******
 Read Oracle_documentation for better understanding.
 More_infoâ¦
 ***** DBTxn MethodsÂ¶ *****
   abort()Â¶
       Aborts the transaction More_infoâ¦
   commit(flags=0)Â¶
@@ -54,22 +53,32 @@
     * Oracle_Berkeley_DB_4.8,_5.3,_6.2_and_18.1_Python_Extension_Package
     * DBEnv
     * DB
     * DBCursor
     * DBLogCursor
     * DBTxn
           o DBTxn_Methods
+                # abort()
+                # commit()
+                # id()
+                # prepare()
+                # discard()
+                # set_timeout()
+                # get_name()
+                # set_name()
+                # get_priority()
+                # set_priority()
     * DBLock
     * DBSequence
     * DBSite
     * History
     * Changelog
     * Changelog_of_legacy_âbsddb3â_project
     * LICENSE
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: DBLogCursor
           o Next: DBLock
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/donate.html` & `berkeleydb-18.1.6/docs/html/donate.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DONATE! &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>DONATE! &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="LICENSE" href="license.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
   
@@ -29,15 +27,15 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="donate">
-<h1>DONATE!<a class="headerlink" href="#donate" title="Permalink to this headline">¶</a></h1>
+<h1>DONATE!<a class="headerlink" href="#donate" title="Permalink to this heading">¶</a></h1>
 <p>Work on this project is currently driven by my own interests, needs and
 spare time. If you appreciate this software or if you want to sponsor a
 currently not translated API feature, please consider donation to the
 project.</p>
 <p>Python Berkeley DB bindings needs your help.</p>
 <p>You can donate using <a class="reference external" href="https://en.wikipedia.org/wiki/Bitcoin">BitCoins</a>. The destination address is
 16avqyUK4vDqBdpUy365PPW44zNqVHLZSC.</p>
@@ -135,32 +133,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
 
 
 
 
 
 
 
-
 ****** DONATE!Â¶ ******
 Work on this project is currently driven by my own interests, needs and spare
 time. If you appreciate this software or if you want to sponsor a currently not
 translated API feature, please consider donation to the project.
 Python Berkeley DB bindings needs your help.
 You can donate using BitCoins. The destination address is
 16avqyUK4vDqBdpUy365PPW44zNqVHLZSC.
@@ -69,8 +68,8 @@
     * LICENSE
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: LICENSE
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/genindex.html` & `berkeleydb-18.1.6/docs/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>Index &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
   
   <meta name="viewport" content="width=device-width, initial-scale=0.9, maximum-scale=0.9" />
@@ -2355,32 +2353,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
 
 
 
 
 
 
-
 ****** Index ******
 A | B | C | D | E | F | G | H | I | J | K | L | M | N | O | P | R | S | T | U |
 V
 ***** A *****
     * abort()
           o built-in_function     * associate()
     * append()                          o built-in_function
@@ -526,8 +525,8 @@
     * Changelog_of_legacy_âbsddb3â_project
     * LICENSE
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/history.html` & `berkeleydb-18.1.6/docs/html/history.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>History &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>History &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Changelog" href="changelog.html" />
     <link rel="prev" title="DBSite" href="dbsite.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,15 +28,15 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="history">
-<h1>History<a class="headerlink" href="#history" title="Permalink to this headline">¶</a></h1>
+<h1>History<a class="headerlink" href="#history" title="Permalink to this heading">¶</a></h1>
 <p>This module was started by Andrew Kuchling (amk) to remove the
 dependency on SWIG in a package by Gregory P. Smith who based his work
 on a similar package by Robin Dunn which wrapped Berkeley DB 2.7.x.</p>
 <p>Development then returned full circle back to Robin Dunn working in
 behalf of <a class="reference external" href="http://www.digicool.com/">Digital Creations</a> to complete the SWIG-less wrapping of the DB
 3.x API and to build a solid unit test suite. Having completed that,
 Robin was now busy with another project (<a class="reference external" href="http://www.wxpython.org/">wxPython</a>) and Greg returned as
@@ -98,32 +96,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** HistoryÂ¶ ******
 This module was started by Andrew Kuchling (amk) to remove the dependency on
 SWIG in a package by Gregory P. Smith who based his work on a similar package
 by Robin Dunn which wrapped Berkeley DB 2.7.x.
 Development then returned full circle back to Robin Dunn working in behalf of
 Digital_Creations to complete the SWIG-less wrapping of the DB 3.x API and to
 build a solid unit test suite. Having completed that, Robin was now busy with
@@ -37,8 +36,8 @@
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: DBSite
           o Next: Changelog
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/images/bitcoin.png` & `berkeleydb-18.1.6/docs/html/images/bitcoin.png`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/html/introduction.html` & `berkeleydb-18.1.6/docs/html/introduction.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DBEnv" href="dbenv.html" />
     <link rel="prev" title="Python Bindings for Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1" href="index.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,17 +28,17 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="oracle-berkeley-db-4-8-5-3-6-2-and-18-1-python-extension-package">
-<h1>Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package<a class="headerlink" href="#oracle-berkeley-db-4-8-5-3-6-2-and-18-1-python-extension-package" title="Permalink to this headline">¶</a></h1>
+<h1>Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package<a class="headerlink" href="#oracle-berkeley-db-4-8-5-3-6-2-and-18-1-python-extension-package" title="Permalink to this heading">¶</a></h1>
 <section id="introduction">
-<h2>Introduction<a class="headerlink" href="#introduction" title="Permalink to this headline">¶</a></h2>
+<h2>Introduction<a class="headerlink" href="#introduction" title="Permalink to this heading">¶</a></h2>
 <p>This is a simple bit of documentation for the berkeleydb.db Python extension
 module which wraps the Oracle Berkeley DB C library. The extension
 module is located in a Python package along with a few pure python
 modules.</p>
 <p>It is expected that this module will be used in the following general
 ways by different programmers in different situations. The goals of
 this module are to allow all of these methods without making things too
@@ -74,15 +72,15 @@
 transaction objects to the methods. Again, most of this advanced
 functionality is activated simply by opening a DBEnv with the proper
 flags, and also by using transactions and being aware of and reacting
 to deadlock exceptions, etc.</p></li>
 </ol>
 </section>
 <section id="types-provided">
-<h2>Types Provided<a class="headerlink" href="#types-provided" title="Permalink to this headline">¶</a></h2>
+<h2>Types Provided<a class="headerlink" href="#types-provided" title="Permalink to this heading">¶</a></h2>
 <p>The berkeleydb.db extension module provides the following object types:</p>
 <ul class="simple">
 <li><p><strong>DB:</strong> The basic database object, capable of Hash, BTree, Recno,
 Queue and Heap access methods.</p></li>
 <li><p><strong>DBEnv:</strong> Provides a Database Environment for more advanced database
 use. Apps using transactions, logging, concurrent access, etc. will
 need to have an environment object.</p></li>
@@ -96,15 +94,15 @@
 <li><p><strong>DBSequence:</strong> Sequences provide an arbitrary number of persistent
 objects that return an increasing or decreasing sequence of integers.
 Opening a sequence handle associates it with a record in a database.</p></li>
 <li><p><strong>DBSite:</strong> Site object for Replication Manager.</p></li>
 </ul>
 </section>
 <section id="top-level-functions">
-<h2>Top level functions<a class="headerlink" href="#top-level-functions" title="Permalink to this headline">¶</a></h2>
+<h2>Top level functions<a class="headerlink" href="#top-level-functions" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="version">
 <span class="sig-name descname"><span class="pre">version</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#version" title="Permalink to this definition">¶</a></dt>
 <dd><p>Returns a tuple with major, minor and patch level.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/envversion.html">More info…</a></p>
 </dd></dl>
 
@@ -114,15 +112,15 @@
 <dd><p>Returns a tuple with the full version string, family, release,
 major, minor and patch level.
 <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/envfullversion.html">More info…</a></p>
 </dd></dl>
 
 </section>
 <section id="exceptions-provided">
-<h2>Exceptions Provided<a class="headerlink" href="#exceptions-provided" title="Permalink to this headline">¶</a></h2>
+<h2>Exceptions Provided<a class="headerlink" href="#exceptions-provided" title="Permalink to this heading">¶</a></h2>
 <p>The Oracle Berkeley DB C API uses function return codes to signal various
 errors. The berkeleydb.db module checks for these error codes and turns them
 into Python exceptions, allowing you to use familiar try:… except:…
 constructs and not have to bother with checking every method’s return
 value.</p>
 <p>Each of the error codes is turned into an exception specific to that
 error code, as outlined in the table below. If you are using the C API
@@ -136,18 +134,14 @@
 help make a DB look and act like a dictionary. We do the same trick with
 DBKeyEmptyError.</p>
 <p>When any of these exceptions is raised, the associated value is a tuple
 containing an integer representing the error code and a string for the
 error message itself.</p>
 <blockquote>
 <div><table class="docutils align-default">
-<colgroup>
-<col style="width: 39%" />
-<col style="width: 61%" />
-</colgroup>
 <tbody>
 <tr class="row-odd"><td><p><strong>DBError</strong></p></td>
 <td><p>Base class, all others derive from this</p></td>
 </tr>
 <tr class="row-even"><td><p><strong>DBCursorClosedError</strong></p></td>
 <td><p>When trying to use a closed cursor</p></td>
 </tr>
@@ -233,15 +227,15 @@
 <td><p>EPERM</p></td>
 </tr>
 </tbody>
 </table>
 </div></blockquote>
 </section>
 <section id="other-package-modules">
-<h2>Other Package Modules<a class="headerlink" href="#other-package-modules" title="Permalink to this headline">¶</a></h2>
+<h2>Other Package Modules<a class="headerlink" href="#other-package-modules" title="Permalink to this heading">¶</a></h2>
 <ul class="simple">
 <li><p><strong>dbshelve.py:</strong> This is an implementation of the standard Python
 shelve concept for storing objects that uses berkeleydb specifically, and
 also exposes some of the more advanced methods and capabilities of the
 underlying DB.</p></li>
 <li><p><strong>dbtables.py:</strong> This is a module by Gregory Smith that implements a
 simplistic table structure on top of a DB.</p></li>
@@ -250,23 +244,23 @@
 <li><p><strong>dbobj.py:</strong> Contains subclassable versions of DB and DBEnv.</p></li>
 <li><p><strong>dbrecio.py:</strong> Contains the DBRecIO class that can be used to do
 partial reads and writes from a DB record using a file-like interface.
 Contributed by Itamar Shtull-Trauring.</p></li>
 </ul>
 </section>
 <section id="testing">
-<h2>Testing<a class="headerlink" href="#testing" title="Permalink to this headline">¶</a></h2>
+<h2>Testing<a class="headerlink" href="#testing" title="Permalink to this heading">¶</a></h2>
 <p>A full unit test suite is being developed to exercise the various object
 types, their methods and the various usage modes described in the
 introduction. <a class="reference external" href="http://pyunit.sourceforge.net/">PyUnit</a> is used and
 the tests are structured such that they can be run unattended and
 automated. There are currently 482 test cases!  (March 2010)</p>
 </section>
 <section id="reference">
-<h2>Reference<a class="headerlink" href="#reference" title="Permalink to this headline">¶</a></h2>
+<h2>Reference<a class="headerlink" href="#reference" title="Permalink to this heading">¶</a></h2>
 <p>See the C language API <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/api_reference/C/index.html">online documentation</a>
 on Oracle’s website for more details of the
 functionality of each of these methods. The names of all the Python
 methods should be the same or similar to the names in the C API.</p>
 <p>Oracle Berkeley DB is very powerful and versatile, but it is complex to
 use correctly. <a class="reference external" href="https://docs.oracle.com/database/bdb181/html/toc.htm">Oracle documentation</a> is very
 complete. Please, review it.</p>
@@ -296,15 +290,19 @@
 
 
 <h3>Navigation</h3>
 <ul class="current">
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension Package</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#introduction">Introduction</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#types-provided">Types Provided</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#top-level-functions">Top level functions</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#top-level-functions">Top level functions</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="#version"><code class="docutils literal notranslate"><span class="pre">version()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="#full_version"><code class="docutils literal notranslate"><span class="pre">full_version()</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="#exceptions-provided">Exceptions Provided</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#other-package-modules">Other Package Modules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#testing">Testing</a></li>
 <li class="toctree-l2"><a class="reference internal" href="#reference">Reference</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="dbenv.html">DBEnv</a></li>
@@ -336,32 +334,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,15 +2,14 @@
 
 
 
 
 
 
 
-
 ****** Oracle Berkeley DB 4.8, 5.3, 6.2 and 18.1 Python Extension PackageÂ¶
 ******
 ***** IntroductionÂ¶ *****
 This is a simple bit of documentation for the berkeleydb.db Python extension
 module which wraps the Oracle Berkeley DB C library. The extension module is
 located in a Python package along with a few pure python modules.
 It is expected that this module will be used in the following general ways by
@@ -154,14 +153,16 @@
 
 ****** BerkeleyDB ******
 **** Navigation ****
     * Oracle_Berkeley_DB_4.8,_5.3,_6.2_and_18.1_Python_Extension_Package
           o Introduction
           o Types_Provided
           o Top_level_functions
+                # version()
+                # full_version()
           o Exceptions_Provided
           o Other_Package_Modules
           o Testing
           o Reference
     * DBEnv
     * DB
     * DBCursor
@@ -178,8 +179,8 @@
 **** Related Topics ****
     * Documentation_overview
           o Previous: Python_Bindings_for_Oracle_Berkeley_DB_4.8,_5.3,_6.2_and
             18.1
           o Next: DBEnv
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/license.html` & `berkeleydb-18.1.6/docs/html/license.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>LICENSE &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>LICENSE &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="DONATE!" href="donate.html" />
     <link rel="prev" title="Changelog of legacy “bsddb3” project" href="changelog-bsddb3.html" />
    
   <link rel="stylesheet" href="static/custom.css" type="text/css" />
   
@@ -30,25 +28,25 @@
       <div class="documentwrapper">
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="license">
-<h1>LICENSE<a class="headerlink" href="#license" title="Permalink to this headline">¶</a></h1>
+<h1>LICENSE<a class="headerlink" href="#license" title="Permalink to this heading">¶</a></h1>
 <p>Except when noted in individual files, this project is distributed
 under <a class="reference external" href="http://opensource.org/licenses/BSD-3-Clause">BSD 3-Clause License</a>.</p>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>If this file is changed, “LICENSE.txt” and “licenses.txt” must be
 updated too.</p>
 </div>
 <section id="license-text-bsd-3-clause-license">
-<h2>License Text (BSD 3-Clause License)<a class="headerlink" href="#license-text-bsd-3-clause-license" title="Permalink to this headline">¶</a></h2>
-<p>Copyright (c) 2008-2022, Jesus Cea Avion &lt;<a class="reference external" href="mailto:jcea&#37;&#52;&#48;jcea&#46;es">jcea<span>&#64;</span>jcea<span>&#46;</span>es</a>&gt;
+<h2>License Text (BSD 3-Clause License)<a class="headerlink" href="#license-text-bsd-3-clause-license" title="Permalink to this heading">¶</a></h2>
+<p>Copyright (c) 2008-2023, Jesus Cea Avion &lt;<a class="reference external" href="mailto:jcea&#37;&#52;&#48;jcea&#46;es">jcea<span>&#64;</span>jcea<span>&#46;</span>es</a>&gt;
 All rights reserved.</p>
 <p>Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:</p>
 <p>1. Redistributions of source code must retain the above copyright
 notice, this list of conditions and the following disclaimer.</p>
 <p>2. Redistributions in binary form must reproduce the above
@@ -69,25 +67,25 @@
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR
 TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF
 THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
 SUCH DAMAGE.</p>
 </section>
 <section id="license-of-individual-files">
-<h2>License of individual files<a class="headerlink" href="#license-of-individual-files" title="Permalink to this headline">¶</a></h2>
+<h2>License of individual files<a class="headerlink" href="#license-of-individual-files" title="Permalink to this heading">¶</a></h2>
 <p>The history of this project is long and complicated, and so are
 their copyrights and licenses. I (Jesus Cea) wrote this document
 in orden to clarify the situation.</p>
 <p>This code was integrated once in Python 2.x, so I guess somebody
 did the paperwork related to contributor agreement. This code is
 derived from that version, so that could be a license
 checkpoint/blank sheet. I must verify that.</p>
 <p>New files will be covered by the 3-clause BSD license.</p>
 <section id="license-of-python-files">
-<h3>License of Python files<a class="headerlink" href="#license-of-python-files" title="Permalink to this headline">¶</a></h3>
+<h3>License of Python files<a class="headerlink" href="#license-of-python-files" title="Permalink to this heading">¶</a></h3>
 <blockquote>
 <div><ul class="simple">
 <li><p>Except the following files, license is 3-clause BSD license.
 Jesus Cea Avion.</p></li>
 <li><p>test2.py, test3.py: Zope Public License, version 2.0.
 Zope Corporation and contributors.</p></li>
 <li><p>src/berkeleydb/dbrecio.py:
@@ -104,15 +102,15 @@
 Autonomous Zone Industries, Gregory P. Smith.</p></li>
 <li><p>src/berkeleydb/dbshelve.py: Free software.
 Total Control Software.</p></li>
 </ul>
 </div></blockquote>
 </section>
 <section id="license-of-c-files">
-<h3>License of C files<a class="headerlink" href="#license-of-c-files" title="Permalink to this headline">¶</a></h3>
+<h3>License of C files<a class="headerlink" href="#license-of-c-files" title="Permalink to this heading">¶</a></h3>
 <blockquote>
 <div><ul class="simple">
 <li><p>src/Modules/berkeleydb.h, _berkeleydb.c: 3-clause BSD license.
 Digital Creations, Andrew Kuchling, Robin Dunn,
 Gregory P. Smith, Duncan Grisby, Jesus Cea Avion.</p></li>
 </ul>
 </div></blockquote>
@@ -176,32 +174,32 @@
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
 </div>
-<script>$('#searchbox').show(0);</script>
+<script>document.getElementById('searchbox').style.display = "block"</script>
 
 
 
 
 
 
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -2,23 +2,22 @@
 
 
 
 
 
 
 
-
 ****** LICENSEÂ¶ ******
 Except when noted in individual files, this project is distributed under BSD_3-
 Clause_License.
 Note
 If this file is changed, âLICENSE.txtâ and âlicenses.txtâ must be
 updated too.
 ***** License Text (BSD 3-Clause License)Â¶ *****
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es> All rights reserved.
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es> All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 1. Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer.
 2. Redistributions in binary form must reproduce the above copyright notice,
 this list of conditions and the following disclaimer in the documentation and/
 or other materials provided with the distribution.
@@ -91,8 +90,8 @@
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
           o Previous: Changelog_of_legacy_âbsddb3â_project
           o Next: DONATE!
 **** Quick search ****
 [q                   ] [Go]
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/search.html` & `berkeleydb-18.1.6/docs/html/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-
 <!DOCTYPE html>
 
-<html>
+<html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; BerkeleyDB 18.1.5 documentation</title>
+    <title>Search &#8212; BerkeleyDB 18.1.6 documentation</title>
     <link rel="stylesheet" type="text/css" href="static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="static/alabaster.css" />
     
     <script data-url_root="./" id="documentation_options" src="static/documentation_options.js"></script>
-    <script src="static/jquery.js"></script>
-    <script src="static/underscore.js"></script>
     <script src="static/doctools.js"></script>
+    <script src="static/sphinx_highlight.js"></script>
     <script src="static/searchtools.js"></script>
     <script src="static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
   <script src="searchindex.js" defer></script>
   
    
@@ -116,18 +114,18 @@
 
 
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="footer">
-      &copy;2008-2022 Jesús Cea Avión.
+      &copy;2008-2023 Jesús Cea Avión.
       
       |
-      Powered by <a href="http://sphinx-doc.org/">Sphinx 4.4.0</a>
+      Powered by <a href="http://sphinx-doc.org/">Sphinx 7.0.0</a>
       &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
       
     </div>
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
 
 
 
 
 
 
-
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 ****** BerkeleyDB ******
 **** Navigation ****
     * Oracle_Berkeley_DB_4.8,_5.3,_6.2_and_18.1_Python_Extension_Package
@@ -23,8 +22,8 @@
     * History
     * Changelog
     * Changelog_of_legacy_âbsddb3â_project
     * LICENSE
     * DONATE!
 **** Related Topics ****
     * Documentation_overview
-©2008-2022 JesÃºs Cea AviÃ³n. | Powered by Sphinx_4.4.0 & Alabaster_0.7.12
+©2008-2023 JesÃºs Cea AviÃ³n. | Powered by Sphinx_7.0.0 & Alabaster_0.7.12
```

### Comparing `berkeleydb-18.1.5/docs/html/static/alabaster.css` & `berkeleydb-18.1.6/docs/html/static/alabaster.css`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/html/static/basic.css` & `berkeleydb-18.1.6/docs/html/static/basic.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
@@ -218,39 +218,29 @@
     padding: 2px;
     border-collapse: collapse;
 }
 
 /* -- general body styles --------------------------------------------------- */
 
 div.body {
-    min-width: 450px;
+    min-width: 360px;
     max-width: 800px;
 }
 
 div.body p, div.body dd, div.body li, div.body blockquote {
     -moz-hyphens: auto;
     -ms-hyphens: auto;
     -webkit-hyphens: auto;
     hyphens: auto;
 }
 
 a.headerlink {
     visibility: hidden;
 }
 
-a.brackets:before,
-span.brackets > a:before{
-    content: "[";
-}
-
-a.brackets:after,
-span.brackets > a:after {
-    content: "]";
-}
-
 h1:hover > a.headerlink,
 h2:hover > a.headerlink,
 h3:hover > a.headerlink,
 h4:hover > a.headerlink,
 h5:hover > a.headerlink,
 h6:hover > a.headerlink,
 dt:hover > a.headerlink,
@@ -331,20 +321,24 @@
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
 
+nav.contents,
+aside.topic,
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
 
+nav.contents,
+aside.topic,
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -375,21 +369,25 @@
     margin-top: 25px;
 }
 
 /* -- content of sidebars/topics/admonitions -------------------------------- */
 
 div.sidebar > :last-child,
 aside.sidebar > :last-child,
+nav.contents > :last-child,
+aside.topic > :last-child,
 div.topic > :last-child,
 div.admonition > :last-child {
     margin-bottom: 0;
 }
 
 div.sidebar::after,
 aside.sidebar::after,
+nav.contents::after,
+aside.topic::after,
 div.topic::after,
 div.admonition::after,
 blockquote::after {
     display: block;
     content: '';
     clear: both;
 }
@@ -424,18 +422,14 @@
     padding: 1px 8px 1px 5px;
     border-top: 0;
     border-left: 0;
     border-right: 0;
     border-bottom: 1px solid #aaa;
 }
 
-table.footnote td, table.footnote th {
-    border: 0 !important;
-}
-
 th {
     text-align: left;
     padding-right: 5px;
 }
 
 table.citation {
     border-left: solid 1px gray;
@@ -611,27 +605,34 @@
 }
 
 ol.simple p,
 ul.simple p {
     margin-bottom: 0;
 }
 
-dl.footnote > dt,
-dl.citation > dt {
+aside.footnote > span,
+div.citation > span {
     float: left;
-    margin-right: 0.5em;
 }
-
-dl.footnote > dd,
-dl.citation > dd {
+aside.footnote > span:last-of-type,
+div.citation > span:last-of-type {
+  padding-right: 0.5em;
+}
+aside.footnote > p {
+  margin-left: 2em;
+}
+div.citation > p {
+  margin-left: 4em;
+}
+aside.footnote > p:last-of-type,
+div.citation > p:last-of-type {
     margin-bottom: 0em;
 }
-
-dl.footnote > dd:after,
-dl.citation > dd:after {
+aside.footnote > p:last-of-type:after,
+div.citation > p:last-of-type:after {
     content: "";
     clear: both;
 }
 
 dl.field-list {
     display: grid;
     grid-template-columns: fit-content(30%) auto;
@@ -640,18 +641,14 @@
 dl.field-list > dt {
     font-weight: bold;
     word-break: break-word;
     padding-left: 0.5em;
     padding-right: 5px;
 }
 
-dl.field-list > dt:after {
-    content: ":";
-}
-
 dl.field-list > dd {
     padding-left: 0.5em;
     margin-top: 0em;
     margin-left: 0em;
     margin-bottom: 0em;
 }
```

### Comparing `berkeleydb-18.1.5/docs/html/static/pygments.css` & `berkeleydb-18.1.6/docs/html/static/pygments.css`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 .highlight .nl { color: #f57900 } /* Name.Label */
 .highlight .nn { color: #000000 } /* Name.Namespace */
 .highlight .nx { color: #000000 } /* Name.Other */
 .highlight .py { color: #000000 } /* Name.Property */
 .highlight .nt { color: #004461; font-weight: bold } /* Name.Tag */
 .highlight .nv { color: #000000 } /* Name.Variable */
 .highlight .ow { color: #004461; font-weight: bold } /* Operator.Word */
+.highlight .pm { color: #000000; font-weight: bold } /* Punctuation.Marker */
 .highlight .w { color: #f8f8f8; text-decoration: underline } /* Text.Whitespace */
 .highlight .mb { color: #990000 } /* Literal.Number.Bin */
 .highlight .mf { color: #990000 } /* Literal.Number.Float */
 .highlight .mh { color: #990000 } /* Literal.Number.Hex */
 .highlight .mi { color: #990000 } /* Literal.Number.Integer */
 .highlight .mo { color: #990000 } /* Literal.Number.Oct */
 .highlight .sa { color: #4e9a06 } /* Literal.String.Affix */
```

### Comparing `berkeleydb-18.1.5/docs/html/static/searchtools.js` & `berkeleydb-18.1.6/docs/html/static/searchtools.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,554 +1,577 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
+"use strict";
 
-if (!Scorer) {
-    /**
-     * Simple result scoring code.
-     */
+/**
+ * Simple result scoring code.
+ */
+if (typeof Scorer === "undefined") {
     var Scorer = {
         // Implement the following function to further tweak the score for each result
-        // The function takes a result array [filename, title, anchor, descr, score]
+        // The function takes a result array [docname, title, anchor, descr, score, filename]
         // and returns the new score.
         /*
-        score: function(result) {
-          return result[4];
+        score: result => {
+          const [docname, title, anchor, descr, score, filename] = result
+          return score
         },
         */
 
         // query matches the full name of an object
         objNameMatch: 11,
         // or matches in the last dotted part of the object name
         objPartialMatch: 6,
         // Additive scores depending on the priority of the object
         objPrio: {
             0: 15, // used to be importantResults
             1: 5, // used to be objectResults
-            2: -5
-        }, // used to be unimportantResults
+            2: -5, // used to be unimportantResults
+        },
         //  Used when the priority is not in the mapping.
         objPrioDefault: 0,
 
         // query found in title
         title: 15,
         partialTitle: 7,
         // query found in terms
         term: 5,
-        partialTerm: 2
+        partialTerm: 2,
     };
 }
 
-if (!splitQuery) {
-    function splitQuery(query) {
-        return query.split(/\s+/);
+const _removeChildren = (element) => {
+    while (element && element.lastChild) element.removeChild(element.lastChild);
+};
+
+/**
+ * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping
+ */
+const _escapeRegExp = (string) =>
+    string.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&"); // $& means the whole matched string
+
+const _displayItem = (item, searchTerms) => {
+    const docBuilder = DOCUMENTATION_OPTIONS.BUILDER;
+    const docUrlRoot = DOCUMENTATION_OPTIONS.URL_ROOT;
+    const docFileSuffix = DOCUMENTATION_OPTIONS.FILE_SUFFIX;
+    const docLinkSuffix = DOCUMENTATION_OPTIONS.LINK_SUFFIX;
+    const showSearchSummary = DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY;
+
+    const [docName, title, anchor, descr, score, _filename] = item;
+
+    let listItem = document.createElement("li");
+    let requestUrl;
+    let linkUrl;
+    if (docBuilder === "dirhtml") {
+        // dirhtml builder
+        let dirname = docName + "/";
+        if (dirname.match(/\/index\/$/))
+            dirname = dirname.substring(0, dirname.length - 6);
+        else if (dirname === "index/") dirname = "";
+        requestUrl = docUrlRoot + dirname;
+        linkUrl = requestUrl;
+    } else {
+        // normal html builders
+        requestUrl = docUrlRoot + docName + docFileSuffix;
+        linkUrl = docName + docLinkSuffix;
+    }
+    let linkEl = listItem.appendChild(document.createElement("a"));
+    linkEl.href = linkUrl + anchor;
+    linkEl.dataset.score = score;
+    linkEl.innerHTML = title;
+    if (descr)
+        listItem.appendChild(document.createElement("span")).innerHTML =
+        " (" + descr + ")";
+    else if (showSearchSummary)
+        fetch(requestUrl)
+        .then((responseData) => responseData.text())
+        .then((data) => {
+            if (data)
+                listItem.appendChild(
+                    Search.makeSearchSummary(data, searchTerms)
+                );
+        });
+    Search.output.appendChild(listItem);
+};
+const _finishSearch = (resultCount) => {
+    Search.stopPulse();
+    Search.title.innerText = _("Search Results");
+    if (!resultCount)
+        Search.status.innerText = Documentation.gettext(
+            "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
+        );
+    else
+        Search.status.innerText = _(
+            `Search finished, found ${resultCount} page(s) matching the search query.`
+        );
+};
+const _displayNextItem = (
+    results,
+    resultCount,
+    searchTerms
+) => {
+    // results left, load the summary and display it
+    // this is intended to be dynamic (don't sub resultsCount)
+    if (results.length) {
+        _displayItem(results.pop(), searchTerms);
+        setTimeout(
+            () => _displayNextItem(results, resultCount, searchTerms),
+            5
+        );
     }
+    // search finished, update title and status message
+    else _finishSearch(resultCount);
+};
+
+/**
+ * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
+ * custom function per language.
+ *
+ * The regular expression works by splitting the string on consecutive characters
+ * that are not Unicode letters, numbers, underscores, or emoji characters.
+ * This is the same as ``\W+`` in Python, preserving the surrogate pair area.
+ */
+if (typeof splitQuery === "undefined") {
+    var splitQuery = (query) => query
+        .split(/[^\p{Letter}\p{Number}_\p{Emoji_Presentation}]+/gu)
+        .filter(term => term) // remove remaining empty strings
 }
 
 /**
  * Search Module
  */
-var Search = {
-
+const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: function(htmlString) {
-        var virtualDocument = document.implementation.createHTMLDocument('virtual');
-        var htmlElement = $(htmlString, virtualDocument);
-        htmlElement.find('.headerlink').remove();
-        docContent = htmlElement.find('[role=main]')[0];
-        if (docContent === undefined) {
-            console.warn("Content block not found. Sphinx search tries to obtain it " +
-                "via '[role=main]'. Could you check your theme or template.");
-            return "";
-        }
-        return docContent.textContent || docContent.innerText;
+    htmlToText: (htmlString) => {
+        const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
+        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
+            el.remove()
+        });
+        const docContent = htmlElement.querySelector('[role="main"]');
+        if (docContent !== undefined) return docContent.textContent;
+        console.warn(
+            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
+        );
+        return "";
     },
 
-    init: function() {
-        var params = $.getQueryParameters();
-        if (params.q) {
-            var query = params.q[0];
-            $('input[name="q"]')[0].value = query;
-            this.performSearch(query);
-        }
+    init: () => {
+        const query = new URLSearchParams(window.location.search).get("q");
+        document
+            .querySelectorAll('input[name="q"]')
+            .forEach((el) => (el.value = query));
+        if (query) Search.performSearch(query);
     },
 
-    loadIndex: function(url) {
-        $.ajax({
-            type: "GET",
-            url: url,
-            data: null,
-            dataType: "script",
-            cache: true,
-            complete: function(jqxhr, textstatus) {
-                if (textstatus != "success") {
-                    document.getElementById("searchindexloader").src = url;
-                }
-            }
-        });
-    },
+    loadIndex: (url) =>
+        (document.body.appendChild(document.createElement("script")).src = url),
 
-    setIndex: function(index) {
-        var q;
-        this._index = index;
-        if ((q = this._queued_query) !== null) {
-            this._queued_query = null;
-            Search.query(q);
+    setIndex: (index) => {
+        Search._index = index;
+        if (Search._queued_query !== null) {
+            const query = Search._queued_query;
+            Search._queued_query = null;
+            Search.query(query);
         }
     },
 
-    hasIndex: function() {
-        return this._index !== null;
-    },
+    hasIndex: () => Search._index !== null,
 
-    deferQuery: function(query) {
-        this._queued_query = query;
-    },
+    deferQuery: (query) => (Search._queued_query = query),
 
-    stopPulse: function() {
-        this._pulse_status = 0;
-    },
+    stopPulse: () => (Search._pulse_status = -1),
 
-    startPulse: function() {
-        if (this._pulse_status >= 0)
-            return;
+    startPulse: () => {
+        if (Search._pulse_status >= 0) return;
 
-        function pulse() {
-            var i;
+        const pulse = () => {
             Search._pulse_status = (Search._pulse_status + 1) % 4;
-            var dotString = '';
-            for (i = 0; i < Search._pulse_status; i++)
-                dotString += '.';
-            Search.dots.text(dotString);
-            if (Search._pulse_status > -1)
-                window.setTimeout(pulse, 500);
-        }
+            Search.dots.innerText = ".".repeat(Search._pulse_status);
+            if (Search._pulse_status >= 0) window.setTimeout(pulse, 500);
+        };
         pulse();
     },
 
     /**
      * perform a search for something (or wait until index is loaded)
      */
-    performSearch: function(query) {
+    performSearch: (query) => {
         // create the required interface elements
-        this.out = $('#search-results');
-        this.title = $('<h2>' + _('Searching') + '</h2>').appendTo(this.out);
-        this.dots = $('<span></span>').appendTo(this.title);
-        this.status = $('<p class="search-summary">&nbsp;</p>').appendTo(this.out);
-        this.output = $('<ul class="search"/>').appendTo(this.out);
-
-        $('#search-progress').text(_('Preparing search...'));
-        this.startPulse();
+        const searchText = document.createElement("h2");
+        searchText.textContent = _("Searching");
+        const searchSummary = document.createElement("p");
+        searchSummary.classList.add("search-summary");
+        searchSummary.innerText = "";
+        const searchList = document.createElement("ul");
+        searchList.classList.add("search");
+
+        const out = document.getElementById("search-results");
+        Search.title = out.appendChild(searchText);
+        Search.dots = Search.title.appendChild(document.createElement("span"));
+        Search.status = out.appendChild(searchSummary);
+        Search.output = out.appendChild(searchList);
+
+        const searchProgress = document.getElementById("search-progress");
+        // Some themes don't use the search progress node
+        if (searchProgress) {
+            searchProgress.innerText = _("Preparing search...");
+        }
+        Search.startPulse();
 
         // index already loaded, the browser was quick!
-        if (this.hasIndex())
-            this.query(query);
-        else
-            this.deferQuery(query);
+        if (Search.hasIndex()) Search.query(query);
+        else Search.deferQuery(query);
     },
 
     /**
      * execute search (requires search index to be loaded)
      */
-    query: function(query) {
-        var i;
+    query: (query) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
+        // stem the search terms and add them to the correct list
+        const stemmer = new Stemmer();
+        const searchTerms = new Set();
+        const excludedTerms = new Set();
+        const highlightTerms = new Set();
+        const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
+        splitQuery(query.trim()).forEach((queryTerm) => {
+            const queryTermLower = queryTerm.toLowerCase();
 
-        // stem the searchterms and add them to the correct list
-        var stemmer = new Stemmer();
-        var searchterms = [];
-        var excluded = [];
-        var hlterms = [];
-        var tmp = splitQuery(query);
-        var objectterms = [];
-        for (i = 0; i < tmp.length; i++) {
-            if (tmp[i] !== "") {
-                objectterms.push(tmp[i].toLowerCase());
-            }
+            // maybe skip this "word"
+            // stopwords array is from language_data.js
+            if (
+                stopwords.indexOf(queryTermLower) !== -1 ||
+                queryTerm.match(/^\d+$/)
+            )
+                return;
 
-            if ($u.indexOf(stopwords, tmp[i].toLowerCase()) != -1 || tmp[i] === "") {
-                // skip this "word"
-                continue;
-            }
             // stem the word
-            var word = stemmer.stemWord(tmp[i].toLowerCase());
-            // prevent stemmer from cutting word smaller than two chars
-            if (word.length < 3 && tmp[i].length >= 3) {
-                word = tmp[i];
-            }
-            var toAppend;
+            let word = stemmer.stemWord(queryTermLower);
             // select the correct list
-            if (word[0] == '-') {
-                toAppend = excluded;
-                word = word.substr(1);
-            } else {
-                toAppend = searchterms;
-                hlterms.push(tmp[i].toLowerCase());
+            if (word[0] === "-") excludedTerms.add(word.substr(1));
+            else {
+                searchTerms.add(word);
+                highlightTerms.add(queryTermLower);
             }
-            // only add if not already in the list
-            if (!$u.contains(toAppend, word))
-                toAppend.push(word);
-        }
-        var highlightstring = '?highlight=' + $.urlencode(hlterms.join(" "));
+        });
 
-        // console.debug('SEARCH: searching for:');
-        // console.info('required: ', searchterms);
-        // console.info('excluded: ', excluded);
+        if (SPHINX_HIGHLIGHT_ENABLED) { // set in sphinx_highlight.js
+            localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
+        }
 
-        // prepare search
-        var terms = this._index.terms;
-        var titleterms = this._index.titleterms;
+        // console.debug("SEARCH: searching for:");
+        // console.info("required: ", [...searchTerms]);
+        // console.info("excluded: ", [...excludedTerms]);
+
+        // array of [docname, title, anchor, descr, score, filename]
+        let results = [];
+        _removeChildren(document.getElementById("search-progress"));
+
+        const queryLower = query.toLowerCase();
+        for (const [title, foundTitles] of Object.entries(allTitles)) {
+            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+                for (const [file, id] of foundTitles) {
+                    let score = Math.round(100 * queryLower.length / title.length)
+                    results.push([
+                        docNames[file],
+                        titles[file] !== title ? `${titles[file]} > ${title}` : title,
+                        id !== null ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
 
-        // array of [filename, title, anchor, descr, score]
-        var results = [];
-        $('#search-progress').empty();
+        // search for explicit entries in index directives
+        for (const [entry, foundEntries] of Object.entries(indexEntries)) {
+            if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
+                for (const [file, id] of foundEntries) {
+                    let score = Math.round(100 * queryLower.length / entry.length)
+                    results.push([
+                        docNames[file],
+                        titles[file],
+                        id ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
 
         // lookup as object
-        for (i = 0; i < objectterms.length; i++) {
-            var others = [].concat(objectterms.slice(0, i),
-                objectterms.slice(i + 1, objectterms.length));
-            results = results.concat(this.performObjectSearch(objectterms[i], others));
-        }
+        objectTerms.forEach((term) =>
+            results.push(...Search.performObjectSearch(term, objectTerms))
+        );
 
         // lookup as search terms in fulltext
-        results = results.concat(this.performTermsSearch(searchterms, excluded, terms, titleterms));
+        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) {
-            for (i = 0; i < results.length; i++)
-                results[i][4] = Scorer.score(results[i]);
-        }
+        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
 
         // now sort the results by score (in opposite order of appearance, since the
         // display function below uses pop() to retrieve items) and then
         // alphabetically
-        results.sort(function(a, b) {
-            var left = a[4];
-            var right = b[4];
-            if (left > right) {
-                return 1;
-            } else if (left < right) {
-                return -1;
-            } else {
+        results.sort((a, b) => {
+            const leftScore = a[4];
+            const rightScore = b[4];
+            if (leftScore === rightScore) {
                 // same score: sort alphabetically
-                left = a[1].toLowerCase();
-                right = b[1].toLowerCase();
-                return (left > right) ? -1 : ((left < right) ? 1 : 0);
+                const leftTitle = a[1].toLowerCase();
+                const rightTitle = b[1].toLowerCase();
+                if (leftTitle === rightTitle) return 0;
+                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
             }
+            return leftScore > rightScore ? 1 : -1;
         });
 
+        // remove duplicate search results
+        // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
+        let seen = new Set();
+        results = results.reverse().reduce((acc, result) => {
+            let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
+            if (!seen.has(resultStr)) {
+                acc.push(result);
+                seen.add(resultStr);
+            }
+            return acc;
+        }, []);
+
+        results = results.reverse();
+
         // for debugging
         //Search.lastresults = results.slice();  // a copy
-        //console.info('search results:', Search.lastresults);
+        // console.info("search results:", Search.lastresults);
 
         // print the results
-        var resultCount = results.length;
-
-        function displayNextItem() {
-            // results left, load the summary and display it
-            if (results.length) {
-                var item = results.pop();
-                var listItem = $('<li></li>');
-                var requestUrl = "";
-                var linkUrl = "";
-                if (DOCUMENTATION_OPTIONS.BUILDER === 'dirhtml') {
-                    // dirhtml builder
-                    var dirname = item[0] + '/';
-                    if (dirname.match(/\/index\/$/)) {
-                        dirname = dirname.substring(0, dirname.length - 6);
-                    } else if (dirname == 'index/') {
-                        dirname = '';
-                    }
-                    requestUrl = DOCUMENTATION_OPTIONS.URL_ROOT + dirname;
-                    linkUrl = requestUrl;
-
-                } else {
-                    // normal html builders
-                    requestUrl = DOCUMENTATION_OPTIONS.URL_ROOT + item[0] + DOCUMENTATION_OPTIONS.FILE_SUFFIX;
-                    linkUrl = item[0] + DOCUMENTATION_OPTIONS.LINK_SUFFIX;
-                }
-                listItem.append($('<a/>').attr('href',
-                    linkUrl +
-                    highlightstring + item[2]).html(item[1]));
-                if (item[3]) {
-                    listItem.append($('<span> (' + item[3] + ')</span>'));
-                    Search.output.append(listItem);
-                    setTimeout(function() {
-                        displayNextItem();
-                    }, 5);
-                } else if (DOCUMENTATION_OPTIONS.HAS_SOURCE) {
-                    $.ajax({
-                        url: requestUrl,
-                        dataType: "text",
-                        complete: function(jqxhr, textstatus) {
-                            var data = jqxhr.responseText;
-                            if (data !== '' && data !== undefined) {
-                                var summary = Search.makeSearchSummary(data, searchterms, hlterms);
-                                if (summary) {
-                                    listItem.append(summary);
-                                }
-                            }
-                            Search.output.append(listItem);
-                            setTimeout(function() {
-                                displayNextItem();
-                            }, 5);
-                        }
-                    });
-                } else {
-                    // no source available, just display title
-                    Search.output.append(listItem);
-                    setTimeout(function() {
-                        displayNextItem();
-                    }, 5);
-                }
-            }
-            // search finished, update title and status message
-            else {
-                Search.stopPulse();
-                Search.title.text(_('Search Results'));
-                if (!resultCount)
-                    Search.status.text(_('Your search did not match any documents. Please make sure that all words are spelled correctly and that you\'ve selected enough categories.'));
-                else
-                    Search.status.text(_('Search finished, found %s page(s) matching the search query.').replace('%s', resultCount));
-                Search.status.fadeIn(500);
-            }
-        }
-        displayNextItem();
+        _displayNextItem(results, results.length, searchTerms);
     },
 
     /**
      * search for object names
      */
-    performObjectSearch: function(object, otherterms) {
-        var filenames = this._index.filenames;
-        var docnames = this._index.docnames;
-        var objects = this._index.objects;
-        var objnames = this._index.objnames;
-        var titles = this._index.titles;
-
-        var i;
-        var results = [];
-
-        for (var prefix in objects) {
-            for (var iMatch = 0; iMatch != objects[prefix].length; ++iMatch) {
-                var match = objects[prefix][iMatch];
-                var name = match[4];
-                var fullname = (prefix ? prefix + '.' : '') + name;
-                var fullnameLower = fullname.toLowerCase()
-                if (fullnameLower.indexOf(object) > -1) {
-                    var score = 0;
-                    var parts = fullnameLower.split('.');
-                    // check for different match types: exact matches of full name or
-                    // "last name" (i.e. last dotted part)
-                    if (fullnameLower == object || parts[parts.length - 1] == object) {
-                        score += Scorer.objNameMatch;
-                        // matches in last name
-                    } else if (parts[parts.length - 1].indexOf(object) > -1) {
-                        score += Scorer.objPartialMatch;
-                    }
-                    var objname = objnames[match[1]][2];
-                    var title = titles[match[0]];
-                    // If more than one term searched for, we require other words to be
-                    // found in the name/title/description
-                    if (otherterms.length > 0) {
-                        var haystack = (prefix + ' ' + name + ' ' +
-                            objname + ' ' + title).toLowerCase();
-                        var allfound = true;
-                        for (i = 0; i < otherterms.length; i++) {
-                            if (haystack.indexOf(otherterms[i]) == -1) {
-                                allfound = false;
-                                break;
-                            }
-                        }
-                        if (!allfound) {
-                            continue;
-                        }
-                    }
-                    var descr = objname + _(', in ') + title;
-
-                    var anchor = match[3];
-                    if (anchor === '')
-                        anchor = fullname;
-                    else if (anchor == '-')
-                        anchor = objnames[match[1]][1] + '-' + fullname;
-                    // add custom score for some objects according to scorer
-                    if (Scorer.objPrio.hasOwnProperty(match[2])) {
-                        score += Scorer.objPrio[match[2]];
-                    } else {
-                        score += Scorer.objPrioDefault;
-                    }
-                    results.push([docnames[match[0]], fullname, '#' + anchor, descr, score, filenames[match[0]]]);
-                }
-            }
-        }
-
+    performObjectSearch: (object, objectTerms) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const objects = Search._index.objects;
+        const objNames = Search._index.objnames;
+        const titles = Search._index.titles;
+
+        const results = [];
+
+        const objectSearchCallback = (prefix, match) => {
+            const name = match[4]
+            const fullname = (prefix ? prefix + "." : "") + name;
+            const fullnameLower = fullname.toLowerCase();
+            if (fullnameLower.indexOf(object) < 0) return;
+
+            let score = 0;
+            const parts = fullnameLower.split(".");
+
+            // check for different match types: exact matches of full name or
+            // "last name" (i.e. last dotted part)
+            if (fullnameLower === object || parts.slice(-1)[0] === object)
+                score += Scorer.objNameMatch;
+            else if (parts.slice(-1)[0].indexOf(object) > -1)
+                score += Scorer.objPartialMatch; // matches in last name
+
+            const objName = objNames[match[1]][2];
+            const title = titles[match[0]];
+
+            // If more than one term searched for, we require other words to be
+            // found in the name/title/description
+            const otherTerms = new Set(objectTerms);
+            otherTerms.delete(object);
+            if (otherTerms.size > 0) {
+                const haystack = `${prefix} ${name} ${objName} ${title}`.toLowerCase();
+                if (
+                    [...otherTerms].some((otherTerm) => haystack.indexOf(otherTerm) < 0)
+                )
+                    return;
+            }
+
+            let anchor = match[3];
+            if (anchor === "") anchor = fullname;
+            else if (anchor === "-") anchor = objNames[match[1]][1] + "-" + fullname;
+
+            const descr = objName + _(", in ") + title;
+
+            // add custom score for some objects according to scorer
+            if (Scorer.objPrio.hasOwnProperty(match[2]))
+                score += Scorer.objPrio[match[2]];
+            else score += Scorer.objPrioDefault;
+
+            results.push([
+                docNames[match[0]],
+                fullname,
+                "#" + anchor,
+                descr,
+                score,
+                filenames[match[0]],
+            ]);
+        };
+        Object.keys(objects).forEach((prefix) =>
+            objects[prefix].forEach((array) =>
+                objectSearchCallback(prefix, array)
+            )
+        );
         return results;
     },
 
     /**
-     * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions
-     */
-    escapeRegExp: function(string) {
-        return string.replace(/[.*+\-?^${}()|[\]\\]/g, '\\$&'); // $& means the whole matched string
-    },
-
-    /**
      * search for full-text terms in the index
      */
-    performTermsSearch: function(searchterms, excluded, terms, titleterms) {
-        var docnames = this._index.docnames;
-        var filenames = this._index.filenames;
-        var titles = this._index.titles;
-
-        var i, j, file;
-        var fileMap = {};
-        var scoreMap = {};
-        var results = [];
+    performTermsSearch: (searchTerms, excludedTerms) => {
+        // prepare search
+        const terms = Search._index.terms;
+        const titleTerms = Search._index.titleterms;
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+
+        const scoreMap = new Map();
+        const fileMap = new Map();
 
         // perform the search on the required terms
-        for (i = 0; i < searchterms.length; i++) {
-            var word = searchterms[i];
-            var files = [];
-            var _o = [{
+        searchTerms.forEach((word) => {
+            const files = [];
+            const arr = [{
                 files: terms[word],
                 score: Scorer.term
             }, {
-                files: titleterms[word],
+                files: titleTerms[word],
                 score: Scorer.title
-            }];
+            }, ];
             // add support for partial matches
             if (word.length > 2) {
-                var word_regex = this.escapeRegExp(word);
-                for (var w in terms) {
-                    if (w.match(word_regex) && !terms[word]) {
-                        _o.push({
-                            files: terms[w],
+                const escapedWord = _escapeRegExp(word);
+                Object.keys(terms).forEach((term) => {
+                    if (term.match(escapedWord) && !terms[word])
+                        arr.push({
+                            files: terms[term],
                             score: Scorer.partialTerm
-                        })
-                    }
-                }
-                for (var w in titleterms) {
-                    if (w.match(word_regex) && !titleterms[word]) {
-                        _o.push({
-                            files: titleterms[w],
+                        });
+                });
+                Object.keys(titleTerms).forEach((term) => {
+                    if (term.match(escapedWord) && !titleTerms[word])
+                        arr.push({
+                            files: titleTerms[word],
                             score: Scorer.partialTitle
-                        })
-                    }
-                }
+                        });
+                });
             }
 
             // no match but word was a required one
-            if ($u.every(_o, function(o) {
-                    return o.files === undefined;
-                })) {
-                break;
-            }
+            if (arr.every((record) => record.files === undefined)) return;
+
             // found search word in contents
-            $u.each(_o, function(o) {
-                var _files = o.files;
-                if (_files === undefined)
-                    return
-
-                if (_files.length === undefined)
-                    _files = [_files];
-                files = files.concat(_files);
-
-                // set score for the word in each file to Scorer.term
-                for (j = 0; j < _files.length; j++) {
-                    file = _files[j];
-                    if (!(file in scoreMap))
-                        scoreMap[file] = {};
-                    scoreMap[file][word] = o.score;
-                }
+            arr.forEach((record) => {
+                if (record.files === undefined) return;
+
+                let recordFiles = record.files;
+                if (recordFiles.length === undefined) recordFiles = [recordFiles];
+                files.push(...recordFiles);
+
+                // set score for the word in each file
+                recordFiles.forEach((file) => {
+                    if (!scoreMap.has(file)) scoreMap.set(file, {});
+                    scoreMap.get(file)[word] = record.score;
+                });
             });
 
             // create the mapping
-            for (j = 0; j < files.length; j++) {
-                file = files[j];
-                if (file in fileMap && fileMap[file].indexOf(word) === -1)
-                    fileMap[file].push(word);
-                else
-                    fileMap[file] = [word];
-            }
-        }
+            files.forEach((file) => {
+                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
+                    fileMap.get(file).push(word);
+                else fileMap.set(file, [word]);
+            });
+        });
 
         // now check if the files don't contain excluded terms
-        for (file in fileMap) {
-            var valid = true;
-
+        const results = [];
+        for (const [file, wordList] of fileMap) {
             // check if all requirements are matched
-            var filteredTermCount = // as search terms with length < 3 are discarded: ignore
-                searchterms.filter(function(term) {
-                    return term.length > 2
-                }).length
+
+            // as search terms with length < 3 are discarded
+            const filteredTermCount = [...searchTerms].filter(
+                (term) => term.length > 2
+            ).length;
             if (
-                fileMap[file].length != searchterms.length &&
-                fileMap[file].length != filteredTermCount
-            ) continue;
+                wordList.length !== searchTerms.size &&
+                wordList.length !== filteredTermCount
+            )
+                continue;
 
             // ensure that none of the excluded terms is in the search result
-            for (i = 0; i < excluded.length; i++) {
-                if (terms[excluded[i]] == file ||
-                    titleterms[excluded[i]] == file ||
-                    $u.contains(terms[excluded[i]] || [], file) ||
-                    $u.contains(titleterms[excluded[i]] || [], file)) {
-                    valid = false;
-                    break;
-                }
-            }
+            if (
+                [...excludedTerms].some(
+                    (term) =>
+                    terms[term] === file ||
+                    titleTerms[term] === file ||
+                    (terms[term] || []).includes(file) ||
+                    (titleTerms[term] || []).includes(file)
+                )
+            )
+                break;
 
-            // if we have still a valid result we can add it to the result list
-            if (valid) {
-                // select one (max) score for the file.
-                // for better ranking, we should calculate ranking by using words statistics like basic tf-idf...
-                var score = $u.max($u.map(fileMap[file], function(w) {
-                    return scoreMap[file][w]
-                }));
-                results.push([docnames[file], titles[file], '', null, score, filenames[file]]);
-            }
+            // select one (max) score for the file.
+            const score = Math.max(...wordList.map((w) => scoreMap.get(file)[w]));
+            // add result to the result list
+            results.push([
+                docNames[file],
+                titles[file],
+                "",
+                null,
+                score,
+                filenames[file],
+            ]);
         }
         return results;
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
-     * of stemmed words, hlwords is the list of normal, unstemmed
-     * words. the first one is used to find the occurrence, the
-     * latter for highlighting it.
+     * of stemmed words.
      */
-    makeSearchSummary: function(htmlText, keywords, hlwords) {
-        var text = Search.htmlToText(htmlText);
-        if (text == "") {
-            return null;
-        }
-        var textLower = text.toLowerCase();
-        var start = 0;
-        $.each(keywords, function() {
-            var i = textLower.indexOf(this.toLowerCase());
-            if (i > -1)
-                start = i;
-        });
-        start = Math.max(start - 120, 0);
-        var excerpt = ((start > 0) ? '...' : '') +
-            $.trim(text.substr(start, 240)) +
-            ((start + 240 - text.length) ? '...' : '');
-        var rv = $('<p class="context"></p>').text(excerpt);
-        $.each(hlwords, function() {
-            rv = rv.highlightText(this, 'highlighted');
-        });
-        return rv;
-    }
+    makeSearchSummary: (htmlText, keywords) => {
+        const text = Search.htmlToText(htmlText);
+        if (text === "") return null;
+
+        const textLower = text.toLowerCase();
+        const actualStartPosition = [...keywords]
+            .map((k) => textLower.indexOf(k.toLowerCase()))
+            .filter((i) => i > -1)
+            .slice(-1)[0];
+        const startWithContext = Math.max(actualStartPosition - 120, 0);
+
+        const top = startWithContext === 0 ? "" : "...";
+        const tail = startWithContext + 240 < text.length ? "..." : "";
+
+        let summary = document.createElement("p");
+        summary.classList.add("context");
+        summary.textContent = top + text.substr(startWithContext, 240).trim() + tail;
+
+        return summary;
+    },
 };
 
-$(document).ready(function() {
-    Search.init();
-});
+_ready(Search.init);
```

### Comparing `berkeleydb-18.1.5/docs/index.rst` & `berkeleydb-18.1.6/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 The Python wrappers allow you to store Python string objects of any
 length, keyed either by strings or integers depending on the database
 access method. With the use of another module in the package standard
 shelve-like functionality is provided allowing you to store any
 picklable Python object!
 
 Oracle Berkeley DB is very powerful and versatile, but it is complex to
-use correctly. :Oracle:`Oracle documentation <toc.htm>` is very
+use correctly. :Oracle:`Oracle documentation <index.html>` is very
 complete. Please, review it.
 
 Since June 2013 (release 6.0.0), this project accepts donations. Please,
 contribute if you can. :doc:`Details <donate>`.
 
 Documentation Index
 -------------------
```

### Comparing `berkeleydb-18.1.5/docs/introduction.rst` & `berkeleydb-18.1.6/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/docs/license.rst` & `berkeleydb-18.1.6/docs/license.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
  If this file is changed, "LICENSE.txt" and "licenses.txt" must be
  updated too.
 
 License Text (BSD 3-Clause License)
 -----------------------------------
 
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/licenses.txt` & `berkeleydb-18.1.6/licenses.txt`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/setup.py` & `berkeleydb-18.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/setup3.py` & `berkeleydb-18.1.6/setup3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/src/Module/berkeleydb.c` & `berkeleydb-18.1.6/src/Module/berkeleydb.c`

 * *Files 1% similar despite different names*

```diff
@@ -9650,118 +9650,80 @@
 ** We can rename the module at import time, so the string allocated
 ** must be big enough, and any use of the name must use this particular
 ** string.
 */
 #define MODULE_NAME_MAX_LEN     32
 static char _berkeleydbModuleName[MODULE_NAME_MAX_LEN+1] = "_berkeleydb";
 
-static struct PyModuleDef berkeleydbmodule = {
-    PyModuleDef_HEAD_INIT,
-    _berkeleydbModuleName,   /* Name of module */
-    NULL,               /* module documentation, may be NULL */
-    -1,                 /* size of per-interpreter state of the module,
-                            or -1 if the module keeps state in global variables. */
-    berkeleydb_methods,
-    NULL,   /* Reload */
-    NULL,   /* Traverse */
-    NULL,   /* Clear */
-    NULL    /* Free */
-};
-
 
-PyMODINIT_FUNC  PyInit__berkeleydb(void)    /* Note the two underscores */
+static int berkeleydb_exec(PyObject *m)
 {
-    PyObject* m;
     PyObject* d;
     PyTypeObject* type;
     PyObject* py_api;
     PyObject* py_berkeleydb_version_s;
     PyObject* db_version_s;
 
     strncpy(_berkeleydbModuleName, "_berkeleydb", MODULE_NAME_MAX_LEN);
 
-    /*
-     * Python 3.7 and newer ALWAYS initialize the GIL.
-     * https://vstinner.github.io/python37-gil-change.html
-     */
-#if (PY_VERSION_HEX < 0x03070000)
-    /* PyEval_InitThreads is called here due to a quirk in python 1.5
-     * - 2.2.1 (at least) according to Russell Williamson <merel@wt.net>:
-     * The global interpreter lock is not initialized until the first
-     * thread is created using thread.start_new_thread() or fork() is
-     * called.  that would cause the ALLOW_THREADS here to segfault due
-     * to a null pointer reference if no threads or child processes
-     * have been created.  This works around that and is a no-op if
-     * threads have already been initialized.
-     *  (see pybsddb-users mailing list post on 2002-08-07)
-     */
-    PyEval_InitThreads();
-#endif
-
     /* This data should be ascii, so UTF-8 conversion is fine */
     py_berkeleydb_version_s = PyUnicode_FromString(PY_BERKELEYDB_VERSION);
     db_version_s = PyUnicode_FromString(DB_VERSION_STRING);
 
     /* Initialize object types */
     type = (PyTypeObject *)PyType_FromSpec(&DBEnv_Type_spec);
     if (type == NULL)
-        return NULL;
+        return -1;
     /* tp_new is used in this type */
     DBEnv_Type = type;
 
     type = (PyTypeObject *)PyType_FromSpec(&DB_Type_spec);
     if (type == NULL)
-        return NULL;
+        return -1;
     /* tp_new is used in this type */
     DB_Type = type;
 
     type = (PyTypeObject *)PyType_FromSpec(&DBTxn_Type_spec);
     if (type == NULL)
-        return NULL;
+        return -1;
     type->tp_new = NULL;
     DBTxn_Type = type;
 
     type = (PyTypeObject *)PyType_FromSpec(&DBCursor_Type_spec);
     if (type == NULL)
-        return NULL;
+        return -1;
     type->tp_new = NULL;
     DBCursor_Type = type;
 
     type = (PyTypeObject *)PyType_FromSpec(&DBLogCursor_Type_spec);
     if (type == NULL)
-        return NULL;
+        return -1;
     type->tp_new = NULL;
     DBLogCursor_Type = type;
 
     type = (PyTypeObject *)PyType_FromSpec(&DBLock_Type_spec);
     if (type == NULL)
-        return NULL;
+        return -1;
     type->tp_new = NULL;
     DBLock_Type = type;
 
     type = (PyTypeObject *)PyType_FromSpec(&DBSequence_Type_spec);
     if (type == NULL)
-        return NULL;
+        return -1;
     /* tp_new is used in this type */
     DBSequence_Type = type;
 
 #if (DBVER >= 53)
     type = (PyTypeObject *)PyType_FromSpec(&DBSite_Type_spec);
     if (type == NULL)
-        return NULL;
+        return -1;
     type->tp_new = NULL;
     DBSite_Type = type;
 #endif
 
-    /* Create the module and add the functions */
-    m=PyModule_Create(&berkeleydbmodule);
-    if (m == NULL) {
-        return NULL;
-    }
-
     /* Add some symbolic constants to the module */
     d = PyModule_GetDict(m);
     PyDict_SetItemString(d, "__version__", py_berkeleydb_version_s);
     PyDict_SetItemString(d, "DB_VERSION_STRING", db_version_s);
     Py_DECREF(py_berkeleydb_version_s);
     py_berkeleydb_version_s = NULL;
     Py_DECREF(db_version_s);
@@ -10356,12 +10318,35 @@
     }
 
 error:
     /* Check for errors */
     if (PyErr_Occurred()) {
         PyErr_Print();
         Py_FatalError("can't initialize module _berkeleydb");
-        Py_DECREF(m);
-        m = NULL;
+        return -1;
     }
-    return m;
+    return 0;
+}
+
+static PyModuleDef_Slot berkeleydb_slots[] = {
+    {Py_mod_exec, berkeleydb_exec},
+    {0, NULL}
+};
+
+static PyModuleDef berkeleydb_def = {
+    PyModuleDef_HEAD_INIT,      /* m_base */
+    _berkeleydbModuleName,      /* m_name - Name of module */
+    NULL,                       /* m_doc - module documentation, may be NULL */
+    0,                          /* m_size -
+                                   size of per-interpreter state of the module,
+                                */
+    berkeleydb_methods,         /* m_methods */
+    berkeleydb_slots,           /* m_slots */
+    NULL,                       /* m_traverse */
+    NULL,                       /* m_clear */
+    NULL                        /* m_free */
+};
+
+PyMODINIT_FUNC  PyInit__berkeleydb(void)    /* Note the two underscores */
+{
+    return PyModuleDef_Init(&berkeleydb_def);
 }
```

### Comparing `berkeleydb-18.1.5/src/Module/berkeleydb.h` & `berkeleydb-18.1.6/src/Module/berkeleydb.h`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 /* 40 = 4.0, 33 = 3.3; this will break if the minor revision is > 9 */
 #define DBVER (DB_VERSION_MAJOR * 10 + DB_VERSION_MINOR)
 #if DB_VERSION_MINOR > 9
 #error "eek! DBVER can't handle minor versions > 9"
 #endif
 
-#define PY_BERKELEYDB_VERSION "18.1.5"
+#define PY_BERKELEYDB_VERSION "18.1.6"
 
 /* Python object definitions */
 
 struct behaviourFlags {
     /* What is the default behaviour when DB->get or DBCursor->get returns a
        DB_NOTFOUND || DB_KEYEMPTY error?  Return None or raise an exception? */
     unsigned int getReturnsNone : 1;
```

### Comparing `berkeleydb-18.1.5/src/berkeleydb/__init__.py` & `berkeleydb-18.1.6/src/berkeleydb/__init__.py`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/src/berkeleydb/db.py` & `berkeleydb-18.1.6/src/berkeleydb/db.py`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/src/berkeleydb/dbobj.py` & `berkeleydb-18.1.6/src/berkeleydb/dbobj.py`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/src/berkeleydb/dbrecio.py` & `berkeleydb-18.1.6/src/berkeleydb/dbrecio.py`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/src/berkeleydb/dbshelve.py` & `berkeleydb-18.1.6/src/berkeleydb/dbshelve.py`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/src/berkeleydb/dbutils.py` & `berkeleydb-18.1.6/src/berkeleydb/dbutils.py`

 * *Files identical despite different names*

### Comparing `berkeleydb-18.1.5/test-full_prerelease.py` & `berkeleydb-18.1.6/test-full_prerelease.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
 1. Redistributions of source code must retain the above copyright
@@ -50,15 +50,15 @@
 import sys
 import os
 
 # We need to be able to test BDB releases, even if the license is incompatible
 os.environ['YES_I_HAVE_THE_RIGHT_TO_USE_THIS_BERKELEY_DB_VERSION'] = ''
 
 def do_matrix_check() :
-  python_versions = ('3.7', '3.8', '3.9', '3.10', '3.11')
+  python_versions = ('3.7', '3.8', '3.9', '3.10', '3.11', '3.12')
 
   berkeleydb_versions=('4.8', '5.3', '6.2', '18.1')
 
   warning_level=("-Wdefault", "-Werror")[1]
 
   for py in python_versions :
     for bdb in berkeleydb_versions :
```

### Comparing `berkeleydb-18.1.5/test.py` & `berkeleydb-18.1.6/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,21 +135,29 @@
 import traceback
 import pathlib
 
 from unittest import TextTestResult
 
 from sysconfig import get_platform
 
+import setuptools
+import pkg_resources
+
 # We need to be able to test BDB releases, even if the license is incompatible
 os.environ['YES_I_HAVE_THE_RIGHT_TO_USE_THIS_BERKELEY_DB_VERSION'] = ''
 
 
 PROGRAM = sys.argv[0]
-version = sys.version_info
-PLAT_SPEC = f'{get_platform()}-{version.major}.{version.minor}'
+min_version = pkg_resources.parse_version('62.1.0')
+if pkg_resources.parse_version(setuptools.__version__) >= min_version:
+    PLAT_SPEC = f'{get_platform()}-{sys.implementation.cache_tag}'
+else:
+    version = sys.version_info
+    PLAT_SPEC = f'{get_platform()}-{version.major}.{version.minor}'
+
 # This hack copied from distutils.command.build.  Too bad distutils
 # doesn't export its build/ directory naming scheme as a library function.
 if hasattr(sys, 'gettotalrefcount'):
     PLAT_SPEC += '-pydebug'
 
 class ImmediateTestResult(TextTestResult):
 
@@ -267,14 +275,15 @@
 class PathInit:
     def __init__(self):
         self.libdir = 'lib.%s' % PLAT_SPEC
         os.chdir('build')
         # Hack sys.path
         self.cwd = os.getcwd()
         sys.path[0] = os.path.join(self.cwd, self.libdir)
+        os.environ['BERKELEYDB_SO_PATH'] = sys.path[0]
 
 
 def match(rx, s):
     if not rx:
         return True
     if rx[0] == '!':
         return re.search(rx[1:], s) is None
```

### Comparing `berkeleydb-18.1.5/tests/test_all.py` & `berkeleydb-18.1.6/tests/test_all.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
@@ -75,22 +75,22 @@
     print('berkeleydb.db.version():   %s' % (db.version(), ))
     if db.version() >= (5, 3) :
         print('berkeleydb.db.full_version(): %s' %repr(db.full_version()))
     print('berkeleydb.db.__version__: %s' % db.__version__)
 
     # Workaround for allowing generating an EGGs as a ZIP files.
     suffix="__"
-    print('py module:            %s' % getattr(berkeleydb, "__file"+suffix))
-    print('extension module:     %s' % getattr(berkeleydb, "__file"+suffix))
+    print('py module:           %s' % getattr(berkeleydb, "__file"+suffix))
+    print('extension module:    %s' % getattr(berkeleydb._db, "__file"+suffix))
 
-    print('Test working dir:     %s' % get_test_path_prefix())
-    print('python version:       %s %s' % \
+    print('Test working dir:    %s' % get_test_path_prefix())
+    print('python version:      %s %s' % \
             (sys.version.replace("\r", "").replace("\n", ""), \
             platform.architecture()[0]))
-    print('My pid:               %s' % os.getpid())
+    print('My pid:              %s' % os.getpid())
     print('-=' * 38)
 
 
 def get_new_path(name) :
     get_new_path.mutex.acquire()
     try :
         path=os.path.join(get_new_path.prefix,
@@ -144,14 +144,28 @@
 printable_bytes = [i.encode('ascii') for i in string.printable]
 
 
 class PrintInfoFakeTest(unittest.TestCase):
     def testPrintVersions(self):
         print_versions()
 
+class pathTest(unittest.TestCase):
+    def test_path(self):
+        path_dir = pathlib.Path(os.environ.get('BERKELEYDB_SO_PATH', None))
+        self.assertIsNotNone(path_dir)
+        path_dir = path_dir.resolve()
+        path_file = pathlib.Path(berkeleydb._db.__file__).resolve()
+        if sys.version_info >= (3, 9):
+            self.assertTrue(path_file.is_relative_to(path_dir),
+                    msg=f"Wrong library: '{path_file}' not in '{path_dir}'")
+        else:
+            path_dir = path_dir.as_posix()
+            path_file = path_file.as_posix()
+            self.assertEqual(path_dir, path_file[:len(path_dir)])
+
 
 def suite(module_prefix='', timing_check=None):
     test_modules = [
         'test_associate',
         'test_basics',
         'test_dbenv',
         'test_db',
@@ -191,15 +205,15 @@
                                                             timing_check)
             alltests.addTest(test)
     return alltests
 
 
 def test_suite():
     suite = unittest.TestSuite()
-    for test in (PrintInfoFakeTest,):
+    for test in (PrintInfoFakeTest, pathTest):
         test = unittest.defaultTestLoader.loadTestsFromTestCase(test)
         suite.addTest(test)
     return suite
 
 
 if __name__ == '__main__':
     print_versions()
```

### Comparing `berkeleydb-18.1.5/tests/test_associate.py` & `berkeleydb-18.1.6/tests/test_associate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_basics.py` & `berkeleydb-18.1.6/tests/test_basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_compare.py` & `berkeleydb-18.1.6/tests/test_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_compat.py` & `berkeleydb-18.1.6/tests/test_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_concurrent_data_store.py` & `berkeleydb-18.1.6/tests/test_concurrent_data_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_cursor_pget_bug.py` & `berkeleydb-18.1.6/tests/test_cursor_pget_bug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_db.py` & `berkeleydb-18.1.6/tests/test_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_dbenv.py` & `berkeleydb-18.1.6/tests/test_dbenv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_dbobj.py` & `berkeleydb-18.1.6/tests/test_dbobj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_dbshelve.py` & `berkeleydb-18.1.6/tests/test_dbshelve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_distributed_transactions.py` & `berkeleydb-18.1.6/tests/test_distributed_transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_early_close.py` & `berkeleydb-18.1.6/tests/test_early_close.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_fileid.py` & `berkeleydb-18.1.6/tests/test_fileid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_get_none.py` & `berkeleydb-18.1.6/tests/test_get_none.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_heap.py` & `berkeleydb-18.1.6/tests/test_heap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_join.py` & `berkeleydb-18.1.6/tests/test_join.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_lock.py` & `berkeleydb-18.1.6/tests/test_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_misc.py` & `berkeleydb-18.1.6/tests/test_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_pickle.py` & `berkeleydb-18.1.6/tests/test_pickle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_queue.py` & `berkeleydb-18.1.6/tests/test_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_recno.py` & `berkeleydb-18.1.6/tests/test_recno.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_replication.py` & `berkeleydb-18.1.6/tests/test_replication.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_sequence.py` & `berkeleydb-18.1.6/tests/test_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_thread.py` & `berkeleydb-18.1.6/tests/test_thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

### Comparing `berkeleydb-18.1.5/tests/test_weakref.py` & `berkeleydb-18.1.6/tests/test_weakref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2008-2022, Jesus Cea Avion <jcea@jcea.es>
+Copyright (c) 2008-2023, Jesus Cea Avion <jcea@jcea.es>
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
     1. Redistributions of source code must retain the above copyright
```

