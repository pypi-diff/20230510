# Comparing `tmp/nonebot_plugin_majsoul-0.1.5.tar.gz` & `tmp/nonebot_plugin_majsoul-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_majsoul-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_majsoul-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_majsoul-0.1.5.tar` & `nonebot_plugin_majsoul-0.1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.1.5/LICENSE
--rw-r--r--   0        0        0      623 2023-03-23 15:10:15.714954 nonebot_plugin_majsoul-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2449 2022-12-17 10:37:40.516448 nonebot_plugin_majsoul-0.1.5/README.md
--rw-r--r--   0        0        0     1321 2023-03-23 15:20:27.440710 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/__init__.py
--rw-r--r--   0        0        0      237 2023-03-01 06:00:00.226716 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/config.py
--rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/errors.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/interceptors/__init__.py
--rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/interceptors/handle_error.py
--rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/network/__init__.py
--rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/network/auto_retry.py
--rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/network/host_prober.py
--rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
--rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/api.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
--rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
--rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
--rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
--rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
--rw-r--r--   0        0        0     1462 2023-03-28 04:44:16.684869 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
--rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
--rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
--rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
--rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
--rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
--rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
--rw-r--r--   0        0        0      437 2022-12-05 03:56:01.874405 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
--rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
--rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
--rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
--rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
--rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
--rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
--rw-r--r--   0        0        0     7084 2023-03-28 04:33:39.952291 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
--rw-r--r--   0        0        0     9420 2023-03-28 05:00:03.699457 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
--rw-r--r--   0        0        0     6787 2023-03-28 04:38:12.028043 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
--rw-r--r--   0        0        0        0 2022-12-05 07:11:39.109850 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/res/__init__.py
--rw-r--r--   0        0        0  9765052 2022-12-05 07:11:39.108850 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/res/LXGWWenKaiMonoLite-Regular.ttf
--rw-r--r--   0        0        0        0 2022-12-04 13:54:54.946684 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/utils/__init__.py
--rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/utils/decode_integer.py
--rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/utils/my_executor.py
--rw-r--r--   0        0        0      101 2022-10-29 00:19:22.302000 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/utils/nonebot.py
--rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/utils/percentile.py
--rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/utils/rank.py
--rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448957 nonebot_plugin_majsoul-0.1.6/LICENSE
+-rw-r--r--   0        0        0      623 2023-05-10 04:23:05.048672 nonebot_plugin_majsoul-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2449 2022-12-17 10:37:40.516448 nonebot_plugin_majsoul-0.1.6/README.md
+-rw-r--r--   0        0        0     1321 2023-03-23 15:20:27.440710 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/__init__.py
+-rw-r--r--   0        0        0      237 2023-03-01 06:00:00.226716 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/config.py
+-rw-r--r--   0        0        0      189 2022-12-04 13:51:12.479077 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/errors.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.480120 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/interceptors/__init__.py
+-rw-r--r--   0        0        0     1463 2022-12-05 01:32:49.512537 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/interceptors/handle_error.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:13:35.630196 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/__init__.py
+-rw-r--r--   0        0        0      730 2022-12-09 13:59:04.659310 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/auto_retry.py
+-rw-r--r--   0        0        0     3623 2022-12-09 13:59:04.628312 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/host_prober.py
+-rw-r--r--   0        0        0      108 2022-12-05 07:11:39.022841 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475435 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/__init__.py
+-rw-r--r--   0        0        0     5024 2022-12-05 14:11:58.665190 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/api.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.475949 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/__init__.py
+-rw-r--r--   0        0        0     1194 2022-12-05 03:49:36.925512 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py
+-rw-r--r--   0        0        0     1967 2022-12-13 10:02:54.142968 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py
+-rw-r--r--   0        0        0      608 2022-12-05 14:13:38.468214 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py
+-rw-r--r--   0        0        0       85 2022-12-04 13:51:12.476988 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_num.py
+-rw-r--r--   0        0        0     1538 2023-05-10 04:19:02.870093 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py
+-rw-r--r--   0        0        0      490 2022-12-13 10:02:53.723372 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_stats.py
+-rw-r--r--   0        0        0     2153 2022-12-04 13:51:12.478551 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.481159 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/__init__.py
+-rw-r--r--   0        0        0     2377 2022-12-05 07:11:39.023842 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py
+-rw-r--r--   0        0        0      262 2022-12-04 13:51:12.481677 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/general.py
+-rw-r--r--   0        0        0     1634 2022-12-04 14:39:58.711032 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py
+-rw-r--r--   0        0        0      232 2022-12-04 13:58:13.904298 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_num.py
+-rw-r--r--   0        0        0      480 2023-05-10 04:19:26.060573 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_rank.py
+-rw-r--r--   0        0        0     2536 2022-12-05 14:13:31.596221 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py
+-rw-r--r--   0        0        0     4126 2022-12-04 13:58:13.909299 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py
+-rw-r--r--   0        0        0        0 2022-12-04 13:51:12.483754 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/__init__.py
+-rw-r--r--   0        0        0      568 2023-01-25 14:19:08.842106 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py
+-rw-r--r--   0        0        0     2544 2022-12-04 15:26:45.927547 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py
+-rw-r--r--   0        0        0     1189 2023-01-25 14:19:08.832105 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py
+-rw-r--r--   0        0        0     7318 2023-05-10 04:08:59.781216 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py
+-rw-r--r--   0        0        0     9420 2023-03-28 05:00:03.699457 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py
+-rw-r--r--   0        0        0     6945 2023-05-10 04:08:59.775198 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py
+-rw-r--r--   0        0        0        0 2022-12-05 07:11:39.109850 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/res/__init__.py
+-rw-r--r--   0        0        0  9765052 2022-12-05 07:11:39.108850 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/res/LXGWWenKaiMonoLite-Regular.ttf
+-rw-r--r--   0        0        0        0 2022-12-04 13:54:54.946684 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/__init__.py
+-rw-r--r--   0        0        0     1148 2022-12-04 13:51:12.509611 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/decode_integer.py
+-rw-r--r--   0        0        0      354 2022-12-11 14:52:31.955889 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/my_executor.py
+-rw-r--r--   0        0        0      101 2022-10-29 00:19:22.302000 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/nonebot.py
+-rw-r--r--   0        0        0       98 2022-12-04 14:29:52.531881 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/percentile.py
+-rw-r--r--   0        0        0      482 2022-12-05 03:18:06.269891 nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/rank.py
+-rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 nonebot_plugin_majsoul-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_majsoul-0.1.5/LICENSE` & `nonebot_plugin_majsoul-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/pyproject.toml` & `nonebot_plugin_majsoul-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-majsoul"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 packages = [
     { include = "nonebot_plugin_majsoul", from = "src" },
 ]
