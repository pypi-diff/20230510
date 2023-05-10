# Comparing `tmp/qwertyenv-0.0.2.tar.gz` & `tmp/qwertyenv-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwertyenv-0.0.2.tar", last modified: Tue Feb  7 12:47:31 2023, max compression
+gzip compressed data, was "qwertyenv-0.1.0.tar", last modified: Wed May 10 08:23:14 2023, max compression
```

## Comparing `qwertyenv-0.0.2.tar` & `qwertyenv-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-02-07 12:47:31.140000 qwertyenv-0.0.2/
--rw-r--r--   0 oren      (1000) oren      (1000)     1313 2023-02-07 12:47:31.140000 qwertyenv-0.0.2/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)      418 2023-02-07 12:21:40.000000 qwertyenv-0.0.2/README.md
--rw-r--r--   0 oren      (1000) oren      (1000)      103 2022-12-24 16:37:54.000000 qwertyenv-0.0.2/pyproject.toml
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-02-07 12:47:31.130000 qwertyenv-0.0.2/qwertyenv/
--rw-r--r--   0 oren      (1000) oren      (1000)      475 2023-02-07 12:11:03.000000 qwertyenv-0.0.2/qwertyenv/__init__.py
--rw-r--r--   0 oren      (1000) oren      (1000)     3785 2023-02-05 19:57:46.000000 qwertyenv-0.0.2/qwertyenv/black_jack.py
--rw-r--r--   0 oren      (1000) oren      (1000)     6517 2023-02-07 12:06:51.000000 qwertyenv-0.0.2/qwertyenv/collect_coins.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1252 2023-02-07 11:56:42.000000 qwertyenv-0.0.2/qwertyenv/ensure_valid_action.py
--rw-r--r--   0 oren      (1000) oren      (1000)      836 2023-02-07 12:35:34.000000 qwertyenv-0.0.2/qwertyenv/up_down_left_right.py
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-02-07 12:47:31.140000 qwertyenv-0.0.2/qwertyenv.egg-info/
--rw-r--r--   0 oren      (1000) oren      (1000)     1313 2023-02-07 12:47:31.000000 qwertyenv-0.0.2/qwertyenv.egg-info/PKG-INFO
--rw-r--r--   0 oren      (1000) oren      (1000)      443 2023-02-07 12:47:31.000000 qwertyenv-0.0.2/qwertyenv.egg-info/SOURCES.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-02-07 12:47:31.000000 qwertyenv-0.0.2/qwertyenv.egg-info/dependency_links.txt
--rw-r--r--   0 oren      (1000) oren      (1000)      105 2023-02-07 12:47:31.000000 qwertyenv-0.0.2/qwertyenv.egg-info/requires.txt
--rw-r--r--   0 oren      (1000) oren      (1000)       16 2023-02-07 12:47:31.000000 qwertyenv-0.0.2/qwertyenv.egg-info/top_level.txt
--rw-r--r--   0 oren      (1000) oren      (1000)        1 2022-12-24 17:15:22.000000 qwertyenv-0.0.2/qwertyenv.egg-info/zip-safe
--rw-r--r--   0 oren      (1000) oren      (1000)     1209 2023-02-07 12:47:31.140000 qwertyenv-0.0.2/setup.cfg
-drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-02-07 12:47:31.140000 qwertyenv-0.0.2/tests/
--rw-r--r--   0 oren      (1000) oren      (1000)        0 2023-02-02 11:54:46.000000 qwertyenv-0.0.2/tests/__init__.py
--rw-r--r--   0 oren      (1000) oren      (1000)     1228 2023-02-07 09:17:40.000000 qwertyenv-0.0.2/tests/test_collect_coins.py
--rw-r--r--   0 oren      (1000) oren      (1000)      347 2023-02-07 12:30:45.000000 qwertyenv-0.0.2/tests/test_up_down_left_right.py
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/
+-rw-r--r--   0 oren      (1000) oren      (1000)     1356 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)      420 2023-02-07 12:50:27.000000 qwertyenv-0.1.0/README.md
+-rw-r--r--   0 oren      (1000) oren      (1000)      103 2022-12-24 16:37:54.000000 qwertyenv-0.1.0/pyproject.toml
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/qwertyenv/
+-rw-r--r--   0 oren      (1000) oren      (1000)      481 2023-05-10 08:21:08.000000 qwertyenv-0.1.0/qwertyenv/__init__.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      689 2023-03-15 14:32:09.000000 qwertyenv-0.1.0/qwertyenv/action_wrapper_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     3826 2023-05-10 07:34:14.000000 qwertyenv-0.1.0/qwertyenv/black_jack.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     3372 2023-05-10 07:44:21.000000 qwertyenv-0.1.0/qwertyenv/collect_coins.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     3230 2023-03-02 16:43:27.000000 qwertyenv-0.1.0/qwertyenv/collect_coins_game.py
+-rw-r--r--   0 oren      (1000) oren      (1000)    10008 2023-03-15 16:58:08.000000 qwertyenv-0.1.0/qwertyenv/collect_coins_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1265 2023-05-10 07:20:30.000000 qwertyenv-0.1.0/qwertyenv/ensure_valid_action.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1309 2023-03-13 11:27:57.000000 qwertyenv-0.1.0/qwertyenv/ensure_valid_action_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     2417 2023-05-10 08:21:49.000000 qwertyenv-0.1.0/qwertyenv/pz_to_gymnasium_wrapper.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1601 2023-03-15 16:43:32.000000 qwertyenv-0.1.0/qwertyenv/tmp.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      850 2023-05-10 07:20:58.000000 qwertyenv-0.1.0/qwertyenv/up_down_left_right.py
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/qwertyenv.egg-info/
+-rw-r--r--   0 oren      (1000) oren      (1000)     1356 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/PKG-INFO
+-rw-r--r--   0 oren      (1000) oren      (1000)      697 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/SOURCES.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/dependency_links.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)      168 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/requires.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)       16 2023-05-10 08:23:14.000000 qwertyenv-0.1.0/qwertyenv.egg-info/top_level.txt
+-rw-r--r--   0 oren      (1000) oren      (1000)        1 2022-12-24 17:15:22.000000 qwertyenv-0.1.0/qwertyenv.egg-info/zip-safe
+-rw-r--r--   0 oren      (1000) oren      (1000)     1257 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/setup.cfg
+drwxr-xr-x   0 oren      (1000) oren      (1000)        0 2023-05-10 08:23:14.068191 qwertyenv-0.1.0/tests/
+-rw-r--r--   0 oren      (1000) oren      (1000)        0 2023-02-02 11:54:46.000000 qwertyenv-0.1.0/tests/__init__.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1228 2023-02-07 09:17:40.000000 qwertyenv-0.1.0/tests/test_collect_coins.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1925 2023-03-13 14:20:33.000000 qwertyenv-0.1.0/tests/test_collect_coins_gym_from_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)     1550 2023-03-14 14:27:41.000000 qwertyenv-0.1.0/tests/test_collect_coins_pz.py
+-rw-r--r--   0 oren      (1000) oren      (1000)      347 2023-02-07 12:30:45.000000 qwertyenv-0.1.0/tests/test_up_down_left_right.py
```

### Comparing `qwertyenv-0.0.2/PKG-INFO` & `qwertyenv-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qwertyenv
-Version: 0.0.2
-Summary: Gym environments (Reinforcement Learning)
+Version: 0.1.0
+Summary: Gym and PettingZoo environments (Reinforcement Learning)
 Home-page: https://github.com/zbenmo/qwertyenv
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 License: BSD 3-Clause License
-Keywords: Gym,Gym environments,Black Jack,Collect Coins (Chesss like),Reinforcement Learning,Gym Wrappers
+Keywords: Gym,Gym environments,Black Jack,Collect Coins (Chesss like),Reinforcement Learning,Gym Wrappers,PettingZoo,MARL,Gymnasium
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,17 @@
 Provides-Extra: examples
 Provides-Extra: tests
 
 # qwertyenv
 Gym environments (Reinforcement Learning)
 
 Black Jack (from RLBook2018)
