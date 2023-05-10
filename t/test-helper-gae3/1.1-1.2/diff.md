# Comparing `tmp/test_helper_gae3-1.1.tar.gz` & `tmp/test_helper_gae3-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_helper_gae3-1.1.tar", last modified: Fri Apr 21 10:39:12 2023, max compression
+gzip compressed data, was "test_helper_gae3-1.2.tar", last modified: Wed May 10 12:09:59 2023, max compression
```

## Comparing `test_helper_gae3-1.1.tar` & `test_helper_gae3-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 10:39:12.870270 test_helper_gae3-1.1/
--rw-rw-rw-   0        0        0     1094 2023-04-17 15:55:38.000000 test_helper_gae3-1.1/LICENSE
--rw-rw-rw-   0        0        0       64 2023-04-18 12:37:07.000000 test_helper_gae3-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2735 2023-04-21 10:39:12.870270 test_helper_gae3-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1787 2023-04-18 12:32:10.000000 test_helper_gae3-1.1/README.md
--rw-rw-rw-   0        0        0      110 2023-04-18 12:37:07.000000 test_helper_gae3-1.1/pyproject.toml
--rw-rw-rw-   0        0        0      655 2023-04-21 10:39:12.870270 test_helper_gae3-1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 10:39:12.854644 test_helper_gae3-1.1/test_helper_gae3/
--rw-rw-rw-   0        0        0     4497 2023-04-21 10:35:40.000000 test_helper_gae3-1.1/test_helper_gae3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:39:12.870270 test_helper_gae3-1.1/test_helper_gae3.egg-info/
--rw-rw-rw-   0        0        0     2735 2023-04-21 10:39:12.000000 test_helper_gae3-1.1/test_helper_gae3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-21 10:39:12.000000 test_helper_gae3-1.1/test_helper_gae3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 10:39:12.000000 test_helper_gae3-1.1/test_helper_gae3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-21 10:39:12.000000 test_helper_gae3-1.1/test_helper_gae3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:09:59.536063 test_helper_gae3-1.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-17 15:55:38.000000 test_helper_gae3-1.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2023-04-18 12:37:07.000000 test_helper_gae3-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2609 2023-05-10 12:09:59.536063 test_helper_gae3-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2056 2023-05-10 12:06:05.000000 test_helper_gae3-1.2/README.md
+-rw-rw-rw-   0        0        0      110 2023-04-18 12:37:07.000000 test_helper_gae3-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      655 2023-05-10 12:09:59.536063 test_helper_gae3-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 12:09:59.520437 test_helper_gae3-1.2/test_helper_gae3/
+-rw-rw-rw-   0        0        0     4969 2023-05-10 12:06:05.000000 test_helper_gae3-1.2/test_helper_gae3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:09:59.536063 test_helper_gae3-1.2/test_helper_gae3.egg-info/
+-rw-rw-rw-   0        0        0     2609 2023-05-10 12:09:59.000000 test_helper_gae3-1.2/test_helper_gae3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-10 12:09:59.000000 test_helper_gae3-1.2/test_helper_gae3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:09:59.000000 test_helper_gae3-1.2/test_helper_gae3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-10 12:09:59.000000 test_helper_gae3-1.2/test_helper_gae3.egg-info/top_level.txt
```

### Comparing `test_helper_gae3-1.1/LICENSE` & `test_helper_gae3-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `test_helper_gae3-1.1/PKG-INFO` & `test_helper_gae3-1.2/test_helper_gae3.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
-Name: test_helper_gae3
-Version: 1.1
+Name: test-helper-gae3
+Version: 1.2
 Summary: Class for autotests GoogleAppEngine python3 app.
 Home-page: https://github.com/vb64/test.helper.gae3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.gae3/issues
-Description: # Class for autotests GoogleAppEngine Python3 app.
-        
-        [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/pep257.yml?label=Pep257&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apep257)
-        [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/py3.yml?label=Python%203.7-3.10&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apy3)
-        [![Codacy Badge](https://app.codacy.com/project/badge/Grade/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-        [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
-        
-        ## Install
-        ```bash
-        pip install test-helper-gae3
-        ```
-        
-        ## Usage in tests
-        
-        ```python
-        import unittest
-        from google.appengine.ext import ndb
-        from test_helper_gae3 import TestGae3
-        
-        
-        class ModelTest(ndb.Model):
-            name = ndb.StringProperty(default='')
-        
-        
-        class TestCase(unittest.TestCase, TestGae3):
-        
-            def setUp(self):
-                super().setUp()
-                TestGae3.set_up(self)  # activate GAE testbed
-        
-            def tearDown(self):
-                TestGae3.tear_down(self)  # deactivate GAE testbed
-                super().tearDown()
-        
-            def test_record_count(self):
-                self.check_db_tables([
-                  (ModelTest, 0),  # no records in ModelTest
-                ])
-        
-                ModelTest().put()
-        
-                self.tester.check_db_tables([
-                  (ModelTest, 1),  # one record in ModelTest
-                ])
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Class for autotests GoogleAppEngine Python3 app.
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/pep257.yml?label=Pep257&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apep257)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/py3.yml?label=Python%203.7-3.11&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apy3)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+
+## Install
+```bash
+pip install test-helper-gae3
+```
+
+## Usage in tests
+
+```python
+import unittest
+from google.appengine.ext import ndb
+from test_helper_gae3 import TestGae3
+
+
+class ModelTest(ndb.Model):
+    name = ndb.StringProperty(default='')
+
+
+class TestCase(unittest.TestCase, TestGae3):
+
+    def setUp(self):
+        super().setUp()
+
+        # For using queues names other then 'default', root_path dir must contain file
+        # 'queue.yaml' (or 'queue.yml') with correct queues definition.
+        # If root_path set to None, only 'default' queue is available.
+        TestGae3.set_up(self, 'path/to/folder/with/queue.yaml')  # activate GAE testbed
+
+    def tearDown(self):
+        TestGae3.tear_down(self)  # deactivate GAE testbed
+        super().tearDown()
+
+    def test_record_count(self):
+        self.check_db_tables([
+          (ModelTest, 0),  # no records in ModelTest
+        ])
+
+        ModelTest().put()
+
+        self.tester.check_db_tables([
+          (ModelTest, 1),  # one record in ModelTest
+        ])
+
+```
```

### Comparing `test_helper_gae3-1.1/README.md` & `test_helper_gae3-1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Class for autotests GoogleAppEngine Python3 app.
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/pep257.yml?label=Pep257&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apep257)
-[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/py3.yml?label=Python%203.7-3.10&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apy3)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/py3.yml?label=Python%203.7-3.11&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apy3)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
 
 ## Install
 ```bash
 pip install test-helper-gae3
 ```
