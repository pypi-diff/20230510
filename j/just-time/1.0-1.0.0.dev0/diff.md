# Comparing `tmp/just_time-1.0.tar.gz` & `tmp/just_time-1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just_time-1.0.tar", last modified: Wed May 10 03:40:06 2023, max compression
+gzip compressed data, was "just_time-1.0.0.dev0.tar", last modified: Wed May 10 03:55:55 2023, max compression
```

## Comparing `just_time-1.0.tar` & `just_time-1.0.0.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 03:40:06.928751 just_time-1.0/
--rw-rw-rw-   0        0        0      164 2023-05-10 03:40:06.927751 just_time-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2196 2021-10-11 08:08:33.000000 just_time-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 03:40:06.906755 just_time-1.0/just_time/
--rw-rw-rw-   0        0        0       28 2023-05-10 03:17:48.000000 just_time-1.0/just_time/__init__.py
--rw-rw-rw-   0        0        0     8024 2021-10-11 09:19:27.000000 just_time-1.0/just_time/main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 03:40:06.924754 just_time-1.0/just_time.egg-info/
--rw-rw-rw-   0        0        0      164 2023-05-10 03:40:06.000000 just_time-1.0/just_time.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-10 03:40:06.000000 just_time-1.0/just_time.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 03:40:06.000000 just_time-1.0/just_time.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-05 08:18:13.000000 just_time-1.0/just_time.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-05-10 03:40:06.000000 just_time-1.0/just_time.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 03:40:06.928751 just_time-1.0/setup.cfg
--rw-rw-rw-   0        0        0      292 2021-02-17 14:57:08.000000 just_time-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:55:55.841241 just_time-1.0.0.dev0/
+-rw-rw-rw-   0        0        0      171 2023-05-10 03:55:55.840241 just_time-1.0.0.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     2196 2021-10-11 08:08:33.000000 just_time-1.0.0.dev0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 03:55:55.826241 just_time-1.0.0.dev0/just_time/
+-rw-rw-rw-   0        0        0       28 2023-05-10 03:17:48.000000 just_time-1.0.0.dev0/just_time/__init__.py
+-rw-rw-rw-   0        0        0     8022 2023-05-10 03:47:09.000000 just_time-1.0.0.dev0/just_time/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 03:55:55.838241 just_time-1.0.0.dev0/just_time.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-05-10 03:55:55.000000 just_time-1.0.0.dev0/just_time.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-10 03:55:55.000000 just_time-1.0.0.dev0/just_time.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 03:55:55.000000 just_time-1.0.0.dev0/just_time.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-05 08:18:13.000000 just_time-1.0.0.dev0/just_time.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-05-10 03:55:55.000000 just_time-1.0.0.dev0/just_time.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 03:55:55.841241 just_time-1.0.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      298 2023-05-10 03:55:16.000000 just_time-1.0.0.dev0/setup.py
```

### Comparing `just_time-1.0/README.md` & `just_time-1.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `just_time-1.0/just_time/main.py` & `just_time-1.0.0.dev0/just_time/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,9 +207,9 @@
     t3: JustTime = JustTime(0, 0, 2, 4_000_100)
     t4: JustTime = JustTime(0, 0, 2, 1_001_300)
     # print(t3._total_microseconds)
     print(t3 + t4)
     print(t3 - t4)
     print(t4 - t3)
     print(t4 <= t3)
-    # print(t3.total_seconds())
+    print(t3.total_seconds())
     # print(t3.hour)
```

