# Comparing `tmp/xhs-0.1.9.tar.gz` & `tmp/xhs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.9.tar", last modified: Tue May  9 04:18:27 2023, max compression
+gzip compressed data, was "xhs-0.2.0.tar", last modified: Wed May 10 02:36:50 2023, max compression
```

## Comparing `xhs-0.1.9.tar` & `xhs-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:18:27.348841 xhs-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-09 04:18:15.000000 xhs-0.1.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-09 04:18:15.000000 xhs-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 04:18:15.000000 xhs-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-09 04:18:27.348841 xhs-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-09 04:18:15.000000 xhs-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-09 04:18:15.000000 xhs-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 04:18:27.348841 xhs-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 04:18:15.000000 xhs-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:18:27.344841 xhs-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-09 04:18:15.000000 xhs-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-09 04:18:15.000000 xhs-0.1.9/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-09 04:18:15.000000 xhs-0.1.9/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-09 04:18:15.000000 xhs-0.1.9/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:18:27.344841 xhs-0.1.9/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21231 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11752 2023-05-09 04:18:15.000000 xhs-0.1.9/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:18:27.344841 xhs-0.1.9/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-09 04:18:27.000000 xhs-0.1.9/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:36:50.052827 xhs-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-10 02:36:33.000000 xhs-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-10 02:36:33.000000 xhs-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 02:36:33.000000 xhs-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-10 02:36:50.052827 xhs-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-10 02:36:33.000000 xhs-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 02:36:33.000000 xhs-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-10 02:36:50.052827 xhs-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-10 02:36:33.000000 xhs-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:36:50.052827 xhs-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-10 02:36:33.000000 xhs-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-10 02:36:33.000000 xhs-0.2.0/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-10 02:36:33.000000 xhs-0.2.0/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 02:36:33.000000 xhs-0.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:36:50.052827 xhs-0.2.0/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-10 02:36:33.000000 xhs-0.2.0/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-10 02:36:33.000000 xhs-0.2.0/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21588 2023-05-10 02:36:33.000000 xhs-0.2.0/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-10 02:36:33.000000 xhs-0.2.0/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-05-10 02:36:33.000000 xhs-0.2.0/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:36:50.052827 xhs-0.2.0/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-10 02:36:50.000000 xhs-0.2.0/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 02:36:50.000000 xhs-0.2.0/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 02:36:50.000000 xhs-0.2.0/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 02:36:49.000000 xhs-0.2.0/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 02:36:50.000000 xhs-0.2.0/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 02:36:50.000000 xhs-0.2.0/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.9/CHANGELOG.md` & `xhs-0.2.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.2.0
+
+### Fixed
+
+- fixed save_files_from_note_id error
+- fixed get_user_all_notes abnormal notes catch error
+
 ## 0.1.9
 
 ### Fixed
 
 - fixed get videos key error
 
 ## 0.1.8
```

### Comparing `xhs-0.1.9/LICENSE` & `xhs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.1.9/PKG-INFO` & `xhs-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.9
+Version: 0.2.0
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
@@ -25,17 +25,18 @@
 
 <div align="center">
 
 <h1 align="center">
 🍰xhs
 </h1>
 
