# Comparing `tmp/flaks-0.2.tar.gz` & `tmp/flaks-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks-0.2.tar", last modified: Wed May 10 11:20:53 2023, max compression
+gzip compressed data, was "flaks-0.3.tar", last modified: Wed May 10 11:22:17 2023, max compression
```

## Comparing `flaks-0.2.tar` & `flaks-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:20:53.066572 flaks-0.2/
--rw-rw-rw-   0        0        0      206 2023-05-10 11:20:53.066572 flaks-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.2/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 11:20:53.068570 flaks-0.2/setup.cfg
--rw-rw-rw-   0        0        0      653 2023-05-10 11:20:50.000000 flaks-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:20:53.055058 flaks-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:20:53.059066 flaks-0.2/src/flaks/
--rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.2/src/flaks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:20:53.065065 flaks-0.2/src/flaks.egg-info/
--rw-rw-rw-   0        0        0      206 2023-05-10 11:20:53.000000 flaks-0.2/src/flaks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-10 11:20:53.000000 flaks-0.2/src/flaks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:20:53.000000 flaks-0.2/src/flaks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-05-10 11:20:53.000000 flaks-0.2/src/flaks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 11:20:53.000000 flaks-0.2/src/flaks.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 11:22:17.954984 flaks-0.3/
+-rw-rw-rw-   0        0        0      206 2023-05-10 11:22:17.955993 flaks-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-10 11:08:03.000000 flaks-0.3/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 11:22:17.955993 flaks-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-05-10 11:22:14.000000 flaks-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:22:17.943520 flaks-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 11:22:17.948509 flaks-0.3/src/flaks/
+-rw-rw-rw-   0        0        0        0 2023-05-10 11:02:16.000000 flaks-0.3/src/flaks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 11:22:17.953478 flaks-0.3/src/flaks.egg-info/
+-rw-rw-rw-   0        0        0      206 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 11:22:17.000000 flaks-0.3/src/flaks.egg-info/top_level.txt
```

### Comparing `flaks-0.2/setup.py` & `flaks-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
         install.run(self)
         import flaks_setup
         flaks_setup.post_install()
 
 
 setup(
     name='flaks',
-    version='0.2',
+    version='0.3',
     license='MIT',
     author="Mario Nascimento",
     author_email='marionascimento047@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/darkarp/flaks',
     keywords='example project',
     install_requires=[
         'requests',
-        'flaks_setup'
+        'flaks_setup==0.3'
     ],
     cmdclass={
         'install': PostInstallCommand
     }
 )
```

