# Comparing `tmp/nsdotpy-1.2.4.tar.gz` & `tmp/nsdotpy-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.2.4.tar", max compression
+gzip compressed data, was "nsdotpy-1.2.5.tar", max compression
```

## Comparing `nsdotpy-1.2.4.tar` & `nsdotpy-1.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-09 21:48:36.153284 nsdotpy-1.2.4/LICENSE.md
--rw-r--r--   0        0        0     2436 2023-05-09 21:48:36.153284 nsdotpy-1.2.4/README.md
--rw-r--r--   0        0        0      790 2023-05-09 21:48:36.165284 nsdotpy-1.2.4/nsdotpy/__init__.py
--rw-r--r--   0        0        0    40182 2023-05-09 21:48:36.165284 nsdotpy-1.2.4/nsdotpy/session.py
--rw-r--r--   0        0        0     2302 2023-05-09 21:48:36.165284 nsdotpy-1.2.4/nsdotpy/valid_tags.py
--rw-r--r--   0        0        0      703 2023-05-09 21:48:36.165284 nsdotpy-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-09 22:57:17.304660 nsdotpy-1.2.5/LICENSE.md
+-rw-r--r--   0        0        0     2436 2023-05-09 22:57:17.304660 nsdotpy-1.2.5/README.md
+-rw-r--r--   0        0        0      790 2023-05-09 22:57:17.312661 nsdotpy-1.2.5/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    40750 2023-05-09 22:57:17.312661 nsdotpy-1.2.5/nsdotpy/session.py
+-rw-r--r--   0        0        0     2302 2023-05-09 22:57:17.312661 nsdotpy-1.2.5/nsdotpy/valid_tags.py
+-rw-r--r--   0        0        0      703 2023-05-09 22:57:17.312661 nsdotpy-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.5/PKG-INFO
```

### Comparing `nsdotpy-1.2.4/LICENSE.md` & `nsdotpy-1.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.4/README.md` & `nsdotpy-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.4/nsdotpy/__init__.py` & `nsdotpy-1.2.5/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.4/nsdotpy/session.py` & `nsdotpy-1.2.5/nsdotpy/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,27 +62,28 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.2.4"
+        self.VERSION = "1.2.5"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
         self._me = SingleInstance()
         # Create a new httpx session
         self._session = httpx.Client(http2=True, timeout=30)  # ns can b slow
         # Set the user agent to the script name, version, author, and user as recommended in the script rules thread:
         # https://forum.nationstates.net/viewtopic.php?p=16394966&sid=be37623536dbc8cee42d8d043945b887#p16394966
+        self._lock: bool = False
         self._set_user_agent(
             script_name, script_version, script_author, script_user, link_to_src
         )
         # If a link to the source code is provided, add it to the user agent
         # Initialize nationstates specific stuff
         self._ns_server = "1"
         self._auth_region = "rwby"
@@ -127,14 +128,15 @@
                     "class": "logging.StreamHandler",
                     "formatter": "f",
                 }
             },
             "loggers": {
                 "NSDotPy": {"handlers": ["console"], "level": "INFO"},
                 "httpx": {"handlers": ["console"], "level": "ERROR"},
+                "bs4": {"handlers": ["console"], "level": "ERROR"},
             },
         }
         logging.config.dictConfig(config)
 
     def _get_auth_values(self, response: httpx.Response):
         soup = BeautifulSoup(response.text, "html.parser")
         # gathering chk and localid so i dont have to worry about authenticating l8r
@@ -282,26 +284,35 @@
                 "page=compose_telegram",
                 "page=store",
             ]
         ):
             raise ValueError(
                 "You cannot use a tool to interact with telegrams, issues, getting help, or the store. Read up on the script rules: https://forum.nationstates.net/viewtopic.php?p=16394966#p16394966"
             )
+        if self._lock:
+            # if lock is true then we're already in the middle of a
+            # request and we're in danger of breaking the simultaneity rule
+            # so raise an error
+            raise PermissionError(
+                "You're already in the middle of a request. Stop trying to violate simultaneity."
+            )
+        self._lock = True
         if "api.cgi" in canonicalize(url):
             # deal with ratelimiting if its an api request
             response = self.api_request(data, _auth=auth)
         elif "nationstates" in canonicalize(url):
             # do all the things that need to be done for html requests
             response = self._html_request(url, data, files, follow_redirects, auth=auth)
         else:
             # if its not nationstates then just pass the request through
             response = self._session.post(
                 url, data=data, follow_redirects=follow_redirects
             )
         self.current_page = (url, response.text)
+        self._lock = False
         return response
 
     def api_request(self, data: dict, _auth=()) -> httpx.Response:
         """Sends a request to the nationstates api with the given data.
 
         Args:
             data (dict): Payload to send with the request, e.g. {"nation": "testlandia", "q": "region"}
@@ -674,15 +685,15 @@
             type (str): Type of file to upload. Must be "flag" or "banner".
             filename (str): Name of the file to upload. e.g. "myflag.png"
 
         Raises:
             ValueError: If type is not "flag" or "banner"
 
         Returns:
-            str: _description_
+            str: Empty string if the upload failed, otherwise the ID of the uploaded file
         """
         self.logger.info(f"Uploading {filename} to {self.region}")
         if type not in ["flag", "banner"]:
             raise ValueError("type must be 'flag' or 'banner'")
         url = "https://www.nationstates.net/cgi-bin/upload.cgi"
         data = {
             "uploadtype": f"r{type}",
@@ -694,16 +705,15 @@
             f"file_upload_r{type}": (
                 filename,
                 open(filename, "rb"),
                 mimetypes.guess_type(filename)[0],
             )
         }
         response = self.request(url, data, files=files)
