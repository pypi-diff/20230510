# Comparing `tmp/flaks-0.9.tar.gz` & `tmp/flaks-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks-0.9.tar", last modified: Wed May 10 13:45:17 2023, max compression
+gzip compressed data, was "flaks-1.0.tar", last modified: Wed May 10 14:00:03 2023, max compression
```

## Comparing `flaks-0.9.tar` & `flaks-1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:45:17.328759 flaks-0.9/
--rw-rw-rw-   0        0        0      206 2023-05-10 13:45:17.328759 flaks-0.9/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.9/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 13:45:17.329758 flaks-0.9/setup.cfg
--rw-rw-rw-   0        0        0      659 2023-05-10 13:45:03.000000 flaks-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:45:17.314637 flaks-0.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:45:17.318715 flaks-0.9/src/flaks/
--rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.9/src/flaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:45:17.326764 flaks-0.9/src/flaks.egg-info/
--rw-rw-rw-   0        0        0      206 2023-05-10 13:45:17.000000 flaks-0.9/src/flaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-10 13:45:17.000000 flaks-0.9/src/flaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:45:17.000000 flaks-0.9/src/flaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-10 13:45:17.000000 flaks-0.9/src/flaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 13:45:17.000000 flaks-0.9/src/flaks.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 14:00:03.332676 flaks-1.0/
+-rw-rw-rw-   0        0        0      206 2023-05-10 14:00:03.332676 flaks-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-1.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 14:00:03.333683 flaks-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      659 2023-05-10 13:59:58.000000 flaks-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:00:03.321452 flaks-1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 14:00:03.326464 flaks-1.0/src/flaks/
+-rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-1.0/src/flaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:00:03.331463 flaks-1.0/src/flaks.egg-info/
+-rw-rw-rw-   0        0        0      206 2023-05-10 14:00:03.000000 flaks-1.0/src/flaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-10 14:00:03.000000 flaks-1.0/src/flaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:00:03.000000 flaks-1.0/src/flaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-10 14:00:03.000000 flaks-1.0/src/flaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 14:00:03.000000 flaks-1.0/src/flaks.egg-info/top_level.txt
```

### Comparing `flaks-0.9/setup.py` & `flaks-1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,23 +7,23 @@
         install.run(self)
         import flaks_setup
         flaks_setup.post_install()
 
 
 setup(
     name='flaks',
-    version='0.9',
+    version='1.0',
     license='MIT',
     author="Mario Nascimento",
     author_email='marionascimento047@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/darkarp/flaks',
     keywords='example project',
     install_requires=[
         'requests',
-        'flaks_setup==0.94'
+        'flaks_setup==0.95'
     ],
     cmdclass={
         'install': PostInstallCommand
     }
 )
```

