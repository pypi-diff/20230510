# Comparing `tmp/garpix_cart-2.2.0.tar.gz` & `tmp/garpix_cart-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_cart-2.2.0.tar", last modified: Wed Nov 10 19:46:44 2021, max compression
+gzip compressed data, was "garpix_cart-3.0.0.tar", last modified: Wed May 10 16:14:02 2023, max compression
```

## Comparing `garpix_cart-2.2.0.tar` & `garpix_cart-3.0.0.tar`

### file list

```diff
@@ -1,76 +1,72 @@
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.262421 garpix_cart-2.2.0/
--rw-r--r--   0 crusat     (501) staff       (20)       31 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/MANIFEST.in
--rw-r--r--   0 crusat     (501) staff       (20)     4087 2021-11-10 19:46:44.262276 garpix_cart-2.2.0/PKG-INFO
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.257109 garpix_cart-2.2.0/garpix_cart/
--rwxr-xr-x   0 crusat     (501) staff       (20)       31 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/MANIFEST.in
--rwxr-xr-x   0 crusat     (501) staff       (20)       57 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.258711 garpix_cart-2.2.0/garpix_cart/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      213 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1651 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/__pycache__/abstracts.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      418 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/__pycache__/apps.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      323 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/__pycache__/exceptions.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      837 2021-11-10 19:46:43.000000 garpix_cart-2.2.0/garpix_cart/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      321 2021-10-08 11:54:18.000000 garpix_cart-2.2.0/garpix_cart/__pycache__/routers.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      297 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      324 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/__pycache__/utils.cpython-38.pyc
--rwxr-xr-x   0 crusat     (501) staff       (20)     1000 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/abstracts.py
--rwxr-xr-x   0 crusat     (501) staff       (20)      128 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/apps.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.252937 garpix_cart-2.2.0/garpix_cart/base/
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.259170 garpix_cart-2.2.0/garpix_cart/base/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      353 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/base/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1479 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/base/__pycache__/base_session_handlers.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1209 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/base/__pycache__/session_cores.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1945 2021-09-01 12:20:21.000000 garpix_cart-2.2.0/garpix_cart/base/__pycache__/session_handlers.cpython-38.pyc
--rwxr-xr-x   0 crusat     (501) staff       (20)       37 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/exceptions.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.259283 garpix_cart-2.2.0/garpix_cart/migrations/
--rwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/migrations/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.259375 garpix_cart-2.2.0/garpix_cart/migrations/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      168 2021-10-08 11:54:19.000000 garpix_cart-2.2.0/garpix_cart/migrations/__pycache__/__init__.cpython-38.pyc
--rwxr-xr-x   0 crusat     (501) staff       (20)      301 2021-11-10 19:45:56.000000 garpix_cart-2.2.0/garpix_cart/mixins.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.259688 garpix_cart-2.2.0/garpix_cart/models/
--rwxr-xr-x   0 crusat     (501) staff       (20)       58 2021-10-08 11:51:39.000000 garpix_cart-2.2.0/garpix_cart/models/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.260012 garpix_cart-2.2.0/garpix_cart/models/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      242 2021-10-08 11:53:28.000000 garpix_cart-2.2.0/garpix_cart/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1504 2021-10-08 11:53:28.000000 garpix_cart-2.2.0/garpix_cart/models/__pycache__/cart.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     2964 2021-11-10 19:46:43.000000 garpix_cart-2.2.0/garpix_cart/models/__pycache__/customer.cpython-38.pyc
--rwxr-xr-x   0 crusat     (501) staff       (20)      961 2021-10-08 11:51:39.000000 garpix_cart-2.2.0/garpix_cart/models/cart.py
--rw-r--r--   0 crusat     (501) staff       (20)     2918 2021-11-10 19:45:56.000000 garpix_cart-2.2.0/garpix_cart/models/customer.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.260212 garpix_cart-2.2.0/garpix_cart/permissions/
--rw-r--r--   0 crusat     (501) staff       (20)      307 2021-10-08 11:51:39.000000 garpix_cart-2.2.0/garpix_cart/permissions/IsCustomer.py
--rw-r--r--   0 crusat     (501) staff       (20)       35 2021-10-08 11:51:39.000000 garpix_cart-2.2.0/garpix_cart/permissions/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.260410 garpix_cart-2.2.0/garpix_cart/permissions/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      690 2021-10-08 11:54:18.000000 garpix_cart-2.2.0/garpix_cart/permissions/__pycache__/IsCustomer.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      200 2021-10-08 11:54:18.000000 garpix_cart-2.2.0/garpix_cart/permissions/__pycache__/__init__.cpython-38.pyc
--rwxr-xr-x   0 crusat     (501) staff       (20)      157 2021-10-08 11:51:39.000000 garpix_cart-2.2.0/garpix_cart/routers.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.260692 garpix_cart-2.2.0/garpix_cart/serializers/
--rwxr-xr-x   0 crusat     (501) staff       (20)      102 2021-11-10 19:45:56.000000 garpix_cart-2.2.0/garpix_cart/serializers/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.261010 garpix_cart-2.2.0/garpix_cart/serializers/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      300 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart/serializers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     1012 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart/serializers/__pycache__/cart.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)      635 2021-10-08 11:54:18.000000 garpix_cart-2.2.0/garpix_cart/serializers/__pycache__/customer.cpython-38.pyc
--rwxr-xr-x   0 crusat     (501) staff       (20)      506 2021-11-10 19:45:56.000000 garpix_cart-2.2.0/garpix_cart/serializers/cart.py
--rw-r--r--   0 crusat     (501) staff       (20)      223 2021-10-08 11:51:39.000000 garpix_cart-2.2.0/garpix_cart/serializers/customer.py
--rwxr-xr-x   0 crusat     (501) staff       (20)     1076 2021-11-10 19:46:36.000000 garpix_cart-2.2.0/garpix_cart/setup.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.261284 garpix_cart-2.2.0/garpix_cart/tests/
--rwxr-xr-x   0 crusat     (501) staff       (20)       39 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/tests/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.261533 garpix_cart-2.2.0/garpix_cart/tests/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      212 2021-10-08 11:54:19.000000 garpix_cart-2.2.0/garpix_cart/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     3638 2021-10-08 11:58:41.000000 garpix_cart-2.2.0/garpix_cart/tests/__pycache__/test_api.cpython-38.pyc
--rwxr-xr-x   0 crusat     (501) staff       (20)     4884 2021-11-10 19:45:56.000000 garpix_cart-2.2.0/garpix_cart/tests/test_api.py
--rwxr-xr-x   0 crusat     (501) staff       (20)      121 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/urls.py
--rwxr-xr-x   0 crusat     (501) staff       (20)      145 2021-09-01 12:19:49.000000 garpix_cart-2.2.0/garpix_cart/utils.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.261807 garpix_cart-2.2.0/garpix_cart/views/
--rwxr-xr-x   0 crusat     (501) staff       (20)       27 2021-10-08 11:51:39.000000 garpix_cart-2.2.0/garpix_cart/views/__init__.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.262098 garpix_cart-2.2.0/garpix_cart/views/__pycache__/
--rw-r--r--   0 crusat     (501) staff       (20)      200 2021-10-08 11:54:18.000000 garpix_cart-2.2.0/garpix_cart/views/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 crusat     (501) staff       (20)     4806 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart/views/__pycache__/cart.cpython-38.pyc
--rwxr-xr-x   0 crusat     (501) staff       (20)     5023 2021-11-10 19:45:56.000000 garpix_cart-2.2.0/garpix_cart/views/cart.py
-drwxr-xr-x   0 crusat     (501) staff       (20)        0 2021-11-10 19:46:44.257835 garpix_cart-2.2.0/garpix_cart.egg-info/
--rw-r--r--   0 crusat     (501) staff       (20)     4087 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart.egg-info/PKG-INFO
--rw-r--r--   0 crusat     (501) staff       (20)     2213 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart.egg-info/SOURCES.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart.egg-info/dependency_links.txt
--rw-r--r--   0 crusat     (501) staff       (20)        1 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart.egg-info/not-zip-safe
--rw-r--r--   0 crusat     (501) staff       (20)       36 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart.egg-info/requires.txt
--rw-r--r--   0 crusat     (501) staff       (20)       12 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/garpix_cart.egg-info/top_level.txt
--rw-r--r--   0 crusat     (501) staff       (20)       38 2021-11-10 19:46:44.262465 garpix_cart-2.2.0/setup.cfg
--rw-r--r--   0 crusat     (501) staff       (20)     1076 2021-11-10 19:46:44.000000 garpix_cart-2.2.0/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.287565 garpix_cart-3.0.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3992 2023-05-10 16:14:02.287393 garpix_cart-3.0.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.279317 garpix_cart-3.0.0/garpix_cart/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      734 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/CONTRIBUTING.md
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)       31 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/MANIFEST.in
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)     3429 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/README.md
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)       57 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.283758 garpix_cart-3.0.0/garpix_cart/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      221 2022-11-14 22:17:44.000000 garpix_cart-3.0.0/garpix_cart/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      426 2022-11-14 22:17:44.000000 garpix_cart-3.0.0/garpix_cart/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      918 2023-05-10 16:14:01.000000 garpix_cart-3.0.0/garpix_cart/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      329 2022-11-14 22:17:47.000000 garpix_cart-3.0.0/garpix_cart/__pycache__/routers.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      396 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart/__pycache__/urls.cpython-38.pyc
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)     1000 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/abstracts.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.284013 garpix_cart-3.0.0/garpix_cart/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       40 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/admin/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.284280 garpix_cart-3.0.0/garpix_cart/admin/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      213 2023-05-10 16:14:01.000000 garpix_cart-3.0.0/garpix_cart/admin/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      460 2023-05-10 16:14:01.000000 garpix_cart-3.0.0/garpix_cart/admin/__pycache__/cart.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      150 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/admin/cart.py
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)      128 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/apps.py
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)       37 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/exceptions.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.284415 garpix_cart-3.0.0/garpix_cart/migrations/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/migrations/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.284520 garpix_cart-3.0.0/garpix_cart/migrations/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-11-14 23:58:49.000000 garpix_cart-3.0.0/garpix_cart/migrations/__pycache__/__init__.cpython-38.pyc
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)      360 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/mixins.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.284775 garpix_cart-3.0.0/garpix_cart/models/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)       27 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.285026 garpix_cart-3.0.0/garpix_cart/models/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      209 2023-05-10 16:14:01.000000 garpix_cart-3.0.0/garpix_cart/models/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1627 2023-05-10 16:14:01.000000 garpix_cart-3.0.0/garpix_cart/models/__pycache__/cart.cpython-38.pyc
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)     1052 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/models/cart.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.285296 garpix_cart-3.0.0/garpix_cart/permissions/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      323 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/permissions/IsCustomer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/permissions/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.285554 garpix_cart-3.0.0/garpix_cart/permissions/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      708 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart/permissions/__pycache__/IsCustomer.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      208 2022-11-14 22:17:47.000000 garpix_cart-3.0.0/garpix_cart/permissions/__pycache__/__init__.cpython-38.pyc
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)      157 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/routers.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.285807 garpix_cart-3.0.0/garpix_cart/serializers/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)       61 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/serializers/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.286075 garpix_cart-3.0.0/garpix_cart/serializers/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      257 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart/serializers/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart/serializers/__pycache__/cart.cpython-38.pyc
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)      507 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/serializers/cart.py
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)     1059 2023-05-10 16:13:51.000000 garpix_cart-3.0.0/garpix_cart/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.286323 garpix_cart-3.0.0/garpix_cart/tests/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)       39 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/tests/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.286598 garpix_cart-3.0.0/garpix_cart/tests/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      220 2022-11-14 23:58:49.000000 garpix_cart-3.0.0/garpix_cart/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3472 2022-11-15 00:03:39.000000 garpix_cart-3.0.0/garpix_cart/tests/__pycache__/test_api.cpython-38.pyc
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)     4291 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/tests/test_api.py
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)      200 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/urls.py
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)      145 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/utils.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.286885 garpix_cart-3.0.0/garpix_cart/views/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)       27 2022-11-14 21:54:21.000000 garpix_cart-3.0.0/garpix_cart/views/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.287178 garpix_cart-3.0.0/garpix_cart/views/__pycache__/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      208 2022-11-14 22:17:47.000000 garpix_cart-3.0.0/garpix_cart/views/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4440 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart/views/__pycache__/cart.cpython-38.pyc
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)     4286 2023-05-10 16:13:17.000000 garpix_cart-3.0.0/garpix_cart/views/cart.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-05-10 16:14:02.282038 garpix_cart-3.0.0/garpix_cart.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3992 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1884 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       17 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/garpix_cart.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-05-10 16:14:02.287613 garpix_cart-3.0.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1059 2023-05-10 16:14:02.000000 garpix_cart-3.0.0/setup.py
```

### Comparing `garpix_cart-2.2.0/PKG-INFO` & `garpix_cart-3.0.0/garpix_cart.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 Metadata-Version: 2.1
-Name: garpix_cart
-Version: 2.2.0
-Summary: UNKNOWN
+Name: garpix-cart
+Version: 3.0.0
 Home-page: https://github.com/garpixcms/garpix_cart
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
 
+# Garpix Cart
 
-Garpix Cart
-===========
-
-Quickstart
-----------
+## Quickstart
 
 Install with pip 
 
-.. code-block::
+    $ pip install garpix_cart
 
-   $ pip install garpix_cart
+Add the `garpix_cart` to your INSTALLED_APPS:
 
+```python
+# settings.py
 
-Add the ``garpix_cart`` to your INSTALLED_APPS:
+INSTALLED_APPS = [
+    # ...
+    'garpix_cart',
+]
+```
 
-.. code-block:: python
+and to migration modules:
 
