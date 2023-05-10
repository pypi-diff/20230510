# Comparing `tmp/mdsanima_cli-0.2.0.tar.gz` & `tmp/mdsanima_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdsanima_cli-0.2.0.tar", last modified: Tue May  2 22:12:21 2023, max compression
+gzip compressed data, was "mdsanima_cli-0.2.1.tar", last modified: Wed May 10 21:16:44 2023, max compression
```

## Comparing `mdsanima_cli-0.2.0.tar` & `mdsanima_cli-0.2.1.tar`

### file list

```diff
@@ -1,57 +1,60 @@
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:21.734365 mdsanima_cli-0.2.0/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1355 2023-04-29 22:46:08.000000 mdsanima_cli-0.2.0/.editorconfig
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       79 2023-04-29 22:45:41.000000 mdsanima_cli-0.2.0/.flake8
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.511366 mdsanima_cli-0.2.0/.github/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       12 2023-02-06 22:39:55.000000 mdsanima_cli-0.2.0/.github/CODEOWNERS
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3873 2023-04-17 16:49:55.000000 mdsanima_cli-0.2.0/.gitignore
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.535361 mdsanima_cli-0.2.0/.idea/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      969 2023-05-02 21:20:31.000000 mdsanima_cli-0.2.0/.idea/commands.md
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      744 2023-04-29 23:16:48.000000 mdsanima_cli-0.2.0/.pylintrc
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.558364 mdsanima_cli-0.2.0/.vscode/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      149 2023-04-17 16:49:55.000000 mdsanima_cli-0.2.0/.vscode/.gitkeep
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    12450 2023-05-02 22:09:00.000000 mdsanima_cli-0.2.0/CHANGELOG.md
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    11356 2023-02-06 20:37:22.000000 mdsanima_cli-0.2.0/LICENSE
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    20472 2023-05-02 22:12:21.731363 mdsanima_cli-0.2.0/PKG-INFO
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4625 2023-05-02 21:43:43.000000 mdsanima_cli-0.2.0/README.md
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.607367 mdsanima_cli-0.2.0/img/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    61689 2023-04-26 18:07:04.000000 mdsanima_cli-0.2.0/img/logo.png
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    68193 2023-04-01 01:28:09.000000 mdsanima_cli-0.2.0/img/watermark.png
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2566 2023-05-02 21:43:14.000000 mdsanima_cli-0.2.0/package.json
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3616 2023-05-01 19:35:27.000000 mdsanima_cli-0.2.0/pyproject.toml
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      106 2023-04-29 22:32:42.000000 mdsanima_cli-0.2.0/requirements-dev.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       48 2023-04-27 16:55:13.000000 mdsanima_cli-0.2.0/requirements.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       38 2023-05-02 22:12:21.736365 mdsanima_cli-0.2.0/setup.cfg
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.631362 mdsanima_cli-0.2.0/src/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      149 2023-02-06 22:38:19.000000 mdsanima_cli-0.2.0/src/.gitkeep
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.739363 mdsanima_cli-0.2.0/src/mdsanima_cli/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1797 2023-05-02 21:20:31.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/__init__.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      230 2023-05-01 18:23:04.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/__main__.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      160 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/_version.py
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:21.451364 mdsanima_cli-0.2.0/src/mdsanima_cli/command/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       47 2023-05-01 17:52:04.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/__init__.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1445 2023-05-02 12:48:58.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/check.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4013 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/grid.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2495 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/jpg.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3497 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/logo.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2062 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/number.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2817 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/pixelart.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2494 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/png.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2973 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/thumbnail.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2000 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/uuids.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4472 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/watermark.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2510 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/command/webp.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     5359 2023-05-02 21:20:31.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/parser.py
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:21.692364 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       47 2023-05-01 17:51:47.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/__init__.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     9503 2023-05-02 21:20:54.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/ascii.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      734 2023-05-01 17:54:54.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/exif.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4367 2023-05-02 21:32:20.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/print.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2398 2023-05-01 17:51:14.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/stats.py
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      564 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.0/src/mdsanima_cli/utils/timer.py
-drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-02 22:12:20.910361 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    20472 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/PKG-INFO
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1203 2023-05-02 22:12:20.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/SOURCES.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        1 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/dependency_links.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       79 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/entry_points.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       48 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/requires.txt
--rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       13 2023-05-02 22:12:18.000000 mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/top_level.txt
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:44.087388 mdsanima_cli-0.2.1/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1355 2023-05-10 19:48:16.000000 mdsanima_cli-0.2.1/.editorconfig
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       79 2023-05-10 19:48:25.000000 mdsanima_cli-0.2.1/.flake8
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:42.254381 mdsanima_cli-0.2.1/.github/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       12 2023-02-06 22:39:55.000000 mdsanima_cli-0.2.1/.github/CODEOWNERS
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3873 2023-04-17 16:49:55.000000 mdsanima_cli-0.2.1/.gitignore
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:42.289381 mdsanima_cli-0.2.1/.idea/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1003 2023-05-06 16:09:11.000000 mdsanima_cli-0.2.1/.idea/commands.md
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      744 2023-05-10 19:48:35.000000 mdsanima_cli-0.2.1/.pylintrc
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:42.355380 mdsanima_cli-0.2.1/.vscode/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      149 2023-04-17 16:49:55.000000 mdsanima_cli-0.2.1/.vscode/.gitkeep
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      123 2023-05-10 20:16:05.000000 mdsanima_cli-0.2.1/.vscode/settings.json
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    13126 2023-05-10 21:14:31.000000 mdsanima_cli-0.2.1/CHANGELOG.md
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    11356 2023-02-06 20:37:22.000000 mdsanima_cli-0.2.1/LICENSE
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    20571 2023-05-10 21:16:44.083384 mdsanima_cli-0.2.1/PKG-INFO
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4724 2023-05-10 19:52:55.000000 mdsanima_cli-0.2.1/README.md
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:42.428382 mdsanima_cli-0.2.1/img/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    61689 2023-04-26 18:07:04.000000 mdsanima_cli-0.2.1/img/logo.png
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    68193 2023-04-01 01:28:09.000000 mdsanima_cli-0.2.1/img/watermark.png
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2566 2023-05-10 21:11:16.000000 mdsanima_cli-0.2.1/package.json
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3616 2023-05-10 19:48:44.000000 mdsanima_cli-0.2.1/pyproject.toml
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      106 2023-04-29 22:32:42.000000 mdsanima_cli-0.2.1/requirements-dev.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       48 2023-04-27 16:55:13.000000 mdsanima_cli-0.2.1/requirements.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       38 2023-05-10 21:16:44.088384 mdsanima_cli-0.2.1/setup.cfg
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:42.465382 mdsanima_cli-0.2.1/src/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      149 2023-02-06 22:38:19.000000 mdsanima_cli-0.2.1/src/.gitkeep
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:42.638383 mdsanima_cli-0.2.1/src/mdsanima_cli/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2031 2023-05-06 15:44:23.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/__init__.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      230 2023-05-01 18:23:04.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/__main__.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      160 2023-05-10 21:16:40.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/_version.py
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:43.808383 mdsanima_cli-0.2.1/src/mdsanima_cli/command/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       47 2023-05-01 17:52:04.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/__init__.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1439 2023-05-10 20:43:37.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/check.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     5186 2023-05-10 20:52:55.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/gifmaker.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4001 2023-05-10 20:45:24.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/grid.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2489 2023-05-10 20:44:43.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/jpg.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3478 2023-05-10 20:44:20.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/logo.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2056 2023-05-10 20:44:06.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/number.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     3135 2023-05-10 20:45:13.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/pixelart.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2488 2023-05-10 20:44:52.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/png.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2885 2023-05-10 20:45:54.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/resize.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2986 2023-05-10 20:45:35.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/thumbnail.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1994 2023-05-10 20:43:46.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/uuids.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4466 2023-05-10 20:44:32.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/watermark.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2504 2023-05-10 20:45:03.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/command/webp.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     5656 2023-05-10 21:01:05.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/parser.py
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:44.037382 mdsanima_cli-0.2.1/src/mdsanima_cli/utils/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       47 2023-05-01 17:51:47.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/utils/__init__.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     9477 2023-05-10 20:04:32.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/utils/ascii.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      734 2023-05-10 20:02:38.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/utils/exif.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     4399 2023-05-10 20:01:36.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/utils/print.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     2398 2023-05-10 19:59:52.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/utils/stats.py
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)      564 2023-05-02 21:20:55.000000 mdsanima_cli-0.2.1/src/mdsanima_cli/utils/timer.py
+drwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        0 2023-05-10 21:16:42.911385 mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)    20571 2023-05-10 21:16:40.000000 mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/PKG-INFO
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)     1297 2023-05-10 21:16:41.000000 mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)        1 2023-05-10 21:16:40.000000 mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       79 2023-05-10 21:16:40.000000 mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/entry_points.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       48 2023-05-10 21:16:40.000000 mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/requires.txt
+-rwxrwxrwx   0 mdsanima  (1000) mdsanima  (1000)       13 2023-05-10 21:16:40.000000 mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/top_level.txt
```

### Comparing `mdsanima_cli-0.2.0/.editorconfig` & `mdsanima_cli-0.2.1/.editorconfig`

 * *Files 6% similar despite different names*

```diff
@@ -41,25 +41,25 @@
 indent_size = 2
 indent_style = space
 end_of_line = lf
 
 [*.md]
 indent_size = 2
 indent_style = space
