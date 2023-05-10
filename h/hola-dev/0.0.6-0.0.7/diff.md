# Comparing `tmp/hola-dev-0.0.6.tar.gz` & `tmp/hola-dev-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hola-dev-0.0.6.tar", last modified: Thu Apr  6 07:23:01 2023, max compression
+gzip compressed data, was "hola-dev-0.0.7.tar", last modified: Wed May 10 01:52:39 2023, max compression
```

## Comparing `hola-dev-0.0.6.tar` & `hola-dev-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:23:01.937991 hola-dev-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-06 07:22:56.000000 hola-dev-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-06 07:23:01.937991 hola-dev-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-06 07:22:56.000000 hola-dev-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:23:01.937991 hola-dev-0.0.6/hola_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-06 07:23:01.000000 hola-dev-0.0.6/hola_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-06 07:23:01.000000 hola-dev-0.0.6/hola_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 07:23:01.000000 hola-dev-0.0.6/hola_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-06 07:23:01.000000 hola-dev-0.0.6/hola_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-06 07:23:01.000000 hola-dev-0.0.6/hola_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-06 07:23:01.000000 hola-dev-0.0.6/hola_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 07:23:01.937991 hola-dev-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-06 07:22:56.000000 hola-dev-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:23:01.937991 hola-dev-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:22:56.000000 hola-dev-0.0.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-06 07:22:56.000000 hola-dev-0.0.6/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-06 07:22:56.000000 hola-dev-0.0.6/src/index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:23:01.937991 hola-dev-0.0.6/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:22:56.000000 hola-dev-0.0.6/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-06 07:22:56.000000 hola-dev-0.0.6/src/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:52:39.255396 hola-dev-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-10 01:52:34.000000 hola-dev-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-10 01:52:39.255396 hola-dev-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 01:52:34.000000 hola-dev-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:52:39.255396 hola-dev-0.0.7/hola_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-10 01:52:39.000000 hola-dev-0.0.7/hola_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-10 01:52:39.000000 hola-dev-0.0.7/hola_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 01:52:39.000000 hola-dev-0.0.7/hola_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 01:52:39.000000 hola-dev-0.0.7/hola_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 01:52:39.000000 hola-dev-0.0.7/hola_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 01:52:39.000000 hola-dev-0.0.7/hola_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 01:52:39.255396 hola-dev-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-10 01:52:34.000000 hola-dev-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:52:39.255396 hola-dev-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 01:52:34.000000 hola-dev-0.0.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 01:52:34.000000 hola-dev-0.0.7/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-05-10 01:52:34.000000 hola-dev-0.0.7/src/index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 01:52:39.255396 hola-dev-0.0.7/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 01:52:34.000000 hola-dev-0.0.7/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 01:52:34.000000 hola-dev-0.0.7/src/utils/util.py
```

### Comparing `hola-dev-0.0.6/LICENSE` & `hola-dev-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hola-dev-0.0.6/setup.py` & `hola-dev-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hola-dev",
-    version="0.0.6",
+    version="0.0.7",
     author="JunBeum Cho",
     author_email="ahengksk@gmail.com",
     description="Common packages installer on MAC",
     url = 'https://github.com/JunBeum-Cho/hola-dev',
     download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',
     entry_points={"console_scripts": ["hola-dev=src.__main__:main"]},
     keywords = ['mac', 'package installers'],
```

### Comparing `hola-dev-0.0.6/src/index.py` & `hola-dev-0.0.7/src/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
 def main():
     try:
         set_secret_manager_env()
         print(chalk.green.bold("env 로드 성공"))
     except:
         print(chalk.red.bold("env 로드 실패"))
-        return
 
     if platform.system() != 'Darwin':
         print('해당 CLI는 MAC에서만 작동합니다.')
         return
 
     if os.system('which brew') != 0:
         os.system('/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"')
```

