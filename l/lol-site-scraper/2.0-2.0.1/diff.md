# Comparing `tmp/lol-site-scraper-2.0.tar.gz` & `tmp/lol-site-scraper-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lol-site-scraper-2.0.tar", last modified: Mon May  8 17:16:02 2023, max compression
+gzip compressed data, was "lol-site-scraper-2.0.1.tar", last modified: Wed May 10 15:10:29 2023, max compression
```

## Comparing `lol-site-scraper-2.0.tar` & `lol-site-scraper-2.0.1.tar`

### file list

```diff
@@ -1,73 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 17:16:02.408765 lol-site-scraper-2.0/
--rw-rw-rw-   0        0        0     1092 2022-08-30 20:23:53.000000 lol-site-scraper-2.0/LICENSE
--rw-rw-rw-   0        0        0     8841 2023-05-08 17:16:02.408045 lol-site-scraper-2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8534 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 17:16:02.331054 lol-site-scraper-2.0/lol_site_scraper.egg-info/
--rw-rw-rw-   0        0        0     8841 2023-05-08 17:16:02.000000 lol-site-scraper-2.0/lol_site_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1748 2023-05-08 17:16:02.000000 lol-site-scraper-2.0/lol_site_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 17:16:02.000000 lol-site-scraper-2.0/lol_site_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-08 17:16:02.000000 lol-site-scraper-2.0/lol_site_scraper.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-05-08 17:16:02.000000 lol-site-scraper-2.0/lol_site_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-08 17:16:02.000000 lol-site-scraper-2.0/lol_site_scraper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 17:16:02.337971 lol-site-scraper-2.0/lols/
--rw-rw-rw-   0        0        0       98 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/__init__.py
--rw-rw-rw-   0        0        0    10849 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/__main__.py
--rw-rw-rw-   0        0        0     1135 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/config.py
--rw-rw-rw-   0        0        0      720 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:16:02.343973 lol-site-scraper-2.0/lols/http/
--rw-rw-rw-   0        0        0      848 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/http/__init__.py
--rw-rw-rw-   0        0        0     2404 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/http/client.py
--rw-rw-rw-   0        0        0     2269 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/http/downloader.py
--rw-rw-rw-   0        0        0      386 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/http/headers.py
--rw-rw-rw-   0        0        0    15468 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/http/m3u8_downloader.py
--rw-rw-rw-   0        0        0     2730 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/http/models.py
--rw-rw-rw-   0        0        0     1520 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/http/types.py
--rw-rw-rw-   0        0        0     2277 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/path_creator.py
-drwxrwxrwx   0        0        0        0 2023-05-08 17:16:02.406047 lol-site-scraper-2.0/lols/scrapers/
--rw-rw-rw-   0        0        0     2099 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/__init__.py
--rw-rw-rw-   0        0        0     5905 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/_scraper_base.py
--rw-rw-rw-   0        0        0     1939 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/_scraper_template.py
--rw-rw-rw-   0        0        0     1964 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/all_scrapers.py
--rw-rw-rw-   0        0        0     1860 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/anonfiles.py
--rw-rw-rw-   0        0        0     4198 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/bunkr.py
--rw-rw-rw-   0        0        0     2907 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/cyberdrop.py
--rw-rw-rw-   0        0        0     2218 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/erome.py
--rw-rw-rw-   0        0        0     4056 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/forum_nudostar.py
--rw-rw-rw-   0        0        0     6328 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/forum_nudostar_auth.py
--rw-rw-rw-   0        0        0     5649 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/forum_socialmediagirls.py
--rw-rw-rw-   0        0        0     5880 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/forum_socialmediagirls_auth.py
--rw-rw-rw-   0        0        0     4179 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/forum_thotsbay.py
--rw-rw-rw-   0        0        0     6266 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/forum_thotsbay_auth.py
--rw-rw-rw-   0        0        0     4573 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/gofile.py
--rw-rw-rw-   0        0        0     2176 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/gofile_auth.py
--rw-rw-rw-   0        0        0     2741 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/hexupload.py
--rw-rw-rw-   0        0        0     7281 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/highload.py
--rw-rw-rw-   0        0        0     4729 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/ibb.py
--rw-rw-rw-   0        0        0     1483 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/imagebam.py
--rw-rw-rw-   0        0        0     1391 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/imagehaha.py
--rw-rw-rw-   0        0        0     1830 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/imagetwist.py
--rw-rw-rw-   0        0        0     2318 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/imgbox.py
--rw-rw-rw-   0        0        0     3460 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/jpgchurch.py
--rw-rw-rw-   0        0        0     5347 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/leakedmodelsforum.py
--rw-rw-rw-   0        0        0     6360 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/leakedmodelsforum_auth.py
--rw-rw-rw-   0        0        0     2625 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/lovefap.py
--rw-rw-rw-   0        0        0     2382 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/mega.py
--rw-rw-rw-   0        0        0     2121 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/pixeldrain.py
--rw-rw-rw-   0        0        0     2017 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/pixhost.py
--rw-rw-rw-   0        0        0     2591 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/pixl.py
--rw-rw-rw-   0        0        0     2270 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/planetsuzy.py
--rw-rw-rw-   0        0        0       88 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/saint.py
--rw-rw-rw-   0        0        0      244 2022-09-09 23:38:57.000000 lol-site-scraper-2.0/lols/scrapers/sbspeed.py
--rw-rw-rw-   0        0        0     1644 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/sendvid.py
--rw-rw-rw-   0        0        0     1909 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/simpcity.py
--rw-rw-rw-   0        0        0     6305 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/simpcity_auth.py
--rw-rw-rw-   0        0        0     1512 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/skygallery.py
--rw-rw-rw-   0        0        0     3738 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/streamlare.py
--rw-rw-rw-   0        0        0     3996 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/streamtape.py
--rw-rw-rw-   0        0        0     2507 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/voe.py
--rw-rw-rw-   0        0        0     1810 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/scrapers/xvideos.py
--rw-rw-rw-   0        0        0     6435 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/settings.py
--rw-rw-rw-   0        0        0     4336 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/utils.py
--rw-rw-rw-   0        0        0       21 2023-05-08 14:43:22.000000 lol-site-scraper-2.0/lols/version.py
--rw-rw-rw-   0        0        0       42 2023-05-08 17:16:02.408765 lol-site-scraper-2.0/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-08 17:15:46.000000 lol-site-scraper-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:10:29.198938 lol-site-scraper-2.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     8876 2023-05-10 15:10:29.198938 lol-site-scraper-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8546 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 15:10:29.167685 lol-site-scraper-2.0.1/lol_site_scraper.egg-info/
+-rw-rw-rw-   0        0        0     8876 2023-05-10 15:10:29.000000 lol-site-scraper-2.0.1/lol_site_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1723 2023-05-10 15:10:29.000000 lol-site-scraper-2.0.1/lol_site_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 15:10:29.000000 lol-site-scraper-2.0.1/lol_site_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-10 15:10:29.000000 lol-site-scraper-2.0.1/lol_site_scraper.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-05-10 15:10:29.000000 lol-site-scraper-2.0.1/lol_site_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-10 15:10:29.000000 lol-site-scraper-2.0.1/lol_site_scraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 15:10:29.167685 lol-site-scraper-2.0.1/lols/
+-rw-rw-rw-   0        0        0       98 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/__init__.py
+-rw-rw-rw-   0        0        0    10849 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/__main__.py
+-rw-rw-rw-   0        0        0     1135 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/config.py
+-rw-rw-rw-   0        0        0      720 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:10:29.183312 lol-site-scraper-2.0.1/lols/http/
+-rw-rw-rw-   0        0        0      848 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/http/__init__.py
+-rw-rw-rw-   0        0        0     3052 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/http/client.py
+-rw-rw-rw-   0        0        0     2269 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/http/downloader.py
+-rw-rw-rw-   0        0        0      386 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/http/headers.py
+-rw-rw-rw-   0        0        0    15468 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/http/m3u8_downloader.py
+-rw-rw-rw-   0        0        0     2730 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/http/models.py
+-rw-rw-rw-   0        0        0     1520 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/http/types.py
+-rw-rw-rw-   0        0        0     2277 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/path_creator.py
+drwxrwxrwx   0        0        0        0 2023-05-10 15:10:29.198938 lol-site-scraper-2.0.1/lols/scrapers/
+-rw-rw-rw-   0        0        0     2099 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/__init__.py
+-rw-rw-rw-   0        0        0     5905 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/_scraper_base.py
+-rw-rw-rw-   0        0        0     1939 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/_scraper_template.py
+-rw-rw-rw-   0        0        0     1964 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/all_scrapers.py
+-rw-rw-rw-   0        0        0     1860 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/anonfiles.py
+-rw-rw-rw-   0        0        0     4198 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/bunkr.py
+-rw-rw-rw-   0        0        0     2907 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/cyberdrop.py
+-rw-rw-rw-   0        0        0     2218 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/erome.py
+-rw-rw-rw-   0        0        0     4056 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/forum_nudostar.py
+-rw-rw-rw-   0        0        0     6328 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/forum_nudostar_auth.py
+-rw-rw-rw-   0        0        0     5649 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/forum_socialmediagirls.py
+-rw-rw-rw-   0        0        0     5880 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/forum_socialmediagirls_auth.py
+-rw-rw-rw-   0        0        0     4179 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/forum_thotsbay.py
+-rw-rw-rw-   0        0        0     6266 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/forum_thotsbay_auth.py
+-rw-rw-rw-   0        0        0     4573 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/gofile.py
+-rw-rw-rw-   0        0        0     2176 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/gofile_auth.py
+-rw-rw-rw-   0        0        0     2741 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/hexupload.py
+-rw-rw-rw-   0        0        0     7281 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/highload.py
+-rw-rw-rw-   0        0        0     4729 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/ibb.py
+-rw-rw-rw-   0        0        0     1483 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/imagebam.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/imagehaha.py
+-rw-rw-rw-   0        0        0     1830 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/imagetwist.py
+-rw-rw-rw-   0        0        0     2318 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/imgbox.py
+-rw-rw-rw-   0        0        0     3460 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/jpgchurch.py
+-rw-rw-rw-   0        0        0     5347 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/leakedmodelsforum.py
+-rw-rw-rw-   0        0        0     6360 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/leakedmodelsforum_auth.py
+-rw-rw-rw-   0        0        0     2625 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/lovefap.py
+-rw-rw-rw-   0        0        0     2382 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/mega.py
+-rw-rw-rw-   0        0        0     2121 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/pixeldrain.py
+-rw-rw-rw-   0        0        0     2017 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/pixhost.py
+-rw-rw-rw-   0        0        0     2591 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/pixl.py
+-rw-rw-rw-   0        0        0     2270 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/planetsuzy.py
+-rw-rw-rw-   0        0        0       88 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/saint.py
+-rw-rw-rw-   0        0        0     1644 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/sendvid.py
+-rw-rw-rw-   0        0        0     1909 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/simpcity.py
+-rw-rw-rw-   0        0        0     6305 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/simpcity_auth.py
+-rw-rw-rw-   0        0        0     1512 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/skygallery.py
+-rw-rw-rw-   0        0        0     3738 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/streamlare.py
+-rw-rw-rw-   0        0        0     3996 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/streamtape.py
+-rw-rw-rw-   0        0        0     2507 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/voe.py
+-rw-rw-rw-   0        0        0     1810 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/scrapers/xvideos.py
+-rw-rw-rw-   0        0        0     6435 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/settings.py
+-rw-rw-rw-   0        0        0     4336 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/utils.py
+-rw-rw-rw-   0        0        0       23 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/lols/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-10 15:10:29.198938 lol-site-scraper-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-10 15:08:44.000000 lol-site-scraper-2.0.1/setup.py
```

### Comparing `lol-site-scraper-2.0/LICENSE` & `lol-site-scraper-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/PKG-INFO` & `lol-site-scraper-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: lol-site-scraper
-Version: 2.0
+Version: 2.0.1
 Summary: Bulk hosting sites scraper/downloader
 Home-page: https://github.com/vladimirpolak/lols
 Author: Vladimír Polák
 Author-email: vladimirpolak2@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 style="text-align: center;">Lols</h1>
 
 <!-- ABOUT THE PROJECT -->
 ## About