-   # settings.py
+```python
+# settings.py
 
-   INSTALLED_APPS = [
-       # ...
-       'garpix_cart',
-   ]
+# ...
+MIGRATION_MODULES = {
+    'garpix_cart': 'app.migrations.garpix_cart',
+}
+```
 
 Make migrations and migrate database:
 
-.. code-block::
-
-   $ ./manage.py makemigrations
-   $ ./manage.py migrate
-
+    $ ./manage.py makemigrations
+    $ ./manage.py migrate
 
-Add to ``urls.py``\ :
+Add to `urls.py`:
 
-.. code-block::
-
-   urlpatterns = [
-       # ...
-       path('', include('garpix_cart.urls'))
-   ]
+```
+urlpatterns = [
+    # ...
+    # garpix_cart
+    path('', include(('garpix_cart.urls', 'cart'), namespace='garpix_cart')),
+]
+```
 
 В интернет магазине обычно посетитель начинает искать интересные товары, надеясь добавить несколько из них в свою корзину. 
 Затем по пути к оформлению заказа они решают, создать ли учетную запись пользователя, использовать существующую или продолжить работу в качестве гостя. 
 Здесь все усложняется.
 
 Во-первых, для неаутентифицированных посетителей сайта корзина никому не принадлежит. Но каждая корзина должна быть 
 связана с ее текущим посетителем сайта.
@@ -73,24 +75,31 @@
 
 Django явно не разрешает использование таких пользовательских объектов в своих моделях баз данных. 
 Но, используя логический флаг is_active, мы можем обмануть приложение, чтобы оно интерпретировало такого гостя как 
 фальшивого анонимного пользователя.
 
 Такой подход неприменим для всех приложений на основе Django, добавляется новая модель - **Customer**
 
-Получить Customer
------------------
 
-Для создания Customer нужно сделать ``POST`` запрос на ``/api/v1/cart/create_customer/``
+## setting.py
+
+`GARPIX_CART_SERIALIZER_MIXIN` - можно задать миксин для сериалайзера элемента корзины
+
+`GARPIX_CART_MIXIN` - можно задать миксин для модели элемента корзины
+
+
+# Changelog
+
+See [CHANGELOG.md](CHANGELOG.md).
 
-Запрос вернет объект ``Customer`` с полем ``number``.
+# Contributing
 
-Далее нужно этот номер отправлять в каждый запрос с заголовок ``Cart-Token``.
+See [CONTRIBUTING.md](CONTRIBUTING.md).
 
-setting.py
-----------
+# License
 
-``GARPIX_CART_SERIALIZER_MIXIN`` - можно задать миксин для сериалайзера элемента корзины
+[MIT](LICENSE)
 
-``GARPIX_CART_MIXIN`` - можно задать миксин для модели элемента корзины
+---
 
