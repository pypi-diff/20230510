# Comparing `tmp/django_shopify_app-1.1.3.tar.gz` & `tmp/django_shopify_app-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_shopify_app-1.1.3.tar", last modified: Sat Feb 18 20:11:00 2023, max compression
+gzip compressed data, was "django_shopify_app-1.1.4.tar", last modified: Wed May 10 03:54:45 2023, max compression
```

## Comparing `django_shopify_app-1.1.3.tar` & `django_shopify_app-1.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.031853 django_shopify_app-1.1.3/django_shopify_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-02-18 20:11:00.000000 django_shopify_app-1.1.3/django_shopify_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-18 20:11:00.000000 django_shopify_app-1.1.3/django_shopify_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 20:11:00.000000 django_shopify_app-1.1.3/django_shopify_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-18 20:11:00.000000 django_shopify_app-1.1.3/django_shopify_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-18 20:11:00.000000 django_shopify_app-1.1.3/django_shopify_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/management/commands/run_shopify_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/management/commands/update_shop_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/services/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/templates/shopify_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/templates/shopify_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/templates/shopify_app/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 20:11:00.035853 django_shopify_app-1.1.3/shopify_app/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-02-18 20:10:48.000000 django_shopify_app-1.1.3/shopify_app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.178917 django_shopify_app-1.1.4/django_shopify_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 03:54:45.000000 django_shopify_app-1.1.4/django_shopify_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/management/commands/run_shopify_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/management/commands/update_shop_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/services/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/templates/shopify_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/templates/shopify_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/templates/shopify_app/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:54:45.182917 django_shopify_app-1.1.4/shopify_app/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-10 03:54:33.000000 django_shopify_app-1.1.4/shopify_app/views.py
```

### Comparing `django_shopify_app-1.1.3/PKG-INFO` & `django_shopify_app-1.1.4/django_shopify_app.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django_shopify_app
-Version: 1.1.3
+Name: django-shopify-app
+Version: 1.1.4
 Summary: A django app with all the tools required to make a Shopify app
 Home-page: http://pypi.python.org/pypi/django_shopify_app/
 Author: Moship
 Author-email: hello@moship.io
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `django_shopify_app-1.1.3/README.md` & `django_shopify_app-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/django_shopify_app.egg-info/PKG-INFO` & `django_shopify_app-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: django-shopify-app
-Version: 1.1.3
+Name: django_shopify_app
+Version: 1.1.4
 Summary: A django app with all the tools required to make a Shopify app
 Home-page: http://pypi.python.org/pypi/django_shopify_app/
 Author: Moship
 Author-email: hello@moship.io
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `django_shopify_app-1.1.3/django_shopify_app.egg-info/SOURCES.txt` & `django_shopify_app-1.1.4/django_shopify_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/setup.py` & `django_shopify_app-1.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='django_shopify_app',
-    version='1.1.3',
+    version='1.1.4',
     author='Moship',
     author_email='hello@moship.io',
     packages=find_packages(),
     scripts=[],
     url='http://pypi.python.org/pypi/django_shopify_app/',
     license="MIT",
     description='A django app with all the tools required to make a Shopify app',
```

### Comparing `django_shopify_app-1.1.3/shopify_app/apps.py` & `django_shopify_app-1.1.4/shopify_app/apps.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/shopify_app/decorators.py` & `django_shopify_app-1.1.4/shopify_app/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,29 +32,38 @@
 
 def shop_session(func):
 
     def wrapper(*args, **kwargs):
         try:
 
             request = args[0]
+
             authorization_header = request.META.get("HTTP_SHOPIFYAUTH")
+            if (
+                not authorization_header
+                and request.user.is_authenticated
+                and request.user.is_admin
+            ):
+                print('user is admin')
 
             app_config = apps.get_app_config("shopify_app")
             decoded_session_token = session_token.decode_from_header(
                 authorization_header=authorization_header,
                 api_key=app_config.SHOPIFY_API_KEY,
                 secret=app_config.SHOPIFY_API_SECRET,
             )
 
             shopify_domain = decoded_session_token.get("dest")
             shopify_domain = shopify_domain.removeprefix("https://")
 
             check_shop_domain(request, kwargs, shopify_domain)
             check_shop_known(request, kwargs)
 
+            kwargs['shopify_user_id'] = decoded_session_token['sub']
+
             return func(*args, **kwargs)
 
         except session_token.SessionTokenError:
             return HttpResponse(status=401)
 
     return wrapper
```

### Comparing `django_shopify_app-1.1.3/shopify_app/management/commands/run_shopify_pubsub.py` & `django_shopify_app-1.1.4/shopify_app/management/commands/run_shopify_pubsub.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/shopify_app/management/commands/update_shop_webhooks.py` & `django_shopify_app-1.1.4/shopify_app/management/commands/update_shop_webhooks.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/shopify_app/models.py` & `django_shopify_app-1.1.4/shopify_app/models.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/shopify_app/services/webhooks.py` & `django_shopify_app-1.1.4/shopify_app/services/webhooks.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/shopify_app/templates/shopify_app/index.html` & `django_shopify_app-1.1.4/shopify_app/templates/shopify_app/index.html`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/shopify_app/urls.py` & `django_shopify_app-1.1.4/shopify_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/shopify_app/utils/__init__.py` & `django_shopify_app-1.1.4/shopify_app/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django_shopify_app-1.1.3/shopify_app/views.py` & `django_shopify_app-1.1.4/shopify_app/views.py`

 * *Files identical despite different names*

