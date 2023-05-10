# Comparing `tmp/blaster-server-0.0.428b0.tar.gz` & `tmp/blaster-server-0.0.429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.428b0.tar", last modified: Mon May  8 21:46:22 2023, max compression
+gzip compressed data, was "blaster-server-0.0.429.tar", last modified: Wed May 10 08:42:54 2023, max compression
```

## Comparing `blaster-server-0.0.428b0.tar` & `blaster-server-0.0.429.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.428b0/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.428b0/README.md
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.428b0/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.616986 blaster-server-0.0.428b0/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.428b0/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.616986 blaster-server-0.0.428b0/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.428b0/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.428b0/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.616986 blaster-server-0.0.428b0/blaster/cloud/aws/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.428b0/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5230 2023-01-28 12:53:32.000000 blaster-server-0.0.428b0/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-06 07:07:21.000000 blaster-server-0.0.428b0/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3796 2023-03-06 12:38:58.000000 blaster-server-0.0.428b0/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.428b0/blaster/connection_pool.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.428b0/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-03-30 07:56:48.000000 blaster-server-0.0.428b0/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-08 19:52:47.000000 blaster-server-0.0.428b0/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    14954 2023-03-22 22:32:18.000000 blaster-server-0.0.428b0/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36583 2023-04-18 10:02:10.000000 blaster-server-0.0.428b0/blaster/server.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    47003 2023-04-18 15:49:13.000000 blaster-server-0.0.428b0/blaster/tools.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/blaster/utils/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.428b0/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.428b0/blaster/utils/data/mime_types.json
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7086 2023-04-16 20:57:56.000000 blaster-server-0.0.428b0/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.428b0/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.428b0/blaster/utils/fork.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.428b0/blaster/utils/lat_long_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5552 2023-02-01 17:01:50.000000 blaster-server-0.0.428b0/blaster/utils/phone_number_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.428b0/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/blaster/websocket/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.428b0/blaster/websocket/_app.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_core.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_exceptions.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_handshake.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_http.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_logging.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_socket.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_ssl_compat.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_url.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.428b0/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/blaster/websocket/tests/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/tests/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/blaster_server.egg-info/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      851 2023-05-08 21:46:22.000000 blaster-server-0.0.428b0/blaster_server.egg-info/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-08 21:46:22.000000 blaster-server-0.0.428b0/blaster_server.egg-info/SOURCES.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-08 21:46:22.000000 blaster-server-0.0.428b0/blaster_server.egg-info/dependency_links.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-05-08 21:46:22.000000 blaster-server-0.0.428b0/blaster_server.egg-info/requires.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-08 21:46:22.000000 blaster-server-0.0.428b0/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/examples/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.428b0/examples/fast_api_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/examples/gevent_wsgi_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.428b0/examples/meinheld_flask.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.428b0/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.428b0/examples/simple_examples.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.428b0/examples/test_chat_room.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.428b0/examples/tornado_hello_world.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.428b0/examples/wheezy_hello.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1560 2023-05-08 20:05:36.000000 blaster-server-0.0.428b0/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-08 21:46:22.620986 blaster-server-0.0.428b0/test/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.428b0/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.428b0/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.428b0/test/test_schema.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.428b0/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.428b0/test/test_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.428b0/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.429/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.429/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-05-10 08:42:54.067221 blaster-server-0.0.429/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.429/README.md
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.429/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.429/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.429/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3215 2023-04-30 12:43:59.000000 blaster-server-0.0.429/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/blaster/cloud/aws/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.429/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5230 2023-01-28 12:53:32.000000 blaster-server-0.0.429/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-06 07:07:21.000000 blaster-server-0.0.429/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3796 2023-03-06 12:38:58.000000 blaster-server-0.0.429/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.429/blaster/connection_pool.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.429/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-03-30 07:56:48.000000 blaster-server-0.0.429/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62877 2023-05-10 08:42:24.000000 blaster-server-0.0.429/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    14954 2023-03-22 22:32:18.000000 blaster-server-0.0.429/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    36583 2023-04-18 10:02:10.000000 blaster-server-0.0.429/blaster/server.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    47003 2023-04-18 15:49:13.000000 blaster-server-0.0.429/blaster/tools.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/blaster/utils/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.429/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.429/blaster/utils/data/mime_types.json
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7086 2023-04-16 20:57:56.000000 blaster-server-0.0.429/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.429/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.429/blaster/utils/fork.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.429/blaster/utils/lat_long_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5564 2023-05-09 13:55:03.000000 blaster-server-0.0.429/blaster/utils/phone_number_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.429/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/blaster/websocket/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.429/blaster/websocket/_app.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_core.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_exceptions.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_handshake.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_http.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_logging.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_socket.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_ssl_compat.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_url.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.429/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/blaster/websocket/tests/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/tests/__init__.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.429/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/blaster_server.egg-info/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      849 2023-05-10 08:42:54.000000 blaster-server-0.0.429/blaster_server.egg-info/PKG-INFO
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1682 2023-05-10 08:42:54.000000 blaster-server-0.0.429/blaster_server.egg-info/SOURCES.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-10 08:42:54.000000 blaster-server-0.0.429/blaster_server.egg-info/dependency_links.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      221 2023-05-10 08:42:54.000000 blaster-server-0.0.429/blaster_server.egg-info/requires.txt
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-10 08:42:54.000000 blaster-server-0.0.429/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/examples/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.429/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.429/examples/fast_api_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.429/examples/gevent_wsgi_test.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.429/examples/meinheld_flask.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.429/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.429/examples/simple_examples.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.429/examples/test_chat_room.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.429/examples/tornado_hello_world.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.429/examples/wheezy_hello.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-10 08:42:54.067221 blaster-server-0.0.429/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1559 2023-05-10 08:40:43.000000 blaster-server-0.0.429/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-10 08:42:54.067221 blaster-server-0.0.429/test/
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.429/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.429/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      503 2022-11-07 18:31:41.000000 blaster-server-0.0.429/test/test_schema.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.429/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.429/test/test_utils.py
+-rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.429/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.428b0/LICENSE.txt` & `blaster-server-0.0.429/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/PKG-INFO` & `blaster-server-0.0.429/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.428b0
+Version: 0.0.429
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.428b0/README.md` & `blaster-server-0.0.429/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/__init__.py` & `blaster-server-0.0.429/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/cloud/analytics.py` & `blaster-server-0.0.429/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.429/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/cloud/push_tasks.py` & `blaster-server-0.0.429/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/cloud/storage.py` & `blaster-server-0.0.429/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/config.py` & `blaster-server-0.0.429/blaster/config.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/connection_pool.py` & `blaster-server-0.0.429/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/logging.py` & `blaster-server-0.0.429/blaster/logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/mongo_orm.py` & `blaster-server-0.0.429/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/schema.py` & `blaster-server-0.0.429/blaster/schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/server.py` & `blaster-server-0.0.429/blaster/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/tools.py` & `blaster-server-0.0.429/blaster/tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/utils/data/countries.json` & `blaster-server-0.0.429/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/utils/data/mime_types.json` & `blaster-server-0.0.429/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/utils/data_utils.py` & `blaster-server-0.0.429/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/utils/events.py` & `blaster-server-0.0.429/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/utils/fork.py` & `blaster-server-0.0.429/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.429/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.429/blaster/utils/phone_number_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from .data_utils import COUNTRY_DATA
 from ..tools import ltrim
 
 PHONE_NUMBER_REGEX = re.compile(r"^\+?[0-9]+")
 
 
