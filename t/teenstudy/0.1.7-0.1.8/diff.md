# Comparing `tmp/TeenStudy-0.1.7.tar.gz` & `tmp/TeenStudy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TeenStudy-0.1.7.tar", max compression
+gzip compressed data, was "TeenStudy-0.1.8.tar", max compression
```

## Comparing `TeenStudy-0.1.7.tar` & `TeenStudy-0.1.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1084 2023-05-06 04:08:57.731309 TeenStudy-0.1.7/LICENSE
--rw-r--r--   0        0        0      955 2023-05-06 09:11:05.637704 TeenStudy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     9960 2023-05-06 08:45:54.744774 TeenStudy-0.1.7/README.md
--rw-r--r--   0        0        0      666 2023-05-06 04:16:34.547526 TeenStudy-0.1.7/TeenStudy/__init__.py
--rw-r--r--   0        0        0       28 2023-05-06 04:08:57.732319 TeenStudy-0.1.7/TeenStudy/models/__init__.py
--rw-r--r--   0        0        0     3547 2023-05-06 04:08:57.733777 TeenStudy-0.1.7/TeenStudy/models/accuont.py
--rw-r--r--   0        0        0     3621 2023-05-06 04:08:57.733777 TeenStudy-0.1.7/TeenStudy/models/dxx.py
--rw-r--r--   0        0        0   881164 2023-05-06 04:08:57.790011 TeenStudy-0.1.7/TeenStudy/resource/answer.png
--rw-r--r--   0        0        0    52240 2023-05-06 04:08:57.791011 TeenStudy-0.1.7/TeenStudy/resource/backgroud1.jpg
--rw-r--r--   0        0        0    52119 2023-05-06 04:08:57.792437 TeenStudy-0.1.7/TeenStudy/resource/backgroud2.jpg
--rw-r--r--   0        0        0    52136 2023-05-06 04:08:57.792437 TeenStudy-0.1.7/TeenStudy/resource/backgroud3.jpg
--rw-r--r--   0        0        0    51874 2023-05-06 04:08:57.793437 TeenStudy-0.1.7/TeenStudy/resource/backgroud4.jpg
--rw-r--r--   0        0        0    51634 2023-05-06 04:08:57.793437 TeenStudy-0.1.7/TeenStudy/resource/backgroud5.jpg
--rw-r--r--   0        0        0 10424793 2023-05-06 04:08:57.825443 TeenStudy-0.1.7/TeenStudy/resource/dxx_jx.json
--rw-r--r--   0        0        0  7977480 2023-05-06 04:08:57.787010 TeenStudy-0.1.7/TeenStudy/resource/MiSans-Light.ttf
--rw-r--r--   0        0        0      121 2023-05-06 04:08:57.826444 TeenStudy-0.1.7/TeenStudy/utils/__init__.py
--rw-r--r--   0        0        0    41094 2023-05-06 08:22:07.953021 TeenStudy-0.1.7/TeenStudy/utils/dxx.py
--rw-r--r--   0        0        0    18819 2023-05-06 06:32:36.543523 TeenStudy-0.1.7/TeenStudy/utils/handle.py
--rw-r--r--   0        0        0     4331 2023-05-06 08:28:06.723801 TeenStudy-0.1.7/TeenStudy/utils/path.py
--rw-r--r--   0        0        0     2026 2023-05-06 04:08:57.828444 TeenStudy-0.1.7/TeenStudy/utils/rule.py
--rw-r--r--   0        0        0    10411 2023-05-06 06:39:01.954182 TeenStudy-0.1.7/TeenStudy/utils/update.py
--rw-r--r--   0        0        0    23399 2023-05-06 08:27:27.912843 TeenStudy-0.1.7/TeenStudy/utils/utils.py
--rw-r--r--   0        0        0     2185 2023-05-06 04:08:57.830444 TeenStudy-0.1.7/TeenStudy/web/__init__.py
--rw-r--r--   0        0        0      396 2023-05-06 04:08:57.830444 TeenStudy-0.1.7/TeenStudy/web/api/__init__.py
--rw-r--r--   0        0        0    33714 2023-05-06 08:09:01.153218 TeenStudy-0.1.7/TeenStudy/web/api/add.py
--rw-r--r--   0        0        0    11925 2023-05-06 04:08:57.831445 TeenStudy-0.1.7/TeenStudy/web/api/admin.py
--rw-r--r--   0        0        0     4706 2023-05-06 04:08:57.831947 TeenStudy-0.1.7/TeenStudy/web/api/home.py
--rw-r--r--   0        0        0     6317 2023-05-06 04:13:39.518045 TeenStudy-0.1.7/TeenStudy/web/api/login.py
--rw-r--r--   0        0        0       78 2023-05-06 04:08:57.832963 TeenStudy-0.1.7/TeenStudy/web/pages/__init__.py
--rw-r--r--   0        0        0    33787 2023-05-06 07:57:07.633870 TeenStudy-0.1.7/TeenStudy/web/pages/add.py
--rw-r--r--   0        0        0    67310 2023-05-06 08:27:27.918859 TeenStudy-0.1.7/TeenStudy/web/pages/admin.py
--rw-r--r--   0        0        0    17385 2023-05-06 06:46:36.426467 TeenStudy-0.1.7/TeenStudy/web/pages/home.py
--rw-r--r--   0        0        0     1731 2023-05-06 04:08:57.834965 TeenStudy-0.1.7/TeenStudy/web/pages/login.py
--rw-r--r--   0        0        0       24 2023-05-06 04:08:57.834965 TeenStudy-0.1.7/TeenStudy/web/utils/__init__.py
--rw-r--r--   0        0        0     1902 2023-05-06 04:08:57.835965 TeenStudy-0.1.7/TeenStudy/web/utils/add.py
--rw-r--r--   0        0        0     2240 2023-05-06 04:08:57.835965 TeenStudy-0.1.7/TeenStudy/web/utils/status.py
--rw-r--r--   0        0        0    11422 1970-01-01 00:00:00.000000 TeenStudy-0.1.7/setup.py
--rw-r--r--   0        0        0    11188 1970-01-01 00:00:00.000000 TeenStudy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-06 04:08:57.731309 TeenStudy-0.1.8/LICENSE
+-rw-r--r--   0        0        0      955 2023-05-10 18:20:01.034562 TeenStudy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    10288 2023-05-10 18:01:43.120708 TeenStudy-0.1.8/README.md
+-rw-r--r--   0        0        0      666 2023-05-06 04:16:34.547526 TeenStudy-0.1.8/TeenStudy/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-06 04:08:57.732319 TeenStudy-0.1.8/TeenStudy/models/__init__.py
+-rw-r--r--   0        0        0     3547 2023-05-06 04:08:57.733777 TeenStudy-0.1.8/TeenStudy/models/accuont.py
+-rw-r--r--   0        0        0     3621 2023-05-06 04:08:57.733777 TeenStudy-0.1.8/TeenStudy/models/dxx.py
+-rw-r--r--   0        0        0   881164 2023-05-06 04:08:57.790011 TeenStudy-0.1.8/TeenStudy/resource/answer.png
+-rw-r--r--   0        0        0    52240 2023-05-06 04:08:57.791011 TeenStudy-0.1.8/TeenStudy/resource/backgroud1.jpg
+-rw-r--r--   0        0        0    52119 2023-05-06 04:08:57.792437 TeenStudy-0.1.8/TeenStudy/resource/backgroud2.jpg
+-rw-r--r--   0        0        0    52136 2023-05-06 04:08:57.792437 TeenStudy-0.1.8/TeenStudy/resource/backgroud3.jpg
+-rw-r--r--   0        0        0    51874 2023-05-06 04:08:57.793437 TeenStudy-0.1.8/TeenStudy/resource/backgroud4.jpg
+-rw-r--r--   0        0        0    51634 2023-05-06 04:08:57.793437 TeenStudy-0.1.8/TeenStudy/resource/backgroud5.jpg
+-rw-r--r--   0        0        0 10424793 2023-05-06 04:08:57.825443 TeenStudy-0.1.8/TeenStudy/resource/dxx_jx.json
+-rw-r--r--   0        0        0  7977480 2023-05-06 04:08:57.787010 TeenStudy-0.1.8/TeenStudy/resource/MiSans-Light.ttf
+-rw-r--r--   0        0        0      121 2023-05-06 04:08:57.826444 TeenStudy-0.1.8/TeenStudy/utils/__init__.py
+-rw-r--r--   0        0        0    50820 2023-05-10 17:47:30.917047 TeenStudy-0.1.8/TeenStudy/utils/dxx.py
+-rw-r--r--   0        0        0    18819 2023-05-06 06:32:36.543523 TeenStudy-0.1.8/TeenStudy/utils/handle.py
+-rw-r--r--   0        0        0     4331 2023-05-06 08:28:06.723801 TeenStudy-0.1.8/TeenStudy/utils/path.py
+-rw-r--r--   0        0        0     2026 2023-05-06 04:08:57.828444 TeenStudy-0.1.8/TeenStudy/utils/rule.py
+-rw-r--r--   0        0        0    10411 2023-05-06 06:39:01.954182 TeenStudy-0.1.8/TeenStudy/utils/update.py
+-rw-r--r--   0        0        0    23823 2023-05-10 17:40:59.938434 TeenStudy-0.1.8/TeenStudy/utils/utils.py
+-rw-r--r--   0        0        0     2185 2023-05-06 04:08:57.830444 TeenStudy-0.1.8/TeenStudy/web/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-06 04:08:57.830444 TeenStudy-0.1.8/TeenStudy/web/api/__init__.py
+-rw-r--r--   0        0        0    38557 2023-05-10 17:45:47.240033 TeenStudy-0.1.8/TeenStudy/web/api/add.py
+-rw-r--r--   0        0        0    11925 2023-05-06 04:08:57.831445 TeenStudy-0.1.8/TeenStudy/web/api/admin.py
+-rw-r--r--   0        0        0     4706 2023-05-06 04:08:57.831947 TeenStudy-0.1.8/TeenStudy/web/api/home.py
+-rw-r--r--   0        0        0     6317 2023-05-06 04:13:39.518045 TeenStudy-0.1.8/TeenStudy/web/api/login.py
+-rw-r--r--   0        0        0       78 2023-05-06 04:08:57.832963 TeenStudy-0.1.8/TeenStudy/web/pages/__init__.py
+-rw-r--r--   0        0        0    37024 2023-05-10 17:14:19.988383 TeenStudy-0.1.8/TeenStudy/web/pages/add.py
+-rw-r--r--   0        0        0    71180 2023-05-10 17:14:19.996044 TeenStudy-0.1.8/TeenStudy/web/pages/admin.py
+-rw-r--r--   0        0        0    17385 2023-05-06 06:46:36.426467 TeenStudy-0.1.8/TeenStudy/web/pages/home.py
+-rw-r--r--   0        0        0     1731 2023-05-06 04:08:57.834965 TeenStudy-0.1.8/TeenStudy/web/pages/login.py
+-rw-r--r--   0        0        0       24 2023-05-06 04:08:57.834965 TeenStudy-0.1.8/TeenStudy/web/utils/__init__.py
+-rw-r--r--   0        0        0     1902 2023-05-06 04:08:57.835965 TeenStudy-0.1.8/TeenStudy/web/utils/add.py
+-rw-r--r--   0        0        0     2240 2023-05-06 04:08:57.835965 TeenStudy-0.1.8/TeenStudy/web/utils/status.py
+-rw-r--r--   0        0        0    11750 1970-01-01 00:00:00.000000 TeenStudy-0.1.8/setup.py
+-rw-r--r--   0        0        0    11508 1970-01-01 00:00:00.000000 TeenStudy-0.1.8/PKG-INFO
```

### Comparing `TeenStudy-0.1.7/LICENSE` & `TeenStudy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/pyproject.toml` & `TeenStudy-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "TeenStudy"
-version = "0.1.7"
+version = "0.1.8"
 description = "基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图"
 authors = ["ZM25XC <xingling25@qq.com>"]
 license="MIT"
 readme="README.md"
 homepage="https://github.com/ZM25XC/TeenStudy"
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `TeenStudy-0.1.7/README.md` & `TeenStudy-0.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
   </div>
 
 ## 说明
 
 - 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版
 - 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档
 -  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**
+-  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**
 - 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交
 - 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常
 - 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。
 - 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试
 
 - 觉得项目不错，不妨点个stars.
 
@@ -32,14 +33,15 @@
 <details>
 
 | 共青团名称 | 开发状态 | 备注 |
 |:-----:|:----:|:----:|
 |青春湖北|支持|无需抓包|
 |江西共青团|支持|无需抓包|
 |安徽共青团|支持|无需抓包|
+|广东共青团|支持|无需抓包|
 |青春上海|支持|微信扫码绑定|
 |青春浙江|支持|微信扫码绑定|
 |江苏共青团|支持|需要自行抓包|
 |青春山东|支持|需要自行抓包|
 |重庆共青团|支持|需要自行抓包|
 |吉青飞扬|支持|需要自行抓包|
 |天府新青年|支持|不进入公众号token时效大于1周|
@@ -54,15 +56,14 @@
 |内蒙古青年|待开发||
 |云南共青团|待开发||
 |三秦青年|待开发||
 |青春北京|待开发||
 |海南共青团|待开发||
 |津彩青春|待开发||
 |青春黔言|待开发||
-|广东共青团|待开发||
 |青春柳州|待开发||
 |辽宁共青团|待开发||
 |宁夏共青团|待开发||
 |新疆共青团|待开发||
 |西藏共青团|待开发||
 </details>
 
@@ -155,21 +156,28 @@
 
 - [ ] 增加更多地区支持
 - [ ] 优化 Bot
 
 
 ## 更新日志
 
-### 2023/05/06
+### 2023/05/11
+
+- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试
+
+
+<details>
+<summary>2023/05/06</summary> 
 
 - 增加吉林地区，需要自行抓包
 - 修复超管更改登录密码后用原密码能继续登录问题
 - 添加二维码转链接开关，需要自行在后台配置页面打开
 - 调整部分依赖
 
+</details>
 
 <details>
 <summary> 2023/04/12</summary> 
 
 - 因河南地区cookie时效小于1周，移除河南地区
 - 添加`删除大学习`功能，用户可自行删除数据
 - 添加`导出用户数据`功能
```

