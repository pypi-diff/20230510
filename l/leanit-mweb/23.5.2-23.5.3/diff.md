# Comparing `tmp/leanit-mweb-23.5.2.tar.gz` & `tmp/leanit-mweb-23.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leanit-mweb-23.5.2.tar", last modified: Mon May  8 15:40:12 2023, max compression
+gzip compressed data, was "leanit-mweb-23.5.3.tar", last modified: Wed May 10 16:05:20 2023, max compression
```

## Comparing `leanit-mweb-23.5.2.tar` & `leanit-mweb-23.5.3.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-08 15:40:12.037685 leanit-mweb-23.5.2/
--rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.5.2/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      533 2023-05-08 15:40:12.033685 leanit-mweb-23.5.2/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)       24 2023-05-08 15:14:30.000000 leanit-mweb-23.5.2/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-08 15:40:12.033685 leanit-mweb-23.5.2/leanit_mweb/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1662 2023-05-08 15:37:40.000000 leanit-mweb-23.5.2/leanit_mweb/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.5.2/leanit_mweb/form.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-08 15:40:12.033685 leanit-mweb-23.5.2/leanit_mweb/jinja_template/
--rw-rw-r--   0 martin    (1000) martin    (1000)      851 2023-05-01 18:12:42.000000 leanit-mweb-23.5.2/leanit_mweb/jinja_template/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.5.2/leanit_mweb/jinja_template/loaders.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-08 15:40:12.033685 leanit-mweb-23.5.2/leanit_mweb/orm/
--rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.5.2/leanit_mweb/orm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.5.2/leanit_mweb/orm/exception.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      974 2023-05-08 15:37:40.000000 leanit-mweb-23.5.2/leanit_mweb/orm/fields.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6850 2023-05-08 15:37:40.000000 leanit-mweb-23.5.2/leanit_mweb/orm/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.5.2/leanit_mweb/orm/password.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.5.2/leanit_mweb/staticfiles.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-05-03 10:40:50.000000 leanit-mweb-23.5.2/leanit_mweb/thread.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      268 2023-05-07 11:18:08.000000 leanit-mweb-23.5.2/leanit_mweb/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6348 2023-05-08 15:37:40.000000 leanit-mweb-23.5.2/leanit_mweb/yuga.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-08 15:40:12.033685 leanit-mweb-23.5.2/leanit_mweb.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)      533 2023-05-08 15:40:11.000000 leanit-mweb-23.5.2/leanit_mweb.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      547 2023-05-08 15:40:12.000000 leanit-mweb-23.5.2/leanit_mweb.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-08 15:40:11.000000 leanit-mweb-23.5.2/leanit_mweb.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      178 2023-05-08 15:40:11.000000 leanit-mweb-23.5.2/leanit_mweb.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       12 2023-05-08 15:40:11.000000 leanit-mweb-23.5.2/leanit_mweb.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-08 15:40:12.037685 leanit-mweb-23.5.2/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1272 2023-05-08 15:40:11.000000 leanit-mweb-23.5.2/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 16:05:19.997005 leanit-mweb-23.5.3/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      962 2023-05-08 15:13:45.000000 leanit-mweb-23.5.3/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)      533 2023-05-10 16:05:19.993005 leanit-mweb-23.5.3/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)       24 2023-05-08 15:14:30.000000 leanit-mweb-23.5.3/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 16:05:19.993005 leanit-mweb-23.5.3/leanit_mweb/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1927 2023-05-10 15:58:26.000000 leanit-mweb-23.5.3/leanit_mweb/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      449 2023-05-08 06:49:29.000000 leanit-mweb-23.5.3/leanit_mweb/form.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 16:05:19.993005 leanit-mweb-23.5.3/leanit_mweb/jinja_template/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      851 2023-05-01 18:12:42.000000 leanit-mweb-23.5.3/leanit_mweb/jinja_template/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4134 2023-05-01 18:09:47.000000 leanit-mweb-23.5.3/leanit_mweb/jinja_template/loaders.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1814 2023-05-10 14:53:10.000000 leanit-mweb-23.5.3/leanit_mweb/manage.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 16:05:19.993005 leanit-mweb-23.5.3/leanit_mweb/orm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      150 2023-05-07 11:08:10.000000 leanit-mweb-23.5.3/leanit_mweb/orm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      205 2023-05-07 11:45:37.000000 leanit-mweb-23.5.3/leanit_mweb/orm/exception.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      974 2023-05-08 15:37:40.000000 leanit-mweb-23.5.3/leanit_mweb/orm/fields.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6850 2023-05-08 15:37:40.000000 leanit-mweb-23.5.3/leanit_mweb/orm/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      914 2023-05-07 12:15:52.000000 leanit-mweb-23.5.3/leanit_mweb/orm/password.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1060 2023-05-01 12:48:02.000000 leanit-mweb-23.5.3/leanit_mweb/staticfiles.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 16:05:19.993005 leanit-mweb-23.5.3/leanit_mweb/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      334 2023-05-10 14:53:10.000000 leanit-mweb-23.5.3/leanit_mweb/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2241 2023-05-03 10:40:50.000000 leanit-mweb-23.5.3/leanit_mweb/thread.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      268 2023-05-07 11:18:08.000000 leanit-mweb-23.5.3/leanit_mweb/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6350 2023-05-10 14:53:10.000000 leanit-mweb-23.5.3/leanit_mweb/yuga.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 16:05:19.993005 leanit-mweb-23.5.3/leanit_mweb.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      533 2023-05-10 16:05:19.000000 leanit-mweb-23.5.3/leanit_mweb.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      599 2023-05-10 16:05:19.000000 leanit-mweb-23.5.3/leanit_mweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-10 16:05:19.000000 leanit-mweb-23.5.3/leanit_mweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      191 2023-05-10 16:05:19.000000 leanit-mweb-23.5.3/leanit_mweb.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       12 2023-05-10 16:05:19.000000 leanit-mweb-23.5.3/leanit_mweb.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-05-10 16:05:19.997005 leanit-mweb-23.5.3/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1329 2023-05-10 16:05:19.000000 leanit-mweb-23.5.3/setup.py
```

### Comparing `leanit-mweb-23.5.2/LICENSE` & `leanit-mweb-23.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.2/PKG-INFO` & `leanit-mweb-23.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leanit-mweb
-Version: 23.5.2
+Version: 23.5.3
 Summary: Web framework
 Author: Martin Klapproth
 Author-email: martin.klapproth@staxnet.de
 Keywords: python,web
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `leanit-mweb-23.5.2/leanit_mweb/__init__.py` & `leanit-mweb-23.5.3/leanit_mweb/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,36 +16,41 @@
     pass
 
 config: Dict = None
 db: YugabytedbThreadPool = None
 loader: FileSystemLoader = None
 templates: Jinja2Templates = None
 
-def _read_config():
-    config_file = os.environ.get("CONFIG")
-    if not config_file:
-        config_file = f"{os.getcwd()}/config.yaml"
-    if not isabs(config_file):
-        config_file = abspath(config_file)
-
-    logger.info(f"Reading config from {config_file}")
-
-    # read yaml config
-    with open(config_file, "r") as f:
-        config = yaml.safe_load(f)
-    return config
+def _read_config(app_root: str) -> Dict:
+    config_data = {}
+    config_profile = os.environ.get("CONFIG_PROFILE", "default")
+    config_dir = f"{app_root}/etc/{config_profile}"
+
+    for config_file in os.listdir(config_dir):
+        # only read .yml and .yaml files
+        if not config_file.endswith(".yml") and not config_file.endswith(".yaml"):
+            continue
+        config_file_abs = f"{config_dir}/{config_file}"
+
+        logger.info(f"Reading config from {config_file_abs}")
+
+        # read yaml config
+        with open(config_file_abs, "r") as f:
+            config_data.update(yaml.safe_load(f))
+
+    return config_data
 
 
 def init(app_root: str):
     """
     :param app_root: path to the root of the application
     :return:
     """
     global config
-    config = _read_config()
+    config = _read_config(app_root)
 
     global db
     pool_config = config["db"].get("pool", {})
     db = YugabytedbThreadPool(
         min_workers=pool_config.get("min_workers", 1),
         max_workers=pool_config.get("max_workers", 10),
     )
```

