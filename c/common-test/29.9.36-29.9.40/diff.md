# Comparing `tmp/common-test-29.9.36.tar.gz` & `tmp/common-test-29.9.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-test-29.9.36.tar", last modified: Tue May  9 01:49:55 2023, max compression
+gzip compressed data, was "common-test-29.9.40.tar", last modified: Wed May 10 06:50:37 2023, max compression
```

## Comparing `common-test-29.9.36.tar` & `common-test-29.9.40.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:55.020889 common-test-29.9.36/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-09 01:49:55.021028 common-test-29.9.36/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:54.979515 common-test-29.9.36/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.36/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:54.981644 common-test-29.9.36/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.36/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 common-test-29.9.36/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.36/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.36/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:54.984236 common-test-29.9.36/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.36/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.36/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.36/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.36/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:54.985273 common-test-29.9.36/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.36/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.36/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:54.987784 common-test-29.9.36/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.36/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17412 2023-05-06 06:06:25.000000 common-test-29.9.36/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.36/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:54.991626 common-test-29.9.36/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.36/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.36/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.36/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.36/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.36/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.36/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:55.001400 common-test-29.9.36/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.36/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.36/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.36/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.36/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.36/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.36/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.36/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:55.002653 common-test-29.9.36/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.36/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.36/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:55.010509 common-test-29.9.36/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3531 2023-05-08 04:08:54.000000 common-test-29.9.36/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.36/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.36/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)    13609 2023-05-05 06:58:50.000000 common-test-29.9.36/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     5059 2023-05-05 07:02:08.000000 common-test-29.9.36/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8570 2023-05-08 05:47:33.000000 common-test-29.9.36/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:55.017625 common-test-29.9.36/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.36/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.36/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.36/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     8116 2023-05-09 01:24:22.000000 common-test-29.9.36/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6706 2023-05-08 05:48:27.000000 common-test-29.9.36/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.36/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.36/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.36/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.36/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    16834 2023-05-08 03:28:26.000000 common-test-29.9.36/common/plugin/pytest_plugin.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-09 01:49:55.020552 common-test-29.9.36/common_test.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-09 01:49:54.000000 common-test-29.9.36/common_test.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-09 01:49:54.000000 common-test-29.9.36/common_test.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-09 01:49:54.000000 common-test-29.9.36/common_test.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-09 01:49:54.000000 common-test-29.9.36/common_test.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-09 01:49:54.000000 common-test-29.9.36/common_test.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-09 01:49:54.000000 common-test-29.9.36/common_test.egg-info/top_level.txt
--rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-09 01:49:55.021783 common-test-29.9.36/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.36/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.639226 common-test-29.9.40/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-10 06:50:37.639351 common-test-29.9.40/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.606327 common-test-29.9.40/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 common-test-29.9.40/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.608648 common-test-29.9.40/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 common-test-29.9.40/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 common-test-29.9.40/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 common-test-29.9.40/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 common-test-29.9.40/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.611263 common-test-29.9.40/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 common-test-29.9.40/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 common-test-29.9.40/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3578 2023-05-08 02:03:18.000000 common-test-29.9.40/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 common-test-29.9.40/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.612283 common-test-29.9.40/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.40/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 common-test-29.9.40/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.615192 common-test-29.9.40/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 common-test-29.9.40/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17412 2023-05-06 06:06:25.000000 common-test-29.9.40/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8662 2023-04-23 07:58:21.000000 common-test-29.9.40/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.619295 common-test-29.9.40/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.40/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3436 2023-04-14 00:29:00.000000 common-test-29.9.40/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 common-test-29.9.40/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 common-test-29.9.40/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 common-test-29.9.40/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 common-test-29.9.40/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.624854 common-test-29.9.40/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 common-test-29.9.40/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 common-test-29.9.40/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11091 2023-05-05 06:58:50.000000 common-test-29.9.40/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-04-14 00:29:00.000000 common-test-29.9.40/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 common-test-29.9.40/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 common-test-29.9.40/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 common-test-29.9.40/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.626320 common-test-29.9.40/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 common-test-29.9.40/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 common-test-29.9.40/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.630209 common-test-29.9.40/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3531 2023-05-08 04:08:54.000000 common-test-29.9.40/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 common-test-29.9.40/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 common-test-29.9.40/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)    13650 2023-05-10 06:42:48.000000 common-test-29.9.40/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     5059 2023-05-05 07:02:08.000000 common-test-29.9.40/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8570 2023-05-08 05:47:33.000000 common-test-29.9.40/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.636839 common-test-29.9.40/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 common-test-29.9.40/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 common-test-29.9.40/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 common-test-29.9.40/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     8263 2023-05-10 00:52:04.000000 common-test-29.9.40/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6651 2023-05-10 00:52:04.000000 common-test-29.9.40/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3721 2023-05-04 05:30:58.000000 common-test-29.9.40/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    10894 2023-05-08 02:03:18.000000 common-test-29.9.40/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 common-test-29.9.40/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 common-test-29.9.40/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    16835 2023-05-10 05:59:48.000000 common-test-29.9.40/common/plugin/pytest_plugin.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-10 06:50:37.638935 common-test-29.9.40/common_test.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      623 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1475 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       57 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-10 06:50:37.000000 common-test-29.9.40/common_test.egg-info/top_level.txt
+-rw-r--r--   0 edz        (502) staff       (20)      440 2023-05-10 06:50:37.640488 common-test-29.9.40/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1641 2023-05-04 07:57:23.000000 common-test-29.9.40/setup.py
```

### Comparing `common-test-29.9.36/PKG-INFO` & `common-test-29.9.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.36
+Version: 29.9.40
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.36/common/autotest/base_requests.py` & `common-test-29.9.40/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/autotest/handle_allure.py` & `common-test-29.9.40/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/autotest/handle_assert.py` & `common-test-29.9.40/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/common/api_driver.py` & `common-test-29.9.40/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/common/constant.py` & `common-test-29.9.40/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/common/test.py` & `common-test-29.9.40/common/common/test.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/config/config.py` & `common-test-29.9.40/common/config/config.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/data/data_process.py` & `common-test-29.9.40/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/data/handle_common.py` & `common-test-29.9.40/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/db/handle_db.py` & `common-test-29.9.40/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/db/handle_db_batch.py` & `common-test-29.9.40/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/db/handle_mysqldb.py` & `common-test-29.9.40/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/db/handle_oracle.py` & `common-test-29.9.40/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/db/handle_sqlserver.py` & `common-test-29.9.40/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/file/ReadFile.py` & `common-test-29.9.40/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/file/handle_excel.py` & `common-test-29.9.40/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/file/handle_file.py` & `common-test-29.9.40/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/file/handle_reques.py` & `common-test-29.9.40/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/file/handle_system.py` & `common-test-29.9.40/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/file/handle_yaml.py` & `common-test-29.9.40/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/mq/handle_rabbit.py` & `common-test-29.9.40/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plat/ATF_platform.py` & `common-test-29.9.40/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plat/jenkin_platform.py` & `common-test-29.9.40/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plat/jira_platform.py` & `common-test-29.9.40/common/plat/jira_platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         try:
             case_desc = json.loads(JiraPlatForm.getJiraIssueInfo(testCaseIssueKey + '?fields=description').content)['fields']['description']
             if DataProcess.isNotNull(case_desc) == False or str(case_desc).strip() != desc.strip():
                 APIDriver.http_request(
                     url=f"{Constant.JIRA_URL}/rest/api/2/issue/{testCaseIssueKey}",
                     method='put',
                     parametric_key='json',
-                    data={"fields" : {"description": f"{desc}"}},
+                    data={"fields" : {"description": f"{desc}","customfield_14903":{"value":"自动化"}}},
                     _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD))
                 )
         except Exception as e:
             logger.info(f' 用例Key:{testCaseIssueKey} 描述信息:{desc} 更新用例描述异常:{e}')
 
     @classmethod
     def getDataByJql(self, jql, fields):