#### html2text {}

```diff
@@ -7,42 +7,44 @@
                            license] [QQ_Chat_Group]
 ## è¯´æ - æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/ZM25XC/
 nonebot_plugin_auto_teenstudy) `Web UI`ç - æ¬é¡¹ç®åºäº[nonebot2](https://
 github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£ -
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**
 -
+**æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**
+-
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤
 -
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸
 - æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã
 -
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯
 - è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars. ## å°åºç¶æ  | å±éå¢åç§° |
 å¼åç¶æ | å¤æ³¨ | |:-----:|:----:|:----:
 | |éæ¥æ¹å|æ¯æ|æ éæå| |æ±è¥¿å±éå¢|æ¯æ|æ éæå|
-|å®å¾½å±éå¢|æ¯æ|æ éæå| |éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|å®å¾½å±éå¢|æ¯æ|æ éæå| |å¹¿ä¸å±éå¢|æ¯æ|æ éæå|
+|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|
 |éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|
 |éåºå±éå¢|æ¯æ|éè¦èªè¡æå|
 |åéé£æ¬|æ¯æ|éè¦èªè¡æå|
 |å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|
 |æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
 |é»é¾æ±å±éå¢|å¾å¼å|| |å¹¿è¥¿éå¹´å|å¾å¼å||
 |éæ¥æ¹å|å¾å¼å|| |çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
 |æ²³åå±éå¢|å¾å¼å|| |ç¦å»ºå±éå¢|å¾å¼å||
 |åèå¤éå¹´|å¾å¼å|| |äºåå±éå¢|å¾å¼å||
 |ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
 |æµ·åå±éå¢|å¾å¼å|| |æ´¥å½©éæ¥|å¾å¼å||
-|éæ¥é»è¨|å¾å¼å|| |å¹¿ä¸å±éå¢|å¾å¼å||
-|éæ¥æ³å·|å¾å¼å|| |è¾½å®å±éå¢|å¾å¼å||
-|å®å¤å±éå¢|å¾å¼å|| |æ°çå±éå¢|å¾å¼å||
-|è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°  ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) -
-ä½¿ç¨`git clone https://github.com/ZM25XC/
+|éæ¥é»è¨|å¾å¼å|| |éæ¥æ³å·|å¾å¼å||
+|è¾½å®å±éå¢|å¾å¼å|| |å®å¤å±éå¢|å¾å¼å||
+|æ°çå±éå¢|å¾å¼å|| |è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°
+ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) - ä½¿ç¨`git clone https://github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶   ç¬¬äºç§æ¹å¼
 (äºéä¸) 1ãä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip install
 TeenStudy -U`è¿è¡æ´æ° 2ãä½¿ç¨`nb plugin install
 TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`nb plugin install TeenStudy -U`è¿è¡æ´æ°
 ## å¯¼å¥æä»¶  ä½¿ç¨ç¬¬ä¸ç§æ¹å¼å®è£çæ­¤æ¹æ³ -
 å°`TeenStudy`æ¾å¨nbç`plugins`ç®å½ä¸ï¼è¿è¡nbæºå¨äººå³å¯ -
 æä»¶ç»æå¦ä¸ ```py ð¦ AweSome-Bot âââ ð awesome_bot â
@@ -74,18 +76,21 @@
 UIé»è®¤éç½® | | éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID |
 |å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|
 |å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|
 |æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|
 |æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|
 ## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿ ###
-2023/05/06 - å¢å åæå°åºï¼éè¦èªè¡æå -
+2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/ZM25XC/
+TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
+neal240)æä¾è´¦å·æµè¯  2023/05/06 -
+å¢å åæå°åºï¼éè¦èªè¡æå -
 ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢ -
 æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼ -
-è°æ´é¨åä¾èµ   2023/04/12 -
+è°æ´é¨åä¾èµ    2023/04/12 -
 å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ® -
 æ·»å `å¯¼åºç¨æ·æ°æ®`åè½ - æ·»å `æ´æ°ç¨æ·æ°æ®`åè½ -
 æ·»å `æ´æ°èµæºæ°æ®`åè½ï¼æ±è¥¿å°åºæ´æ°åè¯·ä½¿ç¨ä¸æ­¤åè½å·æ°å¢æ¯é¨æ°æ®
 - æ·»å æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹ -
 æ·»å å¤§å­¦ä¹ æéå¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
```

### Comparing `TeenStudy-0.1.7/TeenStudy/__init__.py` & `TeenStudy-0.1.8/TeenStudy/__init__.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/models/accuont.py` & `TeenStudy-0.1.8/TeenStudy/models/accuont.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/models/dxx.py` & `TeenStudy-0.1.8/TeenStudy/models/dxx.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/resource/answer.png` & `TeenStudy-0.1.8/TeenStudy/resource/answer.png`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/resource/backgroud1.jpg` & `TeenStudy-0.1.8/TeenStudy/resource/backgroud1.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/resource/backgroud2.jpg` & `TeenStudy-0.1.8/TeenStudy/resource/backgroud2.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/resource/backgroud3.jpg` & `TeenStudy-0.1.8/TeenStudy/resource/backgroud3.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/resource/backgroud4.jpg` & `TeenStudy-0.1.8/TeenStudy/resource/backgroud4.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/resource/backgroud5.jpg` & `TeenStudy-0.1.8/TeenStudy/resource/backgroud5.jpg`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/resource/dxx_jx.json` & `TeenStudy-0.1.8/TeenStudy/resource/dxx_jx.json`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/resource/MiSans-Light.ttf` & `TeenStudy-0.1.8/TeenStudy/resource/MiSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/utils/dxx.py` & `TeenStudy-0.1.8/TeenStudy/utils/dxx.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import random
 import re
 import secrets
 import time
+import urllib.parse
 
 from anti_useragent import UserAgent
 from httpx import AsyncClient
 from nonebot import logger
 
 from ..models.accuont import User, Commit
 from ..models.dxx import Answer
@@ -901,7 +902,176 @@
                 }
         except Exception as e:
             logger.error(e)
             return {
                 "status": 500,
                 "msg": f"提交失败,{e}"
             }
+
+
+async def guangdong(user_id: int) -> dict:
+    """
+    广东共青团
+    :param user_id:用户ID
+    :return:
+    """
+    result = await User.filter(user_id=user_id).values()
+    if not result:
+        return {
+            "status": 500,
+            "msg": "用户数据不存在！"
+        }
+    else:
+        dxx_id = result[0]['dxx_id']
+        token = result[0]["token"]
+        answer = await Answer.all().order_by("time").values()
+        try:
+            study_headers = {
+                'Host': 'youthstudy.12355.net',
+                'Connection': 'keep-alive',
+                'X-Litemall-Token': token,
+                'X-Litemall-IdentiFication': 'young',
+                'User-Agent': 'MicroMessenger',
+                'Accept': '*/*',
+                'Origin': 'https://youthstudy.12355.net',
+                'X-Requested-With': 'com.tencent.mm',
+                'Sec-Fetch-Site': 'same-origin',
+                'Sec-Fetch-Mode': 'cors',
+                'Sec-Fetch-Dest': 'empty',
+                'Referer': 'https://youthstudy.12355.net/h5/',
+                'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+            }
+            new_study_url = "https://youthstudy.12355.net/saomah5/api/young/chapter/new"
+            async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
+                study_response = await client.get(url=new_study_url)
+            study_response.encoding=study_response.charset_encoding
+            if study_response.json()["errno"] == 0:
+                chapterId = study_response.json().get('data').get('entity').get('id')
+                title = study_response.json().get('data').get('entity').get('name').replace('“青年大学习”', "").strip()
+                commit_url = "https://youthstudy.12355.net/saomah5/api/young/course/chapter/saveHistory"
+                async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
+                    commit_response = await client.post(url=commit_url, data={
+                        "chapterId": chapterId
+                    })
+                if commit_response.json()["errno"] == 0:
+                    await User.filter(user_id=user_id).update(
+                        token=token,
+                        commit_time=time.time(),
+                        catalogue=title
+                    )
+                    await commit(user_id=user_id, catalogue=title, status=True)
+                    return {
+                        "status": 0,
+                        "catalogue": title,
+                        "msg": "提交成功！"
+                    }
+                else:
+                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                    return {
+                        "status": 500,
+                        "msg": "提交失败！"
+                    }
+            else:
+                token_headers = {
+                    'Host': 'tuanapi.12355.net',
+                    'Connection': 'keep-alive',
+                    'Accept': 'application/json, text/javascript, */*; q=0.01',
+                    'Origin': 'https://tuan.12355.net',
+                    'User-Agent': 'MicroMessenger',
+                    'X-Requested-With': 'com.tencent.mm',
+                    'Sec-Fetch-Site': 'same-site',
+                    'Sec-Fetch-Mode': 'cors',
+                    'Referer': 'https://tuan.12355.net/wechat/view/YouthLearning/page.html',
+                    'Accept-Encoding': 'gzip, deflate',
+                    'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+                }
+                ger_param_url = f"https://tuanapi.12355.net/questionnaire/getYouthLearningUrl?mid={dxx_id}"
+                async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
+                    param_response = await client.get(url=ger_param_url)
+                    if param_response.json()["status"] == 200:
+                        content = param_response.json()["youthLearningUrl"].split("=")[-1]
+                        token_url = "https://youthstudy.12355.net/apih5/api/user/get"
+                        token_headers = {
+                            'Host': 'youthstudy.12355.net',
+                            'Connection': 'keep-alive',
+                            'Content-Length': '134',
+                            'Origin': 'https://youthstudy.12355.net',
+                            'X-Litemall-Token': '',
+                            'X-Litemall-IdentiFication': 'young',
+                            'User-Agent': 'MicroMessenger',
+                            'Content-Type': 'application/x-www-form-urlencoded',
+                            'Accept': '*/*',
+                            'X-Requested-With': 'com.tencent.mm',
+                            'Sec-Fetch-Site': 'same-origin',
+                            'Sec-Fetch-Mode': 'cors',
+                            'Referer': 'https://youthstudy.12355.net/h5/',
+                            'Accept-Encoding': 'gzip, deflate',
+                            'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7'
+                        }
+                        async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
+                            token_response = await client.post(url=token_url, data="sign="+urllib.parse.quote(content))
+                        if token_response.json()["errno"] == 0:
+                            token = token_response.json()['data']['entity']['token']
+                            study_headers = {
+                                'Host': 'youthstudy.12355.net',
+                                'Connection': 'keep-alive',
+                                'X-Litemall-Token': token,
+                                'X-Litemall-IdentiFication': 'young',
+                                'User-Agent': 'MicroMessenger',
+                                'Accept': '*/*',
+                                'Origin': 'https://youthstudy.12355.net',
+                                'X-Requested-With': 'com.tencent.mm',
+                                'Sec-Fetch-Site': 'same-origin',
+                                'Sec-Fetch-Mode': 'cors',
+                                'Sec-Fetch-Dest': 'empty',
+                                'Referer': 'https://youthstudy.12355.net/h5/',
+                                'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+                            }
+                            new_study_url = "https://youthstudy.12355.net/saomah5/api/young/chapter/new"
+                            async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
+                                study_response = await client.get(url=new_study_url)
+                            if study_response.json()["errno"] == 0:
+                                chapterId = study_response.json().get('data').get('entity').get('id')
+                                title = study_response.json().get('data').get('entity').get('name').replace(
+                                    '"青年大学习”', "").strip()
+                                commit_url = "https://youthstudy.12355.net/saomah5/api/young/course/chapter/saveHistory"
+                                async with AsyncClient(headers=study_headers, timeout=30, max_redirects=5) as client:
+                                    commit_response = await client.post(url=commit_url, data={
+                                        "chapterId": chapterId
+                                    })
+                                if commit_response.json()["errno"] == 0:
+                                    await User.filter(user_id=user_id).update(
+                                        token=token,
+                                        commit_time=time.time(),
+                                        catalogue=title
+                                    )
+                                    await commit(user_id=user_id, catalogue=title, status=True)
+                                    return {
+                                        "status": 0,
+                                        "catalogue": title,
+                                        "msg": "提交成功！"
+                                    }
+                                else:
+                                    await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                                    return {
+                                        "status": 500,
+                                        "msg": "提交失败！"
+                                    }
+                        else:
+                            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                            return {
+                                "status": 500,
+                                "msg": "提交失败，token获取失效！"
+                            }
+                    else:
+                        await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+                        return {
+                            "status": 500,
+                            "msg": "提交失败，token获取失效！"
+                        }
+        except Exception as e:
+            logger.error(e)
+            await commit(user_id=user_id, catalogue=answer[-1]["catalogue"], status=False)
+            return {
+                "status": 500,
+                "msg": "提交失败！"
+            }
```

