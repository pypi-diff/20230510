# Comparing `tmp/flaks-0.5.tar.gz` & `tmp/flaks-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks-0.5.tar", last modified: Wed May 10 11:56:49 2023, max compression
+gzip compressed data, was "flaks-0.6.tar", last modified: Wed May 10 12:53:15 2023, max compression
```

## Comparing `flaks-0.5.tar` & `flaks-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:49.165297 flaks-0.5/
--rw-rw-rw-   0        0        0      206 2023-05-10 11:56:49.165297 flaks-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.5/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 11:56:49.166294 flaks-0.5/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-05-10 11:56:42.000000 flaks-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:49.151889 flaks-0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:49.157354 flaks-0.5/src/flaks/
--rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.5/src/flaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:49.164296 flaks-0.5/src/flaks.egg-info/
--rw-rw-rw-   0        0        0      206 2023-05-10 11:56:49.000000 flaks-0.5/src/flaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-10 11:56:49.000000 flaks-0.5/src/flaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:56:49.000000 flaks-0.5/src/flaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-10 11:56:49.000000 flaks-0.5/src/flaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 11:56:49.000000 flaks-0.5/src/flaks.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:53:15.300970 flaks-0.6/
+-rw-rw-rw-   0        0        0      206 2023-05-10 12:53:15.300970 flaks-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.6/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 12:53:15.301969 flaks-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-05-10 12:53:12.000000 flaks-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:53:15.287135 flaks-0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:53:15.292135 flaks-0.6/src/flaks/
+-rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.6/src/flaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:53:15.299972 flaks-0.6/src/flaks.egg-info/
+-rw-rw-rw-   0        0        0      206 2023-05-10 12:53:15.000000 flaks-0.6/src/flaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-10 12:53:15.000000 flaks-0.6/src/flaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:53:15.000000 flaks-0.6/src/flaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 12:53:15.000000 flaks-0.6/src/flaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 12:53:15.000000 flaks-0.6/src/flaks.egg-info/top_level.txt
```

### Comparing `flaks-0.5/setup.py` & `flaks-0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,23 +7,23 @@
         install.run(self)
         import flaks_setup
         flaks_setup.post_install()
 
 
 setup(
     name='flaks',
-    version='0.5',
+    version='0.6',
     license='MIT',
     author="Mario Nascimento",
     author_email='marionascimento047@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/darkarp/flaks',
     keywords='example project',
     install_requires=[
         'requests',
-        'flaks_setup==0.6'
+        'flaks_setup==0.7'
     ],
     cmdclass={
         'install': PostInstallCommand
     }
 )
```

