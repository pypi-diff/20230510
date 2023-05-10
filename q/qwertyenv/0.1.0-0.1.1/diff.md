# Comparing `tmp/qwertyenv-0.1.0.tar.gz` & `tmp/qwertyenv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwertyenv-0.1.0.tar", last modified: Wed May 10 08:23:14 2023, max compression
+gzip compressed data, was "qwertyenv-0.1.1.tar", last modified: Wed May 10 14:37:46 2023, max compression
```

## Comparing `qwertyenv-0.1.0.tar` & `qwertyenv-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/
--rw-r--r--   0 oren      (1000) oren      (1000)     1356 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)      420 2023-02-07 12:50:27.000000 qwertyenv-0.1.0/README.md
--rw-r--r--   0 oren      (1000) oren      (1000)      103 2022-12-24 16:37:54.000000 qwertyenv-0.1.0/pyproject.toml
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/qwertyenv/
--rw-r--r--   0 oren      (1000) oren      (1000)      481 2023-05-10 08:21:08.000000 qwertyenv-0.1.0/qwertyenv/__init__.py
--rw-r--r--   0 oren      (1000) oren      (1000)      689 2023-03-15 14:32:09.000000 qwertyenv-0.1.0/qwertyenv/action_wrapper_pz.py
--rw-r--r--   0 oren      (1000) oren      (1000)     3826 2023-05-10 07:34:14.000000 qwertyenv-0.1.0/qwertyenv/black_jack.py
--rw-r--r--   0 oren      (1000) oren      (1000)     3372 2023-05-10 07:44:21.000000 qwertyenv-0.1.0/qwertyenv/collect_coins.py
--rw-r--r--   0 oren      (1000) oren      (1000)     3230 2023-03-02 16:43:27.000000 qwertyenv-0.1.0/qwertyenv/collect_coins_game.py
--rw-r--r--   0 oren      (1000) oren      (1000)    10008 2023-03-15 16:58:08.000000 qwertyenv-0.1.0/qwertyenv/collect_coins_pz.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1265 2023-05-10 07:20:30.000000 qwertyenv-0.1.0/qwertyenv/ensure_valid_action.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1309 2023-03-13 11:27:57.000000 qwertyenv-0.1.0/qwertyenv/ensure_valid_action_pz.py
--rw-r--r--   0 oren      (1000) oren      (1000)     2417 2023-05-10 08:21:49.000000 qwertyenv-0.1.0/qwertyenv/pz_to_gymnasium_wrapper.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1601 2023-03-15 16:43:32.000000 qwertyenv-0.1.0/qwertyenv/tmp.py
--rw-r--r--   0 oren      (1000) oren      (1000)      850 2023-05-10 07:20:58.000000 qwertyenv-0.1.0/qwertyenv/up_down_left_right.py
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/qwertyenv.egg-info/
--rw-r--r--   0 oren      (1000) oren      (1000)     1356 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)      697 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/SOURCES.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/dependency_links.txt
--rw-r--r--   0 oren      (1000) oren      (1000)      168 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/requires.txt
--rw-r--r--   0 oren      (1000) oren      (1000)       16 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/top_level.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2022-12-24 17:15:22.000000 qwertyenv-0.1.0/qwertyenv.egg-info/zip-safe
--rw-r--r--   0 oren      (1000) oren      (1000)     1257 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/setup.cfg
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/tests/
--rw-r--r--   0 oren      (1000) oren      (1000)        0 2023-02-02 11:54:46.000000 qwertyenv-0.1.0/tests/__init__.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1228 2023-02-07 09:17:40.000000 qwertyenv-0.1.0/tests/test_collect_coins.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1925 2023-03-13 14:20:33.000000 qwertyenv-0.1.0/tests/test_collect_coins_gym_from_pz.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1550 2023-03-14 14:27:41.000000 qwertyenv-0.1.0/tests/test_collect_coins_pz.py
--rw-r--r--   0 oren      (1000) oren      (1000)      347 2023-02-07 12:30:45.000000 qwertyenv-0.1.0/tests/test_up_down_left_right.py
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 14:37:46.788169 qwertyenv-0.1.1/
+-rw-r--r--   0 oren      (1000) oren      (1000)     1356 2023-05-10 14:37:46.788169 qwertyenv-0.1.1/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)      420 2023-02-07 12:50:27.000000 qwertyenv-0.1.1/README.md
+-rw-r--r--   0 oren      (1000) oren      (1000)      103 2022-12-24 16:37:54.000000 qwertyenv-0.1.1/pyproject.toml
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 14:37:46.788169 qwertyenv-0.1.1/qwertyenv/
+-rw-r--r--   0 oren      (1000) oren      (1000)      608 2023-05-10 13:42:38.000000 qwertyenv-0.1.1/qwertyenv/__init__.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      689 2023-03-15 14:32:09.000000 qwertyenv-0.1.1/qwertyenv/action_wrapper_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     3826 2023-05-10 07:34:14.000000 qwertyenv-0.1.1/qwertyenv/black_jack.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     3372 2023-05-10 07:44:21.000000 qwertyenv-0.1.1/qwertyenv/collect_coins.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     3230 2023-03-02 16:43:27.000000 qwertyenv-0.1.1/qwertyenv/collect_coins_game.py
+-rw-r--r--   0 oren      (1000) oren      (1000)    10008 2023-03-15 16:58:08.000000 qwertyenv-0.1.1/qwertyenv/collect_coins_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1265 2023-05-10 07:20:30.000000 qwertyenv-0.1.1/qwertyenv/ensure_valid_action.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1309 2023-03-13 11:27:57.000000 qwertyenv-0.1.1/qwertyenv/ensure_valid_action_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     5828 2023-05-10 14:07:14.000000 qwertyenv-0.1.1/qwertyenv/pz_to_gymnasium_wrappers.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1602 2023-05-10 14:18:27.000000 qwertyenv-0.1.1/qwertyenv/tmp.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      850 2023-05-10 07:20:58.000000 qwertyenv-0.1.1/qwertyenv/up_down_left_right.py
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 14:37:46.788169 qwertyenv-0.1.1/qwertyenv.egg-info/
+-rw-r--r--   0 oren      (1000) oren      (1000)     1356 2023-05-10 14:37:46.000000 qwertyenv-0.1.1/qwertyenv.egg-info/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)      734 2023-05-10 14:37:46.000000 qwertyenv-0.1.1/qwertyenv.egg-info/SOURCES.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-05-10 14:37:46.000000 qwertyenv-0.1.1/qwertyenv.egg-info/dependency_links.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)      204 2023-05-10 14:37:46.000000 qwertyenv-0.1.1/qwertyenv.egg-info/requires.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)       16 2023-05-10 14:37:46.000000 qwertyenv-0.1.1/qwertyenv.egg-info/top_level.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2022-12-24 17:15:22.000000 qwertyenv-0.1.1/qwertyenv.egg-info/zip-safe
+-rw-r--r--   0 oren      (1000) oren      (1000)     1298 2023-05-10 14:37:46.788169 qwertyenv-0.1.1/setup.cfg
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 14:37:46.788169 qwertyenv-0.1.1/tests/
+-rw-r--r--   0 oren      (1000) oren      (1000)        0 2023-02-02 11:54:46.000000 qwertyenv-0.1.1/tests/__init__.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1298 2023-05-10 14:35:12.000000 qwertyenv-0.1.1/tests/test_collect_coins.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     2170 2023-05-10 14:29:25.000000 qwertyenv-0.1.1/tests/test_collect_coins_gym_from_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1550 2023-03-14 14:27:41.000000 qwertyenv-0.1.1/tests/test_collect_coins_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     2097 2023-05-10 13:44:52.000000 qwertyenv-0.1.1/tests/test_gymnasium_conversions.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      360 2023-05-10 14:14:03.000000 qwertyenv-0.1.1/tests/test_up_down_left_right.py
```

### Comparing `qwertyenv-0.1.0/PKG-INFO` & `qwertyenv-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwertyenv
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gym and PettingZoo environments (Reinforcement Learning)
 Home-page: https://github.com/zbenmo/qwertyenv
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 License: BSD 3-Clause License
 Keywords: Gym,Gym environments,Black Jack,Collect Coins (Chesss like),Reinforcement Learning,Gym Wrappers,PettingZoo,MARL,Gymnasium
 Classifier: Intended Audience :: Developers
