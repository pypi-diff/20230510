# Comparing `tmp/bkapi_plugins_py-0.425.tar.gz` & `tmp/bkapi-plugins-py-0.510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi_plugins_py-0.425.tar", last modified: Tue Apr 25 03:08:16 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.510.tar", last modified: Wed May 10 02:43:08 2023, max compression
```

## Comparing `bkapi_plugins_py-0.425.tar` & `bkapi-plugins-py-0.510.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 03:08:16.171012 bkapi_plugins_py-0.425/
--rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi_plugins_py-0.425/MANIFEST.in
--rw-rw-rw-   0        0        0      257 2023-04-25 03:08:16.171012 bkapi_plugins_py-0.425/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-25 03:08:16.140111 bkapi_plugins_py-0.425/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-04-25 03:08:16.158052 bkapi_plugins_py-0.425/bkapi_plugins/files/
--rw-rw-rw-   0        0        0  3640951 2023-03-24 05:13:43.000000 bkapi_plugins_py-0.425/bkapi_plugins/files/generator1.0.tar.gz
--rw-rw-rw-   0        0        0   579136 2023-04-25 03:01:45.000000 bkapi_plugins_py-0.425/bkapi_plugins/files/ph-live-nginx-master.zip
-drwxrwxrwx   0        0        0        0 2023-04-25 03:08:16.169014 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      257 2023-04-25 03:08:16.000000 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-25 03:08:16.000000 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 03:08:16.000000 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 03:08:16.000000 bkapi_plugins_py-0.425/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 03:08:16.175000 bkapi_plugins_py-0.425/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-04-25 03:08:13.000000 bkapi_plugins_py-0.425/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:43:08.960184 bkapi-plugins-py-0.510/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.510/MANIFEST.in
+-rw-rw-rw-   0        0        0      257 2023-05-10 02:43:08.960700 bkapi-plugins-py-0.510/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 02:43:08.933247 bkapi-plugins-py-0.510/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-05-10 02:43:08.948220 bkapi-plugins-py-0.510/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0    13219 2023-05-10 02:35:23.000000 bkapi-plugins-py-0.510/bkapi_plugins/files/bench.sh
+drwxrwxrwx   0        0        0        0 2023-05-10 02:43:08.958181 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      257 2023-05-10 02:43:08.000000 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-10 02:43:08.000000 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 02:43:08.000000 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 02:43:08.000000 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 02:43:08.963702 bkapi-plugins-py-0.510/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-05-10 02:42:43.000000 bkapi-plugins-py-0.510/setup.py
```

### Comparing `bkapi_plugins_py-0.425/setup.py` & `bkapi-plugins-py-0.510/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
-    name='bkapi_plugins_py', # 包的名字
-    version='0.425', # 版本号每次打包完要改一下
+    name='bkapi-plugins-py', # 包的名字
+    version='0.510', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

