# Comparing `tmp/sftpretty-1.0.8.tar.gz` & `tmp/sftpretty-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sftpretty-1.0.8.tar", last modified: Fri Mar  3 16:08:10 2023, max compression
+gzip compressed data, was "sftpretty-1.0.9.tar", last modified: Tue May  9 23:49:50 2023, max compression
```

## Comparing `sftpretty-1.0.8.tar` & `sftpretty-1.0.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:08:10.787889 sftpretty-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-03 16:07:53.000000 sftpretty-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-03 16:07:53.000000 sftpretty-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-03-03 16:08:10.787889 sftpretty-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-03-03 16:07:53.000000 sftpretty-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:08:10.775889 sftpretty-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-03 16:07:53.000000 sftpretty-1.0.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-03 16:07:53.000000 sftpretty-1.0.8/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-03-03 16:07:53.000000 sftpretty-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-03-03 16:07:53.000000 sftpretty-1.0.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16510 2023-03-03 16:07:53.000000 sftpretty-1.0.8/docs/cookbook.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-03 16:07:53.000000 sftpretty-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-03 16:07:53.000000 sftpretty-1.0.8/docs/sftpretty.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-03 16:07:53.000000 sftpretty-1.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 16:08:10.787889 sftpretty-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-03 16:07:53.000000 sftpretty-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:08:10.775889 sftpretty-1.0.8/sftpretty/
--rw-r--r--   0 runner    (1001) docker     (123)    56790 2023-03-03 16:07:53.000000 sftpretty-1.0.8/sftpretty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-03 16:07:53.000000 sftpretty-1.0.8/sftpretty/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-03-03 16:07:53.000000 sftpretty-1.0.8/sftpretty/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:08:10.775889 sftpretty-1.0.8/sftpretty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-03-03 16:08:10.000000 sftpretty-1.0.8/sftpretty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-03 16:08:10.000000 sftpretty-1.0.8/sftpretty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 16:08:10.000000 sftpretty-1.0.8/sftpretty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-03 16:08:10.000000 sftpretty-1.0.8/sftpretty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-03 16:08:10.000000 sftpretty-1.0.8/sftpretty.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 16:08:10.787889 sftpretty-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_chdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_chown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_ciphers.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_get_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_get_r.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_getcwd.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_getfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_is.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_issue_65.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_issue_xx.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_listdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_localtree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_mkdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_pep8.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_put.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_put_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_put_r.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_putfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_readlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_remote_server_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_remotetree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_rmdir.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_security_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_stat_lstat.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_truncate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-03 16:07:53.000000 sftpretty-1.0.8/tests/test_username.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:49:50.172850 sftpretty-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-09 23:49:37.000000 sftpretty-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-09 23:49:37.000000 sftpretty-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-09 23:49:50.172850 sftpretty-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-09 23:49:37.000000 sftpretty-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:49:50.156849 sftpretty-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 23:49:37.000000 sftpretty-1.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-09 23:49:37.000000 sftpretty-1.0.9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-05-09 23:49:37.000000 sftpretty-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-09 23:49:37.000000 sftpretty-1.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-05-09 23:49:37.000000 sftpretty-1.0.9/docs/cookbook.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-05-09 23:49:37.000000 sftpretty-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 23:49:37.000000 sftpretty-1.0.9/docs/sftpretty.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 23:49:37.000000 sftpretty-1.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 23:49:50.172850 sftpretty-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-09 23:49:37.000000 sftpretty-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:49:50.160849 sftpretty-1.0.9/sftpretty/
+-rw-r--r--   0 runner    (1001) docker     (123)    56862 2023-05-09 23:49:37.000000 sftpretty-1.0.9/sftpretty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-09 23:49:37.000000 sftpretty-1.0.9/sftpretty/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-05-09 23:49:37.000000 sftpretty-1.0.9/sftpretty/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:49:50.160849 sftpretty-1.0.9/sftpretty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-09 23:49:50.000000 sftpretty-1.0.9/sftpretty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-09 23:49:50.000000 sftpretty-1.0.9/sftpretty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 23:49:50.000000 sftpretty-1.0.9/sftpretty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 23:49:50.000000 sftpretty-1.0.9/sftpretty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 23:49:50.000000 sftpretty-1.0.9/sftpretty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 23:49:50.172850 sftpretty-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_chdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_chown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_ciphers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_get_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_get_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_getcwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_getfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_is.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_issue_65.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_issue_xx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_listdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_localtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_pep8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_put.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_put_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_put_r.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_putfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_readlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_remote_server_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_remotetree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_rmdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_security_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_stat_lstat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_truncate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-09 23:49:37.000000 sftpretty-1.0.9/tests/test_username.py
```

### Comparing `sftpretty-1.0.8/LICENSE` & `sftpretty-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/PKG-INFO` & `sftpretty-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpretty
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pretty secure file transfer made easy.
 Home-page: https://github.com/byteskeptical/sftpretty
 Download-URL: https://pypi.python.org/pypi/sftpretty
 Author: byteskeptical
 Author-email: 40208858+byteskeptical@users.noreply.github.com
 License: BSD
 Keywords: ftp scp sftp ssh
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sftpretty
 =========
 
@@ -120,21 +121,32 @@
 
 Requirements
 ------------
 paramiko >= 1.17.0
 
 Supports
 --------
-Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10
+Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
 
 
 Change Log
 ==========
 
-1.0.7 (current, released 2023-02-27)
+1.0.9 (current, released 2023-05-08)
+------------------------------------
+    * added drivedrop to bypass _adjust_cwd's lack of Windows drive support
+    * added file_size logic and default remotepath fallback to putfo
+    * moved Connection.compress to CnOpts.compress
+    * reversion in put_d *again*
+    * removed SKIP_IF_CI from all but one test in response to the above
+    * switched to public key auth for all tests !¿macOS?¡
+    * switched from get_fingerprint() using md5 to helpers.hash using sha3_256
+    * test clean-up and major refactor
+
+1.0.7 (released 2023-02-27)
 ------------------------------------
     * fix reversion in put_d
 
 1.0.6 (released 2023-01-15)
 ------------------------------------
     * allow CnOpts knownhost to be set to None directly
     * standardize on using is for None checks
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sftpretty-1.0.8/README.rst` & `sftpretty-1.0.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -97,10 +97,10 @@
 
 Requirements
 ------------
 paramiko >= 1.17.0
 
 Supports
 --------
-Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10
+Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
```

### Comparing `sftpretty-1.0.8/docs/conf.py` & `sftpretty-1.0.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,24 +43,24 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'sftpretty'
-copyright = u'2021, byteskeptical'
+copyright = u'2020, byteskeptical'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '1.0'
 # The full version, including alpha/beta/rc tags.
-release = '1.0.8'
+release = '1.0.9'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `sftpretty-1.0.8/docs/contributing.rst` & `sftpretty-1.0.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/docs/cookbook.rst` & `sftpretty-1.0.9/docs/cookbook.rst`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
 Don't like how we have over-ridden or modified a paramiko method? Use this
 attribute to get at paramiko's original version. Remember, our goal is to
 augment not supplant paramiko.
 
 
 Remarks
 -------
-We think paramiko is a great python library and it is the backbone of sftpretty.
+Paramiko is a great python library and it is the backbone of sftpretty.
 The methods sftpretty has created are abstractions that serve a programmer's
 productivity by encapsulating many of the higher function use cases of
 interacting with SFTP. Instead of writing your own code to walk directories
 and call get and put, dealing with not only paramiko but Python's own ``os``
 and ``stat`` modules and writing tests *(many code snippets on the net are
 incomplete and don't account for edge cases)* sftpretty supplies a complete
 library for dealing with all three. Leaving you to focus on your primary task.
```

### Comparing `sftpretty-1.0.8/docs/index.rst` & `sftpretty-1.0.9/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 Requirements
 ------------
 paramiko >= 1.17.0
 
 Supports
 --------
-Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10
+Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
 
 Contents
 --------
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `sftpretty-1.0.8/docs/sftpretty.rst` & `sftpretty-1.0.9/docs/sftpretty.rst`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/setup.py` & `sftpretty-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     BUF = BUF.replace('$', '``')        # restore existing code markers
 LONG_DESCRIPTION += BUF
 
 DESCRIPTION = "Pretty secure file transfer made easy."
 
 setup(
     name='sftpretty',
-    version='1.0.8',
+    version='1.0.9',
 
     packages=['sftpretty', ],
 
     install_requires=['paramiko>=1.17'],
 
     # metadata for upload to PyPI
     author='byteskeptical',
@@ -40,10 +40,11 @@
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
     ],
 )
