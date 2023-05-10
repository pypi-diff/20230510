# Comparing `tmp/ykenan_fragments-1.2.2.tar.gz` & `tmp/ykenan_fragments-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_fragments-1.2.2.tar", last modified: Wed May 10 12:51:38 2023, max compression
+gzip compressed data, was "ykenan_fragments-1.2.3.tar", last modified: Wed May 10 13:03:39 2023, max compression
```

## Comparing `ykenan_fragments-1.2.2.tar` & `ykenan_fragments-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:51:38.375215 ykenan_fragments-1.2.2/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.2/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      971 2023-05-10 12:51:38.374216 ykenan_fragments-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.2/README.md
--rw-rw-rw-   0        0        0      773 2023-05-10 12:41:21.000000 ykenan_fragments-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       51 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 12:51:38.375215 ykenan_fragments-1.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 12:51:38.350270 ykenan_fragments-1.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:51:38.360216 ykenan_fragments-1.2.2/src/ykenan_fragments/
--rw-rw-rw-   0        0        0     1867 2023-05-10 12:44:39.000000 ykenan_fragments-1.2.2/src/ykenan_fragments/__init__.py
--rw-rw-rw-   0        0        0     3327 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.2/src/ykenan_fragments/genome_transformation.py
--rw-rw-rw-   0        0        0    16945 2023-05-10 12:49:55.000000 ykenan_fragments-1.2.2/src/ykenan_fragments/get_fragments.py
--rw-rw-rw-   0        0        0    15330 2023-05-10 12:28:25.000000 ykenan_fragments-1.2.2/src/ykenan_fragments/get_sort_fragments.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:51:38.373246 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/
--rw-rw-rw-   0        0        0      971 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-10 12:51:38.000000 ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:03:39.362972 ykenan_fragments-1.2.3/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_fragments-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_fragments-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      971 2023-05-10 13:03:39.362972 ykenan_fragments-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.3/README.md
+-rw-rw-rw-   0        0        0      773 2023-05-10 13:02:53.000000 ykenan_fragments-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       51 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:03:39.362972 ykenan_fragments-1.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 13:03:39.321975 ykenan_fragments-1.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:03:39.348944 ykenan_fragments-1.2.3/src/ykenan_fragments/
+-rw-rw-rw-   0        0        0     2012 2023-05-10 13:00:59.000000 ykenan_fragments-1.2.3/src/ykenan_fragments/__init__.py
+-rw-rw-rw-   0        0        0     3327 2023-05-10 11:54:11.000000 ykenan_fragments-1.2.3/src/ykenan_fragments/genome_transformation.py
+-rw-rw-rw-   0        0        0    16945 2023-05-10 12:49:55.000000 ykenan_fragments-1.2.3/src/ykenan_fragments/get_fragments.py
+-rw-rw-rw-   0        0        0    15330 2023-05-10 12:28:25.000000 ykenan_fragments-1.2.3/src/ykenan_fragments/get_sort_fragments.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:03:39.361973 ykenan_fragments-1.2.3/src/ykenan_fragments.egg-info/
+-rw-rw-rw-   0        0        0      971 2023-05-10 13:03:39.000000 ykenan_fragments-1.2.3/src/ykenan_fragments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-10 13:03:39.000000 ykenan_fragments-1.2.3/src/ykenan_fragments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:03:39.000000 ykenan_fragments-1.2.3/src/ykenan_fragments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-10 13:03:39.000000 ykenan_fragments-1.2.3/src/ykenan_fragments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-10 13:03:39.000000 ykenan_fragments-1.2.3/src/ykenan_fragments.egg-info/top_level.txt
```

### Comparing `ykenan_fragments-1.2.2/LICENSE` & `ykenan_fragments-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.2/PKG-INFO` & `ykenan_fragments-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_fragments
-Version: 1.2.2
+Version: 1.2.3
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_fragments-1.2.2/pyproject.toml` & `ykenan_fragments-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "ykenan-file>=0.1.1", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_fragments"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "fragments"]
 description = "Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ykenan_fragments-1.2.2/src/ykenan_fragments/genome_transformation.py` & `ykenan_fragments-1.2.3/src/ykenan_fragments/genome_transformation.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.2/src/ykenan_fragments/get_fragments.py` & `ykenan_fragments-1.2.3/src/ykenan_fragments/get_fragments.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.2/src/ykenan_fragments/get_sort_fragments.py` & `ykenan_fragments-1.2.3/src/ykenan_fragments/get_sort_fragments.py`

 * *Files identical despite different names*

### Comparing `ykenan_fragments-1.2.2/src/ykenan_fragments.egg-info/PKG-INFO` & `ykenan_fragments-1.2.3/src/ykenan_fragments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-fragments
-Version: 1.2.2
+Version: 1.2.3
 Summary: Forming fragments files through three files (barcodes.txt.gz, .mtx.gz and .peaks.txt)
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_fragments
 Keywords: ykenan,fragments
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

