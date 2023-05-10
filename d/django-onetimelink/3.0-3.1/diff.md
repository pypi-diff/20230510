# Comparing `tmp/django-onetimelink-3.0.tar.gz` & `tmp/django-onetimelink-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-onetimelink-3.0.tar", last modified: Mon Oct 31 09:44:16 2022, max compression
+gzip compressed data, was "django-onetimelink-3.1.tar", last modified: Wed May 10 10:56:42 2023, max compression
```

## Comparing `django-onetimelink-3.0.tar` & `django-onetimelink-3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2022-10-31 09:44:16.869790 django-onetimelink-3.0/
--rw-rw-rw-   0        0        0     1462 2022-10-31 09:00:24.000000 django-onetimelink-3.0/LICENSE
--rw-rw-rw-   0        0        0      118 2021-03-23 16:50:05.000000 django-onetimelink-3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6204 2022-10-31 09:44:16.869790 django-onetimelink-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4104 2022-10-31 09:02:27.000000 django-onetimelink-3.0/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-31 09:44:16.841381 django-onetimelink-3.0/django_onetimelink.egg-info/
--rw-rw-rw-   0        0        0     6204 2022-10-31 09:44:16.000000 django-onetimelink-3.0/django_onetimelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      808 2022-10-31 09:44:16.000000 django-onetimelink-3.0/django_onetimelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-31 09:44:16.000000 django-onetimelink-3.0/django_onetimelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-03-23 17:07:51.000000 django-onetimelink-3.0/django_onetimelink.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2022-10-31 09:44:16.000000 django-onetimelink-3.0/django_onetimelink.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-31 09:44:16.852503 django-onetimelink-3.0/onetimelink/
--rw-rw-rw-   0        0        0      967 2021-03-23 16:50:05.000000 django-onetimelink-3.0/onetimelink/__init__.py
--rw-rw-rw-   0        0        0     3612 2022-10-31 08:59:24.000000 django-onetimelink-3.0/onetimelink/admin.py
--rw-rw-rw-   0        0        0     1128 2022-09-27 00:46:21.000000 django-onetimelink-3.0/onetimelink/api.py
--rw-rw-rw-   0        0        0      136 2022-02-04 11:02:04.000000 django-onetimelink-3.0/onetimelink/apps.py
-drwxrwxrwx   0        0        0        0 2022-10-31 09:44:16.854502 django-onetimelink-3.0/onetimelink/migrations/
--rw-rw-rw-   0        0        0     2213 2022-02-04 11:08:37.000000 django-onetimelink-3.0/onetimelink/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2021-03-23 16:50:05.000000 django-onetimelink-3.0/onetimelink/migrations/__init__.py
--rw-rw-rw-   0        0        0     4245 2022-10-31 08:59:07.000000 django-onetimelink-3.0/onetimelink/models.py
--rw-rw-rw-   0        0        0     1662 2022-10-31 08:59:10.000000 django-onetimelink-3.0/onetimelink/presettings.py
-drwxrwxrwx   0        0        0        0 2022-10-31 09:44:16.828365 django-onetimelink-3.0/onetimelink/static/
-drwxrwxrwx   0        0        0        0 2022-10-31 09:44:16.856503 django-onetimelink-3.0/onetimelink/static/css/
--rw-rw-rw-   0        0        0      130 2021-03-23 16:50:05.000000 django-onetimelink-3.0/onetimelink/static/css/not_available.css
--rw-rw-rw-   0        0        0      632 2021-03-23 16:50:05.000000 django-onetimelink-3.0/onetimelink/static/css/site.css
-drwxrwxrwx   0        0        0        0 2022-10-31 09:44:16.859503 django-onetimelink-3.0/onetimelink/static/js/
--rw-rw-rw-   0        0        0    88147 2021-03-23 16:50:05.000000 django-onetimelink-3.0/onetimelink/static/js/jquery-3.4.1.min.js
--rw-rw-rw-   0        0        0   136409 2021-03-23 16:50:05.000000 django-onetimelink-3.0/onetimelink/static/js/jquery-3.4.1.min.map
-drwxrwxrwx   0        0        0        0 2022-10-31 09:44:16.866789 django-onetimelink-3.0/onetimelink/templates/
--rw-rw-rw-   0        0        0      250 2021-03-23 16:50:05.000000 django-onetimelink-3.0/onetimelink/templates/not_avallible.html
--rw-rw-rw-   0        0        0     2190 2021-03-24 02:48:23.000000 django-onetimelink-3.0/onetimelink/templates/site.html
--rw-rw-rw-   0        0        0      327 2021-03-23 16:50:05.000000 django-onetimelink-3.0/onetimelink/templates/sitedownload_changelist.html
--rw-rw-rw-   0        0        0     2484 2021-11-11 15:29:39.000000 django-onetimelink-3.0/onetimelink/test.py
--rw-rw-rw-   0        0        0      298 2022-10-31 09:14:56.000000 django-onetimelink-3.0/onetimelink/urls.py
--rw-rw-rw-   0        0        0     4784 2022-10-31 08:59:13.000000 django-onetimelink-3.0/onetimelink/views.py
--rw-rw-rw-   0        0        0      996 2022-10-31 09:44:16.869790 django-onetimelink-3.0/setup.cfg
--rw-rw-rw-   0        0        0     1749 2022-10-31 09:01:42.000000 django-onetimelink-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.823763 django-onetimelink-3.1/
+-rw-rw-rw-   0        0        0     1462 2022-10-31 09:00:24.000000 django-onetimelink-3.1/LICENSE
+-rw-rw-rw-   0        0        0      118 2021-03-23 16:50:05.000000 django-onetimelink-3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4931 2023-05-10 10:56:42.824762 django-onetimelink-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4104 2022-10-31 09:49:06.000000 django-onetimelink-3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.714253 django-onetimelink-3.1/django_onetimelink.egg-info/
+-rw-rw-rw-   0        0        0     4931 2023-05-10 10:56:42.000000 django-onetimelink-3.1/django_onetimelink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      808 2023-05-10 10:56:42.000000 django-onetimelink-3.1/django_onetimelink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:56:42.000000 django-onetimelink-3.1/django_onetimelink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-03-23 17:07:51.000000 django-onetimelink-3.1/django_onetimelink.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-10 10:56:42.000000 django-onetimelink-3.1/django_onetimelink.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.740255 django-onetimelink-3.1/onetimelink/
+-rw-rw-rw-   0        0        0      967 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/__init__.py
+-rw-rw-rw-   0        0        0     3612 2022-10-31 08:59:24.000000 django-onetimelink-3.1/onetimelink/admin.py
+-rw-rw-rw-   0        0        0     1128 2022-09-27 00:46:21.000000 django-onetimelink-3.1/onetimelink/api.py
+-rw-rw-rw-   0        0        0      136 2022-02-04 11:02:04.000000 django-onetimelink-3.1/onetimelink/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.745762 django-onetimelink-3.1/onetimelink/migrations/
+-rw-rw-rw-   0        0        0     2213 2022-02-04 11:08:37.000000 django-onetimelink-3.1/onetimelink/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4086 2023-05-10 10:55:26.000000 django-onetimelink-3.1/onetimelink/models.py
+-rw-rw-rw-   0        0        0     1662 2022-10-31 08:59:10.000000 django-onetimelink-3.1/onetimelink/presettings.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.676252 django-onetimelink-3.1/onetimelink/static/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.750763 django-onetimelink-3.1/onetimelink/static/css/
+-rw-rw-rw-   0        0        0      130 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/static/css/not_available.css
+-rw-rw-rw-   0        0        0      632 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/static/css/site.css
+drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.804761 django-onetimelink-3.1/onetimelink/static/js/
+-rw-rw-rw-   0        0        0    88147 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/static/js/jquery-3.4.1.min.js
+-rw-rw-rw-   0        0        0   136409 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/static/js/jquery-3.4.1.min.map
+drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.821763 django-onetimelink-3.1/onetimelink/templates/
+-rw-rw-rw-   0        0        0      250 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/templates/not_avallible.html
+-rw-rw-rw-   0        0        0     2190 2021-03-24 02:48:23.000000 django-onetimelink-3.1/onetimelink/templates/site.html
+-rw-rw-rw-   0        0        0      327 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/templates/sitedownload_changelist.html
+-rw-rw-rw-   0        0        0     2484 2021-11-11 15:29:39.000000 django-onetimelink-3.1/onetimelink/test.py
+-rw-rw-rw-   0        0        0      298 2022-10-31 09:14:56.000000 django-onetimelink-3.1/onetimelink/urls.py
+-rw-rw-rw-   0        0        0     4784 2022-10-31 08:59:13.000000 django-onetimelink-3.1/onetimelink/views.py
+-rw-rw-rw-   0        0        0      996 2023-05-10 10:56:42.826763 django-onetimelink-3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1738 2023-05-10 10:56:26.000000 django-onetimelink-3.1/setup.py
```

### Comparing `django-onetimelink-3.0/LICENSE` & `django-onetimelink-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/PKG-INFO` & `django-onetimelink-3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-onetimelink
-Version: 3.0
+Version: 3.1
 Summary: A django one-time file streaming application
 Home-page: https://github.com/HiroshiFuu/django-onetimelink
