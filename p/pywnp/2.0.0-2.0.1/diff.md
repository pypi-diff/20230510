# Comparing `tmp/pywnp-2.0.0.tar.gz` & `tmp/pywnp-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywnp-2.0.0.tar", last modified: Wed May 10 12:50:25 2023, max compression
+gzip compressed data, was "pywnp-2.0.1.tar", last modified: Wed May 10 14:13:31 2023, max compression
```

## Comparing `pywnp-2.0.0.tar` & `pywnp-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:50:25.276545 pywnp-2.0.0/
--rw-rw-rw-   0        0        0     1060 2023-04-26 13:11:28.000000 pywnp-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     6632 2023-05-10 12:50:25.276545 pywnp-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4908 2023-05-10 12:49:48.000000 pywnp-2.0.0/README.md
--rw-rw-rw-   0        0        0      705 2023-05-10 12:48:33.000000 pywnp-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 12:50:25.276545 pywnp-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 12:50:25.254595 pywnp-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:50:25.257596 pywnp-2.0.0/src/pywnp/
--rw-rw-rw-   0        0        0       27 2023-05-08 22:50:56.000000 pywnp-2.0.0/src/pywnp/__init__.py
--rw-rw-rw-   0        0        0    30285 2023-05-09 14:32:57.000000 pywnp-2.0.0/src/pywnp/pywnp.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:50:25.275543 pywnp-2.0.0/src/pywnp.egg-info/
--rw-rw-rw-   0        0        0     6632 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-10 12:50:25.000000 pywnp-2.0.0/src/pywnp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.144901 pywnp-2.0.1/
+-rw-rw-rw-   0        0        0     1060 2023-04-26 13:11:28.000000 pywnp-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     6632 2023-05-10 14:13:31.144901 pywnp-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4908 2023-05-10 12:49:48.000000 pywnp-2.0.1/README.md
+-rw-rw-rw-   0        0        0      705 2023-05-10 14:10:37.000000 pywnp-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 14:13:31.144901 pywnp-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.126355 pywnp-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.128870 pywnp-2.0.1/src/pywnp/
+-rw-rw-rw-   0        0        0       27 2023-05-08 22:50:56.000000 pywnp-2.0.1/src/pywnp/__init__.py
+-rw-rw-rw-   0        0        0    30394 2023-05-10 14:09:46.000000 pywnp-2.0.1/src/pywnp/pywnp.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:13:31.144901 pywnp-2.0.1/src/pywnp.egg-info/
+-rw-rw-rw-   0        0        0     6632 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-10 14:13:31.000000 pywnp-2.0.1/src/pywnp.egg-info/top_level.txt
```

### Comparing `pywnp-2.0.0/LICENSE` & `pywnp-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywnp-2.0.0/PKG-INFO` & `pywnp-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywnp
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python library to communicate with the WebNowPlaying-Redux browser extension
 Author-email: keifufu <pypi@keifufu.dev>
 License: Copyright 2023 keifufu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `pywnp-2.0.0/README.md` & `pywnp-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pywnp-2.0.0/pyproject.toml` & `pywnp-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pywnp"
-version = "2.0.0"
+version = "2.0.1"
 description = "A python library to communicate with the WebNowPlaying-Redux browser extension"
 authors = [ { name="keifufu", email="pypi@keifufu.dev" } ]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [ "webnowplaying", "wnp", "youtube", "spotify", "media", "music" ]
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywnp-2.0.0/src/pywnp/pywnp.py` & `pywnp-2.0.1/src/pywnp/pywnp.py`

 * *Files 0% similar despite different names*

```diff
@@ -594,16 +594,19 @@
       
       keys_to_remove: List[str] = list()
       for media_info in WNPRedux.media_info_dictionary:
         if media_info._id.startswith(WNPReduxNative.id_prefix):
           if not media_info._id.replace(WNPReduxNative.id_prefix, '') in new_sessions:
             keys_to_remove.append(media_info._id)
       for key in keys_to_remove:
-        if key in WNPRedux.media_info_dictionary:
-          WNPRedux.media_info_dictionary.remove(key)
+        for media_info in WNPRedux.media_info_dictionary:
+          if media_info._id == key:
+            WNPRedux.media_info_dictionary.remove(media_info)
+            break
+      WNPRedux.update_media_info()
 
     @staticmethod
     def is_app_blacklisted(app_id: str) -> bool:
       id = app_id.lower()
       if 'chrome' in id: return True
       if 'chromium' in id: return True
       if 'msedge' in id: return True
```

### Comparing `pywnp-2.0.0/src/pywnp.egg-info/PKG-INFO` & `pywnp-2.0.1/src/pywnp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywnp
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python library to communicate with the WebNowPlaying-Redux browser extension
 Author-email: keifufu <pypi@keifufu.dev>
 License: Copyright 2023 keifufu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

