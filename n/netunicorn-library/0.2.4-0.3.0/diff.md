# Comparing `tmp/netunicorn-library-0.2.4.tar.gz` & `tmp/netunicorn-library-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/netunicorn-library/netunicorn-library/temp/netunicorn/netunicorn-library/dist/.tmp-urk_wqcb/netunicorn-librar", last modified: Wed Apr 12 21:44:44 2023, max compression
+gzip compressed data, was "netunicorn-library-0.3.0.tar", last modified: Wed May 10 08:30:19 2023, max compression
```

## Comparing `netunicorn-library-0.2.4.tar` & `netunicorn-library-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/heartbleeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/pcapture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/ping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/speedtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/upload/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-12 21:44:27.000000 netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 21:44:44.000000 netunicorn-library-0.2.4/src/netunicorn_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.302367 netunicorn-library-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 08:30:19.302367 netunicorn-library-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:30:19.302367 netunicorn-library-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/capture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/capture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/capture/tcpdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/letsencrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/letsencrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/letsencrypt/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/ookla_speedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.294367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/arp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/arp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/arp/spoof.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/cve202141773/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/cve202141773/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/icmp/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/icmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/icmp/redirection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/land/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/land/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/land/landattack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/log4j/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/log4j/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/slowloris.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/loris/smbloris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mac/flooder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/mail/fake_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/upload/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/utils/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-10 08:30:04.000000 netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:30:19.298367 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 08:30:19.000000 netunicorn-library-0.3.0/src/netunicorn_library.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `netunicorn-library-0.2.4/pyproject.toml` & `netunicorn-library-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "netunicorn-library"
-version = "0.2.4"
+version = "0.3.0"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "netunicorn contrib library"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = ["netunicorn"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "netunicorn-base >= 0.2.5",
+    "netunicorn-base >= 0.3.1",
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/basic.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 class DummyTask(Task):
     def run(self):
         return True
 
 
 class SleepTask(Task):
-    def __init__(self, seconds: int):
+    def __init__(self, seconds: int, *args, **kwargs):
         self.seconds = seconds
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
         time.sleep(self.seconds)
         return self.seconds
 
 
 class ShellCommand(Task):
-    def __init__(self, command: str):
+    def __init__(self, command: str, *args, **kwargs):
         self.command = command
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
         return subprocess.check_output(self.command, shell=True)
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/__init__.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import time
 from enum import Enum
-from netunicorn.base.task import Task
-from netunicorn.base.task import Success, Failure
+from netunicorn.base.task import Task, Success, Failure
 from .heartbleeder import connect, send_hello, bleed
 
 
 class TLSVersion(Enum):
     TLS_1_0 = 0x01
     TLS_1_1 = 0x02
     TLS_1_2 = 0x03
@@ -17,22 +16,24 @@
         self,
         dst_host: str,
         dst_port: int,
         src_port: int = None,
         count: int = 1,
         sleep_seconds: int = 0,
         tls_version: TLSVersion = TLSVersion.TLS_1_0,
+        *args,
+        **kwargs
     ):
         self.host = dst_host
         self.port = dst_port
         self.src_port = src_port
         self.count = count
         self.sleep_seconds = sleep_seconds
         self.tls_version = int(tls_version.value)
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
         connection = connect(self.host, self.port, src_port=self.src_port)
         time.sleep(1)
         send_hello(connection, self.tls_version)
         time.sleep(1)
         result = ""
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/heartbleed/heartbleeder.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/network_attacks/heartbleed/heartbleeder.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         0x00,  # Payload length
     ]
 
 
 def _hexdump(payload: bytes) -> str:
     pdat = ""
     for b in range(0, len(payload), 16):
-        lin = [c for c in payload[b : b + 16]]
+        lin = [c for c in payload[b: b + 16]]
         pdat += "".join(
             (chr(c) if ((32 <= c <= 126) or (c == 10) or (c == 13)) else ".")
             for c in lin
         )
     pdat = re.sub(r"([.]{50,})", "", pdat)
     return pdat
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/pcapture.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/capture/tcpdump.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/ping.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/ping.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,34 +25,34 @@
     stddev_rtt: float
     unit_rtt: str
     unparsed_output: List[str]
     raw_output: str
 
 
 class Ping(TaskDispatcher):
-    def __init__(self, address: str, count: int = 1):
+    def __init__(self, address: str, count: int = 1, *args, **kwargs):
         self.address = address
         self.count = count
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
         if node.properties.get("os_family", "").lower() == "linux":
             return PingLinuxImplementation(self.address, self.count)
         raise NotImplementedError(
             f'Ping is not implemented for {node.properties.get("os_family", "")}'
         )
 
 
 class PingLinuxImplementation(Task):
     requirements = ["sudo apt-get install -y inetutils-ping"]
 
-    def __init__(self, address: str, count: int = 1):
-        super().__init__()
+    def __init__(self, address: str, count: int = 1, *args, **kwargs):
         self.address = address.strip()
         self.count = count
+        super().__init__(*args, **kwargs)
 
     def run(self):
         result = subprocess.run(
             ["ping", self.address, "-c", str(self.count)], capture_output=True
         )
         if result.returncode != 0:
             return Failure(
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/__init__.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 import os
 import subprocess
 import time
 from typing import Optional
 
 from jinja2 import Environment, FileSystemLoader
+from netunicorn.base.architecture import Architecture
 from netunicorn.base.nodes import Node
-from netunicorn.base.task import Failure, Success, Task, TaskDispatcher
+from netunicorn.base import Failure, Success, Task, TaskDispatcher, is_successful
 
 
 class StartQoECollectionServer(TaskDispatcher):
     def __init__(
-        self, data_folder: str = ".", interface: str = "0.0.0.0", port: int = 34543
+        self, data_folder: str = ".", interface: str = "0.0.0.0", port: int = 34543, *args, **kwargs,
     ):
         self.data_folder = data_folder
         self.interface = interface
         self.port = port
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
-        if node.properties.get("os_family", "").lower() == "linux":
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             return StartQoECollectionServerLinuxImplementation(
-                self.data_folder, self.interface, self.port
+                self.data_folder, self.interface, self.port, name=self.name
             )
 
         raise NotImplementedError(
-            f'StartQoECollectionServer is not implemented for {node.properties.get("os_family", "")}'
+            f'StartQoECollectionServer is not implemented for {node.architecture}'
         )
 
 
 class StartQoECollectionServerLinuxImplementation(Task):
     requirements = [
         "sudo apt-get update",
         "sudo apt-get install -y python3-pip uvicorn",
         "pip3 install fastapi uvicorn uvloop",
     ]
 
     def __init__(
-        self, data_folder: str = ".", interface: str = "0.0.0.0", port: int = 34543
+        self, data_folder: str = ".", interface: str = "0.0.0.0", port: int = 34543, *args, **kwargs,
     ):
         self.data_folder = data_folder
         self.interface = interface
         self.port = port
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
         env = os.environ.copy()
         env["QOE_DATA_FOLDER"] = self.data_folder
 
         process = subprocess.Popen(
             [
                 "uvicorn",
-                "netunicorn.library.qoe_youtube.qoe_collector:app",
+                "netunicorn.library.tasks.qoe_youtube.qoe_collector:app",
                 "--host",
                 self.interface,
                 "--port",
                 str(self.port),
                 "--log-level",
                 "warning",
             ],
@@ -71,68 +72,72 @@
             f"QoE collection server started with data folder '{self.data_folder}' and "
             f"using interface {self.interface}:{self.port}, process ID: {process.pid}",
             process.pid,
         )
 
 
 class StopQoECollectionServer(TaskDispatcher):
+    def __init__(self, start_task_name: str, *args, **kwargs):
+        self.start_task_name = start_task_name
+        super().__init__(*args, **kwargs)
+
     def dispatch(self, node: Node) -> Task:
         if node.properties.get("os_family", "").lower() == "linux":
-            return StopQoECollectionServerLinuxImplementation()
+            return StopQoECollectionServerLinuxImplementation(start_task_name=self.start_task_name, name=self.name)
 
         raise NotImplementedError(
-            f'StopQoECollectionServer is not implemented for {node.properties.get("os_family", "")}'
+            f'StopQoECollectionServer is not implemented for {node.architecture}'
         )
 
 
 class StopQoECollectionServerLinuxImplementation(Task):
+    def __init__(self, start_task_name: str, *args, **kwargs):
+        self.start_task_name = start_task_name
+        super().__init__(*args, **kwargs)
+
     def run(self):
         # look for the process ID of the QoE collection server and use it to kill the server
-        for element in self.previous_steps:
-            if isinstance(element, Success):
-                element = [element]
-            for result in element:
-                if isinstance(y := result.unwrap(), tuple) and str(y[0]).startswith(
-                    "QoE collection server started"
-                ):
-                    process_id = y[1]
-                    subprocess.run(["kill", str(process_id)])
-                    return Success(
-                        f"QoE collection server stopped with process ID: {process_id}"
-                    )
-        return Failure("QoE collection server not found")
+        result = self.previous_steps.get(self.start_task_name, [Failure("QoE collection server not found")])[-1]
+        if is_successful(result):
+            process_id = result.unwrap()[1]
+            return subprocess.check_output(f"kill {process_id}", shell=True)
+
+        return result
 
 
 class WatchYouTubeVideo(TaskDispatcher):
     def __init__(
         self,
         video_url: str,
         duration: Optional[int] = None,
         quality: Optional[int] = None,
         qoe_server_address: str = "localhost",
         qoe_server_port: int = 34543,
         report_time: int = 250,
+        *args,
+        **kwargs,
     ):
         self.video_url = video_url
         self.duration = duration
         self.quality = quality
         self.qoe_server_address = qoe_server_address
         self.qoe_server_port = qoe_server_port
         self.report_time = report_time
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
-        if node.properties.get("os_family", "").lower() == "linux":
+        if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             return WatchYouTubeVideoLinuxImplementation(
                 self.video_url,
                 self.duration,
                 self.quality,
                 self.qoe_server_address,
                 self.qoe_server_port,
                 self.report_time,
+                name=self.name,
             )
 
         raise NotImplementedError(
             f'WatchYouTubeVideo is not implemented for {node.properties.get("os_family", "")}'
         )
 
 
@@ -154,25 +159,27 @@
         self,
         video_url: str,
         duration: Optional[int] = None,
         quality: Optional[int] = None,
         qoe_server_address: str = "localhost",
         qoe_server_port: int = 34543,
         report_time: int = 250,
+        *args,
+        **kwargs,
     ):
         self.video_url = video_url
         self.duration = duration
         self.quality = quality
         self.qoe_server_address = qoe_server_address
         self.qoe_server_port = qoe_server_port
         self.report_time = report_time
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
-        from netunicorn.library.qoe_youtube import qoe_collector, watcher
+        from netunicorn.library.tasks.qoe_youtube import watcher
 
         adblock_crx_path = os.path.join(".", "extensions", "4.46.2_0.crx")
         qoe_extension_path = os.path.join(".", "extensions", "qoe_extension")
 
         # using jinja substitute QoECollectionServer address and port in script.json
         env = Environment(loader=FileSystemLoader(qoe_extension_path))
         template = env.get_template("script.js.template")
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/qoe_collector.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/qoe_youtube/watcher.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/qoe_youtube/watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     :param goal:
     :return: index of closest option
     """
     sorted_options = sorted(options)
     if not sorted_options:
         raise Exception("Youtube parsing error: quality menu block is empty")
 
+    opt = 0
     for ind, opt in enumerate(sorted_options):
         if opt >= goal:
             if ind > 0 and (goal - sorted_options[ind - 1] < opt - goal):
                 return options.index(sorted_options[ind - 1])
             else:
                 return options.index(opt)
     return options.index(opt)
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/speedtest.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/measurements/ookla_speedtest.py`

 * *Files identical despite different names*

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/upload/webdav.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/upload/webdav.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,35 @@
     def __init__(
         self,
         filepaths: Set[str],
         endpoint: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         authentication: Literal["basic"] = "basic",
+        *args,
+        **kwargs
     ):
         if endpoint[-1] == "/":
             endpoint = endpoint[:-1]
         self.filepaths = filepaths
         self.endpoint = endpoint
         self.username = username
         self.password = password
         self.authentication = authentication
 
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
         result = UploadToWebDavImplementation(
             self.filepaths,
             self.endpoint,
             self.username,
             self.password,
             self.authentication,
+            name=self.name,
         )
 
         if node.architecture in {Architecture.LINUX_AMD64, Architecture.LINUX_ARM64}:
             result.requirements = ["sudo apt-get install -y curl"]
             return result
 
         raise NotImplementedError(
@@ -47,21 +50,23 @@
     def __init__(
         self,
         filepaths: Set[str],
         endpoint: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
         authentication: Literal["basic"] = "basic",
+        *args,
+        **kwargs
     ):
         self.filepaths = filepaths
         self.endpoint = endpoint
         self.username = username
         self.password = password
         self.authentication = authentication
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
         executor_id = os.environ.get("NETUNICORN_EXECUTOR_ID") or "Unknown"
 
         for file in self.filepaths:
             command = ["curl", "-T", file, f"{self.endpoint}/{executor_id}/{file}"]
             if self.authentication == "basic":
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/twitch_watcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import os
 import random
 import subprocess
 import time
 from typing import Optional
 
-from netunicorn.base.task import Result, Success, Task, TaskDispatcher
+from netunicorn.base import Result, Success, Task, TaskDispatcher
 from netunicorn.base.nodes import Node
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 
@@ -38,22 +38,22 @@
     result = Success(f"Video probably finished by timeout: {duration} seconds")
     driver.close()
     xvfb_process.kill()
     return result
 
 
 class WatchTwitchStream(TaskDispatcher):
-    def __init__(self, video_url: str, duration: Optional[int] = None):
+    def __init__(self, video_url: str, duration: Optional[int] = None, *args, **kwargs):
         self.video_url = video_url
         self.duration = duration
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
         if node.properties.get("os_family", "").lower() == "linux":
-            return WatchTwitchStreamLinuxImplementation(self.video_url, self.duration)
+            return WatchTwitchStreamLinuxImplementation(self.video_url, self.duration, name=self.name)
 
         raise NotImplementedError(
             f'WatchYouTubeVideo is not implemented for {node.properties.get("os_family", "")}'
         )
 
 
 class WatchTwitchStreamLinuxImplementation(Task):
@@ -62,22 +62,22 @@
         "sudo apt install -y python3-pip wget xvfb",
         "pip3 install selenium webdriver-manager",
         "sudo apt install -y chromium-browser",
         "from webdriver_manager.chrome import ChromeDriverManager; from webdriver_manager.core.utils import ChromeType; ChromeDriverManager(chrome_type=ChromeType.CHROMIUM,path='/usr/bin/').install()",
     ]
 
     def __init__(
-        self, video_url: str, duration: int = 10, chrome_location: Optional[str] = None
+        self, video_url: str, duration: int = 10, chrome_location: Optional[str] = None, *args, **kwargs
     ):
         self.video_url = video_url
         self.duration = duration
         self.chrome_location = chrome_location
         if not self.chrome_location:
             self.chrome_location = "/usr/bin/chromium-browser"
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
         return watch(self.video_url, self.duration, self.chrome_location)
 
 
 if __name__ == "__main__":
     print(watch("https://www.twitch.tv/videos/1592059689", 10))
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/vimeo_watcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import os
 import random
 import subprocess
 import time
 from typing import Optional
 