+Download-URL: https://pypi.python.org/pypi/django-onetimelink
 Author: FENG Hao
 Author-email: hiroshifuu@outlook.com
 License: BSD
-Download-URL: https://pypi.python.org/pypi/django-onetimelink
-Description: ===========
-        Description
-        ===========
-        
-        A Django file streaming application to provide download links that only valid for one time click. Ispired by django-dynamic-link.
-        
-        **License**
-        
-            BSD-3-Clause license
-        
-        **Notes**
-        
-            * Tested with Django 2.2
-            * Tested with Django 3.1
-        
-        ========
-        Features
-        ========
-        
-            * One-time only download link 
-        
-        ============
-        Installation
-        ============
-        
-        **Dependences**
-        
-            * This app only
-        
-        **Installation**
-        
-            *Installation with pip (recommended)*
-        
-                *Pip will download and install the package and take care of all the dependences.
-                If you havn't pip on your system then install setuptools first after that run "easy_install pip".
-                After that you can use pip in your terminal window.*
-        
-                * Use the stable release (recommended)::
-        
-                    pip install django-onetimelink
-        
-                * With pip you can also uninstall::
-        
-                    pip uninstall django-onetimelink
-        
-        **test your installation**
-        
-            Go to console and type::
-        
-                python
-        
-            ... then type::
-            
-                >>> import onetimelink
-                >>> onetimelink.CKINST()
-                >>> help(onetimelink)
-                >>> exit()
-            
-        =====
-        Setup
-        =====
-            
-            * Add "onetimelink" to you installed apps in the settings file.
-            * Make sure that:
-        
-                1.  Your Admin is enabled ('django.contrib.admin', is in your INSTALLED_APPS).
-                2.  'django.contrib.auth.context_processors.auth', (also for admin) is in TEMPLATE_CONTEXT_PROCESSORS.
-                3.  'django.core.context_processors.request', is in TEMPLATE_CONTEXT_PROCESSORS.
-        
-            * Add the following to your urls.py:
-        
-                1.  from django.conf.urls import include, url
-                2.  from onetimelink import presettings
-                3.  url(r'%s/' % presettings.DYNAMIC_LINK_URL_BASE_COMPONENT, include('onetimelink.urls')),
-                
-            * Finally run::
-            
-                python manage.py makemigrations
-                python manage.py migrate
-                python manage.py runserver
-        
-        **Make it custom**
-        
-            Use the global settings.py in your projects root to overwrite the applications presettings with the following variables.
-        
-            DYNAMIC_LINK_MEDIA
-        
-                - Default: settings.MEDIA_ROOT
-                - A path to a directory. From this point you can walk down the subdirectories to choose your files to serve.
-        
-            DYNAMIC_LINK_URL_BASE_COMPONENT
-            
-                - Default: 'OneTimeLink'
-                - A string that modifies your url serve path.
-                - Example: www.example.com/DYNAMIC_LINK_URL_BASE_COMPONENT/link/3839hd8HKl3/example.zip.
-        
-            DYNAMIC_LINK_UPLOAD_TO
-            
-                - Default: ''
-                - Uploaded files base directory.
-        
-            DYNAMIC_LINK_SCHEMA_PROTO
-            
-                - Default: 'http'
-                - HTTP Schema Protocal.
-        
-        =====
-        Usage
-        =====
-        
-        Open the admin interface and go to "OneTimeLink" section. The rest should be self-explanatory.
-        
-        **Hints**
-        
-            * Upload Files to upload the file to DYNAMIC_LINK_MEDIA
-            * The filename from the in Upload Files is only for human readability. You can delete or change these filenames in any way you want.
-            * Through the action button you can serve a site with all the files from Upload Files.
-        
-        ==========
-        Changelogs
-        ==========
-        
-        **2021-03-24**
-        
-            * Add setting for schema protocol
-            * Prefix links with FORCE_SCRIPT_NAME
-        
-        **2021-03-25**
-        
-            * Fix several bugs
-            * Do NOT use previous versions of this package
-        
-        **2021-06-08**
-        
-            * Fix search bug in admin
-            * clean up code
-            * Do NOT use previous versions of this package
-        
-        **2022-02-04**
-        
-            * Add setting to override HTTP Host
-            * clean up code
-            * Fix several bugs
-            * Do NOT use previous versions of this package
-        
-        **2022-09-27**
-        
-            * Add DYNAMIC_LINK_USE_FORCE_SCRIPT_NAME setting
-            * Add HTTP Host override setting
-            * Fix several bugs
-            * clean up code
-            * Do NOT use previous versions of this package
-        
-        **2022-10-31**
-        
-            * Add support for Django 4
-            * Remove support for Python 3.6, 3.7 as Django 4 requires min 3.8
-            * Do NOT use previous versions of this package
-        
 Keywords: django one-time file link serve
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
+License-File: LICENSE
+
+===========
+Description
+===========
+
+A Django file streaming application to provide download links that only valid for one time click. Ispired by django-dynamic-link.
+
+**License**
+
+    BSD-3-Clause license
+
+**Notes**
+
+    * Tested with Django 2.2
+    * Tested with Django 3.1
+
+========
+Features
+========
+
+    * One-time only download link 
+
+============
+Installation
+============
+
+**Dependences**
+
+    * This app only
+
+**Installation**
+
+    *Installation with pip (recommended)*
+
+        *Pip will download and install the package and take care of all the dependences.
+        If you havn't pip on your system then install setuptools first after that run "easy_install pip".
+        After that you can use pip in your terminal window.*
+
+        * Use the stable release (recommended)::
+
+            pip install django-onetimelink
+
+        * With pip you can also uninstall::
+
+            pip uninstall django-onetimelink
+
+**test your installation**
+
+    Go to console and type::
+
+        python
+
+    ... then type::
+    
+        >>> import onetimelink
+        >>> onetimelink.CKINST()
+        >>> help(onetimelink)
+        >>> exit()
+    
+=====
+Setup
+=====
+    
+    * Add "onetimelink" to you installed apps in the settings file.
+    * Make sure that:
+
+        1.  Your Admin is enabled ('django.contrib.admin', is in your INSTALLED_APPS).
+        2.  'django.contrib.auth.context_processors.auth', (also for admin) is in TEMPLATE_CONTEXT_PROCESSORS.
+        3.  'django.core.context_processors.request', is in TEMPLATE_CONTEXT_PROCESSORS.
+
+    * Add the following to your urls.py:
+
+        1.  from django.conf.urls import include, url
+        2.  from onetimelink import presettings
+        3.  url(r'%s/' % presettings.DYNAMIC_LINK_URL_BASE_COMPONENT, include('onetimelink.urls')),
+        
+    * Finally run::
+    
+        python manage.py makemigrations
+        python manage.py migrate
+        python manage.py runserver
+
+**Make it custom**
+
+    Use the global settings.py in your projects root to overwrite the applications presettings with the following variables.
+
+    DYNAMIC_LINK_MEDIA
+
+        - Default: settings.MEDIA_ROOT
+        - A path to a directory. From this point you can walk down the subdirectories to choose your files to serve.
+
+    DYNAMIC_LINK_URL_BASE_COMPONENT
+    
+        - Default: 'OneTimeLink'
+        - A string that modifies your url serve path.
+        - Example: www.example.com/DYNAMIC_LINK_URL_BASE_COMPONENT/link/3839hd8HKl3/example.zip.
+
+    DYNAMIC_LINK_UPLOAD_TO
+    
+        - Default: ''
+        - Uploaded files base directory.
+
+    DYNAMIC_LINK_SCHEMA_PROTO
+    
+        - Default: 'http'
+        - HTTP Schema Protocal.
+
+=====
+Usage
+=====
+
+Open the admin interface and go to "OneTimeLink" section. The rest should be self-explanatory.
+
+**Hints**
+
+    * Upload Files to upload the file to DYNAMIC_LINK_MEDIA
+    * The filename from the in Upload Files is only for human readability. You can delete or change these filenames in any way you want.
+    * Through the action button you can serve a site with all the files from Upload Files.
+
+==========
+Changelogs
+==========
+
+**2021-03-24**
+
+    * Add setting for schema protocol
+    * Prefix links with FORCE_SCRIPT_NAME
+
+**2021-03-25**
+
+    * Fix several bugs
+    * Do NOT use previous versions of this package
+
+**2021-06-08**
+
+    * Fix search bug in admin
+    * clean up code
+    * Do NOT use previous versions of this package
+
+**2022-02-04**
+
+    * Add setting to override HTTP Host
+    * clean up code
+    * Fix several bugs
+    * Do NOT use previous versions of this package
+
+**2022-09-27**
+
+    * Add DYNAMIC_LINK_USE_FORCE_SCRIPT_NAME setting
+    * Add HTTP Host override setting
+    * Fix several bugs
+    * clean up code
+    * Do NOT use previous versions of this package
+
+**2022-10-31**
+
+    * Add support for Django 4
+    * Remove support for Python 3.6, 3.7 as Django 4 requires min 3.8
+    * Do NOT use previous versions of this package
```

### Comparing `django-onetimelink-3.0/README.rst` & `django-onetimelink-3.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/django_onetimelink.egg-info/PKG-INFO` & `django-onetimelink-3.1/django_onetimelink.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-onetimelink
-Version: 3.0
+Version: 3.1
 Summary: A django one-time file streaming application
 Home-page: https://github.com/HiroshiFuu/django-onetimelink
