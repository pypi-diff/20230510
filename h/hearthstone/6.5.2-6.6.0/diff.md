# Comparing `tmp/hearthstone-6.5.2.tar.gz` & `tmp/hearthstone-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-6.5.2.tar", last modified: Mon Apr 24 10:53:45 2023, max compression
+gzip compressed data, was "hearthstone-6.6.0.tar", last modified: Tue May  9 21:37:00 2023, max compression
```

## Comparing `hearthstone-6.5.2.tar` & `hearthstone-6.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:53:45.425326 hearthstone-6.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-24 10:53:31.000000 hearthstone-6.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 10:53:45.425326 hearthstone-6.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-24 10:53:31.000000 hearthstone-6.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:53:45.425326 hearthstone-6.5.2/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    58839 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:53:45.425326 hearthstone-6.5.2/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-24 10:53:31.000000 hearthstone-6.5.2/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:53:45.425326 hearthstone-6.5.2/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:53:45.000000 hearthstone-6.5.2/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-24 10:53:45.429326 hearthstone-6.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-04-24 10:53:31.000000 hearthstone-6.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:37:00.792928 hearthstone-6.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-09 21:36:54.000000 hearthstone-6.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-09 21:37:00.792928 hearthstone-6.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-09 21:36:54.000000 hearthstone-6.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:37:00.792928 hearthstone-6.6.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59191 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:37:00.792928 hearthstone-6.6.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    11663 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-09 21:36:54.000000 hearthstone-6.6.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:37:00.792928 hearthstone-6.6.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-09 21:37:00.000000 hearthstone-6.6.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 21:37:00.000000 hearthstone-6.6.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:37:00.000000 hearthstone-6.6.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 21:37:00.000000 hearthstone-6.6.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 21:37:00.000000 hearthstone-6.6.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:37:00.000000 hearthstone-6.6.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-09 21:37:00.792928 hearthstone-6.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-05-09 21:36:54.000000 hearthstone-6.6.0/setup.py
```

### Comparing `hearthstone-6.5.2/LICENSE` & `hearthstone-6.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/PKG-INFO` & `hearthstone-6.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 6.5.2
+Version: 6.6.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-6.5.2/README.md` & `hearthstone-6.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/bountyxml.py` & `hearthstone-6.6.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/cardxml.py` & `hearthstone-6.6.0/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/dbf.py` & `hearthstone-6.6.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/deckstrings.py` & `hearthstone-6.6.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/entities.py` & `hearthstone-6.6.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/enums.py` & `hearthstone-6.6.0/hearthstone/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,14 +260,15 @@
 	SHIFTING_WEAPON = 550
 	DEATH_KNIGHT = 554
 	BOSS = 556
 	STAMPEDE = 564
 	EMPOWERED_TREASURE = 646
 	ONE_SIDED_GHOSTLY = 648
 	CURRENT_NEGATIVE_SPELLPOWER = 651
+	DONT_PICK_FROM_SUBSETS = 676
 	IS_VAMPIRE = 680
 	CORRUPTED = 681
 	HIDE_HEALTH = 682
 	HIDE_ATTACK = 683
 	HIDE_COST = 684
 	LIFESTEAL = 685
 	OVERRIDE_EMOTE_0 = 740
@@ -293,15 +294,15 @@
 	REVEAL_CHOICES = 792
 	HERO_DECK_ID = 793
 	HIDDEN_CHOICE = 813
 	ZOMBEAST = 823
 	HERO_EMOTE_SILENCED = 832
 	MINION_IN_HAND_BUFF = 845
 	ECHO = 846
-	MODULAR = 849
+	MAGNETIC = 849
 	IGNORE_HIDE_STATS_FOR_BIG_CARD = 857
 	REAL_TIME_TRANSFORM = 859
 	WAIT_FOR_PLAYER_RECONNECT_PERIOD = 860
 	ETHEREAL = 880
 	EXTRA_DEATHRATTLES_BASE = 882
 	PHASED_RESTART = 888
 	HEALTH_DISPLAY = 917
@@ -477,14 +478,15 @@
 	FORCE_NO_CUSTOM_SPELLS = 1529
 	START_OF_COMBAT = 1531
 	CORRUPTEDCARD = 1551
 	BACON_HERO_EARLY_ACCESS = 1554
 	SPAWN_TIME_COUNT = 1556
 	SKIP_MULLIGAN = 1561
 	COPIED_FROM_ENTITY_ID = 1565
+	BACON_SELL_VALUE = 1587
 	BACON_VERDANTSPHERES = 1598
 	OPPONENT_SIDE_GHOSTLY = 1609
 	FORCE_NO_CUSTOM_LIFETIME_SPELLS = 1613
 	FORCE_NO_CUSTOM_SUMMON_SPELLS = 1614
 	FORCE_NO_CUSTOM_KEYWORD_SPELLS = 1615
 	USE_LEADERBOARD_AS_SPAWN_ORIGIN = 1628
 	BACON_MUKLA_BANANA_SPAWN_COUNT = 1629
@@ -550,14 +552,15 @@
 	BACON_COMEONECOMEALL = 1789
 	LETTUCE_ABILITY_USED_LAST_TURN = 1807
 	LETTUCE_NODE_TYPE = 1808
 	SHOW_DISCOVER_FROM_DECK = 1816
 	MINI_SET = 1824
 	ARMOR_GAINED_THIS_GAME = 1828
 	CANT_TRIGGER_DEATHRATTLE = 1831
