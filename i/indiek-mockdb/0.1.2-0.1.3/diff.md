# Comparing `tmp/indiek-mockdb-0.1.2.tar.gz` & `tmp/indiek-mockdb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-mockdb/dist/.tmp-nnicdprj/indiek-mockdb-0.1.2.tar", last modified: Sun May  7 13:31:15 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-mockdb/dist/.tmp-ltlhbuh_/indiek-mockdb-0.1.3.tar", last modified: Tue May  9 22:07:37 2023, max compression
```

## Comparing `indiek-mockdb-0.1.2.tar` & `indiek-mockdb-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-16 01:06:17.000000 indiek-mockdb-0.1.2/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/PKG-INFO
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.081183 indiek-mockdb-0.1.2/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/indiek/mockdb/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-04-16 01:07:43.000000 indiek-mockdb-0.1.2/indiek/mockdb/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3460 2023-05-06 13:46:41.000000 indiek-mockdb-0.1.2/indiek/mockdb/items.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      279 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       37 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-07 13:31:15.000000 indiek-mockdb-0.1.2/indiek_mockdb.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      618 2023-05-05 21:52:52.000000 indiek-mockdb-0.1.2/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:31:15.097184 indiek-mockdb-0.1.2/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1292 2023-05-06 13:44:24.000000 indiek-mockdb-0.1.2/tests/test_items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-16 01:06:17.000000 indiek-mockdb-0.1.3/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/PKG-INFO
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.829270 indiek-mockdb-0.1.3/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/indiek/mockdb/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-04-16 01:07:43.000000 indiek-mockdb-0.1.3/indiek/mockdb/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     5878 2023-05-08 22:01:42.000000 indiek-mockdb-0.1.3/indiek/mockdb/items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      458 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      279 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       37 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-09 22:07:37.000000 indiek-mockdb-0.1.3/indiek_mockdb.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      618 2023-05-07 14:33:45.000000 indiek-mockdb-0.1.3/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:07:37.857270 indiek-mockdb-0.1.3/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1338 2023-05-07 18:04:47.000000 indiek-mockdb-0.1.3/tests/test_items.py
```

### Comparing `indiek-mockdb-0.1.2/LICENSE` & `indiek-mockdb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-mockdb-0.1.2/setup.py` & `indiek-mockdb-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(name='indiek-mockdb',
       python_requires='>=3.8',
-      version='0.1.2',
+      version='0.1.3',
       description='mock database for indiek',
       long_description='''This is an on-the-fly in-memory mock Database used by indiek-core
       for development and testing purposes. The versioning of this library is locked with that
       of indiek-core.''',
       author='Adrian Ernesto Radillo',
       author_email='adrian.radillo@gmail.com',
       license='GNU Affero General Public License v3.0',
```

### Comparing `indiek-mockdb-0.1.2/tests/test_items.py` & `indiek-mockdb-0.1.3/tests/test_items.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import unittest
-from indiek.mockdb.items import Item
+from indiek.mockdb.items import Definition, Theorem, Proof
 
 
 class TestItemAttr(unittest.TestCase):
     def test_instantiation(self):
         """Test that mockdb Item has the attr specified by indiek-core API."""
 
-        item = Item()
+        item = Theorem()
         expected_attr = [
             'name',
             'content',
             '_ikid',
             'to_dict'
         ]
         for attr_name in expected_attr:
             self.assertTrue(hasattr(item, attr_name))
 
+
 class TestItemIO(unittest.TestCase):
     def test_write_read(self):
         item1_dict = {'name': 'item1', 'content': 'blabla'}
-        item1 = Item(**item1_dict)
+        item1 = Definition(**item1_dict)
         item1_dict['_ikid'] = item1.save()
 
         item2_dict = dict(name='item2', content='nslkdf')
-        item2 = Item(**item2_dict)
+        item2 = Theorem(**item2_dict)
         item2_dict['_ikid'] = item2.save()
         del item1, item2
 
-        item1 = Item.load(item1_dict['_ikid'])
+        item1 = Definition.load(item1_dict['_ikid'])
         self.assertDictEqual(item1.to_dict(), item1_dict)
 
-        item2 = Item.load(item2_dict['_ikid'])
+        item2 = Theorem.load(item2_dict['_ikid'])
         self.assertDictEqual(item2.to_dict(), item2_dict)
 
     def test_list_all(self):
         item3_dict = {'name': 'item1', 'content': 'blabla'}
-        item3 = Item(**item3_dict)
+        item3 = Proof(**item3_dict)
         item3.save()
 
-        stored = Item.list_all()
+        stored = Proof.list_all()
         self.assertIn(item3, stored)
 
 if __name__ == '__main__':
     unittest.main()
```