```

### Comparing `sftpretty-1.0.8/sftpretty/__init__.py` & `sftpretty-1.0.9/sftpretty/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,44 +1,47 @@
-from binascii import hexlify
 from concurrent.futures import as_completed, ThreadPoolExecutor
 from contextlib import contextmanager
 from functools import partial
 from logging import (DEBUG, ERROR, FileHandler, Formatter, getLogger, INFO,
                      StreamHandler)
-from os import environ, utime
+from os import environ, SEEK_END, utime
 from paramiko import (hostkeys, SFTPClient, Transport,
                       PasswordRequiredException, SSHException,
                       DSSKey, ECDSAKey, Ed25519Key, RSAKey)
-from pathlib import Path, PurePath, PureWindowsPath
+from pathlib import Path
 from sftpretty.exceptions import (CredentialException, ConnectionException,
                                   HostKeysException, LoggingException)
-from sftpretty.helpers import _callback, hash, localtree, retry, st_mode_to_int
+from sftpretty.helpers import _callback, drivedrop, hash, localtree, retry
 from socket import gaierror
 from stat import S_ISDIR, S_ISREG
 from tempfile import mkstemp
 from uuid import uuid4
 
 
 class CnOpts(object):
     '''Additional connection options beyond authentication.
 
-    :ivar tuple ciphers: *Default: paramiko.Transport.preferred_ciphers* -
-         Ordered list of preferred ciphers for connection.
-    :ivar tuple compression: *Default: paramiko.Transport.preferred_compression
+    :ivar tuple ciphers: *Default: paramiko.Transport.SecurityOptions.ciphers*
+        - Ordered list of preferred ciphers for connection.
+    :ivar bool compress: *Default: paramiko.Transport.use_compression* -
+        Enable or disable compression.
+    :ivar tuple compression:
+        *Default: paramiko.Transport.SecurityOptions.compression
         * - Ordered tuple of preferred compression algorithms for connection.
-    :ivar tuple digests: *Default: paramiko.Transport.preferred_macs* -
-        Ordered tuple of preferred digests/macs for connection.
+    :ivar tuple digests: *Default: paramiko.Transport.SecurityOptions.digests*
+         - Ordered tuple of preferred digests/macs for connection.
     :ivar dict disabled_algorithms: *Default: {}* - Mapping type to an
         iterable of algorithm identifiers, which will be disabled for the
         lifetime of the transport. Keys should match class builtin attribute.
     :ivar paramiko.hostkeys.HostKeys hostkeys: HostKeys object used for
         host key verifcation.
-    :ivar tuple kex: *Default: paramiko.Transport.preferred_kex* - Ordered
-        tuple of preferred key exchange algorithms for connection.
-    :ivar tuple key_types: *Default: paramiko.Transport.preferred_pubkeys*
+    :ivar tuple kex: *Default: paramiko.Transport.SecurityOptions.kex* -
+        Ordered tuple of preferred key exchange algorithms for connection.
+    :ivar tuple key_types:
+        *Default: paramiko.Transport.SecurityOptions.key_types*
         - Ordered tuple of preferred public key types for connection.
     :param str knownhosts: *Default: ~/.ssh/known_hosts* - File path to load
         hostkeys from.
     :ivar bool|str log: *Default: False* - Log connection details. If set to
         True, creates a temporary file used to capture logs. If set to an
         existing filepath, logs will be appended.
     :ivar str log_level: *Default: info* - Set logging level for connection.
@@ -47,14 +50,15 @@
         extended options to a Connection object.
     :raises HostKeysException:
     '''
     def __init__(self, knownhosts=Path(
                  '~/.ssh/known_hosts').expanduser().as_posix()):
         self.ciphers = ('aes256-ctr', 'aes192-ctr', 'aes128-ctr', 'aes256-cbc',
                         'aes192-cbc', 'aes128-cbc', '3des-cbc')
+        self.compress = False
         self.compression = ('none',)
         self.digests = ('hmac-sha2-512', 'hmac-sha2-256',
                         'hmac-sha2-512-etm@openssh.com',
                         'hmac-sha2-256-etm@openssh.com',
                         'hmac-sha1', 'hmac-md5')
         self.disabled_algorithms = {}
         self.hostkeys = hostkeys.HostKeys()
@@ -104,16 +108,14 @@
 class Connection(object):
     '''Connects and logs into the specified hostname. Arguments that are not
     given are guessed from the environment.
 
     :param str host: *Required* - Hostname or address of the remote machine.
     :param None|CnOpts cnopts: *Default: None* - Extended connection options
         set as a CnOpts object.
-    :param bool compress: *Default: False* - Enables compression on the
-        transport if set to True.
     :param str|None default_path: *Default: None* - Set the default working
         directory upon connection.
     :param str|None password: *Default: None* - Credential for remote machine.
     :param int port: *Default: 22* - SFTP server port of the remote machine.
     :param str|obj|None private_key: *Default: None* - Path to private key
         file(str) or paramiko.AgentKey object
     :param str|None private_key_pass: *Default: None* - Password to use on
@@ -124,66 +126,64 @@
     :raises ConnectionException:
     :raises CredentialException:
     :raises HostKeysException:
     :raises LoggingException:
     :raises PasswordRequiredException:
     :raises SSHException:
     '''
-    def __init__(self, host, cnopts=None, compress=False, default_path=None,
-                 password=None, port=22, private_key=None,
-                 private_key_pass=None, timeout=None, username=None):
+    def __init__(self, host, cnopts=None, default_path=None, password=None,
+                 port=22, private_key=None, private_key_pass=None,
+                 timeout=None, username=None):
         self._cnopts = cnopts or CnOpts()
         self._default_path = default_path
         self._set_logging()
         self._set_username(username)
         self._timeout = timeout
         self._transport = None
-        self._start_transport(host, port, compress=compress)
+        self._start_transport(host, port)
         self._set_authentication(password, private_key, private_key_pass)
 
     def _set_authentication(self, password, private_key, private_key_pass):
         '''Authenticate to transport. Prefer private key if given'''
         if private_key is not None:
             # Use key path or provided key object
-            key_map = {'DSA': DSSKey, 'EC': ECDSAKey, 'OPENSSH': Ed25519Key,
-                       'RSA': RSAKey}
+            key_types = {'DSA': DSSKey, 'EC': ECDSAKey, 'OPENSSH': Ed25519Key,
+                         'RSA': RSAKey}
             if isinstance(private_key, str):
-                private_key_file = Path(private_key).expanduser().absolute()
+                key_file = Path(private_key).expanduser().absolute().as_posix()
                 try:
-                    with open(private_key_file.as_posix(), 'r') as key:
-                        key_head = key.readline()
-                    key_head = key_head.removeprefix('-----BEGIN ')\
-                                       .removesuffix(' PRIVATE KEY-----\n')
-                    log.debug(f'Key Head: [{key_head}]')
-                    key_type = key_map[key_head.strip()]
+                    with open(key_file, 'r', encoding='utf-8') as head:
+                        key_id = head.readline()[11:][:-18]
+                    log.debug(f'Key ID: [{key_id}]')
+                    key = key_types[key_id.strip()]
                 except KeyError as err:
                     log.error(('Unable to identify key type from file provided'
-                              f':\n[{private_key_file}]'))
+                              f':\n[{key_file}]'))
                     raise err
                 except PasswordRequiredException as err:
                     log.error(('No password provided for encrypted private '
                                'key encrypted private key.'))
                     raise err
                 except PermissionError as err:
                     log.error(('File permission preventing user access to:\n'
-                              f'[{private_key_file}]'))
+                              f'[{key_file}]'))
                     raise err
                 except SSHException as err:
                     log.error(('Path provided is an invalid key file, a '
                                'directory or does not exist, please revise '
                                'and provide a path to a valid private key.'))
                     raise err
                 finally:
-                    private_key = key_type.from_private_key_file(
-                        private_key_file.as_posix(), password=private_key_pass)
+                    private_key = key.from_private_key_file(
+                        key_file, password=private_key_pass)
             self._transport.auth_publickey(self._username, private_key)
         elif password is not None:
             self._transport.auth_password(self._username, password)
         else:
-            raise CredentialException('No password or private key specified.')
+            raise CredentialException('No password or private key provided.')
 
     def _set_logging(self):
         '''Set logging location and level for connection'''
         level_map = {'debug': DEBUG, 'error': ERROR, 'info': INFO}
 
         try:
             if self._cnopts.log:
@@ -232,31 +232,31 @@
             channel = _channel.get_channel()
             channel_name = uuid4().hex
             channel.set_name(channel_name)
             channel.settimeout(self._timeout)
             log.debug(f'Channel Name: [{channel_name}]')
 
             if self._default_path is not None:
-                _channel.chdir(self._default_path)
+                _channel.chdir(drivedrop(self._default_path))
                 log.info(f'Current Working Directory: [{self._default_path}]')
 
             yield _channel
         except Exception as err:
             raise err
         finally:
             if _channel and not keepalive:
                 _channel.close()
 
-    def _start_transport(self, host, port, compress=False):
+    def _start_transport(self, host, port):
         '''Start the transport and set connection options if specified.'''
         try:
             self._transport = Transport((host, port))
             self._transport.set_keepalive(60)
             self._transport.set_log_channel(host)
-            self._transport.use_compression(compress=compress)
+            self._transport.use_compression(compress=self._cnopts.compress)
 
             # Set disabled algorithms
             disabled_algorithms = self._cnopts.disabled_algorithms
             self._transport.disabled_algorithms = disabled_algorithms
             log.debug(f'Disabled Algorithms: [{disabled_algorithms}]')
 
             # Security Options
@@ -281,23 +281,23 @@
             self._transport.get_security_options().key_types = key_types
             log.debug(f'Public Key Types: [{key_types}]')
 
             self._transport.start_client(timeout=self._timeout)
 
             if self._transport.is_active():
                 remote_hostkey = self._transport.get_remote_server_key()
-                remote_fingerprint = hexlify(remote_hostkey.get_fingerprint())
+                remote_fingerprint = hash(remote_hostkey)
                 log.info((f'[{host}] Host Key:\n\t'
                           f'Name: {remote_hostkey.get_name()}\n\t'
                           f'Fingerprint: {remote_fingerprint}\n\t'
                           f'Size: {remote_hostkey.get_bits():d}'))
 
                 if self._cnopts.hostkeys is not None:
                     user_hostkey = self._cnopts.get_hostkey(host)
-                    user_fingerprint = hexlify(user_hostkey.get_fingerprint())
+                    user_fingerprint = hash(user_hostkey)
                     log.info(f'Known Fingerprint: {user_fingerprint}')
                     if user_fingerprint != remote_fingerprint:
                         raise HostKeysException((f'{host} key verification: '
                                                  '[FAILED]'))
             else:
                 err = self._transport.get_exception()
                 if err:
@@ -484,25 +484,25 @@
 
         :returns: None
 
         :raises: Any exception raised by operations will be passed through.
         '''
         self.chdir(remotedir)
 
-        directories = {}
-        cwd = self._default_path
+        lwd = Path(localdir).absolute().as_posix()
+        rwd = self._default_path
 
-        directories[cwd] = [(cwd, Path(localdir).joinpath(
-                                       cwd.lstrip('/')).as_posix())]
+        tree = {}
+        tree[rwd] = [(rwd, lwd)]
 
-        self.remotetree(directories, cwd, localdir, recurse=True)
-        log.debug(f'Remote Tree: [{directories}]')
+        self.remotetree(tree, rwd, lwd, recurse=True)
+        log.debug(f'Remote Tree: [{tree}]')
 
-        for tld in directories.keys():
-            for remote, local in directories[tld]:
+        for roots in tree.keys():
+            for remote, local in tree[roots]:
                 self.get_d(remote, local, callback=callback,
                            pattern=pattern, preserve_mtime=preserve_mtime,
                            exceptions=exceptions, tries=tries, backoff=backoff,
                            delay=delay, logger=logger, silent=silent)
 
     def getfo(self, remotefile, flo, callback=None, exceptions=None,
               tries=None, backoff=2, delay=1, logger=getLogger(__name__),
@@ -595,14 +595,15 @@
 
             if preserve_mtime:
                 local_attributes = Path(localfile).stat()
                 local_times = (local_attributes.st_atime,
                                local_attributes.st_mtime)
 
             with self._sftp_channel() as channel:
+                remotepath = drivedrop(remotepath)
                 remote_attributes = channel.put(localfile,
                                                 remotepath=remotepath,
                                                 callback=callback,
                                                 confirm=confirm)
 
                 if preserve_mtime:
                     channel.utime(remotepath, local_times)
@@ -644,29 +645,26 @@
             be attempted.
 
         :returns: None
 
         :raises IOError: if remotedir doesn't exist
         :raises OSError: if localdir doesn't exist
         '''
-        self.mkdir_p(Path(remotedir).joinpath(localdir.stem).as_posix())
+        localdir = Path(localdir)
 
-        if localdir.startswith(':', 1) or localdir.startswith('\\'):
-            localdir = PureWindowsPath(localdir)
-        else:
-            localdir = PurePath(localdir)
+        self.mkdir_p(Path(remotedir).joinpath(localdir.stem).as_posix())
 
         paths = [
                  (localpath.as_posix(),
                   Path(remotedir).joinpath(
                       localpath.relative_to(
                           localdir.parent).as_posix()).as_posix(),
                   callback, confirm, preserve_mtime, exceptions, tries,
                   backoff, delay, logger, silent)
-                 for localpath in Path(localdir).iterdir()
+                 for localpath in localdir.iterdir()
                  if localpath.is_file()
                 ]
 
         if paths != []:
             thread_prefix = uuid4().hex
             with ThreadPoolExecutor(thread_name_prefix=thread_prefix) as pool:
                 logger.debug(f'Thread Prefix: [{thread_prefix}]')
@@ -725,37 +723,39 @@
             be attempted.
 
         :returns: None
 
         :raises IOError: if remotedir doesn't exist
         :raises OSError: if localdir doesn't exist
         '''
-        directories = {}
-        directories['root'] = [(localdir,
-                                Path(remotedir).joinpath(localdir).as_posix())]
+        lwd = Path(localdir).absolute().as_posix()
+        rwd = self.normalize(remotedir)
 
-        localtree(directories, localdir, remotedir, recurse=True)
-        log.debug(f'Local Tree: [{directories}]')
+        tree = {}
+        tree[lwd] = [(lwd, rwd)]
 
-        for tld in directories.keys():
-            for local, remote in directories[tld]:
+        localtree(tree, lwd, rwd, recurse=True)
+        log.debug(f'Local Tree: [{tree}]')
+
+        for roots in tree.keys():
+            for local, remote in tree[roots]:
                 self.put_d(local, remote, callback=callback, confirm=confirm,
                            preserve_mtime=preserve_mtime,
                            exceptions=exceptions, tries=tries, backoff=backoff,
                            delay=delay, logger=logger, silent=silent)
 
-    def putfo(self, flo, remotepath=None, file_size=0, callback=None,
+    def putfo(self, flo, remotepath=None, file_size=None, callback=None,
               confirm=True, exceptions=None, tries=None, backoff=2,
               delay=1, logger=getLogger(__name__), silent=False):
         '''Copies the contents of a file like object to remotepath.
 
         :param flo: File-like object that supports .read()
         :param str remotepath: The remote location to save contents of object.
-        :param int file_size: The size of flo, if not given the second param
-            passed to the callback function will always be 0.
+        :param int file_size: The size of flo, if not given, calculated
+            preventing division by zero in default callback function.
         :param callable callback: Optional callback function (form: ``func(
             int, int``)) that accepts the bytes transferred so far and the
             total bytes to be transferred.
         :param bool confirm: *Default: True* - Whether to do a stat() on the
             file afterwards to confirm the file size.
         :param Exception exceptions: Exception(s) to check. May be a tuple of
             exceptions to check. IOError or IOError(errno.ECOMM) or (IOError,)
@@ -772,23 +772,27 @@
 
         :returns: (obj) SFTPAttributes containing details about the given file.
 
         :raises: TypeError, if remotepath not specified, any underlying error
         '''
         @retry(exceptions, tries=tries, backoff=backoff, delay=delay,
                logger=logger, silent=silent)
-        def _putfo(self, flo, remotepath=None, file_size=0, callback=None,
+        def _putfo(self, flo, remotepath=None, file_size=None, callback=None,
                    confirm=True):
 
-            if remotepath is None:
-                remotepath = Path(flo.name).name
-
             if callback is None:
                 callback = partial(_callback, flo, logger=logger)
 
+            if file_size is None:
+                file_size = flo.seek(0, SEEK_END)
+                flo.seek(0)
+
+            if remotepath is None:
+                remotepath = uuid4().hex
+
             with self._sftp_channel() as channel:
                 flo_attributes = channel.putfo(flo, remotepath=remotepath,
                                                file_size=file_size,
                                                callback=callback,
                                                confirm=confirm)
 
             return flo_attributes
@@ -865,42 +869,43 @@
         :param str remotepath: Remote path to set as current working directory.
 
         :returns: None
 
         :raises: IOError, if path does not exist
         '''
         with self._sftp_channel() as channel:
-            channel.chdir(remotepath)
+            channel.chdir(drivedrop(remotepath))
             self._default_path = channel.normalize('.')
 
-    def chmod(self, remotepath, mode=777):
+    def chmod(self, remotepath, mode=700):
         '''Set the permission mode of a remotepath, where mode is an octal.
 
         :param str remotepath: Remote path to modify permission.
-        :param int mode: *Default: 777* - Octal mode to apply on path.
+        :param int mode: *Default: 700* - Octal mode to apply on path.
 
         :returns: None
 
         :raises: IOError, if the file doesn't exist
         '''
         with self._sftp_channel() as channel:
-            channel.chmod(remotepath, mode=int(str(mode), 8))
+            channel.chmod(drivedrop(remotepath), mode=int(str(mode), 8))
 
     def chown(self, remotepath, uid=None, gid=None):
         '''Set uid/gid on remotepath, you may specify either or both.
 
         :param str remotepath: Remote path to modify ownership.
         :param int uid: User id to set as owner of remote path.
         :param int gid: Group id to set on the remote path.
 
         :returns: None
 
         :raises: IOError, if user lacks permission or if the file doesn't exist
         '''
         with self._sftp_channel() as channel:
+            remotepath = drivedrop(remotepath)
             if uid is None or gid is None:
                 if uid is None and gid is None:
                     return
                 remote_attributes = channel.stat(remotepath)
                 if uid is None:
                     uid = remote_attributes.st_uid
                 if gid is None:
@@ -916,14 +921,16 @@
                 self._transport.close()
             self._transport = None
             # Clean up any loggers
             if log.hasHandlers():
                 # remove lingering handlers if any
                 for handle in log.handlers:
                     log.removeHandler(handle)
+        except AttributeError:
+            pass
         except Exception as err:
             raise err
 
     def exists(self, remotepath):
         '''Test whether a remotepath exists.
 
         :param str remotepath: Remote location to verify existance of.
@@ -988,30 +995,30 @@
 
         :param str remotepath: Remote location to test.
 
         :returns: (bool), True, if lexists, else False
         '''
         with self._sftp_channel() as channel:
             try:
-                channel.lstat(remotepath)
+                channel.lstat(drivedrop(remotepath))
             except IOError:
                 return False
 
         return True
 
     def listdir(self, remotepath='.'):
         '''Return a sorted list of a directory's contents.
 
         :param str remotepath: Remote location to search.
 
         :returns: (list of str) Sorted directory content.
 
         '''
         with self._sftp_channel() as channel:
-            directory = sorted(channel.listdir(remotepath))
+            directory = sorted(channel.listdir(drivedrop(remotepath)))
 
         return directory
 
     def listdir_attr(self, remotepath='.'):
         '''Return a non-sorted list of SFTPAttribute objects for the remote
         directory contents. Will not include the special entries '.' and '..'.
 
@@ -1021,67 +1028,69 @@
         the SFTP server.
 
         :param str remotepath: Remote location to search.
 
         :returns: (list of SFTPAttributes) Sorted directory content as objects.
         '''
         with self._sftp_channel() as channel:
-            directory = sorted(channel.listdir_attr(remotepath),
+            directory = sorted(channel.listdir_attr(drivedrop(remotepath)),
                                key=lambda attribute: attribute.filename)
 
         return directory
 
     def lstat(self, remotepath):
         '''Return information about remote location without following symbolic
         links. Otherwise, the same as .stat().
 
         :param str remotepath: Remote location to stat.
 
         :returns: (obj) SFTPAttributes object
         '''
         with self._sftp_channel() as channel:
-            lstat = channel.lstat(remotepath)
+            lstat = channel.lstat(drivedrop(remotepath))
 
         return lstat
 
-    def mkdir(self, remotedir, mode=777):
+    def mkdir(self, remotedir, mode=700):
         '''Create a directory and set permission mode. On some systems, mode
         is ignored. Where used, the current umask value is first masked out.
 
         :param str remotedir: Remote location to create.
-        :param int mode: *Default: 777* - Octal mode to apply on path.
+        :param int mode: *Default: 700* - Octal mode to apply on path.
 
         :returns: None
         '''
         with self._sftp_channel() as channel:
-            channel.mkdir(remotedir, mode=int(str(mode), 8))
+            channel.mkdir(drivedrop(remotedir), mode=int(str(mode), 8))
 
-    def mkdir_p(self, remotedir, mode=777):
+    def mkdir_p(self, remotedir, mode=700):
         '''Create a directory and any missing parent locations as needed. Set
         permission mode, if created. Silently complete if remotedir already
         exists.
 
         :param str remotedir: Remote location to create.
-        :param int mode: *Default: 777* - Octal mode to apply on created paths.
+        :param int mode: *Default: 700* - Octal mode to apply on created paths.
 
         :returns: None
 
         :raises: OSError
         '''
         try:
+            remotedir = drivedrop(remotedir)
             if self.isdir(remotedir):
-                pass
+                return
             elif self.isfile(remotedir):
-                raise OSError(('A file with the same name as the remotedir, '
-                              f'[{remotedir}], already exists.'))
+                raise OSError((f'A file with the same name, [{remotedir}], '
+                               'already exists.'))
             else:
                 parent = Path(remotedir).parent.as_posix()
                 stem = Path(remotedir).stem
-                if parent and not self.isdir(parent):
-                    self.mkdir_p(parent, mode=mode)
+                if parent != remotedir:
+                    if not self.isdir(parent):
+                        self.mkdir_p(parent, mode=mode)
                 if stem:
                     self.mkdir(remotedir, mode=mode)
         except Exception as err:
             raise err
 
     def normalize(self, remotepath):
         '''Return the fully expanded path of a given location. This can be used
@@ -1091,42 +1100,44 @@
         :param str remotepath: Remote location to be normalized.
 
         :return: (str) Normalized path.
 
         :raises: IOError, if remotepath can't be resolved
         '''
         with self._sftp_channel() as channel:
-            expanded_path = channel.normalize(remotepath)
+            expanded_path = channel.normalize(drivedrop(remotepath))
 
         return expanded_path
 
-    def open(self, remotefile, mode='r', bufsize=-1):
+    def open(self, remotefile, bufsize=-1, mode='r'):
         '''Open a file on the remote server.
 
         :param str remotefile: Path of remote file to open.
         :param str mode: *Default: read-only* - File access mode.
         :param int bufsize: *Default: -1* - Buffering in bytes.
 
         :returns: (obj) SFTPFile, a file-like object handler.
 
         :raises: IOError, if the file could not be opened.
         '''
         with self._sftp_channel(keepalive=True) as channel:
-            flo = channel.open(remotefile, mode=mode, bufsize=bufsize)
+            remotefile = drivedrop(remotefile)
+            flo = channel.open(remotefile, bufsize=bufsize, mode=mode)
 
         return flo
 
     def readlink(self, remotelink):
         '''Return the target of a symlink as an absolute path.
 
         :param str remotelink: Remote location of the symlink.
 
         :return: (str) Absolute path to target.
         '''
         with self._sftp_channel() as channel:
+            remotelink = drivedrop(remotelink)
             link_destination = channel.normalize(channel.readlink(remotelink))
 
         return link_destination
 
     def remotetree(self, container, remotedir, localdir, recurse=True):
         '''recursively descend remote directory mapping the tree to a
         dictionary container.
@@ -1149,22 +1160,21 @@
             localdir = Path(localdir).expanduser().as_posix()
             remotedir = self.normalize(remotedir)
             for attribute in self.listdir_attr(remotedir):
                 if S_ISDIR(attribute.st_mode):
                     remote = Path(remotedir).joinpath(
                         attribute.filename).as_posix()
                     local = Path(localdir).joinpath(
-                        Path(remote).relative_to(
-                            Path(remotedir).anchor).as_posix()).as_posix()
+                        Path(remote).stem).as_posix()
                     if remotedir in container.keys():
                         container[remotedir].append((remote, local))
                     else:
                         container[remotedir] = [(remote, local)]
                     if recurse:
-                        self.remotetree(container, remote, localdir,
+                        self.remotetree(container, remote, local,
                                         recurse=recurse)
         except Exception as err:
             raise err
 
     def remove(self, remotefile):
         '''Delete the remote file. May include a path, if no path, then
         :attr:`.pwd` is used. This method only works on files.
@@ -1172,80 +1182,81 @@
         :param str remotefile: Remote file to delete.
 
         :returns: None
 
         :raises: IOError
         '''
         with self._sftp_channel() as channel:
-            channel.remove(remotefile)
+            channel.remove(drivedrop(remotefile))
 
     def rename(self, remotepath, newpath):
         '''Rename a path on the remote host.
 
         :param str remotepath: Remote path to rename.
 
         :param str newpath: New name for remote path.
 
         :returns: None
 
         :raises: IOError
         '''
         with self._sftp_channel() as channel:
-            channel.posix_rename(remotepath, newpath)
+            channel.posix_rename(drivedrop(remotepath), drivedrop(newpath))
 
     def rmdir(self, remotedir):
         '''Delete remote directory.
 
         :param str remotedir: Remote directory to delete.
 
         :returns: None
         '''
         with self._sftp_channel() as channel:
-            channel.rmdir(remotedir)
+            channel.rmdir(drivedrop(remotedir))
 
     def stat(self, remotepath):
         '''Return information about remote location.
 
         :param str remotepath: Remote location to stat.
 
         :returns: (obj) SFTPAttributes
         '''
         with self._sftp_channel() as channel:
-            stat = channel.stat(remotepath)
+            stat = channel.stat(drivedrop(remotepath))
 
         return stat
 
     def symlink(self, remote_src, remote_dest):
         '''Create a symlink for a remote file on the server
 
         :param str remote_src: path of original file
         :param str remote_dest: path of the created symlink
 
         :returns: None
 
         :raises: any underlying error, IOError if remote_dest already exists
         '''
         with self._sftp_channel() as channel:
-            channel.symlink(remote_src, remote_dest)
+            channel.symlink(remote_src, drivedrop(remote_dest))
 
     def truncate(self, remotepath, size):
         '''Change the size of the file specified by path. Used to modify the
         size of the file, just like the truncate method on Python file objects.
         The new file size is confirmed and returned.
 
         :param str remotepath: remote file path to modify
         :param int|long size: the new file size
 
         :returns: (int) new size of file
 
         :raises: IOError, if file does not exist
         '''
         with self._sftp_channel() as channel:
+            remotepath = drivedrop(remotepath)
             channel.truncate(remotepath, size)
-            size = channel.state(remotepath).st_size
+            size = channel.stat(remotepath).st_size
 
         return size
 
     @property
     def active_ciphers(self):
         '''Get tuple of currently used local and remote ciphers.
```

### Comparing `sftpretty-1.0.8/sftpretty/exceptions.py` & `sftpretty-1.0.9/sftpretty/exceptions.py`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/sftpretty/helpers.py` & `sftpretty-1.0.9/sftpretty/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,21 @@
                f'{bytes_so_far:d}:{bytes_total:d} bytes ')
     if logger:
         logger.info(message)
     else:
         print(message)
 
 
+def drivedrop(filepath):
+    if PureWindowsPath(filepath).drive:
+        filepath = Path('/').joinpath(*Path(filepath).parts[1:]).as_posix()
+
+    return filepath
+
+
 def hash(filename, algorithm=sha3_512(), blocksize=65536):
     '''hash contents of a file, file like object or string
 
     :param bytesIO,IObase,str filename:
         path to file, file object, or string to process
     :param hashlib.hash algorithm:
         hash object to use as digest algorithm
@@ -76,25 +83,21 @@
         if localdir.startswith(':', 1) or localdir.startswith('\\'):
             localdir = PureWindowsPath(localdir)
         else:
             localdir = Path(localdir).expanduser().absolute()
         for localpath in Path(localdir).iterdir():
             if localpath.is_dir():
                 local = localpath.as_posix()
-                remote = Path(remotedir).joinpath(
-                    localpath.relative_to(
-                        localdir.anchor).as_posix()).as_posix()
+                remote = Path(remotedir).joinpath(localpath.stem).as_posix()
                 if localdir.as_posix() in container.keys():
                     container[localdir.as_posix()].append((local, remote))
                 else:
                     container[localdir.as_posix()] = [(local, remote)]
-                container[localdir.as_posix()].sort()
                 if recurse:
-                    localtree(container, local, remotedir,
-                              recurse=recurse)
+                    localtree(container, local, remote, recurse=recurse)
     except Exception as err:
         raise err
 
 
 def retry(exceptions, tries=0, delay=3, backoff=2, silent=False, logger=None):
     '''Exception type based retry decorator for all your problematic functions
```

### Comparing `sftpretty-1.0.8/sftpretty.egg-info/PKG-INFO` & `sftpretty-1.0.9/sftpretty.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sftpretty
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pretty secure file transfer made easy.
 Home-page: https://github.com/byteskeptical/sftpretty
 Download-URL: https://pypi.python.org/pypi/sftpretty
 Author: byteskeptical
 Author-email: 40208858+byteskeptical@users.noreply.github.com
 License: BSD
 Keywords: ftp scp sftp ssh
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 sftpretty
 =========
 
@@ -120,21 +121,32 @@
 
 Requirements
 ------------
 paramiko >= 1.17.0
 
 Supports
 --------
-Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10
+Tested on Python 3.6, 3.7, 3.8, 3.9, 3.10, 3.11
 
 
 Change Log
 ==========
 
-1.0.7 (current, released 2023-02-27)
+1.0.9 (current, released 2023-05-08)
+------------------------------------
+    * added drivedrop to bypass _adjust_cwd's lack of Windows drive support
+    * added file_size logic and default remotepath fallback to putfo
+    * moved Connection.compress to CnOpts.compress
+    * reversion in put_d *again*
+    * removed SKIP_IF_CI from all but one test in response to the above
+    * switched to public key auth for all tests !¿macOS?¡
+    * switched from get_fingerprint() using md5 to helpers.hash using sha3_256
+    * test clean-up and major refactor
+
+1.0.7 (released 2023-02-27)
 ------------------------------------
     * fix reversion in put_d
 
 1.0.6 (released 2023-01-15)
 ------------------------------------
     * allow CnOpts knownhost to be set to None directly
     * standardize on using is for None checks
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sftpretty-1.0.8/sftpretty.egg-info/SOURCES.txt` & `sftpretty-1.0.9/sftpretty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/tests/test_cd.py` & `sftpretty-1.0.9/tests/test_cd.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 '''test sftpretty.cd'''
 
 import pytest
 
 from common import conn, VFS
+from pathlib import Path
 from sftpretty import Connection
 
 
 def test_cd_none(sftpserver):
     '''test sftpretty.cd with None'''
+    pubpath = Path('/home/test').joinpath('pub')
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
             home = sftp.pwd
             with sftp.cd():
                 sftp.chdir('pub')
-                assert sftp.pwd == '/home/test/pub'
-            assert home == sftp.pwd
+                assert sftp.pwd == pubpath.as_posix()
+            assert home == pubpath.parent.as_posix()
 
 
 def test_cd_path(sftpserver):
     '''test sftpretty.cd with a path'''
+    pubpath = Path('/home/test').joinpath('pub')
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
             home = sftp.pwd
             with sftp.cd('pub'):
-                assert sftp.pwd == '/home/test/pub'
-            assert home == sftp.pwd
+                assert sftp.pwd == pubpath.as_posix()
+            assert home == pubpath.parent.as_posix()
 
 
 def test_cd_nested(sftpserver):
     '''test nested cd's'''
+    pubpath = Path('/home/test').joinpath('pub')
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
             home = sftp.pwd
             with sftp.cd('pub'):
-                assert sftp.pwd == '/home/test/pub'
+                assert sftp.pwd == pubpath.as_posix()
                 with sftp.cd('foo1'):
-                    assert sftp.pwd == '/home/test/pub/foo1'
-                assert sftp.pwd == '/home/test/pub'
-            assert home == sftp.pwd
+                    assert sftp.pwd == pubpath.joinpath('foo1').as_posix()
+                assert sftp.pwd == pubpath.as_posix()
+            assert home == pubpath.parent.as_posix()
 
 
 def test_cd_bad_path(sftpserver):
     '''test sftpretty.cd with a bad path'''
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
             home = sftp.pwd
             with pytest.raises(IOError):
                 with sftp.cd('not-there'):
                     pass
-            assert home == sftp.pwd
+            assert home == '/home/test'
```

### Comparing `sftpretty-1.0.8/tests/test_chmod.py` & `sftpretty-1.0.9/tests/test_chmod.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 '''test sftpretty.chmod'''
 
 import pytest
 
-from common import conn, SKIP_IF_CI, tempfile_containing, VFS
+from common import conn, SKIP_IF_WIN, tempfile_containing, VFS
 from pathlib import Path
-from sftpretty import Connection, st_mode_to_int
+from sftpretty import Connection
+from sftpretty.helpers import st_mode_to_int
 
 
 def test_chmod_not_exist(sftpserver):
     '''verify error if trying to chmod something that isn't there'''
     with sftpserver.serve_content(VFS):
-        with Connection(**conn(sftpserver)) as psftp:
+        with Connection(**conn(sftpserver)) as sftp:
             with pytest.raises(IOError):
-                psftp.chmod('i-do-not-exist.txt', 666)
+                sftp.chmod('i-do-not-exist.txt', 666)
 
 
-@SKIP_IF_CI
+@SKIP_IF_WIN
 def test_chmod_simple(lsftp):
     '''test basic chmod with octal mode represented by an int'''
-    new_mode = 744      # user=rwx g=r o=r
+    new_mode = 711
     with tempfile_containing(contents='') as fname:
         base_fname = Path(fname).name
         org_attrs = lsftp.put(fname)
         lsftp.chmod(base_fname, new_mode)
         new_attrs = lsftp.stat(base_fname)
         lsftp.remove(base_fname)
-    # that the new mod 744 is as we wanted
+
     assert st_mode_to_int(new_attrs.st_mode) == new_mode
-    # that we actually changed something
     assert new_attrs.st_mode != org_attrs.st_mode
 
 
 # TODO
 # def test_chmod_fail_ro(psftp):
 #     '''test chmod against read-only server'''
 #     new_mode = 440
```

### Comparing `sftpretty-1.0.8/tests/test_chown.py` & `sftpretty-1.0.9/tests/test_chown.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 '''test sftpretty.chown'''
 
 import pytest
 
-from common import SKIP_IF_CI, tempfile_containing
+from common import SKIP_IF_WIN, tempfile_containing
 from pathlib import Path
 
 
-@SKIP_IF_CI
+@SKIP_IF_WIN  # uid comes through as 0, lacks support
 def test_chown_uid(lsftp):
     '''test changing just the uid'''
     with tempfile_containing() as fname:
         base_fname = Path(fname).name
         org_attrs = lsftp.put(fname)
-        uid = org_attrs.st_uid  # - 1
+        uid = org_attrs.st_uid
         lsftp.chown(base_fname, uid=uid)
         new_attrs = lsftp.stat(base_fname)
         lsftp.remove(base_fname)
+    assert new_attrs.st_gid == org_attrs.st_gid
     assert new_attrs.st_uid == uid
-    assert new_attrs.st_gid == org_attrs.st_gid  # confirm no change to gid
 
 
-@SKIP_IF_CI
+@SKIP_IF_WIN  # gid comes through as 0, lacks support
 def test_chown_gid(lsftp):
     '''test changing just the gid'''
     with tempfile_containing() as fname:
         base_fname = Path(fname).name
         org_attrs = lsftp.put(fname)
-        gid = org_attrs.st_gid  # - 1
+        gid = org_attrs.st_gid
         lsftp.chown(base_fname, gid=gid)
         new_attrs = lsftp.stat(base_fname)
         lsftp.remove(base_fname)
     assert new_attrs.st_gid == gid
-    assert new_attrs.st_uid == org_attrs.st_uid  # confirm no change to uid
+    assert new_attrs.st_uid == org_attrs.st_uid
 
 
-@SKIP_IF_CI
 def test_chown_none(lsftp):
     '''call .chown with no gid or uid specified'''
     with tempfile_containing() as fname:
         base_fname = Path(fname).name
         org_attrs = lsftp.put(fname)
         lsftp.chown(base_fname)
         new_attrs = lsftp.stat(base_fname)
         lsftp.remove(base_fname)
     assert new_attrs.st_gid == org_attrs.st_gid
-    assert new_attrs.st_uid == org_attrs.st_uid  # confirm no change to uid
+    assert new_attrs.st_uid == org_attrs.st_uid
 
 
-@SKIP_IF_CI
 def test_chown_not_exist(lsftp):
     '''call .chown on a non-existing path'''
     with pytest.raises(IOError):
         lsftp.chown('i-do-not-exist.txt', 666)
 
 
 # TODO
```

### Comparing `sftpretty-1.0.8/tests/test_ciphers.py` & `sftpretty-1.0.9/tests/test_ciphers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 '''test CnOpts.ciphers param'''
 
 # these can not use fixtures as we need to set ciphers prior to the connection
 # being made and fixtures are already active connections.
 
-from common import SFTP_LOCAL, SKIP_IF_CI
+from common import LOCAL
 from sftpretty import CnOpts, Connection
 
 
-@SKIP_IF_CI
 def test_connection_ciphers_cnopts():
     '''test the CnOpts.ciphers portion of the Connection'''
-    ciphers = ('aes256-ctr', 'blowfish-cbc', 'aes256-cbc', 'arcfour256')
-    copts = SFTP_LOCAL.copy()  # don't sully the module level variable
-    cnopts = CnOpts()
+    ciphers = ('aes256-ctr', 'aes256-cbc')
+    copts = LOCAL.copy()  # don't sully the module level variable
+    cnopts = CnOpts(knownhosts=None)
     cnopts.ciphers = ciphers
     copts['cnopts'] = cnopts
-    assert copts != SFTP_LOCAL
+    assert copts != LOCAL
     with Connection(**copts) as sftp:
         rslt = sftp.listdir()
         assert len(rslt) > 1
 
 
-@SKIP_IF_CI
 def test_active_ciphers():
     '''test that method returns a tuple of strings, that show ciphers used'''
-    ciphers = ('aes256-ctr', 'blowfish-cbc', 'aes256-cbc', 'arcfour256')
-    copts = SFTP_LOCAL.copy()  # don't sully the module level variable
-    cnopts = CnOpts()
+    ciphers = ('aes256-ctr', 'aes256-cbc')
+    copts = LOCAL.copy()  # don't sully the module level variable
+    cnopts = CnOpts(knownhosts=None)
     cnopts.ciphers = ciphers
     copts['cnopts'] = cnopts
     with Connection(**copts) as sftp:
         local_cipher, remote_cipher = sftp.active_ciphers
     assert local_cipher in ciphers
     assert remote_cipher in ciphers
```

### Comparing `sftpretty-1.0.8/tests/test_get.py` & `sftpretty-1.0.9/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/tests/test_get_d.py` & `sftpretty-1.0.9/tests/test_get_d.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def test_get_d(sftpserver):
     '''test the get_d for remotepath is pwd '.' '''
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
             sftp.chdir('pub')
-            localpath = mkdtemp()
+            localpath = Path(mkdtemp()).as_posix()
             sftp.get_d('.', localpath)
 
             checks = [(['', ], ['make.txt', ]), ]
             for pth, fls in checks:
                 assert sorted([path.name
                                for path in Path(localpath).joinpath(
                                                 *pth).iterdir()]) == fls
@@ -25,15 +25,15 @@
 
 
 def test_get_d_pathed(sftpserver):
     '''test the get_d for localpath, starting deeper then pwd '''
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
             sftp.chdir('pub')
-            localpath = mkdtemp()
+            localpath = Path(mkdtemp()).as_posix()
             sftp.get_d('foo1', localpath)
 
             checks = [(['', ], ['foo1.txt', 'image01.jpg']), ]
             for pth, fls in checks:
                 assert sorted([path.name
                                for path in Path(localpath).joinpath(
                                                 *pth).iterdir()]) == fls
```

### Comparing `sftpretty-1.0.8/tests/test_getcwd.py` & `sftpretty-1.0.9/tests/test_getcwd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-'''test sftpretty.getcwd
-until you issue a .chdir/cwd command paramiko returns None for .getcwd,
-unless you have set default_path in the Connection args'''
+'''test sftpretty.getcwd'''
 
 from common import conn, VFS
+from pathlib import Path
 from sftpretty import Connection
 
 
 def test_getcwd_none(sftpserver):
-    '''test .getcwd as the first operation - need pristine connection
-    and no default_path arg'''
+    '''test .getcwd with no default_path arg'''
     with sftpserver.serve_content(VFS):
         cnn = conn(sftpserver)
         cnn['default_path'] = None
         with Connection(**cnn) as sftp:
             assert sftp.getcwd() is None
 
 
@@ -21,13 +19,14 @@
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
             assert sftp.getcwd() == '/home/test'
 
 
 def test_getcwd_after_chdir(sftpserver):
     '''test getcwd after a chdir operation'''
+    pubpath = Path('/home/test').joinpath('pub/foo1')
     with sftpserver.serve_content(VFS):
         cnn = conn(sftpserver)
         cnn['default_path'] = None
         with Connection(**cnn) as sftp:
-            sftp.chdir('/home/test/pub/foo1')
-            assert sftp.getcwd() == '/home/test/pub/foo1'
+            sftp.chdir(pubpath.as_posix())
+            assert sftp.getcwd() == pubpath.as_posix()
```

### Comparing `sftpretty-1.0.8/tests/test_getfo.py` & `sftpretty-1.0.9/tests/test_getfo.py`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/tests/test_is.py` & `sftpretty-1.0.9/tests/test_is.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             assert sftp.isfile(rfile)
             assert sftp.isfile(rdir) is False
 
 
 # TODO
 # def test_isfile_2(sftp):
 #     '''test .isfile() functionality against a symlink'''
-#     rsym = '/home/test/readme.sym'
+#     rsym = 'readme.sym'
 #     assert sftp.isfile(rsym)
 
 
 def test_isdir(sftpserver):
     '''test .isdir() functionality'''
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
@@ -30,9 +30,9 @@
             assert sftp.isdir(rfile) is False
             assert sftp.isdir(rdir)
 
 
 # TODO
 # def test_isdir_2(sftp):
 #     '''test .isdir() functionality against a symlink'''
-#     rsym = '/home/test/readme.sym'
+#     rsym = 'readme.sym'
 #     assert sftp.isdir(rsym) is False
```

### Comparing `sftpretty-1.0.8/tests/test_issue_65.py` & `sftpretty-1.0.9/tests/test_issue_65.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 '''use the cd contextmanager prior to paramiko establishing a directory
 location'''
 
 from common import conn, VFS
+from pathlib import Path
 from sftpretty import Connection
 
 
 def test_issue_65(sftpserver):
     '''using the .cd() context manager prior to setting a directory
     via chdir causes an error'''
+    pubpath = Path('/home/test').joinpath('pub')
     with sftpserver.serve_content(VFS):
         cnn = conn(sftpserver)
-        cnn['default_path'] = None  # don't call .chdir by setting default_path
+        cnn['default_path'] = None
         with Connection(**cnn) as sftp:
             assert sftp.getcwd() is None
-            with sftp.cd('/home/test/pub'):
+            with sftp.cd(pubpath.as_posix()):
                 pass
 
             assert sftp.getcwd() == '/'
```

### Comparing `sftpretty-1.0.8/tests/test_listdir.py` & `sftpretty-1.0.9/tests/test_listdir.py`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/tests/test_logging.py` & `sftpretty-1.0.9/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/tests/test_mkdir.py` & `sftpretty-1.0.9/tests/test_mkdir.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''test sftpretty.mkdir'''
 
-from common import VFS, conn, SKIP_IF_CI
-from sftpretty import Connection, st_mode_to_int
+from common import conn, VFS
+from sftpretty import Connection
+from sftpretty.helpers import st_mode_to_int
 
 
-@SKIP_IF_CI
 def test_mkdir_mode(lsftp):
     '''test mkdir with mode set to 711'''
     dirname = 'test-dir'
-    mode = 711
+    mode = 700
     assert dirname not in lsftp.listdir()
     lsftp.mkdir(dirname, mode=mode)
     attrs = lsftp.stat(dirname)
     lsftp.rmdir(dirname)
     assert st_mode_to_int(attrs.st_mode) == mode
```

### Comparing `sftpretty-1.0.8/tests/test_open.py` & `sftpretty-1.0.9/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/tests/test_put.py` & `sftpretty-1.0.9/tests/test_put.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 '''test sftpretty.put'''
 
 import pytest
 
-from common import conn, SKIP_IF_CI, tempfile_containing, VFS
+from common import conn, tempfile_containing, VFS
 from pathlib import Path
 from sftpretty import Connection
 from time import sleep
 from unittest.mock import Mock
 
 
-@SKIP_IF_CI
 def test_put_callback(lsftp):
     '''test the callback feature of put'''
     cback = Mock(return_value=None)
     with tempfile_containing() as fname:
         base_fname = Path(fname).name
-        lsftp.chdir('/home/test')
+        lsftp.chdir(Path.home().as_posix())
         lsftp.put(fname, callback=cback)
         # clean up
         lsftp.remove(base_fname)
     # verify callback was called
     assert cback.call_count
 
 
-@SKIP_IF_CI
 def test_put_confirm(lsftp):
     '''test the confirm feature of put'''
     with tempfile_containing() as fname:
         base_fname = Path(fname).name
-        lsftp.chdir('/home/test')
+        lsftp.chdir(Path.home().as_posix())
         result = lsftp.put(fname)
         # clean up
         lsftp.remove(base_fname)
     # verify that an SFTPAttribute like Path.stat() was returned
     assert result.st_size == 8192
     assert result.st_uid is not None
     assert result.st_gid is not None
     assert result.st_atime
     assert result.st_mtime
 
 
-@SKIP_IF_CI
 def test_put(lsftp):
     '''run test on localhost'''
     contents = 'now is the time\nfor all good...'
     with tempfile_containing(contents=contents) as fname:
         base_fname = Path(fname).name
         if base_fname in lsftp.listdir():
             lsftp.remove(base_fname)
@@ -73,21 +70,20 @@
 # def test_put_not_allowed(psftp):
 #     '''try to put a file to a read-only server'''
 #     with tempfile_containing() as fname:
 #         with pytest.raises(IOError):
 #             psftp.put(fname)
 
 
-@SKIP_IF_CI
 def test_put_preserve_mtime(lsftp):
     '''test that m_time is preserved from local to remote, when put'''
     with tempfile_containing() as fname:
         base_fname = Path(fname).name
         base = Path(fname).stat()
-        # with Connection(**SFTP_LOCAL) as sftp:
+        # with Connection(**LOCAL) as sftp:
         result1 = lsftp.put(fname, preserve_mtime=True)
         sleep(2)
         result2 = lsftp.put(fname, preserve_mtime=True)
         # clean up
         lsftp.remove(base_fname)
     # see if times are modified
     # assert base.st_atime == result1.st_atime
```

### Comparing `sftpretty-1.0.8/tests/test_put_d.py` & `sftpretty-1.0.9/tests/test_put_d.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 '''test sftpretty.put_d'''
 
 import pytest
 
 from blddirs import build_dir_struct
-from common import SKIP_IF_CI
+from common import rmdir
 from pathlib import Path
 from tempfile import mkdtemp
 
 
-# TODO 1
-@SKIP_IF_CI
 def test_put_d(lsftp):
     '''test put_d'''
-    localpath = mkdtemp()
-    print(localpath)
-    remote_dir = Path(localpath).stem
+    localpath = Path(mkdtemp()).as_posix()
+    remote = Path.home()
     build_dir_struct(localpath)
-    localpath = Path(localpath).joinpath('pub').as_posix()
-    print(localpath)
-    # run the op
-    lsftp.put_d(localpath, remote_dir)
-
-    # inspect results
-
-    # cleanup remote
-    lsftp.rmdir(remote_dir)
-
-    # cleanup local
-    Path(localpath).rmdir()
+    local = Path(localpath).joinpath('pub')
+    lsftp.put_d(local.as_posix(), remote.as_posix())
 
-    # check results
+    rmdir(localpath)
 
 
 # TODO
 # def test_put_d_ro(psftp):
 #     '''test put_d failure on remote read-only srvr'''
 #     # run the op
 #     with pytest.raises(IOError):
 #         psftp.put_d('.', '.')
 
 
-@SKIP_IF_CI
 def test_put_d_bad_local(lsftp):
     '''test put_d failure on non-existing local directory'''
     # run the op
     with pytest.raises(OSError):
         lsftp.put_d('/non-existing', '.')
```

### Comparing `sftpretty-1.0.8/tests/test_put_r.py` & `sftpretty-1.0.9/tests/test_put_r.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 '''test sftpretty.put_r'''
 
 import pytest
 
 from blddirs import build_dir_struct
-from common import SKIP_IF_CI
+from common import rmdir
 from pathlib import Path
 from tempfile import mkdtemp
 
 
-# TODO 2
-@SKIP_IF_CI
 def test_put_r(lsftp):
     '''test put_r'''
-    localpath = mkdtemp()
-    print(localpath)
-    remote_dir = Path(localpath).stem
+    localpath = Path(mkdtemp()).as_posix()
+    remote = Path.home()
     build_dir_struct(localpath)
-    localpath = Path(localpath).joinpath('pub').as_posix()
-    print(localpath)
-    # run the op
-    lsftp.put_r(localpath, remote_dir)
-
-    # inspect results
-
-    # cleanup remote
-    lsftp.rmdir(remote_dir)
-
-    # cleanup local
-    Path(Path(localpath).parent.as_posix()).rmdir()
+    local = Path(localpath).joinpath('pub')
+    lsftp.put_r(local.as_posix(), remote.as_posix())
 
-    # check results
+    rmdir(localpath)
 
 
 # TODO
 # def test_put_r_ro(psftp):
 #     '''test put_r failure on remote read-only srvr'''
 #     # run the op
 #     with pytest.raises(IOError):
 #         psftp.put_r('.', '.')
 
 
-@SKIP_IF_CI
 def test_put_r_bad_local(lsftp):
     '''test put_r failure on non-existing local directory'''
     # run the op
     with pytest.raises(OSError):
         lsftp.put_r('/non-existing', '.')
```

### Comparing `sftpretty-1.0.8/tests/test_remote_server_key.py` & `sftpretty-1.0.9/tests/test_remote_server_key.py`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/tests/test_rename.py` & `sftpretty-1.0.9/tests/test_rename.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 '''test sftpretty.rename'''
 
-from common import SKIP_IF_CI, tempfile_containing
+from common import tempfile_containing
 from pathlib import Path
 
 
-@SKIP_IF_CI
 def test_rename(lsftp):
     '''test rename on remote'''
     contents = 'now is the time\nfor all good...'
     with tempfile_containing(contents=contents) as fname:
         base_fname = Path(fname).name
         if base_fname in lsftp.listdir():
             lsftp.remove(base_fname)
@@ -21,8 +20,8 @@
         lsftp.remove('bob')
 
 
 # TODO
 # def test_rename_ro(psftp):
 #     '''test rename on a read-only server'''
 #     with pytest.raises(IOError):
-#         psftp.rename('/home/test/readme.txt', 'bob')
+#         psftp.rename('readme.txt', 'bob')
```

### Comparing `sftpretty-1.0.8/tests/test_retry.py` & `sftpretty-1.0.9/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `sftpretty-1.0.8/tests/test_sftp.py` & `sftpretty-1.0.9/tests/test_sftp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 '''test sftpretty module'''
 
-# psftp and lsftp fixtures are from conftest.py
-
-from common import conn, SKIP_IF_CI, tempfile_containing, VFS
+from common import conn, LOCAL, tempfile_containing, VFS
 from pathlib import Path
 from sftpretty import Connection
 from stat import S_ISLNK
 
 
-@SKIP_IF_CI
 def test_sftp_client(lsftp):
     '''test for access to the underlying, active sftpclient'''
-    # with Connection(**SFTP_PUBLIC) as sftp:
-    #     assert 'normalize' in dir(sftp.sftp_client)
-    #     assert 'readlink' in dir(sftp.sftp_client)
+    with Connection(**LOCAL) as sftp:
+        assert 'normalize' in dir(sftp.sftp_client)
+        assert 'readlink' in dir(sftp.sftp_client)
     assert 'normalize' in dir(lsftp.sftp_client)
     assert 'readlink' in dir(lsftp.sftp_client)
 
 
-@SKIP_IF_CI
 def test_mkdir_p(lsftp):
     '''test mkdir_p simple, testing 2 things, oh well'''
     rdir = 'foo/bar/baz'
     rdir2 = 'foo/bar'
     assert lsftp.exists(rdir) is False
     lsftp.mkdir_p(rdir)
     is_dir = lsftp.isdir(rdir)
     lsftp.rmdir(rdir)
     lsftp.rmdir(rdir2)
-    lsftp.mkdir_p(rdir)     # try partially existing path
+    lsftp.mkdir_p(rdir)
     is_dir_partial = lsftp.isdir(rdir)
     lsftp.rmdir(rdir)
     lsftp.rmdir(rdir2)
     lsftp.rmdir('foo')
     assert is_dir
     assert is_dir_partial
 
 
 # def test_lexists_symbolic(psftp):
 #     '''test .lexists() vs. symbolic link'''
 #     rsym = 'readme.sym'
 #     assert psftp.lexists(rsym)
 
 
-@SKIP_IF_CI
 def test_symlink(lsftp):
     '''test symlink creation'''
-    rdest = '/home/test/honey-boo-boo'
+    rdest = Path.home().joinpath('honey-boo-boo')
     with tempfile_containing() as fname:
         lsftp.put(fname)
-        lsftp.symlink(fname, rdest)
-        rslt = lsftp.lstat(rdest)
+        lsftp.symlink(fname, rdest.as_posix())
+        rslt = lsftp.lstat(rdest.as_posix())
         is_link = S_ISLNK(rslt.st_mode)
-        lsftp.remove(rdest)
+        lsftp.remove(rdest.as_posix())
         lsftp.remove(Path(fname).name)
     assert is_link
 
 
 def test_exists(sftpserver):
     '''test .exists() fuctionality'''
     with sftpserver.serve_content(VFS):
@@ -64,18 +59,16 @@
             rfile = 'pub/foo2/bar1/bar1.txt'
             rbad = 'pub/foo2/bar1/peek-a-boo.txt'
             assert sftp.exists(rfile)
             assert sftp.exists(rbad) is False
             assert sftp.exists('pub')
 
 
-@SKIP_IF_CI
 def test_lexists(lsftp):
     '''test .lexists() functionality'''
     with tempfile_containing() as fname:
         base_fname = Path(fname).name
         lsftp.put(fname)
-        # rfile = '/home/test/readme.txt'
-        rbad = '/home/test/peek-a-boo.txt'
+        rbad = Path.home().joinpath('peek-a-boo.txt')
         assert lsftp.lexists(fname)
         lsftp.remove(base_fname)
-        assert lsftp.lexists(rbad) is False
+        assert lsftp.lexists(rbad.as_posix()) is False
```

### Comparing `sftpretty-1.0.8/tests/test_stat_lstat.py` & `sftpretty-1.0.9/tests/test_stat_lstat.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 '''test sftpretty.stat and .lstat'''
 
-from common import VFS, conn, SKIP_IF_CI
+from blddirs import build_dir_struct
+from common import conn, rmdir, VFS
+from pathlib import Path
 from sftpretty import Connection
+from tempfile import mkdtemp
 
 
 def test_stat(sftpserver):
     '''test stat'''
     with sftpserver.serve_content(VFS):
         with Connection(**conn(sftpserver)) as sftp:
             dirname = 'pub'
             rslt = sftp.stat(dirname)
             assert rslt.st_size >= 0
 
 
-@SKIP_IF_CI
 def test_lstat(lsftp):
-    '''test lstat  minimal, have to use real server, plugin doesn't support
+    '''test lstat minimal, have to use real server, plugin doesn't support
     lstat'''
-    dirname = 'pub'
-    lsftp.mkdir(dirname)
-    lsftp.chdir('/home/test')
+    localpath = Path(mkdtemp()).as_posix()
+    build_dir_struct(localpath)
+    dirname = Path(localpath).joinpath('pub').as_posix()
     rslt = lsftp.lstat(dirname)
-    lsftp.rmdir(dirname)
+
     assert rslt.st_size >= 0
+
+    rmdir(localpath)
```

### Comparing `sftpretty-1.0.8/tests/test_truncate.py` & `sftpretty-1.0.9/tests/test_truncate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 '''test sftpretty.listdir'''
 
-from common import SKIP_IF_CI, STARS8192
+from common import STARS8192
 from io import BytesIO
 
 
-@SKIP_IF_CI
 def test_truncate_smaller(lsftp):
     '''test truncate, make file smaller'''
     flo = BytesIO(bytes(STARS8192, 'UTF-8'))
     rname = 'truncate.txt'
     try:
         lsftp.remove(rname)
     except IOError:
         pass
     lsftp.putfo(flo, rname)
     new_size = lsftp.truncate(rname, 4096)
     assert new_size == 4096
     lsftp.remove(rname)
 
 
-@SKIP_IF_CI
 def test_truncate_larger(lsftp):
     '''test truncate, make file larger'''
     flo = BytesIO(bytes(STARS8192, 'UTF-8'))
     rname = 'truncate.txt'
     try:
         lsftp.remove(rname)
     except IOError:
         pass
     lsftp.putfo(flo, rname)
     new_size = lsftp.truncate(rname, 2*8192)
     assert new_size == 2*8192
     lsftp.remove(rname)
 
 
-@SKIP_IF_CI
 def test_truncate_same(lsftp):
     '''test truncate, make file same size'''
     flo = BytesIO(bytes(STARS8192, 'UTF-8'))
     rname = 'truncate.txt'
     try:
         lsftp.remove(rname)
     except IOError:
@@ -48,10 +45,10 @@
     assert new_size == 8192
     lsftp.remove(rname)
 
 
 # TODO
 # def test_truncate_ro(psftp):
 #     '''test truncate, against read-only server'''
-#     rname = '/home/test/readme.txt'
+#     rname = Path.home().joinpath('readme.txt').as_posix()
 #     with pytest.raises(IOError):
 #         _ = psftp.truncate(rname, 8192)
```

### Comparing `sftpretty-1.0.8/tests/test_username.py` & `sftpretty-1.0.9/tests/test_username.py`

 * *Files identical despite different names*