+Download-URL: https://pypi.python.org/pypi/django-onetimelink
 Author: FENG Hao
 Author-email: hiroshifuu@outlook.com
 License: BSD
-Download-URL: https://pypi.python.org/pypi/django-onetimelink
-Description: ===========
-        Description
-        ===========
-        
-        A Django file streaming application to provide download links that only valid for one time click. Ispired by django-dynamic-link.
-        
-        **License**
-        
-            BSD-3-Clause license
-        
-        **Notes**
-        
-            * Tested with Django 2.2
-            * Tested with Django 3.1
-        
-        ========
-        Features
-        ========
-        
-            * One-time only download link 
-        
-        ============
-        Installation
-        ============
-        
-        **Dependences**
-        
-            * This app only
-        
-        **Installation**
-        
-            *Installation with pip (recommended)*
-        
-                *Pip will download and install the package and take care of all the dependences.
-                If you havn't pip on your system then install setuptools first after that run "easy_install pip".
-                After that you can use pip in your terminal window.*
-        
-                * Use the stable release (recommended)::
-        
-                    pip install django-onetimelink
-        
-                * With pip you can also uninstall::
-        
-                    pip uninstall django-onetimelink
-        
-        **test your installation**
-        
-            Go to console and type::
-        
-                python
-        
-            ... then type::
-            
-                >>> import onetimelink
-                >>> onetimelink.CKINST()
-                >>> help(onetimelink)
-                >>> exit()
-            
-        =====
-        Setup
-        =====
-            
-            * Add "onetimelink" to you installed apps in the settings file.
-            * Make sure that:
-        
-                1.  Your Admin is enabled ('django.contrib.admin', is in your INSTALLED_APPS).
-                2.  'django.contrib.auth.context_processors.auth', (also for admin) is in TEMPLATE_CONTEXT_PROCESSORS.
-                3.  'django.core.context_processors.request', is in TEMPLATE_CONTEXT_PROCESSORS.
-        
-            * Add the following to your urls.py:
-        
-                1.  from django.conf.urls import include, url
-                2.  from onetimelink import presettings
-                3.  url(r'%s/' % presettings.DYNAMIC_LINK_URL_BASE_COMPONENT, include('onetimelink.urls')),
-                
-            * Finally run::
-            
-                python manage.py makemigrations
-                python manage.py migrate
-                python manage.py runserver
-        
-        **Make it custom**
-        
-            Use the global settings.py in your projects root to overwrite the applications presettings with the following variables.
-        
-            DYNAMIC_LINK_MEDIA
-        
-                - Default: settings.MEDIA_ROOT
-                - A path to a directory. From this point you can walk down the subdirectories to choose your files to serve.
-        
-            DYNAMIC_LINK_URL_BASE_COMPONENT
-            
-                - Default: 'OneTimeLink'
-                - A string that modifies your url serve path.
-                - Example: www.example.com/DYNAMIC_LINK_URL_BASE_COMPONENT/link/3839hd8HKl3/example.zip.
-        
-            DYNAMIC_LINK_UPLOAD_TO
-            
-                - Default: ''
-                - Uploaded files base directory.
-        
-            DYNAMIC_LINK_SCHEMA_PROTO
-            
-                - Default: 'http'
-                - HTTP Schema Protocal.
-        
-        =====
-        Usage
-        =====
-        
-        Open the admin interface and go to "OneTimeLink" section. The rest should be self-explanatory.
-        
-        **Hints**
-        
-            * Upload Files to upload the file to DYNAMIC_LINK_MEDIA
-            * The filename from the in Upload Files is only for human readability. You can delete or change these filenames in any way you want.
-            * Through the action button you can serve a site with all the files from Upload Files.
-        
-        ==========
-        Changelogs
-        ==========
-        
-        **2021-03-24**
-        
-            * Add setting for schema protocol
-            * Prefix links with FORCE_SCRIPT_NAME
-        
-        **2021-03-25**
-        
-            * Fix several bugs
-            * Do NOT use previous versions of this package
-        
-        **2021-06-08**
-        
-            * Fix search bug in admin
-            * clean up code
-            * Do NOT use previous versions of this package
-        
-        **2022-02-04**
-        
-            * Add setting to override HTTP Host
-            * clean up code
-            * Fix several bugs
-            * Do NOT use previous versions of this package
-        
-        **2022-09-27**
-        
-            * Add DYNAMIC_LINK_USE_FORCE_SCRIPT_NAME setting
-            * Add HTTP Host override setting
-            * Fix several bugs
-            * clean up code
-            * Do NOT use previous versions of this package
-        
-        **2022-10-31**
-        
-            * Add support for Django 4
-            * Remove support for Python 3.6, 3.7 as Django 4 requires min 3.8
-            * Do NOT use previous versions of this package
-        
 Keywords: django one-time file link serve
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet
+License-File: LICENSE
+
+===========
+Description
+===========
+
+A Django file streaming application to provide download links that only valid for one time click. Ispired by django-dynamic-link.
+
+**License**
+
+    BSD-3-Clause license
+
+**Notes**
+
+    * Tested with Django 2.2
+    * Tested with Django 3.1
+
+========
+Features
+========
+
+    * One-time only download link 
+
+============
+Installation
+============
+
+**Dependences**
+
+    * This app only
+
+**Installation**
+
+    *Installation with pip (recommended)*
+
+        *Pip will download and install the package and take care of all the dependences.
+        If you havn't pip on your system then install setuptools first after that run "easy_install pip".
+        After that you can use pip in your terminal window.*
+
+        * Use the stable release (recommended)::
+
+            pip install django-onetimelink
+
+        * With pip you can also uninstall::
+
+            pip uninstall django-onetimelink
+
+**test your installation**
+
+    Go to console and type::
+
+        python
+
+    ... then type::
+    
+        >>> import onetimelink
+        >>> onetimelink.CKINST()
+        >>> help(onetimelink)
+        >>> exit()
+    
+=====
+Setup
+=====
+    
+    * Add "onetimelink" to you installed apps in the settings file.
+    * Make sure that:
+
+        1.  Your Admin is enabled ('django.contrib.admin', is in your INSTALLED_APPS).
+        2.  'django.contrib.auth.context_processors.auth', (also for admin) is in TEMPLATE_CONTEXT_PROCESSORS.
+        3.  'django.core.context_processors.request', is in TEMPLATE_CONTEXT_PROCESSORS.
+
+    * Add the following to your urls.py:
+
+        1.  from django.conf.urls import include, url
+        2.  from onetimelink import presettings
+        3.  url(r'%s/' % presettings.DYNAMIC_LINK_URL_BASE_COMPONENT, include('onetimelink.urls')),
+        
+    * Finally run::
+    
+        python manage.py makemigrations
+        python manage.py migrate
+        python manage.py runserver
+
+**Make it custom**
+
+    Use the global settings.py in your projects root to overwrite the applications presettings with the following variables.
+
+    DYNAMIC_LINK_MEDIA
+
+        - Default: settings.MEDIA_ROOT
+        - A path to a directory. From this point you can walk down the subdirectories to choose your files to serve.
+
+    DYNAMIC_LINK_URL_BASE_COMPONENT
+    
+        - Default: 'OneTimeLink'
+        - A string that modifies your url serve path.
+        - Example: www.example.com/DYNAMIC_LINK_URL_BASE_COMPONENT/link/3839hd8HKl3/example.zip.
+
+    DYNAMIC_LINK_UPLOAD_TO
+    
+        - Default: ''
+        - Uploaded files base directory.
+
+    DYNAMIC_LINK_SCHEMA_PROTO
+    
+        - Default: 'http'
+        - HTTP Schema Protocal.
+
+=====
+Usage
+=====
+
+Open the admin interface and go to "OneTimeLink" section. The rest should be self-explanatory.
+
+**Hints**
+
+    * Upload Files to upload the file to DYNAMIC_LINK_MEDIA
+    * The filename from the in Upload Files is only for human readability. You can delete or change these filenames in any way you want.
+    * Through the action button you can serve a site with all the files from Upload Files.
+
+==========
+Changelogs
+==========
+
+**2021-03-24**
+
+    * Add setting for schema protocol
+    * Prefix links with FORCE_SCRIPT_NAME
+
+**2021-03-25**
+
+    * Fix several bugs
+    * Do NOT use previous versions of this package
+
+**2021-06-08**
+
+    * Fix search bug in admin
+    * clean up code
+    * Do NOT use previous versions of this package
+
+**2022-02-04**
+
+    * Add setting to override HTTP Host
+    * clean up code
+    * Fix several bugs
+    * Do NOT use previous versions of this package
+
+**2022-09-27**
+
+    * Add DYNAMIC_LINK_USE_FORCE_SCRIPT_NAME setting
+    * Add HTTP Host override setting
+    * Fix several bugs
+    * clean up code
+    * Do NOT use previous versions of this package
+
+**2022-10-31**
+
+    * Add support for Django 4
+    * Remove support for Python 3.6, 3.7 as Django 4 requires min 3.8
+    * Do NOT use previous versions of this package
```

### Comparing `django-onetimelink-3.0/django_onetimelink.egg-info/SOURCES.txt` & `django-onetimelink-3.1/django_onetimelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/__init__.py` & `django-onetimelink-3.1/onetimelink/__init__.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/admin.py` & `django-onetimelink-3.1/onetimelink/admin.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/api.py` & `django-onetimelink-3.1/onetimelink/api.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/migrations/0001_initial.py` & `django-onetimelink-3.1/onetimelink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/models.py` & `django-onetimelink-3.1/onetimelink/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,53 +7,51 @@
 
 import os
 
 
 class DownloadSite(models.Model):
     class Meta:
         verbose_name = 'Download Site'