```

### Comparing `qwertyenv-0.1.0/qwertyenv/action_wrapper_pz.py` & `qwertyenv-0.1.1/qwertyenv/action_wrapper_pz.py`

 * *Files identical despite different names*

### Comparing `qwertyenv-0.1.0/qwertyenv/black_jack.py` & `qwertyenv-0.1.1/qwertyenv/black_jack.py`

 * *Files identical despite different names*

### Comparing `qwertyenv-0.1.0/qwertyenv/collect_coins.py` & `qwertyenv-0.1.1/qwertyenv/collect_coins.py`

 * *Files identical despite different names*

### Comparing `qwertyenv-0.1.0/qwertyenv/collect_coins_game.py` & `qwertyenv-0.1.1/qwertyenv/collect_coins_game.py`

 * *Files identical despite different names*

### Comparing `qwertyenv-0.1.0/qwertyenv/collect_coins_pz.py` & `qwertyenv-0.1.1/qwertyenv/collect_coins_pz.py`

 * *Files identical despite different names*

### Comparing `qwertyenv-0.1.0/qwertyenv/ensure_valid_action.py` & `qwertyenv-0.1.1/qwertyenv/ensure_valid_action.py`

 * *Files identical despite different names*

### Comparing `qwertyenv-0.1.0/qwertyenv/ensure_valid_action_pz.py` & `qwertyenv-0.1.1/qwertyenv/ensure_valid_action_pz.py`

 * *Files identical despite different names*

### Comparing `qwertyenv-0.1.0/qwertyenv/tmp.py` & `qwertyenv-0.1.1/qwertyenv/tmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from qwertyenv.collect_coins_pz import CollectCoinsEnv
-from qwertyenv.pz_to_gymnasium_wrapper import PZ2GymnasiumWrapper
+from qwertyenv.pz_to_gymnasium_wrappers import PZ2GymnasiumWrapper
 from qwertyenv.ensure_valid_action_pz import EnsureValidAction
 # import gym
 import qwertyenv
 import numpy as np
 
 import torch
