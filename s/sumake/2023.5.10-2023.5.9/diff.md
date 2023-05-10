# Comparing `tmp/sumake-2023.5.10.tar.gz` & `tmp/sumake-2023.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumake-2023.5.10.tar", last modified: Wed May 10 08:46:02 2023, max compression
+gzip compressed data, was "sumake-2023.5.9.tar", last modified: Tue May  9 10:15:22 2023, max compression
```

## Comparing `sumake-2023.5.10.tar` & `sumake-2023.5.9.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-10 08:46:02.505719 sumake-2023.5.10/
--rw-r--r--   0 peng       (501) staff       (20)      232 2023-05-10 08:46:02.505542 sumake-2023.5.10/PKG-INFO
--rw-r--r--   0 peng       (501) staff       (20)       39 2023-05-09 10:00:42.000000 sumake-2023.5.10/README.md
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-10 08:46:02.503696 sumake-2023.5.10/bin/
--rwxr-xr-x   0 peng       (501) staff       (20)      359 2023-05-10 06:21:51.000000 sumake-2023.5.10/bin/sumake
--rw-r--r--   0 peng       (501) staff       (20)       38 2023-05-10 08:46:02.505773 sumake-2023.5.10/setup.cfg
--rw-r--r--   0 peng       (501) staff       (20)     1884 2023-05-10 08:45:58.000000 sumake-2023.5.10/setup.py
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-10 08:46:02.505071 sumake-2023.5.10/sumake.egg-info/
--rw-r--r--   0 peng       (501) staff       (20)      232 2023-05-10 08:46:02.000000 sumake-2023.5.10/sumake.egg-info/PKG-INFO
--rw-r--r--   0 peng       (501) staff       (20)      226 2023-05-10 08:46:02.000000 sumake-2023.5.10/sumake.egg-info/SOURCES.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-10 08:46:02.000000 sumake-2023.5.10/sumake.egg-info/dependency_links.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-09 10:00:51.000000 sumake-2023.5.10/sumake.egg-info/not-zip-safe
--rw-r--r--   0 peng       (501) staff       (20)       11 2023-05-10 08:46:02.000000 sumake-2023.5.10/sumake.egg-info/requires.txt
--rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-10 08:46:02.000000 sumake-2023.5.10/sumake.egg-info/top_level.txt
-drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-10 08:46:02.505217 sumake-2023.5.10/test/
--rw-r--r--   0 peng       (501) staff       (20)      167 2023-05-10 05:44:52.000000 sumake-2023.5.10/test/test_setup.py
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-09 10:15:22.744792 sumake-2023.5.9/
+-rw-r--r--   0 peng       (501) staff       (20)      231 2023-05-09 10:15:22.744559 sumake-2023.5.9/PKG-INFO
+-rw-r--r--   0 peng       (501) staff       (20)       39 2023-05-09 10:00:42.000000 sumake-2023.5.9/README.md
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-09 10:15:22.741387 sumake-2023.5.9/bin/
+-rw-r--r--   0 peng       (501) staff       (20)       65 2023-05-09 10:00:51.000000 sumake-2023.5.9/bin/sumake
+-rw-r--r--   0 peng       (501) staff       (20)       38 2023-05-09 10:15:22.744865 sumake-2023.5.9/setup.cfg
+-rw-r--r--   0 peng       (501) staff       (20)     1702 2023-05-09 10:00:03.000000 sumake-2023.5.9/setup.py
+drwxr-xr-x   0 peng       (501) staff       (20)        0 2023-05-09 10:15:22.744261 sumake-2023.5.9/sumake.egg-info/
+-rw-r--r--   0 peng       (501) staff       (20)      231 2023-05-09 10:15:22.000000 sumake-2023.5.9/sumake.egg-info/PKG-INFO
+-rw-r--r--   0 peng       (501) staff       (20)      207 2023-05-09 10:15:22.000000 sumake-2023.5.9/sumake.egg-info/SOURCES.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-09 10:15:22.000000 sumake-2023.5.9/sumake.egg-info/dependency_links.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-09 10:00:51.000000 sumake-2023.5.9/sumake.egg-info/not-zip-safe
+-rw-r--r--   0 peng       (501) staff       (20)       11 2023-05-09 10:15:22.000000 sumake-2023.5.9/sumake.egg-info/requires.txt
+-rw-r--r--   0 peng       (501) staff       (20)        1 2023-05-09 10:15:22.000000 sumake-2023.5.9/sumake.egg-info/top_level.txt
```

### Comparing `sumake-2023.5.10/setup.py` & `sumake-2023.5.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 import os.path
 import shutil
