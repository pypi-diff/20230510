# Comparing `tmp/irails-1.2.2.tar.gz` & `tmp/irails-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.2.2.tar", last modified: Tue May  9 15:26:05 2023, max compression
+gzip compressed data, was "irails-1.2.4.tar", last modified: Wed May 10 09:54:28 2023, max compression
```

## Comparing `irails-1.2.2.tar` & `irails-1.2.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.319811 irails-1.2.2/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5079 2023-05-09 15:26:05.318814 irails-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.261651 irails-1.2.2/irails/
--rw-rw-rw-   0        0        0      334 2023-05-09 15:25:50.000000 irails-1.2.2/irails/__init__.py
--rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.2/irails/_i18n.py
--rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.2/irails/_loader.py
--rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.2/irails/_utils.py
--rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.2/irails/auth.py
--rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.2/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.271694 irails-1.2.2/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.272692 irails-1.2.2/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.2/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.2/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.2/irails/cbv.py
--rw-rw-rw-   0        0        0     7252 2023-05-09 06:43:06.000000 irails-1.2.2/irails/config.py
--rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.2/irails/controller_utils.py
--rw-rw-rw-   0        0        0    30828 2023-05-08 14:26:29.000000 irails-1.2.2/irails/core.py
--rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.2/irails/database.py
--rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.2/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.2/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.2/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.2/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.279923 irails-1.2.2/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.2/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.2/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.2/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.2/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.2/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1321 2023-05-04 04:28:43.000000 irails-1.2.2/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.2/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.233710 irails-1.2.2/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.288894 irails-1.2.2/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.2/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.2/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.2/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.2/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.2/irails/scripts/tpls/app/model.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.2/irails/scripts/tpls/app/service.tpl
--rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.2/irails/scripts/tpls/app/test.tpl
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.2/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.290888 irails-1.2.2/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.2/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.291885 irails-1.2.2/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.2/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.302856 irails-1.2.2/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.2/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.2/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.2/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.2/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.2/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      835 2023-04-30 12:07:18.000000 irails-1.2.2/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      665 2023-05-09 06:45:32.000000 irails-1.2.2/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.2/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.2/irails/scripts/tpls/project/configs/upload.yaml
--rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.2.2/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.304851 irails-1.2.2/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.2/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.2/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.307843 irails-1.2.2/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.237700 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.310836 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.314825 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.238698 irails-1.2.2/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.316819 irails-1.2.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.2/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-09 15:26:05.269615 irails-1.2.2/irails.egg-info/
--rw-rw-rw-   0        0        0     5079 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2135 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      766 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-09 15:26:05.000000 irails-1.2.2/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 15:26:05.319811 irails-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.127858 irails-1.2.4/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5079 2023-05-10 09:54:28.126437 irails-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4296 2023-05-09 11:36:53.000000 irails-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.061711 irails-1.2.4/irails/
+-rw-rw-rw-   0        0        0      331 2023-05-10 09:54:12.000000 irails-1.2.4/irails/__init__.py
+-rw-rw-rw-   0        0        0     3402 2023-05-07 08:38:04.000000 irails-1.2.4/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2205 2023-05-06 12:00:36.000000 irails-1.2.4/irails/_loader.py
+-rw-rw-rw-   0        0        0     2390 2023-04-27 14:23:55.000000 irails-1.2.4/irails/_utils.py
+-rw-rw-rw-   0        0        0    11704 2023-05-06 06:47:02.000000 irails-1.2.4/irails/auth.py
+-rw-rw-rw-   0        0        0    11570 2023-05-07 08:42:59.000000 irails-1.2.4/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.072685 irails-1.2.4/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.073679 irails-1.2.4/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.2.4/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10407 2023-04-30 14:28:38.000000 irails-1.2.4/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.2.4/irails/cbv.py
+-rw-rw-rw-   0        0        0     7256 2023-05-10 07:52:10.000000 irails-1.2.4/irails/config.py
+-rw-rw-rw-   0        0        0    12261 2023-05-03 14:53:53.000000 irails-1.2.4/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    32113 2023-05-10 07:54:46.000000 irails-1.2.4/irails/core.py
+-rw-rw-rw-   0        0        0     6285 2023-05-08 14:12:16.000000 irails-1.2.4/irails/database.py
+-rw-rw-rw-   0        0        0     8655 2023-05-09 06:39:34.000000 irails-1.2.4/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.2.4/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9344 2023-04-10 14:09:32.000000 irails-1.2.4/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.2.4/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.079663 irails-1.2.4/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.2.4/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7803 2023-05-09 15:18:47.000000 irails-1.2.4/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     7690 2023-05-09 06:52:08.000000 irails-1.2.4/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     6836 2023-05-07 08:08:21.000000 irails-1.2.4/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.2.4/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1345 2023-05-10 09:52:45.000000 irails-1.2.4/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     1805 2023-05-05 05:41:01.000000 irails-1.2.4/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.035150 irails-1.2.4/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.091632 irails-1.2.4/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.2.4/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.2.4/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.2.4/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.2.4/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:26.000000 irails-1.2.4/irails/scripts/tpls/app/model.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 11:52:38.000000 irails-1.2.4/irails/scripts/tpls/app/service.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-25 12:03:35.000000 irails-1.2.4/irails/scripts/tpls/app/test.tpl
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.2.4/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.093626 irails-1.2.4/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.2.4/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.094623 irails-1.2.4/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.2.4/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.108489 irails-1.2.4/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.2.4/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      198 2023-05-09 06:44:21.000000 irails-1.2.4/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.2.4/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.2.4/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.2.4/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      835 2023-04-30 12:07:18.000000 irails-1.2.4/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      665 2023-05-09 06:45:32.000000 irails-1.2.4/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.2.4/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.2.4/irails/scripts/tpls/project/configs/upload.yaml
+-rw-rw-rw-   0        0        0      144 2023-04-30 09:03:04.000000 irails-1.2.4/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.110479 irails-1.2.4/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.2.4/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.2.4/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.112475 irails-1.2.4/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.039126 irails-1.2.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.117463 irails-1.2.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.2.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.122447 irails-1.2.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.2.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.2.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.2.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.040125 irails-1.2.4/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.124453 irails-1.2.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.2.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     2660 2023-05-05 14:37:24.000000 irails-1.2.4/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-10 09:54:28.069690 irails-1.2.4/irails.egg-info/
+-rw-rw-rw-   0        0        0     5079 2023-05-10 09:54:27.000000 irails-1.2.4/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2135 2023-05-10 09:54:27.000000 irails-1.2.4/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 09:54:27.000000 irails-1.2.4/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-10 09:54:27.000000 irails-1.2.4/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      766 2023-05-10 09:54:27.000000 irails-1.2.4/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 09:54:27.000000 irails-1.2.4/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 09:54:28.127858 irails-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.2.4/setup.py
```

### Comparing `irails-1.2.2/PKG-INFO` & `irails-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.2
+Version: 1.2.4
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
-Metadata-Version: 2.1 Name: irails Version: 1.2.2 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.2.4 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.2.2/README.md` & `irails-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/_i18n.py` & `irails-1.2.4/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/_loader.py` & `irails-1.2.4/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/_utils.py` & `irails-1.2.4/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/auth.py` & `irails-1.2.4/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/base_controller.py` & `irails-1.2.4/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.2.4/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.2.4/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/cbv.py` & `irails-1.2.4/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/config.py` & `irails-1.2.4/irails/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,29 +145,29 @@
                         sub_value = segment_config
                         for sub_key in sub_keys:
                             sub_value = sub_value.get(sub_key, {})
                         value = value.replace("{" + name + "}", str(sub_value))
             else:
                 value = value.replace("{" + name + "}", self.config.get(name, ""))
         return value
