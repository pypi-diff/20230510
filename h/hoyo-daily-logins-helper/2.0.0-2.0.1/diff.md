# Comparing `tmp/hoyo-daily-logins-helper-2.0.0.tar.gz` & `tmp/hoyo-daily-logins-helper-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.0.0.tar", last modified: Wed May 10 03:04:46 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.0.1.tar", last modified: Wed May 10 03:35:36 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.0.0.tar` & `hoyo-daily-logins-helper-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.206197 hoyo-daily-logins-helper-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.202197 hoyo-daily-logins-helper-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.202197 hoyo-daily-logins-helper-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 03:04:46.206197 hoyo-daily-logins-helper-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.202197 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:04:46.206197 hoyo-daily-logins-helper-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.206197 hoyo-daily-logins-helper-2.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.578283 hoyo-daily-logins-helper-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/main.py
```

### Comparing `hoyo-daily-logins-helper-2.0.0/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.0.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.0/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.0.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.0/.gitignore` & `hoyo-daily-logins-helper-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.0/LICENSE` & `hoyo-daily-logins-helper-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.0/PKG-INFO` & `hoyo-daily-logins-helper-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.0.0
+Version: 2.0.1
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.0.0/README.md` & `hoyo-daily-logins-helper-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.0.0
+Version: 2.0.1
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.0/pyproject.toml` & `hoyo-daily-logins-helper-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.0/src/games.py` & `hoyo-daily-logins-helper-2.0.1/src/games.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,19 @@
         "Referer": referer_url,
         "Accept-Encoding": "gzip, deflate, br",
         "Cookie": cookie_str,
     }
 
     info_list = http_get_json(info_url, headers=headers)
 
+    if not info_list.get("data"):
+        message = info_list.get("message", "None")
+        logging.error(f"Could not retrieve data from API endpoint: {message}")
+        return
+
     today = info_list.get("data", {}).get("today")
     total_sign_in_day = info_list.get("data", {}).get("total_sign_day")
     already_signed_in = info_list.get("data", {}).get("is_sign")
     first_bind = info_list.get("data", {}).get("first_bind")
 
     logging.info(f"Attempting checking for game {game_name} ({account_ident})")
```

### Comparing `hoyo-daily-logins-helper-2.0.0/src/http.py` & `hoyo-daily-logins-helper-2.0.1/src/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.0/src/main.py` & `hoyo-daily-logins-helper-2.0.1/src/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 
     for game in GAMES.keys():
         game_name = GAMES[game]["name"]
         parser.add_argument(
             f"--{game}",
             help=f"run for game {game_name}",
             action="store_const",
-            dest="game",
-            const=[game],
+            dest="overwrite_game",
+            const=game,
         )
 
     parser.add_argument(
         "--user-agent",
         help="run the requests against the API with a different user agent",
         action="store",
     )
@@ -112,19 +112,20 @@
         datefmt="%Y-%m-%dT%H:%M:%S"
     )
 
     logging.info(f"Hoyo Daily Logins Helper - v{__version__}")
     logging.info("If this tool fails, try to update your cookie!")
     logging.debug(f"Arguments: {args}")
 
+    if args.overwrite_game:
+        args.game = [args.overwrite_game]
+
     if has_legacy_environment_variable():
         logging.debug("Legacy environment variable found")
 
-        if "LANG" in os.environ:
-            args.language = os.environ["LANG"]
         if "LANGUAGE" in os.environ:
             args.language = os.environ["LANGUAGE"]
         if "COOKIE" in os.environ:
             args.cookie = [os.environ["COOKIE"]]
         if "GAME" in os.environ:
             args.game = [os.environ["GAME"]]
```

