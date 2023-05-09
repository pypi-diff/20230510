# Comparing `tmp/indiek-core-0.1.2.tar.gz` & `tmp/indiek-core-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-vppkdjiq/indiek-core-0.1.2.tar", last modified: Sun May  7 13:33:53 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-core/dist/.tmp-n6x9td7w/indiek-core-0.1.3.tar", last modified: Tue May  9 22:16:55 2023, max compression
```

## Comparing `indiek-core-0.1.2.tar` & `indiek-core-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.157884 indiek-core-0.1.2/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.2/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1210 2023-05-07 13:33:53.157884 indiek-core-0.1.2/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      759 2023-04-23 17:12:42.000000 indiek-core-0.1.2/README.rst
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.141884 indiek-core-0.1.2/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.157884 indiek-core-0.1.2/indiek/core/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       13 2023-04-23 17:12:42.000000 indiek-core-0.1.2/indiek/core/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     2791 2023-05-07 13:27:55.000000 indiek-core-0.1.2/indiek/core/items.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      280 2023-05-07 13:27:55.000000 indiek-core-0.1.2/indiek/core/search.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.157884 indiek-core-0.1.2/indiek_core.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1210 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      319 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       58 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-07 13:33:53.000000 indiek-core-0.1.2/indiek_core.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-07 13:33:53.157884 indiek-core-0.1.2/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      924 2023-05-07 13:27:55.000000 indiek-core-0.1.2/setup.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:33:53.157884 indiek-core-0.1.2/tests/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1172 2023-05-07 13:27:55.000000 indiek-core-0.1.2/tests/test_items.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      416 2023-05-07 13:27:55.000000 indiek-core-0.1.2/tests/test_search.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.678692 indiek-core-0.1.3/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-04-15 20:23:22.000000 indiek-core-0.1.3/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1165 2023-05-09 22:16:55.678692 indiek-core-0.1.3/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      714 2023-05-09 22:12:17.000000 indiek-core-0.1.3/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.674692 indiek-core-0.1.3/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.674692 indiek-core-0.1.3/indiek/core/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       14 2023-05-07 17:29:44.000000 indiek-core-0.1.3/indiek/core/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3310 2023-05-07 18:01:42.000000 indiek-core-0.1.3/indiek/core/items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3488 2023-05-08 22:13:30.000000 indiek-core-0.1.3/indiek/core/search.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.678692 indiek-core-0.1.3/indiek_core.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1165 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      319 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       58 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-09 22:16:55.000000 indiek-core-0.1.3/indiek_core.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       74 2023-05-09 22:16:55.678692 indiek-core-0.1.3/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      924 2023-05-07 14:33:34.000000 indiek-core-0.1.3/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-09 22:16:55.678692 indiek-core-0.1.3/tests/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1503 2023-05-07 17:43:18.000000 indiek-core-0.1.3/tests/test_items.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     3031 2023-05-08 22:21:51.000000 indiek-core-0.1.3/tests/test_search.py
```

### Comparing `indiek-core-0.1.2/LICENSE` & `indiek-core-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-core-0.1.2/indiek/core/items.py` & `indiek-core-0.1.3/indiek/core/items.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,23 @@
     Attributes:
         _ikid (int): a unique identifier.
         name (str): a human-friendly short identifier.
         content (str): some string with data the Item is meant to hold or reference.
         backend (Any): backend port for I/O operations with DB
     """
 
+    BACKEND_CLS = default_driver.Item
+    """Class from backend items module corresponding to present core API class."""
+
+    def __init__(self, *, name: str = '', content: Any = '', _ikid: Optional[int] = None, driver: Any = default_driver):
+        self._ikid = _ikid
+        self.name = name
+        self.content = content
+        self.backend = driver
+
     def __repr__(self):
         _ikid = self._ikid
         name = self.name
         content_hash = hash(self.content)
         driver = self.backend
         return f"module: {__name__}; class:{self.__class__.__name__}; {_ikid=}; {name=}; {content_hash=}; {driver=}"
     
@@ -33,39 +42,54 @@
         # TODO: not sure this __hash__ method follows best practices
         return hash((self._ikid, self.name, self.content, self.__class__.__name__))
 
     def __str__(self):
         return f"Core Item with ID {self._ikid} and name {self.name}"
 
     def __eq__(self, other) -> bool:
-        cond = self._ikid == other._ikid
-        cond = cond and self.name == other.name
-        cond = cond and self.content == other.content
-        return cond and isinstance(other, self.__class__)
-
-    def __init__(self, *, name: str = '', content: Any = '', _ikid: Optional[int] = None, driver: Any = default_driver):
-        self._ikid = _ikid
-        self.name = name
-        self.content = content
-        self.backend = driver
+        return (self._ikid == other._ikid
+                and self.name == other.name
+                and self.content == other.content
+                and type(other) == type(self))
 
     def _to_db(self) -> default_driver.Item:
         """Export core Item to DB Item instance."""
-        return self.backend.Item.from_core(self)
+        return self.BACKEND_CLS.from_core(self)
     
-    def save(self) -> None:
+    def save(self) -> int:
         """Save to backend.
         
         This method delegates the save operation to the backend.
         If _ikid is None in self, it will get set to new value
         generated by backend.
         """
         self._ikid = self._to_db().save()
+        return self._ikid
 
-    @staticmethod
-    def from_db(db_item: default_driver.Item) -> Item:
+    @classmethod
+    def load(cls, ikid) -> Item:
+        """Create Core Item from backend using ikid."""
+        return cls.from_db(cls.BACKEND_CLS.load(ikid))
+
+    @classmethod
+    def from_db(cls, db_item: default_driver.Item) -> Item:
         """Instantiate core Item off of backend Item."""
-        return Item(**db_item.to_dict())
+        return cls(**db_item.to_dict())
     
     def to_dict(self):
         """Export core Item content to dict."""
-        return {'name': self.name, 'content': self.content, '_ikid': self._ikid}
+        return {'name': self.name, 'content': self.content, '_ikid': self._ikid}
+    
+
+class Definition(Item):
+    BACKEND_CLS = default_driver.Definition
+    pass
+
+
+class Theorem(Item):
+    BACKEND_CLS = default_driver.Theorem
+    pass
+
+
+class Proof(Item):
+    BACKEND_CLS = default_driver.Proof
+    pass
```

### Comparing `indiek-core-0.1.2/setup.py` & `indiek-core-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.rst'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='indiek-core',
     python_requires='>=3.8',
-    version='0.1.2',
+    version='0.1.3',
     url='https://pypi.org/project/indiek-core/',
     description='core logic for indiek',
     long_description=long_description,
     author='Adrian Ernesto Radillo',
     author_email='adrian.radillo@gmail.com',
     license='GNU Affero General Public License v3.0',
     packages=['indiek.core'],
-    install_requires=['indiek-mockdb==0.1.2'],
+    install_requires=['indiek-mockdb==0.1.3'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov'
         ]
     },
```

