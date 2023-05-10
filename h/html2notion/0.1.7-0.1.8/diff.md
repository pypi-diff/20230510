# Comparing `tmp/html2notion-0.1.7.tar.gz` & `tmp/html2notion-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.7.tar", last modified: Sat Apr 29 10:42:28 2023, max compression
+gzip compressed data, was "html2notion-0.1.8.tar", last modified: Wed May 10 11:34:46 2023, max compression
```

## Comparing `html2notion-0.1.7.tar` & `html2notion-0.1.8.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.681534 html2notion-0.1.7/
--rw-r--r--   0 feizhao    (501) staff       (20)     1064 2023-03-22 13:58:21.000000 html2notion-0.1.7/LICENSE
--rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-04-29 10:42:28.681904 html2notion-0.1.7/PKG-INFO
--rw-r--r--   0 feizhao    (501) staff       (20)     4111 2023-04-22 07:11:47.000000 html2notion-0.1.7/README.md
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.645708 html2notion-0.1.7/html2notion/
--rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-03-18 15:41:01.000000 html2notion-0.1.7/html2notion/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)     4413 2023-04-29 05:20:41.000000 html2notion-0.1.7/html2notion/main.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.661157 html2notion-0.1.7/html2notion/translate/
--rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-04-08 10:17:44.000000 html2notion-0.1.7/html2notion/translate/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)     4176 2023-04-22 12:42:21.000000 html2notion-0.1.7/html2notion/translate/batch_import.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2724 2023-04-19 14:40:39.000000 html2notion-0.1.7/html2notion/translate/cos_uploader.py
--rw-r--r--   0 feizhao    (501) staff       (20)     3816 2023-04-29 05:20:41.000000 html2notion-0.1.7/html2notion/translate/html2json.py
--rw-r--r--   0 feizhao    (501) staff       (20)    15643 2023-04-29 09:04:36.000000 html2notion-0.1.7/html2notion/translate/html2json_base.py
--rw-r--r--   0 feizhao    (501) staff       (20)     5296 2023-04-29 05:20:41.000000 html2notion-0.1.7/html2notion/translate/html2json_clipper.py
--rw-r--r--   0 feizhao    (501) staff       (20)      430 2023-04-19 23:45:05.000000 html2notion-0.1.7/html2notion/translate/html2json_default.py
--rw-r--r--   0 feizhao    (501) staff       (20)     7443 2023-04-29 09:04:54.000000 html2notion-0.1.7/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 feizhao    (501) staff       (20)     7168 2023-04-23 14:40:05.000000 html2notion-0.1.7/html2notion/translate/notion_export.py
--rw-r--r--   0 feizhao    (501) staff       (20)     3091 2023-04-29 09:56:47.000000 html2notion-0.1.7/html2notion/translate/notion_import.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.668384 html2notion-0.1.7/html2notion/utils/
--rw-r--r--   0 feizhao    (501) staff       (20)      453 2023-04-29 09:56:35.000000 html2notion-0.1.7/html2notion/utils/__init__.py
--rw-r--r--   0 feizhao    (501) staff       (20)      895 2023-04-29 09:55:54.000000 html2notion-0.1.7/html2notion/utils/load_config.py
--rw-r--r--   0 feizhao    (501) staff       (20)     1579 2023-04-20 14:39:58.000000 html2notion-0.1.7/html2notion/utils/log.py
--rw-r--r--   0 feizhao    (501) staff       (20)      437 2023-04-21 14:23:32.000000 html2notion-0.1.7/html2notion/utils/timeutil.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.649918 html2notion-0.1.7/html2notion.egg-info/
--rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 feizhao    (501) staff       (20)      941 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 feizhao    (501) staff       (20)        1 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 feizhao    (501) staff       (20)       54 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 feizhao    (501) staff       (20)      188 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/requires.txt
--rw-r--r--   0 feizhao    (501) staff       (20)       12 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/top_level.txt
--rw-r--r--   0 feizhao    (501) staff       (20)      103 2023-03-18 15:06:24.000000 html2notion-0.1.7/pyproject.toml
--rw-r--r--   0 feizhao    (501) staff       (20)      871 2023-04-29 10:42:28.683316 html2notion-0.1.7/setup.cfg
--rw-r--r--   0 feizhao    (501) staff       (20)       38 2023-03-18 07:34:12.000000 html2notion-0.1.7/setup.py
-drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.679704 html2notion-0.1.7/tests/
--rw-r--r--   0 feizhao    (501) staff       (20)     3940 2023-04-29 10:35:21.000000 html2notion-0.1.7/tests/test_batchimport.py
--rw-r--r--   0 feizhao    (501) staff       (20)     3038 2023-04-20 14:39:58.000000 html2notion-0.1.7/tests/test_cosupload.py
--rw-r--r--   0 feizhao    (501) staff       (20)     2698 2023-04-13 14:42:38.000000 html2notion-0.1.7/tests/test_notionexport.py
--rw-r--r--   0 feizhao    (501) staff       (20)     1690 2023-04-29 09:11:49.000000 html2notion-0.1.7/tests/test_reqlimit.py
--rw-r--r--   0 feizhao    (501) staff       (20)    31656 2023-04-27 14:25:22.000000 html2notion-0.1.7/tests/test_yinxiang.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.060612 html2notion-0.1.8/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.8/LICENSE
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-05-10 11:34:46.060863 html2notion-0.1.8/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.8/README.md
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.039083 html2notion-0.1.8/html2notion/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.8/html2notion/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     6037 2023-05-10 11:12:48.000000 html2notion-0.1.8/html2notion/main.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.050989 html2notion-0.1.8/html2notion/translate/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.8/html2notion/translate/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3610 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/translate/batch_import.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.8/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4003 2023-05-10 11:13:13.000000 html2notion-0.1.8/html2notion/translate/html2json.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    16287 2023-05-10 11:16:12.000000 html2notion-0.1.8/html2notion/translate/html2json_base.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     5812 2023-05-10 11:16:58.000000 html2notion-0.1.8/html2notion/translate/html2json_clipper.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      534 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/translate/html2json_default.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7744 2023-05-10 11:17:48.000000 html2notion-0.1.8/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2331 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/translate/import_stats.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.1.8/html2notion/translate/notion_export.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3894 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/translate/notion_import.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.055179 html2notion-0.1.8/html2notion/utils/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      453 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/utils/__init__.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      895 2023-05-10 11:11:53.000000 html2notion-0.1.8/html2notion/utils/load_config.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.8/html2notion/utils/log.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.8/html2notion/utils/timeutil.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.042275 html2notion-0.1.8/html2notion.egg-info/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      979 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      188 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/requires.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-05-10 11:34:45.000000 html2notion-0.1.8/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.8/pyproject.toml
+-rw-r--r--   0 daemonzhao   (501) staff       (20)      871 2023-05-10 11:34:46.061940 html2notion-0.1.8/setup.cfg
+-rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.8/setup.py
+drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-05-10 11:34:46.059513 html2notion-0.1.8/tests/
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3940 2023-05-10 11:11:53.000000 html2notion-0.1.8/tests/test_batchimport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.8/tests/test_cosupload.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.8/tests/test_notionexport.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)     1801 2023-05-10 11:22:37.000000 html2notion-0.1.8/tests/test_reqlimit.py
+-rw-r--r--   0 daemonzhao   (501) staff       (20)    32686 2023-05-10 11:11:53.000000 html2notion-0.1.8/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.7/LICENSE` & `html2notion-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/PKG-INFO` & `html2notion-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.7
+Version: 0.1.8
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.7/README.md` & `html2notion-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/html2notion/translate/cos_uploader.py` & `html2notion-0.1.8/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/html2notion/translate/html2json.py` & `html2notion-0.1.8/html2notion/translate/html2json.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 from ..translate.html2json_yinxiang import YinXiang_Type
 from ..translate.html2json_clipper import YinXiangClipper_Type
 
 
 """
 <meta name="source" content="yinxiang.superNote"/>
 <meta name="source" content="desktop.mac"/>
+<meta name="source" content="mobile.android"/>
 """
 def _is_yinxiang_export_html(html_soup):
     exporter_version_meta = html_soup.select_one('html > head > meta[name="exporter-version"]')
     meta_source = html_soup.select_one('html > head > meta[name="source"]')
     exporter_version_content = exporter_version_meta.get( 'content', "") if isinstance(exporter_version_meta, Tag) else ""
 
     meta_source_content = meta_source.get('content', "") if isinstance(meta_source, Tag) else ""
     if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
         return False
 
