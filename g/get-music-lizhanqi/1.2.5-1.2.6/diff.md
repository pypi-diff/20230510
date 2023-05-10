# Comparing `tmp/get-music-lizhanqi-1.2.5.tar.gz` & `tmp/get-music-lizhanqi-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\???\Desktop\get_music\dist\.tmp-0ydxs70x\get-music-lizhanqi-1.2.5.tar", last modified: Mon Apr 10 09:52:40 2023, max compression
+gzip compressed data, was "C:\Users\???\Desktop\get_music\dist\.tmp-jls9085t\get-music-lizhanqi-1.2.6.tar", last modified: Wed May 10 10:22:43 2023, max compression
```

## Comparing `get-music-lizhanqi-1.2.5.tar` & `get-music-lizhanqi-1.2.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/
--rw-rw-rw-   0        0        0     1091 2022-04-09 10:07:52.000000 get-music-lizhanqi-1.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1869 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1455 2023-04-10 09:51:35.000000 get-music-lizhanqi-1.2.5/README.md
--rw-rw-rw-   0        0        0       86 2022-04-09 10:04:03.000000 get-music-lizhanqi-1.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      952 2023-04-10 09:43:27.000000 get-music-lizhanqi-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/
-drwxrwxrwx   0        0        0        0 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/tests/get_music/
--rw-rw-rw-   0        0        0      266 2023-04-09 14:18:18.000000 get-music-lizhanqi-1.2.5/tests/get_music/__init__.py
--rw-rw-rw-   0        0        0     3092 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/baidu.py
--rw-rw-rw-   0        0        0     1938 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/download.py
--rw-rw-rw-   0        0        0     2892 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/downloads.py
--rw-rw-rw-   0        0        0     3222 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/fivesing.py
--rw-rw-rw-   0        0        0    10379 2023-04-10 09:41:28.000000 get-music-lizhanqi-1.2.5/tests/get_music/get_music.py
--rw-rw-rw-   0        0        0    11725 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/gui.py
--rw-rw-rw-   0        0        0     2613 2023-04-10 09:28:35.000000 get-music-lizhanqi-1.2.5/tests/get_music/kg_one_playerlist.py
--rw-rw-rw-   0        0        0     2570 2023-04-10 09:22:32.000000 get-music-lizhanqi-1.2.5/tests/get_music/kg_playerlist.py
--rw-rw-rw-   0        0        0     5305 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/kugou.py
--rw-rw-rw-   0        0        0     3985 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/kuwo.py
--rw-rw-rw-   0        0        0     2685 2023-04-10 09:47:01.000000 get-music-lizhanqi-1.2.5/tests/get_music/kw_playerlist.py
--rw-rw-rw-   0        0        0     2861 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/migu.py
--rw-rw-rw-   0        0        0     3763 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/netease.py
--rw-rw-rw-   0        0        0     2090 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/oneting.py
--rw-rw-rw-   0        0        0     3306 2023-04-10 09:21:26.000000 get-music-lizhanqi-1.2.5/tests/get_music/playerlist.py
--rw-rw-rw-   0        0        0     4293 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/qq.py
--rw-rw-rw-   0        0        0     2534 2023-04-10 09:46:23.000000 get-music-lizhanqi-1.2.5/tests/get_music/qq_playerlist.py
--rw-rw-rw-   0        0        0     2562 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/singbz.py
--rw-rw-rw-   0        0        0     6826 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/top.py
--rw-rw-rw-   0        0        0     2100 2023-04-09 14:37:17.000000 get-music-lizhanqi-1.2.5/tests/get_music/ver.py
--rw-rw-rw-   0        0        0     3119 2023-04-10 09:46:07.000000 get-music-lizhanqi-1.2.5/tests/get_music/wy_playerlist.py
--rw-rw-rw-   0        0        0     3692 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.5/tests/get_music/zhidao.py
-drwxrwxrwx   0        0        0        0 2023-04-10 09:52:40.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/
--rw-rw-rw-   0        0        0     1869 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 09:52:39.000000 get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/
+-rw-rw-rw-   0        0        0     1091 2022-04-09 10:07:52.000000 get-music-lizhanqi-1.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1745 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-05-10 10:21:54.000000 get-music-lizhanqi-1.2.6/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-09 10:04:03.000000 get-music-lizhanqi-1.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      952 2023-05-10 10:20:16.000000 get-music-lizhanqi-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/
+drwxrwxrwx   0        0        0        0 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/get_music/
+-rw-rw-rw-   0        0        0      266 2023-04-09 14:18:18.000000 get-music-lizhanqi-1.2.6/tests/get_music/__init__.py
+-rw-rw-rw-   0        0        0     3092 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/baidu.py
+-rw-rw-rw-   0        0        0     1938 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/download.py
+-rw-rw-rw-   0        0        0     2892 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/downloads.py
+-rw-rw-rw-   0        0        0     3222 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/fivesing.py
+-rw-rw-rw-   0        0        0    10519 2023-05-05 00:20:30.000000 get-music-lizhanqi-1.2.6/tests/get_music/get_music.py
+-rw-rw-rw-   0        0        0    11919 2023-04-12 00:27:59.000000 get-music-lizhanqi-1.2.6/tests/get_music/gui.py
+-rw-rw-rw-   0        0        0     2613 2023-04-10 09:28:35.000000 get-music-lizhanqi-1.2.6/tests/get_music/kg_one_playerlist.py
+-rw-rw-rw-   0        0        0     2570 2023-04-10 09:22:32.000000 get-music-lizhanqi-1.2.6/tests/get_music/kg_playerlist.py
+-rw-rw-rw-   0        0        0     5305 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/kugou.py
+-rw-rw-rw-   0        0        0     3985 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/kuwo.py
+-rw-rw-rw-   0        0        0     2685 2023-04-10 09:47:01.000000 get-music-lizhanqi-1.2.6/tests/get_music/kw_playerlist.py
+-rw-rw-rw-   0        0        0     2861 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/migu.py
+-rw-rw-rw-   0        0        0     3763 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/netease.py
+-rw-rw-rw-   0        0        0     2090 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/oneting.py
+-rw-rw-rw-   0        0        0     3306 2023-04-10 09:21:26.000000 get-music-lizhanqi-1.2.6/tests/get_music/playerlist.py
+-rw-rw-rw-   0        0        0     4293 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/qq.py
+-rw-rw-rw-   0        0        0     2534 2023-04-10 09:46:23.000000 get-music-lizhanqi-1.2.6/tests/get_music/qq_playerlist.py
+-rw-rw-rw-   0        0        0     2569 2023-05-05 00:16:37.000000 get-music-lizhanqi-1.2.6/tests/get_music/singbz.py
+-rw-rw-rw-   0        0        0     6826 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/top.py
+-rw-rw-rw-   0        0        0     2214 2023-05-10 10:19:12.000000 get-music-lizhanqi-1.2.6/tests/get_music/ver.py
+-rw-rw-rw-   0        0        0     3119 2023-04-10 09:46:07.000000 get-music-lizhanqi-1.2.6/tests/get_music/wy_playerlist.py
+-rw-rw-rw-   0        0        0     3692 2023-03-24 03:55:47.000000 get-music-lizhanqi-1.2.6/tests/get_music/zhidao.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/
+-rw-rw-rw-   0        0        0     1745 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 10:22:43.000000 get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/top_level.txt
```

### Comparing `get-music-lizhanqi-1.2.5/LICENSE.txt` & `get-music-lizhanqi-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/PKG-INFO` & `get-music-lizhanqi-1.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: get-music-lizhanqi
-Version: 1.2.5
+Version: 1.2.6
 Summary: 可以下载音乐的包哦
 Home-page: 
 Author: Li Zhan Qi
 Author-email: 3101978435@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+
 # get-music-lizhanqi
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-04-10 完成v1.2.5版本,支持手机kugou的歌单链接进行获取歌单中的信息,优化导入模块时会打印的logo导致pyinstaller -w参数打包时会失败的问题，由此取消导入模块时打印logo,只有在命令行执行命令时会打印logo,优化细节
+- 2023-05-10 完成v1.2.6版本,修复5sing伴奏中搜索结果无法正常显示的问题，修复5sing伴奏下载后会保存上传者的名字的问题。
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
```

### Comparing `get-music-lizhanqi-1.2.5/README.md` & `get-music-lizhanqi-1.2.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+
 # get-music-lizhanqi
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-04-10 完成v1.2.5版本,支持手机kugou的歌单链接进行获取歌单中的信息,优化导入模块时会打印的logo导致pyinstaller -w参数打包时会失败的问题，由此取消导入模块时打印logo,只有在命令行执行命令时会打印logo,优化细节
+- 2023-05-10 完成v1.2.6版本,修复5sing伴奏中搜索结果无法正常显示的问题，修复5sing伴奏下载后会保存上传者的名字的问题。
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
```

### Comparing `get-music-lizhanqi-1.2.5/setup.py` & `get-music-lizhanqi-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="get-music-lizhanqi",
-    version="1.2.5",
+    version="1.2.6",
     author="Li Zhan Qi",
     author_email="3101978435@qq.com",
     description="可以下载音乐的包哦",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={
```

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/baidu.py` & `get-music-lizhanqi-1.2.6/tests/get_music/baidu.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/download.py` & `get-music-lizhanqi-1.2.6/tests/get_music/download.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/downloads.py` & `get-music-lizhanqi-1.2.6/tests/get_music/downloads.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/fivesing.py` & `get-music-lizhanqi-1.2.6/tests/get_music/fivesing.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/get_music.py` & `get-music-lizhanqi-1.2.6/tests/get_music/get_music.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,15 +187,18 @@
         for i in song_list:
             try:
                 i=int(i)-1
             except ValueError:
                 console.print("[b red]您输入的序号有问题，请用仔细检查谢谢！")
                 continue
             try:
-                fname=name[i]+"-"+singer[i]+".mp3"
+                singername=singer[i]
+                if self.api=='5Sing伴奏':
+                    singername=singer[i].split('-')[0]
+                fname=name[i]+"-"+singername+".mp3"
                 url=song_url[i]
                 songurl=self.get_music_url(url)
                 if self.l==True:
                     self.get_music_lrc(num=i)
                 if self.p==True:
                     self.get_music_pic(num=i)
                 download.download(songurl,fname,ouput=True)
```

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/gui.py` & `get-music-lizhanqi-1.2.6/tests/get_music/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from get_music import kuwo
 from get_music import fivesing
 from get_music import qq
 from get_music import kuwo
 from get_music import oneting
 from get_music import baidu
 from get_music import migu
+from get_music import singbz
 
  
 
 song_name=[]
 singer_name=[]
 song_url=[]
 page=1
@@ -44,15 +45,16 @@
        2:netease.netease(),
        3:qq.qq(),
        4:kuwo.kuwo(),
        5:migu.migu(),
        6:baidu.baidu(),
        7:oneting.oneting(),
        8:fivesing.fivesing('yc'),
-       9:fivesing.fivesing('fc')}
+       9:fivesing.fivesing('fc'),
+       10:singbz.singbz()}
     global api
     api=d[comboExample.current()+1]
     try:
         song_name,singer_name,song_url=api.search(song)
     except:
         tkinter.messagebox._show('警告信息',"无法返回数据或接口失效,或者您的网络未连接，如果还未解决可联系维护者邮箱：3101978435@qq.com")
         return
