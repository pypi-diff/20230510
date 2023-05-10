# Comparing `tmp/hoyo-daily-logins-helper-2.0.1.tar.gz` & `tmp/hoyo-daily-logins-helper-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.0.1.tar", last modified: Wed May 10 03:35:36 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.1.0.tar", last modified: Wed May 10 03:53:56 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.0.1.tar` & `hoyo-daily-logins-helper-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.578283 hoyo-daily-logins-helper-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:36.582283 hoyo-daily-logins-helper-2.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 03:35:36.000000 hoyo-daily-logins-helper-2.0.1/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-10 03:35:20.000000 hoyo-daily-logins-helper-2.0.1/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.154625 hoyo-daily-logins-helper-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.150625 hoyo-daily-logins-helper-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.150625 hoyo-daily-logins-helper-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-10 03:53:56.154625 hoyo-daily-logins-helper-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.150625 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:53:56.154625 hoyo-daily-logins-helper-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:56.150625 hoyo-daily-logins-helper-2.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 03:53:56.000000 hoyo-daily-logins-helper-2.1.0/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-10 03:53:39.000000 hoyo-daily-logins-helper-2.1.0/src/main.py
```

### Comparing `hoyo-daily-logins-helper-2.0.1/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.1.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.1/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.1.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.1/.gitignore` & `hoyo-daily-logins-helper-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.1/LICENSE` & `hoyo-daily-logins-helper-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.1/PKG-INFO` & `hoyo-daily-logins-helper-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-Metadata-Version: 2.1
-Name: hoyo-daily-logins-helper
-Version: 2.0.1
-Summary: Get hoyo daily login rewards automatically!
-Author-email: Christopher Kaster <me@atomicptr.de>
-Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
 ## Usage
 
 1. Get your cookie string, open the daily check in page
