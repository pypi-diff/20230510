# Comparing `tmp/pysearchconsole-1.0.4.tar.gz` & `tmp/pysearchconsole-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysearchconsole-1.0.4.tar", last modified: Fri May  5 09:10:20 2023, max compression
+gzip compressed data, was "pysearchconsole-1.0.5.tar", last modified: Wed May 10 06:00:27 2023, max compression
```

## Comparing `pysearchconsole-1.0.4.tar` & `pysearchconsole-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     5149 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/PKG-INFO
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4074 2023-05-05 08:58:27.000000 pysearchconsole-1.0.4/README.md
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       38 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/setup.cfg
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1516 2023-05-05 09:09:58.000000 pysearchconsole-1.0.4/setup.py
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/src/
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/src/credential/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 12:49:16.000000 pysearchconsole-1.0.4/src/credential/__init__.py
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     2331 2023-05-04 14:17:57.000000 pysearchconsole-1.0.4/src/credential/credential.py
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     5149 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/PKG-INFO
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)      353 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/SOURCES.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        1 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/dependency_links.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       57 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/requires.txt
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       25 2023-05-05 09:10:20.000000 pysearchconsole-1.0.4/src/pysearchconsole.egg-info/top_level.txt
-drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-05 09:10:20.925138 pysearchconsole-1.0.4/src/searchconsole/
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 13:47:17.000000 pysearchconsole-1.0.4/src/searchconsole/__init__.py
--rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1711 2023-05-04 14:28:31.000000 pysearchconsole-1.0.4/src/searchconsole/searchconsole.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-10 06:00:27.765957 pysearchconsole-1.0.5/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     5149 2023-05-10 06:00:27.765957 pysearchconsole-1.0.5/PKG-INFO
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     4074 2023-05-05 08:58:27.000000 pysearchconsole-1.0.5/README.md
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       38 2023-05-10 06:00:27.765957 pysearchconsole-1.0.5/setup.cfg
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1495 2023-05-10 05:58:52.000000 pysearchconsole-1.0.5/setup.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-10 06:00:27.761957 pysearchconsole-1.0.5/src/
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-10 06:00:27.761957 pysearchconsole-1.0.5/src/credential/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 12:49:16.000000 pysearchconsole-1.0.5/src/credential/__init__.py
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     2331 2023-05-04 14:17:57.000000 pysearchconsole-1.0.5/src/credential/credential.py
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-10 06:00:27.765957 pysearchconsole-1.0.5/src/pysearchconsole.egg-info/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     5149 2023-05-10 06:00:27.000000 pysearchconsole-1.0.5/src/pysearchconsole.egg-info/PKG-INFO
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)      353 2023-05-10 06:00:27.000000 pysearchconsole-1.0.5/src/pysearchconsole.egg-info/SOURCES.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        1 2023-05-10 06:00:27.000000 pysearchconsole-1.0.5/src/pysearchconsole.egg-info/dependency_links.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       47 2023-05-10 06:00:27.000000 pysearchconsole-1.0.5/src/pysearchconsole.egg-info/requires.txt
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)       25 2023-05-10 06:00:27.000000 pysearchconsole-1.0.5/src/pysearchconsole.egg-info/top_level.txt
+drwxrwxr-x   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-10 06:00:27.765957 pysearchconsole-1.0.5/src/searchconsole/
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)        0 2023-05-04 13:47:17.000000 pysearchconsole-1.0.5/src/searchconsole/__init__.py
+-rw-rw-r--   0 rahul.katoch (1988105343) rahul.katoch (1988105343)     1711 2023-05-04 14:28:31.000000 pysearchconsole-1.0.5/src/searchconsole/searchconsole.py
```

### Comparing `pysearchconsole-1.0.4/PKG-INFO` & `pysearchconsole-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysearchconsole
-Version: 1.0.4
+Version: 1.0.5
 Summary: PySearchConsole is a Python library that  allows you to get query and analyze data from your website's Search Console account, including search analytics, crawl errors, sitemaps, and more.
 Home-page: https://github.com/Rahulkatoch99/py_searchconsole
 Author: Rahul Katoch, Harish kumar
 Author-email: rahulkatoch99@gmail.com
 Maintainer-email: rahulkatoch99@gmail.com, echkayweb@gmail.com
 License: MIT
 Keywords: search console api google seo python libraries API integration web traffic analysis
```

### Comparing `pysearchconsole-1.0.4/README.md` & `pysearchconsole-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pysearchconsole-1.0.4/setup.py` & `pysearchconsole-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pysearchconsole',
-    version='1.0.4',
+    version='1.0.5',
     description="PySearchConsole is a Python library that  allows you to get query and analyze data from your website's Search Console account, including search analytics, crawl errors, sitemaps, and more.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Rahul Katoch, Harish kumar',
     author_email='rahulkatoch99@gmail.com',
     maintainer_email='rahulkatoch99@gmail.com, echkayweb@gmail.com',
     url='https://github.com/Rahulkatoch99/py_searchconsole',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
-        'apiclient',
         'google-api-python-client',
         'httplib2',
         'oauth2client'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

### Comparing `pysearchconsole-1.0.4/src/credential/credential.py` & `pysearchconsole-1.0.5/src/credential/credential.py`

 * *Files identical despite different names*

### Comparing `pysearchconsole-1.0.4/src/pysearchconsole.egg-info/PKG-INFO` & `pysearchconsole-1.0.5/src/pysearchconsole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysearchconsole
-Version: 1.0.4
+Version: 1.0.5
 Summary: PySearchConsole is a Python library that  allows you to get query and analyze data from your website's Search Console account, including search analytics, crawl errors, sitemaps, and more.
 Home-page: https://github.com/Rahulkatoch99/py_searchconsole
 Author: Rahul Katoch, Harish kumar
 Author-email: rahulkatoch99@gmail.com
 Maintainer-email: rahulkatoch99@gmail.com, echkayweb@gmail.com
 License: MIT
 Keywords: search console api google seo python libraries API integration web traffic analysis
```

### Comparing `pysearchconsole-1.0.4/src/searchconsole/searchconsole.py` & `pysearchconsole-1.0.5/src/searchconsole/searchconsole.py`

 * *Files identical despite different names*

