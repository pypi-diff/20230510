# Comparing `tmp/time-stamped-model-0.2.3.tar.gz` & `tmp/time-stamped-model-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time-stamped-model-0.2.3.tar", last modified: Mon Jun 20 14:34:52 2022, max compression
+gzip compressed data, was "time-stamped-model-0.2.4.tar", last modified: Wed May 10 13:48:03 2023, max compression
```

## Comparing `time-stamped-model-0.2.3.tar` & `time-stamped-model-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-06-20 14:34:52.363947 time-stamped-model-0.2.3/
--rw-r--r--   0 tom        (501) staff       (20)     1077 2021-07-22 13:24:36.000000 time-stamped-model-0.2.3/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       81 2021-07-22 14:40:12.000000 time-stamped-model-0.2.3/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)     1083 2022-06-20 14:34:52.363503 time-stamped-model-0.2.3/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      615 2021-07-22 15:12:43.000000 time-stamped-model-0.2.3/README.md
--rw-r--r--   0 tom        (501) staff       (20)       38 2022-06-20 14:34:52.364078 time-stamped-model-0.2.3/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      668 2022-06-20 14:26:41.000000 time-stamped-model-0.2.3/setup.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-06-20 14:34:52.361614 time-stamped-model-0.2.3/time_stamped_model/
--rw-r--r--   0 tom        (501) staff       (20)     6148 2021-07-22 13:26:06.000000 time-stamped-model-0.2.3/time_stamped_model/.DS_Store
--rw-r--r--   0 tom        (501) staff       (20)        1 2021-07-22 14:40:41.000000 time-stamped-model-0.2.3/time_stamped_model/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)       98 2021-07-22 13:30:24.000000 time-stamped-model-0.2.3/time_stamped_model/apps.py
--rwxr-xr-x   0 tom        (501) staff       (20)     5709 2022-06-20 14:26:41.000000 time-stamped-model-0.2.3/time_stamped_model/models.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2022-06-20 14:34:52.362896 time-stamped-model-0.2.3/time_stamped_model.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     1083 2022-06-20 14:34:52.000000 time-stamped-model-0.2.3/time_stamped_model.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      322 2022-06-20 14:34:52.000000 time-stamped-model-0.2.3/time_stamped_model.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2022-06-20 14:34:52.000000 time-stamped-model-0.2.3/time_stamped_model.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)       19 2022-06-20 14:34:52.000000 time-stamped-model-0.2.3/time_stamped_model.egg-info/top_level.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-10 13:48:03.841383 time-stamped-model-0.2.4/
+-rw-r--r--   0 tom        (501) staff       (20)     1077 2023-05-10 13:37:31.000000 time-stamped-model-0.2.4/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       81 2023-05-10 13:37:31.000000 time-stamped-model-0.2.4/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)     1083 2023-05-10 13:48:03.841223 time-stamped-model-0.2.4/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      615 2023-05-10 13:37:31.000000 time-stamped-model-0.2.4/README.md
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-05-10 13:48:03.841419 time-stamped-model-0.2.4/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      668 2023-05-10 13:46:41.000000 time-stamped-model-0.2.4/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-10 13:48:03.839329 time-stamped-model-0.2.4/time_stamped_model/
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-10 13:37:31.000000 time-stamped-model-0.2.4/time_stamped_model/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)       98 2023-05-10 13:37:31.000000 time-stamped-model-0.2.4/time_stamped_model/apps.py
+-rwxr-xr-x   0 tom        (501) staff       (20)     6338 2023-05-10 13:45:20.000000 time-stamped-model-0.2.4/time_stamped_model/models.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-05-10 13:48:03.840911 time-stamped-model-0.2.4/time_stamped_model.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     1083 2023-05-10 13:48:03.000000 time-stamped-model-0.2.4/time_stamped_model.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      293 2023-05-10 13:48:03.000000 time-stamped-model-0.2.4/time_stamped_model.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-05-10 13:48:03.000000 time-stamped-model-0.2.4/time_stamped_model.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       19 2023-05-10 13:48:03.000000 time-stamped-model-0.2.4/time_stamped_model.egg-info/top_level.txt
```

### Comparing `time-stamped-model-0.2.3/LICENSE` & `time-stamped-model-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `time-stamped-model-0.2.3/PKG-INFO` & `time-stamped-model-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-stamped-model
-Version: 0.2.3
+Version: 0.2.4
 Summary: Django app to add created and modified
 Home-page: https://github.com/django-advance-utils/time-stamped-model
 Author: Tom Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `time-stamped-model-0.2.3/README.md` & `time-stamped-model-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `time-stamped-model-0.2.3/setup.py` & `time-stamped-model-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="time-stamped-model",
-    version="0.2.3",
+    version="0.2.4",
     author="Tom Turner",
     description="Django app to add created and modified",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/time-stamped-model",
     include_package_data=True,
     packages=['time_stamped_model'],
```

### Comparing `time-stamped-model-0.2.3/time_stamped_model/models.py` & `time-stamped-model-0.2.4/time_stamped_model/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,16 @@
         """
         Using this method allows one to set the modified date manually. This is useful when importing data.
         """
         # noinspection PyAttributeOutsideInit
         self.update_modified = False
         self.modified = modified_date
 
-    def make_new_slug(self, obj=None, name=None, on_edit=False, allow_dashes=True, extra_filters=None):
+    def make_new_slug(self, obj=None, name=None, on_edit=False, allow_dashes=True, extra_filters=None,
+                      exclude_list=None):
         """
         This allow you to populate a slug field. You need to call this function from model save. Only works if you add
         slug = models.SlugField(unique=True)
         on the model
 
         the add
         def save(self, *args, **kwargs):
@@ -108,14 +109,15 @@
             super().save(*args, **kwargs)
 
         :param obj: The class name can be none and it will sort it self out
         :param name: The field to make the slug from
         :param on_edit
         :param allow_dashes:
         :param extra_filters:   this allow for unique together
+        :param exclude_list:   exclude certain slugs
         """
         if obj is None:
             obj = self.__class__
 
         if extra_filters is None:
             extra_filters = {}
 
@@ -128,18 +130,33 @@
 
             if main_slug == '':
                 main_slug = str(uuid.uuid4())
             if not allow_dashes:
                 main_slug = main_slug.replace('-', '_')
             slug = main_slug
             count = 1
+            if exclude_list is not None:
+                while True:
+                    if slug in exclude_list:
+                        slug = f'{slug}{count}'
+                        count += 1
+                    else:
+                        break
+
             while obj.objects.filter(slug=slug, **extra_filters).exists():
                 slug = slugify("%s %d" % (main_slug, count))
                 if not allow_dashes:
                     slug = slug.replace('-', '_')
+                if exclude_list is not None:
+                    while True:
+                        if slug in exclude_list:
+                            slug = f'{slug}{count}'
+                            count += 1
+                        else:
+                            break
                 count += 1
             self.slug = slug
         elif self.pk and on_edit:
             main_slug = slugify(name)[:45]  # limits the slug to 45 chars as slug use 50
             if not allow_dashes:
                 main_slug = main_slug.replace('-', '_')
             slug = main_slug
```

### Comparing `time-stamped-model-0.2.3/time_stamped_model.egg-info/PKG-INFO` & `time-stamped-model-0.2.4/time_stamped_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-stamped-model
-Version: 0.2.3
+Version: 0.2.4
 Summary: Django app to add created and modified
 Home-page: https://github.com/django-advance-utils/time-stamped-model
 Author: Tom Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