```

### Comparing `qwertyenv-0.1.0/qwertyenv/up_down_left_right.py` & `qwertyenv-0.1.1/qwertyenv/up_down_left_right.py`

 * *Files identical despite different names*

### Comparing `qwertyenv-0.1.0/qwertyenv.egg-info/PKG-INFO` & `qwertyenv-0.1.1/qwertyenv.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwertyenv
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gym and PettingZoo environments (Reinforcement Learning)
 Home-page: https://github.com/zbenmo/qwertyenv
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 License: BSD 3-Clause License
 Keywords: Gym,Gym environments,Black Jack,Collect Coins (Chesss like),Reinforcement Learning,Gym Wrappers,PettingZoo,MARL,Gymnasium
 Classifier: Intended Audience :: Developers
```

### Comparing `qwertyenv-0.1.0/qwertyenv.egg-info/SOURCES.txt` & `qwertyenv-0.1.1/qwertyenv.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 qwertyenv/action_wrapper_pz.py
 qwertyenv/black_jack.py
 qwertyenv/collect_coins.py
 qwertyenv/collect_coins_game.py
 qwertyenv/collect_coins_pz.py
 qwertyenv/ensure_valid_action.py
 qwertyenv/ensure_valid_action_pz.py
-qwertyenv/pz_to_gymnasium_wrapper.py
+qwertyenv/pz_to_gymnasium_wrappers.py
 qwertyenv/tmp.py
 qwertyenv/up_down_left_right.py
 qwertyenv.egg-info/PKG-INFO
 qwertyenv.egg-info/SOURCES.txt
 qwertyenv.egg-info/dependency_links.txt
 qwertyenv.egg-info/requires.txt
 qwertyenv.egg-info/top_level.txt
 qwertyenv.egg-info/zip-safe
 tests/__init__.py
 tests/test_collect_coins.py
 tests/test_collect_coins_gym_from_pz.py
 tests/test_collect_coins_pz.py
