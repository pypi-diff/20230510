# Comparing `tmp/kuto-0.0.5.tar.gz` & `tmp/kuto-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuto-0.0.5.tar", last modified: Tue May  9 12:14:15 2023, max compression
+gzip compressed data, was "kuto-0.0.6.tar", last modified: Wed May 10 02:03:44 2023, max compression
```

## Comparing `kuto-0.0.5.tar` & `kuto-0.0.6.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.257390 kuto-0.0.5/
--rw-r--r--   0 UI         (502) staff       (20)      374 2023-05-09 12:14:15.256953 kuto-0.0.5/PKG-INFO
--rw-r--r--   0 UI         (502) staff       (20)    17952 2023-05-09 12:13:54.000000 kuto-0.0.5/README.md
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.216770 kuto-0.0.5/demo/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-10-17 07:22:13.000000 kuto-0.0.5/demo/__init__.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.218135 kuto-0.0.5/demo/page/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-07 03:31:21.000000 kuto-0.0.5/demo/page/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      394 2023-04-25 02:58:48.000000 kuto-0.0.5/demo/page/adr_page.py
--rw-r--r--   0 UI         (502) staff       (20)      394 2023-04-25 02:58:48.000000 kuto-0.0.5/demo/page/web_page.py
--rw-r--r--   0 UI         (502) staff       (20)     1157 2023-05-09 12:05:01.000000 kuto-0.0.5/demo/run.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.221423 kuto-0.0.5/demo/tests/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-07 03:29:41.000000 kuto-0.0.5/demo/tests/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      476 2023-05-09 02:31:22.000000 kuto-0.0.5/demo/tests/test_adr.py
--rw-r--r--   0 UI         (502) staff       (20)      423 2023-05-09 01:53:13.000000 kuto-0.0.5/demo/tests/test_api.py
--rw-r--r--   0 UI         (502) staff       (20)      435 2023-05-09 02:33:26.000000 kuto-0.0.5/demo/tests/test_ios.py
--rw-r--r--   0 UI         (502) staff       (20)      829 2023-05-09 12:05:01.000000 kuto-0.0.5/demo/tests/test_param.py
--rw-r--r--   0 UI         (502) staff       (20)      680 2023-05-09 12:01:30.000000 kuto-0.0.5/demo/tests/test_web.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.224289 kuto-0.0.5/kuto/
--rw-r--r--   0 UI         (502) staff       (20)      580 2023-05-09 12:09:33.000000 kuto-0.0.5/kuto/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     9787 2023-05-09 12:07:43.000000 kuto-0.0.5/kuto/case.py
--rw-r--r--   0 UI         (502) staff       (20)     2057 2023-04-25 02:58:48.000000 kuto-0.0.5/kuto/cli.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.226551 kuto-0.0.5/kuto/core/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-02-03 12:13:24.000000 kuto-0.0.5/kuto/core/__init__.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.228978 kuto-0.0.5/kuto/core/android/
--rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 12:42:07.000000 kuto-0.0.5/kuto/core/android/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      901 2023-04-25 02:58:48.000000 kuto-0.0.5/kuto/core/android/common.py
--rw-r--r--   0 UI         (502) staff       (20)     9622 2023-05-09 02:26:49.000000 kuto-0.0.5/kuto/core/android/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     6964 2023-05-08 12:55:06.000000 kuto-0.0.5/kuto/core/android/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.229925 kuto-0.0.5/kuto/core/api/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-10-17 03:04:55.000000 kuto-0.0.5/kuto/core/api/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    14686 2023-05-09 12:07:10.000000 kuto-0.0.5/kuto/core/api/request.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.231129 kuto-0.0.5/kuto/core/h5/
--rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 13:04:56.000000 kuto-0.0.5/kuto/core/h5/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     7220 2023-05-09 02:28:20.000000 kuto-0.0.5/kuto/core/h5/driver.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.232920 kuto-0.0.5/kuto/core/image/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-12-11 09:49:05.000000 kuto-0.0.5/kuto/core/image/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     2855 2023-05-08 12:35:04.000000 kuto-0.0.5/kuto/core/image/element.py
--rw-r--r--   0 UI         (502) staff       (20)     2414 2023-05-08 12:29:45.000000 kuto-0.0.5/kuto/core/image/image_discern.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.235479 kuto-0.0.5/kuto/core/ios/
--rw-r--r--   0 UI         (502) staff       (20)        2 2022-09-21 12:53:47.000000 kuto-0.0.5/kuto/core/ios/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     2155 2023-04-25 02:58:48.000000 kuto-0.0.5/kuto/core/ios/common.py
--rw-r--r--   0 UI         (502) staff       (20)     7599 2023-05-09 02:28:44.000000 kuto-0.0.5/kuto/core/ios/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     7953 2023-05-08 12:55:23.000000 kuto-0.0.5/kuto/core/ios/element.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.237122 kuto-0.0.5/kuto/core/ocr/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-12-11 09:48:37.000000 kuto-0.0.5/kuto/core/ocr/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     2296 2023-05-08 12:33:55.000000 kuto-0.0.5/kuto/core/ocr/element.py
--rw-r--r--   0 UI         (502) staff       (20)     2839 2023-05-08 12:29:45.000000 kuto-0.0.5/kuto/core/ocr/ocr_discern.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.238170 kuto-0.0.5/kuto/core/sonic/
--rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-20 03:43:29.000000 kuto-0.0.5/kuto/core/sonic/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     4111 2023-04-25 02:58:48.000000 kuto-0.0.5/kuto/core/sonic/sib_util.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.240317 kuto-0.0.5/kuto/core/web/
--rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 13:04:56.000000 kuto-0.0.5/kuto/core/web/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    13075 2023-05-09 02:26:58.000000 kuto-0.0.5/kuto/core/web/driver.py
--rw-r--r--   0 UI         (502) staff       (20)     9474 2023-05-08 12:54:24.000000 kuto-0.0.5/kuto/core/web/element.py
--rw-r--r--   0 UI         (502) staff       (20)     2065 2023-04-23 03:42:32.000000 kuto-0.0.5/kuto/general.py
--rw-r--r--   0 UI         (502) staff       (20)     3261 2023-04-25 02:58:48.000000 kuto-0.0.5/kuto/page.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.242400 kuto-0.0.5/kuto/running/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-05-05 11:41:00.000000 kuto-0.0.5/kuto/running/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)      191 2023-05-09 12:02:18.000000 kuto-0.0.5/kuto/running/conf.yml
--rw-r--r--   0 UI         (502) staff       (20)       72 2022-12-07 07:03:15.000000 kuto-0.0.5/kuto/running/config.py
--rw-r--r--   0 UI         (502) staff       (20)     3946 2023-05-09 01:57:33.000000 kuto-0.0.5/kuto/running/runner.py
--rw-r--r--   0 UI         (502) staff       (20)     5024 2023-05-09 12:05:01.000000 kuto-0.0.5/kuto/scaffold.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.243079 kuto-0.0.5/kuto/testdata/
--rw-r--r--   0 UI         (502) staff       (20)    10654 2023-05-09 12:13:54.000000 kuto-0.0.5/kuto/testdata/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)    18623 2022-09-29 09:22:30.000000 kuto-0.0.5/kuto/testdata/data.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.256060 kuto-0.0.5/kuto/utils/
--rw-r--r--   0 UI         (502) staff       (20)        0 2022-05-05 11:41:00.000000 kuto-0.0.5/kuto/utils/__init__.py
--rw-r--r--   0 UI         (502) staff       (20)     5785 2023-05-08 12:29:45.000000 kuto-0.0.5/kuto/utils/allure_data.py
--rw-r--r--   0 UI         (502) staff       (20)      348 2023-05-09 02:23:26.000000 kuto-0.0.5/kuto/utils/allure_util.py
--rw-r--r--   0 UI         (502) staff       (20)     2304 2023-03-20 05:44:26.000000 kuto-0.0.5/kuto/utils/config.py
--rw-r--r--   0 UI         (502) staff       (20)     3310 2023-05-09 11:58:34.000000 kuto-0.0.5/kuto/utils/decorate.py
--rw-r--r--   0 UI         (502) staff       (20)     3276 2023-05-08 12:29:45.000000 kuto-0.0.5/kuto/utils/dingtalk.py
--rw-r--r--   0 UI         (502) staff       (20)      780 2022-10-26 06:34:19.000000 kuto-0.0.5/kuto/utils/encrypt.py
--rw-r--r--   0 UI         (502) staff       (20)     4438 2023-04-03 00:59:14.000000 kuto-0.0.5/kuto/utils/excel.py
--rw-r--r--   0 UI         (502) staff       (20)     1795 2023-03-20 09:31:36.000000 kuto-0.0.5/kuto/utils/exceptions.py
--rw-r--r--   0 UI         (502) staff       (20)      450 2023-03-27 10:02:36.000000 kuto-0.0.5/kuto/utils/log.py
--rw-r--r--   0 UI         (502) staff       (20)     3895 2023-05-09 12:13:54.000000 kuto-0.0.5/kuto/utils/mail.py
--rw-r--r--   0 UI         (502) staff       (20)     2009 2022-10-17 03:26:18.000000 kuto-0.0.5/kuto/utils/mongo_util.py
--rw-r--r--   0 UI         (502) staff       (20)     2149 2022-10-17 03:26:26.000000 kuto-0.0.5/kuto/utils/mysql_util.py
--rw-r--r--   0 UI         (502) staff       (20)     1719 2023-04-25 02:58:48.000000 kuto-0.0.5/kuto/utils/read_file.py
--rw-r--r--   0 UI         (502) staff       (20)      656 2023-05-09 11:39:05.000000 kuto-0.0.5/kuto/utils/schema_util.py
--rw-r--r--   0 UI         (502) staff       (20)     2177 2022-05-05 11:41:00.000000 kuto-0.0.5/kuto/utils/swagger_util.py
--rw-r--r--   0 UI         (502) staff       (20)     1662 2022-05-05 11:41:00.000000 kuto-0.0.5/kuto/utils/webdriver_manager_extend.py
-drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-09 12:14:15.226229 kuto-0.0.5/kuto.egg-info/
--rw-r--r--   0 UI         (502) staff       (20)      374 2023-05-09 12:14:15.000000 kuto-0.0.5/kuto.egg-info/PKG-INFO
--rw-r--r--   0 UI         (502) staff       (20)     1698 2023-05-09 12:14:15.000000 kuto-0.0.5/kuto.egg-info/SOURCES.txt
--rw-r--r--   0 UI         (502) staff       (20)        1 2023-05-09 12:14:15.000000 kuto-0.0.5/kuto.egg-info/dependency_links.txt
--rw-r--r--   0 UI         (502) staff       (20)       39 2023-05-09 12:14:15.000000 kuto-0.0.5/kuto.egg-info/entry_points.txt
--rw-r--r--   0 UI         (502) staff       (20)      539 2023-05-09 12:14:15.000000 kuto-0.0.5/kuto.egg-info/requires.txt
--rw-r--r--   0 UI         (502) staff       (20)       10 2023-05-09 12:14:15.000000 kuto-0.0.5/kuto.egg-info/top_level.txt
--rw-r--r--   0 UI         (502) staff       (20)       38 2023-05-09 12:14:15.257541 kuto-0.0.5/setup.cfg
--rw-r--r--   0 UI         (502) staff       (20)     1757 2023-05-09 11:39:32.000000 kuto-0.0.5/setup.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.349923 kuto-0.0.6/
+-rw-r--r--   0 UI         (502) staff       (20)      369 2023-05-10 02:03:44.349630 kuto-0.0.6/PKG-INFO
+-rw-r--r--   0 UI         (502) staff       (20)    12753 2023-05-10 02:03:13.000000 kuto-0.0.6/README.md
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.313935 kuto-0.0.6/demo/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-10-17 07:22:13.000000 kuto-0.0.6/demo/__init__.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.315645 kuto-0.0.6/demo/page/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-07 03:31:21.000000 kuto-0.0.6/demo/page/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      394 2023-04-25 02:58:48.000000 kuto-0.0.6/demo/page/adr_page.py
+-rw-r--r--   0 UI         (502) staff       (20)      394 2023-04-25 02:58:48.000000 kuto-0.0.6/demo/page/web_page.py
+-rw-r--r--   0 UI         (502) staff       (20)     1157 2023-05-09 12:05:01.000000 kuto-0.0.6/demo/run.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.318878 kuto-0.0.6/demo/tests/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-07 03:29:41.000000 kuto-0.0.6/demo/tests/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      476 2023-05-09 02:31:22.000000 kuto-0.0.6/demo/tests/test_adr.py
+-rw-r--r--   0 UI         (502) staff       (20)      396 2023-05-10 01:46:30.000000 kuto-0.0.6/demo/tests/test_api.py
+-rw-r--r--   0 UI         (502) staff       (20)      435 2023-05-09 02:33:26.000000 kuto-0.0.6/demo/tests/test_ios.py
+-rw-r--r--   0 UI         (502) staff       (20)      827 2023-05-10 01:37:03.000000 kuto-0.0.6/demo/tests/test_para.py
+-rw-r--r--   0 UI         (502) staff       (20)      680 2023-05-09 12:01:30.000000 kuto-0.0.6/demo/tests/test_web.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.322375 kuto-0.0.6/kuto/
+-rw-r--r--   0 UI         (502) staff       (20)      580 2023-05-10 02:03:13.000000 kuto-0.0.6/kuto/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     9787 2023-05-09 12:07:43.000000 kuto-0.0.6/kuto/case.py
+-rw-r--r--   0 UI         (502) staff       (20)     2057 2023-04-25 02:58:48.000000 kuto-0.0.6/kuto/cli.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.325374 kuto-0.0.6/kuto/core/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-02-03 12:13:24.000000 kuto-0.0.6/kuto/core/__init__.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.327251 kuto-0.0.6/kuto/core/android/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 12:42:07.000000 kuto-0.0.6/kuto/core/android/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      901 2023-04-25 02:58:48.000000 kuto-0.0.6/kuto/core/android/common.py
+-rw-r--r--   0 UI         (502) staff       (20)     9622 2023-05-09 02:26:49.000000 kuto-0.0.6/kuto/core/android/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     6818 2023-05-10 01:58:39.000000 kuto-0.0.6/kuto/core/android/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.327934 kuto-0.0.6/kuto/core/api/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-10-17 03:04:55.000000 kuto-0.0.6/kuto/core/api/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    14686 2023-05-09 12:07:10.000000 kuto-0.0.6/kuto/core/api/request.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.328675 kuto-0.0.6/kuto/core/h5/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 13:04:56.000000 kuto-0.0.6/kuto/core/h5/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     7220 2023-05-09 02:28:20.000000 kuto-0.0.6/kuto/core/h5/driver.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.329989 kuto-0.0.6/kuto/core/image/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-12-11 09:49:05.000000 kuto-0.0.6/kuto/core/image/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     2855 2023-05-08 12:35:04.000000 kuto-0.0.6/kuto/core/image/element.py
+-rw-r--r--   0 UI         (502) staff       (20)     2414 2023-05-08 12:29:45.000000 kuto-0.0.6/kuto/core/image/image_discern.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.331568 kuto-0.0.6/kuto/core/ios/
+-rw-r--r--   0 UI         (502) staff       (20)        2 2022-09-21 12:53:47.000000 kuto-0.0.6/kuto/core/ios/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     2155 2023-04-25 02:58:48.000000 kuto-0.0.6/kuto/core/ios/common.py
+-rw-r--r--   0 UI         (502) staff       (20)     7599 2023-05-09 02:28:44.000000 kuto-0.0.6/kuto/core/ios/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     7827 2023-05-10 01:58:39.000000 kuto-0.0.6/kuto/core/ios/element.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.332971 kuto-0.0.6/kuto/core/ocr/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-12-11 09:48:37.000000 kuto-0.0.6/kuto/core/ocr/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     2296 2023-05-08 12:33:55.000000 kuto-0.0.6/kuto/core/ocr/element.py
+-rw-r--r--   0 UI         (502) staff       (20)     2839 2023-05-08 12:29:45.000000 kuto-0.0.6/kuto/core/ocr/ocr_discern.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.333958 kuto-0.0.6/kuto/core/sonic/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2023-03-20 03:43:29.000000 kuto-0.0.6/kuto/core/sonic/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     4111 2023-04-25 02:58:48.000000 kuto-0.0.6/kuto/core/sonic/sib_util.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.335857 kuto-0.0.6/kuto/core/web/
+-rw-r--r--   0 UI         (502) staff       (20)        1 2022-09-21 13:04:56.000000 kuto-0.0.6/kuto/core/web/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    13075 2023-05-09 02:26:58.000000 kuto-0.0.6/kuto/core/web/driver.py
+-rw-r--r--   0 UI         (502) staff       (20)     9395 2023-05-10 01:57:12.000000 kuto-0.0.6/kuto/core/web/element.py
+-rw-r--r--   0 UI         (502) staff       (20)     2065 2023-04-23 03:42:32.000000 kuto-0.0.6/kuto/general.py
+-rw-r--r--   0 UI         (502) staff       (20)     3261 2023-04-25 02:58:48.000000 kuto-0.0.6/kuto/page.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.337571 kuto-0.0.6/kuto/running/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-05-05 11:41:00.000000 kuto-0.0.6/kuto/running/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)      191 2023-05-09 12:02:18.000000 kuto-0.0.6/kuto/running/conf.yml
+-rw-r--r--   0 UI         (502) staff       (20)       72 2022-12-07 07:03:15.000000 kuto-0.0.6/kuto/running/config.py
+-rw-r--r--   0 UI         (502) staff       (20)     3946 2023-05-09 01:57:33.000000 kuto-0.0.6/kuto/running/runner.py
+-rw-r--r--   0 UI         (502) staff       (20)     5024 2023-05-09 12:05:01.000000 kuto-0.0.6/kuto/scaffold.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.338935 kuto-0.0.6/kuto/testdata/
+-rw-r--r--   0 UI         (502) staff       (20)    10654 2023-05-09 12:13:54.000000 kuto-0.0.6/kuto/testdata/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)    18623 2022-09-29 09:22:30.000000 kuto-0.0.6/kuto/testdata/data.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.348737 kuto-0.0.6/kuto/utils/
+-rw-r--r--   0 UI         (502) staff       (20)        0 2022-05-05 11:41:00.000000 kuto-0.0.6/kuto/utils/__init__.py
+-rw-r--r--   0 UI         (502) staff       (20)     5785 2023-05-08 12:29:45.000000 kuto-0.0.6/kuto/utils/allure_data.py
+-rw-r--r--   0 UI         (502) staff       (20)      348 2023-05-09 02:23:26.000000 kuto-0.0.6/kuto/utils/allure_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     2304 2023-03-20 05:44:26.000000 kuto-0.0.6/kuto/utils/config.py
+-rw-r--r--   0 UI         (502) staff       (20)     3310 2023-05-09 11:58:34.000000 kuto-0.0.6/kuto/utils/decorate.py
+-rw-r--r--   0 UI         (502) staff       (20)     3275 2023-05-10 01:54:30.000000 kuto-0.0.6/kuto/utils/dingtalk.py
+-rw-r--r--   0 UI         (502) staff       (20)      780 2022-10-26 06:34:19.000000 kuto-0.0.6/kuto/utils/encrypt.py
+-rw-r--r--   0 UI         (502) staff       (20)     4438 2023-04-03 00:59:14.000000 kuto-0.0.6/kuto/utils/excel.py
+-rw-r--r--   0 UI         (502) staff       (20)     1795 2023-03-20 09:31:36.000000 kuto-0.0.6/kuto/utils/exceptions.py
+-rw-r--r--   0 UI         (502) staff       (20)      450 2023-03-27 10:02:36.000000 kuto-0.0.6/kuto/utils/log.py
+-rw-r--r--   0 UI         (502) staff       (20)     3894 2023-05-10 01:54:39.000000 kuto-0.0.6/kuto/utils/mail.py
+-rw-r--r--   0 UI         (502) staff       (20)     2009 2022-10-17 03:26:18.000000 kuto-0.0.6/kuto/utils/mongo_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     2149 2022-10-17 03:26:26.000000 kuto-0.0.6/kuto/utils/mysql_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     1719 2023-04-25 02:58:48.000000 kuto-0.0.6/kuto/utils/read_file.py
+-rw-r--r--   0 UI         (502) staff       (20)      656 2023-05-09 11:39:05.000000 kuto-0.0.6/kuto/utils/schema_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     2177 2022-05-05 11:41:00.000000 kuto-0.0.6/kuto/utils/swagger_util.py
+-rw-r--r--   0 UI         (502) staff       (20)     1662 2022-05-05 11:41:00.000000 kuto-0.0.6/kuto/utils/webdriver_manager_extend.py
+drwxr-xr-x   0 UI         (502) staff       (20)        0 2023-05-10 02:03:44.324905 kuto-0.0.6/kuto.egg-info/
+-rw-r--r--   0 UI         (502) staff       (20)      369 2023-05-10 02:03:44.000000 kuto-0.0.6/kuto.egg-info/PKG-INFO
+-rw-r--r--   0 UI         (502) staff       (20)     1697 2023-05-10 02:03:44.000000 kuto-0.0.6/kuto.egg-info/SOURCES.txt
+-rw-r--r--   0 UI         (502) staff       (20)        1 2023-05-10 02:03:44.000000 kuto-0.0.6/kuto.egg-info/dependency_links.txt
+-rw-r--r--   0 UI         (502) staff       (20)       39 2023-05-10 02:03:44.000000 kuto-0.0.6/kuto.egg-info/entry_points.txt
+-rw-r--r--   0 UI         (502) staff       (20)      541 2023-05-10 02:03:44.000000 kuto-0.0.6/kuto.egg-info/requires.txt
+-rw-r--r--   0 UI         (502) staff       (20)       10 2023-05-10 02:03:44.000000 kuto-0.0.6/kuto.egg-info/top_level.txt
+-rw-r--r--   0 UI         (502) staff       (20)       38 2023-05-10 02:03:44.350009 kuto-0.0.6/setup.cfg
+-rw-r--r--   0 UI         (502) staff       (20)     1756 2023-05-10 01:32:00.000000 kuto-0.0.6/setup.py
```

### Comparing `kuto-0.0.5/README.md` & `kuto-0.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # 介绍
 
 [Gitee](https://gitee.com/bluepang2021/kuto)
 
-[![PyPI version](https://badge.fury.io/py/kuto.svg)](https://badge.fury.io/py/kuto) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kuto)
-![visitors](https://visitor-badge.glitch.me/badge?page_id=kuto_new.kuto)
-
 AppUI/WebUI/HTTP automation testing framework based on pytest.
 
 > 基于pytest 的 App UI/Web UI/HTTP自动化测试框架。
 
 ## 特点
 
-* 集成`facebook-wda`/`uiautomator2`/`selenium`/`requests`，支持安卓 UI/IOS UI/Web UI/HTTP测试。
-* 集成`allure`, 支持HTML格式的测试报告。
-* 提供脚手架，快速生成自动化测试项目。
-* 提供强大的`数据驱动`。
-* 提供丰富的断言。
-* 支持生成随机测试数据。
-* 支持设置用例依赖。
+* 集成`facebook-wda`/`uiautomator2`/`selenium`/`requests`
+* 支持安卓 UI/IOS UI/Web UI/HTTP接口测试
+* 集成`allure`, 支持HTML格式的测试报告
+* 提供脚手架，快速生成自动化测试项目
+* 提供强大的`数据驱动`，支持json、yaml、csv、excel
+* 提供丰富的断言
+* 支持生成随机测试数据
+* 支持设置用例依赖
 
 
 ## 三方依赖
 
 * Allure：https://github.com/allure-framework/allure2
 * WebDriverAgent：https://github.com/appium/WebDriverAgent
 
@@ -58,131 +56,122 @@
 
 * ✔️ 在`pyCharm`中右键执行(需要把项目的单元测试框架改成unittests)
 
 * ✔️ 通过命令行工具执行。
 
 4、查看报告
 
-运行`allure server report`浏览器会自动调起报告（需先安装配置allure）
+运行`allure server reports`浏览器会自动调起报告（需先安装配置allure）
 
 
 ## 🔬 Demo
 
 [demo](/demo) 提供了丰富实例，帮你快速了解kuto的用法。
 
 ### 安卓APP 测试
 
+* IOS、Web类似
+
 ```python
 import kuto
 
 from page.adr_page import HomePage
 
 
-class TestSearch(kuto.TestCase):
+class TestCaseClass(kuto.TestCase):
 
     def start(self):
         self.page = HomePage(self.driver)
 
-    def test_pom(self):
+    def test_case1(self):
         self.page.my_entry.click()
         self.page.setting_entry.click()
         self.assert_in_page('设置')
 ```
 
 __说明：__
 
 * 创建测试类必须继承 `kuto.TestCase`。
 * 测试用例文件命名必须以 `test` 开头。
-* kuto的封装了`assertText`、`assertElement` 等断言方法。
+* kuto的封装了`assert_in_page`、`assert_title` 等断言方法。
 * 如果用例间有耦合关系，建议使用pom模式，方便复用；否则，使用普通模式即可
   - pom模式需要继承kuto.Page
   - 页面初始化的时候需要传入driver
 
-### IOS APP 测试
+### HTTP 测试
 
 ```python
 import kuto
 
 
-class TestSearch(kuto.TestCase):
+class TestCaseClass(kuto.TestCase):
 
-    def test_normal(self):
-        self.elem(text='我的', desc='我的入口').click()
-        self.elem(text='settings navi', desc='设置入口').click()
-        self.assert_in_page('设置')
+    def test_case1(self):
+        payload = {"type": 2}
+        headers = {"user-agent-web": "X/b67aaff2200d4fc2a2e5a079abe78cc6"}
+        self.post('/qzd-bff-app/qzd/v1/home/getToolCardListForPc', headers=headers, json=payload)
+        self.assertEq('code', 0)
 ```
 
 __说明：__
 
-* 创建测试类必须继承 `kuto.IosTestCase`。
+* 创建测试类必须继承 `kuto.TestCase`。
 * 测试用例文件命名必须以 `test` 开头。
-* kuto的封装了`assertText`、`assertElement` 等断言方法。
-* 如果用例间有耦合关系，建议使用pom模式，方便复用；否则，使用普通模式即可
-  - pom模式需要继承kuto.Page
-  - 页面初始化的时候需要传入driver
+* kuto的封装了`assertEq`、`assertLenEq` 和 `assertLenGt`等断言方法。
 
-### Web 测试
+### 参数化
 
 ```python
 import kuto
+from kuto import data, file_data
 
-from page.web_page import PatentPage
 
+LIST_DATA = [
+    {"name": "李雷", "age": "33"},
+    {"name": "韩梅梅", "age": "30"}
+]
 
-class TestPatentSearch(kuto.TestCase):
 
-    def start(self):
-        self.page = PatentPage(self.driver)
+class TestParameter(kuto.TestCase):
+    """
+    原则是无论是哪种方式，返回的数据必须是list，用例都通过"param"进行调用
+    """
 
-    def test_pom(self):
-        self.open()
-        self.page.search_input.set_text('无人机')
-        self.page.search_submit.click()
-        self.assert_in_page('无人机')
-```
+    @data(LIST_DATA)
+    def test_list(self, param):
+        print(param)
 
-__说明：__
+    @file_data(file='data.json')
+    def test_json(self, param):
+        print(param)
 
-* 创建测试类必须继承 `kuto.WebTestCase`。
-* 测试用例文件命名必须以 `test` 开头。
-* kuto的封装了`assertTitle`、`assertUrl` 和 `assertText`等断言方法。
-* 如果用例间有耦合关系，建议使用pom模式，方便复用；否则，使用普通模式即可
-  - pom模式需要继承kuto.Page
-  - 页面初始化的时候需要传入driver
+    @file_data(file='data.yml', key='names')
+    def test_yaml(self, param):
+        print(param)
 
-### HTTP 测试
+    @file_data(file='data.csv')
+    def test_csv(self, param):
+        print(param)
 
-```python
-import kuto
+    @file_data(file='data.xlsx', row=1)
+    def test_excel(self, param):
+        print(param)
 
-
-class TestGetToolCardListForPc(kuto.TestCase):
-
-    def test_getToolCardListForPc(self):
-        payload = {"type": 2}
-        headers = {"user-agent-web": "X/b67aaff2200d4fc2a2e5a079abe78cc6"}
-        self.post('/qzd-bff-app/qzd/v1/home/getToolCardListForPc', headers=headers, json=payload)
-        self.assert_eq('code', 0)
 ```
 
-__说明：__
-
-* 创建测试类必须继承 `kuto.TestCase`。
-* 测试用例文件命名必须以 `test` 开头。
-* kuto的封装了`assertEq`、`assertLenEq` 和 `assertLenGt`等断言方法。
-
 ### Run the test
 
 ```python
 import kuto
 
-kuto.main()  # 当前文件，pycharm中需要把默认的测试框架从pytest改成unittest，才能右键run
-kuto.main(path="./")  # 当前目录下的所有测试文件
-kuto.main(path="./test_dir/")  # 指定目录下的所有测试文件
-kuto.main(path="./test_dir/test_api.py")  # 指定目录下的测试文件
+kuto.main()  # 当前文件，pycharm中需要把默认的单元测试框架改成unittests
+kuto.main(path="./")  # 当前目录
+kuto.main(path="./test_dir/")  # 指定目录
+kuto.main(path="./test_dir/test_api.py")  # 指定特定文件
+kuto.main(path="./test_dir/test_api.py::TestCaseClass:test_case1") # 指定特定用例
 ```
 
 ### 感谢
 
 感谢从以下项目中得到思路和帮助。
 
 * [seldom](https://github.com/SeldomQA/seldom)
@@ -391,133 +380,14 @@
 
 数据驱动是测试框架非常重要的功能之一，它可以有效的节约大量重复的测试代码。kuto针对该功能做强大的支持。
 
 ### @data()方法
 
 当测试数据量比较少的情况下，可以通过`@data()`管理测试数据。
 
-
-**参数化测试用例**
-
-```python
-import kuto
-from kuto import data
-
-
-class TestDataDriver(kuto.TestCase):
-    @data('name,keyword', [
-        ("First case", "kuto"),
-        ("Second case", "selenium"),
-        ("Third case", "unittest"),
-    ])
-    def test_tuple_data(self, name, keyword):
-        """
-        Used tuple test data
-        :param name: case desc
-        :param keyword: case data
-        """
-        print(f"test data: {name} + {keyword}")
-
-    @data('name,keyword', [
-        ["First case", "kuto"],
-        ["Second case", "selenium"],
-        ["Third case", "unittest"],
-    ])
-    def test_list_data(self, name, keyword):
-        """
-        Used list test data
-        """
-        print(f"test data: {name} + {keyword}")
-
-    @data('json', [
-        {"scene": 'First case', 'keyword': 'kuto'},
-        {"scene": 'Second case', 'keyword': 'selenium'},
-        {"scene": 'Third case', 'keyword': 'unittest'},
-    ])
-    def test_dict_data(self, json):
-        """
-        used dict test data
-        """
-        print(f"case desc: {json['scene']}")
-        print(f"test data: {json['keyword']}")
-    
-    @data('param', [
-            ("First case", "kuto"),
-            ("Second case", "selenium"),
-            ("Third case", "unittest"),
-        ])
-    def test_tuple_single_param(self, param):
-        """
-        Used tuple test data
-        :param name: case desc
-        :param keyword: case data
-        """
-        print(f"test data: {param[0]} + {param[1]}")
-    
-    @data('param_a', [1, 2])
-    @data('param_b', ['c', 'd'])
-    def test_cartesian_product(self, param_a, param_b):
-        """
-        笛卡尔积
-        :param param_a: case desc
-        :param param_b: case data
-        """
-        print(f"test data: {param_a} + {param_b}")
-```
-
-通过`@data()` 装饰器来参数化测试用例。
-
-### @file_data() 方法
-
-当测试数据量比较大的情况下，可以通过`@file_data()`管理测试数据。
-
-**JSON 文件参数化**
-
-kuto 支持将`JSON`文件的参数化。
-
-json 文件：
-
-```json
-{
-  "login1": [
-    [1, 2],
-    [3, 4]
-  ],
-  "login2": [
-    {"username":  1, "password":  2},
-    {"username":  3, "password": 4}
-  ]
-}
-
-```
-
-> 注：`login1` 和 `login2` 的调用方法一样。 区别是前者更简洁，后者更易读。
-```python
-import kuto
-from kuto import file_data
-
-
-class TestYou(kuto.TestCase):
-
-    @file_data("login1")
-    def test_default(self, login1):
-        """文件名使用默认值
-        file: 'data.json'
-        """
-        print(login1[0], login1[1])
-
-    @file_data(key="login2", file='data.json')
-    def test_full_param(self, login2):
-        """参数都填上"""
-        print(login2["username"], login2["password"])
-```
-
-- key: 指定字典的 key，默认不指定解析整个 JSON 文件。
-- file : 指定 JSON 文件的路径。
-
 # Web UI 测试
 
 ## 浏览器与驱动
 
 ### 下载浏览器驱动
 
 > kuto集成webdriver_manager管理浏览器驱动。
@@ -541,75 +411,41 @@
 > kuto --install ie
 > kuto --install edge
 ```
 1. 默认下载到当前的`C:\Users\username\.wdm\drivers\` 目录下面。
 2. Chrome: `chromedriver` 驱动，众所周知的原因，使用的taobao的镜像。
 3. Safari: `safaridriver` （macOS系统自带，默认路径:`/usr/bin/safaridriver`）
 
-指定浏览器驱动
+指定本地浏览器驱动
 
 ```python
 import kuto
 from kuto import ChromeConfig
 
 
 if __name__ == '__main__':
     ChromeConfig.command_executor = '/Users/UI/Documents/chromedriver'
     kuto.main(platform='web', browser="chrome")
 ```
 
-### 指定不同的浏览器
-
-我们运行的自动化测试不可能只在一个浏览器下运行，我们分别需要在chrome、firefox浏览器下运行。在kuto中需要只需要修改一个配置即可。
-
-```python
-import kuto
-# ……
-if __name__ == '__main__':
-    kuto.main(browser="chrome") # chrome浏览器,默认值
-    kuto.main(browser="gc")     # chrome简写
-    kuto.main(browser="firefox") # firefox浏览器
-    kuto.main(browser="ff")      # firefox简写
-    kuto.main(browser="edge")    # edge浏览器
-    kuto.main(browser="safari")  # safari浏览器
-```
 在`main()`方法中通过`browser`参数设置不同的浏览器，默认为`Chrome`浏览器。
 
-## kuto API
+## API
 
 ### 查找元素
 
 * id_
 * name
-* class_name
+* className
 * tag
-* link_text
-* partial_link_text
+* linkText
+* partialLinkText
 * css
 * xpath
 
-__使用方式__
-
-```python
-import kuto
-
-
-class TestDemo(kuto.TestCase):
-    
-    def test_demo(self):
-        self.elem(id_="kw", desc='xxx')
-        self.elem(name="wd", desc="xxx")
-        self.elem(class_name="s_ipt", desc="xxx")
-        self.elem(tag_name="input", desc="xxx")
-        self.elem(xpath="//input[@id='kw']", desc="xxx")
-        self.elem(css="#kw", desc="xxx")
-        self.elem(link_text="hao123", desc='xxx')
-        self.elem(partial_link_text="hao", desc='xxx')
-```
-
 __帮助信息__
 
 * [CSS选择器](https://www.w3school.com.cn/cssref/css_selectors.asp)
 * [xpath语法](https://www.w3school.com.cn/xpath/xpath_syntax.asp)
 
 # APP UI 测试
 
@@ -623,58 +459,37 @@
 ## 安卓 UI 测试
 
 ### 依赖环境
 
 * [adb](https://formulae.brew.sh/cask/android-platform-tools)
     - 用于查看手机设备id
     
-### kuto API
+### API
 
 #### 查找元素
 
-* id_
-* class_name
+* resourceId
+* className
 * text
 * xpath
 
-__使用方式__
-
-```python
-self.elem(res_id="kw", desc='xxx')
-self.elem(class_name="wd", desc="xxx")
-self.elem(text="s_ipt", desc="xxx")
-self.elem(xpath="input", desc="xxx")
-
-```
-
 ## IOS UI 测试
 
 ### 依赖环境
 
 * [WebDriverAgent](https://testerhome.com/topics/7220)
     - 把代码操作转化成原生操作
 * [tidevice](https://github.com/alibaba/taobao-iphone-device)
     - 查看手机设备id
     - 启动WebDriverAgent
     
-### kuto API
+### API
 
 #### 查找元素
 
 * name
 * label
 * value
 * text
-* class_name
+* className
 * xpath
 
-__使用方式__
-
-```python
-self.elem(name="kw", desc='xxx')
-self.elem(label="wd", desc="xxx")
-self.elem(value="s_ipt", desc="xxx")
-self.elem(text="input", desc="xxx")
-self.elem(class_name="input", desc="xxx")
-self.elem(xpath="input", desc="xxx")
-
-```
```

### Comparing `kuto-0.0.5/demo/run.py` & `kuto-0.0.6/demo/run.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/demo/tests/test_param.py` & `kuto-0.0.6/demo/tests/test_para.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     {"name": "李雷", "age": "33"},
     {"name": "韩梅梅", "age": "30"}
 ]
 
 
 class TestParameter(kuto.TestCase):
     """
-    原则是无论是哪种方式，返回的数据必须是list，用例都通过"params"进行调用
+    原则是无论是哪种方式，返回的数据必须是list，用例都通过"param"进行调用
     """
 
     @data(LIST_DATA)
     def test_list(self, param):
         print(param)
 
     @file_data(file='data.json')
@@ -32,9 +32,9 @@
     @file_data(file='data.xlsx', row=1)
     def test_excel(self, param):
         print(param)
 
 
 if __name__ == '__main__':
     kuto.main(
-        path='test_param.py::TestParameter::test_json'
+        path='test_para.py::TestParameter::test_json'
     )
```

### Comparing `kuto-0.0.5/demo/tests/test_web.py` & `kuto-0.0.6/demo/tests/test_web.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/__init__.py` & `kuto-0.0.6/kuto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 )
 from kuto.running.runner import main
 from kuto.utils.config import config
 from kuto.utils.decorate import *
 from kuto.utils.log import logger
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 __description__ = "移动、web、接口自动化测试框架"
```

### Comparing `kuto-0.0.5/kuto/case.py` & `kuto-0.0.6/kuto/case.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/cli.py` & `kuto-0.0.6/kuto/cli.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/android/common.py` & `kuto-0.0.6/kuto/core/android/common.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/android/driver.py` & `kuto-0.0.6/kuto/core/android/driver.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/android/element.py` & `kuto-0.0.6/kuto/core/android/element.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,47 +15,42 @@
 class AdrElem(object):
     """
     安卓元素定义
     """
 
     def __init__(self,
                  driver: AndroidDriver = None,
-                 res_id: str = None,
-                 class_name: str = None,
+                 resourceId: str = None,
+                 className: str = None,
                  text: str = None,
                  xpath: str = None,
-                 image: str = None,
-                 ocr: str = None,
                  index: int = 0,
                  desc: str = None):
         """
         @param driver: 安卓驱动，必填
-        @param res_id: resourceId定位
-        @param class_name: className定位
+        @param resourceId: resourceId定位
+        @param className: className定位
         @param text: text定位
         @param xpath: xpath定位
-        @param image: 图像识别,
         @param ocr: ocr文本识别,
         @param index: 定位出多个元素时，指定索引
         @param desc: 元素描述，必填
         """
         self._driver = driver
 
         self._kwargs = {}
-        if res_id is not None:
-            self._kwargs["resourceId"] = res_id
-        if class_name is not None:
-            self._kwargs["className"] = class_name
+        if resourceId is not None:
+            self._kwargs["resourceId"] = resourceId
+        if className is not None:
+            self._kwargs["className"] = className
         if text is not None:
             self._kwargs["text"] = text
 
         self._xpath = xpath
         self._index = index
-        self._image = image
-        self._ocr = ocr
 
         if desc is None:
             raise ElementNameEmptyException("请设置控件名称")
         else:
             self._desc = desc
 
     def __get__(self, instance, owner):
```

### Comparing `kuto-0.0.5/kuto/core/api/request.py` & `kuto-0.0.6/kuto/core/api/request.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/h5/driver.py` & `kuto-0.0.6/kuto/core/h5/driver.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/image/element.py` & `kuto-0.0.6/kuto/core/image/element.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/image/image_discern.py` & `kuto-0.0.6/kuto/core/image/image_discern.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/ios/common.py` & `kuto-0.0.6/kuto/core/ios/common.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/ios/driver.py` & `kuto-0.0.6/kuto/core/ios/driver.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/ios/element.py` & `kuto-0.0.6/kuto/core/ios/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 
     def __init__(self,
                  driver: IosDriver = None,
                  name: str = None,
                  label: str = None,
                  value: str = None,
                  text: str = None,
-                 class_name: str = None,
+                 className: str = None,
                  xpath: str = None,
-                 image: str = None,
-                 ocr: str = None,
                  index: int = 0,
                  desc: str = None):
         """
         @param driver,
         @param name,
         param label,
         param value,
         param text,
-        param class_name,
+        param className,
         param xpath,
         @param image: 图像识别,
         @param ocr: ocr文本识别,
         param index: 索引,
         param desc: 控件名称
         """
         # if driver is None:
@@ -48,21 +46,19 @@
             self._kwargs["name"] = name
         if label is not None:
             self._kwargs["label"] = label
         if value is not None:
             self._kwargs["value"] = value
         if text is not None:
             self._kwargs["text"] = text
-        if class_name is not None:
-            self._kwargs["className"] = class_name
+        if className is not None:
+            self._kwargs["className"] = className
 
         self._xpath = xpath
         self._index = index
-        self._image = image
-        self._ocr = ocr
 
         if desc is None:
             raise ElementNameEmptyException("请设置控件名称")
         else:
             self._desc = desc
 
     def __get__(self, instance, owner):
```

### Comparing `kuto-0.0.5/kuto/core/ocr/element.py` & `kuto-0.0.6/kuto/core/ocr/element.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/ocr/ocr_discern.py` & `kuto-0.0.6/kuto/core/ocr/ocr_discern.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/sonic/sib_util.py` & `kuto-0.0.6/kuto/core/sonic/sib_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/web/driver.py` & `kuto-0.0.6/kuto/core/web/driver.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/core/web/element.py` & `kuto-0.0.6/kuto/core/web/element.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,51 +15,50 @@
 from kuto.core.web.driver import WebDriver
 from kuto.core.h5.driver import H5Driver
 
 # 支持的定位方式
 LOC_DICT = {
     "id_": By.ID,
     "name": By.NAME,
-    "link_text": By.LINK_TEXT,
-    "tag_name": By.TAG_NAME,
-    "partial_link_text": By.PARTIAL_LINK_TEXT,
-    "class_name": By.CLASS_NAME,
+    "linkText": By.LINK_TEXT,
+    "tagName": By.TAG_NAME,
+    "partialLinkText": By.PARTIAL_LINK_TEXT,
+    "className": By.CLASS_NAME,
     "xpath": By.XPATH,
     "css": By.CSS_SELECTOR,
 }
 
 
 class WebElem:
     """
     根据定位方式定位元素并进行操作
     """
 
     def __init__(self,
                  driver: Union[WebDriver, H5Driver] = None,
                  id_: str = None,
                  name: str = None,
-                 link_text: str = None,
-                 partial_link_text: str = None,
-                 tag_name: str = None,
-                 class_name: str = None,
+                 linkText: str = None,
+                 partialLinkText: str = None,
+                 tagName: str = None,
+                 className: str = None,
                  xpath: str = None,
                  css: str = None,
                  index: int = 0,
                  desc: str = None
                  ):
         """
 
         @param driver: 浏览器驱动
         @param id_: 根据标签id属性进行定位
         @param name: 根据标签name属性定位
-        @param text: 根据标签内文本定位
-        @param link_text: 根据超链接文本进行定位
-        @param partial_link_text: 根据超链接文本的部分内容进行定位
-        @param tag_name: 根据标签名进行定位
-        @param class_name: 根据class属性进行定位
+        @param linkText: 根据超链接文本进行定位
+        @param partialLinkText: 根据超链接文本的部分内容进行定位
+        @param tagName: 根据标签名进行定位
+        @param className: 根据class属性进行定位
         @param xpath: 根据xpath进行定位
         @param css: 根据css selector进行定位
         @param index: 索引（因为可能定位到多个）
         @param desc: 元素描述，必填项
         """
         # if driver is None:
         #     raise DriverNotFound('该控件未传入web driver参数')
@@ -68,22 +67,22 @@
         self._driver = driver
 
         self._kwargs = {}
         if id_ is not None:
             self._kwargs[LOC_DICT["id_"]] = id_
         if name is not None:
             self._kwargs[LOC_DICT["name"]] = name
-        if link_text is not None:
-            self._kwargs[LOC_DICT["link_text"]] = link_text
-        if partial_link_text is not None:
-            self._kwargs[LOC_DICT["partial_link_text"]] = partial_link_text
-        if tag_name is not None:
-            self._kwargs[LOC_DICT["tag_name"]] = tag_name
-        if class_name is not None:
-            self._kwargs[LOC_DICT["class_name"]] = class_name
+        if linkText is not None:
+            self._kwargs[LOC_DICT["linkText"]] = linkText
+        if partialLinkText is not None:
+            self._kwargs[LOC_DICT["partialLinkText"]] = partialLinkText
+        if tagName is not None:
+            self._kwargs[LOC_DICT["tagName"]] = tagName
+        if className is not None:
+            self._kwargs[LOC_DICT["className"]] = className
         if xpath is not None:
             self._kwargs[LOC_DICT["xpath"]] = xpath
         if css is not None:
             self._kwargs[LOC_DICT["css"]] = css
 
         self._index = index
```

### Comparing `kuto-0.0.5/kuto/general.py` & `kuto-0.0.6/kuto/general.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/page.py` & `kuto-0.0.6/kuto/page.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/running/runner.py` & `kuto-0.0.6/kuto/running/runner.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/scaffold.py` & `kuto-0.0.6/kuto/scaffold.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/testdata/__init__.py` & `kuto-0.0.6/kuto/testdata/__init__.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/testdata/data.py` & `kuto-0.0.6/kuto/testdata/data.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/allure_data.py` & `kuto-0.0.6/kuto/utils/allure_data.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/config.py` & `kuto-0.0.6/kuto/utils/config.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/decorate.py` & `kuto-0.0.6/kuto/utils/decorate.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/dingtalk.py` & `kuto-0.0.6/kuto/utils/dingtalk.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         ret_dict = ret.json()
         if ret_dict.get('errcode') == 0:
             print('消息发送成功')
         else:
             print('消息发送失败: {}'.format(ret_dict.get('errmsg')))
 
     # 从allure报告中获取数据并发送消息
-    def send_reports(self, msg_title, reports_url):
+    def send_report(self, msg_title, reports_url):
         allure_data = get_allure_data('reports')
         total = allure_data.get('total')
         passed = allure_data.get('passed')
         fail = allure_data.get('failed')
         rate = allure_data.get('rate')
 
         color_red = 'FF0000'
```

### Comparing `kuto-0.0.5/kuto/utils/encrypt.py` & `kuto-0.0.6/kuto/utils/encrypt.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/excel.py` & `kuto-0.0.6/kuto/utils/excel.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/exceptions.py` & `kuto-0.0.6/kuto/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/mail.py` & `kuto-0.0.6/kuto/utils/mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     #     except Exception as e:
     #         print(f'发送失败: {str(e)}')
     #     else:
     #         print('发送成功')
     #     # 断开连接
     #     conn.quit()
 
-    def send_reports(self, to_list, title, reports_url):
+    def send_report(self, to_list, title, reports_url):
         allure_data = get_allure_data('reports')
         total = allure_data.get('total')
         fail = allure_data.get('failed')
         passed = allure_data.get('passed')
         rate = allure_data.get('rate')
 
         # 邮件内容
```

### Comparing `kuto-0.0.5/kuto/utils/mongo_util.py` & `kuto-0.0.6/kuto/utils/mongo_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/mysql_util.py` & `kuto-0.0.6/kuto/utils/mysql_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/read_file.py` & `kuto-0.0.6/kuto/utils/read_file.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/schema_util.py` & `kuto-0.0.6/kuto/utils/schema_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/swagger_util.py` & `kuto-0.0.6/kuto/utils/swagger_util.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto/utils/webdriver_manager_extend.py` & `kuto-0.0.6/kuto/utils/webdriver_manager_extend.py`

 * *Files identical despite different names*

### Comparing `kuto-0.0.5/kuto.egg-info/SOURCES.txt` & `kuto-0.0.6/kuto.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 demo/page/__init__.py
 demo/page/adr_page.py
 demo/page/web_page.py
 demo/tests/__init__.py
 demo/tests/test_adr.py
 demo/tests/test_api.py
 demo/tests/test_ios.py
-demo/tests/test_param.py
+demo/tests/test_para.py
 demo/tests/test_web.py
 kuto/__init__.py
 kuto/case.py
 kuto/cli.py
 kuto/general.py
 kuto/page.py
 kuto/scaffold.py
```

### Comparing `kuto-0.0.5/kuto.egg-info/requires.txt` & `kuto-0.0.6/kuto.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 allure-pytest==2.9.45
 PyYAML==6.0
 pandas==1.3.4
 openpyxl==3.0.9
 XlsxWriter==3.0.2
 pycryptodome==3.14.1
 yagmail==0.15.293
-
-[db]
 PyMySQL==0.10.1
 pymongo==4.0.1
 
-[image]
+[ocr]
 easyocr==1.6.2
+
+[opencv]
 opencv-python==4.6.0.66
 opencv-contrib-python==4.6.0.66
 opencv-python-headless==3.4.18.65
```

### Comparing `kuto-0.0.5/setup.py` & `kuto-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 setup(
     name="kuto",
     version=__version__,
     description=__description__,
     author="杨康",
     author_email="772840356@qq.com",
-    url="https://gitee.com/bluepang2021/qrunner_new",
+    url="https://gitee.com/bluepang2021/kuto",
     platforms="Android,IOS,Web,Api",
     packages=find_packages(),
     long_description=long_description,
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     classifiers=[
         "Programming Language :: Python :: 3.9"
     ],
     include_package_data=True,
     package_data={
         r'': ['*.yml'],
     },
@@ -42,20 +42,21 @@
         'pytest-dependency==0.5.1',
         'allure-pytest==2.9.45',
         'PyYAML==6.0',
         'pandas==1.3.4',
         'openpyxl==3.0.9',
         'XlsxWriter==3.0.2',
         'pycryptodome==3.14.1',
-        'yagmail==0.15.293'
+        'yagmail==0.15.293',
+        'PyMySQL==0.10.1',
+        'pymongo==4.0.1'
     ],
     extras_require={
-        "db": ['PyMySQL==0.10.1', 'pymongo==4.0.1'],
-        "image": [
-            'easyocr==1.6.2',
+        "ocr": ["easyocr==1.6.2"],
+        "opencv": [
             'opencv-python==4.6.0.66',
             'opencv-contrib-python==4.6.0.66',
             'opencv-python-headless==3.4.18.65'
         ]
     },
     entry_points={
         'console_scripts': [
```

