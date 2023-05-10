# Comparing `tmp/flaks-0.7.tar.gz` & `tmp/flaks-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks-0.7.tar", last modified: Wed May 10 13:22:13 2023, max compression
+gzip compressed data, was "flaks-0.8.tar", last modified: Wed May 10 13:34:26 2023, max compression
```

## Comparing `flaks-0.7.tar` & `flaks-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:22:13.511923 flaks-0.7/
--rw-rw-rw-   0        0        0      206 2023-05-10 13:22:13.511923 flaks-0.7/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.7/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 13:22:13.512930 flaks-0.7/setup.cfg
--rw-rw-rw-   0        0        0      659 2023-05-10 13:22:05.000000 flaks-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:22:13.500535 flaks-0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:22:13.505125 flaks-0.7/src/flaks/
--rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.7/src/flaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:22:13.510861 flaks-0.7/src/flaks.egg-info/
--rw-rw-rw-   0        0        0      206 2023-05-10 13:22:13.000000 flaks-0.7/src/flaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-10 13:22:13.000000 flaks-0.7/src/flaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:22:13.000000 flaks-0.7/src/flaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-10 13:22:13.000000 flaks-0.7/src/flaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 13:22:13.000000 flaks-0.7/src/flaks.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:34:26.050032 flaks-0.8/
+-rw-rw-rw-   0        0        0      206 2023-05-10 13:34:26.050032 flaks-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.8/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 13:34:26.051032 flaks-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      659 2023-05-10 13:34:01.000000 flaks-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:34:26.039820 flaks-0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:34:26.044515 flaks-0.8/src/flaks/
+-rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.8/src/flaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:34:26.049033 flaks-0.8/src/flaks.egg-info/
+-rw-rw-rw-   0        0        0      206 2023-05-10 13:34:25.000000 flaks-0.8/src/flaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-10 13:34:26.000000 flaks-0.8/src/flaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:34:25.000000 flaks-0.8/src/flaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-10 13:34:25.000000 flaks-0.8/src/flaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 13:34:25.000000 flaks-0.8/src/flaks.egg-info/top_level.txt
```

### Comparing `flaks-0.7/setup.py` & `flaks-0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,23 +7,23 @@
         install.run(self)
         import flaks_setup
         flaks_setup.post_install()
 
 
 setup(
     name='flaks',
-    version='0.7',
+    version='0.8',
     license='MIT',
     author="Mario Nascimento",
     author_email='marionascimento047@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/darkarp/flaks',
     keywords='example project',
     install_requires=[
         'requests',
-        'flaks_setup==0.92'
+        'flaks_setup==0.93'
     ],
     cmdclass={
         'install': PostInstallCommand
     }
 )
```

