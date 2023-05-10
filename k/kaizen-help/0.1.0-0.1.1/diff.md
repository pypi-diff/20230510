# Comparing `tmp/kaizen_help-0.1.0.tar.gz` & `tmp/kaizen_help-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_help-0.1.0.tar", max compression
+gzip compressed data, was "kaizen_help-0.1.1.tar", max compression
```

## Comparing `kaizen_help-0.1.0.tar` & `kaizen_help-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-10 11:39:31.734696 kaizen_help-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-10 11:39:31.734650 kaizen_help-0.1.0/kaizen_help/__init__.py
--rw-r--r--   0        0        0      335 2023-05-10 11:42:57.211566 kaizen_help-0.1.0/kaizen_help/main.py
--rw-r--r--   0        0        0      420 2023-05-10 11:48:15.925890 kaizen_help-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 kaizen_help-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-10 11:39:31.734696 kaizen_help-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 11:39:31.734650 kaizen_help-0.1.1/kaizen_help/__init__.py
+-rw-r--r--   0        0        0     1259 2023-05-10 12:52:49.831959 kaizen_help-0.1.1/kaizen_help/files.py
+-rw-r--r--   0        0        0      254 2023-05-10 12:53:37.048880 kaizen_help-0.1.1/kaizen_help/funk.py
+-rw-r--r--   0        0        0      170 2023-05-10 12:13:37.618606 kaizen_help-0.1.1/kaizen_help/main.py
+-rw-r--r--   0        0        0      420 2023-05-10 12:59:11.960435 kaizen_help-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 kaizen_help-0.1.1/PKG-INFO
```

