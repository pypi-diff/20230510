# Comparing `tmp/pylookyloomonitoring-1.0.3.tar.gz` & `tmp/pylookyloomonitoring-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylookyloomonitoring-1.0.3.tar", max compression
+gzip compressed data, was "pylookyloomonitoring-1.0.4.tar", max compression
```

## Comparing `pylookyloomonitoring-1.0.3.tar` & `pylookyloomonitoring-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1516 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.3/LICENSE
--rw-r--r--   0        0        0      822 2023-02-28 15:25:48.760683 pylookyloomonitoring-1.0.3/README.md
--rw-r--r--   0        0        0      953 2023-02-28 11:41:23.346353 pylookyloomonitoring-1.0.3/pylookyloomonitoring/__init__.py
--rw-r--r--   0        0        0     6741 2023-05-10 12:45:44.060504 pylookyloomonitoring-1.0.3/pylookyloomonitoring/api.py
--rw-r--r--   0        0        0        0 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.3/pylookyloomonitoring/py.typed
--rw-r--r--   0        0        0     1541 2023-05-10 14:05:19.569127 pylookyloomonitoring-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 pylookyloomonitoring-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.4/LICENSE
+-rw-r--r--   0        0        0      822 2023-02-28 15:25:48.760683 pylookyloomonitoring-1.0.4/README.md
+-rw-r--r--   0        0        0      953 2023-02-28 11:41:23.346353 pylookyloomonitoring-1.0.4/pylookyloomonitoring/__init__.py
+-rw-r--r--   0        0        0     6746 2023-05-10 14:23:50.249459 pylookyloomonitoring-1.0.4/pylookyloomonitoring/api.py
+-rw-r--r--   0        0        0        0 2023-02-21 17:02:00.587053 pylookyloomonitoring-1.0.4/pylookyloomonitoring/py.typed
+-rw-r--r--   0        0        0     1541 2023-05-10 14:24:00.109500 pylookyloomonitoring-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 pylookyloomonitoring-1.0.4/PKG-INFO
```

### Comparing `pylookyloomonitoring-1.0.3/LICENSE` & `pylookyloomonitoring-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.3/README.md` & `pylookyloomonitoring-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.3/pylookyloomonitoring/__init__.py` & `pylookyloomonitoring-1.0.4/pylookyloomonitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pylookyloomonitoring-1.0.3/pylookyloomonitoring/api.py` & `pylookyloomonitoring-1.0.4/pylookyloomonitoring/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         r = self.session.get(urljoin(self.root_url, str(Path('json', 'changes', uuid))))
         return r.json()
 
     def monitor(self, capture_settings: CaptureSettings, /, frequency: str, *,
                 expire_at: Optional[Union[datetime, str, int, float]]=None,
                 collection: Optional[str]=None,
                 compare_settings: Optional[CompareSettings]=None,
-                notification: Optional[NotificationSettings]) -> str:
+                notification: Optional[NotificationSettings]=None) -> str:
         """Add a new capture to monitor.
 
         :param capture_settings: The settings of the capture
         :param frequency: The frequency of the monitoring
         :param expire_at: When the monitoring should expire.
         :param collection: The collection the monitored capture is part of.
         :param compare_settings: The comparison settings.
```

### Comparing `pylookyloomonitoring-1.0.3/pyproject.toml` & `pylookyloomonitoring-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylookyloomonitoring"
-version = "1.0.3"
+version = "1.0.4"
 description = "Python API to connect to lookyloo monitoring"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PyLookylooMonitoring"
 documentation = "https://pylookyloomonitoring.readthedocs.io/en/latest/index.html"
 
 readme = "README.md"
```

### Comparing `pylookyloomonitoring-1.0.3/PKG-INFO` & `pylookyloomonitoring-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylookyloomonitoring
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python API to connect to lookyloo monitoring
 Home-page: https://github.com/Lookyloo/PyLookylooMonitoring
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