-country_code_num_digits_map = {"93": [9], "358": [10], "355": [9], "213": [9], "1": [10], "374": [6], "297": [7], "61": [9], "672": [6], "43": [11], "994": [9], "973": [8], "880": [10], "375": [9], "32": [9], "501": [7], "229": [6, 7, 8, 9], "387": [8], "55": [11], "246": [7], "359": [9], "226": [8], "855": [9], "235": [8], "56": [9], "86": [11], "57": [10], "682": [5], "506": [8], "385": [9], "357": [8], "420": [9], "45": [8], "670": [8], "593": [9], "20": [10], "503": [7], "44": [10], "268": [8], "500": [5], "298": [5], "691": [7], "33": [9], "594": [9], "689": [6], "241": [7], "995": [9], "49": [10], "233": [9], "30": [10], "299": [6], "590": [12], "852": [8], "36": [9], "91": [10], "62": [10], "98": [10], "353": [9], "972": [9], "39": [10], "81": [11], "7": [10], "686": [5], "383": [8], "965": [8], "371": [8], "961": [8], "231": [8], "218": [10], "370": [8], "352": [9], "265": [7, 8, 9], "60": [7], "960": [7], "223": [8], "692": [7], "596": [12], "230": [8], "52": [10], "373": [8], "976": [8], "382": [8], "95": [10], "977": [10], "31": [9], "687": [6], "64": [8, 9, 10], "227": [8], "234": [8, 10], "254": [9], "683": [4], "90": [11], "47": [8], "968": [8], "92": [10], "680": [7], "970": [9], "507": [8], "51": [9], "63": [10], "48": [9], "351": [9], "974": [8], "262": [12], "290": [4], "966": [9], "381": [8], "65": [8], "421": [9], "677": [7], "252": [7, 8], "27": [9], "34": [9], "94": [7], "46": [7], "41": [9], "963": [9], "886": [9], "66": [9], "228": [8], "216": [8], "380": [9], "971": [9], "58": [7], "84": [9], "967": [9]}
+country_code_num_digits_map = {"93": [9], "358": [10], "355": [9], "213": [9], "1": [10], "374": [6], "297": [7], "61": [9], "672": [6], "43": [11], "994": [9], "973": [8], "880": [10], "375": [9], "32": [9], "501": [7], "229": [6, 7, 8, 9], "387": [8], "55": [11], "246": [7], "359": [9], "226": [8], "855": [9], "235": [8], "56": [9], "86": [11], "57": [10], "682": [5], "506": [8], "385": [9], "357": [8], "420": [9], "45": [8], "670": [8], "593": [9], "20": [10], "503": [7], "44": [10], "268": [8], "500": [5], "298": [5], "691": [7], "33": [9], "594": [9], "689": [6], "241": [7], "995": [9], "49": [10], "233": [9], "30": [10], "299": [6], "590": [12], "852": [8], "36": [9], "91": [10], "62": [10], "98": [10], "353": [9], "972": [9], "39": [10], "81": [11], "7": [10], "686": [5], "383": [8], "965": [8], "371": [8], "961": [8], "231": [8], "218": [10], "370": [8], "352": [9], "265": [7, 8, 9], "60": [7], "960": [7], "223": [8], "692": [7], "596": [12], "230": [8], "52": [10], "373": [8], "976": [8], "382": [8], "95": [10], "977": [10], "31": [9], "687": [6], "64": [8, 9, 10], "227": [8], "234": [8, 10], "254": [9], "255": [9], "683": [4], "90": [11], "47": [8], "968": [8], "92": [10], "680": [7], "970": [9], "507": [8], "51": [9], "63": [10], "48": [9], "351": [9], "974": [8], "262": [12], "290": [4], "966": [9], "381": [8], "65": [8], "421": [9], "677": [7], "252": [7, 8], "27": [9], "34": [9], "94": [7], "46": [7], "41": [9], "963": [9], "886": [9], "66": [9], "228": [8], "216": [8], "380": [9], "971": [9], "58": [7], "84": [9], "967": [9]}
 
 
 class SimpleTrie(dict):
 	end_obj = None
 
 
 country_code_num_digits_trie = SimpleTrie()
