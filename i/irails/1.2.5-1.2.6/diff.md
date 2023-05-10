# Comparing `tmp/irails-1.2.5.tar.gz` & `tmp/irails-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.2.5.tar", last modified: Wed May 10 10:46:25 2023, max compression
+gzip compressed data, was "irails-1.2.6.tar", last modified: Wed May 10 11:40:37 2023, max compression
```

## Comparing `irails-1.2.5.tar` & `irails-1.2.6.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.452435 irails-1.2.5/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5079 2023-05-10 10:46:25.451438 irails-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.386869 irails-1.2.5/irails/
--rw-rw-rw-   0        0        0      331 2023-05-10 10:46:13.000000 irails-1.2.5/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.5/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.5/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.5/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.5/irails/auth.py
--rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.5/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.397623 irails-1.2.5/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.400616 irails-1.2.5/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.5/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.5/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.5/irails/cbv.py
--rw-rw-rw-   0        0        0     7260 2023-05-10 10:03:41.000000 irails-1.2.5/irails/config.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.5/irails/controller_utils.py
--rw-rw-rw-   0        0        0    32113 2023-05-10 07:54:46.000000 irails-1.2.5/irails/core.py
--rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.5/irails/database.py
--rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.5/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.5/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.5/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.5/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.408575 irails-1.2.5/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.5/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.5/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.5/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.5/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.5/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1319 2023-05-10 10:05:39.000000 irails-1.2.5/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.5/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.351611 irails-1.2.5/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.418551 irails-1.2.5/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.5/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.5/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.5/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.5/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.5/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.5/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.5/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.5/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.420518 irails-1.2.5/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.5/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.421518 irails-1.2.5/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.5/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.432504 irails-1.2.5/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.5/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.5/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.5/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.5/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.5/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.2.5/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      656 2023-05-10 10:04:49.000000 irails-1.2.5/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.5/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.5/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.354601 irails-1.2.5/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.436478 irails-1.2.5/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.2.5/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.2.5/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.2.5/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.2.5/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.437476 irails-1.2.5/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.5/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.5/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.440467 irails-1.2.5/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.356596 irails-1.2.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.442462 irails-1.2.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.446452 irails-1.2.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.357593 irails-1.2.5/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.449455 irails-1.2.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.5/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:46:25.393621 irails-1.2.5/irails.egg-info/
--rw-rw-rw-   0        0        0     5079 2023-05-10 10:46:25.000000 irails-1.2.5/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2287 2023-05-10 10:46:25.000000 irails-1.2.5/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:46:25.000000 irails-1.2.5/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-10 10:46:25.000000 irails-1.2.5/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      766 2023-05-10 10:46:25.000000 irails-1.2.5/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 10:46:25.000000 irails-1.2.5/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 10:46:25.452435 irails-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.949333 irails-1.2.6/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5079 2023-05-10 11:40:37.948292 irails-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.872271 irails-1.2.6/irails/
+-rw-rw-rw-   0        0        0      331 2023-05-10 11:40:23.000000 irails-1.2.6/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.6/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.6/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.6/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.6/irails/auth.py
+-rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.6/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.884238 irails-1.2.6/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.885237 irails-1.2.6/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.6/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.6/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.6/irails/cbv.py
+-rw-rw-rw-   0        0        0     7328 2023-05-10 11:08:55.000000 irails-1.2.6/irails/config.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.6/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    32113 2023-05-10 07:54:46.000000 irails-1.2.6/irails/core.py
+-rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.6/irails/database.py
+-rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.6/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.6/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.6/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.6/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.894212 irails-1.2.6/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.6/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.6/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.6/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.6/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.6/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1423 2023-05-10 10:55:35.000000 irails-1.2.6/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.6/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.840045 irails-1.2.6/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.902190 irails-1.2.6/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.6/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.6/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.6/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.6/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.6/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.6/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.6/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.6/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.905186 irails-1.2.6/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.6/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.907178 irails-1.2.6/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.6/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.922138 irails-1.2.6/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.6/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.6/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.6/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.6/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.6/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.2.6/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      656 2023-05-10 11:09:34.000000 irails-1.2.6/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.6/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.6/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.844036 irails-1.2.6/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.929119 irails-1.2.6/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.2.6/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.2.6/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.2.6/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      307 2023-05-10 11:40:05.000000 irails-1.2.6/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.931994 irails-1.2.6/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.6/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.6/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.934131 irails-1.2.6/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.847030 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.938123 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.944130 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.848024 irails-1.2.6/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.946102 irails-1.2.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.6/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:40:37.881247 irails-1.2.6/irails.egg-info/
+-rw-rw-rw-   0        0        0     5079 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2287 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      766 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 11:40:37.000000 irails-1.2.6/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 11:40:37.949333 irails-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.6/setup.py
```

### Comparing `irails-1.2.5/PKG-INFO` & `irails-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.5
+Version: 1.2.6
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: irails Version: 1.2.5 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.2.6 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.2.5/README.md` & `irails-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/_i18n.py` & `irails-1.2.6/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/_loader.py` & `irails-1.2.6/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/_utils.py` & `irails-1.2.6/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/auth.py` & `irails-1.2.6/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/base_controller.py` & `irails-1.2.6/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.2.6/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.2.6/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/cbv.py` & `irails-1.2.6/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/config.py` & `irails-1.2.6/irails/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,22 +145,22 @@
                         sub_value = segment_config
                         for sub_key in sub_keys:
                             sub_value = sub_value.get(sub_key, {})
                         value = value.replace("{" + name + "}", str(sub_value))
             else:
                 value = value.replace("{" + name + "}", self.config.get(name, ""))
         return value