+
     link_key = models.CharField(max_length=63, editable=False, unique=True)
     timestamp_creation = models.DateTimeField(
         auto_now=False,
         auto_now_add=True,
         editable=False,
         verbose_name=_(u'creation time'),
     )
 
-    def save(self, * args, ** kwargs):
+    def save(self, *args, **kwargs):
         """Perform custom methods before saving."""
         # If not available set a link key before saving
         if not self.link_key:
             self.link_key = api.gen_key()
 
         # call the real save method
         try:
-            super(DownloadSite, self).save(*args, ** kwargs)
+            super(DownloadSite, self).save(*args, **kwargs)
         except IntegrityError:
             # enforce a unique key (with a longer string)
             import time
+
             key = str(time.time()).replace('.', '')
             self.link_key = key + api.gen_key()
             # call the save method again
-            super(DownloadSite, self).save(*args, ** kwargs)
+            super(DownloadSite, self).save(*args, **kwargs)
 
     def __str__(self):
         return self.link_key
 
 
 class UploadFile(models.Model):
     class Meta:
         verbose_name = 'Upload File'
+
     display_name = models.CharField(max_length=63, blank=False, null=False, unique=True, verbose_name=_('Display Name'))
-    file = models.FileField(
-        upload_to=presettings.DYNAMIC_LINK_UPLOAD_TO,
-        help_text=_(u'Select the file to upload'),
-        verbose_name=_(u'file'),
-        max_length=255,
-    )
+    file = models.FileField(upload_to=presettings.DYNAMIC_LINK_UPLOAD_TO, help_text=_(u'Select the file to upload'), verbose_name=_(u'file'), max_length=255, blank=True, null=True)
 
     def __str__(self):
         return self.display_name
 
 
 class Download(models.Model):
     active = models.BooleanField(default=True, verbose_name=_(u'is active'))
