# Comparing `tmp/nonebot_plugin_bawiki-0.7.6.tar.gz` & `tmp/nonebot_plugin_bawiki-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bawiki-0.7.6.tar", last modified: Fri Apr 28 10:10:45 2023, max compression
+gzip compressed data, was "nonebot_plugin_bawiki-0.7.7.tar", last modified: Wed May 10 08:35:56 2023, max compression
```

## Comparing `nonebot_plugin_bawiki-0.7.6.tar` & `nonebot_plugin_bawiki-0.7.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1068 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/LICENSE
--rw-r--r--   0        0        0     7712 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/README.md
--rw-r--r--   0        0        0    15528 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/__init__.py
--rw-r--r--   0        0        0    22651 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/__main__.py
--rw-r--r--   0        0        0     1881 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/config.py
--rw-r--r--   0        0        0     5812 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_bawiki.py
--rw-r--r--   0        0        0     8291 2023-04-28 10:10:23.451967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_gamekee.py
--rw-r--r--   0        0        0    18827 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_schaledb.py
--rw-r--r--   0        0        0     7390 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/gacha.py
--rw-r--r--   0        0        0    21514 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/calender_banner.png
--rw-r--r--   0        0        0  1685142 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_bg.png
--rw-r--r--   0        0        0    13956 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_card_bg.png
--rw-r--r--   0        0        0     2408 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_card_mask.png
--rw-r--r--   0        0        0     4391 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_new.png
--rw-r--r--   0        0        0    10375 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_pickup.png
--rw-r--r--   0        0        0     2022 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_star.png
--rw-r--r--   0        0        0    14652 2023-04-28 10:10:23.455967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_stu_err.png
--rw-r--r--   0        0        0  1764190 2023-04-28 10:10:23.459967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gradient.png
--rw-r--r--   0        0        0      872 2023-04-28 10:10:23.459967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/resource.py
--rw-r--r--   0        0        0     3555 2023-04-28 10:10:23.459967 nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/util.py
--rw-r--r--   0        0        0     1381 2023-04-28 10:10:45.620214 nonebot_plugin_bawiki-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     9053 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/LICENSE
+-rw-r--r--   0        0        0     7722 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/README.md
+-rw-r--r--   0        0        0    15528 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/__init__.py
+-rw-r--r--   0        0        0    22664 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/__main__.py
+-rw-r--r--   0        0        0     1881 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/config.py
+-rw-r--r--   0        0        0     5812 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_bawiki.py
+-rw-r--r--   0        0        0     8291 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_gamekee.py
+-rw-r--r--   0        0        0    18827 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_schaledb.py
+-rw-r--r--   0        0        0     7390 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/gacha.py
+-rw-r--r--   0        0        0    21514 2023-05-10 08:35:30.221850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/calender_banner.png
+-rw-r--r--   0        0        0  1685142 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_bg.png
+-rw-r--r--   0        0        0    13956 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_card_bg.png
+-rw-r--r--   0        0        0     2408 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_card_mask.png
+-rw-r--r--   0        0        0     4391 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_new.png
+-rw-r--r--   0        0        0    10375 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_pickup.png
+-rw-r--r--   0        0        0     2022 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_star.png
+-rw-r--r--   0        0        0    14652 2023-05-10 08:35:30.225850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_stu_err.png
+-rw-r--r--   0        0        0  1764190 2023-05-10 08:35:30.229850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gradient.png
+-rw-r--r--   0        0        0      872 2023-05-10 08:35:30.229850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/resource.py
+-rw-r--r--   0        0        0     3555 2023-05-10 08:35:30.229850 nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/util.py
+-rw-r--r--   0        0        0     1381 2023-05-10 08:35:56.677607 nonebot_plugin_bawiki-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     9063 1970-01-01 00:00:00.000000 nonebot_plugin_bawiki-0.7.7/PKG-INFO
```

### Comparing `nonebot_plugin_bawiki-0.7.6/LICENSE` & `nonebot_plugin_bawiki-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/README.md` & `nonebot_plugin_bawiki-0.7.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,15 @@
 
 </div>
 
 ## 💬 前言
 
 诚邀各位帮忙更新插件数据源仓库！能帮这个小小插件贡献微薄之力，鄙人感激不尽！！
 