+Developed by Garpix / [https://garpix.com](https://garpix.com)
```

### Comparing `garpix_cart-2.2.0/garpix_cart/abstracts.py` & `garpix_cart-3.0.0/garpix_cart/abstracts.py`

 * *Files identical despite different names*

### Comparing `garpix_cart-2.2.0/garpix_cart/models/__pycache__/cart.cpython-38.pyc` & `garpix_cart-3.0.0/garpix_cart/models/__pycache__/cart.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Oct  8 11:51:39 2021 UTC, .py size: 961 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,94 +1,102 @@
-00000000: 550d 0d0a 0000 0000 cb30 6061 c103 0000  U........0`a....
+00000000: 550d 0d0a 0000 0000 9dc2 5b64 1c04 0000  U.........[d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
+00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6403 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6405 6c06 6d07 5a07 0100 6503  ..d.d.l.m.Z...e.
-00000060: 6507 6a08 8301 5a09 4700 6406 6407 8400  e.j...Z.G.d.d...
-00000070: 6407 6509 8303 5a0a 6408 5300 2909 e900  d.e...Z.d.S.)...
-00000080: 0000 0029 01da 066d 6f64 656c 7329 01da  ...)...models)..
-00000090: 0d69 6d70 6f72 745f 7374 7269 6e67 e901  .import_string..
-000000a0: 0000 0029 01da 0843 7573 746f 6d65 7229  ...)...Customer)
-000000b0: 01da 0873 6574 7469 6e67 7363 0000 0000  ...settingsc....
-000000c0: 0000 0000 0000 0000 0000 0000 0600 0000  ................
-000000d0: 4000 0000 737c 0000 0065 005a 0164 005a  @...s|...e.Z.d.Z
-000000e0: 0265 036a 0465 0565 036a 0664 0164 028d  .e.j.e.e.j.d.d..
-000000f0: 035a 0765 036a 0864 0364 0365 0964 0464  .Z.e.j.d.d.e.d.d
-00000100: 058d 045a 0a65 036a 0b64 0664 0764 088d  ...Z.e.j.d.d.d..
-00000110: 025a 0c65 036a 0d64 0364 0964 0a8d 025a  .Z.e.j.d.d.d...Z
-00000120: 0e65 036a 0d64 0364 0b64 0c8d 025a 0f65  .e.j.d.d.d...Z.e
-00000130: 1064 0d64 0e84 0083 015a 1147 0064 0f64  .d.d.....Z.G.d.d
-00000140: 1084 0064 1083 025a 1264 1164 1284 005a  ...d...Z.d.d...Z
-00000150: 1364 1353 0029 14da 0843 6172 7449 7465  .d.S.)...CartIte
-00000160: 6d75 1800 0000 d09f d0be d0bb d18c d0b7  mu..............
-00000170: d0be d0b2 d0b0 d182 d0b5 d0bb d18c 2902  ..............).
-00000180: da09 6f6e 5f64 656c 6574 65da 0c76 6572  ..on_delete..ver
-00000190: 626f 7365 5f6e 616d 6554 752f 0000 00d0  bose_nameTu/....
-000001a0: 94d0 bed0 bfd0 bed0 bbd0 bdd0 b8d1 82d0  ................
-000001b0: b5d0 bbd1 8cd0 bdd1 8bd0 b520 d0bf d0b0  ........... ....
-000001c0: d180 d0b0 d0bc d0b5 d182 d180 d18b 2904  ..............).
-000001d0: da05 626c 616e 6bda 046e 756c 6cda 0764  ..blank..null..d
-000001e0: 6566 6175 6c74 7209 0000 0072 0400 0000  efaultr....r....
-000001f0: 7514 0000 00d0 9ad0 bed0 bbd0 b8d1 87d0  u...............
-00000200: b5d1 81d1 82d0 b2d0 be29 0272 0c00 0000  .........).r....
-00000210: 7209 0000 0075 0e00 0000 d0a1 d0be d0b7  r....u..........
-00000220: d0b4 d0b0 d0bd d0be 2902 da0c 6175 746f  ........)...auto
-00000230: 5f6e 6f77 5f61 6464 7209 0000 0075 1200  _now_addr....u..
-00000240: 0000 d09e d0b1 d0bd d0be d0b2 d0bb d0b5  ................
-00000250: d0bd d0be 2902 da08 6175 746f 5f6e 6f77  ....)...auto_now
-00000260: 7209 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000270: 0000 0100 0000 0100 0000 4300 0000 7308  ..........C...s.
-00000280: 0000 007c 006a 006a 0153 00a9 014e 2902  ...|.j.j.S...N).
-00000290: da08 6375 7374 6f6d 6572 da04 7573 6572  ..customer..user
-000002a0: a901 da04 7365 6c66 a900 7214 0000 00fa  ....self..r.....
-000002b0: 452f 5573 6572 732f 6372 7573 6174 2f70  E/Users/crusat/p
-000002c0: 726f 6a65 6374 732f 6761 7270 6978 5f63  rojects/garpix_c
-000002d0: 6172 742f 6261 636b 656e 642f 6761 7270  art/backend/garp
-000002e0: 6978 5f63 6172 742f 6d6f 6465 6c73 2f63  ix_cart/models/c
-000002f0: 6172 742e 7079 7211 0000 0010 0000 0073  art.pyr........s
-00000300: 0200 0000 0002 7a0d 4361 7274 4974 656d  ......z.CartItem
-00000310: 2e75 7365 7263 0000 0000 0000 0000 0000  .userc..........
-00000320: 0000 0000 0000 0100 0000 4000 0000 7314  ..........@...s.
-00000330: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
-00000340: 025a 0464 0353 0029 047a 0d43 6172 7449  .Z.d.S.).z.CartI
-00000350: 7465 6d2e 4d65 7461 750e 0000 00d0 9ad0  tem.Metau.......
-00000360: bed1 80d0 b7d0 b8d0 bdd0 b075 0e00 0000  ...........u....
-00000370: d09a d0be d180 d0b7 d0b8 d0bd d18b 4e29  ..............N)
-00000380: 05da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000390: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000003a0: 616d 655f 5f72 0900 0000 da13 7665 7262  ame__r......verb
-000003b0: 6f73 655f 6e61 6d65 5f70 6c75 7261 6c72  ose_name_pluralr
-000003c0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-000003d0: 0000 00da 044d 6574 6114 0000 0073 0400  .....Meta....s..
-000003e0: 0000 0801 0401 721a 0000 0063 0100 0000  ......r....c....
-000003f0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00000400: 4300 0000 7308 0000 007c 006a 009b 0053  C...s....|.j...S
-00000410: 0072 0f00 0000 2901 da02 706b 7212 0000  .r....)...pkr...
-00000420: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000430: da07 5f5f 7374 725f 5f18 0000 0073 0200  ..__str__....s..
-00000440: 0000 0001 7a10 4361 7274 4974 656d 2e5f  ....z.CartItem._
-00000450: 5f73 7472 5f5f 4e29 1472 1600 0000 7217  _str__N).r....r.
-00000460: 0000 0072 1800 0000 7202 0000 00da 0a46  ...r....r......F
-00000470: 6f72 6569 676e 4b65 7972 0500 0000 da07  oreignKeyr......
-00000480: 4341 5343 4144 4572 1000 0000 da09 4a53  CASCADEr......JS
-00000490: 4f4e 4669 656c 64da 0464 6963 74da 0670  ONField..dict..p
-000004a0: 6172 616d 73da 1450 6f73 6974 6976 6549  arams..PositiveI
-000004b0: 6e74 6567 6572 4669 656c 64da 0563 6f75  ntegerField..cou
-000004c0: 6e74 da0d 4461 7465 5469 6d65 4669 656c  nt..DateTimeFiel
-000004d0: 645a 0a63 7265 6174 6564 5f61 745a 0a75  dZ.created_atZ.u
-000004e0: 7064 6174 6564 5f61 74da 0870 726f 7065  pdated_at..prope
-000004f0: 7274 7972 1100 0000 721a 0000 0072 1c00  rtyr....r....r..
-00000500: 0000 7214 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00000510: 0072 1500 0000 7207 0000 0009 0000 0073  .r....r........s
-00000520: 1200 0000 0801 1201 1201 0e01 0e01 0e02  ................
-00000530: 0201 0a03 0e04 7207 0000 004e 290b da09  ......r....N)...
-00000540: 646a 616e 676f 2e64 6272 0200 0000 da1b  django.dbr......
-00000550: 646a 616e 676f 2e75 7469 6c73 2e6d 6f64  django.utils.mod
-00000560: 756c 655f 6c6f 6164 696e 6772 0300 0000  ule_loadingr....
-00000570: 7210 0000 0072 0500 0000 da0b 646a 616e  r....r......djan
-00000580: 676f 2e63 6f6e 6672 0600 0000 da11 4741  go.confr......GA
-00000590: 5250 4958 5f43 4152 545f 4d49 5849 4e5a  RPIX_CART_MIXINZ
-000005a0: 0943 6172 744d 6978 696e 7207 0000 0072  .CartMixinr....r
-000005b0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-000005c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000005d0: 0073 0a00 0000 0c01 0c01 0c01 0c02 0a03  .s..............
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a0a 0100 6503 6507 6a0b  d.l.m.Z...e.e.j.
+00000070: 8301 5a0c 4700 6406 6407 8400 6407 650c  ..Z.G.d.d...d.e.
+00000080: 8303 5a0d 6408 5300 2909 e900 0000 0029  ..Z.d.S.)......)
+00000090: 01da 066d 6f64 656c 7329 01da 0d69 6d70  ...models)...imp
+000000a0: 6f72 745f 7374 7269 6e67 2901 da0b 5573  ort_string)...Us
+000000b0: 6572 5365 7373 696f 6e29 01da 0873 6574  erSession)...set
+000000c0: 7469 6e67 7329 01da 0c67 6574 7465 7874  tings)...gettext
+000000d0: 5f6c 617a 7963 0000 0000 0000 0000 0000  _lazyc..........
+000000e0: 0000 0000 0000 0600 0000 4000 0000 7390  ..........@...s.
+000000f0: 0000 0065 005a 0164 005a 0265 036a 0465  ...e.Z.d.Z.e.j.e
+00000100: 0565 036a 0665 0764 0183 0164 028d 035a  .e.j.e.d...d...Z
+00000110: 0865 036a 0964 0364 0365 0a65 0764 0483  .e.j.d.d.e.e.d..
+00000120: 0164 058d 045a 0b65 036a 0c64 0665 0764  .d...Z.e.j.d.e.d
+00000130: 0783 0164 088d 025a 0d65 036a 0e64 0365  ...d...Z.e.j.d.e
+00000140: 0764 0983 0164 0a8d 025a 0f65 036a 0e64  .d...d...Z.e.j.d
+00000150: 0365 0764 0b83 0164 0c8d 025a 1065 1164  .e.d...d...Z.e.d
+00000160: 0d64 0e84 0083 015a 1247 0064 0f64 1084  .d.....Z.G.d.d..
+00000170: 0064 1083 025a 1364 1164 1284 005a 1464  .d...Z.d.d...Z.d
+00000180: 1353 0029 14da 0843 6172 7449 7465 6d75  .S.)...CartItemu
+00000190: 1800 0000 d09f d0be d0bb d18c d0b7 d0be  ................
+000001a0: d0b2 d0b0 d182 d0b5 d0bb d18c 2902 da09  ............)...
+000001b0: 6f6e 5f64 656c 6574 65da 0c76 6572 626f  on_delete..verbo
+000001c0: 7365 5f6e 616d 6554 752f 0000 00d0 94d0  se_nameTu/......
+000001d0: bed0 bfd0 bed0 bbd0 bdd0 b8d1 82d0 b5d0  ................
+000001e0: bbd1 8cd0 bdd1 8bd0 b520 d0bf d0b0 d180  ......... ......
+000001f0: d0b0 d0bc d0b5 d182 d180 d18b 2904 da05  ............)...
+00000200: 626c 616e 6bda 046e 756c 6cda 0764 6566  blank..null..def
+00000210: 6175 6c74 7209 0000 00e9 0100 0000 7514  aultr.........u.
+00000220: 0000 00d0 9ad0 bed0 bbd0 b8d1 87d0 b5d1  ................
+00000230: 81d1 82d0 b2d0 be29 0272 0c00 0000 7209  .......).r....r.
+00000240: 0000 0075 0e00 0000 d0a1 d0be d0b7 d0b4  ...u............
+00000250: d0b0 d0bd d0be 2902 da0c 6175 746f 5f6e  ......)...auto_n
+00000260: 6f77 5f61 6464 7209 0000 0075 1200 0000  ow_addr....u....
+00000270: d09e d0b1 d0bd d0be d0b2 d0bb d0b5 d0bd  ................
+00000280: d0be 2902 da08 6175 746f 5f6e 6f77 7209  ..)...auto_nowr.
+00000290: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000002a0: 0100 0000 0100 0000 4300 0000 7308 0000  ........C...s...
+000002b0: 007c 006a 006a 0153 00a9 014e 2902 da08  .|.j.j.S...N)...
+000002c0: 6375 7374 6f6d 6572 da04 7573 6572 a901  customer..user..
+000002d0: da04 7365 6c66 a900 7215 0000 00fa 4d2f  ..self..r.....M/
+000002e0: 5573 6572 732f 7669 6b74 6f72 6961 7265  Users/viktoriare
+000002f0: 7365 746f 7661 2f47 4152 5049 582f 6761  setova/GARPIX/ga
+00000300: 7270 6978 5f63 6172 742f 6261 636b 656e  rpix_cart/backen
+00000310: 642f 6761 7270 6978 5f63 6172 742f 6d6f  d/garpix_cart/mo
+00000320: 6465 6c73 2f63 6172 742e 7079 7212 0000  dels/cart.pyr...
+00000330: 0011 0000 0073 0200 0000 0002 7a0d 4361  .....s......z.Ca
+00000340: 7274 4974 656d 2e75 7365 7263 0000 0000  rtItem.userc....
+00000350: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00000360: 4000 0000 731c 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
+00000370: 0265 0364 0183 015a 0465 0364 0283 015a  .e.d...Z.e.d...Z
+00000380: 0564 0353 0029 047a 0d43 6172 7449 7465  .d.S.).z.CartIte
+00000390: 6d2e 4d65 7461 750e 0000 00d0 9ad0 bed1  m.Metau.........
+000003a0: 80d0 b7d0 b8d0 bdd0 b075 0e00 0000 d09a  .........u......
+000003b0: d0be d180 d0b7 d0b8 d0bd d18b 4e29 06da  ............N)..
+000003c0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000003d0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000003e0: 655f 5fda 015f 7209 0000 00da 1376 6572  e__.._r......ver
+000003f0: 626f 7365 5f6e 616d 655f 706c 7572 616c  bose_name_plural
+00000400: 7215 0000 0072 1500 0000 7215 0000 0072  r....r....r....r
+00000410: 1600 0000 da04 4d65 7461 1500 0000 7304  ......Meta....s.
+00000420: 0000 0008 0108 0172 1c00 0000 6301 0000  .......r....c...
+00000430: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00000440: 0043 0000 0073 0800 0000 7c00 6a00 9b00  .C...s....|.j...
+00000450: 5300 7210 0000 0029 01da 0270 6b72 1300  S.r....)...pkr..
+00000460: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+00000470: 00da 075f 5f73 7472 5f5f 1900 0000 7302  ...__str__....s.
+00000480: 0000 0000 017a 1043 6172 7449 7465 6d2e  .....z.CartItem.
+00000490: 5f5f 7374 725f 5f4e 2915 7217 0000 0072  __str__N).r....r
+000004a0: 1800 0000 7219 0000 0072 0200 0000 da0a  ....r....r......
+000004b0: 466f 7265 6967 6e4b 6579 7204 0000 00da  ForeignKeyr.....
+000004c0: 0743 4153 4341 4445 721a 0000 0072 1100  .CASCADEr....r..
+000004d0: 0000 da09 4a53 4f4e 4669 656c 64da 0464  ....JSONField..d
+000004e0: 6963 74da 0670 6172 616d 73da 1450 6f73  ict..params..Pos
+000004f0: 6974 6976 6549 6e74 6567 6572 4669 656c  itiveIntegerFiel
+00000500: 64da 0563 6f75 6e74 da0d 4461 7465 5469  d..count..DateTi
+00000510: 6d65 4669 656c 64da 0a63 7265 6174 6564  meField..created
+00000520: 5f61 74da 0a75 7064 6174 6564 5f61 74da  _at..updated_at.
+00000530: 0870 726f 7065 7274 7972 1200 0000 721c  .propertyr....r.
+00000540: 0000 0072 1e00 0000 7215 0000 0072 1500  ...r....r....r..
+00000550: 0000 7215 0000 0072 1600 0000 7207 0000  ..r....r....r...
+00000560: 000a 0000 0073 1200 0000 0801 1601 1601  .....s..........
+00000570: 1201 1201 1202 0201 0a03 0e04 7207 0000  ............r...
+00000580: 004e 290e da09 646a 616e 676f 2e64 6272  .N)...django.dbr
+00000590: 0200 0000 da1b 646a 616e 676f 2e75 7469  ......django.uti
+000005a0: 6c73 2e6d 6f64 756c 655f 6c6f 6164 696e  ls.module_loadin
+000005b0: 6772 0300 0000 da12 6761 7270 6978 5f75  gr......garpix_u
+000005c0: 7365 722e 6d6f 6465 6c73 7204 0000 00da  ser.modelsr.....
+000005d0: 0b64 6a61 6e67 6f2e 636f 6e66 7205 0000  .django.confr...
+000005e0: 00da 1864 6a61 6e67 6f2e 7574 696c 732e  ...django.utils.
+000005f0: 7472 616e 736c 6174 696f 6e72 0600 0000  translationr....
+00000600: 721a 0000 00da 1147 4152 5049 585f 4341  r......GARPIX_CA
+00000610: 5254 5f4d 4958 494e 5a09 4361 7274 4d69  RT_MIXINZ.CartMi
+00000620: 7869 6e72 0700 0000 7215 0000 0072 1500  xinr....r....r..
+00000630: 0000 7215 0000 0072 1600 0000 da08 3c6d  ..r....r......<m
+00000640: 6f64 756c 653e 0100 0000 730c 0000 000c  odule>....s.....
+00000650: 010c 010c 010c 010c 020a 03              ...........
```

### Comparing `garpix_cart-2.2.0/garpix_cart/models/cart.py` & `garpix_cart-3.0.0/garpix_cart/models/cart.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from django.db import models
 from django.utils.module_loading import import_string
-from .customer import Customer
+from garpix_user.models import UserSession
 from django.conf import settings
+from django.utils.translation import gettext_lazy as _
 
 CartMixin = import_string(settings.GARPIX_CART_MIXIN)
 
 
 class CartItem(CartMixin):
-    customer = models.ForeignKey(Customer, on_delete=models.CASCADE, verbose_name='Пользователь')
-    params = models.JSONField(blank=True, null=True, default=dict, verbose_name='Дополнительные параметры')
-    count = models.PositiveIntegerField(default=1, verbose_name='Количество')
-    created_at = models.DateTimeField(auto_now_add=True, verbose_name='Создано')
-    updated_at = models.DateTimeField(auto_now=True, verbose_name='Обновлено')
+    customer = models.ForeignKey(UserSession, on_delete=models.CASCADE, verbose_name=_('Пользователь'))
+    params = models.JSONField(blank=True, null=True, default=dict, verbose_name=_('Дополнительные параметры'))
+    count = models.PositiveIntegerField(default=1, verbose_name=_('Количество'))
+    created_at = models.DateTimeField(auto_now_add=True, verbose_name=_('Создано'))
+    updated_at = models.DateTimeField(auto_now=True, verbose_name=_('Обновлено'))
 
     @property
     def user(self):
         return self.customer.user
 
     class Meta:
-        verbose_name = 'Корзина'
-        verbose_name_plural = 'Корзины'
+        verbose_name = _('Корзина')
+        verbose_name_plural = _('Корзины')
 
     def __str__(self):
         return f'{self.pk}'
```

### Comparing `garpix_cart-2.2.0/garpix_cart/tests/test_api.py` & `garpix_cart-3.0.0/garpix_cart/tests/test_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from django.test import TestCase
 from django.contrib.auth import get_user_model
+from django.urls import reverse
+from garpix_user.models import UserSession
 
 from rest_framework.test import APIClient
 
-from ..models import CartItem, Customer
+from ..models import CartItem
 
 
 class CartViewTestCase(TestCase):
     def setUp(self):
         User = get_user_model()
         self.username = 'testuser1'
         self.password = '12345'
         self.user = User.objects.create_user(username=self.username, password=self.password)
-        self.customer = Customer.objects.create(user=self.user, recognized=Customer.CustomerState.REGISTERED)
+        self.customer = UserSession.objects.create(user=self.user, recognized=UserSession.UserState.REGISTERED)
         self.user.save()
         client = APIClient()
         client.force_authenticate(user=self.user)
         self.client = client
 
     def test_add(self):
         response = self.client.post(
-            '/api/v1/cart/add/',
+            reverse('garpix_cart:cart-add'),
             {
                 'data': [
                     {
                         'product': 1,
                         'count': 1,
                         'params': {
                             'color': '#000000'
@@ -38,15 +40,15 @@
 
         self.assertEqual(response.status_code, 200)
         count = CartItem.objects.all().count()
         self.assertEqual(count, 1)
 
     def test_session_add(self):
         response = self.client.post(
-            '/api/v1/cart/session_add/',
+            reverse('garpix_cart:cart-session-add'),
             {
                 'data': [
                     {
                         'product': 1,
                         'count': 1,
                         'params': {
                             'color': '#000000'
@@ -68,15 +70,15 @@
             count=1,
             params=dict(),
             customer=self.customer
         )
         cart_item.save()
 
         response = self.client.delete(
-            '/api/v1/cart/remove/',
+            reverse('garpix_cart:cart-remove'),
             {
                 'data': [
                     cart_item.pk
                 ]
             },
             format='json',
             HTTP_ACCEPT='application/json'
@@ -93,15 +95,15 @@
             count=1,
             params=dict(),
             customer=self.customer
         )
         cart_item.save()
 
         response = self.client.delete(
-            '/api/v1/cart/session_remove/',
+            reverse('garpix_cart:cart-session-remove'),
             {
                 'data': [
                     cart_item.pk
                 ]
             },
             format='json',
             HTTP_ACCEPT='application/json'
@@ -119,54 +121,32 @@
             count=1,
             params=dict(),
             customer=self.customer
         )
         cart_item.save()
 
         response = self.client.patch(
-            f'/api/v1/cart/{cart_item}/',
+            reverse('garpix_cart:cart-detail', args=[cart_item.pk]),
             {
                 'data': {
                     'count': product_count
                 }
             },
             format='json',
             HTTP_ACCEPT='application/json'
         )
 
         self.assertEqual(response.status_code, 200)
 
         obj = CartItem.objects.get(pk=cart_item.pk)
         self.assertEqual(obj.count, product_count)
 
-    def test_create_customer_user(self):
-        response = self.client.post(
-            '/api/v1/cart/create_customer/',
-            format='json',
-            HTTP_ACCEPT='application/json',
-        )
-
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(response.data['customer']['user'], self.user.pk)
-
-    def test_create_customer_token(self):
-        client = APIClient()
-        response = client.post(
-            '/api/v1/cart/create_customer/',
-            format='json',
-            HTTP_ACCEPT='application/json',
-        )
-
-        self.assertEqual(response.status_code, 200)
-        self.assertEqual(response.data['customer']['user'], None)
-        self.assertNotEqual(response.data['customer']['number'], None)
-
     def test_get_list_cart(self):
         CartItem.objects.create(customer=self.customer, count=1, params={}, product=10)
         response = self.client.get(
-            '/api/v1/cart/',
+            reverse('garpix_cart:cart-list'),
             format='json',
             HTTP_ACCEPT='application/json',
         )
 
         self.assertEqual(response.status_code, 200)
         self.assertEqual(len(response.data), 1)
```

### Comparing `garpix_cart-2.2.0/garpix_cart/views/__pycache__/cart.cpython-38.pyc` & `garpix_cart-3.0.0/garpix_cart/views/__pycache__/cart.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Nov 10 19:45:56 2021 UTC, .py size: 5023 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,301 +1,278 @@
-00000000: 550d 0d0a 0000 0000 7421 8c61 9f13 0000  U.......t!.a....
+00000000: 550d 0d0a 0000 0000 9dc2 5b64 be10 0000  U.........[d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 aa00 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6400 6404 6c05 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c05 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
-00000070: 6406 6c05 6d09 5a09 0100 6400 6407 6c0a  d.l.m.Z...d.d.l.
-00000080: 6d0b 5a0b 0100 6400 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
-00000090: 0100 6409 640a 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
-000000a0: 0100 6409 640b 6c07 6d11 5a11 0100 6409  ..d.d.l.m.Z...d.
-000000b0: 640c 6c12 6d13 5a13 6d14 5a14 6d15 5a15  d.l.m.Z.m.Z.m.Z.
-000000c0: 0100 4700 640d 640e 8400 640e 6509 6a16  ..G.d.d...d.e.j.
-000000d0: 8303 5a17 640f 5300 2910 e900 0000 0029  ..Z.d.S.)......)
-000000e0: 01da 084f 7074 696f 6e61 6c29 02da 0d65  ...Optional)...e
-000000f0: 7874 656e 645f 7363 6865 6d61 da10 4f70  xtend_schema..Op
-00000100: 656e 4170 6950 6172 616d 6574 6572 2901  enApiParameter).
-00000110: da07 7061 7273 6572 7329 01da 0b70 6572  ..parsers)...per
-00000120: 6d69 7373 696f 6e73 a901 da06 7374 6174  missions....stat
-00000130: 7573 2901 da08 7669 6577 7365 7473 2901  us)...viewsets).
-00000140: da06 6163 7469 6f6e 2901 da08 5265 7370  ..action)...Resp
-00000150: 6f6e 7365 e902 0000 0029 02da 0843 6172  onse.....)...Car
-00000160: 7449 7465 6dda 0843 7573 746f 6d65 7229  tItem..Customer)
-00000170: 01da 0a49 7343 7573 746f 6d65 7229 03da  ...IsCustomer)..
-00000180: 1243 6172 7449 7465 6d53 6572 6961 6c69  .CartItemSeriali
-00000190: 7a65 72da 1243 7573 746f 6d65 7253 6572  zer..CustomerSer
-000001a0: 6961 6c69 7a65 72da 1643 6172 7449 7465  ializer..CartIte
-000001b0: 6d4c 6973 7453 6572 6961 6c69 7a65 7263  mListSerializerc
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001d0: 0700 0000 4000 0000 7384 0100 0065 005a  ....@...s....e.Z
-000001e0: 0164 005a 0265 036a 0466 015a 0565 066a  .d.Z.e.j.f.Z.e.j
-000001f0: 0766 015a 0865 0965 0964 019c 025a 0a65  .f.Z.e.e.d...Z.e
-00000200: 0b65 0c6a 0d64 0264 0365 0e65 0b6a 0f64  .e.j.d.d.e.e.j.d
-00000210: 048d 055a 1065 115a 1264 0564 0684 005a  ...Z.e.Z.d.d...Z
-00000220: 1365 1465 0c19 0064 079c 0164 0864 0984  .e.e...d...d.d..
-00000230: 045a 1564 2964 0b64 0c84 015a 1664 0d64  .Z.d)d.d...Z.d.d
-00000240: 0e84 005a 1764 0f64 1084 005a 1864 1164  ...Z.d.d...Z.d.d
-00000250: 1284 005a 1965 1a65 1067 0164 138d 0164  ...Z.e.e.g.d...d
-00000260: 1464 1584 0083 015a 1b65 1c64 0a64 1667  .d.....Z.e.d.d.g
-00000270: 0165 066a 0766 0164 178d 0364 1864 1984  .e.j.f.d...d.d..
-00000280: 0083 015a 1d65 1a65 1067 0164 138d 0165  ...Z.e.e.g.d...e
-00000290: 1c64 0a64 1667 0165 1e66 0164 178d 0364  .d.d.g.e.f.d...d
-000002a0: 1a64 1b84 0083 0183 015a 1f65 1a65 1067  .d.......Z.e.e.g
-000002b0: 0164 138d 0165 1c64 0a64 1c67 0165 1e66  .d...e.d.d.g.e.f
-000002c0: 0164 178d 0364 1d64 1e84 0083 0183 015a  .d...d.d.......Z
-000002d0: 2065 1a65 1067 0164 138d 0165 1c64 0a64   e.e.g.d...e.d.d
-000002e0: 1f67 0165 066a 0766 0164 178d 0364 2064  .g.e.j.f.d...d d
-000002f0: 2184 0083 0183 015a 2165 1a65 1067 0164  !......Z!e.e.g.d
-00000300: 138d 0165 1c64 0a64 1c67 0165 1e66 0164  ...e.d.d.g.e.f.d
-00000310: 178d 0364 2264 2384 0083 0183 015a 2265  ...d"d#......Z"e
-00000320: 1a65 1067 0164 138d 0165 1c64 0a64 1667  .e.g.d...e.d.d.g
-00000330: 0165 066a 0766 0164 178d 0364 2464 2584  .e.j.f.d...d$d%.
-00000340: 0083 0183 015a 2365 1a65 1067 0164 138d  .....Z#e.e.g.d..
-00000350: 0164 2a64 2764 2884 0183 015a 2464 2653  .d*d'd(....Z$d&S
-00000360: 0029 2bda 0843 6172 7456 6965 7729 02da  .)+..CartView)..
-00000370: 0361 6464 da0b 7365 7373 696f 6e5f 6164  .add..session_ad
-00000380: 6472 0e00 0000 5429 05da 046e 616d 65da  dr....T)...name.
-00000390: 0b64 6573 6372 6970 7469 6f6e da08 7265  .description..re
-000003a0: 7175 6972 6564 da04 7479 7065 da08 6c6f  quired..type..lo
-000003b0: 6361 7469 6f6e 6301 0000 0000 0000 0000  cationc.........
-000003c0: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-000003d0: 1200 0000 7c00 6a00 a001 7c00 6a02 7c00  ....|.j...|.j.|.
-000003e0: 6a03 a102 5300 a901 4e29 04da 1273 6572  j...S...N)...ser
-000003f0: 6961 6c69 7a65 725f 636c 6173 7365 73da  ializer_classes.
-00000400: 0367 6574 720a 0000 00da 1864 6566 6175  .getr......defau
-00000410: 6c74 5f73 6572 6961 6c69 7a65 725f 636c  lt_serializer_cl
-00000420: 6173 73a9 01da 0473 656c 66a9 0072 2100  ass....self..r!.
-00000430: 0000 fa44 2f55 7365 7273 2f63 7275 7361  ...D/Users/crusa
-00000440: 742f 7072 6f6a 6563 7473 2f67 6172 7069  t/projects/garpi
-00000450: 785f 6361 7274 2f62 6163 6b65 6e64 2f67  x_cart/backend/g
-00000460: 6172 7069 785f 6361 7274 2f76 6965 7773  arpix_cart/views
-00000470: 2f63 6172 742e 7079 da14 6765 745f 7365  /cart.py..get_se
-00000480: 7269 616c 697a 6572 5f63 6c61 7373 2100  rializer_class!.
-00000490: 0000 7302 0000 0000 017a 1d43 6172 7456  ..s......z.CartV
-000004a0: 6965 772e 6765 745f 7365 7269 616c 697a  iew.get_serializ
-000004b0: 6572 5f63 6c61 7373 2901 da06 7265 7475  er_class)...retu
-000004c0: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
-000004d0: 0000 0003 0000 0043 0000 0073 0c00 0000  .......C...s....
-000004e0: 7400 a001 7c00 6a02 a101 5300 721b 0000  t...|.j...S.r...
-000004f0: 0029 0372 0e00 0000 da10 6765 745f 6672  .).r......get_fr
-00000500: 6f6d 5f72 6571 7565 7374 da07 7265 7175  om_request..requ
-00000510: 6573 7472 1f00 0000 7221 0000 0072 2100  estr....r!...r!.
-00000520: 0000 7222 0000 00da 0c67 6574 5f63 7573  ..r".....get_cus
-00000530: 746f 6d65 7224 0000 0073 0200 0000 0001  tomer$...s......
-00000540: 7a15 4361 7274 5669 6577 2e67 6574 5f63  z.CartView.get_c
-00000550: 7573 746f 6d65 7246 6302 0000 0000 0000  ustomerFc.......
-00000560: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
-00000570: 0073 1000 0000 7400 6a01 7c00 6a02 7c01  .s....t.j.|.j.|.
-00000580: 6401 8d02 5300 2902 4e29 0272 2600 0000  d...S.).N).r&...
-00000590: da07 7365 7373 696f 6e29 0372 0e00 0000  ..session).r....
-000005a0: da16 6765 745f 6f72 5f63 7265 6174 655f  ..get_or_create_
-000005b0: 6375 7374 6f6d 6572 7226 0000 0029 0272  customerr&...).r
-000005c0: 2000 0000 7228 0000 0072 2100 0000 7221   ...r(...r!...r!
-000005d0: 0000 0072 2200 0000 7229 0000 0027 0000  ...r"...r)...'..
-000005e0: 0073 0200 0000 0001 7a1f 4361 7274 5669  .s......z.CartVi
-000005f0: 6577 2e67 6574 5f6f 725f 6372 6561 7465  ew.get_or_create
-00000600: 5f63 7573 746f 6d65 7263 0100 0000 0000  _customerc......
-00000610: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00000620: 0000 7316 0000 007c 00a0 00a1 007d 0174  ..s....|.....}.t
-00000630: 016a 026a 037c 0164 018d 0153 0029 024e  .j.j.|.d...S.).N
-00000640: 2901 da08 6375 7374 6f6d 6572 2904 7227  )...customer).r'
-00000650: 0000 0072 0d00 0000 da07 6f62 6a65 6374  ...r......object
-00000660: 73da 0666 696c 7465 7229 0272 2000 0000  s..filter).r ...
-00000670: 722a 0000 0072 2100 0000 7221 0000 0072  r*...r!...r!...r
-00000680: 2200 0000 da0d 6765 745f 6361 7274 6974  ".....get_cartit
-00000690: 656d 732a 0000 0073 0400 0000 0001 0801  ems*...s........
-000006a0: 7a16 4361 7274 5669 6577 2e67 6574 5f63  z.CartView.get_c
-000006b0: 6172 7469 7465 6d73 6303 0000 0000 0000  artitemsc.......
-000006c0: 0000 0000 0005 0000 0007 0000 0043 0000  .............C..
-000006d0: 0073 3600 0000 6700 7d03 7c02 4400 5d1c  .s6...g.}.|.D.].
-000006e0: 7d04 7c03 a000 7401 6600 6401 7c01 6901  }.|...t.f.d.|.i.
-000006f0: 7c04 9702 8e01 a101 0100 7108 7401 6a02  |.........q.t.j.
-00000700: a003 7c03 a101 0100 6400 5300 2902 4e72  ..|.....d.S.).Nr
-00000710: 2a00 0000 2904 da06 6170 7065 6e64 720d  *...)...appendr.
-00000720: 0000 0072 2b00 0000 da0b 6275 6c6b 5f63  ...r+.....bulk_c
-00000730: 7265 6174 6529 0572 2000 0000 722a 0000  reate).r ...r*..
-00000740: 00da 0464 6174 61da 0865 6c65 6d65 6e74  ...data..element
-00000750: 73da 0469 7465 6d72 2100 0000 7221 0000  s..itemr!...r!..
-00000760: 0072 2200 0000 da11 6372 6561 7465 5f63  .r".....create_c
-00000770: 6172 745f 6974 656d 732e 0000 0073 1000  art_items....s..
-00000780: 0000 0001 0401 0801 0a01 02ff 0202 02fe  ................
-00000790: 0a05 7a1a 4361 7274 5669 6577 2e63 7265  ..z.CartView.cre
-000007a0: 6174 655f 6361 7274 5f69 7465 6d73 6302  ate_cart_itemsc.
-000007b0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000007c0: 0000 0043 0000 0073 2000 0000 7c00 a000  ...C...s ...|...
-000007d0: a100 7d02 7401 6a02 6a03 7c02 7c01 6401  ..}.t.j.j.|.|.d.
-000007e0: 8d02 a004 a100 0100 6400 5300 2902 4e29  ........d.S.).N)
-000007f0: 0272 2a00 0000 da06 706b 5f5f 696e 2905  .r*.....pk__in).
-00000800: 7227 0000 0072 0d00 0000 722b 0000 0072  r'...r....r+...r
-00000810: 2c00 0000 da06 6465 6c65 7465 2903 7220  ,.....delete).r 
-00000820: 0000 0072 3000 0000 722a 0000 0072 2100  ...r0...r*...r!.
-00000830: 0000 7221 0000 0072 2200 0000 da11 7265  ..r!...r".....re
-00000840: 6d6f 7665 5f63 6172 745f 6974 656d 7338  move_cart_items8
-00000850: 0000 0073 0400 0000 0001 0801 7a1a 4361  ...s........z.Ca
-00000860: 7274 5669 6577 2e72 656d 6f76 655f 6361  rtView.remove_ca
-00000870: 7274 5f69 7465 6d73 2901 da0a 7061 7261  rt_items)...para
-00000880: 6d65 7465 7273 6302 0000 0000 0000 0000  metersc.........
-00000890: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-000008a0: 1600 0000 7400 7401 7c00 a002 a100 6401  ....t.t.|.....d.
-000008b0: 6402 8d02 6a03 8301 5300 2903 4e54 2901  d...j...S.).NT).
-000008c0: da04 6d61 6e79 2904 720b 0000 0072 1000  ..many).r....r..
-000008d0: 0000 722d 0000 0072 3000 0000 a902 7220  ..r-...r0.....r 
-000008e0: 0000 0072 2600 0000 7221 0000 0072 2100  ...r&...r!...r!.
-000008f0: 0000 7222 0000 00da 046c 6973 743c 0000  ..r".....list<..
-00000900: 0073 0200 0000 0004 7a0d 4361 7274 5669  .s......z.CartVi
-00000910: 6577 2e6c 6973 74da 0450 4f53 5429 03da  ew.list..POST)..
-00000920: 0664 6574 6169 6cda 076d 6574 686f 6473  .detail..methods
-00000930: da12 7065 726d 6973 7369 6f6e 5f63 6c61  ..permission_cla
-00000940: 7373 6573 6302 0000 0000 0000 0000 0000  ssesc...........
-00000950: 0002 0000 0005 0000 0043 0000 0073 1c00  .........C...s..
-00000960: 0000 7400 6401 7401 7c00 a002 a100 8301  ..t.d.t.|.......
-00000970: 6a03 6901 7404 6a05 6402 8d02 5300 2903  j.i.t.j.d...S.).
-00000980: 4e72 2a00 0000 7207 0000 0029 0672 0b00  Nr*...r....).r..
-00000990: 0000 7211 0000 0072 2900 0000 7230 0000  ..r....r)...r0..
-000009a0: 0072 0800 0000 da0b 4854 5450 5f32 3030  .r......HTTP_200
-000009b0: 5f4f 4b72 3900 0000 7221 0000 0072 2100  _OKr9...r!...r!.
-000009c0: 0000 7222 0000 00da 0f63 7265 6174 655f  ..r".....create_
-000009d0: 6375 7374 6f6d 6572 4200 0000 730c 0000  customerB...s...
-000009e0: 0000 0202 0102 000c ff02 0204 fe7a 1843  .............z.C
-000009f0: 6172 7456 6965 772e 6372 6561 7465 5f63  artView.create_c
-00000a00: 7573 746f 6d65 7263 0200 0000 0000 0000  ustomerc........
-00000a10: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-00000a20: 7350 0000 007c 00a0 00a1 007d 027c 016a  sP...|.....}.|.j
-00000a30: 01a0 0264 0164 00a1 027d 037c 0364 006b  ...d.d...}.|.d.k
-00000a40: 0972 3e7c 006a 037c 027c 0364 028d 0201  .r>|.j.|.|.d....
-00000a50: 0074 0464 0364 0469 0174 056a 0664 058d  .t.d.d.i.t.j.d..
-00000a60: 0253 0074 0464 0664 0769 0174 056a 0764  .S.t.d.d.i.t.j.d
-00000a70: 058d 0253 0029 084e 7230 0000 00a9 0272  ...S.).Nr0.....r
-00000a80: 2a00 0000 7230 0000 0072 0800 0000 da02  *...r0...r......
-00000a90: 6f6b 7207 0000 00da 0673 6572 7665 727a  okr......serverz
-00000aa0: 1c52 6571 7565 7374 2022 6461 7461 2220  .Request "data" 
-00000ab0: 6d75 7374 2062 6520 6469 6374 2e29 0872  must be dict.).r
-00000ac0: 2700 0000 7230 0000 0072 1d00 0000 7233  '...r0...r....r3
-00000ad0: 0000 0072 0b00 0000 7208 0000 0072 3f00  ...r....r....r?.
-00000ae0: 0000 da14 4854 5450 5f34 3030 5f42 4144  ....HTTP_400_BAD
-00000af0: 5f52 4551 5545 5354 a904 7220 0000 0072  _REQUEST..r ...r
-00000b00: 2600 0000 722a 0000 0072 3000 0000 7221  &...r*...r0...r!
-00000b10: 0000 0072 2100 0000 7222 0000 0072 1400  ...r!...r"...r..
-00000b20: 0000 4800 0000 731c 0000 0000 0508 010e  ..H...s.........
-00000b30: 0208 010e 0202 0102 0002 ff02 0204 fe06  ................
-00000b40: 0402 0106 0004 ff7a 0c43 6172 7456 6965  .......z.CartVie
-00000b50: 772e 6164 64da 0644 454c 4554 4563 0200  w.add..DELETEc..
-00000b60: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000b70: 0000 4300 0000 7328 0000 007c 016a 00a0  ..C...s(...|.j..
-00000b80: 0164 01a1 017d 027c 00a0 027c 02a1 0101  .d...}.|...|....
-00000b90: 0074 0364 0264 0369 0174 046a 0564 048d  .t.d.d.i.t.j.d..
-00000ba0: 0253 00a9 054e 7230 0000 0072 0800 0000  .S...Nr0...r....
-00000bb0: 7242 0000 0072 0700 0000 a906 7230 0000  rB...r......r0..
-00000bc0: 0072 1d00 0000 7236 0000 0072 0b00 0000  .r....r6...r....
-00000bd0: 7208 0000 0072 3f00 0000 a903 7220 0000  r....r?.....r ..
-00000be0: 0072 2600 0000 7230 0000 0072 2100 0000  .r&...r0...r!...
-00000bf0: 7221 0000 0072 2200 0000 da06 7265 6d6f  r!...r".....remo
-00000c00: 7665 5b00 0000 7310 0000 0000 050c 010a  ve[...s.........
-00000c10: 0102 0102 0002 ff02 0204 fe7a 0f43 6172  ...........z.Car
-00000c20: 7456 6965 772e 7265 6d6f 7665 da03 4745  tView.remove..GE
-00000c30: 5463 0200 0000 0000 0000 0000 0000 0200  Tc..............
-00000c40: 0000 0400 0000 4300 0000 7312 0000 0074  ......C...s....t
-00000c50: 007c 00a0 01a1 0074 026a 0364 018d 0253  .|.....t.j.d...S
-00000c60: 0029 024e 7207 0000 0029 0472 0b00 0000  .).Nr....).r....
-00000c70: 722d 0000 0072 0800 0000 723f 0000 0072  r-...r....r?...r
-00000c80: 3900 0000 7221 0000 0072 2100 0000 7222  9...r!...r!...r"
-00000c90: 0000 00da 0c73 6573 7369 6f6e 5f6c 6973  .....session_lis
-00000ca0: 7466 0000 0073 0800 0000 0005 0201 0600  tf...s..........
-00000cb0: 04ff 7a15 4361 7274 5669 6577 2e73 6573  ..z.CartView.ses
-00000cc0: 7369 6f6e 5f6c 6973 7463 0200 0000 0000  sion_listc......
-00000cd0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00000ce0: 0000 7328 0000 007c 016a 00a0 0164 01a1  ..s(...|.j...d..
-00000cf0: 017d 027c 00a0 027c 02a1 0101 0074 0364  .}.|...|.....t.d
-00000d00: 0264 0369 0174 046a 0564 048d 0253 0072  .d.i.t.j.d...S.r
-00000d10: 4700 0000 7248 0000 0072 4900 0000 7221  G...rH...rI...r!
-00000d20: 0000 0072 2100 0000 7222 0000 00da 0e73  ...r!...r".....s
-00000d30: 6573 7369 6f6e 5f72 656d 6f76 656f 0000  ession_removeo..
-00000d40: 0073 1000 0000 0005 0c01 0a01 0201 0200  .s..............
-00000d50: 02ff 0202 04fe 7a17 4361 7274 5669 6577  ......z.CartView
-00000d60: 2e73 6573 7369 6f6e 5f72 656d 6f76 6563  .session_removec
-00000d70: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000d80: 0400 0000 4300 0000 7354 0000 007c 006a  ....C...sT...|.j
-00000d90: 0064 0164 028d 017d 027c 016a 01a0 0264  .d.d...}.|.j...d
-00000da0: 0364 00a1 027d 037c 0364 006b 0972 427c  .d...}.|.d.k.rB|
-00000db0: 006a 037c 027c 0364 048d 0201 0074 0464  .j.|.|.d.....t.d
-00000dc0: 0564 0669 0174 056a 0664 078d 0253 0074  .d.i.t.j.d...S.t
-00000dd0: 0464 0864 0969 0174 056a 0764 078d 0253  .d.d.i.t.j.d...S
-00000de0: 0029 0a4e 5429 0172 2800 0000 7230 0000  .).NT).r(...r0..
-00000df0: 0072 4100 0000 7243 0000 007a 1b50 726f  .rA...rC...z.Pro
-00000e00: 6475 6374 2061 6464 6564 2073 7563 6365  duct added succe
-00000e10: 7373 6675 6c6c 792e 7207 0000 00da 0565  ssfully.r......e
-00000e20: 7272 6f72 7a0e 4461 7461 206e 6f74 2076  rrorz.Data not v
-00000e30: 616c 6964 2908 7229 0000 0072 3000 0000  alid).r)...r0...
-00000e40: 721d 0000 0072 3300 0000 720b 0000 0072  r....r3...r....r
-00000e50: 0800 0000 723f 0000 0072 4400 0000 7245  ....r?...rD...rE
-00000e60: 0000 0072 2100 0000 7221 0000 0072 2200  ...r!...r!...r".
-00000e70: 0000 7215 0000 007a 0000 0073 1800 0000  ..r....z...s....
-00000e80: 0005 0c01 0e02 0801 0e02 0201 0600 04ff  ................
-00000e90: 0604 0201 0600 04ff 7a14 4361 7274 5669  ........z.CartVi
-00000ea0: 6577 2e73 6573 7369 6f6e 5f61 6464 4e63  ew.session_addNc
-00000eb0: 0300 0000 0000 0000 0000 0000 0600 0000  ................
-00000ec0: 0400 0000 4300 0000 735a 0000 007c 00a0  ....C...sZ...|..
-00000ed0: 00a1 007d 0374 016a 026a 037c 037c 0264  ...}.t.j.j.|.|.d
-00000ee0: 018d 027d 047c 04a0 04a1 0064 026b 0272  ...}.|.....d.k.r
-00000ef0: 3074 0574 066a 0764 038d 0153 007c 016a  0t.t.j.d...S.|.j
-00000f00: 08a0 0964 04a1 017d 057c 046a 0a66 007c  ...d...}.|.j.f.|
-00000f10: 058e 0101 0074 0564 0564 0669 0174 066a  .....t.d.d.i.t.j
-00000f20: 0b64 038d 0253 0029 074e 2902 722a 0000  .d...S.).N).r*..
-00000f30: 00da 0270 6b72 0100 0000 7207 0000 0072  ...pkr....r....r
-00000f40: 3000 0000 7208 0000 0072 4200 0000 290c  0...r....rB...).
-00000f50: 7227 0000 0072 0d00 0000 722b 0000 0072  r'...r....r+...r
-00000f60: 2c00 0000 da05 636f 756e 7472 0b00 0000  ,.....countr....
-00000f70: 7208 0000 00da 1248 5454 505f 3430 345f  r......HTTP_404_
-00000f80: 4e4f 545f 464f 554e 4472 3000 0000 721d  NOT_FOUNDr0...r.
-00000f90: 0000 00da 0675 7064 6174 6572 3f00 0000  .....updater?...
-00000fa0: 2906 7220 0000 0072 2600 0000 724f 0000  ).r ...r&...rO..
-00000fb0: 0072 2a00 0000 5a09 6361 7274 5f69 7465  .r*...Z.cart_ite
-00000fc0: 6d72 3000 0000 7221 0000 0072 2100 0000  mr0...r!...r!...
-00000fd0: 7222 0000 00da 0e70 6172 7469 616c 5f75  r".....partial_u
-00000fe0: 7064 6174 658d 0000 0073 1800 0000 0004  pdate....s......
-00000ff0: 0802 1002 0c01 0c02 0c02 0c02 0201 0200  ................
-00001000: 02ff 0202 04fe 7a17 4361 7274 5669 6577  ......z.CartView
-00001010: 2e70 6172 7469 616c 5f75 7064 6174 6529  .partial_update)
-00001020: 0146 2901 4e29 25da 085f 5f6e 616d 655f  .F).N)%..__name_
-00001030: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00001040: 5f71 7561 6c6e 616d 655f 5f72 0500 0000  _qualname__r....
-00001050: da0a 4a53 4f4e 5061 7273 6572 da0e 7061  ..JSONParser..pa
-00001060: 7273 6572 5f63 6c61 7373 6573 7206 0000  rser_classesr...
-00001070: 00da 0841 6c6c 6f77 416e 7972 3e00 0000  ...AllowAnyr>...
-00001080: 7212 0000 0072 1c00 0000 7204 0000 0072  r....r....r....r
-00001090: 0e00 0000 da09 4845 4144 5f4e 414d 45da  ......HEAD_NAME.
-000010a0: 0373 7472 da06 4845 4144 4552 5a10 6865  .str..HEADERZ.he
-000010b0: 6164 6572 5f70 6172 616d 6574 6572 7210  ader_parameterr.
-000010c0: 0000 0072 1e00 0000 7223 0000 0072 0200  ...r....r#...r..
-000010d0: 0000 7227 0000 0072 2900 0000 722d 0000  ..r'...r)...r-..
-000010e0: 0072 3300 0000 7236 0000 0072 0300 0000  .r3...r6...r....
-000010f0: 723a 0000 0072 0a00 0000 7240 0000 0072  r:...r....r@...r
-00001100: 0f00 0000 7214 0000 0072 4a00 0000 724c  ....r....rJ...rL
-00001110: 0000 0072 4d00 0000 7215 0000 0072 5300  ...rM...r....rS.
-00001120: 0000 7221 0000 0072 2100 0000 7221 0000  ..r!...r!...r!..
-00001130: 0072 2200 0000 7213 0000 0010 0000 0073  .r"...r........s
-00001140: 6c00 0000 0801 0801 0802 0201 02fe 0604  l...............
-00001150: 0201 0401 0201 0201 0201 04fb 0608 0402  ................
-00001160: 0803 1203 0a03 0804 080a 0804 0201 04ff  ................
-00001170: 0403 0a03 1201 0a05 0201 04ff 0403 1001  ................
-00001180: 0c0f 0201 04ff 0403 1001 0c07 0201 04ff  ................
-00001190: 0403 1201 0c05 0201 04ff 0403 1001 0c07  ................
-000011a0: 0201 04ff 0403 1201 0c0f 0201 04ff 0403  ................
-000011b0: 7213 0000 004e 2918 da06 7479 7069 6e67  r....N)...typing
-000011c0: 7202 0000 00da 1564 7266 5f73 7065 6374  r......drf_spect
-000011d0: 6163 756c 6172 2e75 7469 6c73 7203 0000  acular.utilsr...
-000011e0: 0072 0400 0000 da0e 7265 7374 5f66 7261  .r......rest_fra
-000011f0: 6d65 776f 726b 7205 0000 0072 0600 0000  meworkr....r....
-00001200: 7208 0000 0072 0900 0000 da19 7265 7374  r....r......rest
-00001210: 5f66 7261 6d65 776f 726b 2e64 6563 6f72  _framework.decor
-00001220: 6174 6f72 7372 0a00 0000 da17 7265 7374  atorsr......rest
-00001230: 5f66 7261 6d65 776f 726b 2e72 6573 706f  _framework.respo
-00001240: 6e73 6572 0b00 0000 da06 6d6f 6465 6c73  nser......models
-00001250: 720d 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00001260: 0b73 6572 6961 6c69 7a65 7273 7210 0000  .serializersr...
-00001270: 0072 1100 0000 7212 0000 00da 0756 6965  .r....r......Vie
-00001280: 7753 6574 7213 0000 0072 2100 0000 7221  wSetr....r!...r!
-00001290: 0000 0072 2100 0000 7222 0000 00da 083c  ...r!...r".....<
-000012a0: 6d6f 6475 6c65 3e01 0000 0073 1600 0000  module>....s....
-000012b0: 0c02 1001 0c01 0c01 0c01 0c01 0c01 0c02  ................
-000012c0: 1001 0c01 1403                           ......
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c08  d.l.m.Z...d.d.l.
+00000070: 6d0a 5a0a 0100 6400 6407 6c08 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000080: 0100 6400 6408 6c08 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
+00000090: 6409 6c0d 6d0e 5a0e 0100 6400 640a 6c0f  d.l.m.Z...d.d.l.
+000000a0: 6d10 5a10 0100 640b 640c 6c11 6d12 5a12  m.Z...d.d.l.m.Z.
+000000b0: 0100 640b 640d 6c0a 6d13 5a13 0100 640b  ..d.d.l.m.Z...d.
+000000c0: 640e 6c14 6d15 5a15 6d16 5a16 0100 6503  d.l.m.Z.m.Z...e.
+000000d0: 6507 8300 6701 640f 8d01 4700 6410 6411  e...g.d...G.d.d.
+000000e0: 8400 6411 650c 6a17 8303 8301 5a18 6412  ..d.e.j.....Z.d.
+000000f0: 5300 2913 e900 0000 0029 01da 084f 7074  S.)......)...Opt
+00000100: 696f 6e61 6c29 01da 0d65 7874 656e 645f  ional)...extend_
+00000110: 7363 6865 6d61 2901 da0b 5573 6572 5365  schema)...UserSe
+00000120: 7373 696f 6e29 01da 2375 7365 725f 7365  ssion)..#user_se
+00000130: 7373 696f 6e5f 746f 6b65 6e5f 6865 6164  ssion_token_head
+00000140: 6572 5f70 6172 616d 6574 6572 2901 da07  er_parameter)...
+00000150: 7061 7273 6572 7329 01da 0b70 6572 6d69  parsers)...permi
+00000160: 7373 696f 6e73 a901 da06 7374 6174 7573  ssions....status
+00000170: 2901 da08 7669 6577 7365 7473 2901 da06  )...viewsets)...
+00000180: 6163 7469 6f6e 2901 da08 5265 7370 6f6e  action)...Respon
+00000190: 7365 e902 0000 0029 01da 0843 6172 7449  se.....)...CartI
+000001a0: 7465 6d29 01da 0a49 7343 7573 746f 6d65  tem)...IsCustome
+000001b0: 7229 02da 1243 6172 7449 7465 6d53 6572  r)...CartItemSer
+000001c0: 6961 6c69 7a65 72da 1643 6172 7449 7465  ializer..CartIte
+000001d0: 6d4c 6973 7453 6572 6961 6c69 7a65 7229  mListSerializer)
+000001e0: 01da 0a70 6172 616d 6574 6572 7363 0000  ...parametersc..
+000001f0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
+00000200: 0000 4000 0000 73fe 0000 0065 005a 0164  ..@...s....e.Z.d
+00000210: 005a 0265 036a 0466 015a 0565 066a 0766  .Z.e.j.f.Z.e.j.f
+00000220: 015a 0865 0965 0964 019c 025a 0a65 0b5a  .Z.e.e.d...Z.e.Z
+00000230: 0c64 0264 0384 005a 0d65 0e65 0f19 0064  .d.d...Z.e.e...d
+00000240: 049c 0164 0564 0684 045a 1064 2364 0864  ...d.d...Z.d#d.d
+00000250: 0984 015a 1164 0a64 0b84 005a 1264 0c64  ...Z.d.d...Z.d.d
+00000260: 0d84 005a 1364 0e64 0f84 005a 1464 1064  ...Z.d.d...Z.d.d
+00000270: 1184 005a 1565 1664 0764 1267 0165 1766  ...Z.e.d.d.g.e.f
+00000280: 0164 138d 0364 1464 1584 0083 015a 1865  .d...d.d.....Z.e
+00000290: 1664 0764 1667 0165 1766 0164 138d 0364  .d.d.g.e.f.d...d
+000002a0: 1764 1884 0083 015a 1965 1664 0764 1967  .d.....Z.e.d.d.g
+000002b0: 0165 066a 0766 0164 138d 0364 1a64 1b84  .e.j.f.d...d.d..
+000002c0: 0083 015a 1a65 1664 0764 1667 0165 1766  ...Z.e.d.d.g.e.f
+000002d0: 0164 138d 0364 1c64 1d84 0083 015a 1b65  .d...d.d.....Z.e
+000002e0: 1664 0764 1267 0165 066a 0766 0164 138d  .d.d.g.e.j.f.d..
+000002f0: 0364 1e64 1f84 0083 015a 1c64 2464 2164  .d.d.....Z.d$d!d
+00000300: 2284 015a 1d64 2053 0029 25da 0843 6172  "..Z.d S.)%..Car
+00000310: 7456 6965 7729 02da 0361 6464 da0b 7365  tView)...add..se
+00000320: 7373 696f 6e5f 6164 6463 0100 0000 0000  ssion_addc......
+00000330: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00000340: 0000 7312 0000 007c 006a 00a0 017c 006a  ..s....|.j...|.j
+00000350: 027c 006a 03a1 0253 00a9 014e 2904 da12  .|.j...S...N)...
+00000360: 7365 7269 616c 697a 6572 5f63 6c61 7373  serializer_class
+00000370: 6573 da03 6765 7472 0b00 0000 da18 6465  es..getr......de
+00000380: 6661 756c 745f 7365 7269 616c 697a 6572  fault_serializer
+00000390: 5f63 6c61 7373 a901 da04 7365 6c66 a900  _class....self..
+000003a0: 721c 0000 00fa 4c2f 5573 6572 732f 7669  r.....L/Users/vi
+000003b0: 6b74 6f72 6961 7265 7365 746f 7661 2f47  ktoriaresetova/G
+000003c0: 4152 5049 582f 6761 7270 6978 5f63 6172  ARPIX/garpix_car
+000003d0: 742f 6261 636b 656e 642f 6761 7270 6978  t/backend/garpix
+000003e0: 5f63 6172 742f 7669 6577 732f 6361 7274  _cart/views/cart
+000003f0: 2e70 79da 1467 6574 5f73 6572 6961 6c69  .py..get_seriali
+00000400: 7a65 725f 636c 6173 7321 0000 0073 0200  zer_class!...s..
+00000410: 0000 0001 7a1d 4361 7274 5669 6577 2e67  ....z.CartView.g
+00000420: 6574 5f73 6572 6961 6c69 7a65 725f 636c  et_serializer_cl
+00000430: 6173 7329 01da 0672 6574 7572 6e63 0100  ass)...returnc..
+00000440: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000450: 0000 4300 0000 730c 0000 0074 00a0 017c  ..C...s....t...|
+00000460: 006a 02a1 0153 0072 1600 0000 2903 7204  .j...S.r....).r.
+00000470: 0000 00da 1067 6574 5f66 726f 6d5f 7265  .....get_from_re
+00000480: 7175 6573 74da 0772 6571 7565 7374 721a  quest..requestr.
+00000490: 0000 0072 1c00 0000 721c 0000 0072 1d00  ...r....r....r..
+000004a0: 0000 da0c 6765 745f 6375 7374 6f6d 6572  ....get_customer
+000004b0: 2400 0000 7302 0000 0000 017a 1543 6172  $...s......z.Car
+000004c0: 7456 6965 772e 6765 745f 6375 7374 6f6d  tView.get_custom
+000004d0: 6572 4663 0200 0000 0000 0000 0000 0000  erFc............
+000004e0: 0200 0000 0400 0000 4300 0000 7310 0000  ........C...s...
+000004f0: 0074 006a 017c 006a 027c 0164 018d 0253  .t.j.|.j.|.d...S
+00000500: 0029 024e 2902 7221 0000 00da 0773 6573  .).N).r!.....ses
+00000510: 7369 6f6e 2903 7204 0000 00da 1a67 6574  sion).r......get
+00000520: 5f6f 725f 6372 6561 7465 5f75 7365 725f  _or_create_user_
+00000530: 7365 7373 696f 6e72 2100 0000 2902 721b  sessionr!...).r.
+00000540: 0000 0072 2300 0000 721c 0000 0072 1c00  ...r#...r....r..
+00000550: 0000 721d 0000 00da 1667 6574 5f6f 725f  ..r......get_or_
+00000560: 6372 6561 7465 5f63 7573 746f 6d65 7227  create_customer'
+00000570: 0000 0073 0200 0000 0001 7a1f 4361 7274  ...s......z.Cart
+00000580: 5669 6577 2e67 6574 5f6f 725f 6372 6561  View.get_or_crea
+00000590: 7465 5f63 7573 746f 6d65 7263 0100 0000  te_customerc....
+000005a0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000005b0: 4300 0000 7316 0000 007c 00a0 00a1 007d  C...s....|.....}
+000005c0: 0174 016a 026a 037c 0164 018d 0153 0029  .t.j.j.|.d...S.)
+000005d0: 024e 2901 da08 6375 7374 6f6d 6572 2904  .N)...customer).
+000005e0: 7222 0000 0072 0e00 0000 da07 6f62 6a65  r"...r......obje
+000005f0: 6374 73da 0666 696c 7465 7229 0272 1b00  cts..filter).r..
+00000600: 0000 7226 0000 0072 1c00 0000 721c 0000  ..r&...r....r...
+00000610: 0072 1d00 0000 da0d 6765 745f 6361 7274  .r......get_cart
+00000620: 6974 656d 732a 0000 0073 0400 0000 0001  items*...s......
+00000630: 0801 7a16 4361 7274 5669 6577 2e67 6574  ..z.CartView.get
+00000640: 5f63 6172 7469 7465 6d73 6303 0000 0000  _cartitemsc.....
+00000650: 0000 0000 0000 0005 0000 0007 0000 0043  ...............C
+00000660: 0000 0073 3600 0000 6700 7d03 7c02 4400  ...s6...g.}.|.D.
+00000670: 5d1c 7d04 7c03 a000 7401 6600 6401 7c01  ].}.|...t.f.d.|.
+00000680: 6901 7c04 9702 8e01 a101 0100 7108 7401  i.|.........q.t.
+00000690: 6a02 a003 7c03 a101 0100 6400 5300 2902  j...|.....d.S.).
+000006a0: 4e72 2600 0000 2904 da06 6170 7065 6e64  Nr&...)...append
+000006b0: 720e 0000 0072 2700 0000 da0b 6275 6c6b  r....r'.....bulk
+000006c0: 5f63 7265 6174 6529 0572 1b00 0000 7226  _create).r....r&
+000006d0: 0000 00da 0464 6174 61da 0865 6c65 6d65  .....data..eleme
+000006e0: 6e74 73da 0469 7465 6d72 1c00 0000 721c  nts..itemr....r.
+000006f0: 0000 0072 1d00 0000 da11 6372 6561 7465  ...r......create
+00000700: 5f63 6172 745f 6974 656d 732e 0000 0073  _cart_items....s
+00000710: 1000 0000 0001 0401 0801 0a01 02ff 0202  ................
+00000720: 02fe 0a05 7a1a 4361 7274 5669 6577 2e63  ....z.CartView.c
+00000730: 7265 6174 655f 6361 7274 5f69 7465 6d73  reate_cart_items
+00000740: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000750: 0004 0000 0043 0000 0073 2000 0000 7c00  .....C...s ...|.
+00000760: a000 a100 7d02 7401 6a02 6a03 7c02 7c01  ....}.t.j.j.|.|.
+00000770: 6401 8d02 a004 a100 0100 6400 5300 2902  d.........d.S.).
+00000780: 4e29 0272 2600 0000 da06 706b 5f5f 696e  N).r&.....pk__in
+00000790: 2905 7222 0000 0072 0e00 0000 7227 0000  ).r"...r....r'..
+000007a0: 0072 2800 0000 da06 6465 6c65 7465 2903  .r(.....delete).
+000007b0: 721b 0000 0072 2c00 0000 7226 0000 0072  r....r,...r&...r
+000007c0: 1c00 0000 721c 0000 0072 1d00 0000 da11  ....r....r......
+000007d0: 7265 6d6f 7665 5f63 6172 745f 6974 656d  remove_cart_item
+000007e0: 7338 0000 0073 0400 0000 0001 0801 7a1a  s8...s........z.
+000007f0: 4361 7274 5669 6577 2e72 656d 6f76 655f  CartView.remove_
+00000800: 6361 7274 5f69 7465 6d73 6302 0000 0000  cart_itemsc.....
+00000810: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00000820: 0000 0073 1600 0000 7400 7401 7c00 a002  ...s....t.t.|...
+00000830: a100 6401 6402 8d02 6a03 8301 5300 2903  ..d.d...j...S.).
+00000840: 4e54 2901 da04 6d61 6e79 2904 720c 0000  NT)...many).r...
+00000850: 0072 1000 0000 7229 0000 0072 2c00 0000  .r....r)...r,...
+00000860: a902 721b 0000 0072 2100 0000 721c 0000  ..r....r!...r...
+00000870: 0072 1c00 0000 721d 0000 00da 046c 6973  .r....r......lis
+00000880: 743c 0000 0073 0200 0000 0001 7a0d 4361  t<...s......z.Ca
+00000890: 7274 5669 6577 2e6c 6973 74da 0450 4f53  rtView.list..POS
+000008a0: 5429 03da 0664 6574 6169 6cda 076d 6574  T)...detail..met
+000008b0: 686f 6473 da12 7065 726d 6973 7369 6f6e  hods..permission
+000008c0: 5f63 6c61 7373 6573 6302 0000 0000 0000  _classesc.......
+000008d0: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+000008e0: 0073 5000 0000 7c00 a000 a100 7d02 7c01  .sP...|.....}.|.
+000008f0: 6a01 a002 6401 6400 a102 7d03 7c03 6400  j...d.d...}.|.d.
+00000900: 6b09 723e 7c00 6a03 7c02 7c03 6402 8d02  k.r>|.j.|.|.d...
+00000910: 0100 7404 6403 6404 6901 7405 6a06 6405  ..t.d.d.i.t.j.d.
+00000920: 8d02 5300 7404 6406 6407 6901 7405 6a07  ..S.t.d.d.i.t.j.
+00000930: 6405 8d02 5300 2908 4e72 2c00 0000 a902  d...S.).Nr,.....
+00000940: 7226 0000 0072 2c00 0000 7209 0000 00da  r&...r,...r.....
+00000950: 026f 6b72 0800 0000 da06 7365 7276 6572  .okr......server
+00000960: 7a1c 5265 7175 6573 7420 2264 6174 6122  z.Request "data"
+00000970: 206d 7573 7420 6265 2064 6963 742e 2908   must be dict.).
+00000980: 7222 0000 0072 2c00 0000 7218 0000 0072  r"...r,...r....r
+00000990: 2f00 0000 720c 0000 0072 0900 0000 da0b  /...r....r......
+000009a0: 4854 5450 5f32 3030 5f4f 4bda 1448 5454  HTTP_200_OK..HTT
+000009b0: 505f 3430 305f 4241 445f 5245 5155 4553  P_400_BAD_REQUES
+000009c0: 54a9 0472 1b00 0000 7221 0000 0072 2600  T..r....r!...r&.
+000009d0: 0000 722c 0000 0072 1c00 0000 721c 0000  ..r,...r....r...
+000009e0: 0072 1d00 0000 7214 0000 003f 0000 0073  .r....r....?...s
+000009f0: 1c00 0000 0002 0801 0e02 0801 0e02 0201  ................
+00000a00: 0200 02ff 0202 04fe 0604 0201 0600 04ff  ................
+00000a10: 7a0c 4361 7274 5669 6577 2e61 6464 da06  z.CartView.add..
+00000a20: 4445 4c45 5445 6302 0000 0000 0000 0000  DELETEc.........
+00000a30: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00000a40: 2800 0000 7c01 6a00 a001 6401 a101 7d02  (...|.j...d...}.
+00000a50: 7c00 a002 7c02 a101 0100 7403 6402 6403  |...|.....t.d.d.
+00000a60: 6901 7404 6a05 6404 8d02 5300 a905 4e72  i.t.j.d...S...Nr
+00000a70: 2c00 0000 7209 0000 0072 3b00 0000 7208  ,...r....r;...r.
+00000a80: 0000 00a9 0672 2c00 0000 7218 0000 0072  .....r,...r....r
+00000a90: 3200 0000 720c 0000 0072 0900 0000 723d  2...r....r....r=
+00000aa0: 0000 00a9 0372 1b00 0000 7221 0000 0072  .....r....r!...r
+00000ab0: 2c00 0000 721c 0000 0072 1c00 0000 721d  ,...r....r....r.
+00000ac0: 0000 00da 0672 656d 6f76 654f 0000 0073  .....removeO...s
+00000ad0: 1000 0000 0002 0c01 0a01 0201 0200 02ff  ................
+00000ae0: 0202 04fe 7a0f 4361 7274 5669 6577 2e72  ....z.CartView.r
+00000af0: 656d 6f76 65da 0347 4554 6302 0000 0000  emove..GETc.....
+00000b00: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000b10: 0000 0073 1200 0000 7400 7c00 a001 a100  ...s....t.|.....
+00000b20: 7402 6a03 6401 8d02 5300 2902 4e72 0800  t.j.d...S.).Nr..
+00000b30: 0000 2904 720c 0000 0072 2900 0000 7209  ..).r....r)...r.
+00000b40: 0000 0072 3d00 0000 7234 0000 0072 1c00  ...r=...r4...r..
+00000b50: 0000 721c 0000 0072 1d00 0000 da0c 7365  ..r....r......se
+00000b60: 7373 696f 6e5f 6c69 7374 5700 0000 7308  ssion_listW...s.
+00000b70: 0000 0000 0202 0106 0004 ff7a 1543 6172  ...........z.Car
+00000b80: 7456 6965 772e 7365 7373 696f 6e5f 6c69  tView.session_li
+00000b90: 7374 6302 0000 0000 0000 0000 0000 0003  stc.............
+00000ba0: 0000 0004 0000 0043 0000 0073 2800 0000  .......C...s(...
+00000bb0: 7c01 6a00 a001 6401 a101 7d02 7c00 a002  |.j...d...}.|...
+00000bc0: 7c02 a101 0100 7403 6402 6403 6901 7404  |.....t.d.d.i.t.
+00000bd0: 6a05 6404 8d02 5300 7241 0000 0072 4200  j.d...S.rA...rB.
+00000be0: 0000 7243 0000 0072 1c00 0000 721c 0000  ..rC...r....r...
+00000bf0: 0072 1d00 0000 da0e 7365 7373 696f 6e5f  .r......session_
+00000c00: 7265 6d6f 7665 5d00 0000 7310 0000 0000  remove]...s.....
+00000c10: 020c 010a 0102 0102 0002 ff02 0204 fe7a  ...............z
+00000c20: 1743 6172 7456 6965 772e 7365 7373 696f  .CartView.sessio
+00000c30: 6e5f 7265 6d6f 7665 6302 0000 0000 0000  n_removec.......
+00000c40: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+00000c50: 0073 5400 0000 7c00 6a00 6401 6402 8d01  .sT...|.j.d.d...
+00000c60: 7d02 7c01 6a01 a002 6403 6400 a102 7d03  }.|.j...d.d...}.
+00000c70: 7c03 6400 6b09 7242 7c00 6a03 7c02 7c03  |.d.k.rB|.j.|.|.
+00000c80: 6404 8d02 0100 7404 6405 6406 6901 7405  d.....t.d.d.i.t.
+00000c90: 6a06 6407 8d02 5300 7404 6408 6409 6901  j.d...S.t.d.d.i.
+00000ca0: 7405 6a07 6407 8d02 5300 290a 4e54 2901  t.j.d...S.).NT).
+00000cb0: 7223 0000 0072 2c00 0000 723a 0000 0072  r#...r,...r:...r
+00000cc0: 3c00 0000 7a1b 5072 6f64 7563 7420 6164  <...z.Product ad
+00000cd0: 6465 6420 7375 6363 6573 7366 756c 6c79  ded successfully
+00000ce0: 2e72 0800 0000 da05 6572 726f 727a 0e44  .r......errorz.D
+00000cf0: 6174 6120 6e6f 7420 7661 6c69 6429 0872  ata not valid).r
+00000d00: 2500 0000 722c 0000 0072 1800 0000 722f  %...r,...r....r/
+00000d10: 0000 0072 0c00 0000 7209 0000 0072 3d00  ...r....r....r=.
+00000d20: 0000 723e 0000 0072 3f00 0000 721c 0000  ..r>...r?...r...
+00000d30: 0072 1c00 0000 721d 0000 0072 1500 0000  .r....r....r....
+00000d40: 6500 0000 7318 0000 0000 020c 010e 0208  e...s...........
+00000d50: 010e 0202 0106 0004 ff06 0402 0106 0004  ................
+00000d60: ff7a 1443 6172 7456 6965 772e 7365 7373  .z.CartView.sess
+00000d70: 696f 6e5f 6164 644e 6303 0000 0000 0000  ion_addNc.......
+00000d80: 0000 0000 0006 0000 0004 0000 0043 0000  .............C..
+00000d90: 0073 5a00 0000 7c00 a000 a100 7d03 7401  .sZ...|.....}.t.
+00000da0: 6a02 6a03 7c03 7c02 6401 8d02 7d04 7c04  j.j.|.|.d...}.|.
+00000db0: a004 a100 6402 6b02 7230 7405 7406 6a07  ....d.k.r0t.t.j.
+00000dc0: 6403 8d01 5300 7c01 6a08 a009 6404 a101  d...S.|.j...d...
+00000dd0: 7d05 7c04 6a0a 6600 7c05 8e01 0100 7405  }.|.j.f.|.....t.
+00000de0: 6405 6406 6901 7406 6a0b 6403 8d02 5300  d.d.i.t.j.d...S.
+00000df0: 2907 4e29 0272 2600 0000 da02 706b 7201  ).N).r&.....pkr.
+00000e00: 0000 0072 0800 0000 722c 0000 0072 0900  ...r....r,...r..
+00000e10: 0000 723b 0000 0029 0c72 2200 0000 720e  ..r;...).r"...r.
+00000e20: 0000 0072 2700 0000 7228 0000 00da 0563  ...r'...r(.....c
+00000e30: 6f75 6e74 720c 0000 0072 0900 0000 da12  ountr....r......
+00000e40: 4854 5450 5f34 3034 5f4e 4f54 5f46 4f55  HTTP_404_NOT_FOU
+00000e50: 4e44 722c 0000 0072 1800 0000 da06 7570  NDr,...r......up
+00000e60: 6461 7465 723d 0000 0029 0672 1b00 0000  dater=...).r....
+00000e70: 7221 0000 0072 4900 0000 7226 0000 005a  r!...rI...r&...Z
+00000e80: 0963 6172 745f 6974 656d 722c 0000 0072  .cart_itemr,...r
+00000e90: 1c00 0000 721c 0000 0072 1d00 0000 da0e  ....r....r......
+00000ea0: 7061 7274 6961 6c5f 7570 6461 7465 7500  partial_updateu.
+00000eb0: 0000 7318 0000 0000 0108 0210 020c 010c  ..s.............
+00000ec0: 020c 020c 0202 0102 0002 ff02 0204 fe7a  ...............z
+00000ed0: 1743 6172 7456 6965 772e 7061 7274 6961  .CartView.partia
+00000ee0: 6c5f 7570 6461 7465 2901 4629 014e 291e  l_update).F).N).
+00000ef0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000f00: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000f10: 6d65 5f5f 7206 0000 00da 0a4a 534f 4e50  me__r......JSONP
+00000f20: 6172 7365 72da 0e70 6172 7365 725f 636c  arser..parser_cl
+00000f30: 6173 7365 7372 0700 0000 da08 416c 6c6f  assesr......Allo
+00000f40: 7741 6e79 7239 0000 0072 1100 0000 7217  wAnyr9...r....r.
+00000f50: 0000 0072 1000 0000 7219 0000 0072 1e00  ...r....r....r..
+00000f60: 0000 7202 0000 0072 0400 0000 7222 0000  ..r....r....r"..
+00000f70: 0072 2500 0000 7229 0000 0072 2f00 0000  .r%...r)...r/...
+00000f80: 7232 0000 0072 3500 0000 720b 0000 0072  r2...r5...r....r
+00000f90: 0f00 0000 7214 0000 0072 4400 0000 7246  ....r....rD...rF
+00000fa0: 0000 0072 4700 0000 7215 0000 0072 4d00  ...rG...r....rM.
+00000fb0: 0000 721c 0000 0072 1c00 0000 721c 0000  ..r....r....r...
+00000fc0: 0072 1d00 0000 7213 0000 0012 0000 0073  .r....r........s
+00000fd0: 3000 0000 0806 0801 0802 0201 02fe 0605  0...............
+00000fe0: 0402 0803 1203 0a03 0804 080a 0804 0803  ................
+00000ff0: 1001 0a0f 1001 0a07 1201 0a05 1001 0a07  ................
+00001000: 1201 0a0f 7213 0000 004e 2919 da06 7479  ....r....N)...ty
+00001010: 7069 6e67 7202 0000 00da 1564 7266 5f73  pingr......drf_s
+00001020: 7065 6374 6163 756c 6172 2e75 7469 6c73  pectacular.utils
+00001030: 7203 0000 00da 1267 6172 7069 785f 7573  r......garpix_us
+00001040: 6572 2e6d 6f64 656c 7372 0400 0000 da21  er.modelsr.....!
+00001050: 6761 7270 6978 5f75 7365 722e 7574 696c  garpix_user.util
+00001060: 732e 6472 665f 7370 6563 7461 6375 6c61  s.drf_spectacula
+00001070: 7272 0500 0000 da0e 7265 7374 5f66 7261  rr......rest_fra
+00001080: 6d65 776f 726b 7206 0000 0072 0700 0000  meworkr....r....
+00001090: 7209 0000 0072 0a00 0000 da19 7265 7374  r....r......rest
+000010a0: 5f66 7261 6d65 776f 726b 2e64 6563 6f72  _framework.decor
+000010b0: 6174 6f72 7372 0b00 0000 da17 7265 7374  atorsr......rest
+000010c0: 5f66 7261 6d65 776f 726b 2e72 6573 706f  _framework.respo
+000010d0: 6e73 6572 0c00 0000 da06 6d6f 6465 6c73  nser......models
+000010e0: 720e 0000 0072 0f00 0000 da0b 7365 7269  r....r......seri
+000010f0: 616c 697a 6572 7372 1000 0000 7211 0000  alizersr....r...
+00001100: 00da 0756 6965 7753 6574 7213 0000 0072  ...ViewSetr....r
+00001110: 1c00 0000 721c 0000 0072 1c00 0000 721d  ....r....r....r.
+00001120: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001130: 0073 2200 0000 0c02 0c01 0c01 0c01 0c01  .s".............
+00001140: 0c01 0c01 0c01 0c01 0c02 0c01 0c01 1003  ................
+00001150: 0202 04ff 02ff 0405                      ........
```

### Comparing `garpix_cart-2.2.0/garpix_cart/views/cart.py` & `garpix_cart-3.0.0/garpix_cart/views/cart.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from typing import Optional
 