@@ -61,15 +59,15 @@
     timestamp_creation = models.DateTimeField(
         auto_now=False,
         auto_now_add=True,
         editable=False,
         verbose_name=_(u'creation time'),
     )
     site = models.ForeignKey(DownloadSite, models.CASCADE, related_name='downloads', blank=True, null=True)
-    down_file = models.ForeignKey(UploadFile, models.CASCADE, related_name='downloads', blank=True, null=True)
+    down_file = models.ForeignKey(UploadFile, models.CASCADE, related_name='downloads')
 
     def get_filename(self):
         return os.path.basename(self.down_file.file.path)
 
     def get_path(self):
         """
         if active it returns the full path of stored file to serve.
@@ -77,43 +75,37 @@
         """
         if self.active:
             self.active = False
             self.save()
             return self.down_file.file.path
         return None
 
-    def save(self, * args, ** kwargs):
+    def save(self, *args, **kwargs):
         """Perform custom methods before saving."""
         # If link not created, generate a link key before saving
         if not self.link_key:
             self.link_key = api.gen_key()
 
         # call the real save method
         try:
-            super(Download, self).save(*args, ** kwargs)
+            super(Download, self).save(*args, **kwargs)
         except IntegrityError:
             # enforce a unique key (with a longer string)
             import time