-max_line_length = 100
+max_line_length = 120
 
 [*.ps1]
 indent_size = 2
 indent_style = space
 
 [*.py]
 profile = black
 indent_size = 4
 indent_style = space
-max_line_length = 100
+max_line_length = 120
 
 [*.sh]
 indent_size = 2
 indent_style = space
 
 [*.svg]
 insert_final_newline = false
```

### Comparing `mdsanima_cli-0.2.0/.gitignore` & `mdsanima_cli-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mdsanima_cli-0.2.0/.idea/commands.md` & `mdsanima_cli-0.2.1/.idea/commands.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Command Ideas
+# Commands Idea
 
 Here are some ideas for commands that we need to implement in this package.
 
 You can use the `mdsanima` command or the `mds` alias, which have the same functionality.
 
 - [x] `mdsanima` main command showing help
 - [x] `mdsanima check` print directory info
@@ -12,14 +12,14 @@
 - [x] `mdsanima watermark` append a watermark
 - [x] `mdsanima jpg` convert to jpg
 - [x] `mdsanima png` convert to png
 - [x] `mdsanima webp` convert to webp
 - [x] `mdsanima pixelart` generate pixel art 32px
 - [x] `mdsanima grid` generate grid 2x2
 - [x] `mdsanima thumbnail` generate jpeg thumbnail 128px
-- [ ] `mdsanima gif` generate gif
+- [x] `mdsanima gifmaker` generate gif animation pixel art
+- [x] `mdsanima resize` resizing to 512px width
 - [ ] `mdsanima multi` generate multi resolution
 - [ ] `mdsanima caption` adding caption
 - [ ] `mdsanima bg` adding background
 - [ ] `mdsanima filter` adding filter
-- [ ] `mdsanima resize` resizing image
 - [ ] `mdsanima crop` cropping image
```

### Comparing `mdsanima_cli-0.2.0/.pylintrc` & `mdsanima_cli-0.2.1/.pylintrc`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Use multiple processes to speed up Pylint.
 jobs=4
 
 
 [FORMAT]
 
 # Maximum number of characters on a single line.
-max-line-length=100
+max-line-length=120
 
 # Maximum number of lines in a module.
 max-module-lines=1000
 
 
 [DESIGN]
 
@@ -27,11 +27,11 @@
 # Maximum number of locals for function / method body.
 max-locals=30
 
 # Maximum number of return / yield for function / method body.
 max-returns=6
 
 # Maximum number of branch for function / method body.
-max-branches=12
+max-branches=20
 
 # Maximum number of statements in function / method body.
 max-statements=50
```