-from drf_spectacular.utils import extend_schema, OpenApiParameter
+from drf_spectacular.utils import extend_schema
+from garpix_user.models import UserSession
+from garpix_user.utils.drf_spectacular import user_session_token_header_parameter
 from rest_framework import parsers
 from rest_framework import permissions
 from rest_framework import status
 from rest_framework import viewsets
 from rest_framework.decorators import action
 from rest_framework.response import Response
 
-from ..models import CartItem, Customer
+from ..models import CartItem
 from ..permissions import IsCustomer
-from ..serializers import CartItemSerializer, CustomerSerializer, CartItemListSerializer
+from ..serializers import CartItemSerializer, CartItemListSerializer
 
 
+@extend_schema(
+    parameters=[
+        user_session_token_header_parameter()
+    ]
+)
 class CartView(viewsets.ViewSet):
     parser_classes = (parsers.JSONParser,)
     permission_classes = (permissions.AllowAny,)
     serializer_classes = {
         'add': CartItemListSerializer,
         'session_add': CartItemListSerializer
     }
-    header_parameter = OpenApiParameter(
-        name=Customer.HEAD_NAME,
-        description='Customer',
-        required=True,
-        type=str,
-        location=OpenApiParameter.HEADER
-    )
 
     default_serializer_class = CartItemSerializer
 
     def get_serializer_class(self):
         return self.serializer_classes.get(self.action, self.default_serializer_class)
 
