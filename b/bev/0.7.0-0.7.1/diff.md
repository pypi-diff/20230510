# Comparing `tmp/bev-0.7.0.tar.gz` & `tmp/bev-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bev-0.7.0.tar", last modified: Sun Apr  9 19:35:45 2023, max compression
+gzip compressed data, was "bev-0.7.1.tar", last modified: Wed May 10 13:20:05 2023, max compression
```

## Comparing `bev-0.7.0.tar` & `bev-0.7.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.350534 bev-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-04-09 19:35:41.000000 bev-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-09 19:35:41.000000 bev-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-09 19:35:45.350534 bev-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-09 19:35:41.000000 bev-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.346534 bev-0.7.0/bev/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-09 19:35:41.000000 bev-0.7.0/bev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 19:35:41.000000 bev-0.7.0/bev/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.350534 bev-0.7.0/bev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/blame.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-09 19:35:41.000000 bev-0.7.0/bev/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.350534 bev-0.7.0/bev/config/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/hostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-09 19:35:41.000000 bev-0.7.0/bev/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-09 19:35:41.000000 bev-0.7.0/bev/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-09 19:35:41.000000 bev-0.7.0/bev/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 19:35:41.000000 bev-0.7.0/bev/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 19:35:41.000000 bev-0.7.0/bev/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-09 19:35:41.000000 bev-0.7.0/bev/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:41.000000 bev-0.7.0/bev/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-04-09 19:35:41.000000 bev-0.7.0/bev/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:41.000000 bev-0.7.0/bev/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-09 19:35:41.000000 bev-0.7.0/bev/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-09 19:35:41.000000 bev-0.7.0/bev/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-09 19:35:41.000000 bev-0.7.0/bev/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-09 19:35:41.000000 bev-0.7.0/bev/vc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-04-09 19:35:41.000000 bev-0.7.0/bev/wc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:45.350534 bev-0.7.0/bev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-09 19:35:45.000000 bev-0.7.0/bev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-09 19:35:41.000000 bev-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 19:35:41.000000 bev-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:35:45.350534 bev-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-09 19:35:41.000000 bev-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.399525 bev-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-05-10 13:20:03.000000 bev-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 13:20:03.000000 bev-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-10 13:20:05.395525 bev-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-10 13:20:03.000000 bev-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.395525 bev-0.7.1/bev/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-10 13:20:03.000000 bev-0.7.1/bev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 13:20:03.000000 bev-0.7.1/bev/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.395525 bev-0.7.1/bev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/blame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-10 13:20:03.000000 bev-0.7.1/bev/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.395525 bev-0.7.1/bev/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-10 13:20:03.000000 bev-0.7.1/bev/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-10 13:20:03.000000 bev-0.7.1/bev/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-10 13:20:03.000000 bev-0.7.1/bev/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-10 13:20:03.000000 bev-0.7.1/bev/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-10 13:20:03.000000 bev-0.7.1/bev/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-10 13:20:03.000000 bev-0.7.1/bev/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-10 13:20:03.000000 bev-0.7.1/bev/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-10 13:20:03.000000 bev-0.7.1/bev/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:03.000000 bev-0.7.1/bev/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-10 13:20:03.000000 bev-0.7.1/bev/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-10 13:20:03.000000 bev-0.7.1/bev/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-10 13:20:03.000000 bev-0.7.1/bev/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-10 13:20:03.000000 bev-0.7.1/bev/vc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-10 13:20:03.000000 bev-0.7.1/bev/wc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:05.395525 bev-0.7.1/bev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 13:20:05.000000 bev-0.7.1/bev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-10 13:20:03.000000 bev-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 13:20:03.000000 bev-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:20:05.399525 bev-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-10 13:20:03.000000 bev-0.7.1/setup.py
```

### Comparing `bev-0.7.0/LICENSE` & `bev-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/PKG-INFO` & `bev-0.7.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.7.0
+Version: 0.7.1
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
 License: MIT
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.7.0.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.7.1.tar.gz
 Keywords: data,version control
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -33,23 +33,66 @@
 
 The simplest way is to get it from PyPi:
 
 ```shell
 pip install bev
 ```
 