### Comparing `mdsanima_cli-0.2.0/CHANGELOG.md` & `mdsanima_cli-0.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,25 @@
 Please check [standard-version](https://github.com/conventional-changelog/standard-version)
 and documentation for commit guidelines. Also you should check
 [conventional-changelog](https://github.com/mdsanima/conventional-changelog) for more detail.
 
 Docomentation for _MDSANIMA-CLI_ is available at this repository on [README.md](README.md)
 file be sure to check it.
 
+### 0.2.1 (2023-05-10)
+
+### FEATURES
+
+- generate gif animation pixel art closes [#18](https://github.com/mdsanima-lab/mdsanima-cli/issues/18) ([a502a2e](https://github.com/mdsanima-lab/mdsanima-cli/commit/a502a2e6162b032513398473aad299e5d564b566))
+- resizing to 512px width closes [#14](https://github.com/mdsanima-lab/mdsanima-cli/issues/14) ([c016b43](https://github.com/mdsanima-lab/mdsanima-cli/commit/c016b43e239a5226a04f4fe377176719fea3385f))
+
+### BUG FIXES
+
+- **gifmaker:** generate 512px gif closes [#42](https://github.com/mdsanima-lab/mdsanima-cli/issues/42) ([dddca30](https://github.com/mdsanima-lab/mdsanima-cli/commit/dddca3008d8f43df1339a3d6f604d4730825e559))
+
 ## 0.2.0 (2023-05-02)
 
 ### ⚠ BREAKING CHANGES
 
 - **dev:** helper function for print done message in color
 - module prefix `cli` rename file
 - more stats info for `get_directory_info` function
```

### Comparing `mdsanima_cli-0.2.0/LICENSE` & `mdsanima_cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdsanima_cli-0.2.0/PKG-INFO` & `mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mdsanima_cli
-Version: 0.2.0
+Name: mdsanima-cli
+Version: 0.2.1
 Summary: The package will provide command-line tools for image processing, generating pixel art, adding logos to images, and much more.
 Author-email: Marcin Różewski <marcinrozewski@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -254,16 +254,16 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mdsanima-cli
 
-The package will provide command-line tools for image processing, generating pixel art, adding logos
-to images, and much more.
+The package will provide command-line tools for image processing, generating pixel art, adding logos to images, and much
+more.
 
 ## Installation
 
 Install latest version:
 
 ```shell
 python3 -m pip install mdsanima-cli
@@ -299,29 +299,29 @@
 - `mdsanima watermark` append a watermark
 - `mdsanima jpg` convert to jpg
 - `mdsanima png` convert to png
 - `mdsanima webp` convert to webp
 - `mdsanima pixelart` generate pixel art 32px
 - `mdsanima grid` generate grid 2x2
 - `mdsanima thumbnail` generate jpeg thumbnail 128px
+- `mdsanima gifmaker` generate gif animation pixel art
+- `mdsanima resize` resizing to 512px width
 
-The `pixelart` command works in folder that have only `.png` images and convert this images to pixel
-art with creating the new file and appending the suffix `pixelart` to original file name.
+The `pixelart` command works in folder that have only `.png` images and convert this images to pixel art with creating
+the new file and appending the suffix `pixelart` to original file name.
 
-After executing this command, all image files in the folder you are in will be processed.
-The command does not delete any files in the folder, it only adds new ones and showing the directory
-info.
+After executing this command, all image files in the folder you are in will be processed. The command does not delete
+any files in the folder, it only adds new ones and showing the directory info.
 
 ## Development Setup
 
 Instruction step how to setup development environent is here on this
 [workflow](https://mdsanima-dev.github.io/mdsanima-dev/development/workflow/) instruction.
 
-Creating isolated environment with specific pip version then activate and install requirements, type
-in terminal:
+Creating isolated environment with specific pip version then activate and install requirements, type in terminal:
 
 ```shell
 virtualenv --setuptools 67.7.2 --wheel 0.40.0 --pip 23.1.2 .venv
 source .venv/bin/activate
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
 ```
@@ -360,22 +360,21 @@
 
 ```shell
 python3 src/mdsanima_cli/command/pixelart.py
 ```
 
 ### Extracts Version Package
 
-This `setuptools-scm` tools allow to extract **Python** package version from `git` instead declaring
-them as the version argument.
+This `setuptools-scm` tools allow to extract **Python** package version from `git` instead declaring them as the version
+argument.
 
-Check the `pyproject.toml` file and this
-[instruction](https://pypi.org/project/setuptools-scm/) for more info.
+Check the `pyproject.toml` file and this [instruction](https://pypi.org/project/setuptools-scm/) for more info.
 
-If you need to confirm which version string is being generated or debug the configuration, you can
-install `setuptools-scm` directly in your working environment `pip install setuptools-scm` and run:
+If you need to confirm which version string is being generated or debug the configuration, you can install
+`setuptools-scm` directly in your working environment `pip install setuptools-scm` and run:
 
 ```shell
 python -m setuptools_scm
 ```
 
 ### Creating Release
 
@@ -392,49 +391,48 @@
 
 Important steps is commit the change like this, type in terminal:
 
 ```shell
 git commit -m "feat: generating pixel art command"
 ```
 
-Always use this format for commiting to git, becouse this allows to generate changelog from the
-commit message. Check the `package.json` file on `standard-version` section and types lists for
-fist string thats you can type in commit message.
+Always use this format for commiting to git, becouse this allows to generate changelog from the commit message. Check
+the `package.json` file on `standard-version` section and types lists for fist string thats you can type in commit
+message.
 
-The next step is bumping version on `package.json` file and generate `CHANGELOG.md` file with new
-release information, type in terminal:
+The next step is bumping version on `package.json` file and generate `CHANGELOG.md` file with new release information,
+type in terminal:
 
 ```shell
 standard-version
 ```
 
 Next is a add this changes to git, type in terminal:
 
 ```shell
 git commit -am "chore(release): 0.1.2"
 ```
 
-The version abowe is a from `standard-version` command and this is a only example version.
-The version must always be changed when a new version is released.
+The version abowe is a from `standard-version` command and this is a only example version. The version must always be
+changed when a new version is released.
 
 The next steps is a creating a tag and pushing the change to origin with tag, type in terminal:
 
 ```shell
 git tag 0.1.2
 git push origin && git push origin --tag
 ```
 
 Checking the extracts version, type in terminal:
 
 ```shell
 python -m setuptools_scm
 ```
 
-Finally create the build and update this build to
-[test.pypi.org](https://test.pypi.org/project/mdsanima-cli/) and
+Finally create the build and update this build to [test.pypi.org](https://test.pypi.org/project/mdsanima-cli/) and
 [pypi.org](https://pypi.org/project/mdsanima-cli/) but first you must check and then update.
 
 ```shell
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
```

### Comparing `mdsanima_cli-0.2.0/README.md` & `mdsanima_cli-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # mdsanima-cli
 
-The package will provide command-line tools for image processing, generating pixel art, adding logos
-to images, and much more.
+The package will provide command-line tools for image processing, generating pixel art, adding logos to images, and much
+more.
 
 ## Installation
 
 Install latest version:
 
 ```shell
 python3 -m pip install mdsanima-cli
@@ -41,29 +41,29 @@
 - `mdsanima watermark` append a watermark
 - `mdsanima jpg` convert to jpg
 - `mdsanima png` convert to png
 - `mdsanima webp` convert to webp
 - `mdsanima pixelart` generate pixel art 32px
 - `mdsanima grid` generate grid 2x2
 - `mdsanima thumbnail` generate jpeg thumbnail 128px
+- `mdsanima gifmaker` generate gif animation pixel art
+- `mdsanima resize` resizing to 512px width
 
-The `pixelart` command works in folder that have only `.png` images and convert this images to pixel
-art with creating the new file and appending the suffix `pixelart` to original file name.
+The `pixelart` command works in folder that have only `.png` images and convert this images to pixel art with creating
+the new file and appending the suffix `pixelart` to original file name.
 
-After executing this command, all image files in the folder you are in will be processed.
-The command does not delete any files in the folder, it only adds new ones and showing the directory
-info.
+After executing this command, all image files in the folder you are in will be processed. The command does not delete
+any files in the folder, it only adds new ones and showing the directory info.
 
 ## Development Setup
 
 Instruction step how to setup development environent is here on this
 [workflow](https://mdsanima-dev.github.io/mdsanima-dev/development/workflow/) instruction.
 
-Creating isolated environment with specific pip version then activate and install requirements, type
-in terminal:
+Creating isolated environment with specific pip version then activate and install requirements, type in terminal:
 
 ```shell
 virtualenv --setuptools 67.7.2 --wheel 0.40.0 --pip 23.1.2 .venv
 source .venv/bin/activate
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
 ```
@@ -102,22 +102,21 @@
 
 ```shell
 python3 src/mdsanima_cli/command/pixelart.py
 ```
 
 ### Extracts Version Package
 
-This `setuptools-scm` tools allow to extract **Python** package version from `git` instead declaring
-them as the version argument.
+This `setuptools-scm` tools allow to extract **Python** package version from `git` instead declaring them as the version
+argument.
 
-Check the `pyproject.toml` file and this
-[instruction](https://pypi.org/project/setuptools-scm/) for more info.
+Check the `pyproject.toml` file and this [instruction](https://pypi.org/project/setuptools-scm/) for more info.
 
-If you need to confirm which version string is being generated or debug the configuration, you can
-install `setuptools-scm` directly in your working environment `pip install setuptools-scm` and run:
+If you need to confirm which version string is being generated or debug the configuration, you can install
+`setuptools-scm` directly in your working environment `pip install setuptools-scm` and run:
 
 ```shell
 python -m setuptools_scm
 ```
 
 ### Creating Release
 
@@ -134,49 +133,48 @@
 
 Important steps is commit the change like this, type in terminal:
 
 ```shell
 git commit -m "feat: generating pixel art command"
 ```
 
-Always use this format for commiting to git, becouse this allows to generate changelog from the
-commit message. Check the `package.json` file on `standard-version` section and types lists for
-fist string thats you can type in commit message.
+Always use this format for commiting to git, becouse this allows to generate changelog from the commit message. Check
+the `package.json` file on `standard-version` section and types lists for fist string thats you can type in commit
+message.
 
-The next step is bumping version on `package.json` file and generate `CHANGELOG.md` file with new
-release information, type in terminal:
+The next step is bumping version on `package.json` file and generate `CHANGELOG.md` file with new release information,
+type in terminal:
 
 ```shell
 standard-version
 ```
 
 Next is a add this changes to git, type in terminal:
 
 ```shell
 git commit -am "chore(release): 0.1.2"
 ```
 
-The version abowe is a from `standard-version` command and this is a only example version.
-The version must always be changed when a new version is released.
+The version abowe is a from `standard-version` command and this is a only example version. The version must always be
+changed when a new version is released.
 
 The next steps is a creating a tag and pushing the change to origin with tag, type in terminal:
 
 ```shell
 git tag 0.1.2
 git push origin && git push origin --tag
 ```
 
 Checking the extracts version, type in terminal:
 
 ```shell
 python -m setuptools_scm
 ```
 
-Finally create the build and update this build to
-[test.pypi.org](https://test.pypi.org/project/mdsanima-cli/) and
+Finally create the build and update this build to [test.pypi.org](https://test.pypi.org/project/mdsanima-cli/) and
 [pypi.org](https://pypi.org/project/mdsanima-cli/) but first you must check and then update.
 
 ```shell
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
```

### Comparing `mdsanima_cli-0.2.0/img/logo.png` & `mdsanima_cli-0.2.1/img/logo.png`

 * *Files identical despite different names*

### Comparing `mdsanima_cli-0.2.0/img/watermark.png` & `mdsanima_cli-0.2.1/img/watermark.png`

 * *Files identical despite different names*

### Comparing `mdsanima_cli-0.2.0/package.json` & `mdsanima_cli-0.2.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -77,9 +77,9 @@
             },
             {
                 "hidden": true,
                 "type": "chore"
             }
         ]
     },
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `mdsanima_cli-0.2.0/pyproject.toml` & `mdsanima_cli-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 changelog = 'https://github.com/mdsanima-lab/mdsanima-cli/blob/main/CHANGELOG.md'
 
 [project.scripts]
 mdsanima = 'mdsanima_cli:main_cli'
 mds = 'mdsanima_cli:main_cli'
 
 [tool.black]
-line-length = 100
+line-length = 120
 target-version = ['py310']
 include = '\.pyi?$'
 
 [tool.isort]
 profile = 'black'
 src_paths = ['src', 'tests']
 force_single_line = true
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/__init__.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 
 """Initial main functionality for command-line tools."""
 
 
 from __future__ import annotations
 
 from mdsanima_cli.command.check import cli_check
+from mdsanima_cli.command.gifmaker import cli_gifmaker
 from mdsanima_cli.command.grid import cli_grid
 from mdsanima_cli.command.jpg import cli_jpg
 from mdsanima_cli.command.logo import cli_logo
 from mdsanima_cli.command.number import cli_number
 from mdsanima_cli.command.pixelart import cli_pixelart
 from mdsanima_cli.command.png import cli_png
+from mdsanima_cli.command.resize import cli_resize
 from mdsanima_cli.command.thumbnail import cli_thumbnail
 from mdsanima_cli.command.uuids import cli_uuid
 from mdsanima_cli.command.watermark import cli_watermark
 from mdsanima_cli.command.webp import cli_webp
 from mdsanima_cli.parser import create_parser
 from mdsanima_cli.utils.ascii import ascii_title
 
@@ -50,9 +52,13 @@
             cli_webp()
         if args.command == "pixelart":
             cli_pixelart()
         if args.command == "grid":
             cli_grid()
         if args.command == "thumbnail":
             cli_thumbnail()
+        if args.command == "gifmaker":
+            cli_gifmaker()
+        if args.command == "resize":
+            cli_resize()
     except AttributeError:
         parser.print_help()
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/check.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 """Checking and displaying info about all images in current directory."""
 
 
 from __future__ import annotations
 
-from mdsanima_cli.parser import CHECK_COMMAND
+from mdsanima_cli.parser import CHECK_COMD
 from mdsanima_cli.parser import CHECK_HELP
 from mdsanima_cli.utils.print import print_cli_data
 from mdsanima_cli.utils.print import print_cli_info
 from mdsanima_cli.utils.stats import get_directory_statistic
 
 
 def directory_statistic(cli_command: str, cli_help: str) -> str:
@@ -32,8 +32,8 @@
     print_cli_data("webp", info["webp"], 34, 24, 52)
     print_cli_data("gif", info["gif"], 34, 24, 52)
     print_cli_data("other", info["other"], 34, 24, 52)
 
 
 def cli_check() -> None:
     """Main function for `check` command."""
-    directory_statistic(CHECK_COMMAND, CHECK_HELP)
+    directory_statistic(CHECK_COMD, CHECK_HELP)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/grid.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""Generating a grid from all images in the current directory. It operates within a specified folder
-and can process all images at once.
+"""Generating a grid from all images in the current directory. It operates within a specified folder and can process all
+images at once.
 """
 
 
 from __future__ import annotations
 
 import os
 
 from PIL import Image
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import GRID_COMMAND
+from mdsanima_cli.parser import GRID_COMD
 from mdsanima_cli.parser import GRID_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.exif import get_exif_bytes
 from mdsanima_cli.utils.print import print_cli_comp
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
 
 @timer
-def generate_grid(
-    image_1_path: str, image_2_path: str, image_3_path: str, image_4_path: str, grid_name: str
-) -> None:
-    """Generating a grid 2x2 from four images, and then save the result with a new file name.
-    Images must be the same size. Adding exif data.
+def generate_grid(image_1_path: str, image_2_path: str, image_3_path: str, image_4_path: str, grid_name: str) -> None:
+    """Generating a grid 2x2 from four images, and then save the result with a new file name. Images must be the same
+    size. Adding exif data.
     """
 
     # Open four images file.
     image_1 = Image.open(image_1_path)
     image_2 = Image.open(image_2_path)
     image_3 = Image.open(image_3_path)
     image_4 = Image.open(image_4_path)
@@ -105,12 +103,12 @@
                 grid += 1
                 images = []
             count += 1
 
 
 def cli_grid() -> None:
     """Main function for `grid` command."""
-    directory_statistic(GRID_COMMAND, GRID_HELP)
+    directory_statistic(GRID_COMD, GRID_HELP)
     ascii_title("processing")
     time_taken = compute_grid()
     ascii_title("completed")
     print_cli_done(time_taken)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/jpg.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/jpg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""Converting images to JPG format from all images in the curreny directory. It operates within
-a specified folder and can process all images at once.
+"""Converting images to JPG format from all images in the curreny directory. It operates within a specified folder and
+can process all images at once.
 """
 
 
 from __future__ import annotations
 
 import os
 
 from PIL import Image
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import JPG_COMMAND
+from mdsanima_cli.parser import JPG_COMD
 from mdsanima_cli.parser import JPG_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.exif import get_exif_bytes
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
@@ -67,12 +67,12 @@
             time_taken = convert_to_jpg(file, new_name)
             print_cli_proc("converting", count, file, new_name, time_taken)
             count += 1
 
 
 def cli_jpg() -> None:
     """Main function for `jpg` command."""
-    directory_statistic(JPG_COMMAND, JPG_HELP)
+    directory_statistic(JPG_COMD, JPG_HELP)
     ascii_title("processing")
     time_taken = compute_jpg()
     ascii_title("completed")
     print_cli_done(time_taken)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/logo.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/logo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""Appendign a logo to all images in the current directory. It operates within a specified folder
-and can process all images at once.
+"""Appendign a logo to all images in the current directory. It operates within a specified folder and can process all
+images at once.
 """
 
 
 from __future__ import annotations
 
 import os
 
 from PIL import Image
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import LOGO_COMMAND
+from mdsanima_cli.parser import LOGO_COMD
 from mdsanima_cli.parser import LOGO_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.exif import get_exif_bytes
 from mdsanima_cli.utils.print import print_cli_data
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
 
 LOGO_PATH = os.path.expanduser("~/.mdsanima-cli/config/img/logo.png")
 
 
 @timer
 def append_logo(image_path: str, logo_path: str, new_name: str) -> None:
-    """Append a logo to one image in the bottom right position, and then save the result with a new
-    name and exif data.
-    """
+    """Append a logo to one image in the bottom right position, then save the result with a new name and exif data."""
 
     # Open image and logo file.
     image = Image.open(image_path)
     logo = Image.open(logo_path)
 
     # Image and logo size.
     image_width, image_height = image.size
@@ -89,15 +87,15 @@
             time_taken = append_logo(file, LOGO_PATH, new_name)
             print_cli_proc("computing", count, file, new_name, time_taken)
             count += 1
 
 
 def cli_logo() -> None:
     """Main function for `logo` command."""
-    directory_statistic(LOGO_COMMAND, LOGO_HELP)
+    directory_statistic(LOGO_COMD, LOGO_HELP)
 
     try:
         ascii_title("processing")
         time_taken = compute_logo()
         ascii_title("completed")
         print_cli_done(time_taken)
     except FileNotFoundError:
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/number.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/number.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from __future__ import annotations
 
 import os
 import shutil
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import NUMBER_COMMAND
+from mdsanima_cli.parser import NUMBER_COMD
 from mdsanima_cli.parser import NUMBER_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
 
@@ -57,12 +57,12 @@
             time_taken = rename_to_seq_number(file, new_name)
             print_cli_proc("renaming", count, file, new_name, time_taken)
         count += 1
 
 
 def cli_number() -> None:
     """Main function for `number` command."""
-    directory_statistic(NUMBER_COMMAND, NUMBER_HELP)
+    directory_statistic(NUMBER_COMD, NUMBER_HELP)
     ascii_title("processing")
     time_taken = compute_seq_number()
     ascii_title("completed")
     print_cli_done(time_taken)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/pixelart.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/pixelart.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""Generating images into pixel art. It operates within a specified folder and can process all
-images at once. The first step is to open the original image, scale it to 32x32 pixels, scale it
-back to its original size, and then save it.
+"""Generating images into pixel art. It operates within a specified folder and can process all images at once. The first
+step is to open the original image, scale it to 32 pixels, scale it back to its original size, and then save it.
 """
 
 
 from __future__ import annotations
 
 import os
 
 from PIL import Image
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import PIXELART_COMMAND
+from mdsanima_cli.parser import PIXELART_COMD
 from mdsanima_cli.parser import PIXELART_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.exif import get_exif_bytes
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
 
 @timer
-def generate_pixelart(image_path: str, new_name: str, res: int) -> None:
+def generate_pixelart(image_path: str, new_name: str, resolution: int) -> None:
     """Generate pixel art for one image, then save the result with a new name and exif data."""
 
     # Open image file.
     image = Image.open(image_path)
 
+    # Image size.
+    image_width, image_height = image.size
+
+    # Calculating resolution for pixelart.
+    resize_ratio = int(image_width / resolution)
+    pixelart_width = int(image_width / resize_ratio)
+    pixelart_height = int(image_height / resize_ratio)
+    pixelart_size = (pixelart_width, pixelart_height)
+
     # Generate one pixel art.
-    small_image = image.resize((res, res), resample=Image.Resampling.BILINEAR)
+    small_image = image.resize(pixelart_size, resample=Image.Resampling.BILINEAR)
     result = small_image.resize(image.size, Image.Resampling.NEAREST)
 
     # Add exif data.
     exif_bytes = get_exif_bytes(PIXELART_HELP)
 
     # Save the result.
     result.save(new_name, exif=exif_bytes)
@@ -72,12 +80,12 @@
             time_taken = generate_pixelart(file, new_name, 32)
             print_cli_proc("computing", count, file, new_name, time_taken)
             count += 1
 
 
 def cli_pixelart() -> None:
     """Main function for `pixelart` command."""
-    directory_statistic(PIXELART_COMMAND, PIXELART_HELP)
+    directory_statistic(PIXELART_COMD, PIXELART_HELP)
     ascii_title("processing")
     time_taken = compute_pixelart()
     ascii_title("completed")
     print_cli_done(time_taken)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/png.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/png.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""Converting images to PNG format from all images in the curreny directory. It operates within
-a specified folder and can process all images at once.
+"""Converting images to PNG format from all images in the curreny directory. It operates within a specified folder and
+can process all images at once.
 """
 
 
 from __future__ import annotations
 
 import os
 
 from PIL import Image
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import PNG_COMMAND
+from mdsanima_cli.parser import PNG_COMD
 from mdsanima_cli.parser import PNG_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.exif import get_exif_bytes
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
@@ -67,12 +67,12 @@
             time_taken = convert_to_png(file, new_name)
             print_cli_proc("converting", count, file, new_name, time_taken)
             count += 1
 
 
 def cli_png() -> None:
     """Main function for `png` command."""
-    directory_statistic(PNG_COMMAND, PNG_HELP)
+    directory_statistic(PNG_COMD, PNG_HELP)
     ascii_title("processing")
     time_taken = compute_png()
     ascii_title("completed")
     print_cli_done(time_taken)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/thumbnail.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/thumbnail.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""Generating JPEG thumbnails from all images in the curreny directory. It operates within
-a specified folder and can process all images at once.
+"""Generating JPEG thumbnails from all images in the curreny directory. It operates within a specified folder and can
+process all images at once.
 """
 
 
 from __future__ import annotations
 
 import os
 
 from PIL import Image
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import THUMBNAIL_COMMAND
+from mdsanima_cli.parser import THUMBNAIL_COMD
 from mdsanima_cli.parser import THUMBNAIL_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.exif import get_exif_bytes
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
 
 @timer
-def generate_jpeg_thumbnail(image_path: str, new_name: str) -> None:
-    """Generate JPEG thumbnail 128, and then save the result with a new name and exif data."""
+def generate_jpeg_thumbnail(image_path: str, new_name: str, resolution: int) -> None:
+    """Generate JPEG thumbnail, and then save the result with a new name and exif data."""
 
     # Open image file.
     image = Image.open(image_path)
 
     # Image size.
     image_width, image_height = image.size
 
     # Calculating size for thumbnail.
-    size = 128
-    resize_ratio = int(image_width / size)
+    resize_ratio = int(image_width / resolution)
     thumbnail_width = int(image_width / resize_ratio)
     thumbnail_height = int(image_height / resize_ratio)
     thumbnail_size = (thumbnail_width, thumbnail_height)
 
     # Add exif data.
     exif_bytes = get_exif_bytes(THUMBNAIL_HELP)
 
@@ -61,29 +60,29 @@
     jpg = ".jpg"
     webp = ".webp"
 
     # Checking extension and compute thumbnail from all images in directory.
     for file in directory:
         if file.endswith(png) and not file.endswith(suffix + jpg):
             new_name = file[:-4] + suffix + jpg
-            time_teken = generate_jpeg_thumbnail(file, new_name)
+            time_teken = generate_jpeg_thumbnail(file, new_name, 128)
             print_cli_proc("computing", count, file, new_name, time_teken)
             count += 1
         if file.endswith(jpg) and not file.endswith(suffix + jpg):
             new_name = file[:-4] + suffix + jpg
-            time_teken = generate_jpeg_thumbnail(file, new_name)
+            time_teken = generate_jpeg_thumbnail(file, new_name, 128)
             print_cli_proc("computing", count, file, new_name, time_teken)
             count += 1
         if file.endswith(webp) and not file.endswith(suffix + jpg):
             new_name = file[:-5] + suffix + jpg
-            time_teken = generate_jpeg_thumbnail(file, new_name)
+            time_teken = generate_jpeg_thumbnail(file, new_name, 128)
             print_cli_proc("computing", count, file, new_name, time_teken)
             count += 1
 
 
 def cli_thumbnail() -> None:
     """Main function for `thumbnail` command."""
-    directory_statistic(THUMBNAIL_COMMAND, THUMBNAIL_HELP)
+    directory_statistic(THUMBNAIL_COMD, THUMBNAIL_HELP)
     ascii_title("processing")
     time_taken = compute_thumbnail()
     ascii_title("completed")
     print_cli_done(time_taken)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/uuids.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/uuids.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from __future__ import annotations
 
 import os
 import shutil
 import uuid
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import UUID_COMMAND
+from mdsanima_cli.parser import UUID_COMD
 from mdsanima_cli.parser import UUID_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
 
@@ -59,12 +59,12 @@
             time_taken = rename_to_uuid(file, new_name)
             print_cli_proc("renaming", count, file, new_name, time_taken)
         count += 1
 
 
 def cli_uuid() -> None:
     """Main function for `uuid` command."""
-    directory_statistic(UUID_COMMAND, UUID_HELP)
+    directory_statistic(UUID_COMD, UUID_HELP)
     ascii_title("processing")
     time_taken = compute_uuid()
     ascii_title("completed")
     print_cli_done(time_taken)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/watermark.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/watermark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""This module is designed to adding a watermark to all images in the current directory. It operates
-within a specified folder and can process all images at once.
+"""This module is designed to adding a watermark to all images in the current directory. It operates within a specified
+folder and can process all images at once.
 """
 
 
 from __future__ import annotations
 
 import os
 
 from PIL import Image
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import WATERMARK_COMMAND
+from mdsanima_cli.parser import WATERMARK_COMD
 from mdsanima_cli.parser import WATERMARK_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.exif import get_exif_bytes
 from mdsanima_cli.utils.print import print_cli_data
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
 
 WATERMARK_PATH = os.path.expanduser("~/.mdsanima-cli/config/img/watermark.png")
 
 
 @timer
 def append_watermark(image_path: str, waterm_path: str, new_name: str) -> None:
-    """Append a watermark to one image, and then save the result with a new name and exif data.
-    The watermark is a rotated on 45 degrees and shifted.
+    """Append a watermark to one image, and then save the result with a new name and exif data. The watermark is
+    a rotated on 45 degrees and shifted.
     """
 
     # Open image and watermark file.
     image = Image.open(image_path)
     watermark = Image.open(waterm_path)
 
     # Image and watermark size.
@@ -108,15 +108,15 @@
             time_taken = append_watermark(file, WATERMARK_PATH, new_name)
             print_cli_proc("computing", count, file, new_name, time_taken)
             count += 1
 
 
 def cli_watermark() -> None:
     """Main function for `watermark` command."""
-    directory_statistic(WATERMARK_COMMAND, WATERMARK_HELP)
+    directory_statistic(WATERMARK_COMD, WATERMARK_HELP)
 
     try:
         ascii_title("processing")
         time_taken = compute_watermark()
         ascii_title("completed")
         print_cli_done(time_taken)
     except FileNotFoundError:
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/command/webp.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/command/webp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""Converting images to WebP format from all images in the curreny directory. It operates within
-a specified folder and can process all images at once.
+"""Converting images to WebP format from all images in the curreny directory. It operates within a specified folder and
+can process all images at once.
 """
 
 
 from __future__ import annotations
 
 import os
 
 from PIL import Image
 
 from mdsanima_cli.command.check import directory_statistic
-from mdsanima_cli.parser import WEBP_COMMAND
+from mdsanima_cli.parser import WEBP_COMD
 from mdsanima_cli.parser import WEBP_HELP
 from mdsanima_cli.utils.ascii import ascii_title
 from mdsanima_cli.utils.exif import get_exif_bytes
 from mdsanima_cli.utils.print import print_cli_done
 from mdsanima_cli.utils.print import print_cli_proc
 from mdsanima_cli.utils.timer import timer
 
@@ -67,12 +67,12 @@
             time_taken = convert_to_webp(file, new_name)
             print_cli_proc("converting", count, file, new_name, time_taken)
             count += 1
 
 
 def cli_webp() -> None:
     """Main function for `webp` command."""
-    directory_statistic(WEBP_COMMAND, WEBP_HELP)
+    directory_statistic(WEBP_COMD, WEBP_HELP)
     ascii_title("processing")
     time_taken = compute_webp()
     ascii_title("completed")
     print_cli_done(time_taken)
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/utils/ascii.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/utils/ascii.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 
 from typing import Literal
 
 from mdsanima_dev.colors import get_complex_color
 
 
 def get_ascii_character() -> dict:
-    """This function returns a single ASCII character that includes the entire alphabet, numbers,
-    and some special characters includes spaces. Each character is displayed on 3 lines, and the
-    width is 3 normal-length spaces.
+    """This function returns a single ASCII character that includes the entire alphabet, numbers, and some special
+    characters includes spaces. Each character is displayed on 3 lines, and the width is 3 normal-length spaces.
 
-    Usage: `ascii["a"][0]` returns the first line of the character `a` in ASCII format. To obtain
-    the entire character, you need to retrieve lines `ascii["a"][1]` and `ascii["a"][2]` as well.
+    Usage: `ascii["a"][0]` returns the first line of the character `a` in ASCII format. To obtain the entire character,
+    you need to retrieve lines `ascii["a"][1]` and `ascii["a"][2]` as well.
 
     Return: `dict[str, list[str]]`
 
     Characters: `ABCDEFGHIJKLMNOPQRSTUVWXYZ`
     Numbers: `0123456789`
     Specials: `()[]{}!?$*-+=_|;:,. `
     """
@@ -309,20 +308,16 @@
             "   ",
         ],
     }
 
     return ascii_character
 
 
-def ascii_border(
-    line_1: str, line_2: str, line_3: str, border_color: int, ascii_color: int, width: int = 50
-) -> None:
-    """Generate ASCII art text in color and with a border. Printing ASCI art in 5 lines. You can
-    adjust a width and color.
-    """
+def ascii_border(line_1: str, line_2: str, line_3: str, border_color: int, ascii_color: int, width: int = 50) -> None:
+    """Generate ASCII text in color and with a border. Print ASCI art in 5 lines. You can adjust a width and color."""
 
     # Color print variable.
     mprint = get_complex_color
 
     # Variables for border.
     border_vertical = "│"
     border_horizontal = "─" * width
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/utils/exif.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/utils/exif.py`

 * *Files identical despite different names*

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/utils/print.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/utils/print.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""This module provides various utilities helpers that can be used for one line multiple colors
-printing. The module is intended for use in development.
+"""This module provides various utilities helpers that can be used for one line multiple colors printing. The module is
+intended for use in development.
 """
 
 
 from __future__ import annotations
 
 from typing import Literal
 
 from mdsanima_dev.colors import get_complex_color
 
 
 mprint = get_complex_color
 
 
-def print_cli_info(
-    key: str, info: str, bracket_color: int, key_color: int, info_color: int
-) -> None:
-    """Helper for printing multiple colors info in one line. Aligning the last bracket to the right
-    within a maximum width of 14 characters. You can choose individual colors for the bracket, text
-    inside the bracket, and the last text. The string `key` and `info` are always printed in upper
-    case.
+def print_cli_info(key: str, info: str, bracket_color: int, key_color: int, info_color: int) -> None:
+    """Helper for printing multiple colors info in one line. Aligning the last bracket to the right within a maximum
+    width of 14 characters. You can choose individual colors for the bracket, text inside the bracket, and the last
+    text. The string `key` and `info` are always printed in upper case.
 
     Example look: `[MDSANIMA CLI] -> CHECK`
     """
 
     # Calculating align spaces.
     align = len(key) + 1
 
@@ -34,20 +31,18 @@
     mprint("[".rjust(14 - align), bracket_color, "")
     mprint(str(key).upper(), key_color, "")
     mprint("]", bracket_color, "")
     mprint(" -> ", 197, "")
     mprint(str(info).upper(), info_color)
 
 
-def print_cli_data(
-    key: str, data: str, bracket_color: int, key_color: int, data_color: int
-) -> None:
-    """Helper for printing multiple colors data in one line. Aligning the last bracket to the right
-    within a maximum width of 14 characters. You can choose individual colors for the bracket, text
-    inside the bracket, and the last text. The string `key` are always printed in upper case.
+def print_cli_data(key: str, data: str, bracket_color: int, key_color: int, data_color: int) -> None:
+    """Helper for printing multiple colors data in one line. Aligning the last bracket to the right within a maximum
+    width of 14 characters. You can choose individual colors for the bracket, text inside the bracket, and the last
+    text. The string `key` are always printed in upper case.
 
     Example look: `[REAL PATH] /home/mdsanima/dev/mdsanima-cli`
     """
 
     # Calculating align spaces.
     align = len(key) + 1
 
@@ -55,23 +50,23 @@
     mprint("[".rjust(14 - align), bracket_color, "")
     mprint(str(key).upper(), key_color, "")
     mprint("]", bracket_color, " ")
     mprint(str(data), data_color)
 
 
 def print_cli_proc(
-    process: Literal["appending", "computing", "converting", "renaming"],
+    process: Literal["appending", "computing", "converting", "generating", "renaming", "resizing"],
     count: int,
     old: str,
     new: str,
     time_taken: float,
 ) -> None:
-    """Helper for printing multiple colors processing info in one line. The colors have already been
-    selected, you can configure only the text without changing the colors. The string `process` are
-    always printed in upper case. The colors are shades of green and blue.
+    """Helper for printing multiple colors processing info in one line. The colors have already been selected, you can
+    configure only the text without changing the colors. The string `process` are always printed in upper case.
+    The colors are shades of green and blue.
 
     Example look: `[APPENDING 00001] image.png -> image_pixelart.png -> ran in 1.337 sec`
     """
 
     # Print multiple colors in one line.
     mprint("[", 50, "")
     mprint(str(process).upper(), 37, " ")
@@ -83,23 +78,23 @@
     mprint(" -> ", 197, "")
     mprint("ran in", 25, " ")
     mprint(str(time_taken), 26, " ")
     mprint("sec", 25)
 
 
 def print_cli_comp(
-    process: Literal["appending", "computing", "converting", "renaming"],
+    process: Literal["appending", "computing", "converting", "generating", "renaming", "resizing"],
     count: int,
     old: str,
     new: str,
     time_taken: float,
 ) -> None:
-    """Helper for printing multiple colors computing info in one line. The colors have already been
-    selected, you can configure only the text without changing the colors. The string `process` are
-    always printed in upper case. The colors are shades of red and green.
+    """Helper for printing multiple colors computing info in one line. The colors have already been selected, you can
+    configure only the text without changing the colors. The string `process` are always printed in upper case.
+    The colors are shades of red and green.
 
     Example look: `[COMPUTING 00001] image.png -> image_pixelart.png -> ran in 1.337 sec`
     """
 
     # Print multiple colors in one line.
     mprint("[", 203, "")
     mprint(str(process).upper(), 197, " ")
@@ -111,17 +106,16 @@
     mprint(" -> ", 197, "")
     mprint("ran in", 25, " ")
     mprint(str(time_taken), 26, " ")
     mprint("sec", 25)
 
 
 def print_cli_done(time_taken: float) -> None:
-    """Helper for printing multiple colors done info in one line. The colors and text have already
-    been selected, you can onfigure only the time taken without changing the colors. The colors are
-    shades of blue and red.
+    """Helper for printing multiple colors done info in one line. The colors and text have already been selected, you
+    can onfigure only the time taken without changing the colors. The colors are shades of blue and red.
 
     Configured look: `[DONE] Processing is finished -> ran in 1.337 sec`
     """
 
     # Print multiple colors in one line.
     mprint("[", 28, "")
     mprint("done".upper(), 40, "")
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/utils/stats.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/utils/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright © 2023 Marcin Różewski MDSANIMA
 
 
-"""This module provides various utilities that can be used for command-line tools.
-The module is intended for use in development.
+"""This module provides various utilities that can be used for command-line tools. The module is intended for use in
+development.
 """
 
 
 from __future__ import annotations
 
 import os
 
@@ -66,16 +66,16 @@
         "other": other,
     }
 
     return directory_statistic
 
 
 def get_images_count() -> dict:
-    """This function is intended for counting only the images in the current directory. Instead of
-    using a loop, we will use a Linux command for this and pipe it to another command.
+    """This function is intended for counting only the images in the current directory. Instead of using a loop, we will
+    use a Linux command for this and pipe it to another command.
     """
 
     # Linux terminal commands variable for counting.
     cmd_png = "ls -i *.png | wc -l"
     cmd_jpg = "ls -i *.jpg | wc -l"
     cmd_webp = "ls -i *.webp | wc -l"
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli/utils/timer.py` & `mdsanima_cli-0.2.1/src/mdsanima_cli/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/PKG-INFO` & `mdsanima_cli-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mdsanima-cli
-Version: 0.2.0
+Name: mdsanima_cli
+Version: 0.2.1
 Summary: The package will provide command-line tools for image processing, generating pixel art, adding logos to images, and much more.
 Author-email: Marcin Różewski <marcinrozewski@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -254,16 +254,16 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mdsanima-cli
 
-The package will provide command-line tools for image processing, generating pixel art, adding logos
-to images, and much more.
+The package will provide command-line tools for image processing, generating pixel art, adding logos to images, and much
+more.
 
 ## Installation
 
 Install latest version:
 
 ```shell
 python3 -m pip install mdsanima-cli
@@ -299,29 +299,29 @@
 - `mdsanima watermark` append a watermark
 - `mdsanima jpg` convert to jpg
 - `mdsanima png` convert to png
 - `mdsanima webp` convert to webp
 - `mdsanima pixelart` generate pixel art 32px
 - `mdsanima grid` generate grid 2x2
 - `mdsanima thumbnail` generate jpeg thumbnail 128px
+- `mdsanima gifmaker` generate gif animation pixel art
+- `mdsanima resize` resizing to 512px width
 
-The `pixelart` command works in folder that have only `.png` images and convert this images to pixel
-art with creating the new file and appending the suffix `pixelart` to original file name.
+The `pixelart` command works in folder that have only `.png` images and convert this images to pixel art with creating
+the new file and appending the suffix `pixelart` to original file name.
 
-After executing this command, all image files in the folder you are in will be processed.
-The command does not delete any files in the folder, it only adds new ones and showing the directory
-info.
+After executing this command, all image files in the folder you are in will be processed. The command does not delete
+any files in the folder, it only adds new ones and showing the directory info.
 
 ## Development Setup
 
 Instruction step how to setup development environent is here on this
 [workflow](https://mdsanima-dev.github.io/mdsanima-dev/development/workflow/) instruction.
 
-Creating isolated environment with specific pip version then activate and install requirements, type
-in terminal:
+Creating isolated environment with specific pip version then activate and install requirements, type in terminal:
 
 ```shell
 virtualenv --setuptools 67.7.2 --wheel 0.40.0 --pip 23.1.2 .venv
 source .venv/bin/activate
 pip install -r requirements.txt
 pip install -r requirements-dev.txt
 ```
@@ -360,22 +360,21 @@
 
 ```shell
 python3 src/mdsanima_cli/command/pixelart.py
 ```
 
 ### Extracts Version Package
 
-This `setuptools-scm` tools allow to extract **Python** package version from `git` instead declaring
-them as the version argument.
+This `setuptools-scm` tools allow to extract **Python** package version from `git` instead declaring them as the version
+argument.
 
-Check the `pyproject.toml` file and this
-[instruction](https://pypi.org/project/setuptools-scm/) for more info.
+Check the `pyproject.toml` file and this [instruction](https://pypi.org/project/setuptools-scm/) for more info.
 
-If you need to confirm which version string is being generated or debug the configuration, you can
-install `setuptools-scm` directly in your working environment `pip install setuptools-scm` and run:
+If you need to confirm which version string is being generated or debug the configuration, you can install
+`setuptools-scm` directly in your working environment `pip install setuptools-scm` and run:
 
 ```shell
 python -m setuptools_scm
 ```
 
 ### Creating Release
 
@@ -392,49 +391,48 @@
 
 Important steps is commit the change like this, type in terminal:
 
 ```shell
 git commit -m "feat: generating pixel art command"
 ```
 
-Always use this format for commiting to git, becouse this allows to generate changelog from the
-commit message. Check the `package.json` file on `standard-version` section and types lists for
-fist string thats you can type in commit message.
+Always use this format for commiting to git, becouse this allows to generate changelog from the commit message. Check
+the `package.json` file on `standard-version` section and types lists for fist string thats you can type in commit
+message.
 
-The next step is bumping version on `package.json` file and generate `CHANGELOG.md` file with new
-release information, type in terminal:
+The next step is bumping version on `package.json` file and generate `CHANGELOG.md` file with new release information,
+type in terminal:
 
 ```shell
 standard-version
 ```
 
 Next is a add this changes to git, type in terminal:
 
 ```shell
 git commit -am "chore(release): 0.1.2"
 ```
 
-The version abowe is a from `standard-version` command and this is a only example version.
-The version must always be changed when a new version is released.
+The version abowe is a from `standard-version` command and this is a only example version. The version must always be
+changed when a new version is released.
 
 The next steps is a creating a tag and pushing the change to origin with tag, type in terminal:
 
 ```shell
 git tag 0.1.2
 git push origin && git push origin --tag
 ```
 
 Checking the extracts version, type in terminal:
 
 ```shell
 python -m setuptools_scm
 ```
 
-Finally create the build and update this build to
-[test.pypi.org](https://test.pypi.org/project/mdsanima-cli/) and
+Finally create the build and update this build to [test.pypi.org](https://test.pypi.org/project/mdsanima-cli/) and
 [pypi.org](https://pypi.org/project/mdsanima-cli/) but first you must check and then update.
 
 ```shell
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
```

### Comparing `mdsanima_cli-0.2.0/src/mdsanima_cli.egg-info/SOURCES.txt` & `mdsanima_cli-0.2.1/src/mdsanima_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 package.json
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 .github/CODEOWNERS
 .idea/commands.md
 .vscode/.gitkeep
+.vscode/settings.json
 img/logo.png
 img/watermark.png
 src/.gitkeep
 src/mdsanima_cli/__init__.py
 src/mdsanima_cli/__main__.py
 src/mdsanima_cli/_version.py
 src/mdsanima_cli/parser.py
@@ -23,20 +24,22 @@
 src/mdsanima_cli.egg-info/SOURCES.txt
 src/mdsanima_cli.egg-info/dependency_links.txt
 src/mdsanima_cli.egg-info/entry_points.txt
 src/mdsanima_cli.egg-info/requires.txt
 src/mdsanima_cli.egg-info/top_level.txt
 src/mdsanima_cli/command/__init__.py
 src/mdsanima_cli/command/check.py
+src/mdsanima_cli/command/gifmaker.py
 src/mdsanima_cli/command/grid.py
 src/mdsanima_cli/command/jpg.py
 src/mdsanima_cli/command/logo.py
 src/mdsanima_cli/command/number.py
 src/mdsanima_cli/command/pixelart.py
 src/mdsanima_cli/command/png.py
+src/mdsanima_cli/command/resize.py
 src/mdsanima_cli/command/thumbnail.py
 src/mdsanima_cli/command/uuids.py
 src/mdsanima_cli/command/watermark.py
 src/mdsanima_cli/command/webp.py
 src/mdsanima_cli/utils/__init__.py
 src/mdsanima_cli/utils/ascii.py
 src/mdsanima_cli/utils/exif.py
```

