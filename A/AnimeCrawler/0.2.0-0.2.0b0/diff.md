# Comparing `tmp/AnimeCrawler-0.2.0.tar.gz` & `tmp/AnimeCrawler-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnimeCrawler-0.2.0.tar", last modified: Sat May  6 14:39:52 2023, max compression
+gzip compressed data, was "AnimeCrawler-0.2.0b0.tar", last modified: Wed May 10 12:27:12 2023, max compression
```

## Comparing `AnimeCrawler-0.2.0.tar` & `AnimeCrawler-0.2.0b0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.544256 AnimeCrawler-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.153479 AnimeCrawler-0.2.0/AnimeCrawler/
--rw-rw-rw-   0        0        0      388 2023-05-06 14:06:08.000000 AnimeCrawler-0.2.0/AnimeCrawler/__init__.py
--rw-rw-rw-   0        0        0     2682 2023-05-06 13:57:08.000000 AnimeCrawler-0.2.0/AnimeCrawler/base_spider.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.392346 AnimeCrawler-0.2.0/AnimeCrawler/command/
--rw-rw-rw-   0        0        0      117 2023-05-03 05:18:04.000000 AnimeCrawler-0.2.0/AnimeCrawler/command/__init__.py
--rw-rw-rw-   0        0        0     3250 2023-05-06 14:05:51.000000 AnimeCrawler-0.2.0/AnimeCrawler/command/run.py
--rw-rw-rw-   0        0        0      356 2023-05-03 05:07:40.000000 AnimeCrawler-0.2.0/AnimeCrawler/log.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.493285 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/
--rw-rw-rw-   0        0        0      286 2023-05-03 09:50:27.000000 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/__init__.py
--rw-rw-rw-   0        0        0     2396 2023-05-06 13:55:26.000000 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/downloader.py
--rw-rw-rw-   0        0        0     2084 2023-05-06 13:51:37.000000 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/searcher.py
--rw-rw-rw-   0        0        0     4138 2023-05-06 13:58:10.000000 AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/spider.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.499281 AnimeCrawler-0.2.0/AnimeCrawler/utils/
--rw-rw-rw-   0        0        0      128 2023-05-03 15:03:17.000000 AnimeCrawler-0.2.0/AnimeCrawler/utils/__init__.py
--rw-rw-rw-   0        0        0     1403 2023-05-03 02:47:10.000000 AnimeCrawler-0.2.0/AnimeCrawler/utils/decode.py
--rw-rw-rw-   0        0        0     3017 2023-05-03 15:13:47.000000 AnimeCrawler-0.2.0/AnimeCrawler/utils/file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.348369 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/
--rw-rw-rw-   0        0        0     3268 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      602 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 14:39:51.000000 AnimeCrawler-0.2.0/AnimeCrawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3268 2023-05-06 14:39:52.505278 AnimeCrawler-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2819 2023-05-06 14:03:37.000000 AnimeCrawler-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 14:39:52.545255 AnimeCrawler-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      882 2023-05-06 14:21:26.000000 AnimeCrawler-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:39:52.503279 AnimeCrawler-0.2.0/test/
--rw-rw-rw-   0        0        0      264 2023-05-03 13:36:29.000000 AnimeCrawler-0.2.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.937047 AnimeCrawler-0.2.0b0/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.864089 AnimeCrawler-0.2.0b0/AnimeCrawler/
+-rw-rw-rw-   0        0        0      389 2023-05-10 12:26:57.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-05-10 11:04:59.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/__main__.py
+-rw-rw-rw-   0        0        0     2690 2023-05-10 12:08:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/base_spider.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.899071 AnimeCrawler-0.2.0b0/AnimeCrawler/command/
+-rw-rw-rw-   0        0        0      117 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/command/__init__.py
+-rw-rw-rw-   0        0        0     3250 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/command/run.py
+-rw-rw-rw-   0        0        0      521 2023-05-10 11:07:22.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/log.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.917069 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/
+-rw-rw-rw-   0        0        0      286 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/__init__.py
+-rw-rw-rw-   0        0        0     2396 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/downloader.py
+-rw-rw-rw-   0        0        0     2129 2023-05-10 12:07:35.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/searcher.py
+-rw-rw-rw-   0        0        0     4138 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/spider.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.932050 AnimeCrawler-0.2.0b0/AnimeCrawler/utils/
+-rw-rw-rw-   0        0        0      128 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1403 2023-05-03 02:47:10.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/utils/decode.py
+-rw-rw-rw-   0        0        0     3017 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/AnimeCrawler/utils/file.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.883078 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/
+-rw-rw-rw-   0        0        0     3270 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-10 12:27:12.000000 AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2023-04-15 13:28:24.000000 AnimeCrawler-0.2.0b0/LICENSE
+-rw-rw-rw-   0        0        0     3270 2023-05-10 12:27:12.936047 AnimeCrawler-0.2.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2819 2023-05-06 14:46:25.000000 AnimeCrawler-0.2.0b0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:27:12.938046 AnimeCrawler-0.2.0b0/setup.cfg
+-rw-rw-rw-   0        0        0      883 2023-05-10 12:26:46.000000 AnimeCrawler-0.2.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:27:12.934049 AnimeCrawler-0.2.0b0/test/
+-rw-rw-rw-   0        0        0      264 2023-05-03 13:36:29.000000 AnimeCrawler-0.2.0b0/test/test.py
```

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler/base_spider.py` & `AnimeCrawler-0.2.0b0/AnimeCrawler/base_spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         ValueError: 未定义domain时报错
         ValueError: 未定义downloader时报错
 
     Returns:
         cls: 为了链式调用ruia.Spider.start()
     '''
 
-    logger = get_logger('Spider')
+    logger = get_logger('Spider', 'INFO')
 
     def __init__(self, *args, **spider_kwargs) -> None:
         super().__init__(*args, **spider_kwargs)
         if not hasattr(self, 'domain'):
             raise ValueError(f'{self.__class__.__name__} 未定义domain属性')
         elif not hasattr(self, 'downloader'):
             raise ValueError(f'{self.__class__.__name__} 未定义downloader下载器')
```

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler/command/run.py` & `AnimeCrawler-0.2.0b0/AnimeCrawler/command/run.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/downloader.py` & `AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/downloader.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/searcher.py` & `AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/searcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,28 @@
         many=True,
     )
 
 
 class Searcher(BaseSpider):
     session = None
     downloader = None
