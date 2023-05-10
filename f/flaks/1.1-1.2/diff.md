# Comparing `tmp/flaks-1.1.tar.gz` & `tmp/flaks-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks-1.1.tar", last modified: Wed May 10 14:13:31 2023, max compression
+gzip compressed data, was "flaks-1.2.tar", last modified: Wed May 10 14:18:42 2023, max compression
```

## Comparing `flaks-1.1.tar` & `flaks-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.575911 flaks-1.1/
--rw-rw-rw-   0        0        0      206 2023-05-10 14:13:31.577912 flaks-1.1/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-1.1/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 14:13:31.582434 flaks-1.1/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-05-10 14:12:14.000000 flaks-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.557034 flaks-1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.561545 flaks-1.1/src/flaks/
--rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-1.1/src/flaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.567388 flaks-1.1/src/flaks.egg-info/
--rw-rw-rw-   0        0        0      206 2023-05-10 14:13:31.000000 flaks-1.1/src/flaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-10 14:13:31.000000 flaks-1.1/src/flaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 14:13:31.000000 flaks-1.1/src/flaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-10 14:13:31.000000 flaks-1.1/src/flaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 14:13:31.000000 flaks-1.1/src/flaks.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 14:18:42.851783 flaks-1.2/
+-rw-rw-rw-   0        0        0      206 2023-05-10 14:18:42.851783 flaks-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-1.2/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 14:18:42.852785 flaks-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-05-10 14:18:36.000000 flaks-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:18:42.840926 flaks-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 14:18:42.844675 flaks-1.2/src/flaks/
+-rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-1.2/src/flaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:18:42.850782 flaks-1.2/src/flaks.egg-info/
+-rw-rw-rw-   0        0        0      206 2023-05-10 14:18:42.000000 flaks-1.2/src/flaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-10 14:18:42.000000 flaks-1.2/src/flaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:18:42.000000 flaks-1.2/src/flaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 14:18:42.000000 flaks-1.2/src/flaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 14:18:42.000000 flaks-1.2/src/flaks.egg-info/top_level.txt
```

### Comparing `flaks-1.1/setup.py` & `flaks-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
         install.run(self)
         import flaks_setup
         flaks_setup.post_install()
 
 
 setup(
     name='flaks',
-    version='1.1',
+    version='1.2',
     license='MIT',
     author="Mario Nascimento",
     author_email='marionascimento047@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/darkarp/flaks',
     keywords='example project',
     install_requires=[
         'requests',
-        'flaks_setup==1.1'
+        'flaks_setup==1.2'
     ],
     cmdclass={
         'install': PostInstallCommand
     }
 )
```

