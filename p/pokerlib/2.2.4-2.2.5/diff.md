# Comparing `tmp/pokerlib-2.2.4.tar.gz` & `tmp/pokerlib-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerlib-2.2.4.tar", max compression
+gzip compressed data, was "pokerlib-2.2.5.tar", max compression
```

## Comparing `pokerlib-2.2.4.tar` & `pokerlib-2.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.4/LICENSE
--rw-r--r--   0        0        0     5980 2023-05-05 21:16:26.697525 pokerlib-2.2.4/README.md
--rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.4/pokerlib/__init__.py
--rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/_handparser.py
--rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/_player.py
--rw-r--r--   0        0        0    17944 2023-05-08 12:46:59.828312 pokerlib-2.2.4/pokerlib/_round.py
--rw-r--r--   0        0        0     6937 2023-05-08 12:36:12.798296 pokerlib-2.2.4/pokerlib/_table.py
--rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/enums.py
--rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/implementations/__init__.py
--rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/implementations/_no_muck_showdown_table.py
--rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.4/pokerlib/implementations/_no_muck_table.py
--rw-r--r--   0        0        0      663 2023-05-09 16:39:25.052221 pokerlib-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 pokerlib-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.5/LICENSE
+-rw-r--r--   0        0        0     5980 2023-05-05 21:16:26.697525 pokerlib-2.2.5/README.md
+-rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.5/pokerlib/__init__.py
+-rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/_handparser.py
+-rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/_player.py
+-rw-r--r--   0        0        0    18193 2023-05-10 20:45:00.132337 pokerlib-2.2.5/pokerlib/_round.py
+-rw-r--r--   0        0        0     6937 2023-05-08 12:36:12.798296 pokerlib-2.2.5/pokerlib/_table.py
+-rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/enums.py
+-rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/implementations/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/implementations/_no_muck_showdown_table.py
+-rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/implementations/_no_muck_table.py
+-rw-r--r--   0        0        0      663 2023-05-10 20:45:42.772328 pokerlib-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 pokerlib-2.2.5/PKG-INFO
```

### Comparing `pokerlib-2.2.4/LICENSE` & `pokerlib-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.4/README.md` & `pokerlib-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.4/pokerlib/_handparser.py` & `pokerlib-2.2.5/pokerlib/_handparser.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.4/pokerlib/_player.py` & `pokerlib-2.2.5/pokerlib/_player.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.4/pokerlib/_round.py` & `pokerlib-2.2.5/pokerlib/_round.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,32 @@
         return player in self.players
 
     def __getitem__(self, _id):
         return self.players.getPlayerById(_id)
 
     @property
     def starting_player_index(self):
+        if getattr(self, 'turn', Turn.PREFLOP) == Turn.PREFLOP:
+            return self.players.nextUnfoldedIndex(self.big_blind_player_index)
         return self.players.nextUnfoldedIndex(self.button)
     @property
     def last_aggressor_index(self):
         return self.players.previousUnfoldedIndex(
             self.current_index)
     @property
     def small_blind_player_index(self):
-        return (self.button - 1) % len(self.players)
+        return (self.button + 1) % len(self.players)
     @property
     def big_blind_player_index(self):
-        return (self.button - 2) % len(self.players)
+        return (self.button + 2) % len(self.players)
 
     @property
     def current_player(self):
+        if not isinstance(self.current_index, int):
+            self.current_index = self.current_index()
         return self.players[self.current_index]
 
     @property
     def turn_stake(self):
         return max(map(
             lambda player: player.turn_stake[self.turn],
             self.players
```

### Comparing `pokerlib-2.2.4/pokerlib/_table.py` & `pokerlib-2.2.5/pokerlib/_table.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.4/pokerlib/enums.py` & `pokerlib-2.2.5/pokerlib/enums.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.4/pyproject.toml` & `pokerlib-2.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokerlib"
-version = "2.2.4"
+version = "2.2.5"
 description = "Python poker library"
 repository = "https://github.com/kuco23/pokerlib/"
 authors = ["kuco23 <nseverkar@gmail.com>"]
 keywords = ['python', 'poker', 'library']
 readme = "README.md"
 classifiers=  [
     'Development Status :: 3 - Alpha',
```

### Comparing `pokerlib-2.2.4/PKG-INFO` & `pokerlib-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerlib
-Version: 2.2.4
+Version: 2.2.5
 Summary: Python poker library
 Home-page: https://github.com/kuco23/pokerlib/
 Keywords: python,poker,library
 Author: kuco23
 Author-email: nseverkar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