@@ -76,15 +78,16 @@
        2:netease.netease(),
        3:qq.qq(),
        4:kuwo.kuwo(),
        5:migu.migu(),
        6:baidu.baidu(),
        7:oneting.oneting(),
        8:fivesing.fivesing('yc'),
-       9:fivesing.fivesing('fc')}
+       9:fivesing.fivesing('fc'),
+       10:singbz.singbz()}
     global api
     api=d[comboExample.current()+1]
     try:
         song_name,singer_name,song_url=api.search(song)
     except:
         tkinter.messagebox._show('警告信息',"无法返回数据或接口失效,或者您的网络未连接，如果还未解决可联系维护者邮箱：3101978435@qq.com")
         return
@@ -108,15 +111,16 @@
        2:netease.netease(),
        3:qq.qq(),
        4:kuwo.kuwo(),
        5:migu.migu(),
        6:baidu.baidu(),
        7:oneting.oneting(),
        8:fivesing.fivesing('yc'),
-       9:fivesing.fivesing('fc')}
+       9:fivesing.fivesing('fc'),
+       10:singbz.singbz()}
     global api
     global page
     page=page+1
     api=d[comboExample.current()+1]
     try:
         song_name,singer_name,song_url=api.search(song,page)
     except:
@@ -140,15 +144,16 @@
        2:netease.netease(),
        3:qq.qq(),
        4:kuwo.kuwo(),
        5:migu.migu(),
        6:baidu.baidu(),
        7:oneting.oneting(),
        8:fivesing.fivesing('yc'),