### Comparing `TeenStudy-0.1.7/TeenStudy/utils/handle.py` & `TeenStudy-0.1.8/TeenStudy/utils/handle.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/utils/path.py` & `TeenStudy-0.1.8/TeenStudy/utils/path.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/utils/rule.py` & `TeenStudy-0.1.8/TeenStudy/utils/rule.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/utils/update.py` & `TeenStudy-0.1.8/TeenStudy/utils/update.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/utils/utils.py` & `TeenStudy-0.1.8/TeenStudy/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,23 @@
         "host": "jqfy.jl54.org",
         "referer": None,
         "origin": "http://jqfy.jl54.org/jltw/wechat",
         "url": "http://jqfy.jl54.org/jltw/wechat",
         "status": True,
         "catalogue": None
     },
+    {
+        "area": "广东",
+        "host": "tuanapi.12355.net",
+        "referer": None,
+        "origin": "https://tuan.12355.net",
+        "url": "https://youthstudy.12355.net/saomah5/api/young/chapter/new",
+        "status": True,
+        "catalogue": None
+    },
 ]
 RESOURCE = [
     {
         "name": "MiSans-Light.ttf",
         "url": "",
         "type": "字体",
         "size": "7.6 M"
@@ -502,14 +511,16 @@
         return await dxx.sichuan(user_id=user_id)
     elif area == "山东":
         return await dxx.shandong(user_id=user_id)
     elif area == "重庆":
         return await dxx.chongqing(user_id=user_id)
     elif area == "吉林":
         return await dxx.jilin(user_id=user_id)
+    elif area == "广东":
+        return await dxx.guangdong(user_id=user_id)
     else:
         return {
             "status": 404,
             "msg": "该地区暂未支持！"
         }
 
 
@@ -527,14 +538,16 @@
         province = "sichuan"
     elif province == "山东":
         province = "shandong"
     elif province == "重庆":
         province = "chongqing"
     elif province == "吉林":
         province = "jilin"
+    elif province == "广东":
+        province="guangdong"
     data = f"http://{config['DXX_IP']}:{config['DXX_PORT']}/TeenStudy/api/{province}?user_id={user_id}&group_id={group_id}"
     img = qrcode.make(data=data)
     buf = BytesIO()
     img.save(buf, format="PNG")
     base64_str = base64.b64encode(buf.getbuffer()).decode()
     content = "base64://" + base64_str
     return {
```

### Comparing `TeenStudy-0.1.7/TeenStudy/web/__init__.py` & `TeenStudy-0.1.8/TeenStudy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/web/api/add.py` & `TeenStudy-0.1.8/TeenStudy/web/api/add.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 import re
 import time
+import urllib.parse
 from typing import Optional
 
 from fastapi import APIRouter
 from fastapi.responses import HTMLResponse, JSONResponse, RedirectResponse
 from httpx import AsyncClient
 
 from ..pages.add import hubei_page, jiangxi_page, jiangsu_page, anhui_page, sichuan_page, shandong_page, \
-    chongqing_page, jilin_page
+    chongqing_page, jilin_page, guangdong_page
 from ..utils.add import write_to_database
 from ...models.accuont import User, AddUser
 from ...models.dxx import JiangXi
 
 route = APIRouter()
 
 
@@ -647,15 +648,15 @@
 
 
 @route.post("/jilin/add", response_class=HTMLResponse)
 async def jilin_add(data: dict) -> JSONResponse:
     user_id = data["user_id"]
     if await User.filter(user_id=user_id).count():
         return JSONResponse({
-            "status": 0,
+            "status": 500,
             "msg": "添加失败！，用户信息存在！"
         })
     else:
         try:
             openid = data["openid"]
             headers = {
                 "Host": "jqfy.jl54.org",
@@ -714,7 +715,102 @@
         return jilin_page.render(
             site_title='吉青飞扬 | TeenStudy',
             site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
         )
     return RedirectResponse(
         url="/TeenStudy/login"
     )
+
+
+@route.post("/guangdong/add", response_class=HTMLResponse)
+async def guangdong_add(data: dict) -> JSONResponse:
+    user_id = data["user_id"]
+    if await User.filter(user_id=user_id).count():
+        return JSONResponse({
+            "status": 500,
+            "msg": "添加失败！，用户信息存在！"
+        })
+    else:
+        try:
+            url = data["url"]
+            dxx_id = re.findall(r"memberId=(.*?)&showMemberAdditionNames", url)[0]
+            token_headers = {
+                'Host': 'tuanapi.12355.net',
+                'Connection': 'keep-alive',
+                'Accept': 'application/json, text/javascript, */*; q=0.01',
+                'Origin': 'https://tuan.12355.net',
+                'User-Agent': 'MicroMessenger',
+                'X-Requested-With': 'com.tencent.mm',
+                'Sec-Fetch-Site': 'same-site',
+                'Sec-Fetch-Mode': 'cors',
+                'Referer': 'https://tuan.12355.net/wechat/view/YouthLearning/page.html',
+                'Accept-Encoding': 'gzip, deflate',
+                'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7',
+            }
+            ger_param_url = f"https://tuanapi.12355.net/questionnaire/getYouthLearningUrl?mid={dxx_id}"
+            async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
+                param_response = await client.get(url=ger_param_url)
+                if param_response.json()["status"] == 200:
+                    content = param_response.json()["youthLearningUrl"].split("=")[-1]
+                    token_url = "https://youthstudy.12355.net/apih5/api/user/get"
+                    token_headers = {
+                        'Host': 'youthstudy.12355.net',
+                        'Connection': 'keep-alive',
+                        'Origin': 'https://youthstudy.12355.net',
+                        'X-Litemall-Token': '',
+                        'X-Litemall-IdentiFication': 'young',
+                        'User-Agent': 'MicroMessenger',
+                        'Content-Type': 'application/x-www-form-urlencoded',
+                        'Accept': '*/*',
+                        'X-Requested-With': 'com.tencent.mm',
+                        'Sec-Fetch-Site': 'same-origin',
+                        'Sec-Fetch-Mode': 'cors',
+                        'Referer': 'https://youthstudy.12355.net/h5/',
+                        'Accept-Encoding': 'gzip, deflate',
+                        'Accept-Language': 'zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7'
+                    }
+                    async with AsyncClient(headers=token_headers, timeout=30, max_redirects=5) as client:
+                        token_response = await client.post(url=token_url, data="sign="+urllib.parse.quote(content))
+                    if token_response.json()["errno"] == 0:
+                        token = token_response.json()['data']['entity']['token']
+                        name = token_response.json()['data']['entity']['nickName']
+                        organization_id = token_response.json()['data']['entity']['organizeId']
+                        data["name"] = name
+                        data["organization_id"] = organization_id
+                        data["dxx_id"] = dxx_id
+                        data["token"]=token
+                        data.pop("url")
+                        status = await write_to_database(data=data)
+                        if status:
+                            return JSONResponse(
+                                {
+                                    "status": 0,
+                                    "msg": "添加成功！"
+                                }
+                            )
+                        else:
+                            return JSONResponse({
+                                "status": 500,
+                                "msg": "添加失败！"
+                            })
+                    else:
+                        return JSONResponse({"status": 500, "msg": "添加失败！"})
+                else:
+                    return JSONResponse({"status": 500, "msg": "添加失败！"})
+        except Exception as e:
+            return JSONResponse({
+                "status": 500,
+                "msg": f"添加失败,{e}"
+            })
+
+
+@route.get("/guangdong", response_class=HTMLResponse)
+async def guangdong(user_id: int, group_id: int):
+    result = await AddUser.filter(user_id=user_id, group_id=group_id, status="未通过").count()
+    if result:
+        return guangdong_page.render(
+            site_title='广东共青团 | TeenStudy',
+            site_icon="https://i.328888.xyz/2023/02/23/xIh5k.png"
+        )
+    return RedirectResponse(
+        url="/TeenStudy/login"
+    )
```

### Comparing `TeenStudy-0.1.7/TeenStudy/web/api/admin.py` & `TeenStudy-0.1.8/TeenStudy/web/api/admin.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/web/api/home.py` & `TeenStudy-0.1.8/TeenStudy/web/api/home.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/web/api/login.py` & `TeenStudy-0.1.8/TeenStudy/web/api/login.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/web/pages/add.py` & `TeenStudy-0.1.8/TeenStudy/web/pages/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -838,7 +838,103 @@
             maxLength=32
         )
 
     ]
 )
 
 jilin_page = Page(title='添加大学习', body=[logo, Divider(), jilin_table, footer])
+
+guangdong_table = Form(
+    title="广东共青团",
+    mode=DisplayModeEnum.horizontal,
+    api="post:/TeenStudy/api/guangdong/add",
+    redirect="/TeenStudy/login",
+    body=[
+        Alert(level=LevelEnum.info,
+              className='white-space-pre-wrap',
+              body=(
+                  "链接获取方式:\n12355青春之声公众号\n智慧团建-认证资料-生成电子团员证，点击最下方生成按钮。\n在团员证页面复制链接 应为：https://tuan.12355.net/wechat/view/information/member_certification_generated.html?memberId=xxxxxx&showMemberAdditionNames=&showMemberRewardIds=&isShowAllFee=true \n其中xxxxxx即为mid")),
+        InputText(
+            label="用户ID",
+            description="用户ID，为用户QQ号，无需填写",
+            name="user_id",
+            value="${user_id}",
+            disabled=True
+        ),
+        InputText(
+            label="通知群ID",
+            description="通知群号，无需填写",
+            name="group_id",
+            value="${group_id}",
+            disabled=True
+        ),
+        InputText(
+            label="地区",
+            description="所处省份",
+            name="area",
+            value="广东",
+            disabled=True
+        ),
+        InputText(
+            label="登录密码",
+            type='input-password',
+            description="可不填，默认为用户ID",
+            name="password",
+            inline=False,
+            required=False,
+            value="",
+            clearable=True,
+            maxLength=16
+        ),
+        InputText(
+            label="姓名",
+            description="您的姓名",
+            name="name",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=8
+        ),
+        InputText(
+            label="url",
+            description="链接格式：https://tuan.12355.net/wechat/view/information/member_certification_generated.html?memberId=xxxxxx&showMemberAdditionNames=&showMemberRewardIds=&isShowAllFee=true",
+            name="url",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=512
+        ),
+        InputText(
+            label="学校",
+            description="你就读的高校",
+            name="university",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=24
+        ),
+        InputText(
+            label="学院",
+            description="学院名称",
+            name="college",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=32
+        ),
+        InputText(
+            label="团支部",
+            description="团支部|班级，没有可不填",
+            name="organization",
+            inline=False,
+            required=False,
+            value="",
+            clearable=True,
+            maxLength=32
+        )]
+)
+
+guangdong_page = Page(title='添加大学习', body=[logo, Divider(), guangdong_table, footer])
```

#### html2text {}

```diff
@@ -328,8 +328,38 @@
 description="ä½ å°±è¯»çé«æ ¡", name="university", inline=False,
 required=True, value="", clearable=True, maxLength=24 ), InputText
 ( label="å­¦é¢", description="å­¦é¢åç§°", name="college", inline=False,
 required=True, value="", clearable=True, maxLength=32 ), InputText
 ( label="å¢æ¯é¨", description="å¢æ¯é¨|ç­çº§ï¼æ²¡æå¯ä¸å¡«",
 name="organization", inline=False, required=False, value="", clearable=True,
 maxLength=32 ) ] ) jilin_page = Page(title='æ·»å å¤§å­¦ä¹ ', body=[logo,
-Divider(), jilin_table, footer])
+Divider(), jilin_table, footer]) guangdong_table = Form
+( title="å¹¿ä¸å±éå¢", mode=DisplayModeEnum.horizontal, api="post:/
+TeenStudy/api/guangdong/add", redirect="/TeenStudy/login", body=[ Alert
+(level=LevelEnum.info, className='white-space-pre-wrap', body=
+( "é¾æ¥è·åæ¹å¼:\n12355éæ¥ä¹å£°å¬ä¼å·\næºæ§å¢å»º-è®¤è¯èµæ-
+çæçµå­å¢åè¯ï¼ç¹å»æä¸æ¹çææé®ã\nå¨å¢åè¯é¡µé¢å¤å¶é¾æ¥
+åºä¸ºï¼https://tuan.12355.net/wechat/view/information/
+member_certification_generated.html?memberId=xxxxxx&showMemberAdditionNames=&showMemberRewardIds=&isShowAllFee=true
+\nå¶ä¸­xxxxxxå³ä¸ºmid")), InputText( label="ç¨æ·ID",
+description="ç¨æ·IDï¼ä¸ºç¨æ·QQå·ï¼æ éå¡«å", name="user_id",
+value="${user_id}", disabled=True ), InputText( label="éç¥ç¾¤ID",
+description="éç¥ç¾¤å·ï¼æ éå¡«å", name="group_id", value="$
+{group_id}", disabled=True ), InputText( label="å°åº",
+description="æå¤çä»½", name="area", value="å¹¿ä¸", disabled=True ),
+InputText( label="ç»å½å¯ç ", type='input-password',
+description="å¯ä¸å¡«ï¼é»è®¤ä¸ºç¨æ·ID", name="password", inline=False,
+required=False, value="", clearable=True, maxLength=16 ), InputText
+( label="å§å", description="æ¨çå§å", name="name", inline=False,
+required=True, value="", clearable=True, maxLength=8 ), InputText( label="url",
+description="é¾æ¥æ ¼å¼ï¼https://tuan.12355.net/wechat/view/information/
+member_certification_generated.html?memberId=xxxxxx&showMemberAdditionNames=&showMemberRewardIds=&isShowAllFee=true",
+name="url", inline=False, required=True, value="", clearable=True,
+maxLength=512 ), InputText( label="å­¦æ ¡", description="ä½ å°±è¯»çé«æ ¡",
+name="university", inline=False, required=True, value="", clearable=True,
+maxLength=24 ), InputText( label="å­¦é¢", description="å­¦é¢åç§°",
+name="college", inline=False, required=True, value="", clearable=True,
+maxLength=32 ), InputText( label="å¢æ¯é¨",
+description="å¢æ¯é¨|ç­çº§ï¼æ²¡æå¯ä¸å¡«", name="organization",
+inline=False, required=False, value="", clearable=True, maxLength=32 )] )
+guangdong_page = Page(title='æ·»å å¤§å­¦ä¹ ', body=[logo, Divider(),
+guangdong_table, footer])
```

### Comparing `TeenStudy-0.1.7/TeenStudy/web/pages/admin.py` & `TeenStudy-0.1.8/TeenStudy/web/pages/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1390,14 +1390,123 @@
             value="",
             clearable=True,
             maxLength=32
         )
 
     ]
 )
