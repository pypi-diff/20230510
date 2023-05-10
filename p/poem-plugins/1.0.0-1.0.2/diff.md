# Comparing `tmp/poem_plugins-1.0.0.tar.gz` & `tmp/poem_plugins-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poem_plugins-1.0.0.tar", max compression
+gzip compressed data, was "poem_plugins-1.0.2.tar", max compression
```

## Comparing `poem_plugins-1.0.0.tar` & `poem_plugins-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1068 2023-02-03 09:22:00.689034 poem_plugins-1.0.0/LICENSE
--rw-r--r--   0        0        0     3899 2023-03-07 10:16:01.172838 poem_plugins-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-03-07 10:11:09.615671 poem_plugins-1.0.0/poem_plugins/__init__.py
--rw-r--r--   0        0        0      976 2023-03-07 10:16:01.173047 poem_plugins-1.0.0/poem_plugins/config/__init__.py
--rw-r--r--   0        0        0      920 2023-03-07 10:16:01.173221 poem_plugins-1.0.0/poem_plugins/config/base.py
--rw-r--r--   0        0        0      559 2023-03-07 10:16:01.173385 poem_plugins-1.0.0/poem_plugins/config/git.py
--rw-r--r--   0        0        0     1704 2023-05-10 08:10:38.820613 poem_plugins-1.0.0/poem_plugins/dispatchers/.null-ls_652473_version.py
--rw-r--r--   0        0        0        0 2023-03-07 10:11:09.619918 poem_plugins-1.0.0/poem_plugins/dispatchers/__init__.py
--rw-r--r--   0        0        0      418 2023-05-10 08:03:25.648558 poem_plugins-1.0.0/poem_plugins/dispatchers/base.py
--rw-r--r--   0        0        0     1704 2023-05-10 08:10:33.973841 poem_plugins-1.0.0/poem_plugins/dispatchers/version.py
--rw-r--r--   0        0        0        0 2023-03-07 10:11:09.591018 poem_plugins-1.0.0/poem_plugins/general/__init__.py
--rw-r--r--   0        0        0      227 2023-03-07 10:11:09.603142 poem_plugins-1.0.0/poem_plugins/general/strenum.py
--rw-r--r--   0        0        0      339 2023-03-07 10:11:09.604862 poem_plugins-1.0.0/poem_plugins/general/version/__init__.py
--rw-r--r--   0        0        0      332 2023-05-10 08:03:25.649086 poem_plugins-1.0.0/poem_plugins/general/version/drivers/__init__.py
--rw-r--r--   0        0        0     2477 2023-05-10 08:03:25.649258 poem_plugins-1.0.0/poem_plugins/general/version/drivers/git.py
--rw-r--r--   0        0        0      210 2023-05-10 08:03:25.649406 poem_plugins-1.0.0/poem_plugins/handlers/__init__.py
--rw-r--r--   0        0        0     2437 2023-05-10 08:10:33.974122 poem_plugins-1.0.0/poem_plugins/handlers/version.py
--rw-r--r--   0        0        0       86 2023-03-07 10:16:01.174074 poem_plugins-1.0.0/poem_plugins/plugins/__init__.py
--rw-r--r--   0        0        0      133 2023-05-10 08:03:25.650066 poem_plugins-1.0.0/poem_plugins/plugins/base.py
--rw-r--r--   0        0        0      540 2023-05-10 08:03:25.650236 poem_plugins-1.0.0/poem_plugins/plugins/version.py
--rw-r--r--   0        0        0     2457 2023-05-10 08:12:14.458290 poem_plugins-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 poem_plugins-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-02-03 09:22:00.689034 poem_plugins-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3899 2023-03-07 10:16:01.172838 poem_plugins-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-03-07 10:11:09.615671 poem_plugins-1.0.2/poem_plugins/__init__.py
+-rw-r--r--   0        0        0      976 2023-03-07 10:16:01.173047 poem_plugins-1.0.2/poem_plugins/config/__init__.py
+-rw-r--r--   0        0        0      920 2023-03-07 10:16:01.173221 poem_plugins-1.0.2/poem_plugins/config/base.py
+-rw-r--r--   0        0        0      559 2023-03-07 10:16:01.173385 poem_plugins-1.0.2/poem_plugins/config/git.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:11:09.619918 poem_plugins-1.0.2/poem_plugins/dispatchers/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-10 08:03:25.648558 poem_plugins-1.0.2/poem_plugins/dispatchers/base.py
+-rw-r--r--   0        0        0     1652 2023-05-10 08:35:45.781348 poem_plugins-1.0.2/poem_plugins/dispatchers/version.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:11:09.591018 poem_plugins-1.0.2/poem_plugins/general/__init__.py
+-rw-r--r--   0        0        0      227 2023-03-07 10:11:09.603142 poem_plugins-1.0.2/poem_plugins/general/strenum.py
+-rw-r--r--   0        0        0      339 2023-03-07 10:11:09.604862 poem_plugins-1.0.2/poem_plugins/general/version/__init__.py
+-rw-r--r--   0        0        0      332 2023-05-10 08:03:25.649086 poem_plugins-1.0.2/poem_plugins/general/version/drivers/__init__.py
+-rw-r--r--   0        0        0     2477 2023-05-10 08:03:25.649258 poem_plugins-1.0.2/poem_plugins/general/version/drivers/git.py
+-rw-r--r--   0        0        0      210 2023-05-10 08:03:25.649406 poem_plugins-1.0.2/poem_plugins/handlers/__init__.py
+-rw-r--r--   0        0        0     2493 2023-05-10 08:35:45.781658 poem_plugins-1.0.2/poem_plugins/handlers/version.py
+-rw-r--r--   0        0        0       86 2023-03-07 10:16:01.174074 poem_plugins-1.0.2/poem_plugins/plugins/__init__.py
+-rw-r--r--   0        0        0      133 2023-05-10 08:03:25.650066 poem_plugins-1.0.2/poem_plugins/plugins/base.py
+-rw-r--r--   0        0        0      540 2023-05-10 08:03:25.650236 poem_plugins-1.0.2/poem_plugins/plugins/version.py
+-rw-r--r--   0        0        0     2457 2023-05-10 08:36:00.922592 poem_plugins-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5283 1970-01-01 00:00:00.000000 poem_plugins-1.0.2/PKG-INFO
```

### Comparing `poem_plugins-1.0.0/LICENSE` & `poem_plugins-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poem_plugins-1.0.0/README.md` & `poem_plugins-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `poem_plugins-1.0.0/poem_plugins/config/__init__.py` & `poem_plugins-1.0.2/poem_plugins/config/__init__.py`

 * *Files identical despite different names*