-from netunicorn.base.task import Result, Failure, Success, Task, TaskDispatcher
+from netunicorn.base import Result, Failure, Success, Task, TaskDispatcher
 from netunicorn.base.nodes import Node
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 
@@ -68,22 +68,22 @@
 
     driver.close()
     xvfb_process.kill()
     return result
 
 
 class WatchVimeoVideo(TaskDispatcher):
-    def __init__(self, video_url: str, duration: Optional[int] = None):
+    def __init__(self, video_url: str, duration: Optional[int] = None, *args, **kwargs):
         self.video_url = video_url
         self.duration = duration
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
         if node.properties.get("os_family", "").lower() == "linux":
-            return WatchVimeoVideoLinuxImplementation(self.video_url, self.duration)
+            return WatchVimeoVideoLinuxImplementation(self.video_url, self.duration, name=self.name)
 
         raise NotImplementedError(
             f'WatchYouTubeVideo is not implemented for {node.properties.get("os_family", "")}'
         )
 
 
 class WatchVimeoVideoLinuxImplementation(Task):
@@ -96,21 +96,23 @@
     ]
 
     def __init__(
         self,
         video_url: str,
         duration: Optional[int] = None,
         chrome_location: Optional[str] = None,
+        *args,
+        **kwargs
     ):
         self.video_url = video_url
         self.duration = duration
         self.chrome_location = chrome_location
         if not self.chrome_location:
             self.chrome_location = "/usr/bin/chromium-browser"
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
         return watch(self.video_url, self.duration, self.chrome_location)
 
 
 if __name__ == "__main__":
     print(watch("https://vimeo.com/440421754", 10))
