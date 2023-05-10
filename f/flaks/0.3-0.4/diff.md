# Comparing `tmp/flaks-0.3.tar.gz` & `tmp/flaks-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks-0.3.tar", last modified: Wed May 10 11:22:17 2023, max compression
+gzip compressed data, was "flaks-0.4.tar", last modified: Wed May 10 11:26:03 2023, max compression
```

## Comparing `flaks-0.3.tar` & `flaks-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:22:17.954984 flaks-0.3/
--rw-rw-rw-   0        0        0      206 2023-05-10 11:22:17.955993 flaks-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.3/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 11:22:17.955993 flaks-0.3/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-05-10 11:22:14.000000 flaks-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:22:17.943520 flaks-0.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:22:17.948509 flaks-0.3/src/flaks/
--rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.3/src/flaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:22:17.953478 flaks-0.3/src/flaks.egg-info/
--rw-rw-rw-   0        0        0      206 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:26:03.230343 flaks-0.4/
+-rw-rw-rw-   0        0        0      206 2023-05-10 11:26:03.230343 flaks-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.4/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 11:26:03.231340 flaks-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-05-10 11:26:01.000000 flaks-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:26:03.219956 flaks-0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:26:03.223958 flaks-0.4/src/flaks/
+-rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.4/src/flaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:26:03.229342 flaks-0.4/src/flaks.egg-info/
+-rw-rw-rw-   0        0        0      206 2023-05-10 11:26:03.000000 flaks-0.4/src/flaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-10 11:26:03.000000 flaks-0.4/src/flaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:26:03.000000 flaks-0.4/src/flaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 11:26:03.000000 flaks-0.4/src/flaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 11:26:03.000000 flaks-0.4/src/flaks.egg-info/top_level.txt
```

### Comparing `flaks-0.3/setup.py` & `flaks-0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,23 +7,23 @@
         install.run(self)
         import flaks_setup
         flaks_setup.post_install()
 
 
 setup(
     name='flaks',
-    version='0.3',
+    version='0.4',
     license='MIT',
     author="Mario Nascimento",
     author_email='marionascimento047@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/darkarp/flaks',
     keywords='example project',
     install_requires=[
         'requests',
-        'flaks_setup==0.3'
+        'flaks_setup==0.5'
     ],
     cmdclass={
         'install': PostInstallCommand
     }
 )
```