-       9:fivesing.fivesing('fc')}
+       9:fivesing.fivesing('fc'),
+       10:singbz.singbz()}
     global api
     global page
     if page==1:
         tkinter.messagebox._show('警告信息','已经是第一页啦！')
         show()
         return 
     page=page-1
@@ -263,15 +268,16 @@
                                     "网易云音乐",
                                     "QQ音乐",
                                     "酷我音乐",
                                     "咪咕音乐",
                                     "千千静听",
                                     "一听音乐",
                                     "5sing原唱",
-                                    "5sing翻唱"],font=("Consolas", 15),state="readonly")
+                                    "5sing翻唱",
+                                    "5sing伴奏"],font=("Consolas", 15),state="readonly")
 comboExample.grid(row=0, column=0)
 comboExample.current(0)
 
  
 
 Button(root, text="搜索", relief = 'ridge',font=("Consolas", 15), command=show).grid(row=0, column=2)
```

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/kg_one_playerlist.py` & `get-music-lizhanqi-1.2.6/tests/get_music/kg_one_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/kg_playerlist.py` & `get-music-lizhanqi-1.2.6/tests/get_music/kg_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/kugou.py` & `get-music-lizhanqi-1.2.6/tests/get_music/kugou.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/kuwo.py` & `get-music-lizhanqi-1.2.6/tests/get_music/kuwo.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/kw_playerlist.py` & `get-music-lizhanqi-1.2.6/tests/get_music/kw_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/migu.py` & `get-music-lizhanqi-1.2.6/tests/get_music/migu.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/netease.py` & `get-music-lizhanqi-1.2.6/tests/get_music/netease.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/oneting.py` & `get-music-lizhanqi-1.2.6/tests/get_music/oneting.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/playerlist.py` & `get-music-lizhanqi-1.2.6/tests/get_music/playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/qq.py` & `get-music-lizhanqi-1.2.6/tests/get_music/qq.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/qq_playerlist.py` & `get-music-lizhanqi-1.2.6/tests/get_music/qq_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/singbz.py` & `get-music-lizhanqi-1.2.6/tests/get_music/singbz.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         d=req.json()
         self.songs_url=[]
         self.songname=[]
         self.singername=[]
         for i in d['list']:
                     self.songs_url.append(i['songId'])
                     self.singername.append(i['originSinger']+'-'+i['nickName'])
-                    self.songname.append(re.findall('<em class="keyword">(.*?)</em>',i['songName'])[0])
+                    self.songname.append(i['songName'].replace('<em class="keyword">','').replace('</em>',''))
 
         return self.songname,self.singername,self.songs_url
     
     def get_music_url(self,songid):
         
         jx='http://service.5sing.kugou.com/song/getsongurl?songid={}&songtype=bz&from=web&version=6.6.72&_=1673862766682'.format(songid)
         headers={'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.84 Safari/537.36'
```

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/top.py` & `get-music-lizhanqi-1.2.6/tests/get_music/top.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/ver.py` & `get-music-lizhanqi-1.2.6/tests/get_music/ver.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,27 @@
     
     if ip==True:
             try:
                 txt=requests.get('http://ip.tool.lu',timeout=1).text.split()
                 ip=txt[1]
                 area=' '.join(txt[3:])
                 console.print('\n[b green]信息一:本机外网ip地址为:[b red]{}[/]，归属:[b red]{}[/]'.format(ip,area))
