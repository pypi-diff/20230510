# Comparing `tmp/vk-url-scraper-0.3.5.tar.gz` & `tmp/vk-url-scraper-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vk-url-scraper-0.3.5.tar", last modified: Tue Jun 21 17:28:20 2022, max compression
+gzip compressed data, was "vk-url-scraper-0.3.8.tar", last modified: Thu Nov  3 16:20:55 2022, max compression
```

## Comparing `vk-url-scraper-0.3.5.tar` & `vk-url-scraper-0.3.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 17:28:20.531528 vk-url-scraper-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-06-21 17:28:20.531528 vk-url-scraper-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4213 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-21 17:28:20.531528 vk-url-scraper-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 17:28:20.527528 vk-url-scraper-0.3.5/vk_url_scraper/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/vk_url_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/vk_url_scraper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/vk_url_scraper/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    13766 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/vk_url_scraper/scraper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/vk_url_scraper/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-06-21 17:27:48.000000 vk-url-scraper-0.3.5/vk_url_scraper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 17:28:20.531528 vk-url-scraper-0.3.5/vk_url_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4894 2022-06-21 17:28:20.000000 vk-url-scraper-0.3.5/vk_url_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-06-21 17:28:20.000000 vk-url-scraper-0.3.5/vk_url_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-21 17:28:20.000000 vk-url-scraper-0.3.5/vk_url_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-06-21 17:28:20.000000 vk-url-scraper-0.3.5/vk_url_scraper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-06-21 17:28:20.000000 vk-url-scraper-0.3.5/vk_url_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-06-21 17:28:20.000000 vk-url-scraper-0.3.5/vk_url_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:20:55.025123 vk-url-scraper-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-11-03 16:20:55.025123 vk-url-scraper-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4891 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 16:20:55.025123 vk-url-scraper-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:20:55.025123 vk-url-scraper-0.3.8/vk_url_scraper/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/vk_url_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/vk_url_scraper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/vk_url_scraper/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    14242 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/vk_url_scraper/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/vk_url_scraper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2022-11-03 16:20:21.000000 vk-url-scraper-0.3.8/vk_url_scraper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:20:55.025123 vk-url-scraper-0.3.8/vk_url_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-11-03 16:20:54.000000 vk-url-scraper-0.3.8/vk_url_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-11-03 16:20:54.000000 vk-url-scraper-0.3.8/vk_url_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 16:20:54.000000 vk-url-scraper-0.3.8/vk_url_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-03 16:20:54.000000 vk-url-scraper-0.3.8/vk_url_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-11-03 16:20:54.000000 vk-url-scraper-0.3.8/vk_url_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-03 16:20:54.000000 vk-url-scraper-0.3.8/vk_url_scraper.egg-info/top_level.txt
```

### Comparing `vk-url-scraper-0.3.5/LICENSE` & `vk-url-scraper-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vk-url-scraper-0.3.5/PKG-INFO` & `vk-url-scraper-0.3.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,17 @@
-Metadata-Version: 2.1
-Name: vk-url-scraper
-Version: 0.3.5
-Summary: Scrape VK URLs to fetch info and media - python API or command line tool.
-Home-page: https://github.com/bellingcat/vk-url-scraper
-Author: Bellingcat
-Author-email: tech@bellingcat.com
-License: MIT
-Keywords: scraper,vk,vkontakte,vk-api,media-downloader
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # vk-url-scraper
-Library to scrape data and especially media links (videos and photos) from vk.com URLs.
+Python library to scrape data, and especially media links like videos and photos, from vk.com URLs.
+
+
+[![PyPI version](https://badge.fury.io/py/vk-url-scraper.svg)](https://badge.fury.io/py/vk-url-scraper)
+[![PyPI download month](https://img.shields.io/pypi/dm/vk-url-scraper.svg)](https://pypi.python.org/pypi/vk-url-scraper/)
+[![Documentation Status](https://readthedocs.org/projects/vk-url-scraper/badge/?version=latest)](https://vk-url-scraper.readthedocs.io/en/latest/?badge=latest)
 
-You can use it via the [command line](#command-line-usage) or as a [python library](#python-library-usage).
+
+You can use it via the [command line](#command-line-usage) or as a [python library](#python-library-usage), check the **[documentation](https://vk-url-scraper.readthedocs.io/en/latest/)**.
 
 ## Installation
 You can install the most recent release from [pypi](https://pypi.org/project/vk-url-scraper/) via `pip install vk-url-scraper`.
 
 To use the library you will need a valid username/password combination for vk.com. 
 
 ## Command line usage
@@ -37,15 +23,16 @@
 vk_url_scraper -username "username here" --password "password here" --urls https://vk.com/wall12345_6789
 # OR
 vk_url_scraper -u "username here" -p "password here" --urls https://vk.com/wall12345_6789
 # you can also have multiple urls
 vk_url_scraper -u "username here" -p "password here" --urls https://vk.com/wall12345_6789 https://vk.com/photo-12345_6789 https://vk.com/video12345_6789
 
 # you can pass a token as well to avoid always authenticating 
-# and possibly getting captch prompts
+# and possibly getting captcha prompts
+# you can fetch the token from the bk_config.v2.json file generated under by searching for "access_token"
 vk_url_scraper -u "username" -p "password" -t "vktoken goes here" --urls https://vk.com/wall12345_6789
 
 # save the JSON output into a file
 vk_url_scraper -u "username here" -p "password here" --urls https://vk.com/wall12345_6789 > output.json
 
 # download any photos or videos found in these URLS
 # this will use or create an output/ folder and dump the files there
@@ -64,15 +51,15 @@
 res = vks.scrape("https://vk.com/photo1_278184324?rev=1")
 
 # scrape any "wall" URL
 res = vks.scrape("https://vk.com/wall-1_398461")
 
 # scrape any "video" URL
 res = vks.scrape("https://vk.com/video-6596301_145810025")
-print(res[0]["text]) # eg: -> to get the text from code
+print(res[0]["text"]) # eg: -> to get the text from code
 ```
 
 ```python
 # Every scrape* function returns a list of dict like
 {
 	"id": "wall_id",
 	"text": "text in this post" ,
@@ -109,18 +96,18 @@
 
 
 ## Releasing new version
 1. edit [version.py](vk_url_scraper/version.py) with proper versioning
 2. run `./scripts/release.sh` to create a tag and push, alternatively
    1. `git tag vx.y.z` to tag version
    2. `git push origin vx.y.z` -> this will trigger workflow and put project on [pypi](https://pypi.org/project/vk-url-scraper/)
+3. go to https://readthedocs.org/ to deploy new docs version (if webhook is not setup)
 
 ### Fixing a failed release
 
 If for some reason the GitHub Actions release workflow failed with an error that needs to be fixed, you'll have to delete both the tag and corresponding release from GitHub. After you've pushed a fix, delete the tag from your local clone with
 
 ```bash
 git tag -l | xargs git tag -d && git fetch -t
 ```
 
 Then repeat the steps above.
-
```

### Comparing `vk-url-scraper-0.3.5/setup.py` & `vk-url-scraper-0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `vk-url-scraper-0.3.5/vk_url_scraper/__main__.py` & `vk-url-scraper-0.3.8/vk_url_scraper/__main__.py`

 * *Files identical despite different names*

### Comparing `vk-url-scraper-0.3.5/vk_url_scraper/scraper.py` & `vk-url-scraper-0.3.8/vk_url_scraper/scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,32 +36,45 @@
     """
 
     WALL_PATTERN = re.compile(r"(wall.{0,1}\d+_\d+)")
     PHOTO_PATTERN = re.compile(r"(photo.{0,1}\d+_\d+)")
     VIDEO_PATTERN = re.compile(r"(video.{0,1}\d+_\d+)")
 
     def __init__(
-        self, username: str, password: str, token: str = None, captcha_handler=captcha_handler
+        self,
+        username: str,
+        password: str,
+        token: str = None,
+        session_file="vk_config.v2.json",
+        captcha_handler=captcha_handler,
     ) -> None:
         """Initializes the scraper.
 
         This function receives a username and password (or access token) and performs
         authentication on vk.com to then call api endpoints. If token is passed, authentication will not be performed again.
 
         Parameters
         ----------
         username : str
             Username on vk.com, can be a phone number or email
         password : str
             Matching password on vk.com
         token : str
             Access token received after authenticating, can be found in the vl_config.v2.json file
+        session_file : str
+            File name where the VK session is saved so future logins are easier, this will not be created if token is passed
+        captcha_handler : func
+            Function that can receive a vk_api captcha instance and help the user solve it, default is a complete CLI handler
         """
         self.session = vk_api.VkApi(
-            username, password, token=token, captcha_handler=captcha_handler
+            username,
+            password,
+            token=token,
+            config_filename=session_file,
+            captcha_handler=captcha_handler,
         )
         if token is None or len(token) == 0:
             self.session.auth(token_only=True)
 
     def scrape(self, url: str) -> List:
         """Scrapes a URL for multiple possibilities of inner links such as wall, video, photo, ...
```

### Comparing `vk-url-scraper-0.3.5/vk_url_scraper/utils.py` & `vk-url-scraper-0.3.8/vk_url_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `vk-url-scraper-0.3.5/vk_url_scraper.egg-info/PKG-INFO` & `vk-url-scraper-0.3.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: vk-url-scraper
-Version: 0.3.5
+Version: 0.3.8
 Summary: Scrape VK URLs to fetch info and media - python API or command line tool.
 Home-page: https://github.com/bellingcat/vk-url-scraper
 Author: Bellingcat
 Author-email: tech@bellingcat.com
 License: MIT
 Keywords: scraper,vk,vkontakte,vk-api,media-downloader
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # vk-url-scraper
-Library to scrape data and especially media links (videos and photos) from vk.com URLs.
+Python library to scrape data, and especially media links like videos and photos, from vk.com URLs.
 
-You can use it via the [command line](#command-line-usage) or as a [python library](#python-library-usage).
+
+[![PyPI version](https://badge.fury.io/py/vk-url-scraper.svg)](https://badge.fury.io/py/vk-url-scraper)
+[![PyPI download month](https://img.shields.io/pypi/dm/vk-url-scraper.svg)](https://pypi.python.org/pypi/vk-url-scraper/)
+[![Documentation Status](https://readthedocs.org/projects/vk-url-scraper/badge/?version=latest)](https://vk-url-scraper.readthedocs.io/en/latest/?badge=latest)
+
+
+You can use it via the [command line](#command-line-usage) or as a [python library](#python-library-usage), check the **[documentation](https://vk-url-scraper.readthedocs.io/en/latest/)**.
 
 ## Installation
 You can install the most recent release from [pypi](https://pypi.org/project/vk-url-scraper/) via `pip install vk-url-scraper`.
 
 To use the library you will need a valid username/password combination for vk.com. 
 
 ## Command line usage
@@ -37,15 +42,16 @@
 vk_url_scraper -username "username here" --password "password here" --urls https://vk.com/wall12345_6789
 # OR
 vk_url_scraper -u "username here" -p "password here" --urls https://vk.com/wall12345_6789
 # you can also have multiple urls
 vk_url_scraper -u "username here" -p "password here" --urls https://vk.com/wall12345_6789 https://vk.com/photo-12345_6789 https://vk.com/video12345_6789
 
 # you can pass a token as well to avoid always authenticating 
-# and possibly getting captch prompts
+# and possibly getting captcha prompts
+# you can fetch the token from the bk_config.v2.json file generated under by searching for "access_token"
 vk_url_scraper -u "username" -p "password" -t "vktoken goes here" --urls https://vk.com/wall12345_6789
 
 # save the JSON output into a file
 vk_url_scraper -u "username here" -p "password here" --urls https://vk.com/wall12345_6789 > output.json
 
 # download any photos or videos found in these URLS
 # this will use or create an output/ folder and dump the files there
@@ -64,15 +70,15 @@
 res = vks.scrape("https://vk.com/photo1_278184324?rev=1")
 
 # scrape any "wall" URL
 res = vks.scrape("https://vk.com/wall-1_398461")
 
 # scrape any "video" URL
 res = vks.scrape("https://vk.com/video-6596301_145810025")
-print(res[0]["text]) # eg: -> to get the text from code
+print(res[0]["text"]) # eg: -> to get the text from code
 ```
 
 ```python
 # Every scrape* function returns a list of dict like
 {
 	"id": "wall_id",
 	"text": "text in this post" ,
@@ -109,18 +115,18 @@
 
 
 ## Releasing new version
 1. edit [version.py](vk_url_scraper/version.py) with proper versioning
 2. run `./scripts/release.sh` to create a tag and push, alternatively
    1. `git tag vx.y.z` to tag version
    2. `git push origin vx.y.z` -> this will trigger workflow and put project on [pypi](https://pypi.org/project/vk-url-scraper/)
+3. go to https://readthedocs.org/ to deploy new docs version (if webhook is not setup)
 
 ### Fixing a failed release
 
 If for some reason the GitHub Actions release workflow failed with an error that needs to be fixed, you'll have to delete both the tag and corresponding release from GitHub. After you've pushed a fix, delete the tag from your local clone with
 
 ```bash
 git tag -l | xargs git tag -d && git fetch -t
 ```
 
 Then repeat the steps above.
-
```

