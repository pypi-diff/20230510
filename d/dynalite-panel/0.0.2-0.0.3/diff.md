# Comparing `tmp/dynalite-panel-0.0.2.tar.gz` & `tmp/dynalite-panel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynalite-panel-0.0.2.tar", last modified: Mon Aug 22 15:46:41 2022, max compression
+gzip compressed data, was "dynalite-panel-0.0.3.tar", last modified: Wed May 10 12:06:07 2023, max compression
```

## Comparing `dynalite-panel-0.0.2.tar` & `dynalite-panel-0.0.3.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 15:46:41.946943 dynalite-panel-0.0.2/
--rw-rw-r--   0 root         (0) root         (0)    11357 2022-08-22 14:51:30.000000 dynalite-panel-0.0.2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       46 2022-08-22 14:51:30.000000 dynalite-panel-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      365 2022-08-22 15:46:41.946943 dynalite-panel-0.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       15 2022-08-22 14:51:30.000000 dynalite-panel-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 15:46:41.894943 dynalite-panel-0.0.2/dynalite_panel/
--rw-rw-r--   0 root         (0) root         (0)      277 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/constants.py
--rw-r--r--   0 root         (0) root         (0)      407 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/entrypoint-94572d1e.js
--rw-r--r--   0 root         (0) root         (0)      281 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/entrypoint-94572d1e.js.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 15:46:41.926943 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/
--rw-r--r--   0 root         (0) root         (0)    31191 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/0176177f.js
--rw-r--r--   0 root         (0) root         (0)     6481 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/0176177f.js.gz
--rw-r--r--   0 root         (0) root         (0)    32234 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/280bd5a8.js
--rw-r--r--   0 root         (0) root         (0)      149 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/280bd5a8.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7387 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/280bd5a8.js.gz
--rw-r--r--   0 root         (0) root         (0)    12448 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/28deee2e.js
--rw-r--r--   0 root         (0) root         (0)     3913 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/28deee2e.js.gz
--rw-r--r--   0 root         (0) root         (0)    39866 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/3934967e.js
--rw-r--r--   0 root         (0) root         (0)      149 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/3934967e.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     8724 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/3934967e.js.gz
--rw-r--r--   0 root         (0) root         (0)    47936 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/544a6346.js
--rw-r--r--   0 root         (0) root         (0)     1933 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/544a6346.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    11201 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/544a6346.js.gz
--rw-r--r--   0 root         (0) root         (0)   207337 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/549f5f17.js
--rw-r--r--   0 root         (0) root         (0)     1498 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/549f5f17.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    34974 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/549f5f17.js.gz
--rw-r--r--   0 root         (0) root         (0)     6587 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/59e04dd8.js
--rw-r--r--   0 root         (0) root         (0)     2119 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/59e04dd8.js.gz
--rw-r--r--   0 root         (0) root         (0)    43014 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/6914a402.js
--rw-r--r--   0 root         (0) root         (0)      416 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/6914a402.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     9735 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/6914a402.js.gz
--rw-r--r--   0 root         (0) root         (0)   208591 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/7cba2f88.js
--rw-r--r--   0 root         (0) root         (0)     3180 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/7cba2f88.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    36185 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/7cba2f88.js.gz
--rw-r--r--   0 root         (0) root         (0)    19637 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8081cb55.js
--rw-r--r--   0 root         (0) root         (0)     5944 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8081cb55.js.gz
--rw-r--r--   0 root         (0) root         (0)    13429 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/811ccb02.js
--rw-r--r--   0 root         (0) root         (0)     4047 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/811ccb02.js.gz
--rw-r--r--   0 root         (0) root         (0)    20851 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8ddbc98a.js
--rw-r--r--   0 root         (0) root         (0)      149 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8ddbc98a.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     6499 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8ddbc98a.js.gz
--rw-r--r--   0 root         (0) root         (0)   138764 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/9096b401.js
--rw-r--r--   0 root         (0) root         (0)      149 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/9096b401.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    19708 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/9096b401.js.gz
--rw-r--r--   0 root         (0) root         (0)     9822 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/a0807cba.js
--rw-r--r--   0 root         (0) root         (0)     3460 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/a0807cba.js.gz
--rw-r--r--   0 root         (0) root         (0)    52108 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/b01dfb96.js
--rw-r--r--   0 root         (0) root         (0)      149 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/b01dfb96.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     8122 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/b01dfb96.js.gz
--rw-r--r--   0 root         (0) root         (0)   106997 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/cd7b8f7d.js
--rw-r--r--   0 root         (0) root         (0)      149 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/cd7b8f7d.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    14795 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/cd7b8f7d.js.gz
--rw-r--r--   0 root         (0) root         (0)     3144 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/e720b3fd.js
--rw-r--r--   0 root         (0) root         (0)     1474 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/e720b3fd.js.gz
--rw-r--r--   0 root         (0) root         (0)  2455993 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js
--rw-r--r--   0 root         (0) root         (0)     4845 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   437239 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js.gz
--rw-r--r--   0 root         (0) root         (0)    35472 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f20b187d.js
--rw-r--r--   0 root         (0) root         (0)      240 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f20b187d.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     7764 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f20b187d.js.gz
--rw-r--r--   0 root         (0) root         (0)     8898 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f7fc5e73.js
--rw-r--r--   0 root         (0) root         (0)      811 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f7fc5e73.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2829 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f7fc5e73.js.gz
--rw-r--r--   0 root         (0) root         (0)     3144 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f879cd62.js
--rw-r--r--   0 root         (0) root         (0)     1474 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f879cd62.js.gz
--rw-r--r--   0 root         (0) root         (0)       77 2022-08-22 15:44:05.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_es5/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 15:46:41.946943 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/
--rw-r--r--   0 root         (0) root         (0)    41489 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/29a9f7c8.js
--rw-r--r--   0 root         (0) root         (0)     1933 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/29a9f7c8.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     9634 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/29a9f7c8.js.gz
--rw-r--r--   0 root         (0) root         (0)    15645 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/29a9f7c8.js.map
--rw-r--r--   0 root         (0) root         (0)    19235 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/3e82c6b4.js
--rw-r--r--   0 root         (0) root         (0)     5056 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/3e82c6b4.js.gz
--rw-r--r--   0 root         (0) root         (0)     5090 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/3e82c6b4.js.map
--rw-r--r--   0 root         (0) root         (0)    28068 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/46cae3ee.js
--rw-r--r--   0 root         (0) root         (0)      266 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/46cae3ee.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     5788 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/46cae3ee.js.gz
--rw-r--r--   0 root         (0) root         (0)    13751 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/46cae3ee.js.map
--rw-r--r--   0 root         (0) root         (0)     3844 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/4dbe2863.js
--rw-r--r--   0 root         (0) root         (0)     1643 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/4dbe2863.js.gz
--rw-r--r--   0 root         (0) root         (0)    98487 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/643b760f.js
--rw-r--r--   0 root         (0) root         (0)    12232 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/643b760f.js.gz
--rw-r--r--   0 root         (0) root         (0)    54878 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/643b760f.js.map
--rw-r--r--   0 root         (0) root         (0)   143037 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/649f060e.js
--rw-r--r--   0 root         (0) root         (0)     3030 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/649f060e.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    27072 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/649f060e.js.gz
--rw-r--r--   0 root         (0) root         (0)    82004 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/649f060e.js.map
--rw-r--r--   0 root         (0) root         (0)    26006 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/6502cf65.js
--rw-r--r--   0 root         (0) root         (0)     5455 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/6502cf65.js.gz
--rw-r--r--   0 root         (0) root         (0)    16922 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/6502cf65.js.map
--rw-r--r--   0 root         (0) root         (0)    16735 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/7717c19d.js
--rw-r--r--   0 root         (0) root         (0)     5049 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/7717c19d.js.gz
--rw-r--r--   0 root         (0) root         (0)    13502 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/7717c19d.js.map
--rw-r--r--   0 root         (0) root         (0)     3844 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/87a36f14.js
--rw-r--r--   0 root         (0) root         (0)     1643 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/87a36f14.js.gz
--rw-r--r--   0 root         (0) root         (0)    74230 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/9e0116ac.js
--rw-r--r--   0 root         (0) root         (0)     8461 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/9e0116ac.js.gz
--rw-r--r--   0 root         (0) root         (0)    24755 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/9e0116ac.js.map
--rw-r--r--   0 root         (0) root         (0)     8909 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a4ced4db.js
--rw-r--r--   0 root         (0) root         (0)      811 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a4ced4db.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2840 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a4ced4db.js.gz
--rw-r--r--   0 root         (0) root         (0)   143025 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a6a2535a.js
--rw-r--r--   0 root         (0) root         (0)      539 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a6a2535a.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    24077 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a6a2535a.js.gz
--rw-r--r--   0 root         (0) root         (0)    40960 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a6a2535a.js.map
--rw-r--r--   0 root         (0) root         (0)     6329 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/cda223e0.js
--rw-r--r--   0 root         (0) root         (0)     2064 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/cda223e0.js.gz
--rw-r--r--   0 root         (0) root         (0)    22811 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/ce0043e4.js
--rw-r--r--   0 root         (0) root         (0)     4680 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/ce0043e4.js.gz
--rw-r--r--   0 root         (0) root         (0)     9256 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/ce0043e4.js.map
--rw-r--r--   0 root         (0) root         (0)    20779 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/d5e406e6.js
--rw-r--r--   0 root         (0) root         (0)     4376 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/d5e406e6.js.gz
--rw-r--r--   0 root         (0) root         (0)     5941 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/d5e406e6.js.map
--rw-r--r--   0 root         (0) root         (0)    27269 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e65326f9.js
--rw-r--r--   0 root         (0) root         (0)     4160 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e65326f9.js.gz
--rw-r--r--   0 root         (0) root         (0)     6367 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e65326f9.js.map
--rw-r--r--   0 root         (0) root         (0)    14038 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e7b29574.js
--rw-r--r--   0 root         (0) root         (0)       90 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e7b29574.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3520 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e7b29574.js.gz
--rw-r--r--   0 root         (0) root         (0)   339554 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/entrypoint-94572d1e.js
--rw-r--r--   0 root         (0) root         (0)     5695 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    71327 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.gz
--rw-r--r--   0 root         (0) root         (0)    81963 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.map
--rw-r--r--   0 root         (0) root         (0)    10229 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3b7e75a.js
--rw-r--r--   0 root         (0) root         (0)     3282 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3b7e75a.js.gz
--rw-r--r--   0 root         (0) root         (0)     4640 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3b7e75a.js.map
--rw-r--r--   0 root         (0) root         (0)    20094 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3dea0e7.js
--rw-r--r--   0 root         (0) root         (0)     3946 2022-08-22 15:43:39.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3dea0e7.js.gz
--rw-r--r--   0 root         (0) root         (0)     5581 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3dea0e7.js.map
--rw-r--r--   0 root         (0) root         (0)       80 2022-08-22 15:43:41.000000 dynalite-panel-0.0.2/dynalite_panel/frontend_latest/manifest.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-22 15:46:41.894943 dynalite-panel-0.0.2/dynalite_panel.egg-info/
--rw-r--r--   0 root         (0) root         (0)      365 2022-08-22 15:46:40.000000 dynalite-panel-0.0.2/dynalite_panel.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5830 2022-08-22 15:46:41.000000 dynalite-panel-0.0.2/dynalite_panel.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-22 15:46:40.000000 dynalite-panel-0.0.2/dynalite_panel.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-22 15:27:48.000000 dynalite-panel-0.0.2/dynalite_panel.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2022-08-22 15:46:41.000000 dynalite-panel-0.0.2/dynalite_panel.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      715 2022-08-22 15:42:40.000000 dynalite-panel-0.0.2/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2022-08-22 15:46:41.946943 dynalite-panel-0.0.2/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 12:06:07.456204 dynalite-panel-0.0.3/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    11357 2023-05-10 11:22:49.000000 dynalite-panel-0.0.3/LICENSE
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       46 2023-05-10 11:22:49.000000 dynalite-panel-0.0.3/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      365 2023-05-10 12:06:07.456204 dynalite-panel-0.0.3/PKG-INFO
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       15 2023-05-10 11:22:49.000000 dynalite-panel-0.0.3/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 12:06:07.412204 dynalite-panel-0.0.3/dynalite_panel/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      277 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       35 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/constants.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      407 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/entrypoint-94572d1e.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      281 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/entrypoint-94572d1e.js.gz
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 12:06:07.436204 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    31191 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/0176177f.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6481 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/0176177f.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32234 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/280bd5a8.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/280bd5a8.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7387 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/280bd5a8.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12448 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/28deee2e.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3913 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/28deee2e.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    39866 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/3934967e.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/3934967e.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8724 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/3934967e.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    47936 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/544a6346.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1933 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/544a6346.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11201 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/544a6346.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   207337 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/549f5f17.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1498 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/549f5f17.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    34974 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/549f5f17.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6587 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/59e04dd8.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2119 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/59e04dd8.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    43014 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/6914a402.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      416 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/6914a402.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9735 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/6914a402.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   208591 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/7cba2f88.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3180 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/7cba2f88.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    36185 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/7cba2f88.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19637 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8081cb55.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5944 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8081cb55.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13429 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/811ccb02.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4047 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/811ccb02.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    20851 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8ddbc98a.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8ddbc98a.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6499 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8ddbc98a.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   138764 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/9096b401.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/9096b401.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19708 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/9096b401.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9822 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/a0807cba.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3460 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/a0807cba.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    52108 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/b01dfb96.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/b01dfb96.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8122 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/b01dfb96.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   106997 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/cd7b8f7d.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      149 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/cd7b8f7d.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14795 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/cd7b8f7d.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3144 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/e720b3fd.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1474 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/e720b3fd.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)  2455993 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4845 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   437239 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    35472 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f20b187d.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      240 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f20b187d.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7764 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f20b187d.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8898 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f7fc5e73.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      811 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f7fc5e73.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2829 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f7fc5e73.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3144 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f879cd62.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1474 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f879cd62.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       77 2023-05-10 12:03:08.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_es5/manifest.json
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 12:06:07.456204 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    41489 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/29a9f7c8.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1933 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/29a9f7c8.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9634 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/29a9f7c8.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15645 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/29a9f7c8.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19235 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/3e82c6b4.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5056 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/3e82c6b4.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5090 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/3e82c6b4.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    28068 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/46cae3ee.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      266 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/46cae3ee.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5788 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/46cae3ee.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13751 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/46cae3ee.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3844 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/4dbe2863.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1643 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/4dbe2863.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    98487 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/643b760f.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12232 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/643b760f.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    54878 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/643b760f.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   143037 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/649f060e.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3030 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/649f060e.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    27072 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/649f060e.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    82004 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/649f060e.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26006 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/6502cf65.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5455 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/6502cf65.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16922 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/6502cf65.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16735 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/7717c19d.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5049 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/7717c19d.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13502 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/7717c19d.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3844 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/87a36f14.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1643 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/87a36f14.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    74230 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/9e0116ac.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8461 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/9e0116ac.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24755 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/9e0116ac.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8909 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a4ced4db.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      811 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a4ced4db.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2840 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a4ced4db.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   143025 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a6a2535a.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      539 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a6a2535a.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24077 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a6a2535a.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    40960 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a6a2535a.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6329 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/cda223e0.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2064 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/cda223e0.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22811 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/ce0043e4.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4680 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/ce0043e4.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9256 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/ce0043e4.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    20779 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/d5e406e6.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4376 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/d5e406e6.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5941 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/d5e406e6.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    27269 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e65326f9.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4160 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e65326f9.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6367 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e65326f9.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14038 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e7b29574.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       90 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e7b29574.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3520 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e7b29574.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   339554 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/entrypoint-94572d1e.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5695 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.LICENSE.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    71327 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    81963 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10229 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3b7e75a.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3282 2023-05-10 12:02:40.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3b7e75a.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4640 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3b7e75a.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    20094 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3dea0e7.js
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3946 2023-05-10 12:02:41.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3dea0e7.js.gz
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5581 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3dea0e7.js.map
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       80 2023-05-10 12:02:43.000000 dynalite-panel-0.0.3/dynalite_panel/frontend_latest/manifest.json
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-10 12:06:07.416204 dynalite-panel-0.0.3/dynalite_panel.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      365 2023-05-10 12:06:06.000000 dynalite-panel-0.0.3/dynalite_panel.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5830 2023-05-10 12:06:07.000000 dynalite-panel-0.0.3/dynalite_panel.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-10 12:06:06.000000 dynalite-panel-0.0.3/dynalite_panel.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-10 11:53:00.000000 dynalite-panel-0.0.3/dynalite_panel.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-10 12:06:07.000000 dynalite-panel-0.0.3/dynalite_panel.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      715 2023-05-10 12:01:37.000000 dynalite-panel-0.0.3/pyproject.toml
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       38 2023-05-10 12:06:07.460204 dynalite-panel-0.0.3/setup.cfg
```

### Comparing `dynalite-panel-0.0.2/LICENSE` & `dynalite-panel-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/0176177f.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/0176177f.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/0176177f.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/0176177f.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/280bd5a8.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/280bd5a8.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/280bd5a8.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/280bd5a8.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/28deee2e.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/28deee2e.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/28deee2e.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/28deee2e.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/3934967e.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/3934967e.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/3934967e.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/3934967e.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/544a6346.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/544a6346.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/544a6346.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/544a6346.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/544a6346.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/544a6346.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/549f5f17.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/549f5f17.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/549f5f17.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/549f5f17.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/549f5f17.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/549f5f17.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/59e04dd8.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/59e04dd8.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/59e04dd8.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/59e04dd8.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/6914a402.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/6914a402.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/6914a402.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/6914a402.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/7cba2f88.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/7cba2f88.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/7cba2f88.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/7cba2f88.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/7cba2f88.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/7cba2f88.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8081cb55.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8081cb55.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8081cb55.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8081cb55.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/811ccb02.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/811ccb02.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/811ccb02.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/811ccb02.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8ddbc98a.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8ddbc98a.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/8ddbc98a.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/8ddbc98a.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/9096b401.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/9096b401.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/9096b401.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/9096b401.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/a0807cba.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/a0807cba.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/a0807cba.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/a0807cba.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/b01dfb96.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/b01dfb96.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/b01dfb96.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/b01dfb96.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/cd7b8f7d.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/cd7b8f7d.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/cd7b8f7d.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/cd7b8f7d.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/e720b3fd.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/e720b3fd.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/e720b3fd.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/e720b3fd.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/entrypoint-e859e4b8.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f20b187d.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f20b187d.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f20b187d.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f20b187d.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f7fc5e73.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f7fc5e73.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f7fc5e73.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f7fc5e73.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f7fc5e73.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f7fc5e73.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f879cd62.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f879cd62.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_es5/f879cd62.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_es5/f879cd62.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/29a9f7c8.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/29a9f7c8.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/29a9f7c8.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/29a9f7c8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/29a9f7c8.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/29a9f7c8.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/29a9f7c8.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/29a9f7c8.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/3e82c6b4.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/3e82c6b4.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/3e82c6b4.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/3e82c6b4.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/3e82c6b4.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/3e82c6b4.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/46cae3ee.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/46cae3ee.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/46cae3ee.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/46cae3ee.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/46cae3ee.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/46cae3ee.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/4dbe2863.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/4dbe2863.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/4dbe2863.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/4dbe2863.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/643b760f.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/643b760f.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/643b760f.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/643b760f.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/643b760f.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/643b760f.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/649f060e.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/649f060e.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/649f060e.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/649f060e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/649f060e.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/649f060e.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/649f060e.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/649f060e.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/6502cf65.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/6502cf65.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/6502cf65.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/6502cf65.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/6502cf65.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/6502cf65.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/7717c19d.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/7717c19d.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/7717c19d.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/7717c19d.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/7717c19d.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/7717c19d.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/87a36f14.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/87a36f14.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/87a36f14.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/87a36f14.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/9e0116ac.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/9e0116ac.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/9e0116ac.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/9e0116ac.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/9e0116ac.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/9e0116ac.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a4ced4db.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a4ced4db.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a4ced4db.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a4ced4db.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a4ced4db.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a4ced4db.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a6a2535a.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a6a2535a.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a6a2535a.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a6a2535a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a6a2535a.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a6a2535a.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/a6a2535a.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/a6a2535a.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/cda223e0.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/cda223e0.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/cda223e0.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/cda223e0.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/ce0043e4.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/ce0043e4.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/ce0043e4.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/ce0043e4.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/ce0043e4.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/ce0043e4.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/d5e406e6.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/d5e406e6.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/d5e406e6.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/d5e406e6.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/d5e406e6.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/d5e406e6.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e65326f9.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e65326f9.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e65326f9.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e65326f9.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e65326f9.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e65326f9.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e7b29574.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e7b29574.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/e7b29574.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/e7b29574.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/entrypoint-94572d1e.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/entrypoint-94572d1e.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.LICENSE.txt` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/entrypoint-94572d1e.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3b7e75a.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3b7e75a.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3b7e75a.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3b7e75a.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3b7e75a.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3b7e75a.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3dea0e7.js` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3dea0e7.js`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3dea0e7.js.gz` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3dea0e7.js.gz`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel/frontend_latest/f3dea0e7.js.map` & `dynalite-panel-0.0.3/dynalite_panel/frontend_latest/f3dea0e7.js.map`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/dynalite_panel.egg-info/SOURCES.txt` & `dynalite-panel-0.0.3/dynalite_panel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynalite-panel-0.0.2/pyproject.toml` & `dynalite-panel-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "dynalite-panel"
-version      = "0.0.2"
+version      = "0.0.3"
 license      = {text = "Apache-2.0"}
 description  = "Dynalite panel for Home Assistant"
 readme       = "README.md"
 authors      = [
     {name = "Ziv", email = "16467659+ziv1234@users.noreply.github.com"}
 ]
 requires-python = ">=3.4.0"
```