+
             key = str(time.time()).replace('.', '')
             self.link_key = key + api.gen_key()
             # call the save method again
-            super(Download, self).save(*args, ** kwargs)
+            super(Download, self).save(*args, **kwargs)
 
     def __unicode__(self):
         if self.down_file is not None:
-            return '%s: %s, %s' % (
-                str(_(u'Filename')),
-                self.down_file.display_name,
-                self.get_filename()
-            )
+            return '%s: %s, %s' % (str(_(u'Filename')), self.down_file.display_name, self.get_filename())
         else:
-            return '%s: %s' % (
-                str(_(u'Filename')),
-                self.get_filename()
-            )
+            return '%s: %s' % (str(_(u'Filename')), self.get_filename())
 
     def __str__(self):
         if self.down_file is not None:
             return 'Name: %s  Key: %s  Path: %s' % (self.down_file.display_name, self.link_key, self.down_file.file.path)
         else:
             return self.link_key
```

### Comparing `django-onetimelink-3.0/onetimelink/presettings.py` & `django-onetimelink-3.1/onetimelink/presettings.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/static/css/site.css` & `django-onetimelink-3.1/onetimelink/static/css/site.css`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/static/js/jquery-3.4.1.min.js` & `django-onetimelink-3.1/onetimelink/static/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/static/js/jquery-3.4.1.min.map` & `django-onetimelink-3.1/onetimelink/static/js/jquery-3.4.1.min.map`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/templates/site.html` & `django-onetimelink-3.1/onetimelink/templates/site.html`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/test.py` & `django-onetimelink-3.1/onetimelink/test.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/onetimelink/views.py` & `django-onetimelink-3.1/onetimelink/views.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/setup.cfg` & `django-onetimelink-3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.0/setup.py` & `django-onetimelink-3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,39 @@
     # set requierment only if django not avallible.
     REQUIRES.append('django')
 
 if sys.version_info < (3, 8):
     REQUIRES.append('python >= 3.8')
 
 
-setup(name='django-onetimelink',
-      version=3.0,
-      description='A django one-time file streaming application',
-      long_description=long_description,
-      author='FENG Hao',
-      author_email='hiroshifuu@outlook.com',
-      url='https://github.com/HiroshiFuu/django-onetimelink',
-      download_url='https://pypi.python.org/pypi/django-onetimelink',
-      license='BSD',
-      packages=find_packages(exclude=['example', ]),
-      include_package_data=True,
-      keywords="django one-time file link serve",
-      classifiers=[
-          'Development Status :: 5 - Production/Stable',
-          'Framework :: Django :: 3.0',
-          'Framework :: Django :: 4.0',
-          'License :: OSI Approved :: BSD License',
-          'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3 :: Only',
-          'Environment :: Console',
-          'Natural Language :: English',
-          'Intended Audience :: Developers',
-          'Topic :: Internet',
-      ],
-      install_requires=REQUIRES,
-      zip_safe=False,
-      )
+setup(
+    name='django-onetimelink',
+    version=3.1,
+    description='A django one-time file streaming application',
+    long_description=long_description,
+    author='FENG Hao',
+    author_email='hiroshifuu@outlook.com',
+    url='https://github.com/HiroshiFuu/django-onetimelink',
+    download_url='https://pypi.python.org/pypi/django-onetimelink',
+    license='BSD',
+    packages=find_packages(
+        exclude=[
+            'example',
+        ]
+    ),
+    include_package_data=True,
+    keywords="django one-time file link serve",
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Framework :: Django :: 3.0',
+        'Framework :: Django :: 4.0',
+        'License :: OSI Approved :: BSD License',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python :: 3 :: Only',
+        'Environment :: Console',
+        'Natural Language :: English',
+        'Intended Audience :: Developers',
+        'Topic :: Internet',
+    ],
+    install_requires=REQUIRES,
+    zip_safe=False,
+)
```