-    yinxiang_source_content = ["yinxiang", "desktop"]
+    yinxiang_source_content = ["yinxiang", "desktop", "mobile"]
     for prefix in yinxiang_source_content:
         if isinstance(meta_source_content, str) and meta_source_content.startswith(prefix):
             return True
     return False
 
 
 """
@@ -42,57 +43,57 @@
 
     if isinstance(exporter_version_content, str) and not exporter_version_content.startswith("Evernote"):
         return False
     clipper_source_meta = html_soup.select_one('html > head > meta[name="source-application"]')
     clipper_source_content = clipper_source_meta.get('content', "") if isinstance(clipper_source_meta, Tag) else ""
     if isinstance(clipper_source_content, str) and clipper_source_content.endswith("evernote"):
         return True
-    if isinstance(clipper_source_content, str) and clipper_source_content in ("微信"):
+    if isinstance(clipper_source_content, str) and clipper_source_content in ["微信",]:
         return True
     return False
 
 
 def _infer_input_type(html_content):
     soup = BeautifulSoup(html_content, 'html.parser')
-    if _is_yinxiang_export_html(soup):
-        return YinXiang_Type
-    elif _is_yinxiang_clipper_html(soup):
+    if _is_yinxiang_clipper_html(soup):
         return YinXiangClipper_Type
+    elif _is_yinxiang_export_html(soup):
+        return YinXiang_Type
     return Default_Type
 
 
-def _get_converter(html_content):
+def _get_converter(html_content, import_stat):
     html_type = _infer_input_type(html_content)
     logger.info(f"Input type: {html_type}")
-    converter = Html2JsonBase.create(html_type, html_content)
+    converter = Html2JsonBase.create(html_type, html_content, import_stat)
     return converter
 
 
 @singledispatch
-def html2json_process(html_content):
-    raise TypeError("Unsupported param type")
+def html2json_process(html_content, import_stat):
+    raise TypeError(f"Unsupported {type(html_content)}, {import_stat}")
 
 
 @html2json_process.register
-def _(html_content: str):
-    converter = _get_converter(html_content)
+def _(html_content: str, import_stat):
+    converter = _get_converter(html_content, import_stat)
     result = converter.process()
     return converter.get_notion_data(), result
 
 
 @html2json_process.register
-def _(html_file: Path):
+def _(html_file: Path, import_stat):
     if not html_file.is_file():
         print(f"Load file: {html_file.resolve()} failed")
-        sys.exit(1)
+        raise FileNotFoundError
 
     with open(html_file, "r") as file:
         html_content = file.read()
 
-    converter = _get_converter(html_content)
+    converter = _get_converter(html_content, import_stat)
     result = converter.process()
     return converter.get_notion_data(), result
 
 
 if __name__ == "__main__":
     test_prepare_conf()
     html_file = Path("./demos/Test Case D.html")
```

### Comparing `html2notion-0.1.7/html2notion/translate/html2json_base.py` & `html2notion-0.1.8/html2notion/translate/html2json_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 import os
 from collections import namedtuple
 from bs4 import NavigableString, Tag, PageElement
-# from typing import Union
 from enum import Enum
 from ..utils import logger, config
 
 class Block(Enum):
     FAIL = "fail"
     PARAGRAPH = "paragraph"
     QUOTE = "quote"
@@ -40,19 +39,20 @@
         _color_tuple("blue", 0, 0, 255),
         _color_tuple("purple", 128, 0, 128),
         _color_tuple("pink", 255, 192, 203),
         _color_tuple("red", 255, 0, 0),
     ]
 
     # Page content should be: https://developers.notion.com/reference/post-page
-    def __init__(self, html_content):
+    def __init__(self, html_content, import_stat):
         self.html_content = html_content
         self.children = []
         self.properties = {}
         self.parent = {}
+        self.import_stat = import_stat
         if 'GITHUB_ACTIONS' in os.environ:
             notion_database_id = os.environ['notion_db_id_1']
         else:
             notion_database_id = config['notion']['database_id']
         self.parent = {"type": "database_id", "database_id": notion_database_id}
 
     def process(self):
@@ -79,14 +79,16 @@
         elif isinstance(tag, Tag):
             for child in tag.children:
                 if isinstance(child, NavigableString):
                     if child.strip():
                         text = child.text
                         parent_tags = [p for p in parents + [tag]]
                         results.append((text, parent_tags))
+                elif isinstance(child, Tag) and child.name == 'br':  
+                    results.append(('<br>', []))
                 else:
                     results.extend(Html2JsonBase.extract_text_and_parents(child, parents + [tag]))
         return results
 
     @staticmethod
     def parse_one_style(tag_soup: Tag, text_params: dict):
         tag_name = tag_soup.name.lower()
@@ -118,70 +120,82 @@
         return
 
     # https://developers.notion.com/reference/request-limits
     # Process one tag and return a list of objects
     # <b><u>unlineline and bold</u></b>
     # <div><font color="#ff2600">Red color4</font></div>
     # <div> Code in super note</div>
-    @staticmethod
-    def generate_inline_obj(tag: PageElement):
+    def generate_inline_obj(self, tag: PageElement):
         res_obj = []
         text_with_parents = Html2JsonBase.extract_text_and_parents(tag)
         for (text, parent_tags) in text_with_parents:
             # Split the text into chunks of 2000 characters
             text_chunks = [text[i:i+2000] for i in range(0, len(text), 2000)]
             for chunk in text_chunks:
                 text_params = {"plain_text": chunk}
                 for parent in parent_tags:
                     Html2JsonBase.parse_one_style(parent, text_params)
+                # process inline line break
+                if chunk == "<br>":
+                    try:
+                        res_obj[-1]["text"]["content"] += "\n"
+                        res_obj[-1]["plain_text"] += "\n"
+                    except Exception as e:
+                        logger.error(f'{res_obj}, {str(e)}')
+                    continue
 
                 if text_params.get("url", ""):
-                    text_obj = Html2JsonBase.generate_link(**text_params)
+                    text_obj = self.generate_link(**text_params)
                 else:
-                    text_obj = Html2JsonBase.generate_text(**text_params)
+                    text_obj = self.generate_text(**text_params)
                 if text_obj:
                     res_obj.append(text_obj)
         return res_obj
 
-    @staticmethod
-    def generate_link(**kwargs):
-        if not kwargs.get("plain_text", ""):
+
+    
+    def generate_link(self, **kwargs):
+        plain_text = kwargs.get("plain_text", "")
+        if not plain_text:
             return
+        
+        self.import_stat.add_notion_text(plain_text)
         return {
             "href": kwargs.get("url", ""),
-            "plain_text": kwargs.get("plain_text", ""),
+            "plain_text": plain_text,
             "text": {
                 "link": {"url": kwargs.get("url", "")},
-                "content": kwargs.get("plain_text", "")
+                "content": plain_text
             },
             "type": "text"
         }
 
-    @staticmethod
-    def generate_text(**kwargs):
+    def generate_text(self, **kwargs):
         plain_text = kwargs.get("plain_text", "")
         if not plain_text:
             return
         annotations = {
             key: value
             for key, value in kwargs.items()
             if key in Html2JsonBase._text_annotations and isinstance(value, Html2JsonBase._text_annotations[key])
         }
+        stats_count = kwargs.get("stats_count", True)
+        if stats_count:
+            self.import_stat.add_notion_text(plain_text)
         text_obj = {
             "plain_text": plain_text,
             "text": {"content": plain_text},
             "type": "text"
         }
         if annotations:
             text_obj["annotations"] = annotations
 
         return text_obj
 
-    @staticmethod
-    def generate_properties(**kwargs):
+    def generate_properties(self, **kwargs):
         title = kwargs.get("title", "")
         url = kwargs.get("url", "")
         tags = kwargs.get("tags", [])
         created_time = kwargs.get("created_time", "")
 
         property_map = {
             "Title": {"title": [{"text": {"content": title}}]} if title else None,
@@ -390,15 +404,15 @@
             "object": "block",
             list_type: {
                 "rich_text": []
             },
             "type": list_type,
         }
         rich_text = json_obj[list_type]["rich_text"]
-        text_obj = Html2JsonBase.generate_inline_obj(soup)
+        text_obj = self.generate_inline_obj(soup)
         if text_obj:
             rich_text.extend(text_obj)
 
         return json_obj
 
     """
     <div>