```

### Comparing `netunicorn-library-0.2.4/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py` & `netunicorn-library-0.3.0/src/netunicorn/library/tasks/video_watchers/youtube_watcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import random
 import subprocess
 import time
 from typing import Optional
 from enum import IntEnum
 
-from netunicorn.base.task import Result, Failure, Success, Task, TaskDispatcher
+from netunicorn.base import Result, Failure, Success, Task, TaskDispatcher
 from netunicorn.base.nodes import Node
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
@@ -91,22 +91,22 @@
 
     driver.close()
     xvfb_process.kill()
     return result
 
 
 class WatchYouTubeVideo(TaskDispatcher):
-    def __init__(self, video_url: str, duration: Optional[int] = None):
+    def __init__(self, video_url: str, duration: Optional[int] = None, *args, **kwargs):
         self.video_url = video_url
         self.duration = duration
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def dispatch(self, node: Node) -> Task:
         if node.properties.get("os_family", "").lower() == "linux":
-            return WatchYouTubeVideoLinuxImplementation(self.video_url, self.duration)
+            return WatchYouTubeVideoLinuxImplementation(self.video_url, self.duration, name=self.name)
 
         raise NotImplementedError(
             f'WatchYouTubeVideo is not implemented for {node.properties.get("os_family", "")}'
         )
 
 
 class WatchYouTubeVideoLinuxImplementation(Task):
@@ -119,21 +119,23 @@
     ]
 
     def __init__(
         self,
         video_url: str,
         duration: Optional[int] = None,
         chrome_location: Optional[str] = None,
+        *args,
+        **kwargs,
     ):
         self.video_url = video_url
         self.duration = duration
         self.chrome_location = chrome_location
         if not self.chrome_location:
             self.chrome_location = "/usr/bin/chromium-browser"
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
     def run(self):
         return watch(self.video_url, self.duration, self.chrome_location)
 
 
 if __name__ == "__main__":
     print(watch("https://www.youtube.com/watch?v=dQw4w9WgXcQ", 10))
```