@@ -28,15 +29,15 @@
 you can incorporate it into your own python scripts as an external library.
 
 ### Installation
 
 1. Download and install latest [python](https://www.python.org/downloads/).
 2. In command line run:
    ```sh
-   pip install lols
+   pip install lol-site-scraper
    ```
 
 ## Usage
 ### Command Line Application
 
 1. Navigate to the folder where you want scraper to be downloading files.
 Bare in mind Lols create separate subfolder for each scrape.
@@ -213,7 +214,8 @@
 ## Contact
 
 Vladimír Polák - vladimirpolak2@gmail.com - Dio#7865
 
 Project Link: [https://github.com/vladimirpolak/lols](https://github.com/vladimirpolak/lols)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
+
```

#### html2text {}

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 2.1 Name: lol-site-scraper Version: 2.0 Summary: Bulk hosting
-sites scraper/downloader Home-page: https://github.com/vladimirpolak/lols
-Author: VladimÃ­r PolÃ¡k Author-email: vladimirpolak2@gmail.com License: MIT
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: lol-site-scraper Version: 2.0.1 Summary: Bulk
+hosting sites scraper/downloader Home-page: https://github.com/vladimirpolak/
+lols Author: VladimÃ­r PolÃ¡k Author-email: vladimirpolak2@gmail.com License:
+MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-File:
+LICENSE
 ****** Lols ******
  ## About Goal of this project is to have Bulk downloader/Content scraper
 capable of scraping content from multiple hosting sites/forums. Simple premise:
 user inputs a page url and scraper downloads it's contents.  ## Supported sites
 View supported sites and their corresponding codenames [here](docs/
 supported_sites.txt)  ## Getting Started You can use Lols as either a command
 line application or you can incorporate it into your own python scripts as an
 external library. ### Installation 1. Download and install latest [python]
 (https://www.python.org/downloads/). 2. In command line run: ```sh pip install
-lols ``` ## Usage ### Command Line Application 1. Navigate to the folder where
-you want scraper to be downloading files. Bare in mind Lols create separate
-subfolder for each scrape. 2. Basic usage syntax is as follows: ```sh lols
-[output_directory] [url] [options] ``` _Learn all options in Command Line App
-Options section or with help dialogue:_ ```sh lols --help ``` ### Library You
-can use Lols in your own custom script and take advantage of all the prewritten
-extractors. Once you pip-installed Lols in either global interpreter or the
-virtual evniroment you set up you can use the library as follows. ```python
-from lols import LolsClient, Item from typing import List url = "www.url.you/
-want-to-scrape" # Initiate client client = LolsClient() # Scrape URL items:
-List[Item] = client.scrape(url=url) ``` To disable specific extractor for
-whatever reason be it buggy servers or your disinterest initiate the client
-like so: ```python client = LolsClient( scrapers_to_disable=['bunkr'] # Option
-accepts list of codenames in string format ) ``` Or you can specify the only
-Extractor/s to use: ```python client = LolsClient( enabled_extractors=['bunkr']
-# Option accepts list of codenames in string format ) ```
+lol-site-scraper ``` ## Usage ### Command Line Application 1. Navigate to the
+folder where you want scraper to be downloading files. Bare in mind Lols create
+separate subfolder for each scrape. 2. Basic usage syntax is as follows: ```sh
+lols [output_directory] [url] [options] ``` _Learn all options in Command Line
+App Options section or with help dialogue:_ ```sh lols --help ``` ### Library
+You can use Lols in your own custom script and take advantage of all the
+prewritten extractors. Once you pip-installed Lols in either global interpreter
+or the virtual evniroment you set up you can use the library as follows.
+```python from lols import LolsClient, Item from typing import List url =
+"www.url.you/want-to-scrape" # Initiate client client = LolsClient() # Scrape
+URL items: List[Item] = client.scrape(url=url) ``` To disable specific
+extractor for whatever reason be it buggy servers or your disinterest initiate
+the client like so: ```python client = LolsClient( scrapers_to_disable=
+['bunkr'] # Option accepts list of codenames in string format ) ``` Or you can
+specify the only Extractor/s to use: ```python client = LolsClient
+( enabled_extractors=['bunkr'] # Option accepts list of codenames in string
+format ) ```
                                                                   (back_to_top)
 ## Command Line App Options ``` usage: lols [-h] [-a FILE] [-u] [--version] [--
 supported-sites] [-d] [--page-limit CRAWL_PAGE_LIMIT] [--omit-download] [--
 skip-existing] [--overwrite-existing] [--download-path DOWNLOAD_PATH] [-s] [--
 skip-vid] [--skip-img] [--skip-audio] [--skip-archive] [--d-anon] [--d-bunkr]
 [--d-cdrop] [--d-erome] [--d-forum_lm] [--d-forum_nstar] [--d-forum_ps] [--d-
 forum_smg] [--d-gofile] [--d-hex] [--d-hload] [--d-ibam] [--d-ibb] [--d-imgbox]
```

### Comparing `lol-site-scraper-2.0/README.md` & `lol-site-scraper-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 you can incorporate it into your own python scripts as an external library.
 
 ### Installation
 
 1. Download and install latest [python](https://www.python.org/downloads/).
 2. In command line run:
    ```sh
-   pip install lols
+   pip install lol-site-scraper
    ```
 
 ## Usage
 ### Command Line Application
 
 1. Navigate to the folder where you want scraper to be downloading files.
 Bare in mind Lols create separate subfolder for each scrape.
```

#### html2text {}

```diff
@@ -3,30 +3,31 @@
 capable of scraping content from multiple hosting sites/forums. Simple premise:
 user inputs a page url and scraper downloads it's contents.  ## Supported sites
 View supported sites and their corresponding codenames [here](docs/
 supported_sites.txt)  ## Getting Started You can use Lols as either a command
 line application or you can incorporate it into your own python scripts as an
 external library. ### Installation 1. Download and install latest [python]
 (https://www.python.org/downloads/). 2. In command line run: ```sh pip install
-lols ``` ## Usage ### Command Line Application 1. Navigate to the folder where
-you want scraper to be downloading files. Bare in mind Lols create separate
-subfolder for each scrape. 2. Basic usage syntax is as follows: ```sh lols
-[output_directory] [url] [options] ``` _Learn all options in Command Line App
-Options section or with help dialogue:_ ```sh lols --help ``` ### Library You
-can use Lols in your own custom script and take advantage of all the prewritten
-extractors. Once you pip-installed Lols in either global interpreter or the
-virtual evniroment you set up you can use the library as follows. ```python
-from lols import LolsClient, Item from typing import List url = "www.url.you/
-want-to-scrape" # Initiate client client = LolsClient() # Scrape URL items:
-List[Item] = client.scrape(url=url) ``` To disable specific extractor for
-whatever reason be it buggy servers or your disinterest initiate the client
-like so: ```python client = LolsClient( scrapers_to_disable=['bunkr'] # Option
-accepts list of codenames in string format ) ``` Or you can specify the only
-Extractor/s to use: ```python client = LolsClient( enabled_extractors=['bunkr']
-# Option accepts list of codenames in string format ) ```
+lol-site-scraper ``` ## Usage ### Command Line Application 1. Navigate to the
+folder where you want scraper to be downloading files. Bare in mind Lols create
+separate subfolder for each scrape. 2. Basic usage syntax is as follows: ```sh
+lols [output_directory] [url] [options] ``` _Learn all options in Command Line
+App Options section or with help dialogue:_ ```sh lols --help ``` ### Library
+You can use Lols in your own custom script and take advantage of all the
+prewritten extractors. Once you pip-installed Lols in either global interpreter
+or the virtual evniroment you set up you can use the library as follows.
+```python from lols import LolsClient, Item from typing import List url =
+"www.url.you/want-to-scrape" # Initiate client client = LolsClient() # Scrape
+URL items: List[Item] = client.scrape(url=url) ``` To disable specific
+extractor for whatever reason be it buggy servers or your disinterest initiate
+the client like so: ```python client = LolsClient( scrapers_to_disable=
+['bunkr'] # Option accepts list of codenames in string format ) ``` Or you can
+specify the only Extractor/s to use: ```python client = LolsClient
+( enabled_extractors=['bunkr'] # Option accepts list of codenames in string
+format ) ```
                                                                   (back_to_top)
 ## Command Line App Options ``` usage: lols [-h] [-a FILE] [-u] [--version] [--
 supported-sites] [-d] [--page-limit CRAWL_PAGE_LIMIT] [--omit-download] [--
 skip-existing] [--overwrite-existing] [--download-path DOWNLOAD_PATH] [-s] [--
 skip-vid] [--skip-img] [--skip-audio] [--skip-archive] [--d-anon] [--d-bunkr]
 [--d-cdrop] [--d-erome] [--d-forum_lm] [--d-forum_nstar] [--d-forum_ps] [--d-
 forum_smg] [--d-gofile] [--d-hex] [--d-hload] [--d-ibam] [--d-ibb] [--d-imgbox]
```

### Comparing `lol-site-scraper-2.0/lol_site_scraper.egg-info/PKG-INFO` & `lol-site-scraper-2.0.1/lol_site_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: lol-site-scraper
-Version: 2.0
+Version: 2.0.1
 Summary: Bulk hosting sites scraper/downloader
 Home-page: https://github.com/vladimirpolak/lols
 Author: Vladimír Polák
 Author-email: vladimirpolak2@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 style="text-align: center;">Lols</h1>
 
 <!-- ABOUT THE PROJECT -->
 ## About
@@ -28,15 +29,15 @@
 you can incorporate it into your own python scripts as an external library.
 
 ### Installation
 
 1. Download and install latest [python](https://www.python.org/downloads/).
 2. In command line run:
    ```sh
-   pip install lols
+   pip install lol-site-scraper
    ```
 
 ## Usage
 ### Command Line Application
 
 1. Navigate to the folder where you want scraper to be downloading files.
 Bare in mind Lols create separate subfolder for each scrape.
@@ -213,7 +214,8 @@
 ## Contact
 
 Vladimír Polák - vladimirpolak2@gmail.com - Dio#7865
 
 Project Link: [https://github.com/vladimirpolak/lols](https://github.com/vladimirpolak/lols)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
+
```

#### html2text {}

```diff
@@ -1,36 +1,38 @@
-Metadata-Version: 2.1 Name: lol-site-scraper Version: 2.0 Summary: Bulk hosting
-sites scraper/downloader Home-page: https://github.com/vladimirpolak/lols
-Author: VladimÃ­r PolÃ¡k Author-email: vladimirpolak2@gmail.com License: MIT
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: lol-site-scraper Version: 2.0.1 Summary: Bulk
+hosting sites scraper/downloader Home-page: https://github.com/vladimirpolak/
+lols Author: VladimÃ­r PolÃ¡k Author-email: vladimirpolak2@gmail.com License:
+MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-File:
+LICENSE
 ****** Lols ******
  ## About Goal of this project is to have Bulk downloader/Content scraper
 capable of scraping content from multiple hosting sites/forums. Simple premise:
 user inputs a page url and scraper downloads it's contents.  ## Supported sites
 View supported sites and their corresponding codenames [here](docs/
 supported_sites.txt)  ## Getting Started You can use Lols as either a command
 line application or you can incorporate it into your own python scripts as an
 external library. ### Installation 1. Download and install latest [python]
 (https://www.python.org/downloads/). 2. In command line run: ```sh pip install
-lols ``` ## Usage ### Command Line Application 1. Navigate to the folder where
-you want scraper to be downloading files. Bare in mind Lols create separate
-subfolder for each scrape. 2. Basic usage syntax is as follows: ```sh lols
-[output_directory] [url] [options] ``` _Learn all options in Command Line App
-Options section or with help dialogue:_ ```sh lols --help ``` ### Library You
-can use Lols in your own custom script and take advantage of all the prewritten
-extractors. Once you pip-installed Lols in either global interpreter or the
-virtual evniroment you set up you can use the library as follows. ```python
-from lols import LolsClient, Item from typing import List url = "www.url.you/
-want-to-scrape" # Initiate client client = LolsClient() # Scrape URL items:
-List[Item] = client.scrape(url=url) ``` To disable specific extractor for
-whatever reason be it buggy servers or your disinterest initiate the client
-like so: ```python client = LolsClient( scrapers_to_disable=['bunkr'] # Option
-accepts list of codenames in string format ) ``` Or you can specify the only
-Extractor/s to use: ```python client = LolsClient( enabled_extractors=['bunkr']
-# Option accepts list of codenames in string format ) ```
+lol-site-scraper ``` ## Usage ### Command Line Application 1. Navigate to the
+folder where you want scraper to be downloading files. Bare in mind Lols create
+separate subfolder for each scrape. 2. Basic usage syntax is as follows: ```sh
+lols [output_directory] [url] [options] ``` _Learn all options in Command Line
+App Options section or with help dialogue:_ ```sh lols --help ``` ### Library
+You can use Lols in your own custom script and take advantage of all the
+prewritten extractors. Once you pip-installed Lols in either global interpreter
+or the virtual evniroment you set up you can use the library as follows.
+```python from lols import LolsClient, Item from typing import List url =
+"www.url.you/want-to-scrape" # Initiate client client = LolsClient() # Scrape
+URL items: List[Item] = client.scrape(url=url) ``` To disable specific
+extractor for whatever reason be it buggy servers or your disinterest initiate
+the client like so: ```python client = LolsClient( scrapers_to_disable=
+['bunkr'] # Option accepts list of codenames in string format ) ``` Or you can
+specify the only Extractor/s to use: ```python client = LolsClient
+( enabled_extractors=['bunkr'] # Option accepts list of codenames in string
+format ) ```
                                                                   (back_to_top)
 ## Command Line App Options ``` usage: lols [-h] [-a FILE] [-u] [--version] [--
 supported-sites] [-d] [--page-limit CRAWL_PAGE_LIMIT] [--omit-download] [--
 skip-existing] [--overwrite-existing] [--download-path DOWNLOAD_PATH] [-s] [--
 skip-vid] [--skip-img] [--skip-audio] [--skip-archive] [--d-anon] [--d-bunkr]
 [--d-cdrop] [--d-erome] [--d-forum_lm] [--d-forum_nstar] [--d-forum_ps] [--d-
 forum_smg] [--d-gofile] [--d-hex] [--d-hload] [--d-ibam] [--d-ibb] [--d-imgbox]
```

### Comparing `lol-site-scraper-2.0/lol_site_scraper.egg-info/SOURCES.txt` & `lol-site-scraper-2.0.1/lol_site_scraper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 lols/scrapers/lovefap.py
 lols/scrapers/mega.py
 lols/scrapers/pixeldrain.py
 lols/scrapers/pixhost.py
 lols/scrapers/pixl.py
 lols/scrapers/planetsuzy.py
 lols/scrapers/saint.py
-lols/scrapers/sbspeed.py
 lols/scrapers/sendvid.py
 lols/scrapers/simpcity.py
 lols/scrapers/simpcity_auth.py
 lols/scrapers/skygallery.py
 lols/scrapers/streamlare.py
 lols/scrapers/streamtape.py
 lols/scrapers/voe.py
```

### Comparing `lol-site-scraper-2.0/lols/__main__.py` & `lol-site-scraper-2.0.1/lols/__main__.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/config.py` & `lol-site-scraper-2.0.1/lols/config.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/exceptions.py` & `lol-site-scraper-2.0.1/lols/exceptions.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/http/__init__.py` & `lol-site-scraper-2.0.1/lols/http/__init__.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/http/client.py` & `lol-site-scraper-2.0.1/lols/http/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from .headers import HeadersMixin
 
 import time
 import requests
 from requests.exceptions import SSLError
 from urllib3.exceptions import ProtocolError
 import retry
@@ -26,15 +28,19 @@
 
     def send_request(self, url, method, **kwargs) -> requests.Response:
         prepped_req = self._prepare_request(
             url=url,
             method=method,
             **kwargs
         )
-        response = self._send_request(prepped_req, **kwargs)
+        try:
+            response = self._send_request(prepped_req, **kwargs)
+        except requests.RequestException as e:
+            logging.error(f"Failed accessing url '{url}' {e}")
+            response = self.failed_response
         return response
 
     def _prepare_request(self, method: str, url: str, **kwargs) -> requests.PreparedRequest:
         headers = self.general_headers
         headers.update(kwargs.pop("headers", dict()))
 
         req = requests.Request(
@@ -59,15 +65,27 @@
         except SSLError:
             res = self._session.send(
                 request=prepared_request,
                 stream=kwargs.get("stream", None),
                 allow_redirects=kwargs.get("allow_redirects", True),
                 verify=False
             )
+
+        # Timeout in case of rate limiting
         if res.status_code == 429:
-            time.sleep(10)
-            raise requests.exceptions.RequestException()
+            retry_after = int(res.headers.get('Retry-After', 0))
+            if retry_after:
+                time.sleep(retry_after)
+                raise requests.exceptions.RequestException()
         return res
 
+    @property
+    def failed_response(self) -> requests.Response:
+        response = requests.Response()
+        response.status_code = 500
+        response.reason = "Internal Server Error"
+        response._content = b"An error occurred while making the request"
+        return response
+
     def update_cookies(self, cookies: dict, domain: str):
         for k, v in cookies.items():
             self._session.cookies.set(k, v, domain=domain)
```

### Comparing `lol-site-scraper-2.0/lols/http/downloader.py` & `lol-site-scraper-2.0.1/lols/http/downloader.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/http/m3u8_downloader.py` & `lol-site-scraper-2.0.1/lols/http/m3u8_downloader.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/http/models.py` & `lol-site-scraper-2.0.1/lols/http/models.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/http/types.py` & `lol-site-scraper-2.0.1/lols/http/types.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/path_creator.py` & `lol-site-scraper-2.0.1/lols/path_creator.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/__init__.py` & `lol-site-scraper-2.0.1/lols/scrapers/__init__.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/_scraper_base.py` & `lol-site-scraper-2.0.1/lols/scrapers/_scraper_base.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/_scraper_template.py` & `lol-site-scraper-2.0.1/lols/scrapers/_scraper_template.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/all_scrapers.py` & `lol-site-scraper-2.0.1/lols/scrapers/all_scrapers.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/anonfiles.py` & `lol-site-scraper-2.0.1/lols/scrapers/anonfiles.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/bunkr.py` & `lol-site-scraper-2.0.1/lols/scrapers/bunkr.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/cyberdrop.py` & `lol-site-scraper-2.0.1/lols/scrapers/cyberdrop.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/erome.py` & `lol-site-scraper-2.0.1/lols/scrapers/erome.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/forum_nudostar.py` & `lol-site-scraper-2.0.1/lols/scrapers/forum_nudostar.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/forum_nudostar_auth.py` & `lol-site-scraper-2.0.1/lols/scrapers/forum_nudostar_auth.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/forum_socialmediagirls.py` & `lol-site-scraper-2.0.1/lols/scrapers/forum_socialmediagirls.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/forum_socialmediagirls_auth.py` & `lol-site-scraper-2.0.1/lols/scrapers/forum_socialmediagirls_auth.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/forum_thotsbay.py` & `lol-site-scraper-2.0.1/lols/scrapers/forum_thotsbay.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/forum_thotsbay_auth.py` & `lol-site-scraper-2.0.1/lols/scrapers/forum_thotsbay_auth.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/gofile.py` & `lol-site-scraper-2.0.1/lols/scrapers/gofile.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/gofile_auth.py` & `lol-site-scraper-2.0.1/lols/scrapers/gofile_auth.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/hexupload.py` & `lol-site-scraper-2.0.1/lols/scrapers/hexupload.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/highload.py` & `lol-site-scraper-2.0.1/lols/scrapers/highload.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/ibb.py` & `lol-site-scraper-2.0.1/lols/scrapers/ibb.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/imagebam.py` & `lol-site-scraper-2.0.1/lols/scrapers/imagebam.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/imagehaha.py` & `lol-site-scraper-2.0.1/lols/scrapers/imagehaha.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/imagetwist.py` & `lol-site-scraper-2.0.1/lols/scrapers/imagetwist.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/imgbox.py` & `lol-site-scraper-2.0.1/lols/scrapers/imgbox.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/jpgchurch.py` & `lol-site-scraper-2.0.1/lols/scrapers/jpgchurch.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/leakedmodelsforum.py` & `lol-site-scraper-2.0.1/lols/scrapers/leakedmodelsforum.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/leakedmodelsforum_auth.py` & `lol-site-scraper-2.0.1/lols/scrapers/leakedmodelsforum_auth.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/lovefap.py` & `lol-site-scraper-2.0.1/lols/scrapers/lovefap.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/mega.py` & `lol-site-scraper-2.0.1/lols/scrapers/mega.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/pixeldrain.py` & `lol-site-scraper-2.0.1/lols/scrapers/pixeldrain.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/pixhost.py` & `lol-site-scraper-2.0.1/lols/scrapers/pixhost.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/pixl.py` & `lol-site-scraper-2.0.1/lols/scrapers/pixl.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/planetsuzy.py` & `lol-site-scraper-2.0.1/lols/scrapers/planetsuzy.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/sendvid.py` & `lol-site-scraper-2.0.1/lols/scrapers/sendvid.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/simpcity.py` & `lol-site-scraper-2.0.1/lols/scrapers/simpcity.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/simpcity_auth.py` & `lol-site-scraper-2.0.1/lols/scrapers/simpcity_auth.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/skygallery.py` & `lol-site-scraper-2.0.1/lols/scrapers/skygallery.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/streamlare.py` & `lol-site-scraper-2.0.1/lols/scrapers/streamlare.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/streamtape.py` & `lol-site-scraper-2.0.1/lols/scrapers/streamtape.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/voe.py` & `lol-site-scraper-2.0.1/lols/scrapers/voe.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/scrapers/xvideos.py` & `lol-site-scraper-2.0.1/lols/scrapers/xvideos.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/settings.py` & `lol-site-scraper-2.0.1/lols/settings.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/lols/utils.py` & `lol-site-scraper-2.0.1/lols/utils.py`

 * *Files identical despite different names*

### Comparing `lol-site-scraper-2.0/setup.py` & `lol-site-scraper-2.0.1/setup.py`

 * *Files identical despite different names*