```

### Comparing `blaster-server-0.0.428b0/blaster/utils/xss_html.py` & `blaster-server-0.0.429/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/__init__.py` & `blaster-server-0.0.429/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_abnf.py` & `blaster-server-0.0.429/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_app.py` & `blaster-server-0.0.429/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_core.py` & `blaster-server-0.0.429/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_exceptions.py` & `blaster-server-0.0.429/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_handshake.py` & `blaster-server-0.0.429/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_http.py` & `blaster-server-0.0.429/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_logging.py` & `blaster-server-0.0.429/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_socket.py` & `blaster-server-0.0.429/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.429/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_url.py` & `blaster-server-0.0.429/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/_utils.py` & `blaster-server-0.0.429/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/server.py` & `blaster-server-0.0.429/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.429/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.429/blaster_server.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.428b0
+Version: 0.0.429
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.428b0/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.429/blaster_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/examples/gevent_wsgi_test.py` & `blaster-server-0.0.429/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/examples/mongo_ormexample.py` & `blaster-server-0.0.429/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/examples/simple_examples.py` & `blaster-server-0.0.429/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/examples/test_chat_room.py` & `blaster-server-0.0.429/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/examples/tornado_hello_world.py` & `blaster-server-0.0.429/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/examples/wheezy_hello.py` & `blaster-server-0.0.429/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/setup.py` & `blaster-server-0.0.429/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.428b',
+	version='0.0.429',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
```

### Comparing `blaster-server-0.0.428b0/test/test_mongo_orm.py` & `blaster-server-0.0.429/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/test/test_tools.py` & `blaster-server-0.0.429/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/test/test_utils.py` & `blaster-server-0.0.429/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.428b0/test/timeit_snippets.py` & `blaster-server-0.0.429/test/timeit_snippets.py`

 * *Files identical despite different names*