### Comparing `leanit-mweb-23.5.2/leanit_mweb/jinja_template/__init__.py` & `leanit-mweb-23.5.3/leanit_mweb/jinja_template/__init__.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.2/leanit_mweb/jinja_template/loaders.py` & `leanit-mweb-23.5.3/leanit_mweb/jinja_template/loaders.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.2/leanit_mweb/orm/fields.py` & `leanit-mweb-23.5.3/leanit_mweb/orm/fields.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.2/leanit_mweb/orm/model.py` & `leanit-mweb-23.5.3/leanit_mweb/orm/model.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.2/leanit_mweb/orm/password.py` & `leanit-mweb-23.5.3/leanit_mweb/orm/password.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.2/leanit_mweb/staticfiles.py` & `leanit-mweb-23.5.3/leanit_mweb/staticfiles.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.2/leanit_mweb/thread.py` & `leanit-mweb-23.5.3/leanit_mweb/thread.py`

 * *Files identical despite different names*

### Comparing `leanit-mweb-23.5.2/leanit_mweb/yuga.py` & `leanit-mweb-23.5.3/leanit_mweb/yuga.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     kwargs = dict(
         dbname=leanit_mweb.config['db']['dbname'],
         host=leanit_mweb.config['db']['host'],
         port=leanit_mweb.config['db']['port'],
         user=leanit_mweb.config['db']['user'],
         password=leanit_mweb.config['db']['password'],