+"""广东地区添加用户"""
+guangdong_table = Form(
+    title="广东共青团",
+    mode=DisplayModeEnum.horizontal,
+    api="post:/TeenStudy/api/guangdong/add",
+    redirect="/TeenStudy/login",
+    body=[
+        Alert(level=LevelEnum.info,
+              className='white-space-pre-wrap',
+              body=(
+                  "链接获取方式:\n12355青春之声公众号\n智慧团建-认证资料-生成电子团员证，点击最下方生成按钮。\n在团员证页面复制链接 应为：https://tuan.12355.net/wechat/view/information/member_certification_generated.html?memberId=xxxxxx&showMemberAdditionNames=&showMemberRewardIds=&isShowAllFee=true \n其中xxxxxx即为mid")),
+        Select(
+            label="群聊",
+            name="group_id",
+            description="需要添加的群组",
+            checkAll=False,
+            source="get:/TeenStudy/api/get_group_list",
+            value='',
+            multiple=False,
+            required=True,
+            searchable=True,
+            joinValues=False,
+            extractValue=True,
+            statistics=True,
+        ),
+        Select(
+            label="用户ID",
+            name="user_id",
+            description="需要添加的用户ID",
+            checkAll=False,
+            source="get:/TeenStudy/api/get_member_list?group_id=${group_id}",
+            value='',
+            multiple=False,
+            required=True,
+            searchable=True,
+            joinValues=False,
+            extractValue=True,
+            statistics=True,
+            hiddenOn="${group_id==''?true:false}"
+        ),
+        InputText(
+            label="地区",
+            description="所处省份",
+            name="area",
+            value="广东",
+            disabled=True
+        ),
+        InputText(
+            label="登录密码",
+            type='input-password',
+            description="可不填，默认为用户ID",
+            name="password",
+            inline=False,
+            required=False,
+            value="",
+            clearable=True,
+            maxLength=16
+        ),
+        InputText(
+            label="姓名",
+            description="您的姓名",
+            name="name",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=8
+        ),
+        InputText(
+            label="url",
+            description="链接格式：https://tuan.12355.net/wechat/view/information/member_certification_generated.html?memberId=xxxxxx&showMemberAdditionNames=&showMemberRewardIds=&isShowAllFee=true",
+            name="url",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=512
+        ),
+        InputText(
+            label="学校",
+            description="你就读的高校",
+            name="university",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=24
+        ),
+        InputText(
+            label="学院",
+            description="学院名称",
+            name="college",
+            inline=False,
+            required=True,
+            value="",
+            clearable=True,
+            maxLength=32
+        ),
+        InputText(
+            label="团支部",
+            description="团支部|班级，没有可不填",
+            name="organization",
+            inline=False,
+            required=False,
+            value="",
+            clearable=True,
+            maxLength=32
+        )]
+)
 """推送群聊模板"""
 push_table = CRUD(mode='table',
                   title='',
                   syncLocation=False,
                   api='/TeenStudy/api/get_push_list',
                   type='crud',
                   headerToolbar=[ActionType.Ajax(label='删除所有推送群聊',
@@ -1471,23 +1580,25 @@
                           schema=Page(title='天府新青年', body=[sichuan_table]))
 shandong_page = PageSchema(url='/add/shandong', icon='fa fa-pen-to-square', label='青春山东',
                            schema=Page(title='青春山东', body=[shandong_table]))
 chongqing_page = PageSchema(url='/add/chongqing', icon='fa fa-pen-to-square', label='重庆共青团',
                             schema=Page(title='重庆共青团', body=[chongqing_table]))
 jilin_page = PageSchema(url='/add/jilin', icon='fa fa-pen-to-square', label='吉青飞扬',
                         schema=Page(title='吉青飞扬', body=[jilin_table]))
+guangdong_page = PageSchema(url='/add/guangdong', icon='fa fa-pen-to-square', label='广东共青团',
+                        schema=Page(title='广东共青团', body=[guangdong_table]))
 admin_app = App(brandName='TeenStudy',
                 logo='https://i.328888.xyz/2023/02/23/xIh5k.png',
                 header=header,
                 pages=[{
                     'children': [
                         admin_page,
                         PageSchema(icon='fa fa-circle-user', label='成员管理',
                                    children=[list_page, hubei_page, jiangxi_page, jiangsu_page, anhui_page,
-                                             sichuan_page, shandong_page, chongqing_page, jilin_page]),
+                                             sichuan_page, shandong_page, chongqing_page, jilin_page,guangdong_page]),
                         PageSchema(url="/notice", label='推送列表', icon='fa fa-bell',
                                    schema=Page(title='', body=[push_table])),
                         PageSchema(url="/request", label='申请记录', icon='fa fa-circle-info',
                                    schema=Page(title='', body=[request_table])),
                         PageSchema(url="/answer", label='大学习列表', icon='fa fa-book-open',
                                    schema=Page(title='', body=[answer_table])),
                         PageSchema(url="/records", label='提交记录', icon='fa fa-code-commit',
```

#### html2text {}

```diff
@@ -549,16 +549,49 @@
 value="", clearable=True, ), InputText( label="å­¦æ ¡",
 description="ä½ å°±è¯»çé«æ ¡", name="university", inline=False,
 required=True, value="", clearable=True, maxLength=24 ), InputText
 ( label="å­¦é¢", description="å­¦é¢åç§°", name="college", inline=False,
 required=True, value="", clearable=True, maxLength=32 ), InputText
 ( label="å¢æ¯é¨", description="å¢æ¯é¨|ç­çº§ï¼æ²¡æå¯ä¸å¡«",
 name="organization", inline=False, required=False, value="", clearable=True,
-maxLength=32 ) ] ) """æ¨éç¾¤èæ¨¡æ¿""" push_table = CRUD(mode='table',
-title='', syncLocation=False, api='/TeenStudy/api/get_push_list', type='crud',
+maxLength=32 ) ] ) """å¹¿ä¸å°åºæ·»å ç¨æ·""" guangdong_table = Form
+( title="å¹¿ä¸å±éå¢", mode=DisplayModeEnum.horizontal, api="post:/
+TeenStudy/api/guangdong/add", redirect="/TeenStudy/login", body=[ Alert
+(level=LevelEnum.info, className='white-space-pre-wrap', body=
+( "é¾æ¥è·åæ¹å¼:\n12355éæ¥ä¹å£°å¬ä¼å·\næºæ§å¢å»º-è®¤è¯èµæ-
+çæçµå­å¢åè¯ï¼ç¹å»æä¸æ¹çææé®ã\nå¨å¢åè¯é¡µé¢å¤å¶é¾æ¥
+åºä¸ºï¼https://tuan.12355.net/wechat/view/information/
+member_certification_generated.html?memberId=xxxxxx&showMemberAdditionNames=&showMemberRewardIds=&isShowAllFee=true
+\nå¶ä¸­xxxxxxå³ä¸ºmid")), Select( label="ç¾¤è", name="group_id",
+description="éè¦æ·»å çç¾¤ç»", checkAll=False, source="get:/TeenStudy/
+api/get_group_list", value='', multiple=False, required=True, searchable=True,
+joinValues=False, extractValue=True, statistics=True, ), Select
+( label="ç¨æ·ID", name="user_id", description="éè¦æ·»å çç¨æ·ID",
+checkAll=False, source="get:/TeenStudy/api/get_member_list?group_id=$
+{group_id}", value='', multiple=False, required=True, searchable=True,
+joinValues=False, extractValue=True, statistics=True, hiddenOn="$
+{group_id==''?true:false}" ), InputText( label="å°åº",
+description="æå¤çä»½", name="area", value="å¹¿ä¸", disabled=True ),
+InputText( label="ç»å½å¯ç ", type='input-password',
+description="å¯ä¸å¡«ï¼é»è®¤ä¸ºç¨æ·ID", name="password", inline=False,
+required=False, value="", clearable=True, maxLength=16 ), InputText
+( label="å§å", description="æ¨çå§å", name="name", inline=False,
+required=True, value="", clearable=True, maxLength=8 ), InputText( label="url",
+description="é¾æ¥æ ¼å¼ï¼https://tuan.12355.net/wechat/view/information/
+member_certification_generated.html?memberId=xxxxxx&showMemberAdditionNames=&showMemberRewardIds=&isShowAllFee=true",
+name="url", inline=False, required=True, value="", clearable=True,
+maxLength=512 ), InputText( label="å­¦æ ¡", description="ä½ å°±è¯»çé«æ ¡",
+name="university", inline=False, required=True, value="", clearable=True,
+maxLength=24 ), InputText( label="å­¦é¢", description="å­¦é¢åç§°",
+name="college", inline=False, required=True, value="", clearable=True,
+maxLength=32 ), InputText( label="å¢æ¯é¨",
+description="å¢æ¯é¨|ç­çº§ï¼æ²¡æå¯ä¸å¡«", name="organization",
+inline=False, required=False, value="", clearable=True, maxLength=32 )] )
+"""æ¨éç¾¤èæ¨¡æ¿""" push_table = CRUD(mode='table', title='',
+syncLocation=False, api='/TeenStudy/api/get_push_list', type='crud',
 headerToolbar=[ActionType.Ajax(label='å é¤æææ¨éç¾¤è',
 level=LevelEnum.warning, confirmText='ç¡®å®è¦å é¤æææ¨éç¾¤èåï¼',
 api='delete:/TeenStudy/api/delete_all?type=push_list'), "bulkActions",
 "reload", ActionType.Dialog( label='æ·»å æ¨éç¾¤è', level=LevelEnum.info,
 icon='fa fa-plus', dialog=Dialog(title='æ·»å æ¨éç¾¤è', size='lg', body=
 [ Form(title='', api='post:/TeenStudy/api/add_push', submitText='æ·»å ',
 mode=DisplayModeEnum.horizontal, labelAlign='right', body=[Select
@@ -594,23 +627,25 @@
 pen-to-square', label='å¤©åºæ°éå¹´', schema=Page(title='å¤©åºæ°éå¹´',
 body=[sichuan_table])) shandong_page = PageSchema(url='/add/shandong', icon='fa
 fa-pen-to-square', label='éæ¥å±±ä¸', schema=Page(title='éæ¥å±±ä¸',
 body=[shandong_table])) chongqing_page = PageSchema(url='/add/chongqing',
 icon='fa fa-pen-to-square', label='éåºå±éå¢', schema=Page
 (title='éåºå±éå¢', body=[chongqing_table])) jilin_page = PageSchema
 (url='/add/jilin', icon='fa fa-pen-to-square', label='åéé£æ¬',
-schema=Page(title='åéé£æ¬', body=[jilin_table])) admin_app = App
-(brandName='TeenStudy', logo='https://i.328888.xyz/2023/02/23/xIh5k.png',
-header=header, pages=[{ 'children': [ admin_page, PageSchema(icon='fa fa-
-circle-user', label='æåç®¡ç', children=[list_page, hubei_page,
-jiangxi_page, jiangsu_page, anhui_page, sichuan_page, shandong_page,
-chongqing_page, jilin_page]), PageSchema(url="/notice", label='æ¨éåè¡¨',
-icon='fa fa-bell', schema=Page(title='', body=[push_table])), PageSchema(url="/
-request", label='ç³è¯·è®°å½', icon='fa fa-circle-info', schema=Page(title='',
-body=[request_table])), PageSchema(url="/answer", label='å¤§å­¦ä¹ åè¡¨',
-icon='fa fa-book-open', schema=Page(title='', body=[answer_table])), PageSchema
-(url="/records", label='æäº¤è®°å½', icon='fa fa-code-commit', schema=Page
-(title='', body=[record_table])), PageSchema(url="/setting", label='éç½®',
-icon='fa fa-gear', schema=Page(title='', body=[setting_table])), ]}],
-footer=Html( html=f'
+schema=Page(title='åéé£æ¬', body=[jilin_table])) guangdong_page =
+PageSchema(url='/add/guangdong', icon='fa fa-pen-to-square',
+label='å¹¿ä¸å±éå¢', schema=Page(title='å¹¿ä¸å±éå¢', body=
+[guangdong_table])) admin_app = App(brandName='TeenStudy', logo='https://
+i.328888.xyz/2023/02/23/xIh5k.png', header=header, pages=[{ 'children':
+[ admin_page, PageSchema(icon='fa fa-circle-user', label='æåç®¡ç',
+children=[list_page, hubei_page, jiangxi_page, jiangsu_page, anhui_page,
+sichuan_page, shandong_page, chongqing_page, jilin_page,guangdong_page]),
+PageSchema(url="/notice", label='æ¨éåè¡¨', icon='fa fa-bell', schema=Page
+(title='', body=[push_table])), PageSchema(url="/request",
+label='ç³è¯·è®°å½', icon='fa fa-circle-info', schema=Page(title='', body=
+[request_table])), PageSchema(url="/answer", label='å¤§å­¦ä¹ åè¡¨', icon='fa
+fa-book-open', schema=Page(title='', body=[answer_table])), PageSchema(url="/
+records", label='æäº¤è®°å½', icon='fa fa-code-commit', schema=Page(title='',
+body=[record_table])), PageSchema(url="/setting", label='éç½®', icon='fa fa-
+gear', schema=Page(title='', body=[setting_table])), ]}], footer=Html( html=f'
 Copyright Â© 2022 - 2023 TeenStudy Xamis_v2.2.0
 '))
```

### Comparing `TeenStudy-0.1.7/TeenStudy/web/pages/home.py` & `TeenStudy-0.1.8/TeenStudy/web/pages/home.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/web/pages/login.py` & `TeenStudy-0.1.8/TeenStudy/web/pages/login.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/web/utils/add.py` & `TeenStudy-0.1.8/TeenStudy/web/utils/add.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/TeenStudy/web/utils/status.py` & `TeenStudy-0.1.8/TeenStudy/web/utils/status.py`

 * *Files identical despite different names*

### Comparing `TeenStudy-0.1.7/setup.py` & `TeenStudy-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,17 @@
  'qrcode>=7.4.2,<8.0.0',
  'tortoise-orm>=0.19.3,<0.20.0',
  'ujson>=5.7.0,<6.0.0',
  'uvicorn>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'teenstudy',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': '基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图',
-    'long_description': '<div align="center">\n    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>\n    <h1>TeenStudy</h1>\n    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>\n    <br/>\n    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>\n  \t<a href="https://pypi.python.org/pypi/TeenStudy">\n    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>\n\t  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  </div>\n\n## 说明\n\n- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版\n- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档\n-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**\n- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交\n- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常\n- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。\n- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试\n\n- 觉得项目不错，不妨点个stars.\n\n## 地区状态\n\n<details>\n\n| 共青团名称 | 开发状态 | 备注 |\n|:-----:|:----:|:----:|\n|青春湖北|支持|无需抓包|\n|江西共青团|支持|无需抓包|\n|安徽共青团|支持|无需抓包|\n|青春上海|支持|微信扫码绑定|\n|青春浙江|支持|微信扫码绑定|\n|江苏共青团|支持|需要自行抓包|\n|青春山东|支持|需要自行抓包|\n|重庆共青团|支持|需要自行抓包|\n|吉青飞扬|支持|需要自行抓包|\n|天府新青年|支持|不进入公众号token时效大于1周|\n|河南共青团|不支持|cookie时效小于1周|\n|黑龙江共青团|待开发||\n|广西青年圈|待开发||\n|青春湖南|待开发||\n|甘肃青年|待开发||\n|山西青年|待开发||\n|河北共青团|待开发||\n|福建共青团|待开发||\n|内蒙古青年|待开发||\n|云南共青团|待开发||\n|三秦青年|待开发||\n|青春北京|待开发||\n|海南共青团|待开发||\n|津彩青春|待开发||\n|青春黔言|待开发||\n|广东共青团|待开发||\n|青春柳州|待开发||\n|辽宁共青团|待开发||\n|宁夏共青团|待开发||\n|新疆共青团|待开发||\n|西藏共青团|待开发||\n</details>\n\n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n1、使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新\n2、使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 TeenStudy\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`\n\n</details>\n\n## 机器人配置\n\n- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP\n\n  ```py\n  HOST = "0.0.0.0"  #nonebot2监听的IP\n  SUPERUSERS = [""] # 超级用户\n  COMMAND_START=[""] # 命令前缀,根据需要自行修改\n  DXX_IP = ""\n  ```\n\n## 使用方式\n\n- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）\n- 在管理后台的推送列表中添加需要开启大学习使用的群聊\n\n## 功能列表\n|    指令    |               指令格式               |                               说明                               |\n| :--------: | :----------------------------------: | :--------------------------------------------------------------: |\n| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |\n| 我的大学习 |              我的大学习              |                           查询个人信息                           |\n| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |\n|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |\n|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |\n| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |\n|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |\n|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |\n|删除大学习|删除大学习|用户申请清除数据库的信息|\n|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|\n|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|\n|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|\n\n\n## ToDo\n\n\n- [ ] 增加更多地区支持\n- [ ] 优化 Bot\n\n\n## 更新日志\n\n### 2023/05/06\n\n- 增加吉林地区，需要自行抓包\n- 修复超管更改登录密码后用原密码能继续登录问题\n- 添加二维码转链接开关，需要自行在后台配置页面打开\n- 调整部分依赖\n\n\n<details>\n<summary> 2023/04/12</summary> \n\n- 因河南地区cookie时效小于1周，移除河南地区\n- 添加`删除大学习`功能，用户可自行删除数据\n- 添加`导出用户数据`功能\n- 添加`更新用户数据`功能\n- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据\n- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改\n- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改\n- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改\n- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法\n- 修复Web UI 首页公网IP显示异常\n- 修复浙江地区用户重复显示\n- 更新江西共青团团支部数据\n  \n</details>\n\n\n<details>\n<summary>2023/03/18</summary>\n\n- 适配河南地区，需要自行抓包\n- 适配四川地区，需要自行抓包\n- 适配山东地区，需要自行抓包\n- 适配重庆地区，需要自行抓包\n- 添加自动获取公网IP功能，别再问如何配置公网IP啦\n- 添加重置密码功能，指令`重置密码`\n- 添加重置配置功能，指令`重置配置`，`刷新配置`\n- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`\n- 管理后台开放添加用户权限（浙江，上海地区无法添加）\n- 优化用户信息页\n- 优化登录界面提示\n- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些\n- 修复Ubuntu系统导入资源失败BUG\n  \n</details>\n\n<details>\n\n<summary>2023/03/05</summary>\n\n- 适配浙江地区，使用微信扫码进行绑定\n- 适配上海地区，使用微信扫码进行绑定\n- 适配江苏地区，需要自行抓包\n- 适配安徽地区，需要自行抓包\n\n</details>\n\n<details>\n<summary>2023/03/01</summary>\n\n- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件\n- 上传基础代码\n- 适配湖北地区，无需抓包，安装即用\n- 适配江西地区，无需抓包，安装即用\n\n</details>\n',
+    'long_description': '<div align="center">\n    <img src="https://i.328888.xyz/2023/02/28/z23ho.png" alt="TeenStudy.png" border="0" width="500px" height="500px"/>\n    <h1>TeenStudy</h1>\n    <b>基于nonebot2和go-cqhttp的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图</b>\n    <br/>\n    <a href="https://github.com/ZM25XC/TeenStudy/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://github.com/ZM25XC/TeenStudy/stargazers"><img alt="GitHub stars" src="https://img.shields.io/github/stars/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://pypi.python.org/pypi/TeenStudy"><img src="https://img.shields.io/pypi/v/TeenStudy?color=yellow" alt="pypi"></a>\n  \t<a href="https://pypi.python.org/pypi/TeenStudy">\n    <img src="https://img.shields.io/pypi/dm/TeenStudy" alt="pypi download"></a>\n\t  <a href="https://github.com/ZM25XC/TeenStudy/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/ZM25XC/TeenStudy?style=flat-square"></a>\n    <a href="https://jq.qq.com/?_wv=1027&k=NGFEwXyS">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-511173803-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  </div>\n\n## 说明\n\n- 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版\n- 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档\n-  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**\n-  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**\n- 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交\n- 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常\n- 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。\n- 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试\n\n- 觉得项目不错，不妨点个stars.\n\n## 地区状态\n\n<details>\n\n| 共青团名称 | 开发状态 | 备注 |\n|:-----:|:----:|:----:|\n|青春湖北|支持|无需抓包|\n|江西共青团|支持|无需抓包|\n|安徽共青团|支持|无需抓包|\n|广东共青团|支持|无需抓包|\n|青春上海|支持|微信扫码绑定|\n|青春浙江|支持|微信扫码绑定|\n|江苏共青团|支持|需要自行抓包|\n|青春山东|支持|需要自行抓包|\n|重庆共青团|支持|需要自行抓包|\n|吉青飞扬|支持|需要自行抓包|\n|天府新青年|支持|不进入公众号token时效大于1周|\n|河南共青团|不支持|cookie时效小于1周|\n|黑龙江共青团|待开发||\n|广西青年圈|待开发||\n|青春湖南|待开发||\n|甘肃青年|待开发||\n|山西青年|待开发||\n|河北共青团|待开发||\n|福建共青团|待开发||\n|内蒙古青年|待开发||\n|云南共青团|待开发||\n|三秦青年|待开发||\n|青春北京|待开发||\n|海南共青团|待开发||\n|津彩青春|待开发||\n|青春黔言|待开发||\n|青春柳州|待开发||\n|辽宁共青团|待开发||\n|宁夏共青团|待开发||\n|新疆共青团|待开发||\n|西藏共青团|待开发||\n</details>\n\n\n##  安装及更新\n\n<details>\n<summary>第一种方式(不推荐)</summary>\n\n- 使用`git clone https://github.com/ZM25XC/TeenStudy.git`指令克隆本仓库或下载压缩包文件\n\n</details>\n\n<details>\n<summary>第二种方式(二选一)</summary>\n\n1、使用`pip install TeenStudy`来进行安装,使用`pip install TeenStudy -U`进行更新\n2、使用`nb plugin install TeenStudy`来进行安装,使用`nb plugin install TeenStudy -U`进行更新\n\n</details>\n\n\n## 导入插件\n\n<details>\n<summary>使用第一种方式安装看此方法</summary>\n\n- 将`TeenStudy`放在nb的`plugins`目录下，运行nb机器人即可\n\n- 文件结构如下\n\n    ```py\n    📦 AweSome-Bot\n    ├── 📂 awesome_bot\n    │   └── 📂 plugins\n    |       └── 📂 TeenStudy\n    |           └── 📜 __init__.py\n    ├── 📜 .env.prod\n    ├── 📜 .gitignore\n    ├── 📜 pyproject.toml\n    └── 📜 README.md\n    ```\n\n    \n\n</details>\n\n<details>\n<summary>使用第二种方式安装看此方法</summary>\n\n- 在`pyproject.toml`里的`[tool.nonebot]`中添加`plugins = ["TeenStudy"]`\n\n</details>\n\n## 机器人配置\n\n- 在nonebot的`.env` 或 `.env.prod`配置文件中修改nonebot2的`HOST`为`0.0.0.0`、设置好超管账号和公网IP\n\n  ```py\n  HOST = "0.0.0.0"  #nonebot2监听的IP\n  SUPERUSERS = [""] # 超级用户\n  COMMAND_START=[""] # 命令前缀,根据需要自行修改\n  DXX_IP = ""\n  ```\n\n## 使用方式\n\n- 启动nb,等待插件加载数据，加载完毕后登录后台，账号默认为`nonebot配置文件中的超管账号`，密码默认为：`admin`,开放端口（默认为.env中配置的port）\n- 在管理后台的推送列表中添加需要开启大学习使用的群聊\n\n## 功能列表\n|    指令    |               指令格式               |                               说明                               |\n| :--------: | :----------------------------------: | :--------------------------------------------------------------: |\n| 添加大学习 |           添加大学习`地区`           |                    添加大学习湖北 添加大学习                     |\n| 我的大学习 |              我的大学习              |                           查询个人信息                           |\n| 提交大学习 |         提交大学习 戳一戳Bot         |                        提交最新一期大学习                        |\n|   大学习   |     大学习答案、大学习、答案截图     |                    获取最新一期青年大学习答案                    |\n|  完成截图  | 完成截图、大学习截图、大学习完成截图 |            获取最新一期青年大学习完成截图（带状态栏）            |\n| 完成大学习 |        完成大学习、全员大学习        | 团支书可用，需要成员填写团支书ID，填写后团支书可发指令提交大学习 |\n|  重置配置  |          重置配置、刷新配置          |                   超管可用，刷新Web UI默认配置                   |\n|  重置密码  |               重置密码               |                   重置登录Web UI的密码为用户ID                   |\n|删除大学习|删除大学习|用户申请清除数据库的信息|\n|导出用户数据|导出用户数据、导出数据|将数据导出至TeenStudy目录下|\n|更新用户数据|更新用户数据、刷新用户数据|将用户数据导入到数据库|\n|更新资源数据|更新资源数据、刷新资源数据|更新数据库中的资源数据（江西共青团团支部数据）|\n\n\n## ToDo\n\n\n- [ ] 增加更多地区支持\n- [ ] 优化 Bot\n\n\n## 更新日志\n\n### 2023/05/11\n\n- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试\n\n\n<details>\n<summary>2023/05/06</summary> \n\n- 增加吉林地区，需要自行抓包\n- 修复超管更改登录密码后用原密码能继续登录问题\n- 添加二维码转链接开关，需要自行在后台配置页面打开\n- 调整部分依赖\n\n</details>\n\n<details>\n<summary> 2023/04/12</summary> \n\n- 因河南地区cookie时效小于1周，移除河南地区\n- 添加`删除大学习`功能，用户可自行删除数据\n- 添加`导出用户数据`功能\n- 添加`更新用户数据`功能\n- 添加`更新资源数据`功能，江西地区更新后请使用下此功能刷新团支部数据\n- 添加戳一戳提交大学习开关，默认开启，请在Web UI后台配置页面进行修改\n- 添加大学习提醒开关，默认开启，支持修改时间，请在Web UI后台配置页面进行修改\n- 添加自动提交大学习开关，默认开启，支持修改时间，请在Web UI后台进行修改\n- 调整安徽地区添加方式[#9](https://github.com/ZM25XC/TeenStudy/issues/9)，无需抓包，感谢[@yhzcake](https://github.com/yhzcake)测试提供方法\n- 修复Web UI 首页公网IP显示异常\n- 修复浙江地区用户重复显示\n- 更新江西共青团团支部数据\n  \n</details>\n\n\n<details>\n<summary>2023/03/18</summary>\n\n- 适配河南地区，需要自行抓包\n- 适配四川地区，需要自行抓包\n- 适配山东地区，需要自行抓包\n- 适配重庆地区，需要自行抓包\n- 添加自动获取公网IP功能，别再问如何配置公网IP啦\n- 添加重置密码功能，指令`重置密码`\n- 添加重置配置功能，指令`重置配置`，`刷新配置`\n- 添加完成大学习功能，团支书可一次性提交全班的大学习，指令`完成大学习`，`全员大学习`\n- 管理后台开放添加用户权限（浙江，上海地区无法添加）\n- 优化用户信息页\n- 优化登录界面提示\n- 将添加链接，登录链接转化成二维码，减少公网IP暴露，没啥用，样式好看一些\n- 修复Ubuntu系统导入资源失败BUG\n  \n</details>\n\n<details>\n\n<summary>2023/03/05</summary>\n\n- 适配浙江地区，使用微信扫码进行绑定\n- 适配上海地区，使用微信扫码进行绑定\n- 适配江苏地区，需要自行抓包\n- 适配安徽地区，需要自行抓包\n\n</details>\n\n<details>\n<summary>2023/03/01</summary>\n\n- 将代码上传至pypi，可使用`pip install TeenStudy`指令安装本插件\n- 上传基础代码\n- 适配湖北地区，无需抓包，安装即用\n- 适配江西地区，无需抓包，安装即用\n\n</details>\n',
     'author': 'ZM25XC',
     'author_email': 'xingling25@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ZM25XC/TeenStudy',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -6,37 +6,38 @@
 useragent>=1.0.10,<2.0.0', 'beautifulsoup4>=4.11.2,<5.0.0',
 'bs4>=0.0.1,<0.0.2', 'fastapi>=0.95.0,<0.96.0', 'httpx>=0.23.3,<0.24.0',
 'lxml>=4.9.2,<5.0.0', 'nonebot-adapter-onebot>=2.2.1,<3.0.0', 'nonebot-plugin-
 apscheduler>=0.2.0,<0.3.0', 'nonebot2>=2.0.0rc2,<3.0.0',
 'psutil>=5.9.4,<6.0.0', 'python-jose>=3.3.0,<4.0.0', 'qrcode>=7.4.2,<8.0.0',
 'tortoise-orm>=0.19.3,<0.20.0', 'ujson>=5.7.0,<6.0.0',
 'uvicorn>=0.21.0,<0.22.0'] setup_kwargs = { 'name': 'teenstudy', 'version':
-'0.1.7', 'description':
+'0.1.8', 'description':
 'åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾',
 'long_description': '
                              \n [TeenStudy.png]\n
                             ****** TeenStudy ******
                             \n åºäºnonebot2ågo-
 cqhttpçéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾\n
 
   \n [GitHub_issues]\n [GitHub_forks]\n [GitHub_stars]\n [pypi]\n \t\n_[pypi
             download]\n\t [GitHub_license]\n \n_[QQ_Chat_Group]\n\n
 \n\n## è¯´æ\n\n- æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/
 ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`ç\n- æ¬é¡¹ç®åºäº[nonebot2]
 (https://github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/
 go-cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£\n-
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**\n-
+**æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**\n-
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤\n-
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸\n-
 æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/
 ?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã\n-
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯\n\n-
 è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars.\n\n## å°åºç¶æ\n\n\n\n|
 å±éå¢åç§° | å¼åç¶æ | å¤æ³¨ |\n|:-----:|:----:|:----:
-|\n|éæ¥æ¹å|æ¯æ|æ éæå|\n|æ±è¥¿å±éå¢|æ¯æ|æ éæå|\n|å®å¾½å±éå¢|æ¯æ|æ éæå|\n|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|\n|éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|\n|éåºå±éå¢|æ¯æ|éè¦èªè¡æå|\n|åéé£æ¬|æ¯æ|éè¦èªè¡æå|\n|å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|\n|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|\n|é»é¾æ±å±éå¢|å¾å¼å||\n|å¹¿è¥¿éå¹´å|å¾å¼å||\n|éæ¥æ¹å|å¾å¼å||\n|çèéå¹´|å¾å¼å||\n|å±±è¥¿éå¹´|å¾å¼å||\n|æ²³åå±éå¢|å¾å¼å||\n|ç¦å»ºå±éå¢|å¾å¼å||\n|åèå¤éå¹´|å¾å¼å||\n|äºåå±éå¢|å¾å¼å||\n|ä¸ç§¦éå¹´|å¾å¼å||\n|éæ¥åäº¬|å¾å¼å||\n|æµ·åå±éå¢|å¾å¼å||\n|æ´¥å½©éæ¥|å¾å¼å||\n|éæ¥é»è¨|å¾å¼å||\n|å¹¿ä¸å±éå¢|å¾å¼å||\n|éæ¥æ³å·|å¾å¼å||\n|è¾½å®å±éå¢|å¾å¼å||\n|å®å¤å±éå¢|å¾å¼å||\n|æ°çå±éå¢|å¾å¼å||\n|è¥¿èå±éå¢|å¾å¼å||\n\n\n\n##
+|\n|éæ¥æ¹å|æ¯æ|æ éæå|\n|æ±è¥¿å±éå¢|æ¯æ|æ éæå|\n|å®å¾½å±éå¢|æ¯æ|æ éæå|\n|å¹¿ä¸å±éå¢|æ¯æ|æ éæå|\n|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|\n|æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|\n|éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|\n|éåºå±éå¢|æ¯æ|éè¦èªè¡æå|\n|åéé£æ¬|æ¯æ|éè¦èªè¡æå|\n|å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|\n|æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|\n|é»é¾æ±å±éå¢|å¾å¼å||\n|å¹¿è¥¿éå¹´å|å¾å¼å||\n|éæ¥æ¹å|å¾å¼å||\n|çèéå¹´|å¾å¼å||\n|å±±è¥¿éå¹´|å¾å¼å||\n|æ²³åå±éå¢|å¾å¼å||\n|ç¦å»ºå±éå¢|å¾å¼å||\n|åèå¤éå¹´|å¾å¼å||\n|äºåå±éå¢|å¾å¼å||\n|ä¸ç§¦éå¹´|å¾å¼å||\n|éæ¥åäº¬|å¾å¼å||\n|æµ·åå±éå¢|å¾å¼å||\n|æ´¥å½©éæ¥|å¾å¼å||\n|éæ¥é»è¨|å¾å¼å||\n|éæ¥æ³å·|å¾å¼å||\n|è¾½å®å±éå¢|å¾å¼å||\n|å®å¤å±éå¢|å¾å¼å||\n|æ°çå±éå¢|å¾å¼å||\n|è¥¿èå±éå¢|å¾å¼å||\n\n\n\n##
 å®è£åæ´æ°\n\n\nç¬¬ä¸ç§æ¹å¼(ä¸æ¨è)\n\n- ä½¿ç¨`git clone https://
 github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶\n\n\n\n\nç¬¬äºç§æ¹å¼
 (äºéä¸)\n\n1ãä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip
 install TeenStudy -U`è¿è¡æ´æ°\n2ãä½¿ç¨`nb plugin install
 TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`nb plugin install TeenStudy -
 U`è¿è¡æ´æ°\n\n\n\n\n##
@@ -68,18 +69,21 @@
 å®æå¤§å­¦ä¹  | å®æå¤§å­¦ä¹ ãå¨åå¤§å­¦ä¹  |
 å¢æ¯ä¹¦å¯ç¨ï¼éè¦æåå¡«åå¢æ¯ä¹¦IDï¼å¡«ååå¢æ¯ä¹¦å¯åæä»¤æäº¤å¤§å­¦ä¹ 
 |\n| éç½®éç½® | éç½®éç½®ãå·æ°éç½® | è¶ç®¡å¯ç¨ï¼å·æ°Web
 UIé»è®¤éç½® |\n| éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID
 |\n|å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|\n|å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|\n|æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|\n|æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|\n\n\n##
 ToDo\n\n\n- [ ] å¢å æ´å¤å°åºæ¯æ\n- [ ] ä¼å Bot\n\n\n##
-æ´æ°æ¥å¿\n\n### 2023/05/06\n\n- å¢å åæå°åºï¼éè¦èªè¡æå\n-
+æ´æ°æ¥å¿\n\n### 2023/05/11\n\n- å¢å å¹¿ä¸å°åºï¼æ éæå[#13]
+(https://github.com/ZM25XC/TeenStudy/issues/13)ï¼æè°¢[@neal240](https://
+github.com/neal240)æä¾è´¦å·æµè¯\n\n\n\n2023/05/06 \n\n-
+å¢å åæå°åºï¼éè¦èªè¡æå\n-
 ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢\n-
 æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼\n-
-è°æ´é¨åä¾èµ\n\n\n\n 2023/04/12 \n\n-
+è°æ´é¨åä¾èµ\n\n\n\n\n 2023/04/12 \n\n-
 å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº\n-
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ®\n-
 æ·»å `å¯¼åºç¨æ·æ°æ®`åè½\n- æ·»å `æ´æ°ç¨æ·æ°æ®`åè½\n-
 æ·»å `æ´æ°èµæºæ°æ®`åè½ï¼æ±è¥¿å°åºæ´æ°åè¯·ä½¿ç¨ä¸æ­¤åè½å·æ°å¢æ¯é¨æ°æ®\n-
 æ·»å æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹\n-
 æ·»å å¤§å­¦ä¹ æéå¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
```

### Comparing `TeenStudy-0.1.7/PKG-INFO` & `TeenStudy-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teenstudy
-Version: 0.1.7
+Version: 0.1.8
 Summary: 基于nonebot2异步框架的青年大学自动提交插件基于nonebot2的青年大学习自动提交插件，用于自动完成大学习，在后台留下记录，返回完成截图
 Home-page: https://github.com/ZM25XC/TeenStudy
 License: MIT
 Author: ZM25XC
 Author-email: xingling25@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -50,14 +50,15 @@
   </div>
 
 ## 说明
 
 - 本项目为[青年大学习提交](https://github.com/ZM25XC/nonebot_plugin_auto_teenstudy) `Web UI`版
 - 本项目基于[nonebot2](https://github.com/nonebot/nonebot2)和[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)，使用本插件前请先阅读以上两个项目的使用文档
 -  **启动插件之后，一定要登录后台在推送列表中添加需要开启大学习功能的群聊**
+-  **本项目无法在国外IP环境下使用，如有开启代理，请关闭或添加代理规则**
 - 需要抓包的地区，绑定后尽量别进官方公众号，避免token或cookie刷新导致无法提交
 - 本项目需要部署在公网可访问的容器中，并开放端口（nonebot2配置的port），否则大部分功能将出现异常
 - 欢迎加入[QQ群](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)，交流讨论。
 - 时间精力有限，目前只维护湖北和江西两个地区，其他地区出问题请提交Issues,我找个时间修，需要增加地区请进群帮忙测试，个别地区没账号无法测试
 
 - 觉得项目不错，不妨点个stars.
 
@@ -66,14 +67,15 @@
 <details>
 
 | 共青团名称 | 开发状态 | 备注 |
 |:-----:|:----:|:----:|
 |青春湖北|支持|无需抓包|
 |江西共青团|支持|无需抓包|
 |安徽共青团|支持|无需抓包|
+|广东共青团|支持|无需抓包|
 |青春上海|支持|微信扫码绑定|
 |青春浙江|支持|微信扫码绑定|
 |江苏共青团|支持|需要自行抓包|
 |青春山东|支持|需要自行抓包|
 |重庆共青团|支持|需要自行抓包|
 |吉青飞扬|支持|需要自行抓包|
 |天府新青年|支持|不进入公众号token时效大于1周|
@@ -88,15 +90,14 @@
 |内蒙古青年|待开发||
 |云南共青团|待开发||
 |三秦青年|待开发||
 |青春北京|待开发||
 |海南共青团|待开发||
 |津彩青春|待开发||
 |青春黔言|待开发||
-|广东共青团|待开发||
 |青春柳州|待开发||
 |辽宁共青团|待开发||
 |宁夏共青团|待开发||
 |新疆共青团|待开发||
 |西藏共青团|待开发||
 </details>
 
@@ -189,21 +190,28 @@
 
 - [ ] 增加更多地区支持
 - [ ] 优化 Bot
 
 
 ## 更新日志
 
-### 2023/05/06
+### 2023/05/11
+
+- 增加广东地区，无需抓包[#13](https://github.com/ZM25XC/TeenStudy/issues/13)，感谢[@neal240](https://github.com/neal240)提供账号测试
+
+
+<details>
+<summary>2023/05/06</summary> 
 
 - 增加吉林地区，需要自行抓包
 - 修复超管更改登录密码后用原密码能继续登录问题
 - 添加二维码转链接开关，需要自行在后台配置页面打开
 - 调整部分依赖
 
+</details>
 
 <details>
 <summary> 2023/04/12</summary> 
 
 - 因河南地区cookie时效小于1周，移除河南地区
 - 添加`删除大学习`功能，用户可自行删除数据
 - 添加`导出用户数据`功能
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teenstudy Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: teenstudy Version: 0.1.8 Summary:
 åºäºnonebot2å¼æ­¥æ¡æ¶çéå¹´å¤§å­¦èªå¨æäº¤æä»¶åºäºnonebot2çéå¹´å¤§å­¦ä¹ èªå¨æäº¤æä»¶ï¼ç¨äºèªå¨å®æå¤§å­¦ä¹ ï¼å¨åå°çä¸è®°å½ï¼è¿åå®ææªå¾
 Home-page: https://github.com/ZM25XC/TeenStudy License: MIT Author: ZM25XC
 Author-email: xingling25@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) Requires-Dist: Pillow (>=9.4.0,<10.0.0)
@@ -25,42 +25,44 @@
                            license] [QQ_Chat_Group]
 ## è¯´æ - æ¬é¡¹ç®ä¸º[éå¹´å¤§å­¦ä¹ æäº¤](https://github.com/ZM25XC/
 nonebot_plugin_auto_teenstudy) `Web UI`ç - æ¬é¡¹ç®åºäº[nonebot2](https://
 github.com/nonebot/nonebot2)å[go-cqhttp](https://github.com/Mrs4s/go-
 cqhttp)ï¼ä½¿ç¨æ¬æä»¶åè¯·åéè¯»ä»¥ä¸ä¸¤ä¸ªé¡¹ç®çä½¿ç¨ææ¡£ -
 **å¯å¨æä»¶ä¹åï¼ä¸å®è¦ç»å½åå°å¨æ¨éåè¡¨ä¸­æ·»å éè¦å¼å¯å¤§å­¦ä¹ åè½çç¾¤è**
 -
+**æ¬é¡¹ç®æ æ³å¨å½å¤IPç¯å¢ä¸ä½¿ç¨ï¼å¦æå¼å¯ä»£çï¼è¯·å³é­ææ·»å ä»£çè§å**
+-
 éè¦æåçå°åºï¼ç»å®åå°½éå«è¿å®æ¹å¬ä¼å·ï¼é¿åtokenæcookieå·æ°å¯¼è´æ æ³æäº¤
 -
 æ¬é¡¹ç®éè¦é¨ç½²å¨å¬ç½å¯è®¿é®çå®¹å¨ä¸­ï¼å¹¶å¼æ¾ç«¯å£ï¼nonebot2éç½®çportï¼ï¼å¦åå¤§é¨ååè½å°åºç°å¼å¸¸
 - æ¬¢è¿å å¥[QQç¾¤](https://jq.qq.com/?_wv=1027&k=NGFEwXyS)ï¼äº¤æµè®¨è®ºã
 -
 æ¶é´ç²¾åæéï¼ç®ååªç»´æ¤æ¹ååæ±è¥¿ä¸¤ä¸ªå°åºï¼å¶ä»å°åºåºé®é¢è¯·æäº¤Issues,ææ¾ä¸ªæ¶é´ä¿®ï¼éè¦å¢å å°åºè¯·è¿ç¾¤å¸®å¿æµè¯ï¼ä¸ªå«å°åºæ²¡è´¦å·æ æ³æµè¯
 - è§å¾é¡¹ç®ä¸éï¼ä¸å¦¨ç¹ä¸ªstars. ## å°åºç¶æ  | å±éå¢åç§° |
 å¼åç¶æ | å¤æ³¨ | |:-----:|:----:|:----:
 | |éæ¥æ¹å|æ¯æ|æ éæå| |æ±è¥¿å±éå¢|æ¯æ|æ éæå|
-|å®å¾½å±éå¢|æ¯æ|æ éæå| |éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
+|å®å¾½å±éå¢|æ¯æ|æ éæå| |å¹¿ä¸å±éå¢|æ¯æ|æ éæå|
+|éæ¥ä¸æµ·|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |éæ¥æµæ±|æ¯æ|å¾®ä¿¡æ«ç ç»å®|
 |æ±èå±éå¢|æ¯æ|éè¦èªè¡æå|
 |éæ¥å±±ä¸|æ¯æ|éè¦èªè¡æå|
 |éåºå±éå¢|æ¯æ|éè¦èªè¡æå|
 |åéé£æ¬|æ¯æ|éè¦èªè¡æå|
 |å¤©åºæ°éå¹´|æ¯æ|ä¸è¿å¥å¬ä¼å·tokenæ¶æå¤§äº1å¨|
 |æ²³åå±éå¢|ä¸æ¯æ|cookieæ¶æå°äº1å¨|
 |é»é¾æ±å±éå¢|å¾å¼å|| |å¹¿è¥¿éå¹´å|å¾å¼å||
 |éæ¥æ¹å|å¾å¼å|| |çèéå¹´|å¾å¼å|| |å±±è¥¿éå¹´|å¾å¼å||
 |æ²³åå±éå¢|å¾å¼å|| |ç¦å»ºå±éå¢|å¾å¼å||
 |åèå¤éå¹´|å¾å¼å|| |äºåå±éå¢|å¾å¼å||
 |ä¸ç§¦éå¹´|å¾å¼å|| |éæ¥åäº¬|å¾å¼å||
 |æµ·åå±éå¢|å¾å¼å|| |æ´¥å½©éæ¥|å¾å¼å||
-|éæ¥é»è¨|å¾å¼å|| |å¹¿ä¸å±éå¢|å¾å¼å||
-|éæ¥æ³å·|å¾å¼å|| |è¾½å®å±éå¢|å¾å¼å||
-|å®å¤å±éå¢|å¾å¼å|| |æ°çå±éå¢|å¾å¼å||
-|è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°  ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) -
-ä½¿ç¨`git clone https://github.com/ZM25XC/
+|éæ¥é»è¨|å¾å¼å|| |éæ¥æ³å·|å¾å¼å||
+|è¾½å®å±éå¢|å¾å¼å|| |å®å¤å±éå¢|å¾å¼å||
+|æ°çå±éå¢|å¾å¼å|| |è¥¿èå±éå¢|å¾å¼å||  ## å®è£åæ´æ°
+ç¬¬ä¸ç§æ¹å¼(ä¸æ¨è) - ä½¿ç¨`git clone https://github.com/ZM25XC/
 TeenStudy.git`æä»¤åéæ¬ä»åºæä¸è½½åç¼©åæä»¶   ç¬¬äºç§æ¹å¼
 (äºéä¸) 1ãä½¿ç¨`pip install TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`pip install
 TeenStudy -U`è¿è¡æ´æ° 2ãä½¿ç¨`nb plugin install
 TeenStudy`æ¥è¿è¡å®è£,ä½¿ç¨`nb plugin install TeenStudy -U`è¿è¡æ´æ°
 ## å¯¼å¥æä»¶  ä½¿ç¨ç¬¬ä¸ç§æ¹å¼å®è£çæ­¤æ¹æ³ -
 å°`TeenStudy`æ¾å¨nbç`plugins`ç®å½ä¸ï¼è¿è¡nbæºå¨äººå³å¯ -
 æä»¶ç»æå¦ä¸ ```py ð¦ AweSome-Bot âââ ð awesome_bot â
@@ -92,18 +94,21 @@
 UIé»è®¤éç½® | | éç½®å¯ç  | éç½®å¯ç  | éç½®ç»å½Web
 UIçå¯ç ä¸ºç¨æ·ID |
 |å é¤å¤§å­¦ä¹ |å é¤å¤§å­¦ä¹ |ç¨æ·ç³è¯·æ¸é¤æ°æ®åºçä¿¡æ¯|
 |å¯¼åºç¨æ·æ°æ®|å¯¼åºç¨æ·æ°æ®ãå¯¼åºæ°æ®|å°æ°æ®å¯¼åºè³TeenStudyç®å½ä¸|
 |æ´æ°ç¨æ·æ°æ®|æ´æ°ç¨æ·æ°æ®ãå·æ°ç¨æ·æ°æ®|å°ç¨æ·æ°æ®å¯¼å¥å°æ°æ®åº|
 |æ´æ°èµæºæ°æ®|æ´æ°èµæºæ°æ®ãå·æ°èµæºæ°æ®|æ´æ°æ°æ®åºä¸­çèµæºæ°æ®ï¼æ±è¥¿å±éå¢å¢æ¯é¨æ°æ®ï¼|
 ## ToDo - [ ] å¢å æ´å¤å°åºæ¯æ - [ ] ä¼å Bot ## æ´æ°æ¥å¿ ###
-2023/05/06 - å¢å åæå°åºï¼éè¦èªè¡æå -
+2023/05/11 - å¢å å¹¿ä¸å°åºï¼æ éæå[#13](https://github.com/ZM25XC/
+TeenStudy/issues/13)ï¼æè°¢[@neal240](https://github.com/
+neal240)æä¾è´¦å·æµè¯  2023/05/06 -
+å¢å åæå°åºï¼éè¦èªè¡æå -
 ä¿®å¤è¶ç®¡æ´æ¹ç»å½å¯ç åç¨åå¯ç è½ç»§ç»­ç»å½é®é¢ -
 æ·»å äºç»´ç è½¬é¾æ¥å¼å³ï¼éè¦èªè¡å¨åå°éç½®é¡µé¢æå¼ -
-è°æ´é¨åä¾èµ   2023/04/12 -
+è°æ´é¨åä¾èµ    2023/04/12 -
 å æ²³åå°åºcookieæ¶æå°äº1å¨ï¼ç§»é¤æ²³åå°åº -
 æ·»å `å é¤å¤§å­¦ä¹ `åè½ï¼ç¨æ·å¯èªè¡å é¤æ°æ® -
 æ·»å `å¯¼åºç¨æ·æ°æ®`åè½ - æ·»å `æ´æ°ç¨æ·æ°æ®`åè½ -
 æ·»å `æ´æ°èµæºæ°æ®`åè½ï¼æ±è¥¿å°åºæ´æ°åè¯·ä½¿ç¨ä¸æ­¤åè½å·æ°å¢æ¯é¨æ°æ®
 - æ·»å æ³ä¸æ³æäº¤å¤§å­¦ä¹ å¼å³ï¼é»è®¤å¼å¯ï¼è¯·å¨Web
 UIåå°éç½®é¡µé¢è¿è¡ä¿®æ¹ -
 æ·»å å¤§å­¦ä¹ æéå¼å³ï¼é»è®¤å¼å¯ï¼æ¯æä¿®æ¹æ¶é´ï¼è¯·å¨Web
```

