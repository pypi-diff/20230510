# Comparing `tmp/twint_fork-2.5.0.tar.gz` & `tmp/twint_fork-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twint_fork-2.5.0.tar", last modified: Wed Apr 26 06:40:36 2023, max compression
+gzip compressed data, was "twint_fork-2.5.1.tar", last modified: Wed May 10 05:07:37 2023, max compression
```

## Comparing `twint_fork-2.5.0.tar` & `twint_fork-2.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-26 06:40:36.090996 twint_fork-2.5.0/
--rw-r--r--   0 hyi        (502) staff       (20)     1071 2023-03-22 13:37:09.000000 twint_fork-2.5.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)       26 2023-03-22 13:37:09.000000 twint_fork-2.5.0/MANIFEST.in
--rw-r--r--   0 hyi        (502) staff       (20)     7620 2023-04-26 06:40:36.089236 twint_fork-2.5.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     6808 2023-04-26 03:16:17.000000 twint_fork-2.5.0/README.md
--rw-r--r--   0 hyi        (502) staff       (20)       38 2023-04-26 06:40:36.091074 twint_fork-2.5.0/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1803 2023-04-26 06:34:18.000000 twint_fork-2.5.0/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-26 06:40:36.076925 twint_fork-2.5.0/twint/
--rw-r--r--   0 hyi        (502) staff       (20)      808 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       61 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)       64 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/__version__.py
--rw-r--r--   0 hyi        (502) staff       (20)    15324 2023-04-26 06:33:01.000000 twint_fork-2.5.0/twint/cli.py
--rw-r--r--   0 hyi        (502) staff       (20)     2513 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/config.py
--rw-r--r--   0 hyi        (502) staff       (20)     1080 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/datelock.py
--rw-r--r--   0 hyi        (502) staff       (20)     4131 2023-04-26 06:33:01.000000 twint_fork-2.5.0/twint/feed.py
--rw-r--r--   0 hyi        (502) staff       (20)     4464 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/format.py
--rw-r--r--   0 hyi        (502) staff       (20)    11838 2023-04-26 00:44:20.000000 twint_fork-2.5.0/twint/get.py
--rw-r--r--   0 hyi        (502) staff       (20)     8168 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/output.py
--rw-r--r--   0 hyi        (502) staff       (20)    19339 2023-04-26 06:33:01.000000 twint_fork-2.5.0/twint/run.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-26 06:40:36.080912 twint_fork-2.5.0/twint/storage/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-22 13:37:09.000000 twint_fork-2.5.0/twint/storage/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)    11197 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/db.py
--rw-r--r--   0 hyi        (502) staff       (20)    13379 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/elasticsearch.py
--rw-r--r--   0 hyi        (502) staff       (20)     6307 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/panda.py
--rw-r--r--   0 hyi        (502) staff       (20)     2161 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/write.py
--rw-r--r--   0 hyi        (502) staff       (20)     3493 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/write_meta.py
--rw-r--r--   0 hyi        (502) staff       (20)     3937 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/token.py
--rw-r--r--   0 hyi        (502) staff       (20)     5533 2023-04-25 13:25:39.000000 twint_fork-2.5.0/twint/tweet.py
--rw-r--r--   0 hyi        (502) staff       (20)     6026 2023-04-26 02:31:23.000000 twint_fork-2.5.0/twint/url.py
--rw-r--r--   0 hyi        (502) staff       (20)     1285 2023-04-26 00:44:03.000000 twint_fork-2.5.0/twint/user.py
--rw-r--r--   0 hyi        (502) staff       (20)      622 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/verbose.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-26 06:40:36.085332 twint_fork-2.5.0/twint_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)     7620 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      645 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)       62 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       51 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)      137 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)        6 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/top_level.txt
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-10 05:07:37.508225 twint_fork-2.5.1/
+-rw-r--r--   0 hyi        (502) staff       (20)     1071 2023-03-22 13:37:09.000000 twint_fork-2.5.1/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)       26 2023-03-22 13:37:09.000000 twint_fork-2.5.1/MANIFEST.in
+-rw-r--r--   0 hyi        (502) staff       (20)     7665 2023-05-10 05:07:37.507943 twint_fork-2.5.1/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     6853 2023-04-26 08:12:43.000000 twint_fork-2.5.1/README.md
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-05-10 05:07:37.508269 twint_fork-2.5.1/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1815 2023-05-10 05:07:28.000000 twint_fork-2.5.1/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-10 05:07:37.501821 twint_fork-2.5.1/twint/
+-rw-r--r--   0 hyi        (502) staff       (20)      808 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       61 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       64 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/__version__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    15324 2023-04-26 06:33:01.000000 twint_fork-2.5.1/twint/cli.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2513 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/config.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1080 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/datelock.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4001 2023-04-26 14:18:09.000000 twint_fork-2.5.1/twint/feed.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4464 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/format.py
+-rw-r--r--   0 hyi        (502) staff       (20)    11838 2023-04-26 00:44:20.000000 twint_fork-2.5.1/twint/get.py
+-rw-r--r--   0 hyi        (502) staff       (20)     8168 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/output.py
+-rw-r--r--   0 hyi        (502) staff       (20)    19377 2023-04-26 14:17:01.000000 twint_fork-2.5.1/twint/run.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-10 05:07:37.504830 twint_fork-2.5.1/twint/storage/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-22 13:37:09.000000 twint_fork-2.5.1/twint/storage/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    11197 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/db.py
+-rw-r--r--   0 hyi        (502) staff       (20)    13379 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/elasticsearch.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6307 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/panda.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2161 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/write.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3493 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/storage/write_meta.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3937 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/token.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5533 2023-04-25 13:25:39.000000 twint_fork-2.5.1/twint/tweet.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5660 2023-04-26 14:18:30.000000 twint_fork-2.5.1/twint/url.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1285 2023-04-26 00:44:03.000000 twint_fork-2.5.1/twint/user.py
+-rw-r--r--   0 hyi        (502) staff       (20)      622 2023-04-20 09:29:26.000000 twint_fork-2.5.1/twint/verbose.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-05-10 05:07:37.507343 twint_fork-2.5.1/twint_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)     7665 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      645 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       62 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       51 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)      142 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        6 2023-05-10 05:07:37.000000 twint_fork-2.5.1/twint_fork.egg-info/top_level.txt
```

### Comparing `twint_fork-2.5.0/LICENSE` & `twint_fork-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/PKG-INFO` & `twint_fork-2.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twint_fork
-Version: 2.5.0
+Version: 2.5.1
 Summary: An advanced Twitter scraping & OSINT tool.
 Home-page: https://github.com/yihong0618/twint
 Author: Cody Zacharias, yihong0618
 Author-email: codyzacharias@pm.me, zouzou0208@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # This is a fork from twint maintain by yihong0618