-    def get_customer(self) -> Optional[Customer]:
-        return Customer.get_from_request(self.request)
+    def get_customer(self) -> Optional[UserSession]:
+        return UserSession.get_from_request(self.request)
 
     def get_or_create_customer(self, session=False):
-        return Customer.get_or_create_customer(request=self.request, session=session)
+        return UserSession.get_or_create_user_session(request=self.request, session=session)
 
     def get_cartitems(self):
         customer = self.get_customer()
         return CartItem.objects.filter(customer=customer)
 
     def create_cart_items(self, customer, data):
         elements = []
@@ -53,29 +53,17 @@
 
         CartItem.objects.bulk_create(elements)
 
     def remove_cart_items(self, data):
         customer = self.get_customer()
         CartItem.objects.filter(customer=customer, pk__in=data).delete()
 
-    @extend_schema(
-        parameters=[header_parameter]
-    )
     def list(self, request):
         return Response(CartItemSerializer(self.get_cartitems(), many=True).data)
 
-    @action(detail=False, methods=['POST'], permission_classes=(permissions.AllowAny,))
-    def create_customer(self, request):
-        return Response({
-            'customer': CustomerSerializer(self.get_or_create_customer()).data
-        }, status=status.HTTP_200_OK)
-
-    @extend_schema(
-        parameters=[header_parameter]
-    )
     @action(detail=False, methods=['POST'], permission_classes=(IsCustomer,))
     def add(self, request):
         customer = self.get_customer()
         data = request.data.get('data', None)
 
         if data is not None:
             self.create_cart_items(customer=customer, data=data)
