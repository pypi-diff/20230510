# Comparing `tmp/django-onetimelink-3.1.tar.gz` & `tmp/django-onetimelink-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-onetimelink-3.1.tar", last modified: Wed May 10 10:56:42 2023, max compression
+gzip compressed data, was "django-onetimelink-3.2.tar", last modified: Wed May 10 11:41:16 2023, max compression
```

## Comparing `django-onetimelink-3.1.tar` & `django-onetimelink-3.2.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.823763 django-onetimelink-3.1/
--rw-rw-rw-   0        0        0     1462 2022-10-31 09:00:24.000000 django-onetimelink-3.1/LICENSE
--rw-rw-rw-   0        0        0      118 2021-03-23 16:50:05.000000 django-onetimelink-3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4931 2023-05-10 10:56:42.824762 django-onetimelink-3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4104 2022-10-31 09:49:06.000000 django-onetimelink-3.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.714253 django-onetimelink-3.1/django_onetimelink.egg-info/
--rw-rw-rw-   0        0        0     4931 2023-05-10 10:56:42.000000 django-onetimelink-3.1/django_onetimelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      808 2023-05-10 10:56:42.000000 django-onetimelink-3.1/django_onetimelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:56:42.000000 django-onetimelink-3.1/django_onetimelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-03-23 17:07:51.000000 django-onetimelink-3.1/django_onetimelink.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-05-10 10:56:42.000000 django-onetimelink-3.1/django_onetimelink.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.740255 django-onetimelink-3.1/onetimelink/
--rw-rw-rw-   0        0        0      967 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/__init__.py
--rw-rw-rw-   0        0        0     3612 2022-10-31 08:59:24.000000 django-onetimelink-3.1/onetimelink/admin.py
--rw-rw-rw-   0        0        0     1128 2022-09-27 00:46:21.000000 django-onetimelink-3.1/onetimelink/api.py
--rw-rw-rw-   0        0        0      136 2022-02-04 11:02:04.000000 django-onetimelink-3.1/onetimelink/apps.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.745762 django-onetimelink-3.1/onetimelink/migrations/
--rw-rw-rw-   0        0        0     2213 2022-02-04 11:08:37.000000 django-onetimelink-3.1/onetimelink/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/migrations/__init__.py
--rw-rw-rw-   0        0        0     4086 2023-05-10 10:55:26.000000 django-onetimelink-3.1/onetimelink/models.py
--rw-rw-rw-   0        0        0     1662 2022-10-31 08:59:10.000000 django-onetimelink-3.1/onetimelink/presettings.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.676252 django-onetimelink-3.1/onetimelink/static/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.750763 django-onetimelink-3.1/onetimelink/static/css/
--rw-rw-rw-   0        0        0      130 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/static/css/not_available.css
--rw-rw-rw-   0        0        0      632 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/static/css/site.css
-drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.804761 django-onetimelink-3.1/onetimelink/static/js/
--rw-rw-rw-   0        0        0    88147 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/static/js/jquery-3.4.1.min.js
--rw-rw-rw-   0        0        0   136409 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/static/js/jquery-3.4.1.min.map
-drwxrwxrwx   0        0        0        0 2023-05-10 10:56:42.821763 django-onetimelink-3.1/onetimelink/templates/
--rw-rw-rw-   0        0        0      250 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/templates/not_avallible.html
--rw-rw-rw-   0        0        0     2190 2021-03-24 02:48:23.000000 django-onetimelink-3.1/onetimelink/templates/site.html
--rw-rw-rw-   0        0        0      327 2021-03-23 16:50:05.000000 django-onetimelink-3.1/onetimelink/templates/sitedownload_changelist.html
--rw-rw-rw-   0        0        0     2484 2021-11-11 15:29:39.000000 django-onetimelink-3.1/onetimelink/test.py
--rw-rw-rw-   0        0        0      298 2022-10-31 09:14:56.000000 django-onetimelink-3.1/onetimelink/urls.py
--rw-rw-rw-   0        0        0     4784 2022-10-31 08:59:13.000000 django-onetimelink-3.1/onetimelink/views.py
--rw-rw-rw-   0        0        0      996 2023-05-10 10:56:42.826763 django-onetimelink-3.1/setup.cfg
--rw-rw-rw-   0        0        0     1738 2023-05-10 10:56:26.000000 django-onetimelink-3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:41:16.480946 django-onetimelink-3.2/
+-rw-rw-rw-   0        0        0     1462 2022-10-31 09:00:24.000000 django-onetimelink-3.2/LICENSE
+-rw-rw-rw-   0        0        0      118 2021-03-23 16:50:05.000000 django-onetimelink-3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4931 2023-05-10 11:41:16.480946 django-onetimelink-3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4104 2022-10-31 09:49:06.000000 django-onetimelink-3.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-10 11:41:16.412623 django-onetimelink-3.2/django_onetimelink.egg-info/
+-rw-rw-rw-   0        0        0     4931 2023-05-10 11:41:16.000000 django-onetimelink-3.2/django_onetimelink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      886 2023-05-10 11:41:16.000000 django-onetimelink-3.2/django_onetimelink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:41:16.000000 django-onetimelink-3.2/django_onetimelink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-03-23 17:07:51.000000 django-onetimelink-3.2/django_onetimelink.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-10 11:41:16.000000 django-onetimelink-3.2/django_onetimelink.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:41:16.433947 django-onetimelink-3.2/onetimelink/
+-rw-rw-rw-   0        0        0      967 2021-03-23 16:50:05.000000 django-onetimelink-3.2/onetimelink/__init__.py
+-rw-rw-rw-   0        0        0     3612 2022-10-31 08:59:24.000000 django-onetimelink-3.2/onetimelink/admin.py
+-rw-rw-rw-   0        0        0     1128 2022-09-27 00:46:21.000000 django-onetimelink-3.2/onetimelink/api.py
+-rw-rw-rw-   0        0        0      136 2022-02-04 11:02:04.000000 django-onetimelink-3.2/onetimelink/apps.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:41:16.441947 django-onetimelink-3.2/onetimelink/migrations/
+-rw-rw-rw-   0        0        0     2213 2022-02-04 11:08:37.000000 django-onetimelink-3.2/onetimelink/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      965 2023-05-10 11:39:58.000000 django-onetimelink-3.2/onetimelink/migrations/0002_alter_download_down_file_alter_uploadfile_file.py
+-rw-rw-rw-   0        0        0        0 2021-03-23 16:50:05.000000 django-onetimelink-3.2/onetimelink/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4086 2023-05-10 10:55:26.000000 django-onetimelink-3.2/onetimelink/models.py
+-rw-rw-rw-   0        0        0     1662 2022-10-31 08:59:10.000000 django-onetimelink-3.2/onetimelink/presettings.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:41:16.391020 django-onetimelink-3.2/onetimelink/static/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:41:16.444946 django-onetimelink-3.2/onetimelink/static/css/
+-rw-rw-rw-   0        0        0      130 2021-03-23 16:50:05.000000 django-onetimelink-3.2/onetimelink/static/css/not_available.css
+-rw-rw-rw-   0        0        0      632 2021-03-23 16:50:05.000000 django-onetimelink-3.2/onetimelink/static/css/site.css
+drwxrwxrwx   0        0        0        0 2023-05-10 11:41:16.464946 django-onetimelink-3.2/onetimelink/static/js/
+-rw-rw-rw-   0        0        0    88147 2021-03-23 16:50:05.000000 django-onetimelink-3.2/onetimelink/static/js/jquery-3.4.1.min.js
+-rw-rw-rw-   0        0        0   136409 2021-03-23 16:50:05.000000 django-onetimelink-3.2/onetimelink/static/js/jquery-3.4.1.min.map
+drwxrwxrwx   0        0        0        0 2023-05-10 11:41:16.478946 django-onetimelink-3.2/onetimelink/templates/
+-rw-rw-rw-   0        0        0      250 2021-03-23 16:50:05.000000 django-onetimelink-3.2/onetimelink/templates/not_avallible.html
+-rw-rw-rw-   0        0        0     2190 2021-03-24 02:48:23.000000 django-onetimelink-3.2/onetimelink/templates/site.html
+-rw-rw-rw-   0        0        0      327 2021-03-23 16:50:05.000000 django-onetimelink-3.2/onetimelink/templates/sitedownload_changelist.html
+-rw-rw-rw-   0        0        0     2484 2021-11-11 15:29:39.000000 django-onetimelink-3.2/onetimelink/test.py
+-rw-rw-rw-   0        0        0      298 2022-10-31 09:14:56.000000 django-onetimelink-3.2/onetimelink/urls.py
+-rw-rw-rw-   0        0        0     4784 2022-10-31 08:59:13.000000 django-onetimelink-3.2/onetimelink/views.py
+-rw-rw-rw-   0        0        0      996 2023-05-10 11:41:16.482946 django-onetimelink-3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1738 2023-05-10 11:41:10.000000 django-onetimelink-3.2/setup.py
```

### Comparing `django-onetimelink-3.1/LICENSE` & `django-onetimelink-3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/PKG-INFO` & `django-onetimelink-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-onetimelink
-Version: 3.1
+Version: 3.2
 Summary: A django one-time file streaming application
 Home-page: https://github.com/HiroshiFuu/django-onetimelink
 Download-URL: https://pypi.python.org/pypi/django-onetimelink
 Author: FENG Hao
 Author-email: hiroshifuu@outlook.com
 License: BSD
 Keywords: django one-time file link serve