+[![PyPI](https://img.shields.io/pypi/v/xhs?label=xhs)](https://pypi.org/project/xhs/)
 [![](https://static.pepy.tech/badge/xhs)](https://pepy.tech/project/xhs)
 [![](https://img.shields.io/github/license/ReaJason/xhs)](https://github.com/ReaJason/xhs/blob/master/LICENSE)
-[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
+<br /> [![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
 [![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
 [![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
 
 </div>
 
 > **Warning**
 >
```

### Comparing `xhs-0.1.9/README.md` & `xhs-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 <div align="center">
 
 <h1 align="center">
 🍰xhs
 </h1>
 
+[![PyPI](https://img.shields.io/pypi/v/xhs?label=xhs)](https://pypi.org/project/xhs/)
 [![](https://static.pepy.tech/badge/xhs)](https://pepy.tech/project/xhs)
 [![](https://img.shields.io/github/license/ReaJason/xhs)](https://github.com/ReaJason/xhs/blob/master/LICENSE)
-[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
+<br /> [![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
 [![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
 [![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
 
 </div>
 
 > **Warning**
 >
```

### Comparing `xhs-0.1.9/setup.py` & `xhs-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.9/tests/__init__.py` & `xhs-0.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.9/tests/test_help.py` & `xhs-0.2.0/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.9/tests/test_xhs.py` & `xhs-0.2.0/tests/test_xhs.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     data = xhs_client.get_user_notes(user_id)
     beauty_print(data)
     assert len(data["notes"]) > 0
 
 
 @pytest.mark.skip(reason="it take much request and time")
 def test_get_user_all_notes(xhs_client: XhsClient):
-    user_id = "63273a77000000002303cc9b"
+    user_id = "5cbbc6f50000000016032ff2"
     notes = xhs_client.get_user_all_notes(user_id, 0)
     beauty_print(notes)
 
 
 def test_get_note_comments(xhs_client: XhsClient):
     note_id = "63db8819000000001a01ead1"
     comments = xhs_client.get_note_comments(note_id)
```

### Comparing `xhs-0.1.9/xhs/core.py` & `xhs-0.2.0/xhs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,19 +105,21 @@
                                     "Chrome/111.0.0.0 Safari/537.36")
         self.__session.headers = {
             "user-agent": user_agent,
             "Content-Type": "application/json"
         }
         self.IP_ERROR_STR = "网络连接异常，请检查网络设置或重启试试"
         self.IP_ERROR_CODE = 300012
+        self.NOTE_ABNORMAL_STR = "笔记状态异常，请稍后查看"
+        self.NOTE_ABNORMAL_CODE = -510001
         self.cookie = cookie
 
     @property
     def cookie(self):
-        return cookie_jar_to_cookie_str(self.__session)
+        return cookie_jar_to_cookie_str(self.__session.cookies)
 
     @cookie.setter
     def cookie(self, cookie: str):
         update_session_cookies_from_cookie(self.__session, cookie)
         if "web_session" not in self.cookie_dict:
             self.activate()
 
@@ -234,19 +236,19 @@
             title = note_id
 
         new_dir_path = os.path.join(dir_path, title)
         if not os.path.exists(new_dir_path):
             os.mkdir(new_dir_path)
 
         if note["type"] == NoteType.VIDEO.value:
-            video_url = self._get_video_url_from_note(note)
-            video_filename = os.path.join(new_dir_path, f"{title}.mov")
+            video_url = get_video_url_from_note(note)
+            video_filename = os.path.join(new_dir_path, f"{title}.mp4")
             download_file(video_url, video_filename)
         else:
-            img_urls = self._get_img_urls_from_note(note)
+            img_urls = get_imgs_url_from_note(note)
             for index, img_url in enumerate(img_urls):
                 img_file_name = os.path.join(new_dir_path, f"{title}{index}.png")
                 download_file(img_url, img_file_name)
 
     def get_self_info(self):
         uri = "/api/sns/web/v1/user/selfinfo"
         res = self.get(uri)
@@ -324,15 +326,15 @@
             "num": 30,
             "cursor": cursor,
             "user_id": user_id
         }
         return self.get(uri, params)
 
     def get_user_all_notes(self, user_id: str, crawl_interval: int = 1):
-        """get user all notes with more info
+        """get user all notes with more info, abnormal notes will be ignored
 
         :param user_id: user_id you want to fetch
         :type user_id: str
         :param crawl_interval: sleep seconds, defaults to 1
         :type crawl_interval: int, optional
         :return: note info list
         :rtype: list[Note]
@@ -343,15 +345,21 @@
         while has_more:
             res = self.get_user_notes(user_id, cursor)
             has_more = res["has_more"]
             cursor = res["cursor"]
             note_ids = map(lambda note: note["note_id"], res["notes"])
 
             for note_id in note_ids:
-                note = self.get_note_by_id(note_id)
+                try:
+                    note = self.get_note_by_id(note_id)
+                except DataFetchError as e:
+                    if self.NOTE_ABNORMAL_STR in str(e):
+                        continue
+                    else:
+                        raise
                 interact_info = note["interact_info"]
                 note_info = Note(
                     note_id=note["note_id"],
                     title=note["title"],
                     desc=note["desc"],
                     type=note["type"],
                     user=note["user"],
```

### Comparing `xhs-0.1.9/xhs/help.py` & `xhs-0.2.0/xhs/help.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,16 +357,16 @@
 
 def cookie_str_to_cookie_dict(cookie_str: str):
     cookie_blocks = [cookie_block.split("=")
                      for cookie_block in cookie_str.split(";") if cookie_block]
     return {cookie[0]: cookie[1] for cookie in cookie_blocks}
 
 
-def cookie_jar_to_cookie_str(session: requests.Session):
-    cookie_dict = requests.utils.dict_from_cookiejar(session.cookies)
+def cookie_jar_to_cookie_str(cookie_jar):
+    cookie_dict = requests.utils.dict_from_cookiejar(cookie_jar)
     return ";".join([f"{key}={value}" for key, value in cookie_dict.items()])
 
 
 def update_session_cookies_from_cookie(session: requests.Session, cookie: str):
     cookie_dict = cookie_str_to_cookie_dict(cookie) if cookie else {}
     if "a1" not in cookie_dict or "webId" not in cookie_dict:
         # a1, web_id = get_a1_and_web_id()
```

### Comparing `xhs-0.1.9/xhs.egg-info/PKG-INFO` & `xhs-0.2.0/xhs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.9
+Version: 0.2.0
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
@@ -25,17 +25,18 @@
 
 <div align="center">
 
 <h1 align="center">
 🍰xhs
 </h1>
 
+[![PyPI](https://img.shields.io/pypi/v/xhs?label=xhs)](https://pypi.org/project/xhs/)
 [![](https://static.pepy.tech/badge/xhs)](https://pepy.tech/project/xhs)
 [![](https://img.shields.io/github/license/ReaJason/xhs)](https://github.com/ReaJason/xhs/blob/master/LICENSE)
-[![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
+<br /> [![](https://github.com/ReaJason/xhs/actions/workflows/doc.yml/badge.svg)](https://reajason.github.io/xhs/)
 [![](https://github.com/ReaJason/xhs/actions/workflows/test.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/test.yml)
 [![](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml/badge.svg)](https://github.com/ReaJason/xhs/actions/workflows/pypi.yml)
 
 </div>
 
 > **Warning**
 >
```