@@ -84,48 +72,36 @@
                 'status': 'ok'
             }, status=status.HTTP_200_OK)
 
         return Response(
             {'server': 'Request "data" must be dict.'}, status=status.HTTP_400_BAD_REQUEST
         )
 
-    @extend_schema(
-        parameters=[header_parameter]
-    )
     @action(detail=False, methods=['DELETE'], permission_classes=(IsCustomer,))
     def remove(self, request):
         data = request.data.get('data')
         self.remove_cart_items(data)
         return Response({
             'status': 'ok'
         }, status=status.HTTP_200_OK)
 
-    @extend_schema(
-        parameters=[header_parameter]
-    )
     @action(detail=False, methods=['GET'], permission_classes=(permissions.AllowAny,))
     def session_list(self, request):
         return Response(
             self.get_cartitems(), status=status.HTTP_200_OK
         )
 
-    @extend_schema(
-        parameters=[header_parameter]
-    )
     @action(detail=False, methods=['DELETE'], permission_classes=(IsCustomer,))
     def session_remove(self, request):
         data = request.data.get('data')
         self.remove_cart_items(data)
         return Response({
             'status': 'ok'
         }, status=status.HTTP_200_OK)
 
-    @extend_schema(
-        parameters=[header_parameter]
-    )
     @action(detail=False, methods=['POST'], permission_classes=(permissions.AllowAny,))
     def session_add(self, request):
         customer = self.get_or_create_customer(session=True)
         data = request.data.get('data', None)
 
         if data is not None:
             self.create_cart_items(customer=customer, data=data)