@@ -424,15 +438,15 @@
             one_row = {
                 "type": "table_row",
                 "table_row": {
                     "cells": []
                 }
             }
             for td in td_tags:
-                col = Html2JsonBase.generate_inline_obj(td)
+                col = self.generate_inline_obj(td)
                 one_row["table_row"]["cells"].append(col)
             table_rows.append(one_row)
 
         table_obj = {
             "table": {
                 "has_row_header": False,
                 "has_column_header": False,
@@ -443,12 +457,12 @@
         return table_obj
 
     @classmethod
     def register(cls, input_type, subclass):
         cls._registry[input_type] = subclass
 
     @classmethod
-    def create(cls, input_type, html_content):
+    def create(cls, input_type, html_content, import_stat):
         subclass = cls._registry.get(input_type)
         if subclass is None:
             raise ValueError(f"noknown: {input_type}")
-        return subclass(html_content)
+        return subclass(html_content, import_stat)
```

### Comparing `html2notion-0.1.7/html2notion/translate/html2json_clipper.py` & `html2notion-0.1.8/html2notion/translate/html2json_clipper.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 
 YinXiangClipper_Type = "clipper.yinxiang"
 
 
 class Html2JsonYinXiang(Html2JsonBase):
     input_type = YinXiangClipper_Type
 
-    def __init__(self, html_content):
-        super().__init__(html_content)
+    def __init__(self, html_content, import_stat):
+        super().__init__(html_content, import_stat)
 
     def process(self):
         soup = BeautifulSoup(self.html_content, 'html.parser')
         self.convert_properties(soup)
 
         content_tags = soup.body
         if not content_tags:
-            logger.warning("No content found")
-            return
+            logger.error("No content found")
+            raise Exception("No content found")
+
+        self.import_stat.add_text(content_tags.get_text())
         self.convert_children(content_tags)  # Assesume only one body tag
 
         return YinXiangClipper_Type
 
     def convert_properties(self, soup):
         properties = {"title": "Unknown"}
         title_tag = soup.select_one('head > title')
@@ -55,16 +57,14 @@
             return Block.HEADING.value
         elif tag_name == 'hr':
             return Block.DIVIDER.value
         elif tag_name == 'ol':
             return Block.NUMBERED_LIST.value
         elif tag_name == 'ul':
             return Block.BULLETED_LIST.value
-        elif tag_name == 'p':
-            return Block.PARAGRAPH.value
         elif element.name == 'pre' and element.code:
             return Block.CODE.value
         elif self._check_is_block(element):
             return Block.QUOTE.value
 
         return Block.FAIL.value
 
@@ -79,16 +79,25 @@
             block_type = self.get_block_type(element)
             if hasattr(self, f"convert_{block_type}"):
                 converter = getattr(self, f"convert_{block_type}")
                 block = converter(element)
                 if block:
                     self.children.extend([block] if not isinstance(block, list) else block)
                     processed_tags.add(id(element))
-            else:
-                logger.warning(f"Unknown cnvert {element}, {block_type}")
+        unprocessed_tags = set()
+        for element in soup.descendants:
+            if not isinstance(element, NavigableString) or id(element) in processed_tags:
+                continue
+            if any(id(ancestor) in processed_tags for ancestor in element.parents):
+                continue
+            unprocessed_tags.add(element)
+
+        for unprocessed_tag in unprocessed_tags:
+            logger.warning(f"Unknown tag {unprocessed_tag.name}, {self.get_block_type(unprocessed_tag)}")
+            self.import_stat.add_skip_tag(unprocessed_tag.get_text())
         return
 
     # <pre><code><code>line number</code>... code content ...</code></pre>
     def convert_code(self, soup):
         json_obj = {
             "object": "block",
             "type": "code",
```

### Comparing `html2notion-0.1.7/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.1.8/html2notion/translate/html2json_yinxiang.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from bs4 import BeautifulSoup, NavigableString, Tag
+from bs4 import BeautifulSoup, Tag
 from ..utils import logger
 from ..translate.html2json_base import Html2JsonBase, Block
 from ..utils.timeutil import DateStrToISO8601
 
 YinXiang_Type = "yinxiang"
 
 
 class Html2JsonYinXiang(Html2JsonBase):
     input_type = YinXiang_Type
 
-    def __init__(self, html_content):
-        super().__init__(html_content)
+    def __init__(self, html_content, import_stat):
+        super().__init__(html_content, import_stat)
 
     def process(self):
         soup = BeautifulSoup(self.html_content, 'html.parser')
         self.convert_children(soup)
         self.convert_properties(soup)
         return YinXiang_Type
 
@@ -39,26 +39,29 @@
         self.properties = self.generate_properties(**properties)
         return
 
     def convert_children(self, soup):
         content_tags = soup.find_all('body', recursive=True)
         if not content_tags:
             logger.warning("No content found")
-            return
+            raise Exception("No content found")
 
+        self.import_stat.add_text(content_tags[0].get_text())
         for child in content_tags[0].children:
             block_type = self.get_block_type(child)
+            # Computer all text len in html
             logger.debug(f'Support tag {child} with style {block_type}')
-            converter = getattr(self, f"convert_{block_type}")
-            if converter:
+            if hasattr(self, f"convert_{block_type}"):
+                converter = getattr(self, f"convert_{block_type}")
                 block = converter(child)
                 if block:
                     self.children.extend([block] if not isinstance(block, list) else block)
             else:
-                logger.warning(f"Unknown block type: {block_type}")
+                self.import_stat.add_skip_tag(child.get_text())
+                logger.warning(f"Unknown tag : {child}")
     
     def convert_code(self, soup):
         json_obj = {
             "object": "block",
             "type": "code",
             "code": {
                 "rich_text": [],
@@ -70,15 +73,15 @@
         children_list = list(soup.children) if isinstance(soup, Tag) else [soup]
         for index, child in enumerate(children_list):
             is_last_child = index == len(children_list) - 1
             text_obj = self.generate_inline_obj(child)
             if text_obj:
                 rich_text.extend(text_obj)
             if not is_last_child:
-                rich_text.append(self.generate_text(plain_text='\n'))
+                rich_text.append(self.generate_text(plain_text='\n', stats_count=False))
         json_obj["code"]["rich_text"] = self.merge_rich_text(rich_text)
 
         style = soup.get('style', "") if soup.name else ""
         css_dict = {}
         if isinstance(style, str):
             style = ''.join(style.split())
             css_dict = {rule.split(':')[0].strip(): rule.split(':')[1].strip() for rule in style.split(';') if rule}
@@ -100,15 +103,15 @@
         children_list = list(soup.children)
         for index, child in enumerate(children_list):
             is_last_child = index == len(children_list) - 1
             text_obj = self.generate_inline_obj(child)
             if text_obj:
                 rich_text.extend(text_obj)
             if not is_last_child:
-                rich_text.append(self.generate_text(plain_text='\n'))
+                rich_text.append(self.generate_text(plain_text='\n', stats_count=False))
 
         # Merge tags has same anotions
         logger.debug(f'before merge: {rich_text}')
         json_obj["quote"]["rich_text"] = self.merge_rich_text(rich_text)
         return json_obj
 
     def convert_to_do(self, soup: Tag):
@@ -151,30 +154,31 @@
             return Block.BULLETED_LIST.value
         elif tag_name == 'p':
             return Block.PARAGRAPH.value
         elif tag_name in ('h1', 'h2', 'h3', 'h4', 'h5', 'h6'):
             return Block.HEADING.value
         elif tag_name == 'table' or self._check_is_table(single_tag):
             return Block.TABLE.value
-        if not style and tag_name == 'div':
-            return Block.PARAGRAPH.value
 
         css_dict = {}
         if style:
             # Remove all space such as \t \n in style
             style = ''.join(style.split())
             css_dict = {rule.split(':')[0].strip(): rule.split(
                 ':')[1].strip().lower() for rule in style.split(';') if rule}
         if css_dict.get('--en-blockquote', None) == 'true':
             return Block.QUOTE.value
         if css_dict.get('--en-codeblock', None) == 'true':
             return Block.CODE.value
         if css_dict.get('-en-codeblock', None) == 'true':
             return Block.CODE.value
-        
+
+        # Issue 5: <div style="orphans: 2; widows: 2">
+        if tag_name == 'div':
+            return Block.PARAGRAPH.value
         return Block.FAIL.value
 
     def _check_is_table(self, tag):
         if tag.name == "div":
             children = list(filter(lambda x: x != '\n', tag.contents))
             table_count = sum(1 for child in children if child.name == "table")
             div_br_count = sum(1 for child in children if child.name == "div" and len(
```

### Comparing `html2notion-0.1.7/html2notion/translate/notion_export.py` & `html2notion-0.1.8/html2notion/translate/notion_export.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/html2notion/translate/notion_import.py` & `html2notion-0.1.8/html2notion/translate/notion_import.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,51 +3,68 @@
 from aiohttp import ClientSession
 from pathlib import Path
 from notion_client import AsyncClient
 from notion_client.errors import RequestTimeoutError
 from tenacity import retry, stop_after_attempt, wait_exponential, retry_if_exception_type
 from ..utils import logger, test_prepare_conf, config, rate_limit
 from ..translate.html2json import html2json_process
+from ..translate.import_stats import ImportStats
 
 
 class NotionImporter:
     def __init__(self, session: ClientSession, notion_client):
         self.session = session
         self.notion_client = notion_client
+        self.import_stats = ImportStats()
 
     async def process_file(self, file_path: Path):
+        self.import_stats.set_filename(file_path)
+
         if not file_path.is_file():
+            self.import_stats.set_exception(Exception(f"{file_path} is not file"))
             logger.error(f"{file_path} is not a file.")
-            return
+            return "fail"
 
         with file_path.open() as f:
             content = f.read()
 
         logger.info(f"Process file {file_path}")
         if content == "main_hold":                  # local debug
             await asyncio.sleep(1)
             return "main_hold"
 
-        notion_data, html_type = html2json_process(file_path)
-        logger.info(f"path: {file_path}, html type: {html_type}")
-
-        create_result = await self.create_new_page(notion_data)
+        try:
+            notion_data, html_type = html2json_process(file_path, self.import_stats)
+        except Exception as e:
+            self.import_stats.set_exception(e)
+            logger.error(f"Error processing {file_path}: {str(e)}")
+            return "fail"
+
+        logger.info(f"Process path: {file_path}, html type: {html_type}, {self.import_stats.get_detail()}")
+        try:
+            create_result = await self.create_new_page(notion_data)
+        except Exception as e:
+            self.import_stats.set_exception(e)
+            logger.error(f"Error create notion page {file_path}: {str(e)}")
+            return "fail"
         logger.info(f"Create notion page: {create_result}")
         return "succ"
 
     # https://developers.notion.com/reference/request-limits
     # The rate limit for incoming requests per integration is an average of three requests per second. 
     # Doc of create page: https://developers.notion.com/reference/post-page
     @retry(stop=stop_after_attempt(5),
            wait=wait_exponential(multiplier=1, min=3, max=30),
            retry=retry_if_exception_type(RequestTimeoutError))
     async def create_new_page(self, notion_data):
         # logger.debug(f'Create new page: {notion_data["parent"]}, {notion_data["properties"]}')
         # body.children.length should be ≤ `100`,
         blocks = notion_data.get("children", [])
+        # logger.debug(f'Create new page: {notion_data["parent"]}, {notion_data["properties"]}, blocks: {blocks}')
+        
         limit_size = 100
         chunks = [blocks[i: i + limit_size] for i in range(0, len(blocks), limit_size)]
         if blocks:
             notion_data.pop("children")
         first_chunk = chunks[0] if chunks else []
         async with rate_limit:
             created_page = await self.notion_client.pages.create(**notion_data, children=first_chunk)
```

### Comparing `html2notion-0.1.7/html2notion/utils/load_config.py` & `html2notion-0.1.8/html2notion/utils/load_config.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/html2notion/utils/log.py` & `html2notion-0.1.8/html2notion/utils/log.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/html2notion.egg-info/PKG-INFO` & `html2notion-0.1.8/html2notion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.7
+Version: 0.1.8
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.7/html2notion.egg-info/SOURCES.txt` & `html2notion-0.1.8/html2notion.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 html2notion/translate/batch_import.py
 html2notion/translate/cos_uploader.py
 html2notion/translate/html2json.py
 html2notion/translate/html2json_base.py
 html2notion/translate/html2json_clipper.py
 html2notion/translate/html2json_default.py
 html2notion/translate/html2json_yinxiang.py
+html2notion/translate/import_stats.py
 html2notion/translate/notion_export.py
 html2notion/translate/notion_import.py
 html2notion/utils/__init__.py
 html2notion/utils/load_config.py
 html2notion/utils/log.py
 html2notion/utils/timeutil.py
 tests/test_batchimport.py
```

### Comparing `html2notion-0.1.7/setup.cfg` & `html2notion-0.1.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.7
+version = 0.1.8
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
```

### Comparing `html2notion-0.1.7/tests/test_batchimport.py` & `html2notion-0.1.8/tests/test_batchimport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/tests/test_cosupload.py` & `html2notion-0.1.8/tests/test_cosupload.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/tests/test_notionexport.py` & `html2notion-0.1.8/tests/test_notionexport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.7/tests/test_reqlimit.py` & `html2notion-0.1.8/tests/test_reqlimit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
 import os
 from html2notion.translate.html2json_yinxiang import Html2JsonYinXiang
+from html2notion.translate.import_stats import ImportStats
+
 
 paragram_rich_content = f'<div>{"Some words" * 400} more words</div>'
 block_max_conent = "Some words" * 200
 paragram_rich_block = [
     {
         "object": "block",
         "type": "paragraph",
@@ -45,15 +47,16 @@
 
     html_jsons = {
         paragram_rich_content: paragram_rich_block,
     }
 
     for html_content in html_jsons:
         body_content = '<body>' + html_content + '</body>'
-        yinxiang = Html2JsonYinXiang(body_content)
+        import_stats = ImportStats()
+        yinxiang = Html2JsonYinXiang(body_content, import_stats)
         yinxiang.process()
         json_obj = yinxiang.children
         # print(json.dumps(json_obj, indent=4))
         assert json_obj == html_jsons[html_content]
 
 
 if __name__ == '__main__':
```

### Comparing `html2notion-0.1.7/tests/test_yinxiang.py` & `html2notion-0.1.8/tests/test_yinxiang.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import os
 from html2notion.translate.html2json_yinxiang import Html2JsonYinXiang
+from html2notion.translate.import_stats import ImportStats
 
 link_content = "<div><a href='https://google.com'>Google</a></div>"
 link_block = [
     {
         "object": "block",
         "type": "paragraph",
         "paragraph": {
@@ -279,14 +280,39 @@
                     }
                 }
             ]
         }
     }
 ]
 
+paragram_br_content = """<div>su<div><br/></div>dd if=/sdcard/twrp.img of=/dev/block/platform/msm_sdcc.1/by-name/recovery<div><br/></div></div>"""
+paragram_br_block = [
+    {
+        "object": "block",
+        "type": "paragraph",
+        "paragraph": {
+            "rich_text": [
+                {
+                    "plain_text": "su\n",
+                    "text": {
+                        "content": "su\n"
+                    },
+                    "type": "text"
+                },
+                {
+                    "plain_text": "dd if=/sdcard/twrp.img of=/dev/block/platform/msm_sdcc.1/by-name/recovery\n",
+                    "text": {
+                        "content": "dd if=/sdcard/twrp.img of=/dev/block/platform/msm_sdcc.1/by-name/recovery\n"
+                    },
+                    "type": "text"
+                }
+            ]
+        }
+    }
+]
 
 heading_content = '<h1>Heading 1</h1><h2>Heading 2</h2><h3>Heading 3</h3><h4>Heading 4</h4><h5>Heading 5</h5><h6>Heading 6</h6>'
 heading_block = [
     {
         "object": "block",
         "type": "heading_1",
         "heading_1": {
@@ -814,14 +840,15 @@
 def test_convert():
     if 'GITHUB_ACTIONS' not in os.environ:
         from html2notion.utils import test_prepare_conf, logger
         test_prepare_conf()
         logger.info("prepare_conf_fixture")
 
     html_jsons = {
+        paragram_br_content: paragram_br_block,
         link_content: link_block,
         order_list_content: ordered_list_block,
         nested_bold_content: nested_bold_block,
         paragram_rich_content: paragram_rich_block,
         heading_content: heading_block,
         code_content: code_block,
         code_paragraph_content: code_paragraph_block,
@@ -832,15 +859,16 @@
         to_do_normal_content: to_do_block,
         divider_content: divider_block,
         quote_content: quote_block,
     }
 
     for html_content in html_jsons:
         body_content = '<body>' + html_content + '</body>'
-        yinxiang = Html2JsonYinXiang(body_content)
+        import_stats = ImportStats()
+        yinxiang = Html2JsonYinXiang(body_content, import_stats)
         yinxiang.process()
         json_obj = yinxiang.children
         # print(json.dumps(json_obj, indent=4))
         assert json_obj == html_jsons[html_content]
 
 
 if __name__ == '__main__':
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 import json import os from html2notion.translate.html2json_yinxiang import
-Html2JsonYinXiang link_content = "
+Html2JsonYinXiang from html2notion.translate.import_stats import ImportStats
+link_content = "
 Google
 " link_block = [ { "object": "block", "type": "paragraph", "paragraph":
 { "rich_text": [ { "href": "https://google.com", "plain_text": "Google",
 "text": { "link": { "url": "https://google.com" }, "content": "Google" },
 "type": "text" } ] } } ] order_list_content = '
    1. first
    2. second
@@ -47,15 +48,25 @@
 "type": "text" }, { "plain_text": "Bold text", "text": { "content": "Bold text"
 }, "type": "text", "annotations": { "bold": True } }, { "plain_text": ",",
 "text": { "content": "," }, "type": "text" }, { "plain_text": "Strikethrough
 text", "text": { "content": "Strikethrough text" }, "type": "text",
 "annotations": { "strikethrough": True } }, { "plain_text": ",", "text":
 { "content": "," }, "type": "text" }, { "plain_text": "Italic text", "text":
 { "content": "Italic text" }, "type": "text", "annotations": { "italic": True }
-} ] } } ] heading_content = '
+} ] } } ] paragram_br_content = """
+su
+
+dd if=/sdcard/twrp.img of=/dev/block/platform/msm_sdcc.1/by-name/recovery
+
+""" paragram_br_block = [ { "object": "block", "type": "paragraph",
+"paragraph": { "rich_text": [ { "plain_text": "su\n", "text": { "content":
+"su\n" }, "type": "text" }, { "plain_text": "dd if=/sdcard/twrp.img of=/dev/
+block/platform/msm_sdcc.1/by-name/recovery\n", "text": { "content": "dd if=/
+sdcard/twrp.img of=/dev/block/platform/msm_sdcc.1/by-name/recovery\n" },
+"type": "text" } ] } } ] heading_content = '
 ****** Heading 1 ******
 ***** Heading 2 *****
 **** Heading 3 ****
 *** Heading 4 ***
 ** Heading 5 **
 * Heading 6 *
 ' heading_block = [ { "object": "block", "type": "heading_1", "heading_1":
