# Comparing `tmp/hoyo-daily-logins-helper-1.2.3.tar.gz` & `tmp/hoyo-daily-logins-helper-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-1.2.3.tar", last modified: Sat May  6 21:50:24 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.0.0.tar", last modified: Wed May 10 03:04:46 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-1.2.3.tar` & `hoyo-daily-logins-helper-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.381270 hoyo-daily-logins-helper-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.381270 hoyo-daily-logins-helper-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.381270 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/src/games/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/games/genshin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/games/hoyo_checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/games/starrail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.206197 hoyo-daily-logins-helper-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.202197 hoyo-daily-logins-helper-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.202197 hoyo-daily-logins-helper-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 03:04:46.206197 hoyo-daily-logins-helper-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.202197 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:04:46.206197 hoyo-daily-logins-helper-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:46.206197 hoyo-daily-logins-helper-2.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 03:04:46.000000 hoyo-daily-logins-helper-2.0.0/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-10 03:04:26.000000 hoyo-daily-logins-helper-2.0.0/src/main.py
```

### Comparing `hoyo-daily-logins-helper-1.2.3/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.0.0/.github/workflows/deploy.yml`

 * *Files 9% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     environment:
       name: pypi
       url: https://pypi.org/p/hoyo-daily-logins-helper
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v2
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -r requirements.txt
+          pip install .
       - name: Build package
         run: |
           pip install build
           make build
       - name: Publish package to pypi
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `hoyo-daily-logins-helper-1.2.3/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.0.0/.github/workflows/tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,19 @@
   tests:
     name: tests
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v2
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -r requirements.txt
+          pip install .
           pip install ruff
       - name: Lint
         run: ruff check src
       - name: Build
         run: |
           pip install build
           make build
```

### Comparing `hoyo-daily-logins-helper-1.2.3/.gitignore` & `hoyo-daily-logins-helper-2.0.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 /.vscode
+/hoyo-daily-logins-helper.toml
+/_hoyo-daily-logins-helper.toml
 src/_version.py
 
 # Created by https://www.toptal.com/developers/gitignore/api/windows,macos,linux,python,intellij+all,visualstudiocode
 # Edit at https://www.toptal.com/developers/gitignore?templates=windows,macos,linux,python,intellij+all,visualstudiocode
 
 ### Intellij+all ###
 # Covers JetBrains IDEs: IntelliJ, RubyMine, PhpStorm, AppCode, PyCharm, CLion, Android Studio, WebStorm and Rider
```

### Comparing `hoyo-daily-logins-helper-1.2.3/LICENSE` & `hoyo-daily-logins-helper-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.3/PKG-INFO` & `hoyo-daily-logins-helper-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: hoyo-daily-logins-helper
-Version: 1.2.3
-Summary: Get hoyo daily login rewards automatically!
-Author-email: Christopher Kaster <me@atomicptr.de>
-Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hoyo-daily-login-helper
 
 Get hoyo daily login rewards automatically!
 
 ## Usage
 
 1. Get your cookie string, open the daily check in page
@@ -34,15 +23,15 @@
 
 ### Docker
 
 The command line options are also available via environment variables which
 allows you to easily run this script in Docker/Podman!
 
 ```bash
-$ docker run --rm --env GAME=starrail --env COOKIE="your cookie string" ghcr.io/atomicptr/hoyo-daily-logins-helper
+$ docker run --rm --env HOYO_GAME=starrail --env HOYO_COOKIE="your cookie string" ghcr.io/atomicptr/hoyo-daily-logins-helper
 ```
 
 ### pip
 
 ```bash
 $ pip install hoyo-daily-logins-helper
 ```
@@ -50,36 +39,91 @@
 PyPi: https://pypi.org/project/hoyo-daily-logins-helper/
 
 
 ## Configuration
 
 ### Cookie
 
-You can provide the cookie information either via the **COOKIE** environment variable or using the --cookie CLI flag.
+You can provide the cookie information either via the **HOYO_COOKIE** environment variable or using the --cookie CLI flag.
 
 ### Game
 