- 
+debug = False
 def __init_log(__logCfg):
     if not __logCfg:
         return None
     from fastapi.logger import logger
     __log_level = __logCfg['level'] or 'DEBUG'
     __log_file = __logCfg['file'] or None 
-    __isdebug = config.get("debug") or False
+    debug = config.get("debug") or False
     logger.name = __logCfg.get("name",'iRails')
     if __log_file:
         __log_file = os.path.abspath(__log_file)
     log_format="%(asctime)s %(name)s:%(levelname)s:%(message)s"
     datefmt="%Y-%M-%d %H:%M:%S" 
     if __log_file:
-        if __isdebug:
+        if debug:
             try:
                 os.remove(__log_file)
             except:
                 pass
             import io
             
         handler = logging.FileHandler(__log_file,mode='a')
```

### Comparing `irails-1.2.2/irails/controller_utils.py` & `irails-1.2.4/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/core.py` & `irails-1.2.4/irails/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     def __init__(self,  **kwargs):
         self.__authObj:auth.AuthenticationBackend_ = None 
         self._data_engine:database.Engine = None
         self.__user_auth_url=""
         self.__public_auth_url=""
         self._app_views_dirs = {} 
         self.routers_map = {}
+        self.__apps_dirs = []
         super().__init__(**kwargs)
     
     def route(self, path: str, methods: List[str] | None = None, name: str | None = None, include_in_schema: bool = True) -> Callable[..., Any]:
         '''disabled'''
         raise RuntimeError(_("Please use api.http,MVC app not allow to use this direct!"))
         #return super().route(path, methods, name, include_in_schema)
     def post(self, path: str, *, response_model: Any = ..., status_code: int | None = None, tags: List[str | Enum] | None = None, dependencies: Sequence[Depends] | None = None, summary: str | None = None, description: str | None = None, response_description: str = "Successful Response", responses: Dict[int | str, Dict[str, Any]] | None = None, deprecated: bool | None = None, operation_id: str | None = None, response_model_include: SetIntStr | DictIntStrAny | None = None, response_model_exclude: SetIntStr | DictIntStrAny | None = None, response_model_by_alias: bool = True, response_model_exclude_unset: bool = False, response_model_exclude_defaults: bool = False, response_model_exclude_none: bool = False, include_in_schema: bool = True, response_class: Type[Response] = ..., name: str | None = None, callbacks: List[BaseRoute] | None = None, openapi_extra: Dict[str, Any] | None = None, generate_unique_id_function: Callable[[APIRouter], str] = ...) -> Callable[[DecoratedCallable], DecoratedCallable]:
@@ -76,14 +77,17 @@
         raise RuntimeError(_("Please use api.patch,MVC app not allow to use this direct!"))
         #return super().patch(path, response_model=response_model, status_code=status_code, tags=tags, dependencies=dependencies, summary=summary, description=description, response_description=response_description, responses=responses, deprecated=deprecated, operation_id=operation_id, response_model_include=response_model_include, response_model_exclude=response_model_exclude, response_model_by_alias=response_model_by_alias, response_model_exclude_unset=response_model_exclude_unset, response_model_exclude_defaults=response_model_exclude_defaults, response_model_exclude_none=response_model_exclude_none, include_in_schema=include_in_schema, response_class=response_class, name=name, callbacks=callbacks, openapi_extra=openapi_extra, generate_unique_id_function=generate_unique_id_function)
     def trace(self, path: str, *, response_model: Any = ..., status_code: int | None = None, tags: List[str | Enum] | None = None, dependencies: Sequence[Depends] | None = None, summary: str | None = None, description: str | None = None, response_description: str = "Successful Response", responses: Dict[int | str, Dict[str, Any]] | None = None, deprecated: bool | None = None, operation_id: str | None = None, response_model_include: SetIntStr | DictIntStrAny | None = None, response_model_exclude: SetIntStr | DictIntStrAny | None = None, response_model_by_alias: bool = True, response_model_exclude_unset: bool = False, response_model_exclude_defaults: bool = False, response_model_exclude_none: bool = False, include_in_schema: bool = True, response_class: Type[Response] = ..., name: str | None = None, callbacks: List[BaseRoute] | None = None, openapi_extra: Dict[str, Any] | None = None, generate_unique_id_function: Callable[[APIRoute], str] = ...) -> Callable[[DecoratedCallable], DecoratedCallable]:
         '''disabled'''
         raise RuntimeError(_("Please use api.trace,MVC app not allow to use this direct!"))
         #return super().trace(path, response_model=response_model, status_code=status_code, tags=tags, dependencies=dependencies, summary=summary, description=description, response_description=response_description, responses=responses, deprecated=deprecated, operation_id=operation_id, response_model_include=response_model_include, response_model_exclude=response_model_exclude, response_model_by_alias=response_model_by_alias, response_model_exclude_unset=response_model_exclude_unset, response_model_exclude_defaults=response_model_exclude_defaults, response_model_exclude_none=response_model_exclude_none, include_in_schema=include_in_schema, response_class=response_class, name=name, callbacks=callbacks, openapi_extra=openapi_extra, generate_unique_id_function=generate_unique_id_function)
     
+    @property
+    def apps_dirs(self)->List:
+        return self.__apps_dirs
     
     @property
     def public_auth_url(self):
         """public user auth url"""
         return self.__public_auth_url
     @public_auth_url.setter
     def public_auth_url(self,url):