-    domain = 'https://www.mhyyy.com'
+    domain = 'https://www.mh620.com'
     # logger = get_logger('Searcher')
 
     @classmethod
     def init(cls, anime_title) -> BaseSpider:
         cls.start_urls = [
             cls.urljoin(cls, cls.domain, f'/search.html?wd={anime_title}')
         ]
         return super().init()
 
     async def select_anime(self, animes) -> None:
         answer = int(input('Which anime do you want to download? >>> '))
+        if answer <= 0:
+            return
         anime = animes[answer - 1][1]
         title, url = anime[0].replace(' ', '_'), self.domain + anime[1]
         print(
             f'\nDownload Command:\nAnimeCrawler download -t {title} -u {url} --del_ts'
         )
 
     async def pretty_print(self, animes) -> None:
```

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler/mhyyy/spider.py` & `AnimeCrawler-0.2.0b0/AnimeCrawler/mhyyy/spider.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler/utils/decode.py` & `AnimeCrawler-0.2.0b0/AnimeCrawler/utils/decode.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler/utils/file.py` & `AnimeCrawler-0.2.0b0/AnimeCrawler/utils/file.py`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler.egg-info/PKG-INFO` & `AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.2.0
+Version: 0.2.0b0
 Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AnimeCrawler-0.2.0/AnimeCrawler.egg-info/SOURCES.txt` & `AnimeCrawler-0.2.0b0/AnimeCrawler.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 AnimeCrawler/__init__.py
+AnimeCrawler/__main__.py
 AnimeCrawler/base_spider.py
 AnimeCrawler/log.py
 AnimeCrawler.egg-info/PKG-INFO
 AnimeCrawler.egg-info/SOURCES.txt
 AnimeCrawler.egg-info/dependency_links.txt
 AnimeCrawler.egg-info/entry_points.txt
 AnimeCrawler.egg-info/requires.txt
```

### Comparing `AnimeCrawler-0.2.0/LICENSE` & `AnimeCrawler-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0/PKG-INFO` & `AnimeCrawler-0.2.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimeCrawler
-Version: 0.2.0
+Version: 0.2.0b0
 Summary: 一个可免费下载动漫的爬虫
 Home-page: https://github.com/Senvlin/AnimeCrawler
 Author: Senvlin
 Author-email: 2994515402@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AnimeCrawler-0.2.0/README.md` & `AnimeCrawler-0.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `AnimeCrawler-0.2.0/setup.py` & `AnimeCrawler-0.2.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AnimeCrawler",
-    version="v0.2.0",
+    version="v0.2.0b",
     author="Senvlin",
     author_email="2994515402@qq.com",
     description="一个可免费下载动漫的爬虫",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Senvlin/AnimeCrawler",
     packages=setuptools.find_packages(),
```