+# **For now we can only backup 3200 tweets**
 
 # TWINT - Twitter Intelligence Tool
 ![2](https://i.imgur.com/iaH3s7z.png)
 ![3](https://i.imgur.com/hVeCrqL.png)
 
 [![PyPI](https://img.shields.io/pypi/v/twint.svg)](https://pypi.org/project/twint/) [![Build Status](https://travis-ci.org/twintproject/twint.svg?branch=master)](https://travis-ci.org/twintproject/twint) [![Python 3.6|3.7|3.8](https://img.shields.io/badge/Python-3.6%2F3.7%2F3.8-blue.svg)](https://www.python.org/download/releases/3.0/) [![GitHub license](https://img.shields.io/github/license/haccer/tweep.svg)](https://github.com/haccer/tweep/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/twint)](https://pepy.tech/project/twint) [![Downloads](https://pepy.tech/badge/twint/week)](https://pepy.tech/project/twint/week) [![Patreon](https://img.shields.io/endpoint.svg?url=https:%2F%2Fshieldsio-patreon.herokuapp.com%2Ftwintproject)](https://www.patreon.com/twintproject) ![](https://img.shields.io/twitter/follow/noneprivacy.svg?label=Follow&style=social)
```

### Comparing `twint_fork-2.5.0/README.md` & `twint_fork-2.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # This is a fork from twint maintain by yihong0618
+# **For now we can only backup 3200 tweets**
 
 # TWINT - Twitter Intelligence Tool
 ![2](https://i.imgur.com/iaH3s7z.png)
 ![3](https://i.imgur.com/hVeCrqL.png)
 
 [![PyPI](https://img.shields.io/pypi/v/twint.svg)](https://pypi.org/project/twint/) [![Build Status](https://travis-ci.org/twintproject/twint.svg?branch=master)](https://travis-ci.org/twintproject/twint) [![Python 3.6|3.7|3.8](https://img.shields.io/badge/Python-3.6%2F3.7%2F3.8-blue.svg)](https://www.python.org/download/releases/3.0/) [![GitHub license](https://img.shields.io/github/license/haccer/tweep.svg)](https://github.com/haccer/tweep/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/twint)](https://pepy.tech/project/twint) [![Downloads](https://pepy.tech/badge/twint/week)](https://pepy.tech/project/twint/week) [![Patreon](https://img.shields.io/endpoint.svg?url=https:%2F%2Fshieldsio-patreon.herokuapp.com%2Ftwintproject)](https://www.patreon.com/twintproject) ![](https://img.shields.io/twitter/follow/noneprivacy.svg?label=Follow&style=social)
```

### Comparing `twint_fork-2.5.0/setup.py` & `twint_fork-2.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,24 +23,25 @@
     "pysocks",
     "pandas",
     "aiohttp_socks",
     "schedule",
     "geopy",
     "fake-useragent",
     "googletransx",
+    "rich",
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
 setup(
     name=NAME,
-    version="2.5.0",
+    version="2.5.1",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
```

### Comparing `twint_fork-2.5.0/twint/__init__.py` & `twint_fork-2.5.1/twint/__init__.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/cli.py` & `twint_fork-2.5.1/twint/cli.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/config.py` & `twint_fork-2.5.1/twint/config.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/datelock.py` & `twint_fork-2.5.1/twint/datelock.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/feed.py` & `twint_fork-2.5.1/twint/feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,18 @@
 
 class NoMoreTweetsException(Exception):
     def __init__(self, msg):
         super().__init__(msg)
 
 
 def Follow(response):
-    from rich import print_json
 
     follows = loads(response)
-    print(follows["users"])
     follow = follows["users"]
     logme.debug(__name__ + ":Follow")
-    soup = BeautifulSoup(response, "html.parser")
     cursor = follows["next_cursor_str"]
 
     return follow, cursor
 
 
 # TODO: this won't be used by --profile-full anymore. if it isn't used anywhere else, perhaps remove this in future
 def Mobile(response):
@@ -42,15 +39,14 @@
 
     return tweets, max_id
 
 
 def MobileFav(response):
     from rich import print_json
 
-    print(response)
     soup = BeautifulSoup(response, "html.parser")
     tweets = soup.find_all("table", "tweet")
     max_id = soup.find_all("div", "w-button-more")
     try:
         max_id = findall(r'max_id=(.*?)">', str(max_id))[0]
     except Exception as e:
         print(str(e) + " [x] feed.MobileFav")
```

### Comparing `twint_fork-2.5.0/twint/format.py` & `twint_fork-2.5.1/twint/format.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/get.py` & `twint_fork-2.5.1/twint/get.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/output.py` & `twint_fork-2.5.1/twint/output.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/run.py` & `twint_fork-2.5.1/twint/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
                             time.sleep(1)
                         if favorite_err_cnt == 5:
                             print("Favorite page could not be fetched")
                     if not self.count % 40:
                         time.sleep(5)
                 elif self.config.Followers or self.config.Following:
                     self.feed, self.init = feed.Follow(response)
+                    print(self.count)
                     if not self.count % 40:
                         time.sleep(5)
                 elif self.config.Profile or self.config.TwitterSearch:
                     try:
                         # track the max_id if we need to continue
                         # ticky to make slef.feed to empty
                         # TODO
```

### Comparing `twint_fork-2.5.0/twint/storage/db.py` & `twint_fork-2.5.1/twint/storage/db.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/storage/elasticsearch.py` & `twint_fork-2.5.1/twint/storage/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/storage/panda.py` & `twint_fork-2.5.1/twint/storage/panda.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/storage/write.py` & `twint_fork-2.5.1/twint/storage/write.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/storage/write_meta.py` & `twint_fork-2.5.1/twint/storage/write_meta.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/token.py` & `twint_fork-2.5.1/twint/token.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/tweet.py` & `twint_fork-2.5.1/twint/tweet.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/url.py` & `twint_fork-2.5.1/twint/url.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,35 +26,34 @@
 
 
 async def Favorites(username, init):
     logme.debug(__name__ + ":Favorites")
     url = f"{mobile}/{username}/favorites?lang=en"
 
     url = f"https://api.twitter.com/1.1/favorites/list.json?screen_name={username}"
-    print(url)
     if init != "-1":
         url += f"&max_id={init}"
 
     return url
 
 
 async def Followers(username, init):
     logme.debug(__name__ + ":Followers")
     url = f"{mobile}/{username}/followers?lang=en"
-    url = f"https://api.twitter.com/1.1/followers/list.json?screen_name={username}&count=100"
+    url = f"https://api.twitter.com/1.1/followers/list.json?screen_name={username}&count=200"
 
     if init != "-1":
         url += f"&cursor={init}"
 
     return url
 
 
 async def Following(username, init):
     logme.debug(__name__ + ":Following")
-    url = f"https://api.twitter.com/1.1/friends/list.json?screen_name={username}&count=100"
+    url = f"https://api.twitter.com/1.1/friends/list.json?screen_name={username}&count=200"
 
     if init != "-1":
         url += f"&cursor={init}"
 
     return url
 
 
@@ -70,36 +69,26 @@
 
 async def Search(config, init):
     logme.debug(__name__ + ":Search")
     url = base
     tweet_count = 100 if not config.Limit else config.Limit
     q = ""
     params = [
-        # ('include_blocking', '1'),
-        # ('include_blocked_by', '1'),
-        # ('include_followed_by', '1'),
-        # ('include_want_retweets', '1'),
-        # ('include_mute_edge', '1'),
-        # ('include_can_dm', '1'),
         ("include_can_media_tag", "1"),
-        # ('skip_status', '1'),
-        # ('include_cards', '1'),
         ("include_ext_alt_text", "true"),
         ("include_quote_count", "true"),
         ("include_reply_count", "1"),
         ("tweet_mode", "extended"),
         ("include_entities", "true"),
         ("include_user_entities", "true"),
         ("include_ext_media_availability", "true"),
         ("send_error_codes", "true"),
         ("simple_quoted_tweet", "true"),
         ("count", tweet_count),
         ("query_source", "typed_query"),
-        # ('pc', '1'),
-        ("cursor", str(init)),
         ("spelling_corrections", "1"),
         ("ext", "mediaStats%2ChighlightedLabel"),
         (
             "tweet_search_mode",
             "live",
         ),  # this can be handled better, maybe take an argument and set it then
     ]
@@ -136,17 +125,17 @@
         q += " exclude:links"
     if config.Source:
         q += f' source:"{config.Source}"'
     q = q.strip()
     params.append(("q", q))
     _serialQuery = _sanitizeQuery(url, params)
     if init != -1:
-        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&count=100&max_id={init}"
+        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&count=200&max_id={init}"
     else:
-        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&count=100"
+        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&count=200"
     return url, params, _serialQuery
 
 
 def SearchProfile(config, init=None):
     logme.debug(__name__ + ":SearchProfile")
     _url = "https://api.twitter.com/2/timeline/profile/{user_id}.json".format(
         user_id=config.User_id
```

### Comparing `twint_fork-2.5.0/twint/user.py` & `twint_fork-2.5.1/twint/user.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint/verbose.py` & `twint_fork-2.5.1/twint/verbose.py`

 * *Files identical despite different names*

### Comparing `twint_fork-2.5.0/twint_fork.egg-info/PKG-INFO` & `twint_fork-2.5.1/twint_fork.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twint-fork
-Version: 2.5.0
+Version: 2.5.1
 Summary: An advanced Twitter scraping & OSINT tool.
 Home-page: https://github.com/yihong0618/twint
 Author: Cody Zacharias, yihong0618
 Author-email: codyzacharias@pm.me, zouzou0208@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # This is a fork from twint maintain by yihong0618
+# **For now we can only backup 3200 tweets**
 
 # TWINT - Twitter Intelligence Tool
 ![2](https://i.imgur.com/iaH3s7z.png)
 ![3](https://i.imgur.com/hVeCrqL.png)
 
 [![PyPI](https://img.shields.io/pypi/v/twint.svg)](https://pypi.org/project/twint/) [![Build Status](https://travis-ci.org/twintproject/twint.svg?branch=master)](https://travis-ci.org/twintproject/twint) [![Python 3.6|3.7|3.8](https://img.shields.io/badge/Python-3.6%2F3.7%2F3.8-blue.svg)](https://www.python.org/download/releases/3.0/) [![GitHub license](https://img.shields.io/github/license/haccer/tweep.svg)](https://github.com/haccer/tweep/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/twint)](https://pepy.tech/project/twint) [![Downloads](https://pepy.tech/badge/twint/week)](https://pepy.tech/project/twint/week) [![Patreon](https://img.shields.io/endpoint.svg?url=https:%2F%2Fshieldsio-patreon.herokuapp.com%2Ftwintproject)](https://www.patreon.com/twintproject) ![](https://img.shields.io/twitter/follow/noneprivacy.svg?label=Follow&style=social)
```

### Comparing `twint_fork-2.5.0/twint_fork.egg-info/SOURCES.txt` & `twint_fork-2.5.1/twint_fork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