### Comparing `poem_plugins-1.0.0/poem_plugins/config/base.py` & `poem_plugins-1.0.2/poem_plugins/config/base.py`

 * *Files identical despite different names*

### Comparing `poem_plugins-1.0.0/poem_plugins/config/git.py` & `poem_plugins-1.0.2/poem_plugins/config/git.py`

 * *Files identical despite different names*

### Comparing `poem_plugins-1.0.0/poem_plugins/dispatchers/.null-ls_652473_version.py` & `poem_plugins-1.0.2/poem_plugins/dispatchers/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,12 +44,9 @@
         except Exception as exc:
             io.write_error_line(
                 "<b>poem-plugins</b>: "
                 f"Cannot load version config, skipping: {exc}",
             )
             return
 
-        if not config.provider:
-            return
-
         handler = VersionHandler.factory(config)
         handler.handle(poetry, io)
```

### Comparing `poem_plugins-1.0.0/poem_plugins/general/version/drivers/git.py` & `poem_plugins-1.0.2/poem_plugins/general/version/drivers/git.py`

 * *Files identical despite different names*

### Comparing `poem_plugins-1.0.0/poem_plugins/handlers/version.py` & `poem_plugins-1.0.2/poem_plugins/handlers/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,16 @@
             driver = GitVersionDriver(settings=config.git)
         return cls(
             config=config,
             driver=driver,
         )
 
     def handle(self, poetry: Poetry, io: IO) -> None:
+        if not self.config.provider:
+            return
         try:
             version = self.driver.get_version()
         except Exception as exc:
             io.write_error_line(f"<b>poem-plugins</b>: {exc}")
             raise exc
 
         io.write_line(
```

### Comparing `poem_plugins-1.0.0/poem_plugins/plugins/version.py` & `poem_plugins-1.0.2/poem_plugins/plugins/version.py`

 * *Files identical despite different names*

### Comparing `poem_plugins-1.0.0/pyproject.toml` & `poem_plugins-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poem-plugins"
-version = "1.0.0"
+version = "1.0.2"
 description = "Some set of poetry plugins"
 authors = ["Ivan Sitkin <alvinera@yandex.ru>"]
 repository = "https://github.com/alviner/poem-plugins"
 homepage = "https://pypi.org/project/poem-plugins"
 documentation = "https://github.com/alviner/poem-plugins"
 keywords = ["plugins", "poetry"]
 license = "MIT"
```

### Comparing `poem_plugins-1.0.0/PKG-INFO` & `poem_plugins-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poem-plugins
-Version: 1.0.0
+Version: 1.0.2
 Summary: Some set of poetry plugins
 Home-page: https://pypi.org/project/poem-plugins
 License: MIT
 Keywords: plugins,poetry
 Author: Ivan Sitkin
 Author-email: alvinera@yandex.ru
 Requires-Python: >=3.9,<4.0
```

