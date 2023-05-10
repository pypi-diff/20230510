# Comparing `tmp/bkapi-plugins-py-0.510.tar.gz` & `tmp/bkapi-plugins-py-0.510-1314.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.510.tar", last modified: Wed May 10 02:43:08 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.510-1314.tar", last modified: Wed May 10 05:14:21 2023, max compression
```

## Comparing `bkapi-plugins-py-0.510.tar` & `bkapi-plugins-py-0.510-1314.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 02:43:08.960184 bkapi-plugins-py-0.510/
--rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.510/MANIFEST.in
--rw-rw-rw-   0        0        0      257 2023-05-10 02:43:08.960700 bkapi-plugins-py-0.510/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-10 02:43:08.933247 bkapi-plugins-py-0.510/bkapi_plugins/
-drwxrwxrwx   0        0        0        0 2023-05-10 02:43:08.948220 bkapi-plugins-py-0.510/bkapi_plugins/files/
--rw-rw-rw-   0        0        0    13219 2023-05-10 02:35:23.000000 bkapi-plugins-py-0.510/bkapi_plugins/files/bench.sh
-drwxrwxrwx   0        0        0        0 2023-05-10 02:43:08.958181 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      257 2023-05-10 02:43:08.000000 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-10 02:43:08.000000 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 02:43:08.000000 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 02:43:08.000000 bkapi-plugins-py-0.510/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 02:43:08.963702 bkapi-plugins-py-0.510/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-05-10 02:42:43.000000 bkapi-plugins-py-0.510/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 05:14:21.002051 bkapi-plugins-py-0.510-1314/
+-rw-rw-rw-   0        0        0       39 2023-04-17 10:01:55.000000 bkapi-plugins-py-0.510-1314/MANIFEST.in
+-rw-rw-rw-   0        0        0      262 2023-05-10 05:14:21.003045 bkapi-plugins-py-0.510-1314/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-10 05:14:20.989094 bkapi-plugins-py-0.510-1314/bkapi_plugins/
+drwxrwxrwx   0        0        0        0 2023-05-10 05:14:20.994073 bkapi-plugins-py-0.510-1314/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0    11355 2023-05-10 05:13:36.000000 bkapi-plugins-py-0.510-1314/bkapi_plugins/files/nginx.md
+drwxrwxrwx   0        0        0        0 2023-05-10 05:14:21.001053 bkapi-plugins-py-0.510-1314/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-10 05:14:20.000000 bkapi-plugins-py-0.510-1314/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-10 05:14:20.000000 bkapi-plugins-py-0.510-1314/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 05:14:20.000000 bkapi-plugins-py-0.510-1314/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 05:14:20.000000 bkapi-plugins-py-0.510-1314/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 05:14:21.006037 bkapi-plugins-py-0.510-1314/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-05-10 05:14:05.000000 bkapi-plugins-py-0.510-1314/setup.py
```

### Comparing `bkapi-plugins-py-0.510/setup.py` & `bkapi-plugins-py-0.510-1314/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.510', # 版本号每次打包完要改一下
+    version='0.510_1314', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