+
 Collect Coins (Chess like)
 
 "Ensure Valid Action" Gym wrapper.
+
 "Up/Down/Left/Right" Gym wrapper - relevant for example for the Collect Coins environment when the piece is a rock.
 
 > pip install qwertyenv
 
 Example usages for the Black Jack environment and for the Collect Coins environment can be found on github (the project's home).
```

### Comparing `qwertyenv-0.0.2/qwertyenv/black_jack.py` & `qwertyenv-0.1.0/qwertyenv/black_jack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 import random
 
 
 class BJEnv(gym.Env):
     """
     Blackjack
     """
@@ -60,16 +60,17 @@
         obs_space = dict(
             player_sum = gym.spaces.Discrete(11), # x -> x + 11
             player_useful_Ace = gym.spaces.Discrete(2), # 0 no, 1 yes
             dealer_shown_card = gym.spaces.Discrete(10) # 0 - Ace, x -> x + 1 (ex. 1 is 2, 9 is 10)
         )
         
         self.observation_space = gym.spaces.Dict(obs_space)
+        self.render_mode = None
         self.reset()
-    def render(self, mode: str):
+    def render(self):
         self.state.render()
     def reset(self, seed=None, options=None):
         if seed:
           random.seed(seed)
         self.state = BJEnv.State()
         return self._state_to_obs(), {}
     def _state_to_obs(self):
@@ -100,8 +101,8 @@
             reward = 0
             info['new card'] = self.state.card_to_image(new_card)
             if self.state.player_sum > 21:
                 reward = -1
                 done = True
         else:
             assert False, f"unkown action {action}"
-        return self._state_to_obs(), reward, done, info
+        return self._state_to_obs(), reward, done, False, info
```

### Comparing `qwertyenv-0.0.2/qwertyenv/ensure_valid_action.py` & `qwertyenv-0.1.0/qwertyenv/ensure_valid_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import TypeVar, Callable
-import gym
+import gymnasium as gym
 
 
 Action = TypeVar("Action")
 
 
 class EnsureValidAction(gym.ActionWrapper):
   """
```

### Comparing `qwertyenv-0.0.2/qwertyenv/up_down_left_right.py` & `qwertyenv-0.1.0/qwertyenv/up_down_left_right.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import gym
+import gymnasium as gym
 from typing import Tuple, Callable
 import numpy as np
 
 
 class UpDownLeftRight(gym.ActionWrapper):
   """
   A gym environment wrapper to enable U/D/L/R action space when the wrapped environment
   actually expects a destination in cartesian coordinates.
   """
+
   def __init__(self, env: gym.Env,
                get_current_location: Callable[[], Tuple[int, int]]):
 
     super().__init__(env)
     self.get_current_location = get_current_location
 
     self.action_space = gym.spaces.Discrete(4)
```

### Comparing `qwertyenv-0.0.2/qwertyenv.egg-info/PKG-INFO` & `qwertyenv-0.1.0/qwertyenv.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: qwertyenv
-Version: 0.0.2
-Summary: Gym environments (Reinforcement Learning)
+Version: 0.1.0
+Summary: Gym and PettingZoo environments (Reinforcement Learning)
 Home-page: https://github.com/zbenmo/qwertyenv
 Author: Oren Zeev-Ben-Mordehai
 Author-email: zbenmo@gmail.com
 License: BSD 3-Clause License
-Keywords: Gym,Gym environments,Black Jack,Collect Coins (Chesss like),Reinforcement Learning,Gym Wrappers
+Keywords: Gym,Gym environments,Black Jack,Collect Coins (Chesss like),Reinforcement Learning,Gym Wrappers,PettingZoo,MARL,Gymnasium
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,17 @@
 Provides-Extra: examples
 Provides-Extra: tests
 
 # qwertyenv
 Gym environments (Reinforcement Learning)
 
 Black Jack (from RLBook2018)
+
 Collect Coins (Chess like)
 
 "Ensure Valid Action" Gym wrapper.
+
 "Up/Down/Left/Right" Gym wrapper - relevant for example for the Collect Coins environment when the piece is a rock.
 
 > pip install qwertyenv
 
 Example usages for the Black Jack environment and for the Collect Coins environment can be found on github (the project's home).
```

### Comparing `qwertyenv-0.0.2/setup.cfg` & `qwertyenv-0.1.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = qwertyenv
 version = attr: qwertyenv.__version__
 author = Oren Zeev-Ben-Mordehai
 author_email = zbenmo@gmail.com
 url = https://github.com/zbenmo/qwertyenv
-description = Gym environments (Reinforcement Learning)
+description = Gym and PettingZoo environments (Reinforcement Learning)
 long_description = file: README.md
 long_description_content_type = text/markdown
-keywords = Gym, Gym environments, Black Jack, Collect Coins (Chesss like), Reinforcement Learning, Gym Wrappers
+keywords = Gym, Gym environments, Black Jack, Collect Coins (Chesss like), Reinforcement Learning, Gym Wrappers, PettingZoo, MARL, Gymnasium
 license = BSD 3-Clause License
 classifiers = 
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
@@ -21,22 +21,24 @@
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 
 [options]
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
-	gym >= 0.21.0, <= 0.22
+	gymnasium >= 0.28.1, < 0.29
+	pettingzoo >= 1.22.3, < 1.23
 
 [options.extras_require]
 examples = 
 	jupyterlab
 	matplotlib
-	stable_baselines3[extra]
-	ipywidgets # todo: jupyter labextension install @jupyter-widgets/jupyterlab-manager
+	stable_baselines3[extra] >= 2.0.0a5, < 2.1
+	ipywidgets
+	tianshou >= 0.5, < 0.6
 tests = 
 	pytest
 
 [options.package_data]
 * = README.md
 
 [egg_info]
```

### Comparing `qwertyenv-0.0.2/tests/test_collect_coins.py` & `qwertyenv-0.1.0/tests/test_collect_coins.py`

 * *Files identical despite different names*