@@ -285,8 +285,7 @@
                 method='get',
                 _auth=HTTPBasicAuth(get_system_key(Constant.JIRA_USERNAME), get_system_key(Constant.JIRA_PASSWORD)))
             cycleInfo = jsonpath(json.loads(content.content), f'$.[?(@.id=={cycle_id})]')[0]
             return cycleInfo
         except Exception as e:
             logger.info(f'获取测试计划：{testPlanIssueKey}中周期{cycle_id}信息异常信息:'+repr(e))
             return ""
-
```

### Comparing `common-test-29.9.36/common/plat/mysql_platform.py` & `common-test-29.9.40/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plat/service_platform.py` & `common-test-29.9.40/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plugin/allure_plugin.py` & `common-test-29.9.40/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plugin/assert_plugin.py` & `common-test-29.9.40/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plugin/atf_plugin.py` & `common-test-29.9.40/common/plugin/atf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,18 @@
                 uid = uids[i]
                 _caseurl = f'{buildurl}allure/#behaviors/{parentUid}/{uid}'
                 _caseTitleList = caseName[i].split(';')
                 for temp in _caseTitleList:
                     ATFPlatForm.sent_result_byCaseName(temp, "", "", _caseurl)
 
 
+if __name__ == '__main__':
+    print(ATFPlugin.db_ops("psn", "select * from flight_quota where FLIGHT_NO = 'MU5119' ORDER BY FLIGHT_DATE desc"))
+
+
```

### Comparing `common-test-29.9.36/common/plugin/data_bus.py` & `common-test-29.9.40/common/plugin/data_bus.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,16 +180,15 @@
         print_databus_info(Constant.TEST_CASE_MARK, "用例等级")
         print_databus_info(Constant.TEST_TYPE, "测试集类型")
         print_databus_info(Constant.RUN_TYPE, "运行方式")
         print_databus_info(Constant.ENV, "运行环境")
         print_databus_info(Constant.PASS_RATE,"预期通过率")
         print_databus_info(Constant.SEND_URSER_LIST, "通知人列表")
 
