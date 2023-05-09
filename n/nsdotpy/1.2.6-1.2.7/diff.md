# Comparing `tmp/nsdotpy-1.2.6.tar.gz` & `tmp/nsdotpy-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.2.6.tar", max compression
+gzip compressed data, was "nsdotpy-1.2.7.tar", max compression
```

## Comparing `nsdotpy-1.2.6.tar` & `nsdotpy-1.2.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-09 23:48:13.434463 nsdotpy-1.2.6/LICENSE.md
--rw-r--r--   0        0        0     2436 2023-05-09 23:48:13.434463 nsdotpy-1.2.6/README.md
--rw-r--r--   0        0        0      790 2023-05-09 23:48:13.446463 nsdotpy-1.2.6/nsdotpy/__init__.py
--rw-r--r--   0        0        0    40837 2023-05-09 23:48:13.446463 nsdotpy-1.2.6/nsdotpy/session.py
--rw-r--r--   0        0        0     4963 2023-05-09 23:48:13.446463 nsdotpy-1.2.6/nsdotpy/valid.py
--rw-r--r--   0        0        0      703 2023-05-09 23:48:13.446463 nsdotpy-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-09 23:52:00.967120 nsdotpy-1.2.7/LICENSE.md
+-rw-r--r--   0        0        0     2436 2023-05-09 23:52:00.967120 nsdotpy-1.2.7/README.md
+-rw-r--r--   0        0        0      790 2023-05-09 23:52:00.979121 nsdotpy-1.2.7/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    40841 2023-05-09 23:52:00.979121 nsdotpy-1.2.7/nsdotpy/session.py
+-rw-r--r--   0        0        0     4963 2023-05-09 23:52:00.979121 nsdotpy-1.2.7/nsdotpy/valid.py
+-rw-r--r--   0        0        0      703 2023-05-09 23:52:00.979121 nsdotpy-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.7/PKG-INFO
```

### Comparing `nsdotpy-1.2.6/LICENSE.md` & `nsdotpy-1.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.6/README.md` & `nsdotpy-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.6/nsdotpy/__init__.py` & `nsdotpy-1.2.7/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.6/nsdotpy/session.py` & `nsdotpy-1.2.7/nsdotpy/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.2.6"
+        self.VERSION = "1.2.7"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -134,15 +134,15 @@
                 "httpx": {"handlers": ["console"], "level": "ERROR"},
             },
         }
         logging.config.dictConfig(config)
 
     def _get_auth_values(self, response: httpx.Response):
         # make sure it's actually html first
-        if response.headers["Content-Type"].startswith("text/html"):
+        if not response.headers["Content-Type"].startswith("text/html"):
             return
         # parse the html
         soup = BeautifulSoup(response.text, "html.parser")
         # gathering chk and localid so i dont have to worry about authenticating l8r
         if chk := soup.find("input", {"name": "chk"}):
             self.chk = chk["value"].strip()  # type: ignore
         if localid := soup.find("input", {"name": "localid"}):
```

### Comparing `nsdotpy-1.2.6/nsdotpy/valid.py` & `nsdotpy-1.2.7/nsdotpy/valid.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.6/pyproject.toml` & `nsdotpy-1.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.2.6"
+version = "1.2.7"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.2.6/PKG-INFO` & `nsdotpy-1.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.2.6
+Version: 1.2.7
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