```

### Comparing `django-onetimelink-3.1/README.rst` & `django-onetimelink-3.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/django_onetimelink.egg-info/PKG-INFO` & `django-onetimelink-3.2/django_onetimelink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-onetimelink
-Version: 3.1
+Version: 3.2
 Summary: A django one-time file streaming application
 Home-page: https://github.com/HiroshiFuu/django-onetimelink
 Download-URL: https://pypi.python.org/pypi/django-onetimelink
 Author: FENG Hao
 Author-email: hiroshifuu@outlook.com
 License: BSD
 Keywords: django one-time file link serve
```

### Comparing `django-onetimelink-3.1/django_onetimelink.egg-info/SOURCES.txt` & `django-onetimelink-3.2/django_onetimelink.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 onetimelink/apps.py
 onetimelink/models.py
 onetimelink/presettings.py
 onetimelink/test.py
 onetimelink/urls.py
 onetimelink/views.py
 onetimelink/migrations/0001_initial.py
+onetimelink/migrations/0002_alter_download_down_file_alter_uploadfile_file.py
 onetimelink/migrations/__init__.py
 onetimelink/static/css/not_available.css
 onetimelink/static/css/site.css
 onetimelink/static/js/jquery-3.4.1.min.js
 onetimelink/static/js/jquery-3.4.1.min.map
 onetimelink/templates/not_avallible.html
 onetimelink/templates/site.html
