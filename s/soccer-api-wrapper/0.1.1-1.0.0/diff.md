# Comparing `tmp/soccer-api-wrapper-0.1.1.tar.gz` & `tmp/soccer-api-wrapper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccer-api-wrapper-0.1.1.tar", last modified: Mon Mar 27 01:33:11 2023, max compression
+gzip compressed data, was "soccer-api-wrapper-1.0.0.tar", last modified: Wed May 10 18:39:32 2023, max compression
```

## Comparing `soccer-api-wrapper-0.1.1.tar` & `soccer-api-wrapper-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 01:33:11.232004 soccer-api-wrapper-0.1.1/
--rw-rw-rw-   0        0        0    11558 2023-02-12 16:14:18.000000 soccer-api-wrapper-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    18424 2023-03-27 01:33:11.232004 soccer-api-wrapper-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4416 2023-03-27 00:30:33.000000 soccer-api-wrapper-0.1.1/README.md
--rw-rw-rw-   0        0        0     2309 2023-03-27 01:12:20.000000 soccer-api-wrapper-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-27 01:33:11.232004 soccer-api-wrapper-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-11 21:31:58.000000 soccer-api-wrapper-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 01:33:11.198902 soccer-api-wrapper-0.1.1/soccer_api_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-24 14:22:52.000000 soccer-api-wrapper-0.1.1/soccer_api_wrapper/__init__.py
--rw-rw-rw-   0        0        0     2963 2023-03-27 00:30:33.000000 soccer-api-wrapper-0.1.1/soccer_api_wrapper/soccerapi.py
-drwxrwxrwx   0        0        0        0 2023-03-27 01:33:11.232004 soccer-api-wrapper-0.1.1/soccer_api_wrapper/tests/
--rw-rw-rw-   0        0        0     2005 2023-03-27 00:30:33.000000 soccer-api-wrapper-0.1.1/soccer_api_wrapper/tests/soccerapi_test.py
-drwxrwxrwx   0        0        0        0 2023-03-27 01:33:11.232004 soccer-api-wrapper-0.1.1/soccer_api_wrapper.egg-info/
--rw-rw-rw-   0        0        0    18424 2023-03-27 01:33:11.000000 soccer-api-wrapper-0.1.1/soccer_api_wrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-03-27 01:33:11.000000 soccer-api-wrapper-0.1.1/soccer_api_wrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 01:33:11.000000 soccer-api-wrapper-0.1.1/soccer_api_wrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2023-03-27 01:33:11.000000 soccer-api-wrapper-0.1.1/soccer_api_wrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-27 01:33:11.000000 soccer-api-wrapper-0.1.1/soccer_api_wrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 18:39:32.625426 soccer-api-wrapper-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-10 19:59:22.000000 soccer-api-wrapper-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    18632 2023-05-10 18:39:32.625426 soccer-api-wrapper-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4624 2023-04-10 20:53:01.000000 soccer-api-wrapper-1.0.0/README.md
+-rw-rw-rw-   0        0        0     2309 2023-05-07 01:56:01.000000 soccer-api-wrapper-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:39:32.625426 soccer-api-wrapper-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-10 19:59:22.000000 soccer-api-wrapper-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:39:32.602104 soccer-api-wrapper-1.0.0/soccer_api_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-04-10 19:59:22.000000 soccer-api-wrapper-1.0.0/soccer_api_wrapper/__init__.py
+-rw-rw-rw-   0        0        0    10222 2023-05-07 01:39:52.000000 soccer-api-wrapper-1.0.0/soccer_api_wrapper/soccerapi.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:39:32.624427 soccer-api-wrapper-1.0.0/soccer_api_wrapper/tests/
+-rw-rw-rw-   0        0        0     3853 2023-05-07 01:39:52.000000 soccer-api-wrapper-1.0.0/soccer_api_wrapper/tests/soccerapi_test.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:39:32.619435 soccer-api-wrapper-1.0.0/soccer_api_wrapper.egg-info/
+-rw-rw-rw-   0        0        0    18632 2023-05-10 18:39:32.000000 soccer-api-wrapper-1.0.0/soccer_api_wrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-05-10 18:39:32.000000 soccer-api-wrapper-1.0.0/soccer_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:39:32.000000 soccer-api-wrapper-1.0.0/soccer_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-05-10 18:39:32.000000 soccer-api-wrapper-1.0.0/soccer_api_wrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-10 18:39:32.000000 soccer-api-wrapper-1.0.0/soccer_api_wrapper.egg-info/top_level.txt
```

### Comparing `soccer-api-wrapper-0.1.1/LICENSE` & `soccer-api-wrapper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soccer-api-wrapper-0.1.1/PKG-INFO` & `soccer-api-wrapper-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soccer-api-wrapper
-Version: 0.1.1
+Version: 1.0.0
 Summary: Soccer Api Wrapper
 Author-email: Debi Ejeta <dme2136@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,20 +221,20 @@
 License-File: LICENSE
 
 # soccer-api-wrapper
 
 soccer-api-wrapper is a library for getting information about soccer matches in the five big club competitions, with live score, fixtures, and stats of games available. 
 
 [![](https://img.shields.io/static/v1?label=license&message=Apache-2.0&color=%3CCOLOR%3E)](./LICENSE)
-
 [![](https://img.shields.io/github/issues/Debi-Ejeta/soccer-api-wrapper)](../../issues)
-
 [![codecov](https://codecov.io/gh/Debi-Ejeta/soccer-api-wrapper/branch/main/graph/badge.svg?token=1MBRYEYR2J)](https://codecov.io/gh/Debi-Ejeta/soccer-api-wrapper)
-
 [![Build Status](https://github.com/Debi-Ejeta/soccer-api-wrapper/actions/workflows/workflow.yml/badge.svg)](https://github.com/Debi-Ejeta/soccer-api-wrapper/actions/workflows/workflow.yml)
+[![PyPI](https://img.shields.io/pypi/v/soccer-api-wrapper)](https://pypi.org/project/soccer-api-wrapper/)
+[![Documentation Status](https://readthedocs.org/projects/soccer-api-wrapper/badge/?version=latest)](https://soccer-api-wrapper.readthedocs.io/en/latest/?badge=latest)
+[![Github Page](https://img.shields.io/badge/%20doc-github%20page-%231674b1?style=flat&labelColor=ef8336)](https://debi-ejeta.github.io/soccer-api-wrapper/)
 
 ## Overview
 
 As writing GET and POST requests multiple times to get data can be frustrating, the library will streamline the process of retrieving information about soccer by making the API calls under the hood as an API Wrapper. So if anyone wants to create an app or a bot on apps like Telegram, they will be able to make use of this library to easily create their apps or bots for anything related to soccer without having to make api calls every single time. 
 
 ## Getting Started
 
@@ -254,22 +254,15 @@
 https://www.football-data.org/ as this library is completely based on that 
 API and you will need to provide that token every time you use the functions 
 listed below
 
 In the first verion of this library, only the premier league is supported. 
 Other league functionalities will be added in future versions. 
 
-```py
-from soccer_api_wrapper import soccerapi
-# To check the current standings in the premier league
-teams = soccerapi.get_epl_team_standings("YourAPIToken")
-for team in teams:
-    # prints information about the team strating from club at position 1
-    print(team)
-```
+![[Project Preview]](./docs/previews/get_epl_scorers.gif)
 
 Similarly, there are other functions you can call on soccerapi after importing it:
 
 ```py
 # returns the matches happening within the next couple of days
 soccerapi.get_recent_matches("YourAPIToken")
 ```
```

### Comparing `soccer-api-wrapper-0.1.1/README.md` & `soccer-api-wrapper-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # soccer-api-wrapper
 
 soccer-api-wrapper is a library for getting information about soccer matches in the five big club competitions, with live score, fixtures, and stats of games available. 
 
 [![](https://img.shields.io/static/v1?label=license&message=Apache-2.0&color=%3CCOLOR%3E)](./LICENSE)
-
 [![](https://img.shields.io/github/issues/Debi-Ejeta/soccer-api-wrapper)](../../issues)
-
 [![codecov](https://codecov.io/gh/Debi-Ejeta/soccer-api-wrapper/branch/main/graph/badge.svg?token=1MBRYEYR2J)](https://codecov.io/gh/Debi-Ejeta/soccer-api-wrapper)
-
 [![Build Status](https://github.com/Debi-Ejeta/soccer-api-wrapper/actions/workflows/workflow.yml/badge.svg)](https://github.com/Debi-Ejeta/soccer-api-wrapper/actions/workflows/workflow.yml)
+[![PyPI](https://img.shields.io/pypi/v/soccer-api-wrapper)](https://pypi.org/project/soccer-api-wrapper/)
+[![Documentation Status](https://readthedocs.org/projects/soccer-api-wrapper/badge/?version=latest)](https://soccer-api-wrapper.readthedocs.io/en/latest/?badge=latest)
+[![Github Page](https://img.shields.io/badge/%20doc-github%20page-%231674b1?style=flat&labelColor=ef8336)](https://debi-ejeta.github.io/soccer-api-wrapper/)
 
 ## Overview
 
 As writing GET and POST requests multiple times to get data can be frustrating, the library will streamline the process of retrieving information about soccer by making the API calls under the hood as an API Wrapper. So if anyone wants to create an app or a bot on apps like Telegram, they will be able to make use of this library to easily create their apps or bots for anything related to soccer without having to make api calls every single time. 
 
 ## Getting Started
 
@@ -32,22 +32,15 @@
 https://www.football-data.org/ as this library is completely based on that 
 API and you will need to provide that token every time you use the functions 
 listed below
 
 In the first verion of this library, only the premier league is supported. 
 Other league functionalities will be added in future versions. 
 
-```py
-from soccer_api_wrapper import soccerapi
-# To check the current standings in the premier league
-teams = soccerapi.get_epl_team_standings("YourAPIToken")
-for team in teams:
-    # prints information about the team strating from club at position 1
-    print(team)
-```
+![[Project Preview]](./docs/previews/get_epl_scorers.gif)
 
 Similarly, there are other functions you can call on soccerapi after importing it:
 
 ```py
 # returns the matches happening within the next couple of days
 soccerapi.get_recent_matches("YourAPIToken")
 ```
```

### Comparing `soccer-api-wrapper-0.1.1/pyproject.toml` & `soccer-api-wrapper-1.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "soccer-api-wrapper"
 authors = [{name = "Debi Ejeta", email = "dme2136@columbia.edu"}]
 description="Soccer Api Wrapper"
 readme = "README.md"
-version = "0.1.1"
+version = "1.0.0"
 requires-python = ">=3.7"
 
 dependencies = [
     "requests"
 ]
 
 classifiers = [
```

### Comparing `soccer-api-wrapper-0.1.1/soccer_api_wrapper/tests/soccerapi_test.py` & `soccer-api-wrapper-1.0.0/soccer_api_wrapper/tests/soccerapi_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 class Tests(unittest.TestCase):
     def test_get_recent_matches(self):
         with patch('requests.get') as mock_get:
             soccerapi.get_recent_matches("test_token")
             self.assertEqual(mock_get.called, True)
 
-    def test_get_epl_team_matches(self):
+    def test_get_team_matches(self):
         with patch('requests.get') as mock_get:
-            soccerapi.get_epl_team_matches("test_token", "test")
+            soccerapi.get_team_matches("test_token", "test")
             self.assertEqual(mock_get.called, True)
 
     def test_get_epl_team_matches_for_a_team(self):
         with patch('requests.get') as mock_get:
             mock_get.return_value.json().text = {
                 "id": "57",
                 "team": "Arsenal",
                 "matchday": "14",
                 "opposition": "Manchester City",
             }
-            response = soccerapi.get_epl_team_matches("test_token", "Arsenal")
+            response = soccerapi.get_team_matches("test_token", "Arsenal")
             self.assertEqual(response.text["id"], "57")
             self.assertEqual(response.text["team"], "Arsenal")
             self.assertEqual(response.text["matchday"], "14")
             self.assertEqual(response.text["opposition"], "Manchester City")
 
     def test_get_epl_team_standings(self):
         with patch('requests.get') as mock_get:
@@ -43,7 +43,52 @@
             soccerapi.get_epl_matchday("test_token", 23)
             self.assertEqual(mock_get.called, True)
 
     def test_get_team_info(self):
         with patch('requests.get') as mock_get:
             soccerapi.get_team_info("test_token", 23)
             self.assertEqual(mock_get.called, True)
+
+    def test_get_competitions_for_team(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_competitions_for_team("test_token", 41)
+            self.assertEqual(mock_get.called, True)
+
+    def test_get_players_of_team(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_players_of_team("test_token", 41)
+            self.assertEqual(mock_get.called, True)
+
+    def test_get_player_by_position(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_player_by_position("test_token", 57, "Defender")
+            self.assertEqual(mock_get.called, True)
+
+    def test_get_ucl_matches(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_ucl_matches("test_token")
+            self.assertEqual(mock_get.called, True)
+
+    def test_get_matches(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_matches("test_token", "DED")
+            self.assertEqual(mock_get.called, True)
+
+    def test_get_head_to_head_matches(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_head_to_head_matches("test_token", 43, 34)
+            self.assertEqual(mock_get.called, True)
+
+    def test_get_head_to_head_stats(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_head_to_head_stats("test_token", 43, 34)
+            self.assertEqual(mock_get.called, True)
+
+    def test_get_epl_teams(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_epl_teams("test_token")
+            self.assertEqual(mock_get.called, True)
+
+    def test_get_player_info(self):
+        with patch('requests.get') as mock_get:
+            soccerapi.get_player_info("test_token", 701)
+            self.assertEqual(mock_get.called, True)
```

### Comparing `soccer-api-wrapper-0.1.1/soccer_api_wrapper.egg-info/PKG-INFO` & `soccer-api-wrapper-1.0.0/soccer_api_wrapper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soccer-api-wrapper
-Version: 0.1.1
+Version: 1.0.0
 Summary: Soccer Api Wrapper
 Author-email: Debi Ejeta <dme2136@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,20 +221,20 @@
 License-File: LICENSE
 
 # soccer-api-wrapper
 
 soccer-api-wrapper is a library for getting information about soccer matches in the five big club competitions, with live score, fixtures, and stats of games available. 
 
 [![](https://img.shields.io/static/v1?label=license&message=Apache-2.0&color=%3CCOLOR%3E)](./LICENSE)
-
 [![](https://img.shields.io/github/issues/Debi-Ejeta/soccer-api-wrapper)](../../issues)
-
 [![codecov](https://codecov.io/gh/Debi-Ejeta/soccer-api-wrapper/branch/main/graph/badge.svg?token=1MBRYEYR2J)](https://codecov.io/gh/Debi-Ejeta/soccer-api-wrapper)
-
 [![Build Status](https://github.com/Debi-Ejeta/soccer-api-wrapper/actions/workflows/workflow.yml/badge.svg)](https://github.com/Debi-Ejeta/soccer-api-wrapper/actions/workflows/workflow.yml)
+[![PyPI](https://img.shields.io/pypi/v/soccer-api-wrapper)](https://pypi.org/project/soccer-api-wrapper/)
+[![Documentation Status](https://readthedocs.org/projects/soccer-api-wrapper/badge/?version=latest)](https://soccer-api-wrapper.readthedocs.io/en/latest/?badge=latest)
+[![Github Page](https://img.shields.io/badge/%20doc-github%20page-%231674b1?style=flat&labelColor=ef8336)](https://debi-ejeta.github.io/soccer-api-wrapper/)
 
 ## Overview
 
 As writing GET and POST requests multiple times to get data can be frustrating, the library will streamline the process of retrieving information about soccer by making the API calls under the hood as an API Wrapper. So if anyone wants to create an app or a bot on apps like Telegram, they will be able to make use of this library to easily create their apps or bots for anything related to soccer without having to make api calls every single time. 
 
 ## Getting Started
 
@@ -254,22 +254,15 @@
 https://www.football-data.org/ as this library is completely based on that 
 API and you will need to provide that token every time you use the functions 
 listed below
 
 In the first verion of this library, only the premier league is supported. 
 Other league functionalities will be added in future versions. 
 
-```py
-from soccer_api_wrapper import soccerapi
-# To check the current standings in the premier league
-teams = soccerapi.get_epl_team_standings("YourAPIToken")
-for team in teams:
-    # prints information about the team strating from club at position 1
-    print(team)
-```
+![[Project Preview]](./docs/previews/get_epl_scorers.gif)
 
 Similarly, there are other functions you can call on soccerapi after importing it:
 
 ```py
 # returns the matches happening within the next couple of days
 soccerapi.get_recent_matches("YourAPIToken")
 ```
```