-[点击跳转 bawiki-data](https://github.com/lgc2333/bawiki-data)
-
-修改后提交 Pull Request 即可！
+[点击跳转 bawiki-data 查看详细贡献说明](https://github.com/lgc2333/bawiki-data)
 
 ## 📖 介绍
 
 一个碧蓝档案的 Wiki 插件，主要数据来源为 [GameKee](https://ba.gamekee.com/) 与 [SchaleDB](https://lonqie.github.io/SchaleDB/)  
 插件灵感来源：[ba_calender](https://f.xiaolz.cn/forum.php?mod=viewthread&tid=145)
 
 ## 💿 安装
@@ -152,14 +150,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.7.7
+
+- 修复 bug
+
 ### 0.7.6
 
 - 修复卡池为空不会提示的 bug
 
 ### 0.7.5
 
 - 插件可以自动帮你配置 PicMenu 的字体了
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
                                    [BAWiki]
 # NoneBot-Plugin-BAWiki _â¨ åºäº NoneBot2 çç¢§èæ¡£æ¡ Wiki æä»¶ â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð¬ åè¨
 è¯éåä½å¸®å¿æ´æ°æä»¶æ°æ®æºä»åºï¼è½å¸®è¿ä¸ªå°å°æä»¶è´¡ç®å¾®èä¹åï¼éäººææ¿ä¸å°½ï¼ï¼
-[ç¹å»è·³è½¬ bawiki-data](https://github.com/lgc2333/bawiki-data)
-ä¿®æ¹åæäº¤ Pull Request å³å¯ï¼ ## ð ä»ç» ä¸ä¸ªç¢§èæ¡£æ¡ç
-Wiki æä»¶ï¼ä¸»è¦æ°æ®æ¥æºä¸º [GameKee](https://ba.gamekee.com/) ä¸
+[ç¹å»è·³è½¬ bawiki-data æ¥çè¯¦ç»è´¡ç®è¯´æ](https://github.com/lgc2333/
+bawiki-data) ## ð ä»ç» ä¸ä¸ªç¢§èæ¡£æ¡ç Wiki
+æä»¶ï¼ä¸»è¦æ°æ®æ¥æºä¸º [GameKee](https://ba.gamekee.com/) ä¸
 [SchaleDB](https://lonqie.github.io/SchaleDB/) æä»¶çµææ¥æºï¼
 [ba_calender](https://f.xiaolz.cn/forum.php?mod=viewthread&tid=145) ## ð¿
 å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
 å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-bawiki
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
@@ -39,18 +39,18 @@
 126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
 æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
-æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº - ç»æ½å¡æ°å¢äºå·å´
-### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ### 0.7.0 -
-ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
+0.7.7 - ä¿®å¤ bug ### 0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5
+- æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
+ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
+æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
 [cyberczy.xyz](http://cyberczy.xyz/)ï¼ - å¶ä»å°æ´æ¹ ### 0.6.4 -
 ä¿®å¤ç±äº `imageutils` æ¥å£æ¹å¨é æçç»å¾å¤±è´¥ç bug ### 0.6.3 -
```

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/__init__.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
 
 from . import __main__ as __main__  # noqa: E402
 
-__version__ = "0.7.6"
+__version__ = "0.7.7"
 __plugin_meta__ = PluginMetadata(
     name="BAWiki",
     description="碧蓝档案Wiki插件",
     usage=(
         "感谢各位sensei使用本插件！\n"
         "插件有缓存机制，每3小时自动清空一次，如果插件遇到问题可以先手动清空缓存试一下捏\n"
         "装载PicMenu插件即可查看插件详细菜单哦\n"
```

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/__main__.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 fav = on_command("ba好感度", aliases={"ba羁绊", "bal2d", "baL2D", "balive2d", "baLive2D"})
 
 
 @fav.handle()
 async def _(matcher: Matcher, cmd_arg: Message = CommandArg()):
     async def get_l2d(stu_name):
         if r := (await db_get_extra_l2d_list()).get(stu_name):
-            return f"{config.ba_bawiki_db_url}{r}"
+            return [f"{config.ba_bawiki_db_url}{x}" for x in r]
 
         return await game_kee_grab_l2d((await game_kee_get_stu_cid_li()).get(stu_name))
 
     arg = cmd_arg.extract_plain_text().strip()
     if not arg:
         await matcher.finish("请提供学生名称或所需的羁绊等级")
```

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/config.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_bawiki.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_bawiki.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_gamekee.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_gamekee.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/data_schaledb.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/data_schaledb.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/gacha.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/gacha.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/calender_banner.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/calender_banner.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_bg.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_card_bg.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_card_bg.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_card_mask.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_card_mask.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_new.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_new.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_pickup.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_pickup.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_star.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_star.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gacha_stu_err.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gacha_stu_err.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/res/gradient.png` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/res/gradient.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/resource.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/nonebot_plugin_bawiki/util.py` & `nonebot_plugin_bawiki-0.7.7/nonebot_plugin_bawiki/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bawiki-0.7.6/pyproject.toml` & `nonebot_plugin_bawiki-0.7.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bawiki"
-version = "0.7.6"
+version = "0.7.7"
 description = "A nonebot2 plugin for Blue Archive."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.3",
     "nonebot2>=2.0.0b5",
```

### Comparing `nonebot_plugin_bawiki-0.7.6/PKG-INFO` & `nonebot_plugin_bawiki-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bawiki
-Version: 0.7.6
+Version: 0.7.7
 Summary: A nonebot2 plugin for Blue Archive.
 Keywords: blue archive nonebot nonebot2 bot qq
 Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications
@@ -58,17 +58,15 @@
 
 </div>
 
 ## 💬 前言
 
 诚邀各位帮忙更新插件数据源仓库！能帮这个小小插件贡献微薄之力，鄙人感激不尽！！
 
-[点击跳转 bawiki-data](https://github.com/lgc2333/bawiki-data)
-
-修改后提交 Pull Request 即可！
+[点击跳转 bawiki-data 查看详细贡献说明](https://github.com/lgc2333/bawiki-data)
 
 ## 📖 介绍
 
 一个碧蓝档案的 Wiki 插件，主要数据来源为 [GameKee](https://ba.gamekee.com/) 与 [SchaleDB](https://lonqie.github.io/SchaleDB/)  
 插件灵感来源：[ba_calender](https://f.xiaolz.cn/forum.php?mod=viewthread&tid=145)
 
 ## 💿 安装
@@ -184,14 +182,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.7.7
+
+- 修复 bug
+
 ### 0.7.6
 
 - 修复卡池为空不会提示的 bug
 
 ### 0.7.5
 
 - 插件可以自动帮你配置 PicMenu 的字体了
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.6 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bawiki Version: 0.7.7 Summary: A
 nonebot2 plugin for Blue Archive. Keywords: blue archive nonebot nonebot2 bot
 qq Home-page: https://github.com/lgc2333/nonebot-plugin-bawiki/ Author-Email:
 student_2333
 126.com> License: MIT Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Communications :: Chat :: ICQ Classifier: Topic :: Games/
 Entertainment Classifier: Topic :: Games/Entertainment :: Board Games
@@ -18,17 +18,17 @@
 Requires-Dist: lxml>=4.9.1 Requires-Dist: pil-utils>=0.1.4 Description-Content-
 Type: text/markdown
                                    [BAWiki]
 # NoneBot-Plugin-BAWiki _â¨ åºäº NoneBot2 çç¢§èæ¡£æ¡ Wiki æä»¶ â¨_
              [license] [pypi] [python] [pypi_download] [wakatime]
 ## ð¬ åè¨
 è¯éåä½å¸®å¿æ´æ°æä»¶æ°æ®æºä»åºï¼è½å¸®è¿ä¸ªå°å°æä»¶è´¡ç®å¾®èä¹åï¼éäººææ¿ä¸å°½ï¼ï¼
-[ç¹å»è·³è½¬ bawiki-data](https://github.com/lgc2333/bawiki-data)
-ä¿®æ¹åæäº¤ Pull Request å³å¯ï¼ ## ð ä»ç» ä¸ä¸ªç¢§èæ¡£æ¡ç
-Wiki æä»¶ï¼ä¸»è¦æ°æ®æ¥æºä¸º [GameKee](https://ba.gamekee.com/) ä¸
+[ç¹å»è·³è½¬ bawiki-data æ¥çè¯¦ç»è´¡ç®è¯´æ](https://github.com/lgc2333/
+bawiki-data) ## ð ä»ç» ä¸ä¸ªç¢§èæ¡£æ¡ç Wiki
+æä»¶ï¼ä¸»è¦æ°æ®æ¥æºä¸º [GameKee](https://ba.gamekee.com/) ä¸
 [SchaleDB](https://lonqie.github.io/SchaleDB/) æä»¶çµææ¥æºï¼
 [ba_calender](https://f.xiaolz.cn/forum.php?mod=viewthread&tid=145) ## ð¿
 å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli
 å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-bawiki
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
@@ -58,18 +58,18 @@
 126.com> ## ð¡ é¸£è°¢ ### [RainNight0](https://github.com/RainNight0) -
 æ¥ç¨è¡¨ html æ¨¡æ¿æä¾ï¼å·²å¼ç¨ï¼ ### `bawiki-data`
 æ°æ®æºè´¡ç®åè¡¨ - è§ [bawiki-data](http://github.com/lgc2333/bawiki-
 data) ## ð° èµå© æè°¢åä½å¤§ä½¬çæåâ¦â¦ï¼ï¼æ¬ fw
 å®å¨ææ¿ä¸å°½â¦â¦ - [ç±åçµ](https://afdian.net/@lgc2333) -
 èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ ![è®¨é¥­](https://raw.githubusercontent.com/
 lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ###
-0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5 -
-æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº - ç»æ½å¡æ°å¢äºå·å´
-### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 - æ´æ¹éç½®é¡¹åç§° ### 0.7.0 -
-ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
+0.7.7 - ä¿®å¤ bug ### 0.7.6 - ä¿®å¤å¡æ± ä¸ºç©ºä¸ä¼æç¤ºç bug ### 0.7.5
+- æä»¶å¯ä»¥èªå¨å¸®ä½ éç½® PicMenu çå­ä½äº -
+ç»æ½å¡æ°å¢äºå·å´ ### 0.7.2 ~ 0.7.4 - ä¿®å¤ bug ### 0.7.1 -
+æ´æ¹éç½®é¡¹åç§° ### 0.7.0 - ä¿®å¤ SchaleDB æºæ¥ç¨è¡¨åºéçé®é¢ -
 æ·»å äºå ä¸ªéç½®é¡¹ï¼ç°å¨å¯ä»¥å¨ `.env`
 æä»¶ä¸­ä¿®æ¹æ°æ®æºé¾æ¥äº - ä¿®æ¹äºé»è®¤æ°æ®æºé¾æ¥ -
 ä¹°äºä¸çäºç CDNï¼è®¾ç½®çæ°æ®ç¼å­ 12
 å°æ¶ãä¸ç¥éç°å¨éåº¦æä¹æ ·â¦â¦
 å¸æä¸è¦æäººææææâ¦â¦ æè°¢å¤§ä½¬åç¨çå·²å¤æ¡åå
 [cyberczy.xyz](http://cyberczy.xyz/)ï¼ - å¶ä»å°æ´æ¹ ### 0.6.4 -
 ä¿®å¤ç±äº `imageutils` æ¥å£æ¹å¨é æçç»å¾å¤±è´¥ç bug ### 0.6.3 -
```