@@ -116,15 +120,15 @@
         return self._data_engine
     @data_engine.setter
     def data_engine(self,value):
         self._data_engine = value
 
 __app = MvcApp( ) 
 
-__all_controller__ = []
+__all_controller__ = {}
 
 application = __app
 api.init(application)
 
  
 def check_init_database(): 
     db_cfg = config.get("database")
@@ -160,35 +164,44 @@
 
     caller_frame = inspect.currentframe().f_back
     caller_file = caller_frame.f_code.co_filename
     relative_path = caller_file.replace(ROOT_PATH,"")
     if relative_path.count(os.sep)>2:
         app_dir = os.sep.join(relative_path.split(os.sep)[:-2]) # os.path.dirname(os.path.dirname(relative_path)).replace(os.sep,"")
     else:
-        app_dir = "app"
-    app_dir = os.path.join(ROOT_PATH,app_dir.lstrip(os.sep))
+        raise RuntimeError(_("app dir must in apps dir"))
+     
 
     def format_path(p,v):
         if p and not p.startswith("/"):
             raise RuntimeError(_("route path must start with '/',%s is not alowed!") % p)
         if p and  '{controller}' not in p :
             p += '/{controller}' 
             p += '/{version}' if v else ''
         if v and not path:
             p = "/{controller}/{version}"
         return p
     path = format_path(path,version) 
      
-    abs_path = app_dir
+    abs_path = os.path.join(ROOT_PATH,app_dir.lstrip(os.sep))
+
+    if os.path.dirname(abs_path) not in application.apps_dirs:
+        application.apps_dirs.append(os.path.dirname(abs_path))
+    
     _controllerBase = create_controller(path,version)  
-        
-    __all_controller__.append(_controllerBase)
+    
+    
+    
     
     def _wapper(targetController):  
-        
+        _name = app_dir.replace(os.sep,".").lstrip(".") + "." + targetController.__name__ + "@" + version 
+        _controller_hash = f"{_name}" 
+        if not _controller_hash in __all_controller__:
+            __all_controller__[_controller_hash] = {'label':'new','obj': _controllerBase}
+
         class puppetController( targetController ,_controllerBase ): 
             '''puppet class inherited by the User defined controller class '''
             def __init__(self,**kwags) -> None: 
                 
                 super().__init__()
             def _user_logout(self,msg=_('your are successed logout!'),redirect:str="/"):
                 """see .core.py"""
@@ -275,30 +288,30 @@
         setattr(puppetController,AUTH_KEY,allargs['auth'])         
         setattr(puppetController,"__name__",targetController.__name__)  
         controller_name = get_controller_name(targetController.__name__)
         setattr(puppetController,"__controller_name__",controller_name)  
         
         setattr(puppetController,"__version__",version)  
         setattr(puppetController,"__location__",relative_path)  
-        setattr(puppetController,"__appdir__",app_dir)  
+        setattr(puppetController,"__appdir__",abs_path)  
 
         setattr(puppetController,"__controler_url__",controller_name)  
         #for generate url_for function
         url_path = path
        
-        _view_url_path:str = url_path.replace("{controller}",controller_name).replace("{version}",version) # "/" + os.path.basename(app_dir) + '_views'  
+        _view_url_path:str = url_path.replace("{controller}",controller_name).replace("{version}",version)  
         
-        controller_current_view_path = abs_path + '/views/' + controller_name # app_dir.replace(ROOT_PATH,'').replace("\\",'/') + '/views/' + controller_name 
+        controller_current_view_path = abs_path + '/views/' + controller_name  
         if version:
             controller_current_view_path += '/' + version
         setattr(puppetController,"__view_url__",_view_url_path) 
 
         #add app dir sub views to StaticFiles
         if not controller_current_view_path in application._app_views_dirs: #ensure  load it once
-            application._app_views_dirs[controller_current_view_path] = _view_url_path#os.path.join(app_dir,"views")
+            application._app_views_dirs[controller_current_view_path] = _view_url_path 
             #path match static files
             
             
  
         return puppetController 
     return _wapper #: @puppetController 
 
@@ -308,80 +321,116 @@
     while hasattr(ret,'__wrapped__'):
         ret = getattr(ret,'__wrapped__')
     return ret
 def _register_controllers():
     global __is_debug
     all_routers = []
     all_routers_map = {}