@@ -209,19 +220,21 @@
 with an instruction.\u00a0" }, "type": "text" }, { "plain_text": "Submit this
 prompt", "text": { "content": "Submit this prompt" }, "type": "text",
 "annotations": { "bold": True } }, { "plain_text": "\u00a0to generate your
 first completion.", "text": { "content": "\u00a0to generate your first
 completion." }, "type": "text" } ] } } ] def test_convert(): if
 'GITHUB_ACTIONS' not in os.environ: from html2notion.utils import
 test_prepare_conf, logger test_prepare_conf() logger.info
-("prepare_conf_fixture") html_jsons = { link_content: link_block,
-order_list_content: ordered_list_block, nested_bold_content: nested_bold_block,
-paragram_rich_content: paragram_rich_block, heading_content: heading_block,
-code_content: code_block, code_paragraph_content: code_paragraph_block,
-language_code_content: language_code_block, table_content: table_block,
-super_note_table_content: table_block, to_do_content: to_do_block,
-to_do_normal_content: to_do_block, divider_content: divider_block,
-quote_content: quote_block, } for html_content in html_jsons: body_content = '
+("prepare_conf_fixture") html_jsons = { paragram_br_content: paragram_br_block,
+link_content: link_block, order_list_content: ordered_list_block,
+nested_bold_content: nested_bold_block, paragram_rich_content:
+paragram_rich_block, heading_content: heading_block, code_content: code_block,
+code_paragraph_content: code_paragraph_block, language_code_content:
+language_code_block, table_content: table_block, super_note_table_content:
+table_block, to_do_content: to_do_block, to_do_normal_content: to_do_block,
+divider_content: divider_block, quote_content: quote_block, } for html_content
+in html_jsons: body_content = '
 ' + html_content + '
-' yinxiang = Html2JsonYinXiang(body_content) yinxiang.process() json_obj =
-yinxiang.children # print(json.dumps(json_obj, indent=4)) assert json_obj ==
-html_jsons[html_content] if __name__ == '__main__': test_convert()
+' import_stats = ImportStats() yinxiang = Html2JsonYinXiang(body_content,
+import_stats) yinxiang.process() json_obj = yinxiang.children # print
+(json.dumps(json_obj, indent=4)) assert json_obj == html_jsons[html_content] if
+__name__ == '__main__': test_convert()
```