-   * [Daily Check-in page for Genshin](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
-   * [Daily Check-in page for Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
+   * [Daily Check-in page for Genshin Impact](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
+   * [Daily Check-in page for Honkai: Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
+   * [Daily Check-in page for Honkai Impact 3rd](https://act.hoyolab.com/bbs/event/signin-bh3/index.html?act_id=e202110291205111)
+   * [Daily Check-in page for Tears of Themis](https://act.hoyolab.com/bbs/event/signin/nxx/index.html?act_id=e202202281857121)
 2. Open a development console (F12) and insert the following code:
     ```javascript
     document.cookie
     ```
 3. Copy the returned string should be something like "ltoken=....; account_id=....;" this is your cookie string
 4. Open a terminal with the command prepared and enter:
     ```bash
@@ -56,15 +47,19 @@
 
 You can provide the cookie information either via the **HOYO_COOKIE** environment variable or using the --cookie CLI flag.
 
 ### Game
 
 You can provide the cookie information either via the **HOYO_GAME** environment variable or using the --game NAME/--genshin/--starrail CLI flags.
 
-**Supported Games**: Genshin Impact (genshin), Honkai Starrail (starrail)
+**Supported Games**:
+* Genshin Impact (genshin)
+* Honkai: Star Rail (starrail)
+* Honkai Impact 3rd (honkai)
+* Tears of Themis (themis)
 
 ### Debug mode
 
 If something doesn't work properly and/or you want to report an issue try running the tool with the **DEBUG_MODE** environment variable set to 1! Or provide the --debug flag!
 
 ```bash
 $ HOYO_DEBUG=1 hoyo-daily-logins-helper --starrail --cookie="..."
@@ -133,8 +128,8 @@
 cookie = "My Starrail Cookie..."
 ```
 
 ## License
 
 GNU General Public License v3
 
-![](https://www.gnu.org/graphics/gplv3-127x51.png)
+![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.0.1/README.md` & `hoyo-daily-logins-helper-2.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+Metadata-Version: 2.1
+Name: hoyo-daily-logins-helper
+Version: 2.1.0
+Summary: Get hoyo daily login rewards automatically!
+Author-email: Christopher Kaster <me@atomicptr.de>
+Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
 ## Usage
 
 1. Get your cookie string, open the daily check in page
-   * [Daily Check-in page for Genshin](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
-   * [Daily Check-in page for Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
+   * [Daily Check-in page for Genshin Impact](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
+   * [Daily Check-in page for Honkai: Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
+   * [Daily Check-in page for Honkai Impact 3rd](https://act.hoyolab.com/bbs/event/signin-bh3/index.html?act_id=e202110291205111)
+   * [Daily Check-in page for Tears of Themis](https://act.hoyolab.com/bbs/event/signin/nxx/index.html?act_id=e202202281857121)
 2. Open a development console (F12) and insert the following code:
     ```javascript
     document.cookie
     ```
 3. Copy the returned string should be something like "ltoken=....; account_id=....;" this is your cookie string
 4. Open a terminal with the command prepared and enter:
     ```bash
@@ -45,15 +58,19 @@
 
 You can provide the cookie information either via the **HOYO_COOKIE** environment variable or using the --cookie CLI flag.
 
 ### Game
 
 You can provide the cookie information either via the **HOYO_GAME** environment variable or using the --game NAME/--genshin/--starrail CLI flags.
 
-**Supported Games**: Genshin Impact (genshin), Honkai Starrail (starrail)
+**Supported Games**:
+* Genshin Impact (genshin)
+* Honkai: Star Rail (starrail)
+* Honkai Impact 3rd (honkai)
+* Tears of Themis (themis)
 
 ### Debug mode
 
 If something doesn't work properly and/or you want to report an issue try running the tool with the **DEBUG_MODE** environment variable set to 1! Or provide the --debug flag!
 
 ```bash
 $ HOYO_DEBUG=1 hoyo-daily-logins-helper --starrail --cookie="..."
@@ -122,8 +139,8 @@
 cookie = "My Starrail Cookie..."
 ```
 
 ## License
 
 GNU General Public License v3
 
-![](https://www.gnu.org/graphics/gplv3-127x51.png)
+![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.0.1
+Version: 2.1.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,16 +12,18 @@
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
 ## Usage
 
 1. Get your cookie string, open the daily check in page
-   * [Daily Check-in page for Genshin](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
-   * [Daily Check-in page for Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
+   * [Daily Check-in page for Genshin Impact](https://act.hoyolab.com/ys/event/signin-sea-v3/index.html?act_id=e202102251931481)
+   * [Daily Check-in page for Honkai: Star Rail](https://act.hoyolab.com/bbs/event/signin/hkrpg/index.html?act_id=e202303301540311)
+   * [Daily Check-in page for Honkai Impact 3rd](https://act.hoyolab.com/bbs/event/signin-bh3/index.html?act_id=e202110291205111)
+   * [Daily Check-in page for Tears of Themis](https://act.hoyolab.com/bbs/event/signin/nxx/index.html?act_id=e202202281857121)
 2. Open a development console (F12) and insert the following code:
     ```javascript
     document.cookie
     ```
 3. Copy the returned string should be something like "ltoken=....; account_id=....;" this is your cookie string
 4. Open a terminal with the command prepared and enter:
     ```bash
@@ -56,15 +58,19 @@
 
 You can provide the cookie information either via the **HOYO_COOKIE** environment variable or using the --cookie CLI flag.
 
 ### Game
 
 You can provide the cookie information either via the **HOYO_GAME** environment variable or using the --game NAME/--genshin/--starrail CLI flags.
 
-**Supported Games**: Genshin Impact (genshin), Honkai Starrail (starrail)
+**Supported Games**:
+* Genshin Impact (genshin)
+* Honkai: Star Rail (starrail)
+* Honkai Impact 3rd (honkai)
+* Tears of Themis (themis)
 
 ### Debug mode
 
 If something doesn't work properly and/or you want to report an issue try running the tool with the **DEBUG_MODE** environment variable set to 1! Or provide the --debug flag!
 
 ```bash
 $ HOYO_DEBUG=1 hoyo-daily-logins-helper --starrail --cookie="..."
```

### Comparing `hoyo-daily-logins-helper-2.0.1/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.1.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.1/pyproject.toml` & `hoyo-daily-logins-helper-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.1/src/games.py` & `hoyo-daily-logins-helper-2.1.0/src/games.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,24 @@
         "event_base_url": "https://hk4e-api-os.mihoyo.com/event/sol",
         "act_id": "e202102251931481",
     },
     "starrail": {
         "name": "Honkai: Star Rail",
         "event_base_url": "https://sg-public-api.hoyolab.com/event/luna/os",
         "act_id": "e202303301540311",
+    },
+    "honkai": {
+        "name": "Honkai Impact 3rd",
+        "event_base_url": "https://sg-public-api.hoyolab.com/event/mani",
+        "act_id": "e202110291205111",
+    },
+    "themis": {
+        "name": "Tears of Themis",
+        "event_base_url": "https://sg-public-api.hoyolab.com/event/luna/os",
+        "act_id": "e202202281857121",
     }
 }
 
 
 def game_perform_checkin(
     account_ident: str,
     game: str,
```

### Comparing `hoyo-daily-logins-helper-2.0.1/src/http.py` & `hoyo-daily-logins-helper-2.1.0/src/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.0.1/src/main.py` & `hoyo-daily-logins-helper-2.1.0/src/main.py`

 * *Files identical despite different names*

