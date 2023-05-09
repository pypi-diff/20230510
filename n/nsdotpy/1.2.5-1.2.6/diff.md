# Comparing `tmp/nsdotpy-1.2.5.tar.gz` & `tmp/nsdotpy-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.2.5.tar", max compression
+gzip compressed data, was "nsdotpy-1.2.6.tar", max compression
```

## Comparing `nsdotpy-1.2.5.tar` & `nsdotpy-1.2.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-09 22:57:17.304660 nsdotpy-1.2.5/LICENSE.md
--rw-r--r--   0        0        0     2436 2023-05-09 22:57:17.304660 nsdotpy-1.2.5/README.md
--rw-r--r--   0        0        0      790 2023-05-09 22:57:17.312661 nsdotpy-1.2.5/nsdotpy/__init__.py
--rw-r--r--   0        0        0    40750 2023-05-09 22:57:17.312661 nsdotpy-1.2.5/nsdotpy/session.py
--rw-r--r--   0        0        0     2302 2023-05-09 22:57:17.312661 nsdotpy-1.2.5/nsdotpy/valid_tags.py
--rw-r--r--   0        0        0      703 2023-05-09 22:57:17.312661 nsdotpy-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-09 23:48:13.434463 nsdotpy-1.2.6/LICENSE.md
+-rw-r--r--   0        0        0     2436 2023-05-09 23:48:13.434463 nsdotpy-1.2.6/README.md
+-rw-r--r--   0        0        0      790 2023-05-09 23:48:13.446463 nsdotpy-1.2.6/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    40837 2023-05-09 23:48:13.446463 nsdotpy-1.2.6/nsdotpy/session.py
+-rw-r--r--   0        0        0     4963 2023-05-09 23:48:13.446463 nsdotpy-1.2.6/nsdotpy/valid.py
+-rw-r--r--   0        0        0      703 2023-05-09 23:48:13.446463 nsdotpy-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.6/PKG-INFO
```

### Comparing `nsdotpy-1.2.5/LICENSE.md` & `nsdotpy-1.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.5/README.md` & `nsdotpy-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.5/nsdotpy/__init__.py` & `nsdotpy-1.2.6/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.5/nsdotpy/session.py` & `nsdotpy-1.2.6/nsdotpy/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # external library imports
 import keyboard  # for the required user input
 import httpx  # for http stuff
 from tendo.singleton import SingleInstance  # so it can only be run once at a time
 from bs4 import BeautifulSoup  # for parsing html and xml
 
 # local imports
-from . import valid_tags  # for valid region tags
+from . import valid  # for valid region tags
 
 
 def canonicalize(string: str) -> str:
     """Converts a string to its canonical form used by the nationstates api.
 
     Args:
         string (str): The string to convert
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.2.5"
+        self.VERSION = "1.2.6"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -128,20 +128,23 @@
                     "class": "logging.StreamHandler",
                     "formatter": "f",
                 }
             },
             "loggers": {
                 "NSDotPy": {"handlers": ["console"], "level": "INFO"},
                 "httpx": {"handlers": ["console"], "level": "ERROR"},
-                "bs4": {"handlers": ["console"], "level": "ERROR"},
             },
         }
         logging.config.dictConfig(config)
 
     def _get_auth_values(self, response: httpx.Response):
+        # make sure it's actually html first
+        if response.headers["Content-Type"].startswith("text/html"):
+            return
+        # parse the html
         soup = BeautifulSoup(response.text, "html.parser")
         # gathering chk and localid so i dont have to worry about authenticating l8r
         if chk := soup.find("input", {"name": "chk"}):
             self.chk = chk["value"].strip()  # type: ignore
         if localid := soup.find("input", {"name": "localid"}):
             self.localid = localid["value"].strip()  # type: ignore
         if pin := self._session.cookies.get("pin"):
@@ -842,15 +845,15 @@
             ValueError: If action is not "add" or "remove", or if tag is not a valid tag.
 
         Returns:
             bool: Whether the tag was successfully added or removed
         """
         if action not in ["add", "remove"]:
             raise ValueError("action must be 'add' or 'remove'")
-        if canonicalize(tag) not in valid_tags.tags:
+        if canonicalize(tag) not in valid.region_tags:
             raise ValueError(f"{tag} is not a valid tag")
         self.logger.info(f"{action.capitalize()}ing tag {tag} for {self.region}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {
             f"{action}_tag": canonicalize(tag),
             "updatetagsbutton": "1",
         }
```

### Comparing `nsdotpy-1.2.5/pyproject.toml` & `nsdotpy-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.2.5"
+version = "1.2.6"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.2.5/PKG-INFO` & `nsdotpy-1.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.2.5
+Version: 1.2.6
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

