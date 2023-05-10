# Comparing `tmp/django-celery-ilmoitus-0.2.6.tar.gz` & `tmp/django-celery-ilmoitus-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-celery-ilmoitus-0.2.6.tar", last modified: Mon May  8 14:01:40 2023, max compression
+gzip compressed data, was "django-celery-ilmoitus-0.2.7.tar", last modified: Wed May 10 06:34:03 2023, max compression
```

## Comparing `django-celery-ilmoitus-0.2.6.tar` & `django-celery-ilmoitus-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.117506 django-celery-ilmoitus-0.2.6/
--rw-r--r--   0 aha        (501) staff       (20)       39 2021-02-12 12:19:21.000000 django-celery-ilmoitus-0.2.6/MANIFEST.in
--rw-r--r--   0 aha        (501) staff       (20)      278 2023-05-08 14:01:40.117359 django-celery-ilmoitus-0.2.6/PKG-INFO
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.115066 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/
--rw-r--r--   0 aha        (501) staff       (20)      278 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/PKG-INFO
--rw-r--r--   0 aha        (501) staff       (20)      543 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/SOURCES.txt
--rw-r--r--   0 aha        (501) staff       (20)        1 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/dependency_links.txt
--rw-r--r--   0 aha        (501) staff       (20)      103 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/entry_points.txt
--rw-r--r--   0 aha        (501) staff       (20)     1913 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/historia.json
--rw-r--r--   0 aha        (501) staff       (20)        1 2021-02-23 10:09:09.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/not-zip-safe
--rw-r--r--   0 aha        (501) staff       (20)       42 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/requires.txt
--rw-r--r--   0 aha        (501) staff       (20)        9 2023-05-08 14:01:40.000000 django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/top_level.txt
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.116907 django-celery-ilmoitus-0.2.6/ilmoitus/
--rw-r--r--   0 aha        (501) staff       (20)        0 2021-02-12 12:05:10.000000 django-celery-ilmoitus-0.2.6/ilmoitus/__init__.py
--rw-r--r--   0 aha        (501) staff       (20)      173 2021-02-12 12:13:02.000000 django-celery-ilmoitus-0.2.6/ilmoitus/celery.py
--rw-r--r--   0 aha        (501) staff       (20)     3724 2023-05-02 09:42:25.000000 django-celery-ilmoitus-0.2.6/ilmoitus/nakyma.py
--rw-r--r--   0 aha        (501) staff       (20)      565 2021-02-12 12:10:06.000000 django-celery-ilmoitus-0.2.6/ilmoitus/sovellus.py
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.113583 django-celery-ilmoitus-0.2.6/ilmoitus/templates/
-drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-08 14:01:40.117063 django-celery-ilmoitus-0.2.6/ilmoitus/templates/ilmoitus/
--rw-r--r--   0 aha        (501) staff       (20)     2409 2023-01-25 12:51:55.000000 django-celery-ilmoitus-0.2.6/ilmoitus/templates/ilmoitus/ilmoitus.html
--rw-r--r--   0 aha        (501) staff       (20)     1558 2021-02-12 12:41:21.000000 django-celery-ilmoitus-0.2.6/ilmoitus/uusi.py
--rw-r--r--   0 aha        (501) staff       (20)       79 2023-05-08 14:01:33.000000 django-celery-ilmoitus-0.2.6/pyproject.toml
--rw-r--r--   0 aha        (501) staff       (20)       38 2023-05-08 14:01:40.117541 django-celery-ilmoitus-0.2.6/setup.cfg
--rw-r--r--   0 aha        (501) staff       (20)      664 2021-02-12 12:16:25.000000 django-celery-ilmoitus-0.2.6/setup.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-10 06:34:03.000702 django-celery-ilmoitus-0.2.7/
+-rw-r--r--   0 aha        (501) staff       (20)       39 2021-02-12 12:19:21.000000 django-celery-ilmoitus-0.2.7/MANIFEST.in
+-rw-r--r--   0 aha        (501) staff       (20)      278 2023-05-10 06:34:03.000556 django-celery-ilmoitus-0.2.7/PKG-INFO
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-10 06:34:02.999290 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/
+-rw-r--r--   0 aha        (501) staff       (20)      278 2023-05-10 06:34:02.000000 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/PKG-INFO
+-rw-r--r--   0 aha        (501) staff       (20)      543 2023-05-10 06:34:02.000000 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/SOURCES.txt
+-rw-r--r--   0 aha        (501) staff       (20)        1 2023-05-10 06:34:02.000000 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/dependency_links.txt
+-rw-r--r--   0 aha        (501) staff       (20)      103 2023-05-10 06:34:02.000000 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/entry_points.txt
+-rw-r--r--   0 aha        (501) staff       (20)     2048 2023-05-10 06:34:02.000000 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/historia.json
+-rw-r--r--   0 aha        (501) staff       (20)        1 2021-02-23 10:09:09.000000 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/not-zip-safe
+-rw-r--r--   0 aha        (501) staff       (20)       42 2023-05-10 06:34:02.000000 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/requires.txt
+-rw-r--r--   0 aha        (501) staff       (20)        9 2023-05-10 06:34:02.000000 django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/top_level.txt
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-10 06:34:03.000114 django-celery-ilmoitus-0.2.7/ilmoitus/
+-rw-r--r--   0 aha        (501) staff       (20)        0 2021-02-12 12:05:10.000000 django-celery-ilmoitus-0.2.7/ilmoitus/__init__.py
+-rw-r--r--   0 aha        (501) staff       (20)      173 2021-02-12 12:13:02.000000 django-celery-ilmoitus-0.2.7/ilmoitus/celery.py
+-rw-r--r--   0 aha        (501) staff       (20)     3760 2023-05-09 12:55:07.000000 django-celery-ilmoitus-0.2.7/ilmoitus/nakyma.py
+-rw-r--r--   0 aha        (501) staff       (20)      565 2021-02-12 12:10:06.000000 django-celery-ilmoitus-0.2.7/ilmoitus/sovellus.py
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-10 06:34:02.997598 django-celery-ilmoitus-0.2.7/ilmoitus/templates/
+drwxr-xr-x   0 aha        (501) staff       (20)        0 2023-05-10 06:34:03.000263 django-celery-ilmoitus-0.2.7/ilmoitus/templates/ilmoitus/
+-rw-r--r--   0 aha        (501) staff       (20)     2409 2023-01-25 12:51:55.000000 django-celery-ilmoitus-0.2.7/ilmoitus/templates/ilmoitus/ilmoitus.html
+-rw-r--r--   0 aha        (501) staff       (20)     1558 2021-02-12 12:41:21.000000 django-celery-ilmoitus-0.2.7/ilmoitus/uusi.py
+-rw-r--r--   0 aha        (501) staff       (20)       79 2023-05-08 14:01:33.000000 django-celery-ilmoitus-0.2.7/pyproject.toml
+-rw-r--r--   0 aha        (501) staff       (20)       38 2023-05-10 06:34:03.000737 django-celery-ilmoitus-0.2.7/setup.cfg
+-rw-r--r--   0 aha        (501) staff       (20)      664 2021-02-12 12:16:25.000000 django-celery-ilmoitus-0.2.7/setup.py
```

### Comparing `django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/SOURCES.txt` & `django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-celery-ilmoitus-0.2.6/django_celery_ilmoitus.egg-info/historia.json` & `django-celery-ilmoitus-0.2.7/django_celery_ilmoitus.egg-info/historia.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9230769230769231%*

 * *Differences: {'insert': "[(0, OrderedDict([('revisio', '2be4adda38fdb7ed0a85ec04fdf8af17d2359839'), ('versio', "*

 * *           "'0.2.7'), ('kuvaus', 'Parannettu vikasietoisuutta')]))]"}*