-Or if you want to try the latest version from GitHub:
+# Cheatsheet
+
+### Adding new files
+
+```shell
+ls
+# image.png ids.json some-folder
+bev add image.png
+ls
+# image.png.hash ids.json some-folder
+bev add ids.json some-folder
+ls
+# image.png.hash ids.json.hash some-folder.hash
+
+git add image.png.hash ids.json.hash some-folder.hash
+git commit -m "added new files"
+```
+
+### Restoring the hashed files and folders
+
+```shell
+ls
+# image.png.hash ids.json.hash some-folder.hash
+bev pull image.png.hash --mode copy
+ls
+# image.png ids.json.hash some-folder.hash
+bev pull some-folder.hash --mode copy
+ls
+# image.png ids.json.hash some-folder
+```
+
+### Browsing a hashed folder
+
+In this recipe we "expand" the hashed folder and fill it with the hashes of the files it contains.
+This is much faster than copying back the entire folder.
 
 ```shell
-git clone https://github.com/neuro-ml/bev.git
-cd bev
-pip install -e .
+ls
+# image.png.hash ids.json.hash some-folder.hash
+bev pull some-folder.hash --mode hash
+ls
+# image.png.hash ids.json.hash some-folder
+ls some-folder
+# photo.jpg.hash some-text-file.txt.hash nested-folder
+```
 
-# or let pip handle the cloning:
-pip install git+https://github.com/neuro-ml/bev.git
+Afterwards you can add the folder back
+
+```shell
+bev add some-folder
+ls
+# image.png.hash ids.json.hash some-folder.hash
 ```
 
 # Getting started
 
 1. Choose a folder for your repository and create a basic config (`.bev.yml`):
 
 ```yaml
@@ -65,17 +108,17 @@
 ```shell
 bev init
 ```
 
 3. Add files to bev
 
 ```shell
-bev add /path/to/some/file.json .
-bev add /path/to/some/folder/ .
-bev add /path/to/some/image.png .
+bev add /path/to/some/file.json
+# also can provide several paths
+bev add /path/to/some/folder/ /path/to/some/image.png
 ```
 
 4. ... and to git
 
 ```shell
 git add file.json.hash folder.hash image.png.hash
 git commit -m "added files"
@@ -88,14 +131,25 @@
 from bev import Repository
 
 # `version` can be a commit hash or a git tag 
 repo = Repository('/path/to/repo', version='8a7fe6')
 image = imageio.imread(repo.resolve('image.png'))
 ```
 
+6. Or from cli
+
+```shell
+# replace the folder's hash by the hashes of its files
+bev pull folder.hash --mode hash
+# entirely restore the folder (inverse of `bev add folder`)
+bev pull folder.hash --mode copy
+# same for files
+bev pull image.png.hash --mode copy
+```
+
 ### Advanced usage
 
 Here are some tutorials that cover more advanced configuration, including multiple storage locations and machines:
 
 1. [Create a repository](https://github.com/neuro-ml/bev/wiki/Creating-a-repository) - needed only at first time setup
 2. [Adding files](https://github.com/neuro-ml/bev/wiki/Adding-files)
 3. [Accessing files](https://github.com/neuro-ml/bev/wiki/Accessing-the-stored-files)
```

### Comparing `bev-0.7.0/bev/cli/add.py` & `bev-0.7.1/bev/cli/add.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/cli/app.py` & `bev-0.7.1/bev/cli/app.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/cli/blame.py` & `bev-0.7.1/bev/cli/blame.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/cli/fetch.py` & `bev-0.7.1/bev/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/cli/init.py` & `bev-0.7.1/bev/cli/init.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/cli/pull.py` & `bev-0.7.1/bev/cli/pull.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/cli/storage.py` & `bev-0.7.1/bev/cli/storage.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/cli/update.py` & `bev-0.7.1/bev/cli/update.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/cli/utils.py` & `bev-0.7.1/bev/cli/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/config/base.py` & `bev-0.7.1/bev/config/base.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/config/hostname.py` & `bev-0.7.1/bev/config/hostname.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/config/include.py` & `bev-0.7.1/bev/config/include.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/config/parse.py` & `bev-0.7.1/bev/config/parse.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/config/registry.py` & `bev-0.7.1/bev/config/registry.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/config/remote.py` & `bev-0.7.1/bev/config/remote.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/config/utils.py` & `bev-0.7.1/bev/config/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/hash.py` & `bev-0.7.1/bev/hash.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/interface.py` & `bev-0.7.1/bev/interface.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/ops.py` & `bev-0.7.1/bev/ops.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/shortcuts.py` & `bev-0.7.1/bev/shortcuts.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/testing.py` & `bev-0.7.1/bev/testing.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/utils.py` & `bev-0.7.1/bev/utils.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/vc.py` & `bev-0.7.1/bev/vc.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev/wc.py` & `bev-0.7.1/bev/wc.py`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/bev.egg-info/PKG-INFO` & `bev-0.7.1/bev.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bev
-Version: 0.7.0
+Version: 0.7.1
 Summary: A small manager for versioned data
 Home-page: https://github.com/neuro-ml/bev
 License: MIT
