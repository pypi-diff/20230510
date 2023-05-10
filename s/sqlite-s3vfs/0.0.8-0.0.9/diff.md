# Comparing `tmp/sqlite-s3vfs-0.0.8.tar.gz` & `tmp/sqlite-s3vfs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite-s3vfs-0.0.8.tar", last modified: Fri Oct  1 15:52:35 2021, max compression
+gzip compressed data, was "sqlite-s3vfs-0.0.9.tar", last modified: Sat Oct  2 09:59:46 2021, max compression
```

## Comparing `sqlite-s3vfs-0.0.8.tar` & `sqlite-s3vfs-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-10-01 15:52:35.977994 sqlite-s3vfs-0.0.8/
--rw-r--r--   0 dituser    (501) staff       (20)     2918 2021-10-01 15:52:35.977682 sqlite-s3vfs-0.0.8/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)     2429 2021-10-01 09:07:32.000000 sqlite-s3vfs-0.0.8/README.md
--rw-r--r--   0 dituser    (501) staff       (20)       38 2021-10-01 15:52:35.978081 sqlite-s3vfs-0.0.8/setup.cfg
--rw-r--r--   0 dituser    (501) staff       (20)      781 2021-10-01 15:51:59.000000 sqlite-s3vfs-0.0.8/setup.py
-drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-10-01 15:52:35.977291 sqlite-s3vfs-0.0.8/sqlite_s3vfs.egg-info/
--rw-r--r--   0 dituser    (501) staff       (20)     2918 2021-10-01 15:52:35.000000 sqlite-s3vfs-0.0.8/sqlite_s3vfs.egg-info/PKG-INFO
--rw-r--r--   0 dituser    (501) staff       (20)      213 2021-10-01 15:52:35.000000 sqlite-s3vfs-0.0.8/sqlite_s3vfs.egg-info/SOURCES.txt
--rw-r--r--   0 dituser    (501) staff       (20)        1 2021-10-01 15:52:35.000000 sqlite-s3vfs-0.0.8/sqlite_s3vfs.egg-info/dependency_links.txt
--rw-r--r--   0 dituser    (501) staff       (20)       15 2021-10-01 15:52:35.000000 sqlite-s3vfs-0.0.8/sqlite_s3vfs.egg-info/requires.txt
--rw-r--r--   0 dituser    (501) staff       (20)       13 2021-10-01 15:52:35.000000 sqlite-s3vfs-0.0.8/sqlite_s3vfs.egg-info/top_level.txt
--rw-r--r--   0 dituser    (501) staff       (20)     4673 2021-10-01 15:49:33.000000 sqlite-s3vfs-0.0.8/sqlite_s3vfs.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-10-02 09:59:46.740192 sqlite-s3vfs-0.0.9/
+-rw-r--r--   0 dituser    (501) staff       (20)     2918 2021-10-02 09:59:46.739852 sqlite-s3vfs-0.0.9/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)     2429 2021-10-01 09:07:32.000000 sqlite-s3vfs-0.0.9/README.md
+-rw-r--r--   0 dituser    (501) staff       (20)       38 2021-10-02 09:59:46.740311 sqlite-s3vfs-0.0.9/setup.cfg
+-rw-r--r--   0 dituser    (501) staff       (20)      781 2021-10-02 09:58:23.000000 sqlite-s3vfs-0.0.9/setup.py
+drwxr-xr-x   0 dituser    (501) staff       (20)        0 2021-10-02 09:59:46.739470 sqlite-s3vfs-0.0.9/sqlite_s3vfs.egg-info/
+-rw-r--r--   0 dituser    (501) staff       (20)     2918 2021-10-02 09:59:46.000000 sqlite-s3vfs-0.0.9/sqlite_s3vfs.egg-info/PKG-INFO
+-rw-r--r--   0 dituser    (501) staff       (20)      213 2021-10-02 09:59:46.000000 sqlite-s3vfs-0.0.9/sqlite_s3vfs.egg-info/SOURCES.txt
+-rw-r--r--   0 dituser    (501) staff       (20)        1 2021-10-02 09:59:46.000000 sqlite-s3vfs-0.0.9/sqlite_s3vfs.egg-info/dependency_links.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       15 2021-10-02 09:59:46.000000 sqlite-s3vfs-0.0.9/sqlite_s3vfs.egg-info/requires.txt
+-rw-r--r--   0 dituser    (501) staff       (20)       13 2021-10-02 09:59:46.000000 sqlite-s3vfs-0.0.9/sqlite_s3vfs.egg-info/top_level.txt
+-rw-r--r--   0 dituser    (501) staff       (20)     4698 2021-10-02 09:58:12.000000 sqlite-s3vfs-0.0.9/sqlite_s3vfs.py
```

### Comparing `sqlite-s3vfs-0.0.8/PKG-INFO` & `sqlite-s3vfs-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-s3vfs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Virtual filesystem for SQLite to read from and write to S3
 Home-page: https://github.com/uktrade/sqlite-s3vfs
 Author: Department for International Trade
 Author-email: sre@digital.trade.gov.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlite-s3vfs-0.0.8/README.md` & `sqlite-s3vfs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sqlite-s3vfs-0.0.8/setup.py` & `sqlite-s3vfs-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
 
 setuptools.setup(
     name='sqlite-s3vfs',
-    version='0.0.8',
+    version='0.0.9',
     author='Department for International Trade',
     author_email='sre@digital.trade.gov.uk',
     description='Virtual filesystem for SQLite to read from and write to S3',
     long_description=long_description(),
     long_description_content_type='text/markdown',
     url='https://github.com/uktrade/sqlite-s3vfs',
     classifiers=[
```

### Comparing `sqlite-s3vfs-0.0.8/sqlite_s3vfs.egg-info/PKG-INFO` & `sqlite-s3vfs-0.0.9/sqlite_s3vfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-s3vfs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Virtual filesystem for SQLite to read from and write to S3
 Home-page: https://github.com/uktrade/sqlite-s3vfs
 Author: Department for International Trade
 Author-email: sre@digital.trade.gov.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sqlite-s3vfs-0.0.8/sqlite_s3vfs.py` & `sqlite-s3vfs-0.0.9/sqlite_s3vfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     def xFileSize(self):
         return sum(o.size for o in self._bucket.objects.filter(Prefix=self._key_prefix + "/"))
 
     def xSync(self, flags):
         return True
 
     def xTruncate(self, newsize):
-        num_blocks = newsize // self._block_size
+        num_blocks = (newsize + self._block_size - 1) // self._block_size
         for obj in self._bucket.objects.filter(Prefix=self._key_prefix + "/"):
             block = int(obj.key[-10:])
             if block >= num_blocks:
                 obj.delete()
         return True
 
     def xWrite(self, data, offset):
```