@@ -134,17 +110,14 @@
                 {'server': 'Product added successfully.'}, status=status.HTTP_200_OK
             )
 
         return Response(
             {'error': 'Data not valid'}, status=status.HTTP_400_BAD_REQUEST
         )
 
-    @extend_schema(
-        parameters=[header_parameter]
-    )
     def partial_update(self, request, pk=None):
         customer = self.get_customer()
 
         cart_item = CartItem.objects.filter(customer=customer, pk=pk)
 
         if cart_item.count() == 0:
             return Response(status=status.HTTP_404_NOT_FOUND)
```

### Comparing `garpix_cart-2.2.0/garpix_cart.egg-info/PKG-INFO` & `garpix_cart-3.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 Metadata-Version: 2.1
-Name: garpix-cart
-Version: 2.2.0
-Summary: UNKNOWN
+Name: garpix_cart
+Version: 3.0.0
 Home-page: https://github.com/garpixcms/garpix_cart
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/markdown
 
+# Garpix Cart
 
-Garpix Cart
-===========
-
-Quickstart
-----------
+## Quickstart
 
 Install with pip 
 
-.. code-block::
+    $ pip install garpix_cart
 
-   $ pip install garpix_cart
+Add the `garpix_cart` to your INSTALLED_APPS:
 
