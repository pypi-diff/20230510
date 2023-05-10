# Comparing `tmp/pylookyloomonitoring-1.0.2.tar.gz` & `tmp/pylookyloomonitoring-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylookyloomonitoring-1.0.2.tar", max compression
+gzip compressed data, was "pylookyloomonitoring-1.0.3.tar", max compression
```

## Comparing `pylookyloomonitoring-1.0.2.tar` & `pylookyloomonitoring-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1516 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.2/LICENSE
--rw-r--r--   0        0        0      822 2023-02-28 15:25:48.760683 pylookyloomonitoring-1.0.2/README.md
--rw-r--r--   0        0        0      953 2023-02-28 11:41:23.346353 pylookyloomonitoring-1.0.2/pylookyloomonitoring/__init__.py
--rw-r--r--   0        0        0     6376 2023-04-17 12:01:59.260660 pylookyloomonitoring-1.0.2/pylookyloomonitoring/api.py
--rw-r--r--   0        0        0        0 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.2/pylookyloomonitoring/py.typed
--rw-r--r--   0        0        0     1461 2023-04-17 12:03:18.353656 pylookyloomonitoring-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 pylookyloomonitoring-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.3/LICENSE
+-rw-r--r--   0        0        0      822 2023-02-28 15:25:48.760683 pylookyloomonitoring-1.0.3/README.md
+-rw-r--r--   0        0        0      953 2023-02-28 11:41:23.346353 pylookyloomonitoring-1.0.3/pylookyloomonitoring/__init__.py
+-rw-r--r--   0        0        0     6741 2023-05-10 12:45:44.060504 pylookyloomonitoring-1.0.3/pylookyloomonitoring/api.py
+-rw-r--r--   0        0        0        0 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.3/pylookyloomonitoring/py.typed
+-rw-r--r--   0        0        0     1541 2023-05-10 14:05:19.569127 pylookyloomonitoring-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 pylookyloomonitoring-1.0.3/PKG-INFO
```

### Comparing `pylookyloomonitoring-1.0.2/LICENSE` & `pylookyloomonitoring-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.2/README.md` & `pylookyloomonitoring-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.2/pylookyloomonitoring/__init__.py` & `pylookyloomonitoring-1.0.3/pylookyloomonitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.2/pylookyloomonitoring/api.py` & `pylookyloomonitoring-1.0.3/pylookyloomonitoring/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,22 +38,29 @@
 class CompareSettings(TypedDict, total=False):
     '''The settings that can be passed to the compare method on lookyloo side to filter out some differences'''
 
     ressources_ignore_domains: Optional[List[str]]
     ressources_ignore_regexes: Optional[List[str]]
 
 
+class NotificationSettings(TypedDict, total=False):
+    '''The notification settings for a monitoring'''
+
+    email: str
+
+
 class MonitorSettings(TypedDict, total=False):
     '''The settings for the capture we want to monitor'''
 
     capture_settings: CaptureSettings
     frequency: str
     expire_at: Optional[float]
     collection: Optional[str]
     compare_settings: Optional[CompareSettings]
+    notification: Optional[NotificationSettings]
 
 
 class MonitoringInstanceSettings(TypedDict):
     '''The settings of the monitoring instance.'''
     min_frequency: int
     max_captures: int
     force_expire: bool
@@ -142,22 +149,24 @@
         """
         r = self.session.get(urljoin(self.root_url, str(Path('json', 'changes', uuid))))
         return r.json()
 
     def monitor(self, capture_settings: CaptureSettings, /, frequency: str, *,
                 expire_at: Optional[Union[datetime, str, int, float]]=None,
                 collection: Optional[str]=None,
-                compare_settings: Optional[CompareSettings]=None) -> str:
+                compare_settings: Optional[CompareSettings]=None,
+                notification: Optional[NotificationSettings]) -> str:
         """Add a new capture to monitor.
 
         :param capture_settings: The settings of the capture
         :param frequency: The frequency of the monitoring
         :param expire_at: When the monitoring should expire.
         :param collection: The collection the monitored capture is part of.
         :param compare_settings: The comparison settings.
+        :param notification: The notification settings.
         """
         to_post: MonitorSettings = {
             'capture_settings': capture_settings,
             'frequency': frequency
         }
         if expire_at:
             if isinstance(expire_at, (str, int, float)):
@@ -167,17 +176,18 @@
             if _expire < datetime.now().timestamp():
                 # The expiration time is in the past.
                 self.logger.warning(f'Expiration time in the past ({expire_at}), forcing it to tomorrow.')
                 _expire = (datetime.now() + timedelta(hours=24)).timestamp()
             to_post['expire_at'] = _expire
         if collection:
             to_post['collection'] = collection
-
         if compare_settings:
             to_post['compare_settings'] = compare_settings
+        if notification:
+            to_post['notification'] = notification
 
         r = self.session.post(urljoin(self.root_url, 'monitor'), json=to_post)
         return r.json()
 
     def instance_settings(self) -> MonitoringInstanceSettings:
         """Get the settings of the monitoring instance."""
         r = self.session.get(urljoin(self.root_url, str(Path('json', 'settings'))))
```

### Comparing `pylookyloomonitoring-1.0.2/pyproject.toml` & `pylookyloomonitoring-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylookyloomonitoring"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python API to connect to lookyloo monitoring"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PyLookylooMonitoring"
 documentation = "https://pylookyloomonitoring.readthedocs.io/en/latest/index.html"
 
 readme = "README.md"
@@ -29,23 +29,26 @@
 include = ['README.md']
 
 [tool.poetry.scripts]
 lookyloo_monitor= 'pylookyloomonitoring:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.28.2"
-Sphinx = { version = "^6.1.3", optional = true }
+requests = "^2.30.0"
+Sphinx = { version = "^7.0.0", optional = true }
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [tool.poetry.group.dev.dependencies]
-pylint = "^2.17.2"
+pylint = "^2.17.4"
 mypy = "^1.2.0"
-types-requests = "^2.28.11.17"
-ipython = "^8.12.0"
+types-requests = "^2.30.0.0"
+ipython = [
+    {version = "<8.13.0", python = "<3.9"},
+    {version = "^8.13.0", python = ">=3.9"}
+]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry_core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pylookyloomonitoring-1.0.2/PKG-INFO` & `pylookyloomonitoring-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookyloomonitoring
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API to connect to lookyloo monitoring
 Home-page: https://github.com/Lookyloo/PyLookylooMonitoring
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,16 +23,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: Sphinx (>=7.0.0,<8.0.0) ; extra == "docs"
+Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Documentation, https://pylookyloomonitoring.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/Lookyloo/PyLookylooMonitoring
 Description-Content-Type: text/markdown
 
 # Python client and module for Lookyloo Monitoring
 
 There is no public monitoring instance for now, so you will need to
```

