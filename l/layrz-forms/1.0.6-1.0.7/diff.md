# Comparing `tmp/layrz-forms-1.0.6.tar.gz` & `tmp/layrz-forms-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-forms-1.0.6.tar", last modified: Mon May  8 17:20:48 2023, max compression
+gzip compressed data, was "layrz-forms-1.0.7.tar", last modified: Wed May 10 00:46:44 2023, max compression
```

## Comparing `layrz-forms-1.0.6.tar` & `layrz-forms-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:20:48.694725 layrz-forms-1.0.6/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-08 17:20:48.693724 layrz-forms-1.0.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:20:48.689724 layrz-forms-1.0.6/layrz/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:20:48.689724 layrz-forms-1.0.6/layrz/forms/
--rw-rw-rw-   0 root         (0) root         (0)     5934 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:20:48.692724 layrz-forms-1.0.6/layrz/forms/fields/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/fields/base.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/fields/boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/fields/char.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/fields/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/fields/id.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/fields/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/layrz/forms/fields/number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 17:20:48.693724 layrz-forms-1.0.6/layrz_forms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-08 17:20:48.000000 layrz-forms-1.0.6/layrz_forms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-08 17:20:48.000000 layrz-forms-1.0.6/layrz_forms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 17:20:48.000000 layrz-forms-1.0.6/layrz_forms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 17:20:48.000000 layrz-forms-1.0.6/layrz_forms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 17:20:48.694725 layrz-forms-1.0.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-08 17:20:38.000000 layrz-forms-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.331884 layrz-forms-1.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-10 00:46:44.330884 layrz-forms-1.0.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.325883 layrz-forms-1.0.7/layrz/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.326883 layrz-forms-1.0.7/layrz/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     5934 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.329884 layrz-forms-1.0.7/layrz/forms/fields/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/char.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/layrz/forms/fields/number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 00:46:44.330884 layrz-forms-1.0.7/layrz_forms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-10 00:46:44.000000 layrz-forms-1.0.7/layrz_forms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-10 00:46:44.000000 layrz-forms-1.0.7/layrz_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 00:46:44.000000 layrz-forms-1.0.7/layrz_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-10 00:46:44.000000 layrz-forms-1.0.7/layrz_forms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 00:46:44.331884 layrz-forms-1.0.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-10 00:46:34.000000 layrz-forms-1.0.7/setup.py
```

### Comparing `layrz-forms-1.0.6/LICENSE` & `layrz-forms-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/PKG-INFO` & `layrz-forms-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.6
+Version: 1.0.7
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.6/README.md` & `layrz-forms-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/layrz/forms/__init__.py` & `layrz-forms-1.0.7/layrz/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/layrz/forms/fields/base.py` & `layrz-forms-1.0.7/layrz/forms/fields/base.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/layrz/forms/fields/boolean.py` & `layrz-forms-1.0.7/layrz/forms/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/layrz/forms/fields/char.py` & `layrz-forms-1.0.7/layrz/forms/fields/char.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,17 +82,18 @@
               'code': 'minLength',
               'expected': self.min_length,
               'received': len(value),
             },
           )
 
       if self.choices is not None:
-        if value not in self.choices:
+        mapped_choices = [choice[0] for choice in self.choices]
+        if value not in mapped_choices:
           self._append_error(
             key=key,
             errors=errors,
             to_add={
               'code': 'invalidChoice',
-              'expected': self.choices,
+              'expected': mapped_choices,
               'received': value,
             },
           )
```

### Comparing `layrz-forms-1.0.6/layrz/forms/fields/email.py` & `layrz-forms-1.0.7/layrz/forms/fields/email.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/layrz/forms/fields/id.py` & `layrz-forms-1.0.7/layrz/forms/fields/id.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/layrz/forms/fields/json.py` & `layrz-forms-1.0.7/layrz/forms/fields/json.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/layrz/forms/fields/number.py` & `layrz-forms-1.0.7/layrz/forms/fields/number.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.6/layrz_forms.egg-info/PKG-INFO` & `layrz-forms-1.0.7/layrz_forms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.6
+Version: 1.0.7
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.6/setup.py` & `layrz-forms-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   """ Return long description """
   with open('README.md', 'r', encoding='utf-8') as fh:
     return fh.read()
 
 
 setuptools.setup(
   name="layrz-forms",
-  version="1.0.6",
+  version="1.0.7",
   author="Golden M",
   author_email="software@goldenmcorp.com",
   description="Layrz forms and tools for Python",
   long_description=long_description(),
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