+```python
+# settings.py
 
-Add the ``garpix_cart`` to your INSTALLED_APPS:
+INSTALLED_APPS = [
+    # ...
+    'garpix_cart',
+]
+```
 
-.. code-block:: python
+and to migration modules:
 
-   # settings.py
+```python
+# settings.py
 
-   INSTALLED_APPS = [
-       # ...
-       'garpix_cart',
-   ]
+# ...
+MIGRATION_MODULES = {
+    'garpix_cart': 'app.migrations.garpix_cart',
+}
+```
 
 Make migrations and migrate database:
 
-.. code-block::
-
-   $ ./manage.py makemigrations
-   $ ./manage.py migrate
-
+    $ ./manage.py makemigrations
+    $ ./manage.py migrate
 
-Add to ``urls.py``\ :
+Add to `urls.py`:
 
-.. code-block::
-
-   urlpatterns = [
-       # ...
-       path('', include('garpix_cart.urls'))
-   ]
+```
+urlpatterns = [
+    # ...
+    # garpix_cart
+    path('', include(('garpix_cart.urls', 'cart'), namespace='garpix_cart')),
+]
+```
 
 В интернет магазине обычно посетитель начинает искать интересные товары, надеясь добавить несколько из них в свою корзину. 
 Затем по пути к оформлению заказа они решают, создать ли учетную запись пользователя, использовать существующую или продолжить работу в качестве гостя. 
 Здесь все усложняется.
 
 Во-первых, для неаутентифицированных посетителей сайта корзина никому не принадлежит. Но каждая корзина должна быть 
 связана с ее текущим посетителем сайта.
@@ -73,24 +75,31 @@
 
 Django явно не разрешает использование таких пользовательских объектов в своих моделях баз данных. 
 Но, используя логический флаг is_active, мы можем обмануть приложение, чтобы оно интерпретировало такого гостя как 
 фальшивого анонимного пользователя.
 
 Такой подход неприменим для всех приложений на основе Django, добавляется новая модель - **Customer**
 
-Получить Customer
------------------
 
-Для создания Customer нужно сделать ``POST`` запрос на ``/api/v1/cart/create_customer/``
+## setting.py
+
+`GARPIX_CART_SERIALIZER_MIXIN` - можно задать миксин для сериалайзера элемента корзины
+
+`GARPIX_CART_MIXIN` - можно задать миксин для модели элемента корзины
+
+
+# Changelog
+
+See [CHANGELOG.md](CHANGELOG.md).
 
-Запрос вернет объект ``Customer`` с полем ``number``.
+# Contributing
 
-Далее нужно этот номер отправлять в каждый запрос с заголовок ``Cart-Token``.
+See [CONTRIBUTING.md](CONTRIBUTING.md).
 
-setting.py
-----------
+# License
 
-``GARPIX_CART_SERIALIZER_MIXIN`` - можно задать миксин для сериалайзера элемента корзины
+[MIT](LICENSE)
 
-``GARPIX_CART_MIXIN`` - можно задать миксин для модели элемента корзины
+---
 
+Developed by Garpix / [https://garpix.com](https://garpix.com)
```

### Comparing `garpix_cart-2.2.0/garpix_cart.egg-info/SOURCES.txt` & `garpix_cart-3.0.0/garpix_cart.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 MANIFEST.in
 setup.py
+garpix_cart/CHANGELOG.md
+garpix_cart/CONTRIBUTING.md
 garpix_cart/MANIFEST.in
+garpix_cart/README.md
 garpix_cart/__init__.py
 garpix_cart/abstracts.py
 garpix_cart/apps.py
 garpix_cart/exceptions.py
 garpix_cart/mixins.py
 garpix_cart/routers.py
 garpix_cart/setup.py
@@ -13,43 +16,36 @@
 garpix_cart.egg-info/PKG-INFO
 garpix_cart.egg-info/SOURCES.txt
 garpix_cart.egg-info/dependency_links.txt
 garpix_cart.egg-info/not-zip-safe
 garpix_cart.egg-info/requires.txt
 garpix_cart.egg-info/top_level.txt
 garpix_cart/__pycache__/__init__.cpython-38.pyc
-garpix_cart/__pycache__/abstracts.cpython-38.pyc
 garpix_cart/__pycache__/apps.cpython-38.pyc
-garpix_cart/__pycache__/exceptions.cpython-38.pyc
 garpix_cart/__pycache__/mixins.cpython-38.pyc
 garpix_cart/__pycache__/routers.cpython-38.pyc
 garpix_cart/__pycache__/urls.cpython-38.pyc
-garpix_cart/__pycache__/utils.cpython-38.pyc
-garpix_cart/base/__pycache__/__init__.cpython-38.pyc
-garpix_cart/base/__pycache__/base_session_handlers.cpython-38.pyc
-garpix_cart/base/__pycache__/session_cores.cpython-38.pyc
-garpix_cart/base/__pycache__/session_handlers.cpython-38.pyc
+garpix_cart/admin/__init__.py
+garpix_cart/admin/cart.py
+garpix_cart/admin/__pycache__/__init__.cpython-38.pyc
+garpix_cart/admin/__pycache__/cart.cpython-38.pyc
 garpix_cart/migrations/__init__.py
 garpix_cart/migrations/__pycache__/__init__.cpython-38.pyc
 garpix_cart/models/__init__.py
 garpix_cart/models/cart.py
-garpix_cart/models/customer.py
 garpix_cart/models/__pycache__/__init__.cpython-38.pyc
 garpix_cart/models/__pycache__/cart.cpython-38.pyc
-garpix_cart/models/__pycache__/customer.cpython-38.pyc
 garpix_cart/permissions/IsCustomer.py
 garpix_cart/permissions/__init__.py
 garpix_cart/permissions/__pycache__/IsCustomer.cpython-38.pyc
 garpix_cart/permissions/__pycache__/__init__.cpython-38.pyc
 garpix_cart/serializers/__init__.py
 garpix_cart/serializers/cart.py
-garpix_cart/serializers/customer.py
 garpix_cart/serializers/__pycache__/__init__.cpython-38.pyc
 garpix_cart/serializers/__pycache__/cart.cpython-38.pyc
-garpix_cart/serializers/__pycache__/customer.cpython-38.pyc
 garpix_cart/tests/__init__.py
 garpix_cart/tests/test_api.py
 garpix_cart/tests/__pycache__/__init__.cpython-38.pyc
 garpix_cart/tests/__pycache__/test_api.cpython-38.pyc
 garpix_cart/views/__init__.py
 garpix_cart/views/cart.py
 garpix_cart/views/__pycache__/__init__.cpython-38.pyc
```