-    for ctrl in __all_controller__:
-        all_routers.append(register_controllers_to_app(application, ctrl))
+    for hash,dict_obj in __all_controller__.items():
+
+        if dict_obj['label'] == 'new':
+            if __is_debug:  
+                _log.info(hash+" mountting...")
+            all_routers.append(register_controllers_to_app(application, dict_obj['obj']))
+            dict_obj['label'] = 'mounted'
+
     for router in all_routers:
         for r in router.routes:
             funcname = str(r.endpoint).split('<function ')[1].split(" at ")[0] 
             end_point_abs = get_wrapped_endpoint(r.endpoint)
             auth_type = getattr(end_point_abs,AUTH_KEY) if hasattr(end_point_abs,AUTH_KEY) else 'None'
             doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
             if hasattr(r,'methods'):
                 methods = r.methods
             else:
                 methods = r.name
             if __is_debug:  
                 _log.info((str(methods),r.path,funcname) )
-            all_routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type}
-    application.routers_map = all_routers_map  
+            application.routers_map[funcname] = {'path':r.path,'methods':methods,'doc':doc_map,'auth':auth_type}
+      
+    _log.info(_("static files mouting..."))
+    midware.init(app=application,debug=__is_debug)
+
+def check_db_migrate():
+    db_cfg = config.get("database")
+    if __is_debug and db_cfg:
+        _log.info(_("checking database migrations...."))
+    try:
+            
+        alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
+        uri = db_cfg.get("uri")
+        if uri:
+            database.check_migration(application.data_engine,uri,alembic_ini)
+    except Exception as e:
+        _log.disabled = False
+        _log.error(e.args)
 def generate_mvc_app( ):
     global __is_debug
     _log.disabled = False
     from ._loader import _load_apps
     
     _log.info(_("\n\init mvc app..."))
     loaded,unloaded=_load_apps(debug=__is_debug) 
     _log.info(_('Load Apps Completed,%s loaded,%s unloaded') %(loaded,unloaded))  
     if not len(__all_controller__)>0:
         raise RuntimeError(_("not found any controller class"))
     
     _register_controllers()
 
-    _log.info(_("static files mouting..."))
-    midware.init(app=application,debug=__is_debug)
-
+    
     if __is_debug:
         _log.info(_("checking database configure..."))
-    db_cfg = check_init_database()
+    check_init_database()
+
     auth_type = config.get("auth",None)
     _casbin_adapter_class=None
     _adapter_uri:str=None
     if auth_type:
         auth_type=auth_type.get("type" )
         if auth_type:
             __type_casbin_adapter = config.get("auth").get("casbin_adapter","file")
             _casbin_adapter_class =  auth.get_adapter_module(__type_casbin_adapter)
             _adapter_uri = config.get("auth").get("adapter_uri") 
             if not _casbin_adapter_class:
                 raise RuntimeError(_( "Not support %s ,Adapter config error in auth.casbin_adapter") % __type_casbin_adapter)
             
     
-    if __is_debug and db_cfg:
-        _log.info(_("checking database migrations...."))
-        try:
-             
-            alembic_ini = db_cfg.get("alembic_ini",'./configs/alembic.ini')
-            uri = db_cfg.get("uri")
-            if uri:
-                database.check_migration(application.data_engine,uri,alembic_ini)
-        except Exception as e:
-            _log.disabled = False
-            _log.error(e.args)
+    check_db_migrate()
+
     if _casbin_adapter_class and _adapter_uri:
         _log.info(_("init casbin auth system..."))
         application.authObj = __init_auth(application,auth_type,_casbin_adapter_class,_adapter_uri)
     _log.info(_("init mvc app end."))
     return application
+# import subprocess
+# import time
+# # 定义启动和停止进程的方法
+# def start_uvicon():
+#     cmd = 'uvicorn main:app --host 0.0.0.0 --port 8000'
+#     uvicorn_process = subprocess.Popen(cmd.split(), stdout=subprocess.PIPE)
+#     return uvicorn_process
+
+# def restart_uvicon(uvicorn_process):
+#     uvicorn_process.terminate()
+#     # 等待 10 秒后重启进程
+#     time.sleep(10)
+#     # 启动进程
+#     uvicorn_process = start_uvicon()
 