+config = YamlConfig(os.path.join(ROOT_PATH,"configs") )
+
 debug = False
-def __init_log(__logCfg):
-    if not __logCfg:
-        return None
-    from fastapi.logger import logger
+def set_logger(logger:logging.Logger):
+    __logCfg = config.get("log")
     __log_level = __logCfg['level'] or 'DEBUG'
     __log_file = __logCfg['file'] or None 
-    debug = config.get("debug") or False
+    debug = config.get("debug",False)   
     logger.name = __logCfg.get("name",'iRails')
     if __log_file:
         __log_file = os.path.abspath(__log_file)
     log_format="%(asctime)s %(name)s:%(levelname)s:%(message)s"
     datefmt="%Y-%M-%d %H:%M:%S" 
     if __log_file:
         if debug:
@@ -176,24 +176,30 @@
         import sys
         handler = logging.StreamHandler(sys.stdout)  
     handler.setLevel(logging._nameToLevel[__log_level]) 
     handler.setFormatter(logging.Formatter(fmt= log_format,datefmt=datefmt)) 
     logger.addHandler(handler)
     
     logger.setLevel(logging._nameToLevel[__log_level]) 
+
+def __init_log( ):
+    __logCfg = config.get("log")
+    logger = logging.getLogger(__logCfg.get('name','IRAILS'))
+    # from fastapi.logger import logger
+    set_logger(logger)
     return logger
-    # return logging.getLogger(__logCfg['name'] or 'FastapiMvcFramework')
+     
+
 
-config = YamlConfig(os.path.join(ROOT_PATH,"configs") )
 
 #test:
 # dbcfg = config.get('database')
 # uri = dbcfg.get("uri")
 # assert uri
 # errors = config.get("errors")
 # p404 = errors.get("error_404_page")
 # assert p404
 
-_log = __init_log(config.get("log"))
+_log = __init_log()
 if _log:
     _log.setLevel(logging.DEBUG)
```

### Comparing `irails-1.2.5/irails/controller_utils.py` & `irails-1.2.6/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/core.py` & `irails-1.2.6/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/database.py` & `irails-1.2.6/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/midware.py` & `irails-1.2.6/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/midware_casbin.py` & `irails-1.2.6/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/midware_session.py` & `irails-1.2.6/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/mvc_router.py` & `irails-1.2.6/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/_app.py` & `irails-1.2.6/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/_controller.py` & `irails-1.2.6/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/_i18n.py` & `irails-1.2.6/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/_project.py` & `irails-1.2.6/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/_run.py` & `irails-1.2.6/irails/scripts/_run.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,11 +29,13 @@
         kwargs['reload_dirs'] = apps_dirs
         kwargs['reload_includes'] = ['*.po']
     # module_path = 'main.py'
     # spec = importlib.util.spec_from_file_location(module_path, module_path)
     # module = importlib.util.module_from_spec(spec)
     # spec.loader.exec_module(module)
     
-    
+    from uvicorn.main import logger
+    from irails.config import set_logger
+    set_logger(logger=logger)
 
     uvicorn.run(app="irails.core:generate_mvc_app",**kwargs)
```

### Comparing `irails-1.2.5/irails/scripts/main.py` & `irails-1.2.6/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/app/home.css.tpl` & `irails-1.2.6/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/app/home.tpl` & `irails-1.2.6/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.2.6/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.2.6/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.2.6/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.2.6/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/public/error_404.html` & `irails-1.2.6/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/public/error_500.html` & `irails-1.2.6/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.2.6/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.2.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.2.6/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.2.6/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails/view.py` & `irails-1.2.6/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails.egg-info/PKG-INFO` & `irails-1.2.6/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.5
+Version: 1.2.6
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: irails Version: 1.2.5 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.2.6 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.2.5/irails.egg-info/SOURCES.txt` & `irails-1.2.6/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/irails.egg-info/requires.txt` & `irails-1.2.6/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.5/setup.py` & `irails-1.2.6/setup.py`

 * *Files identical despite different names*