-You can provide the cookie information either via the **GAME** environment variable or using the --genshin/--starrail CLI flags.
+You can provide the cookie information either via the **HOYO_GAME** environment variable or using the --game NAME/--genshin/--starrail CLI flags.
 
 **Supported Games**: Genshin Impact (genshin), Honkai Starrail (starrail)
 
 ### Debug mode
 
 If something doesn't work properly and/or you want to report an issue try running the tool with the **DEBUG_MODE** environment variable set to 1! Or provide the --debug flag!
 
 ```bash
-$ DEBUG_MODE=1 hoyo-daily-logins-helper --starrail --cookie="..."
+$ HOYO_DEBUG=1 hoyo-daily-logins-helper --starrail --cookie="..."
 ```
 
 ### Language
 
-If you want to see the results in other languages than English you can change them via the **LANGUAGE** environment variable
+If you want to see the results in other languages than English you can change it via the **HOYO_LANGUAGE** environment variable or the --language CLI flag
+
+```bash
+$ HOYO_LANGUAGE=ja-jp hoyo-daily-logins-helper --genshin --cookie="..."
+```
+
+### Multiple accounts
+
+You can run this tool for multiple accounts at once:
+
+```bash
+$ hoyo-daily-logins-helper --game genshin --cookie "cookie for acc 1" --game starrail --cookie "cookie for acc 2"
+```
+
+If you want to do this with environment variables it works basically the same, you just have to seperate the values by a ","
 
 ```bash
-$ LANGUAGE=ja-jp hoyo-daily-logins-helper --genshin --cookie="..."
+$ HOYO_GAME=genshin,starrail HOYO_COOKIE="cookie 1 data...,cookie 2 data..." hoyo-daily-logins-helper
+```
+
+Although I'd recommend you to use a configuration file for this (see the next point)
+
+### Configuration file
+
+If there is a file called "hoyo-daily-logins-helper.toml" in the current working directory (or you provided one via --config-file) the tool will read data from there.
+
+```bash
+$ hoyo-daily-logins-helper --config-file ~/.my-hoyo-logins-helper-config.toml
+```
+
+Content:
+
+```toml
+# you can configurate some things here like the language or the user agent
+# keep in mind that config and every key in there is optional and you can omit it
+[config]
+user-agent = "My fancy user agent"
+language = "en-us"
+
+# every account starts with this index/key 
+[[accounts]]
+# accounts can have identifiers for you to differentiate them in the logs
+# you could for instance add your account name or UID here
+identifier = "My Genshin Account Name"
+# the game identifier which has to be genshin or starrail
+game = "genshin"
+# and the cookie value
+cookie = "My Genshin Cookie..."
+
+# repeat this for every other account you might have
+[[accounts]]
+identifier = "My Starrail Account #1"
+game = "starrail"
+cookie = "My Starrail Cookie..."
+
+[[accounts]]
+identifier = "My Starrail Account #2"
+game = "starrail"
+cookie = "My Starrail Cookie..."
 ```
 
 ## License
 
 GNU General Public License v3
 
