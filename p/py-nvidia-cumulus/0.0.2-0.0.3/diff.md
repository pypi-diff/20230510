# Comparing `tmp/py_nvidia_cumulus-0.0.2.tar.gz` & `tmp/py_nvidia_cumulus-0.0.3.tar.gz`

## Comparing `py_nvidia_cumulus-0.0.2.tar` & `py_nvidia_cumulus-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/Makefile
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/main.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/requirements.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/cumulus/__init__.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/cumulus/api.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/cumulus/base.py
--rw-r--r--   0        0        0     9134 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/cumulus/models.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/cumulus/util.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/tests/test_api.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/tests/test_base.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/tests/test_models.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/LICENSE
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/README.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/Makefile
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/__init__.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/api.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/base.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/models.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/cumulus/util.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/tests/test_api.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/tests/test_base.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/tests/test_models.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/README.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 py_nvidia_cumulus-0.0.3/PKG-INFO
```

### Comparing `py_nvidia_cumulus-0.0.2/cumulus/api.py` & `py_nvidia_cumulus-0.0.3/cumulus/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from requests import Session
 from .base import Request
 from .models import (Revision, Root,
                      Router, Platform, Bridge,
                      Mlag, Evpn, Qos,
                      Interface, Service, System,
-                     Vrf, Nve, Acl,
-                     Bridge, Evpn)
+                     Vrf, Nve, Acl, AAA,
+                     Bridge, Evpn, User, Role)
 
 
 class Cumulus:
     """
     A thin wrapper around Cumulus API endpoints
     :param str url: a URL to the Cumulus host in the format <protocol>://<host>:<port>
     :param tuple auth: Cumulus host authentication details in the format ('user', 'pass')
@@ -33,14 +33,17 @@
         self.qos = Qos(self, "qos")
         self.interface = Interface(self, "interface")
         self.service = Service(self, "service")
         self.system = System(self, "system")
         self.vrf = Vrf(self, "vrf")
         self.nve = Nve(self, "nve")
         self.acl = Acl(self, "acl")
+        self.aaa = AAA(self, "system/aaa")
+        self.user = User(self, "system/aaa/user")
+        self.role = Role(self, "system/aaa/role")
 
     @staticmethod
     def _format_url(url):
         """
         Set the provided URL in the correct format
         """
         return "{}/nvue_v1".format(url if url[-1] != "/" else url[-1])
```

### Comparing `py_nvidia_cumulus-0.0.2/cumulus/base.py` & `py_nvidia_cumulus-0.0.3/cumulus/base.py`

 * *Files identical despite different names*

### Comparing `py_nvidia_cumulus-0.0.2/cumulus/models.py` & `py_nvidia_cumulus-0.0.3/cumulus/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,7 +321,25 @@
         super().__init__(client, endpoint)
 
 
 class Acl(BaseModel):
 
     def __init__(self, client, endpoint: str) -> None:
         super().__init__(client, endpoint)
+
+
+class AAA(BaseModel):
+
+    def __init__(self, client, endpoint: str) -> None:
+        super().__init__(client, endpoint)
+
+
+class User(BaseModel):
+
+    def __init__(self, client, endpoint: str) -> None:
+        super().__init__(client, endpoint)
+
+
+class Role(BaseModel):
+
+    def __init__(self, client, endpoint: str) -> None:
+        super().__init__(client, endpoint)
```

### Comparing `py_nvidia_cumulus-0.0.2/tests/test_api.py` & `py_nvidia_cumulus-0.0.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `py_nvidia_cumulus-0.0.2/tests/test_base.py` & `py_nvidia_cumulus-0.0.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `py_nvidia_cumulus-0.0.2/tests/test_models.py` & `py_nvidia_cumulus-0.0.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `py_nvidia_cumulus-0.0.2/LICENSE` & `py_nvidia_cumulus-0.0.3/LICENSE`

 * *Files identical despite different names*