```

### Comparing `nonebot_plugin_majsoul-0.1.5/README.md` & `nonebot_plugin_majsoul-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/__init__.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/interceptors/handle_error.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/interceptors/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/network/auto_retry.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/auto_retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/network/host_prober.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/network/host_prober.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/api.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/player_rank.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 class PlayerMajorRank(int, Enum):
     novice = 1
     adept = 2
     expert = 3
     master = 4
     saint = 5
+    celestial_old = 6
     celestial = 7
 
 
 _RANK_MAX_PT = {
     203: 1000,
     301: 1200,
     302: 1400,
@@ -45,15 +46,15 @@
         game_players = code // 10000
         major_rank = code % 1000 // 100
         minor_rank = code % 100
         return PlayerRank(PlayerNum(game_players), PlayerMajorRank(major_rank), minor_rank)
 
     @property
     def max_pt(self) -> int:
-        if self.major_rank != PlayerMajorRank.celestial:
+        if self.major_rank != PlayerMajorRank.celestial and self.major_rank != PlayerMajorRank.celestial_old:
             return _RANK_MAX_PT[self.major_rank * 100 + self.minor_rank]
         else:
             return _CELESTIAL_MAX_PT
 
     def __lt__(self, other):
         if isinstance(other, PlayerRank):
             return self.code < other.code
```

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/data/models/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/game_record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_extended_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/player_stats.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/mappers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/limit_of_games.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/room_rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/parsers/time_span.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,36 +105,36 @@
             sio.write("没有查询到该角色在金之间以上的对局数据呢~")
         else:
             if len(players) > 1:
                 sio.write("查询到多条角色昵称呢~，若输出不是您想查找的昵称，请补全查询昵称。\n")
 
             sio.write(f"昵称：{players[0].nickname}\n\n")
 
-            if limit is not None:
-                records = await api[player_num].player_records(
+            try:
+                if limit is not None:
+                    records = await api[player_num].player_records(
+                        players[0].id,
+                        start_time,
+                        end_time,
+                        room_rank,
+                        limit=limit,
+                        descending=True)
+                    start_time = records[-1].start_time
+
+                player_stats = create_task(api[player_num].player_stats(
                     players[0].id,
                     start_time,
                     end_time,
-                    room_rank,
-                    limit=limit,
-                    descending=True)
-                start_time = records[-1].start_time
-
-            player_stats = create_task(api[player_num].player_stats(
-                players[0].id,
-                start_time,
-                end_time,
-                room_rank))
-            player_extended_stats = create_task(api[player_num].player_extended_stats(
-                players[0].id,
-                start_time,
-                end_time,
-                room_rank))
+                    room_rank))
+                player_extended_stats = create_task(api[player_num].player_extended_stats(
+                    players[0].id,
+                    start_time,
+                    end_time,
+                    room_rank))
 
-            try:
                 player_stats = await player_stats
                 player_extended_stats = await player_extended_stats
             except HTTPStatusError as e:
                 if e.response.status_code == 404:
                     player_stats = None
                 else:
                     raise e
@@ -146,15 +146,18 @@
                 map_player_stats(sio, player_stats, room_rank_text, player_num)
                 sio.write('\n')
                 map_player_extended_stats(sio, player_extended_stats, room_rank_text)
 
             sio.write("\nPS：本数据不包含金之间以下对局以及2019.11.29之前的对局")
 
             with StringIO() as url:
-                url.write(f"https://amae-koromo.sapk.ch/player/{players[0].id}/")
+                if player_num == PlayerNum.four:
+                    url.write(f"https://amae-koromo.sapk.ch/player/{players[0].id}/")
+                else:
+                    url.write(f"https://ikeda.sapk.ch/player/{players[0].id}/")
                 url.write(".".join(map(lambda x: str(x.value), room_rank)))
                 if not default_start_time:
                     url.write("/")
                     url.write(start_time.strftime("%Y-%m-%d"))
                 if not default_end_time:
                     url.write("/")
                     url.write(end_time.strftime("%Y-%m-%d"))
```

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_pt_plot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/paifuya/query_majsoul_records.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,18 @@
 
             for i, r in enumerate(records):
                 with StringIO() as sio:
                     map_game_record(sio, r, players[0].id)
                     msgs.append(MessageFactory(Text(sio.getvalue().strip())))
 
             with StringIO() as url:
-                url.write(f"https://amae-koromo.sapk.ch/player/{players[0].id}/")
+                if player_num == PlayerNum.four:
+                    url.write(f"https://amae-koromo.sapk.ch/player/{players[0].id}/")
+                else:
+                    url.write(f"https://ikeda.sapk.ch/player/{players[0].id}/")
                 url.write(".".join(map(lambda x: str(x.value), room_rank)))
 
                 msgs.append(MessageFactory(Text(f"更多信息：{url.getvalue()}")))
 
     if len(msgs) == 1:
         await msgs[0].send(reply=True)
     else:
```

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/res/LXGWWenKaiMonoLite-Regular.ttf` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/res/LXGWWenKaiMonoLite-Regular.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/src/nonebot_plugin_majsoul/utils/decode_integer.py` & `nonebot_plugin_majsoul-0.1.6/src/nonebot_plugin_majsoul/utils/decode_integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_majsoul-0.1.5/PKG-INFO` & `nonebot_plugin_majsoul-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-majsoul
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 License: AGPL-3.0
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-majsoul Version: 0.1.6 Summary:
 License: AGPL-3.0 Author: ssttkkl Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.0,<0.24.0) Requires-
 Dist: icmplib (>=3.0.3,<4.0.0) Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: monthdelta (>=0.9.1,<0.10.0) Requires-Dist: nonebot-plugin-send-
```