-![](https://www.gnu.org/graphics/gplv3-127x51.png)
+![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

### Comparing `hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.0.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 .dockerignore
 .gitignore
 Dockerfile
 LICENSE
 Makefile
-Pipfile
-Pipfile.lock
 README.md
+hoyo-daily-logins-helper.toml.template
 pyproject.toml
-requirements.txt
 setup.py
 .github/workflows/deploy.yml
 .github/workflows/tests.yml
 hoyo_daily_logins_helper.egg-info/PKG-INFO
 hoyo_daily_logins_helper.egg-info/SOURCES.txt
 hoyo_daily_logins_helper.egg-info/dependency_links.txt
 hoyo_daily_logins_helper.egg-info/entry_points.txt
 hoyo_daily_logins_helper.egg-info/requires.txt
 hoyo_daily_logins_helper.egg-info/top_level.txt
 src/__init__.py
 src/__main__.py
 src/_version.py
-src/config.py
+src/games.py
 src/http.py
-src/main.py
-src/games/__init__.py
-src/games/genshin.py
-src/games/hoyo_checkin.py
-src/games/starrail.py
+src/main.py
```

### Comparing `hoyo-daily-logins-helper-1.2.3/src/games/hoyo_checkin.py` & `hoyo-daily-logins-helper-2.0.0/src/games.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,66 @@
 import json
 import random
 import time
 import logging
 
 from src.http import http_get_json, http_post_json
-from src.config import get_config, CONFIG_LANG
 
 
 RET_CODE_ALREADY_SIGNED_IN = -5003
 
+GAMES = {
+    "genshin": {
+        "name": "Genshin Impact",
+        "event_base_url": "https://hk4e-api-os.mihoyo.com/event/sol",
+        "act_id": "e202102251931481",
+    },
+    "starrail": {
+        "name": "Honkai: Star Rail",
+        "event_base_url": "https://sg-public-api.hoyolab.com/event/luna/os",
+        "act_id": "e202303301540311",
+    }
+}
+
 
-def hoyo_checkin(
-    event_base_url: str,
-    act_id: str,
-    cookie_str: str
+def game_perform_checkin(
+    account_ident: str,
+    game: str,
+    cookie_str: str,
+    language: str,
 ):
-    lang = get_config(CONFIG_LANG)
+    if game not in GAMES:
+        raise Exception(f"unknown game identifier found: {game}")
+
+    game_name = GAMES[game]["name"]
+    event_base_url = GAMES[game]["event_base_url"]
+    act_id = GAMES[game]["act_id"]
+
     referer_url = "https://act.hoyolab.com/"
-    reward_url = f"{event_base_url}/home?lang={lang}" \
+    reward_url = f"{event_base_url}/home?lang={language}" \
                  f"&act_id={act_id}"
-    info_url = f"{event_base_url}/info?lang={lang}" \
+    info_url = f"{event_base_url}/info?lang={language}" \
                f"&act_id={act_id}"
-    sign_url = f"{event_base_url}/sign?lang={lang}"
+    sign_url = f"{event_base_url}/sign?lang={language}"
 
     headers = {
         "Referer": referer_url,
         "Accept-Encoding": "gzip, deflate, br",
         "Cookie": cookie_str,
     }
 
     info_list = http_get_json(info_url, headers=headers)
 
     today = info_list.get("data", {}).get("today")
     total_sign_in_day = info_list.get("data", {}).get("total_sign_day")
     already_signed_in = info_list.get("data", {}).get("is_sign")
     first_bind = info_list.get("data", {}).get("first_bind")
 
+    logging.info(f"Attempting checking for game {game_name} ({account_ident})")
+
     if already_signed_in:
         logging.info("Already checked in today")
         return
 
     if first_bind:
         logging.info("Please check in manually once")
         return
```

### Comparing `hoyo-daily-logins-helper-1.2.3/src/http.py` & `hoyo-daily-logins-helper-2.0.0/src/http.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import json
 import logging
 from typing import Dict
 
 import requests
 from requests import HTTPError, Response
 
-from src.config import get_config, CONFIG_USER_AGENT
+USER_AGENT = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) " \
+              "AppleWebKit/537.36 (KHTML, like Gecko) " \
+              "Chrome/74.0.3729.169 Safari/537.36"
+_http_req_settings = {"user_agent": USER_AGENT}
+
+
+def http_set_user_agent(user_agent: str):
+    _http_req_settings["user_agent"] = user_agent
 
 
 def http_get(url: str, max_retries: int = 2, **kwargs) -> Response:
     return http_request("get", url, max_retries, **kwargs)
 
 
 def http_get_json(url: str, max_retries: int = 2, **kwargs) -> Dict[str, any]:
@@ -34,15 +41,15 @@
     max_retries: int = 2,
     **kwargs
 ) -> Response:
     for i in range(max_retries + 1):
         try:
             logging.debug(f"{method.upper()} {url}, REQ: {i+1}/{max_retries}")
             session = requests.Session()
-            session.headers["USER_AGENT"] = get_config(CONFIG_USER_AGENT)
+            session.headers["USER_AGENT"] = _http_req_settings["user_agent"]
             resp = session.request(method, url, **kwargs)
             logging.debug(f"Response: {resp.status_code}\n\n{resp.text}\n")
         except HTTPError as e:
             logging.error(f"HTTP error: {e}, REQ: {i+1}/{max_retries}")
         except KeyError as e:
             logging.error(f"Wrong response: {e}, REQ: {i+1}/{max_retries}")
         except Exception as e:
```