```diff
@@ -1,9 +1,14 @@
 [
     {
+        "kuvaus": "Parannettu vikasietoisuutta",
+        "revisio": "2be4adda38fdb7ed0a85ec04fdf8af17d2359839",
+        "versio": "0.2.7"
+    },
+    {
         "kuvaus": "Pistoke v0.8 -yhteensopivuus",
         "revisio": "000c8cd66e67e1225e58d751bdd72ed983b792bc",
         "versio": "0.2.6"
     },
     {
         "kuvaus": "Django 4.1 -yhteensopivuus",
         "revisio": "a1d6c3497145dddec4ba2576fadcf31559fa1c11",
```

### Comparing `django-celery-ilmoitus-0.2.6/ilmoitus/nakyma.py` & `django-celery-ilmoitus-0.2.7/ilmoitus/nakyma.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # sillä sitä ei tunnisteta HTTP-verbin toteutukseksi.
 try:
   from pistoke.nakyma import WebsocketNakyma
   from pistoke import WebsocketProtokolla
 except ImportError:
   # pylint: disable=ungrouped-imports
   from django.views.generic import View as WebsocketNakyma
+  WebsocketProtokolla = lambda x: x
 
 from .celery import celery_app, celery_viestikanava
 
 
 class Ilmoitukset(LoginRequiredMixin, WebsocketNakyma):
 
   bootstrap_luokat = {
```

### Comparing `django-celery-ilmoitus-0.2.6/ilmoitus/sovellus.py` & `django-celery-ilmoitus-0.2.7/ilmoitus/sovellus.py`

 * *Files identical despite different names*

### Comparing `django-celery-ilmoitus-0.2.6/ilmoitus/templates/ilmoitus/ilmoitus.html` & `django-celery-ilmoitus-0.2.7/ilmoitus/templates/ilmoitus/ilmoitus.html`

 * *Files identical despite different names*

### Comparing `django-celery-ilmoitus-0.2.6/ilmoitus/uusi.py` & `django-celery-ilmoitus-0.2.7/ilmoitus/uusi.py`

 * *Files identical despite different names*

### Comparing `django-celery-ilmoitus-0.2.6/setup.py` & `django-celery-ilmoitus-0.2.7/setup.py`

 * *Files identical despite different names*