+                
+            except:
+                console.print("\n[b red]ip地址信息一查询失败！")
 
+            try:
                 url = 'http://api.ip33.com/ip/search?s='                     
                 d = requests.get(url,timeout=1).json()                                                       
                 console.print('\n[b green]信息二:本机外网ip地址为:[b red]{}[/]，归属:[b red]{}[/]'.format(d['ip'],d['area']))
-                return
             except:
-                console.print("\n[b red]ip地址查询失败！")
-                return
+                console.print("\n[b red]ip地址信息查二询失败！")
+            return
     
-    version = '1.2.5'
+    version = '1.2.6'
     console.print("[green]当前版本:"+"v"+version)
     url = 'https://pypi.org/project/get-music-lizhanqi/#history'
     try:
         with console.status("[b green]检查最新版中..."):
             html = requests.get(url,timeout = 5)
             txt = html.text
             crad = re.findall(r' <a class="card release__card" href="/project/get-music-lizhanqi/(.*?)/">',txt,re.S)
```

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/wy_playerlist.py` & `get-music-lizhanqi-1.2.6/tests/get_music/wy_playerlist.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music/zhidao.py` & `get-music-lizhanqi-1.2.6/tests/get_music/zhidao.py`

 * *Files identical despite different names*

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/PKG-INFO` & `get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: get-music-lizhanqi
-Version: 1.2.5
+Version: 1.2.6
 Summary: 可以下载音乐的包哦
 Home-page: 
 Author: Li Zhan Qi
 Author-email: 3101978435@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+
 # get-music-lizhanqi
 - 这是一个可以下载和搜索音乐的python命令行工具，支持，酷狗，酷我，百度，网易云，咪咕，qq音乐，5sing，欢迎前来学习的指点
 
 ## 使用方法
 - 长话短说**get-music -help**或**get-music-lizhanqi -help**打开帮助，帮助里面有全部命令的介绍，或者前往github地址:<https://github.com/lzq-hopego/get-music-lizhanqi>
 
 
 ## 更新记录
-- 2023-04-10 完成v1.2.5版本,支持手机kugou的歌单链接进行获取歌单中的信息,优化导入模块时会打印的logo导致pyinstaller -w参数打包时会失败的问题，由此取消导入模块时打印logo,只有在命令行执行命令时会打印logo,优化细节
+- 2023-05-10 完成v1.2.6版本,修复5sing伴奏中搜索结果无法正常显示的问题，修复5sing伴奏下载后会保存上传者的名字的问题。
 
 
 
 
 ## THE END
 - 本脚本仅支持学习使用，如有发现有任何商业用途，一经发现您将受到法律责任。
 - 本程序使用的接口全部来源于网络，切不可有任何商业用途，或我程序中有涉及你公司利益的，你可以联系我，我会及时删除源代码，并不再更新。
```

### Comparing `get-music-lizhanqi-1.2.5/tests/get_music_lizhanqi.egg-info/SOURCES.txt` & `get-music-lizhanqi-1.2.6/tests/get_music_lizhanqi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

