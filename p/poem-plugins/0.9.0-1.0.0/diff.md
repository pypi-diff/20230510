# Comparing `tmp/poem_plugins-0.9.0.tar.gz` & `tmp/poem_plugins-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poem_plugins-0.9.0.tar", max compression
+gzip compressed data, was "poem_plugins-1.0.0.tar", max compression
```

## Comparing `poem_plugins-0.9.0.tar` & `poem_plugins-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,22 @@
--rw-r--r--   0        0        0     1068 2022-12-27 10:24:21.659617 poem_plugins-0.9.0/LICENSE
--rw-r--r--   0        0        0     1069 2022-12-27 13:09:07.229773 poem_plugins-0.9.0/README.md
--rw-r--r--   0        0        0        0 2022-12-27 10:25:45.722676 poem_plugins-0.9.0/poem_plugins/__init__.py
--rw-r--r--   0        0        0      299 2022-12-27 11:17:52.887688 poem_plugins-0.9.0/poem_plugins/base.py
--rw-r--r--   0        0        0      278 2022-12-27 13:09:07.230863 poem_plugins-0.9.0/poem_plugins/config.py
--rw-r--r--   0        0        0        0 2022-12-27 10:25:45.724315 poem_plugins-0.9.0/poem_plugins/general/__init__.py
--rw-r--r--   0        0        0      108 2022-12-27 13:14:54.687049 poem_plugins-0.9.0/poem_plugins/general/strenum.py
--rw-r--r--   0        0        0        0 2022-12-27 10:25:45.725571 poem_plugins-0.9.0/poem_plugins/versions/__init__.py
--rw-r--r--   0        0        0     3168 2022-12-27 13:16:51.598608 poem_plugins-0.9.0/poem_plugins/versions/git.py
--rw-r--r--   0        0        0     1749 2022-12-27 13:17:04.264842 poem_plugins-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 poem_plugins-0.9.0/setup.py
--rw-r--r--   0        0        0     2246 1970-01-01 00:00:00.000000 poem_plugins-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-03 09:22:00.689034 poem_plugins-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3899 2023-03-07 10:16:01.172838 poem_plugins-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-07 10:11:09.615671 poem_plugins-1.0.0/poem_plugins/__init__.py
+-rw-r--r--   0        0        0      976 2023-03-07 10:16:01.173047 poem_plugins-1.0.0/poem_plugins/config/__init__.py
+-rw-r--r--   0        0        0      920 2023-03-07 10:16:01.173221 poem_plugins-1.0.0/poem_plugins/config/base.py
+-rw-r--r--   0        0        0      559 2023-03-07 10:16:01.173385 poem_plugins-1.0.0/poem_plugins/config/git.py
+-rw-r--r--   0        0        0     1704 2023-05-10 08:10:38.820613 poem_plugins-1.0.0/poem_plugins/dispatchers/.null-ls_652473_version.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:11:09.619918 poem_plugins-1.0.0/poem_plugins/dispatchers/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-10 08:03:25.648558 poem_plugins-1.0.0/poem_plugins/dispatchers/base.py
+-rw-r--r--   0        0        0     1704 2023-05-10 08:10:33.973841 poem_plugins-1.0.0/poem_plugins/dispatchers/version.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:11:09.591018 poem_plugins-1.0.0/poem_plugins/general/__init__.py
+-rw-r--r--   0        0        0      227 2023-03-07 10:11:09.603142 poem_plugins-1.0.0/poem_plugins/general/strenum.py
+-rw-r--r--   0        0        0      339 2023-03-07 10:11:09.604862 poem_plugins-1.0.0/poem_plugins/general/version/__init__.py
+-rw-r--r--   0        0        0      332 2023-05-10 08:03:25.649086 poem_plugins-1.0.0/poem_plugins/general/version/drivers/__init__.py
+-rw-r--r--   0        0        0     2477 2023-05-10 08:03:25.649258 poem_plugins-1.0.0/poem_plugins/general/version/drivers/git.py
+-rw-r--r--   0        0        0      210 2023-05-10 08:03:25.649406 poem_plugins-1.0.0/poem_plugins/handlers/__init__.py
+-rw-r--r--   0        0        0     2437 2023-05-10 08:10:33.974122 poem_plugins-1.0.0/poem_plugins/handlers/version.py
+-rw-r--r--   0        0        0       86 2023-03-07 10:16:01.174074 poem_plugins-1.0.0/poem_plugins/plugins/__init__.py
+-rw-r--r--   0        0        0      133 2023-05-10 08:03:25.650066 poem_plugins-1.0.0/poem_plugins/plugins/base.py
+-rw-r--r--   0        0        0      540 2023-05-10 08:03:25.650236 poem_plugins-1.0.0/poem_plugins/plugins/version.py
+-rw-r--r--   0        0        0     2457 2023-05-10 08:12:14.458290 poem_plugins-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 poem_plugins-1.0.0/PKG-INFO
```

### Comparing `poem_plugins-0.9.0/LICENSE` & `poem_plugins-1.0.0/LICENSE`

 * *Files identical despite different names*