+	BACON_BLOODGEMBUFFATKVALUE = 1844
 	CANT_MOVE_MINION = 1848
 	LETTUCE_MERCENARY_EXPERIENCE = 1852
 	LETTUCE_IS_EQUPIMENT = 1855
 	LETTUCE_EQUIPMENT_ID = 1856
 	DARKMOON_FAIRE_PRIZES_ACTIVE = 1895
 	IGNORE_DECK_RULESET = 1896
 	HONORABLEKILL = 1920
@@ -759,24 +762,27 @@
 	BACON_HERO_REWARD_MINION_TYPE = 2750
 	BACON_HERO_HEROPOWER_REWARD_MINION_TYPE = 2751
 	MERCENARIES_DISCOVER_SOURCE = 2752
 	HERO_ATTACK_GIVEN_ADDITIONAL = 2776
 	HERO_ARMOR_GIVEN_ADDITIONAL = 2778
 	LETTUCE_CHARGE = 2779
 	BACON_DIED_LAST_COMBAT_HINT = 2780
+	SHIFTING_LOCATION = 2783
 	UNPLAYABLE_VISUALS = 2798
 	CARDTEXT_ENTITY_AS_NUMBERS = 2802
 	BACON_DOUBLE_QUEST_HERO_POWER = 2803
 	MERCENARIES_TREASURE_SCALE_LEVEL = 2810
 	CARD_COSTS_ARMOR = 2811
 	FINALE = 2820
 	OVERHEAL = 2821
+	BACON_BLOODGEMBUFFHEALTHVALUE = 2827
 	EMOTECHARACTER = 2839
 	HAS_ACTIVATE_POWER = 2840
 	EMOTECLASS = 2851
+	VENOMOUS = 2853
 	MAGNETIC_TO_RACE = 2859
 	BACON_MAX_LEADERBOARD_ARMOR = 2867
 	BACON_REBORN_TOOLTIP = 2870
 	BACON_PUTRICIDESCREATION_TOOLTIP = 2875
 	TAG_SCRIPT_DATA_NUM_3 = 2889
 	CARD_NAME_DATA_1 = 2890
 	BACON_COSTS_HEALTH_TO_BUY = 2911
@@ -788,14 +794,18 @@
 	BONUSEFFECTS = 2934
 	BACON_USE_COIN_BASED_BUDDY_METER = 2935
 	BACON_BUY_BUDDY = 2937
 	BACON_BUY_BUDDY_2 = 2938
 	BACON_SHOW_HEROPOWER_BUDDY_AS_EVOLVING_BIG_CARD = 2943
 	HIDDEN_CHOICE_OVERRIDE = 2946
 	BUILDING_UP = 3016
+	BACON_PAIR_CANDIDATE = 3031
+	BACON_TRIGGER_UPBEAT = 3046
+	BACON_TRIGGER_XY = 3047
+	FAN_LINK = 3052
 
 	InvisibleDeathrattle = 335
 	ImmuneToSpellpower = 349
 	AttackVisualType = 251
 	DevState = 268
 	GrantCharge = 355
 	HealTarget = 361
@@ -824,14 +834,15 @@
 	EXTRA_DEATHRATTLES = EXTRA_MINION_DEATHRATTLES_BASE
 	HAND_REVEALED = ZONES_REVEALED
 	HEALING_DOUBLE = SPELL_HEALING_DOUBLE
 	# HIDE_COST = HIDE_STATS  # Added back
 	KAZAKUS_POTION_POWER_1 = MODULAR_ENTITY_PART_1
 	KAZAKUS_POTION_POWER_2 = MODULAR_ENTITY_PART_2
 	LINKEDCARD = LINKED_ENTITY
+	MODULAR = MAGNETIC
 	RECALL = OVERLOAD
 	RECALL_OWED = OVERLOAD_OWED
 	RED_MANA_CRYSTALS = RED_MANA_GEM
 	TAG_HERO_POWER_DOUBLE = HERO_POWER_DOUBLE
 	TAG_AI_MUST_PLAY = AI_MUST_PLAY
 	# TREASURE = DISCOVER  # Added back
 	SHOWN_HERO_POWER = HERO_POWER
@@ -2090,14 +2101,15 @@
 	SCRIPT_DATA_NUM_1_NUM_2 = 26
 	POWERED_UP = 27
 	MULTIPLE_ALT_TEXT_SCRIPT_DATA_NUMS = 28
 	REFERENCE_SCRIPT_DATA_NUM_1_ENTITY_POWER = 29
 	REFERENCE_SCRIPT_DATA_NUM_1_CARD_DBID = 30
 	REFERENCE_SCRIPT_DATA_NUM_CARD_RACE = 31
 	BG_QUEST = 32
+	MULTIPLE_ALT_TEXT_SCRIPT_DATA_NUMS_REF_SDN6_CARD_DBID = 33
 
 	# Renamed
 	DEPRECATED_5 = PRIMORDIAL_WAND
 	DEPRECATED_6 = ALTERNATE_CARD_TEXT
 	DEPRECATED_8 = GALAKROND_COUNTER
 	DEPRECATED_10 = PLAYER_TAG_THRESHOLD
 	DEPRECATED_11 = ENTITY_TAG_THRESHOLD
```

### Comparing `hearthstone-6.5.2/hearthstone/mercenaryxml.py` & `hearthstone-6.6.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/stringsfile.py` & `hearthstone-6.6.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/utils/__init__.py` & `hearthstone-6.6.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone/xmlutils.py` & `hearthstone-6.6.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/hearthstone.egg-info/PKG-INFO` & `hearthstone-6.6.0/hearthstone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 6.5.2
+Version: 6.6.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-6.5.2/hearthstone.egg-info/SOURCES.txt` & `hearthstone-6.6.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-6.5.2/setup.cfg` & `hearthstone-6.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 6.5.2
+version = 6.6.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