-def run(app,*args,**kwargs): 
-    import uvicorn
-    global __is_debug 
-    if  "debug" in kwargs:
-        __is_debug = kwargs["debug"] 
-        del kwargs['debug'] 
-     
-    uvicorn.run(app, **kwargs)
+    
+ 
+
+
+# def run(app,*args,**kwargs): 
+#     import uvicorn
+#     global __is_debug 
+#     if  "debug" in kwargs:
+#         __is_debug = kwargs["debug"] 
+#         del kwargs['debug'] 
+#     if __is_debug:
+#         kwargs['reload'] = __is_debug
+#         kwargs['log_level'] = _log.level
+#         kwargs['reload_dirs'] = application.apps_dirs 
+#         uvicorn.run('irails.core:application', **kwargs)
+   
+         
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `irails-1.2.2/irails/database.py` & `irails-1.2.4/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/midware.py` & `irails-1.2.4/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/midware_casbin.py` & `irails-1.2.4/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/midware_session.py` & `irails-1.2.4/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/mvc_router.py` & `irails-1.2.4/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/_app.py` & `irails-1.2.4/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/_controller.py` & `irails-1.2.4/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/_i18n.py` & `irails-1.2.4/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/_project.py` & `irails-1.2.4/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/_run.py` & `irails-1.2.4/irails/scripts/_run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import argparse
 import os,importlib,sys
-from irails import  run as runserver 
+import uvicorn
 from irails.config import IS_IN_irails
+import irails.core
+from irails.core import application
+from irails.config import config
 
 def main():
-
+     
     if not IS_IN_irails:
         print(f"`run` command must run in the directory of irails project")
         exit()
     self_file = os.path.basename(__file__).lstrip("_").replace(".py",'')
     parser = argparse.ArgumentParser(usage=f"{sys.argv[0]} {self_file} [-h] [-p port]", description='run app') 
     parser.add_argument('-p','--port',type=int, help="http port")    
     parser.add_argument('-d','--debug',action='store_true',  help="enable debug mode")    
     args = parser.parse_args()
-    module_path = 'main.py'
-    kwargs = {'debug':False}
-    if args.debug:
-        kwargs['debug'] = args.debug
+    
+    kwargs = { }
+
     if args.port:
         kwargs['port'] = args.port
-    def do_run(app):
-        runserver(app,**kwargs)
-    if os.path.exists(module_path):
-        spec = importlib.util.spec_from_file_location(module_path, module_path)
-        module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(module)
-        do_run(module.app) 
-    else:
-        from irails import generate_mvc_app
-        app = generate_mvc_app()
-        do_run(app)
-         
-        # print(f'please exec on irals project\'s dir,missing main.py')
-        # exit()
+    kwargs['reload'] = True
+    if args.debug: 
+        kwargs['reload'] = args.debug 
+        app_cfg = config.get('app')
+        apps_dirs = app_cfg.get("appdir") 
+        kwargs['reload_dirs'] = apps_dirs
+        kwargs['reload_includes'] = ['*.po']
+    # module_path = 'main.py'
+    # spec = importlib.util.spec_from_file_location(module_path, module_path)
+    # module = importlib.util.module_from_spec(spec)
+    # spec.loader.exec_module(module)
+    
+    
+
+    uvicorn.run(app="irails.core:generate_mvc_app",**kwargs)      
+
```

### Comparing `irails-1.2.2/irails/scripts/main.py` & `irails-1.2.4/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/app/home.css.tpl` & `irails-1.2.4/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/app/home.tpl` & `irails-1.2.4/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.2.4/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.2.4/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.2.4/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/public/error_404.html` & `irails-1.2.4/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/public/error_500.html` & `irails-1.2.4/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.2.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.2.4/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.2.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.2.4/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.2.4/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails/view.py` & `irails-1.2.4/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails.egg-info/PKG-INFO` & `irails-1.2.4/irails.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.2.2
+Version: 1.2.4
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
-Metadata-Version: 2.1 Name: irails Version: 1.2.2 Summary: Simple and elegant
+Metadata-Version: 2.1 Name: irails Version: 1.2.4 Summary: Simple and elegant
 use of FastApi in MVC mode Home-page: https://github.com/smjkzsl/irails Author:
 Bruce chou Author-email: smjkzsl@gmail.com License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `irails-1.2.2/irails.egg-info/SOURCES.txt` & `irails-1.2.4/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/irails.egg-info/requires.txt` & `irails-1.2.4/irails.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `irails-1.2.2/setup.py` & `irails-1.2.4/setup.py`

 * *Files identical despite different names*