-        load_balance='true',
+        # load_balance='true',
     )
     if 'sslmode' in leanit_mweb.config['db']:
         kwargs['sslmode'] = leanit_mweb.config['db']['sslmode']
     if 'sslcert' in leanit_mweb.config['db']:
         sslcert = leanit_mweb.config['db']['sslcert']
         if"BEGIN CERTIFICATE" in sslcert:
             # assume it's a certificate
```

### Comparing `leanit-mweb-23.5.2/leanit_mweb.egg-info/PKG-INFO` & `leanit-mweb-23.5.3/leanit_mweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leanit-mweb
-Version: 23.5.2
+Version: 23.5.3
 Summary: Web framework
 Author: Martin Klapproth
 Author-email: martin.klapproth@staxnet.de
 Keywords: python,web
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `leanit-mweb-23.5.2/leanit_mweb.egg-info/SOURCES.txt` & `leanit-mweb-23.5.3/leanit_mweb.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 leanit_mweb/__init__.py
 leanit_mweb/form.py
+leanit_mweb/manage.py
 leanit_mweb/staticfiles.py
 leanit_mweb/thread.py
 leanit_mweb/utils.py
 leanit_mweb/yuga.py
 leanit_mweb.egg-info/PKG-INFO
 leanit_mweb.egg-info/SOURCES.txt
 leanit_mweb.egg-info/dependency_links.txt
@@ -14,8 +15,9 @@
 leanit_mweb.egg-info/top_level.txt
 leanit_mweb/jinja_template/__init__.py
 leanit_mweb/jinja_template/loaders.py
 leanit_mweb/orm/__init__.py
 leanit_mweb/orm/exception.py
 leanit_mweb/orm/fields.py
 leanit_mweb/orm/model.py
-leanit_mweb/orm/password.py
+leanit_mweb/orm/password.py
+leanit_mweb/tests/__init__.py
```

### Comparing `leanit-mweb-23.5.2/setup.py` & `leanit-mweb-23.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '23.5.2'
+VERSION = '23.5.3'
 DESCRIPTION = 'Web framework'
 LONG_DESCRIPTION = 'Web framework'
 
 # Setting up
 setup(
     name="leanit-mweb",
     version=VERSION,
@@ -29,14 +29,17 @@
         'python-multipart~=0.0',
         'wtforms~=3.0',
         'email_validator~=2.0',
         'multidict~=6.0',
         'psycopg2-yugabytedb~=2.9',
         'PyYAML~=6.0',
         'python-ulid~=1.1',
+        # for testing
+        'pytest',
+        'httpx',
     ],
     keywords=['python', 'web'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

