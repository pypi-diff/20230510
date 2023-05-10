# Comparing `tmp/rover_arm-1.1.7.tar.gz` & `tmp/rover_arm-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rover_arm-1.1.7.tar", last modified: Wed May 10 00:05:04 2023, max compression
+gzip compressed data, was "rover_arm-1.1.8.tar", last modified: Wed May 10 01:48:19 2023, max compression
```

## Comparing `rover_arm-1.1.7.tar` & `rover_arm-1.1.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.830580 rover_arm-1.1.7/
--rw-r--r--   0 saiphani724   (501) staff       (20)    10244 2023-05-08 00:27:00.000000 rover_arm-1.1.7/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-05-08 00:22:59.000000 rover_arm-1.1.7/.gitignore
--rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.1.7/MANIFEST.in
--rw-r--r--   0 saiphani724   (501) staff       (20)     2620 2023-05-10 00:05:04.830430 rover_arm-1.1.7/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     2442 2023-05-08 00:21:36.000000 rover_arm-1.1.7/README.md
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.801346 rover_arm-1.1.7/rover_arm/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-05-03 22:23:09.000000 rover_arm-1.1.7/rover_arm/.DS_Store
--rw-r--r--   0 saiphani724   (501) staff       (20)      388 2023-05-04 06:40:53.000000 rover_arm-1.1.7/rover_arm/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.802905 rover_arm-1.1.7/rover_arm/data/
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.803469 rover_arm-1.1.7/rover_arm/data/meshes/
--rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/.DS_Store
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.807410 rover_arm-1.1.7/rover_arm/data/meshes/collision/
--rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link0.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/collision/link7.obj
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.824213 rover_arm-1.1.7/rover_arm/data/meshes/visual/
--rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/colors.png
--rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/finger.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/finger.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/hand.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/hand.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link1.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link1.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link2.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link2.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link3.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link3.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link4.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link4.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link5.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link5.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link6.mtl
--rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/meshes/visual/link6.obj
--rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/panda.urdf
--rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.1.7/rover_arm/data/rover_arm.xml
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.827262 rover_arm-1.1.7/rover_arm/envs/
--rw-r--r--   0 saiphani724   (501) staff       (20)      302 2023-05-04 06:31:51.000000 rover_arm-1.1.7/rover_arm/envs/__init__.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.828728 rover_arm-1.1.7/rover_arm/envs/__pycache__/
--rw-r--r--   0 saiphani724   (501) staff       (20)      374 2023-05-06 20:45:05.000000 rover_arm-1.1.7/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)     7490 2023-05-06 22:09:38.000000 rover_arm-1.1.7/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
--rw-r--r--   0 saiphani724   (501) staff       (20)    11807 2023-05-06 22:08:52.000000 rover_arm-1.1.7/rover_arm/envs/roverarm_env.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.1.7/rover_arm/envs/roverarm_env_arrange.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    11785 2023-05-10 00:03:45.000000 rover_arm-1.1.7/rover_arm/envs/roverarm_env_gym.py
--rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.1.7/rover_arm/envs/roverarm_env_place.py
--rw-r--r--   0 saiphani724   (501) staff       (20)     2366 2023-04-27 20:10:52.000000 rover_arm-1.1.7/rover_arm/keyboard_control.py
-drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 00:05:04.802249 rover_arm-1.1.7/rover_arm.egg-info/
--rw-r--r--   0 saiphani724   (501) staff       (20)     2620 2023-05-10 00:05:04.000000 rover_arm-1.1.7/rover_arm.egg-info/PKG-INFO
--rw-r--r--   0 saiphani724   (501) staff       (20)     1775 2023-05-10 00:05:04.000000 rover_arm-1.1.7/rover_arm.egg-info/SOURCES.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-05-10 00:05:04.000000 rover_arm-1.1.7/rover_arm.egg-info/dependency_links.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       37 2023-05-10 00:05:04.000000 rover_arm-1.1.7/rover_arm.egg-info/requires.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-05-10 00:05:04.000000 rover_arm-1.1.7/rover_arm.egg-info/top_level.txt
--rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-05-10 00:05:04.830632 rover_arm-1.1.7/setup.cfg
--rw-r--r--   0 saiphani724   (501) staff       (20)      583 2023-05-10 00:05:02.000000 rover_arm-1.1.7/setup.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.613501 rover_arm-1.1.8/
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10244 2023-05-08 00:27:00.000000 rover_arm-1.1.8/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      304 2023-05-08 00:22:59.000000 rover_arm-1.1.8/.gitignore
+-rw-r--r--   0 saiphani724   (501) staff       (20)       35 2023-03-29 21:25:47.000000 rover_arm-1.1.8/MANIFEST.in
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2620 2023-05-10 01:48:19.613371 rover_arm-1.1.8/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2442 2023-05-08 00:21:36.000000 rover_arm-1.1.8/README.md
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.602135 rover_arm-1.1.8/rover_arm/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-05-03 22:23:09.000000 rover_arm-1.1.8/rover_arm/.DS_Store
+-rw-r--r--   0 saiphani724   (501) staff       (20)      388 2023-05-04 06:40:53.000000 rover_arm-1.1.8/rover_arm/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.603177 rover_arm-1.1.8/rover_arm/data/
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.603355 rover_arm-1.1.8/rover_arm/data/meshes/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     6148 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/.DS_Store
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.605213 rover_arm-1.1.8/rover_arm/data/meshes/collision/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7603 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    15247 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    14925 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link0.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22976 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22688 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    22870 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    68016 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    67745 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3827 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   140218 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    45132 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/collision/link7.obj
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.611220 rover_arm-1.1.8/rover_arm/data/meshes/visual/
+-rw-r--r--   0 saiphani724   (501) staff       (20)    33337 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/colors.png
+-rw-r--r--   0 saiphani724   (501) staff       (20)      481 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/finger.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)    65359 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/finger.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1132 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/hand.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)   713204 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/hand.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      262 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link1.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1070650 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link1.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      261 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link2.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1084458 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link2.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      931 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link3.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1237175 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link3.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      925 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link4.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1272305 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link4.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)      676 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link5.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  1582192 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link5.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)     3552 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link6.mtl
+-rw-r--r--   0 saiphani724   (501) staff       (20)  2236857 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/meshes/visual/link6.obj
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11263 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/panda.urdf
+-rw-r--r--   0 saiphani724   (501) staff       (20)    17075 2023-03-25 23:52:17.000000 rover_arm-1.1.8/rover_arm/data/rover_arm.xml
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.612913 rover_arm-1.1.8/rover_arm/envs/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      302 2023-05-04 06:31:51.000000 rover_arm-1.1.8/rover_arm/envs/__init__.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.613162 rover_arm-1.1.8/rover_arm/envs/__pycache__/
+-rw-r--r--   0 saiphani724   (501) staff       (20)      374 2023-05-06 20:45:05.000000 rover_arm-1.1.8/rover_arm/envs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)     7490 2023-05-06 22:09:38.000000 rover_arm-1.1.8/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11807 2023-05-06 22:08:52.000000 rover_arm-1.1.8/rover_arm/envs/roverarm_env.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    10141 2023-03-30 20:15:25.000000 rover_arm-1.1.8/rover_arm/envs/roverarm_env_arrange.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11859 2023-05-10 01:44:28.000000 rover_arm-1.1.8/rover_arm/envs/roverarm_env_gym.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)    11763 2023-04-27 19:26:02.000000 rover_arm-1.1.8/rover_arm/envs/roverarm_env_place.py
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2366 2023-04-27 20:10:52.000000 rover_arm-1.1.8/rover_arm/keyboard_control.py
+drwxr-xr-x   0 saiphani724   (501) staff       (20)        0 2023-05-10 01:48:19.602844 rover_arm-1.1.8/rover_arm.egg-info/
+-rw-r--r--   0 saiphani724   (501) staff       (20)     2620 2023-05-10 01:48:19.000000 rover_arm-1.1.8/rover_arm.egg-info/PKG-INFO
+-rw-r--r--   0 saiphani724   (501) staff       (20)     1775 2023-05-10 01:48:19.000000 rover_arm-1.1.8/rover_arm.egg-info/SOURCES.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)        1 2023-05-10 01:48:19.000000 rover_arm-1.1.8/rover_arm.egg-info/dependency_links.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       37 2023-05-10 01:48:19.000000 rover_arm-1.1.8/rover_arm.egg-info/requires.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       10 2023-05-10 01:48:19.000000 rover_arm-1.1.8/rover_arm.egg-info/top_level.txt
+-rw-r--r--   0 saiphani724   (501) staff       (20)       38 2023-05-10 01:48:19.613549 rover_arm-1.1.8/setup.cfg
+-rw-r--r--   0 saiphani724   (501) staff       (20)      583 2023-05-10 01:48:17.000000 rover_arm-1.1.8/setup.py
```

### Comparing `rover_arm-1.1.7/.DS_Store` & `rover_arm-1.1.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/PKG-INFO` & `rover_arm-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rover_arm
-Version: 1.1.7
+Version: 1.1.8
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.1.7/README.md` & `rover_arm-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/.DS_Store` & `rover_arm-1.1.8/rover_arm/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/.DS_Store` & `rover_arm-1.1.8/rover_arm/data/meshes/.DS_Store`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/finger.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/hand.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link0.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link0.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link1.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link2.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link3.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link4.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link5.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link6.mtl` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link6.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/collision/link7.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/collision/link7.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/colors.png` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/colors.png`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/finger.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/finger.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/hand.mtl` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/hand.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/hand.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/hand.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link1.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link1.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link2.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link2.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link3.mtl` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link3.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link3.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link3.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link4.mtl` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link4.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link4.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link4.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link5.mtl` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link5.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link5.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link5.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link6.mtl` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link6.mtl`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/meshes/visual/link6.obj` & `rover_arm-1.1.8/rover_arm/data/meshes/visual/link6.obj`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/panda.urdf` & `rover_arm-1.1.8/rover_arm/data/panda.urdf`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/data/rover_arm.xml` & `rover_arm-1.1.8/rover_arm/data/rover_arm.xml`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc` & `rover_arm-1.1.8/rover_arm/envs/__pycache__/roverarm_env.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/envs/roverarm_env.py` & `rover_arm-1.1.8/rover_arm/envs/roverarm_env.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/envs/roverarm_env_arrange.py` & `rover_arm-1.1.8/rover_arm/envs/roverarm_env_arrange.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/envs/roverarm_env_gym.py` & `rover_arm-1.1.8/rover_arm/envs/roverarm_env_gym.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,24 +204,26 @@
 
         self.observation = state_rover + state_arm + state_fingers + tuple(state_object)
         info = {'state_rover_pos': pos, 'state_rover_ang' : ang, 'state_rover_vel' : vel ,'state_arm' : state_arm, 'state_fingers': state_fingers, 'state_object': state_object}
 
         return np.array(self.observation).astype(np.float32), reward, terminated, truncated, info
 
 
-    def render(self, width = None, height = None):
+    def render(self, mode = None, width = None, height = None):
         # cam = p.getDebugVisualizerCamera()
         # xyz = cam[11]
         # x= float(xyz[0]) + 0.125
         # y = xyz[1]
         # z = xyz[2]
         # p.resetDebugVisualizerCamera(cameraYaw = cam[8], cameraPitch= cam[9],cameraDistance = cam[10],cameraTargetPosition=[x,y,z])
         if width == None or height == None:
             width = self._width
             height = self._height
+        if mode != None:
+            self.render_mode = mode
         if self.render_mode != 'rgb_array':
             return None
         view_matrix1 = p.computeViewMatrixFromYawPitchRoll(cameraTargetPosition=self._cam_target_p,
                                                             distance=self._cam_dist,
                                                             yaw=self._cam_yaw,
                                                             pitch=self._cam_pitch,
                                                             roll=0,
```

### Comparing `rover_arm-1.1.7/rover_arm/envs/roverarm_env_place.py` & `rover_arm-1.1.8/rover_arm/envs/roverarm_env_place.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm/keyboard_control.py` & `rover_arm-1.1.8/rover_arm/keyboard_control.py`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/rover_arm.egg-info/PKG-INFO` & `rover_arm-1.1.8/rover_arm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rover-arm
-Version: 1.1.7
+Version: 1.1.8
 Summary: A OpenAI Gym Env for Rover with Arm
 Author: Sai Phani
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 A OpenAI Gym Env for Rover with Arm
```

### Comparing `rover_arm-1.1.7/rover_arm.egg-info/SOURCES.txt` & `rover_arm-1.1.8/rover_arm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rover_arm-1.1.7/setup.py` & `rover_arm-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 from pathlib import Path
 
 setuptools.setup(
     name='rover_arm',
-    version='1.1.7',
+    version='1.1.8',
     description="A OpenAI Gym Env for Rover with Arm",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     author="Sai Phani",
     packages = setuptools.find_packages(include="rover_arm*"),
     package_data={'data' :['rover_arm/data/*']},
     include_package_data=True,
```