-if __name__ == '__main__':
-    DataBus.save_init_data()
+
```

### Comparing `common-test-29.9.36/common/plugin/data_plugin.py` & `common-test-29.9.40/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plugin/file_plugin.py` & `common-test-29.9.40/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plugin/hooks_plugin.py` & `common-test-29.9.40/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plugin/pytest_playwright.py` & `common-test-29.9.40/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common/plugin/pytest_plugin.py` & `common-test-29.9.40/common/plugin/pytest_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         if DataProcess.isNotNull(_caseNo) and _caseNo != '00000':
             _caseTitleList.extend(_caseNo.split(';'))
         if DataProcess.isNotNull(_caseTitleList):
             caseInfoList = ""
             if DataProcess.isNotNull(get_system_key('type')) and get_system_key('type').strip() == '脚本同步':
                 logger.info(f"---获取用例列表：{_caseTitleList} 脚本路径:{_caseurl} 执行状态:用例同步")
                 for _name in _caseTitleList:
-                    if DataProcess.isNotNull(_name) and _name !='00000':
+                    if DataProcess.isNotNull(_name) and _name != '00000':
                         info = ATFPlatForm.getCaseInfoByNameOrID(_name)
                         caseInfoList = caseInfoList + _name + "(" + info['key'] + "),"
                         MysqlPlatForm.sync_autotest_script(info['summary'], info['key'], _caseurl)
                 logger.info(f"---用例列表：{caseInfoList} 脚本路径:{_caseurl}  执行状态:同步成功")
                 assert "测试用例检查" == "脚本用例同步【执行结果可忽略】"
             if PytestPlugin.checkCaseRun(item, _caseTitle, _caseNo) == False:
                 logger.info(f"---获取用例列表：{_caseTitleList} 脚本路径:{_caseurl} 执行状态:执行中断")
```

### Comparing `common-test-29.9.36/common_test.egg-info/PKG-INFO` & `common-test-29.9.40/common_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: common-test
-Version: 29.9.36
+Version: 29.9.40
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: shiqiang.ou
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `common-test-29.9.36/common_test.egg-info/SOURCES.txt` & `common-test-29.9.40/common_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/common_test.egg-info/requires.txt` & `common-test-29.9.40/common_test.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `common-test-29.9.36/setup.py` & `common-test-29.9.40/setup.py`

 * *Files identical despite different names*