-Download-URL: https://github.com/neuro-ml/bev/archive/v0.7.0.tar.gz
+Download-URL: https://github.com/neuro-ml/bev/archive/v0.7.1.tar.gz
 Keywords: data,version control
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -33,23 +33,66 @@
 
 The simplest way is to get it from PyPi:
 
 ```shell
 pip install bev
 ```
 
-Or if you want to try the latest version from GitHub:
+# Cheatsheet
+
+### Adding new files
+
+```shell
+ls
+# image.png ids.json some-folder
+bev add image.png
+ls
+# image.png.hash ids.json some-folder
+bev add ids.json some-folder
+ls
+# image.png.hash ids.json.hash some-folder.hash
+
+git add image.png.hash ids.json.hash some-folder.hash
+git commit -m "added new files"
+```
+
+### Restoring the hashed files and folders
+
+```shell
+ls
+# image.png.hash ids.json.hash some-folder.hash
+bev pull image.png.hash --mode copy
+ls
+# image.png ids.json.hash some-folder.hash
+bev pull some-folder.hash --mode copy
+ls
+# image.png ids.json.hash some-folder
+```
+
+### Browsing a hashed folder
+
+In this recipe we "expand" the hashed folder and fill it with the hashes of the files it contains.
+This is much faster than copying back the entire folder.
 
 ```shell
-git clone https://github.com/neuro-ml/bev.git
-cd bev
-pip install -e .
+ls
+# image.png.hash ids.json.hash some-folder.hash
+bev pull some-folder.hash --mode hash
+ls
+# image.png.hash ids.json.hash some-folder
+ls some-folder
+# photo.jpg.hash some-text-file.txt.hash nested-folder
+```
 
-# or let pip handle the cloning:
-pip install git+https://github.com/neuro-ml/bev.git
+Afterwards you can add the folder back
+
+```shell
+bev add some-folder
+ls
+# image.png.hash ids.json.hash some-folder.hash
 ```
 
 # Getting started
 
 1. Choose a folder for your repository and create a basic config (`.bev.yml`):
 
 ```yaml
@@ -65,17 +108,17 @@
 ```shell
 bev init
 ```
 
 3. Add files to bev
 
 ```shell
-bev add /path/to/some/file.json .
-bev add /path/to/some/folder/ .
-bev add /path/to/some/image.png .
+bev add /path/to/some/file.json
+# also can provide several paths
+bev add /path/to/some/folder/ /path/to/some/image.png
 ```
 
 4. ... and to git
 
 ```shell
 git add file.json.hash folder.hash image.png.hash
 git commit -m "added files"
@@ -88,14 +131,25 @@
 from bev import Repository
 
 # `version` can be a commit hash or a git tag 
 repo = Repository('/path/to/repo', version='8a7fe6')
 image = imageio.imread(repo.resolve('image.png'))
 ```
 
+6. Or from cli
+
+```shell
+# replace the folder's hash by the hashes of its files
+bev pull folder.hash --mode hash
+# entirely restore the folder (inverse of `bev add folder`)
+bev pull folder.hash --mode copy
+# same for files
+bev pull image.png.hash --mode copy
+```
+
 ### Advanced usage
 
 Here are some tutorials that cover more advanced configuration, including multiple storage locations and machines:
 
 1. [Create a repository](https://github.com/neuro-ml/bev/wiki/Creating-a-repository) - needed only at first time setup
 2. [Adding files](https://github.com/neuro-ml/bev/wiki/Adding-files)
 3. [Accessing files](https://github.com/neuro-ml/bev/wiki/Accessing-the-stored-files)
```

### Comparing `bev-0.7.0/bev.egg-info/SOURCES.txt` & `bev-0.7.1/bev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/pyproject.toml` & `bev-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bev-0.7.0/setup.py` & `bev-0.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 with open(root / 'bev/__version__.py', encoding='utf-8') as file:
     scope = {}
     exec(file.read(), scope)
     __version__ = scope['__version__']
 
 setup(
     name='bev',
-    packages=find_packages(include=('bev',)),
-    include_package_data=True,
+    packages=find_packages(include=('bev*',)),
     version=__version__,
     description='A small manager for versioned data',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/neuro-ml/bev',
     download_url='https://github.com/neuro-ml/bev/archive/v%s.tar.gz' % __version__,
```