-import sysconfig
-from pathlib import Path
 
+from setuptools import find_packages
 from setuptools import setup
+import sysconfig
+
+from setuptools.command.develop import develop
+from setuptools.command.install import install
 from wheel.bdist_wheel import bdist_wheel
+from pathlib import Path
 
+# home_dir = os.path.expanduser("~")
 home_dir = Path.home()
 install_dir = sysconfig.get_paths()['purelib']
 print(home_dir)
 print(install_dir)
 
-VERSION = "2023.5.10"
+VERSION = "2023.5.9"
 
 current = Path(__file__).parent.absolute()
-
-
-def generate_sumake(home_dir, current):
-    sumake_dir = home_dir / ".sumake"
-    bin_dir = current / "bin"
-
-    utils_mk = sumake_dir / "utils.mk"
-
-    if not os.path.exists(sumake_dir):
-        os.makedirs(sumake_dir)
-    if not os.path.exists(bin_dir):
-        os.makedirs(bin_dir)
-    print("current", current)
-
-    shutil.copy(current / "utils.mk", utils_mk)
-    # open("./sumake")
-    with open(current / "./sumake", "r") as template:
-        with open(bin_dir / "sumake", "w") as target:
-            res = template.read().format(
-                UTILS_MK=utils_mk,
-                VERSION=VERSION, )
-            target.write(res)
+sumake_dir = home_dir / ".sumake"
+utils_mk = sumake_dir / "utils.mk"
+bin_dir = current / "bin"
 
 
 class PreInstallCommand(bdist_wheel):
     def run(self):
-        generate_sumake(home_dir, current)
+        if not os.path.exists(sumake_dir):
+            os.makedirs(sumake_dir)
+        if not os.path.exists(bin_dir):
+            os.makedirs(bin_dir)
+        print("current", current)
+
+        shutil.copy(current / "utils.mk", utils_mk)
+        with open(bin_dir / "sumake", "w") as f:
+            f.write(f"""
+#!/bin/bash
+make -f {utils_mk} $@
+            """)
         bdist_wheel.run(self)
 
 
-if __name__ == '__main__':
-    setup(
-        author="SuCicada",
-        author_email="pengyifu@gmail.com",
-        classifiers=[],
-        description="A generic makefile for projects.",
-        scripts=["bin/sumake"],
-        cmdclass={
-            # "install": PreInstallCommand,
-            "bdist_wheel": PreInstallCommand
-        },
-        install_requires=["setuptools"],
-
-        # include_package_data=True,
-        # install_requires=[],
-        # keywords="",
-        # license="",
-        long_description=open("README.md").read(),
-        name="sumake",
-        # namespace_packages=[],
-        # packages=find_packages(),
-        # py_modules=["."],
-        # test_suite="",
-        url="https://github.com/SuCicada/sumake",
-        version=VERSION,
-        zip_safe=False,
-    )
+setup(
+    author="SuCicada",
+    author_email="pengyifu@gmail.com",
+    classifiers=[],
+    description="A generic makefile for projects.",
+    scripts=["bin/sumake"],
+    cmdclass={
+        # "install": PreInstallCommand,
+        "bdist_wheel": PreInstallCommand
+    },
+    install_requires=["setuptools"],
+
+    # include_package_data=True,
+    # install_requires=[],
+    # keywords="",
+    # license="",
+    long_description=open("README.md").read(),
+    name="sumake",
+    # namespace_packages=[],
+    # packages=find_packages(),
+    # py_modules=["."],
+    # test_suite="",
+    url="https://github.com/SuCicada/sumake",
+    version=VERSION,
+    zip_safe=False,
+)
```

