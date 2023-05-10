# Comparing `tmp/discordgpt-0.0.1.tar.gz` & `tmp/discordgpt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordgpt-0.0.1.tar", last modified: Mon May  8 17:06:29 2023, max compression
+gzip compressed data, was "discordgpt-1.0.0.tar", last modified: Wed May 10 16:09:15 2023, max compression
```

## Comparing `discordgpt-0.0.1.tar` & `discordgpt-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:06:29.158201 discordgpt-0.0.1/
--rw-rw-rw-   0        0        0      124 2023-05-08 17:06:29.157202 discordgpt-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-08 17:06:29.156202 discordgpt-0.0.1/discordgpt.egg-info/
--rw-rw-rw-   0        0        0      124 2023-05-08 17:06:29.000000 discordgpt-0.0.1/discordgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-05-08 17:06:29.000000 discordgpt-0.0.1/discordgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:06:29.000000 discordgpt-0.0.1/discordgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-08 17:06:29.000000 discordgpt-0.0.1/discordgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-08 17:06:29.000000 discordgpt-0.0.1/discordgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       21 2023-05-08 16:39:07.000000 discordgpt-0.0.1/main.py
--rw-rw-rw-   0        0        0      262 2023-05-08 17:06:22.000000 discordgpt-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-08 17:06:29.158201 discordgpt-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 16:09:15.556112 discordgpt-1.0.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-10 15:51:27.000000 discordgpt-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     6631 2023-05-10 16:09:15.555110 discordgpt-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4625 2023-05-10 14:46:16.000000 discordgpt-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 16:09:15.550009 discordgpt-1.0.0/discordgpt/
+-rw-rw-rw-   0        0        0     4548 2023-05-10 16:08:43.000000 discordgpt-1.0.0/discordgpt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:09:15.554103 discordgpt-1.0.0/discordgpt.egg-info/
+-rw-rw-rw-   0        0        0     6631 2023-05-10 16:09:15.000000 discordgpt-1.0.0/discordgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-05-10 16:09:15.000000 discordgpt-1.0.0/discordgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:09:15.000000 discordgpt-1.0.0/discordgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-10 16:09:15.000000 discordgpt-1.0.0/discordgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-10 16:09:15.000000 discordgpt-1.0.0/discordgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      805 2023-05-10 16:02:53.000000 discordgpt-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 16:09:15.556112 discordgpt-1.0.0/setup.cfg
```

