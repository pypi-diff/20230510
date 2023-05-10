# Comparing `tmp/types-setuptools-67.7.0.1.tar.gz` & `tmp/types-setuptools-67.7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-setuptools-67.7.0.1.tar", last modified: Mon May  1 15:15:12 2023, max compression
+gzip compressed data, was "types-setuptools-67.7.0.2.tar", last modified: Wed May 10 15:20:33 2023, max compression
```

## Comparing `types-setuptools-67.7.0.1.tar` & `types-setuptools-67.7.0.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:12.890948 types-setuptools-67.7.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-05-01 15:15:09.000000 types-setuptools-67.7.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 15:15:09.000000 types-setuptools-67.7.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 15:15:12.890948 types-setuptools-67.7.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:12.882948 types-setuptools-67.7.0.1/pkg_resources-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-01 15:15:09.000000 types-setuptools-67.7.0.1/pkg_resources-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/pkg_resources-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:15:12.890948 types-setuptools-67.7.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-01 15:15:09.000000 types-setuptools-67.7.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:12.886948 types-setuptools-67.7.0.1/setuptools-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-01 15:15:09.000000 types-setuptools-67.7.0.1/setuptools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:12.886948 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/cmd.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:12.886948 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/_distutils/filelist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/archive_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/build_meta.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:12.890948 types-setuptools-67.7.0.1/setuptools-stubs/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/alias.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/build_clib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/build_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/build_py.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/develop.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/dist_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/easy_install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/install.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/install_egg_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/install_lib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/install_scripts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/register.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/rotate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/saveopts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/sdist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/setopt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/test.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/command/upload_docs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/dep_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/depends.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/dist.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/extension.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:12.890948 types-setuptools-67.7.0.1/setuptools-stubs/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/extern/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/glob.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/installer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/launch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/monkey.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/msvc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/namespaces.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/package_index.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/sandbox.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/unicode_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/warnings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/wheel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-01 15:14:47.000000 types-setuptools-67.7.0.1/setuptools-stubs/windows_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:15:12.890948 types-setuptools-67.7.0.1/types_setuptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-01 15:15:12.000000 types-setuptools-67.7.0.1/types_setuptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-01 15:15:12.000000 types-setuptools-67.7.0.1/types_setuptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:15:12.000000 types-setuptools-67.7.0.1/types_setuptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-01 15:15:12.000000 types-setuptools-67.7.0.1/types_setuptools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.022217 types-setuptools-67.7.0.2/pkg_resources-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/pkg_resources-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/pkg_resources-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.026217 types-setuptools-67.7.0.2/setuptools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/setuptools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.026217 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/cmd.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.026217 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/_distutils/filelist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/archive_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/build_meta.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/setuptools-stubs/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/alias.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/build_clib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/build_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/build_py.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/develop.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/dist_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/easy_install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/install.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/install_egg_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/install_lib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/install_scripts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/register.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/rotate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/saveopts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/sdist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/setopt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/test.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/command/upload_docs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/dep_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/depends.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/dist.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/extension.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/setuptools-stubs/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/extern/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/glob.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/installer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/launch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/monkey.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/msvc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/namespaces.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/package_index.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/sandbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/unicode_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/warnings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/wheel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 15:19:44.000000 types-setuptools-67.7.0.2/setuptools-stubs/windows_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:33.030217 types-setuptools-67.7.0.2/types_setuptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/types_setuptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/types_setuptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/types_setuptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 15:20:32.000000 types-setuptools-67.7.0.2/types_setuptools.egg-info/top_level.txt
```

### Comparing `types-setuptools-67.7.0.1/CHANGELOG.md` & `types-setuptools-67.7.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 67.7.0.2 (2023-05-10)
+
+Add `partial_stub` metadata field (#10157)
+
 ## 67.7.0.1 (2023-05-01)
 
 Avoid unnecessary forward refs in class definitions (#10124)
 
 ## 67.7.0.0 (2023-04-22)
 
 setuptools: bump to 67.7 (#10069)
```

### Comparing `types-setuptools-67.7.0.1/PKG-INFO` & `types-setuptools-67.7.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.7.0.1
+Version: 67.7.0.2
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e816acffddf9d984bac131224b0eb0f6a3e1c9fc`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-setuptools-67.7.0.1/pkg_resources-stubs/__init__.pyi` & `types-setuptools-67.7.0.2/pkg_resources-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setup.py` & `types-setuptools-67.7.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e816acffddf9d984bac131224b0eb0f6a3e1c9fc`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
 '''.lstrip()
 
 setup(name=name,
-      version="67.7.0.1",
+      version="67.7.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md",
```

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/__init__.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/cmd.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/build_clib.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_clib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/build_ext.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/build_py.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/install.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/install_lib.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/install_lib.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/register.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/register.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/command/sdist.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/dist.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/errors.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/extension.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/_distutils/filelist.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/_distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/archive_util.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/build_meta.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/build_meta.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/build_ext.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/build_ext.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/build_py.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/build_py.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/develop.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/develop.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/easy_install.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/easy_install.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/egg_info.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/egg_info.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/sdist.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/sdist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/setopt.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/setopt.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/test.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/test.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/command/upload_docs.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/command/upload_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/depends.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/depends.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/dist.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/dist.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/errors.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/extension.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/extern/__init__.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/extern/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/msvc.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/msvc.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/package_index.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/package_index.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/setuptools-stubs/sandbox.pyi` & `types-setuptools-67.7.0.2/setuptools-stubs/sandbox.pyi`

 * *Files identical despite different names*

### Comparing `types-setuptools-67.7.0.1/types_setuptools.egg-info/PKG-INFO` & `types-setuptools-67.7.0.2/types_setuptools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-setuptools
-Version: 67.7.0.1
+Version: 67.7.0.2
 Summary: Typing stubs for setuptools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/setuptools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `setuptools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/setuptools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e816acffddf9d984bac131224b0eb0f6a3e1c9fc`.
+This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
```

### Comparing `types-setuptools-67.7.0.1/types_setuptools.egg-info/SOURCES.txt` & `types-setuptools-67.7.0.2/types_setuptools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