-
-        return response.json()["id"]
+        return "" if "id" not in response.json() else response.json()["id"]
 
     def set_flag_and_banner(
         self, flag_id: str = "", banner_id: str = "", flag_mode: str = ""
     ) -> bool:
         """Sets the uploaded flag and/or banner for the current region.
 
         Args:
@@ -713,15 +723,14 @@
 
         Raises:
             ValueError: If flagmode is not "flag", "logo", or ""
 
         Returns:
             bool: Whether the change was successful or not
         """
-        self.logger.info(f"Setting flag and banner for {self.region}")
         if flag_mode not in ["flag", "logo", ""]:
             raise ValueError("flagmode must be 'flag', 'logo', or ''")
         self.logger.info(f"Setting flag and banner for {self.region}")
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {
             "newflag": flag_id,
             "newbanner": banner_id,
@@ -735,25 +744,25 @@
 
         return "Regional banner/flag updated!" in response.text
 
     def change_wfe(self, wfe: str = "") -> bool:
         """Changes the WFE of the current region.
 
         Args:
-            wfe (str, optional): _description_. Defaults to the oldest WFE the region has, for detags.
+            wfe (str, optional): World Factbook Entry to change to. Defaults to the oldest WFE the region has, for detags.
 
         Returns:
             bool: True if successful, False otherwise
         """
         self.logger.info(f"Changing WFE for {self.region}")
         if not wfe:
             wfe = self._get_detag_wfe()  # haku im sorry for hitting your site so much
         url = "https://www.nationstates.net/template-overall=none/page=region_control/"
         data = {
-            "message": wfe.encode("iso-8859-1", "xmlcharrefreplace"),  # lol.
+            "message": wfe.encode("iso-8859-1", "xmlcharrefreplace").decode(),  # lol.
             "setwfebutton": "1",
         }
         response = self.request(url, data)
         return "World Factbook Entry updated!" in response.text
 
     # methods for embassies
 
@@ -932,52 +941,58 @@
 
         data = {"new_price": price, "remove_ask_price": price}
         response = self.request(url, data)
         return f"Removed your ask for {price}" in response.text
 
     def remove_bid(self, price: str, card_id: str, season: str) -> bool:
         """Removes a bid on a card
+
         Args:
             price (str): Price of the bid to remove
             card_id (str): ID of the card
             season (str): Season of the card
+
         Returns:
             bool: Whether the bid was successfully removed or not
         """
 
         self.logger.info(f"Removing a bid for {price} on {card_id} season {season}")
         url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={season}"
 
         data = {"new_price": price, "remove_bid_price": price}
         response = self.request(url, data)
 
         return f"Removed your bid for {price}" in response.text
 
     def expand_deck(self, price: str) -> bool:
-        """Upgrades deck capcity
+        """Upgrades deck capacity
+
         Args:
             price (str): Price of the Upgrade
+
         Returns:
             bool: Whether the upgrade was successfully removed or not
         """
 
         self.logger.info(f"Upgrading your deck at a cost of {price}")
         url = "https://www.nationstates.net/template-overall=none/page=deck"
 
         data = {"embiggen_deck": price}
         response = self.request(url, data)
 
         return "Increased deck capacity from" in response.text
 
     def add_to_collection(self, card_id: str, card_season: str, collection_id: str):
         """Adds a card to collection_id
+
         Args:
             card_id (str): Card ID
             card_season (str): Cards season
             collection_id (str): The ID of the collection you want to add to
+
         Returns:
             bool: Whether the adding was successfully added or not
         """
         self.logger.info(f"Adding {card_id} of season {card_season} to {collection_id}")
         url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={card_season}"
 
         data = {
@@ -990,18 +1005,20 @@
 
         return "Updated collections." in response.text
 
     def remove_from_collection(
         self, card_id: str, card_season: str, collection_id: str
     ):
         """Removes a card from collection_id
+
         Args:
             card_id (str): Card ID
             card_season (str): Cards season
             collection_id (str): The ID of the collection you want to remove from
+
         Returns:
             bool: Whether the removal was successfully added or not
         """
         self.logger.info(
             f"Removing {card_id} of season {card_season} from {collection_id}"
         )
         url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={card_season}"
@@ -1015,31 +1032,35 @@
         }
         response = self.request(url, data)
 
         return "Updated collections." in response.text
 
     def create_collection(self, name: str):
         """Creates a collection named name
+
         Args:
             name (str): The name of the collection you want to create
+
         Returns:
             bool: Whether the creating was successfully added or not
         """
         self.logger.info(f"Creating {name} collection")
         url = "https://www.nationstates.net/template-overall=none/page=deck"
 
         data = {"edit": "1", "collection_name": name, "save_collection": "1"}
         response = self.request(url, data)
 
         return "Created collection!" in response.text
 
     def delete_collection(self, name: str):
         """Deletes a collection named name
+
         Args:
             name (str): The name of the collection you want to delete
+
         Returns:
             bool: Whether the deleting was successfully added or not
         """
         self.logger.info(f"Deleting {name} collection")
         url = "https://www.nationstates.net/template-overall=none/page=deck"
 
         data = {"edit": "1", "collection_name": name, "delete_collection": "1"}
```

### Comparing `nsdotpy-1.2.4/nsdotpy/valid_tags.py` & `nsdotpy-1.2.5/nsdotpy/valid_tags.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.4/pyproject.toml` & `nsdotpy-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.2.4"
+version = "1.2.5"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.2.4/PKG-INFO` & `nsdotpy-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.2.4
+Version: 1.2.5
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