+tests/test_gymnasium_conversions.py
 tests/test_up_down_left_right.py
```

### Comparing `qwertyenv-0.1.0/setup.cfg` & `qwertyenv-0.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 	jupyterlab
 	matplotlib
 	stable_baselines3[extra] >= 2.0.0a5, < 2.1
 	ipywidgets
 	tianshou >= 0.5, < 0.6
 tests = 
 	pytest
+	pettingzoo[butterfly] >= 1.22.3, < 1.23
 
 [options.package_data]
 * = README.md
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `qwertyenv-0.1.0/tests/test_collect_coins.py` & `qwertyenv-0.1.1/tests/test_collect_coins.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-import gym
+import gymnasium as gym
 from qwertyenv import EnsureValidAction
 from stable_baselines3 import PPO
 from stable_baselines3.ppo.policies import MultiInputPolicy
 from stable_baselines3.common.evaluation import evaluate_policy
 
 
 def test_evaluate():
@@ -23,20 +23,21 @@
       env.provide_alternative_valid_action,
       another_action_taken
   )
   agent_w = PPO(MultiInputPolicy, env)
   for episode in range(1):
     # print(f'{episode=}')
     # print("-------")
-    obs = env.reset()
+    obs, _ = env.reset()
     # env.render()
     while True:
       action, _state = agent_w.predict(obs)
       # print(f'action predicted: {action}')
-      obs, reward, done, info = env.step(action)
+      obs, reward, terminated, truncated, info = env.step(action)
+      done = terminated or truncated
       # print(f'action taken: {action}')
       # env.render()
       # print(f'{reward=}')
       # print(f'{done=}')
       # print(f'{info=}')
       if done:
         break
```

### Comparing `qwertyenv-0.1.0/tests/test_collect_coins_gym_from_pz.py` & `qwertyenv-0.1.1/tests/test_collect_coins_gym_from_pz.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from qwertyenv.ensure_valid_action_pz import EnsureValidAction
-from qwertyenv.pz_to_gymnasium_wrapper import PZ2GymnasiumWrapper
+from qwertyenv import aec_to_gymnasium
 
 from tianshou.data import Collector
 from tianshou.env import DummyVectorEnv
 from tianshou.policy import RandomPolicy
 
 
 from qwertyenv.collect_coins_pz import CollectCoinsEnv
@@ -28,15 +28,23 @@
       env.provide_alternative_valid_action,
       another_action_taken
   )
 
   def act_agent_1(obs):
       return (0, 0)
 
-  env = PZ2GymnasiumWrapper(env, act_others={'agent_1': act_agent_1}) # Note: Gymnasium environment
+  def act_others(agent: str, obs):
+    mapping = {'player_1': act_agent_1}
+    return mapping[agent](obs)
+
+  env = aec_to_gymnasium(
+     env,
+     act_others=act_others,
+     external_agent='player_0'
+  ) # Note: Gymnasium environment
 
   check_env(env) # , num_cycles=10, verbose_progress=False)
 
 
 def test_with_tianshou():
 
   action = None
@@ -56,15 +64,23 @@
       env.provide_alternative_valid_action,
       another_action_taken
   )
 
   def act_agent_1(obs):
       return (0, 0)
 
-  env = PZ2GymnasiumWrapper(env, act_others={'agent_1': act_agent_1}) # Note: Gymnasium environment
+  def act_others(agent: str, obs):
+    mapping = {'player_1': act_agent_1}
+    return mapping[agent](obs)
+
+  env = aec_to_gymnasium(
+     env,
+     act_others=act_others,
+     external_agent='player_0'
+  ) # Note: Gymnasium environment
 
   env = DummyVectorEnv([lambda: env])
 
   policy = RandomPolicy()
 
   collector = Collector(policy, env)
```

### Comparing `qwertyenv-0.1.0/tests/test_collect_coins_pz.py` & `qwertyenv-0.1.1/tests/test_collect_coins_pz.py`

 * *Files identical despite different names*