```

### Comparing `django-onetimelink-3.1/onetimelink/__init__.py` & `django-onetimelink-3.2/onetimelink/__init__.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/admin.py` & `django-onetimelink-3.2/onetimelink/admin.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/api.py` & `django-onetimelink-3.2/onetimelink/api.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/migrations/0001_initial.py` & `django-onetimelink-3.2/onetimelink/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/models.py` & `django-onetimelink-3.2/onetimelink/models.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/presettings.py` & `django-onetimelink-3.2/onetimelink/presettings.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/static/css/site.css` & `django-onetimelink-3.2/onetimelink/static/css/site.css`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/static/js/jquery-3.4.1.min.js` & `django-onetimelink-3.2/onetimelink/static/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/static/js/jquery-3.4.1.min.map` & `django-onetimelink-3.2/onetimelink/static/js/jquery-3.4.1.min.map`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/templates/site.html` & `django-onetimelink-3.2/onetimelink/templates/site.html`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/test.py` & `django-onetimelink-3.2/onetimelink/test.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/onetimelink/views.py` & `django-onetimelink-3.2/onetimelink/views.py`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/setup.cfg` & `django-onetimelink-3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-onetimelink-3.1/setup.py` & `django-onetimelink-3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 if sys.version_info < (3, 8):
     REQUIRES.append('python >= 3.8')
 
 
 setup(
     name='django-onetimelink',
-    version=3.1,
+    version=3.2,
     description='A django one-time file streaming application',
     long_description=long_description,
     author='FENG Hao',
     author_email='hiroshifuu@outlook.com',
     url='https://github.com/HiroshiFuu/django-onetimelink',
     download_url='https://pypi.python.org/pypi/django-onetimelink',
     license='BSD',
```