@@ -22,15 +22,19 @@
     name = ndb.StringProperty(default='')
 
 
 class TestCase(unittest.TestCase, TestGae3):
 
     def setUp(self):
         super().setUp()
-        TestGae3.set_up(self)  # activate GAE testbed
+
+        # For using queues names other then 'default', root_path dir must contain file
+        # 'queue.yaml' (or 'queue.yml') with correct queues definition.
+        # If root_path set to None, only 'default' queue is available.
+        TestGae3.set_up(self, 'path/to/folder/with/queue.yaml')  # activate GAE testbed
 
     def tearDown(self):
         TestGae3.tear_down(self)  # deactivate GAE testbed
         super().tearDown()
 
     def test_record_count(self):
         self.check_db_tables([
```

### Comparing `test_helper_gae3-1.1/setup.cfg` & `test_helper_gae3-1.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6573 745f 6865 6c70 6572 5f67   = test_helper_g
 00000020: 6165 330d 0a76 6572 7369 6f6e 203d 2031  ae3..version = 1
-00000030: 2e31 0d0a 6175 7468 6f72 203d 2056 6974  .1..author = Vit
+00000030: 2e32 0d0a 6175 7468 6f72 203d 2056 6974  .2..author = Vit
 00000040: 616c 7920 426f 676f 6d6f 6c6f 760d 0a61  aly Bogomolov..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6d61  uthor_email = ma
 00000060: 696c 4076 6974 616c 792d 626f 676f 6d6f  il@vitaly-bogomo
 00000070: 6c6f 762e 7275 0d0a 6465 7363 7269 7074  lov.ru..descript
 00000080: 696f 6e20 3d20 436c 6173 7320 666f 7220  ion = Class for 
 00000090: 6175 746f 7465 7374 7320 476f 6f67 6c65  autotests Google
 000000a0: 4170 7045 6e67 696e 6520 7079 7468 6f6e  AppEngine python
```

### Comparing `test_helper_gae3-1.1/test_helper_gae3/__init__.py` & `test_helper_gae3-1.2/test_helper_gae3/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,40 @@
 class TestGae3:
     """Mixing class for GAE testbed use."""
 
     gae_testbed = None
     blobstore_stub = None
     taskqueue_stub = None
 
-    def set_up(self):
-        """Activate GAE testbed for project in given dir."""
+    def set_up(self, root_path, queue_config_path=None):
+        """Activate GAE testbed for project in root_path dir.
+
+        For using queues names other then 'default', root_path dir must contain file 'queue.yaml' (or 'queue.yml')
+        with correct queues definition.
+
+        If root_path set to None, only 'default' queue is available.
+
+        Argument `queue_config_path` can contain the full path to queue.yaml; supersedes root_path.
+        """
         self.gae_testbed = testbed.Testbed()
         self.gae_testbed.activate()
         # self.gae_testbed.setup_env()
         self.gae_testbed.init_datastore_v3_stub()
         self.gae_testbed.init_memcache_stub()
 
         self.gae_testbed.init_blobstore_stub()
         self.blobstore_stub = self.gae_testbed.get_stub(testbed.BLOBSTORE_SERVICE_NAME)
 
         self.gae_testbed.init_images_stub()
         self.gae_testbed.init_mail_stub()
 
-        self.gae_testbed.init_taskqueue_stub()
+        self.gae_testbed.init_taskqueue_stub(
+          root_path=root_path,
+          queue_config_path=queue_config_path
+        )
         self.taskqueue_stub = self.gae_testbed.get_stub(testbed.TASKQUEUE_SERVICE_NAME)
 
         self.gae_testbed.init_urlfetch_stub()
         self.gae_testbed.init_user_stub()
 
     def tear_down(self):
         """Deactivate GAE testbed."""
```

### Comparing `test_helper_gae3-1.1/test_helper_gae3.egg-info/PKG-INFO` & `test_helper_gae3-1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
-Name: test-helper-gae3
-Version: 1.1
+Name: test_helper_gae3
+Version: 1.2
 Summary: Class for autotests GoogleAppEngine python3 app.
 Home-page: https://github.com/vb64/test.helper.gae3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.gae3/issues
-Description: # Class for autotests GoogleAppEngine Python3 app.
-        
-        [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/pep257.yml?label=Pep257&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apep257)
-        [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/py3.yml?label=Python%203.7-3.10&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apy3)
-        [![Codacy Badge](https://app.codacy.com/project/badge/Grade/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-        [![Codacy Badge](https://app.codacy.com/project/badge/Coverage/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
-        
-        ## Install
-        ```bash
-        pip install test-helper-gae3
-        ```
-        
-        ## Usage in tests
-        
-        ```python
-        import unittest
-        from google.appengine.ext import ndb
-        from test_helper_gae3 import TestGae3
-        
-        
-        class ModelTest(ndb.Model):
-            name = ndb.StringProperty(default='')
-        
-        
-        class TestCase(unittest.TestCase, TestGae3):
-        
-            def setUp(self):
-                super().setUp()
-                TestGae3.set_up(self)  # activate GAE testbed
-        
-            def tearDown(self):
-                TestGae3.tear_down(self)  # deactivate GAE testbed
-                super().tearDown()
-        
-            def test_record_count(self):
-                self.check_db_tables([
-                  (ModelTest, 0),  # no records in ModelTest
-                ])
-        
-                ModelTest().put()
-        
-                self.tester.check_db_tables([
-                  (ModelTest, 1),  # one record in ModelTest
-                ])
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Class for autotests GoogleAppEngine Python3 app.
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/pep257.yml?label=Pep257&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apep257)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.gae3/py3.yml?label=Python%203.7-3.11&style=plastic&branch=main)](https://github.com/vb64/test.helper.gae3/actions?query=workflow%3Apy3)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/abee606aca3047f9952c43196aa5d2b7)](https://app.codacy.com/gh/vb64/test.helper.gae3/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_coverage)
+
+## Install
+```bash
+pip install test-helper-gae3
+```
+
+## Usage in tests
+
+```python
+import unittest
+from google.appengine.ext import ndb
+from test_helper_gae3 import TestGae3
+
+
+class ModelTest(ndb.Model):
+    name = ndb.StringProperty(default='')
+
+
+class TestCase(unittest.TestCase, TestGae3):
+
+    def setUp(self):
+        super().setUp()
+
+        # For using queues names other then 'default', root_path dir must contain file
+        # 'queue.yaml' (or 'queue.yml') with correct queues definition.
+        # If root_path set to None, only 'default' queue is available.
+        TestGae3.set_up(self, 'path/to/folder/with/queue.yaml')  # activate GAE testbed
+
+    def tearDown(self):
+        TestGae3.tear_down(self)  # deactivate GAE testbed
+        super().tearDown()
+
+    def test_record_count(self):
+        self.check_db_tables([
+          (ModelTest, 0),  # no records in ModelTest
+        ])
+
+        ModelTest().put()
+
+        self.tester.check_db_tables([
+          (ModelTest, 1),  # one record in ModelTest
+        ])
+
+```
```

