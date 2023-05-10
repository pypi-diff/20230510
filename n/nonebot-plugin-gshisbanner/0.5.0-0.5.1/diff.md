# Comparing `tmp/nonebot_plugin_gshisbanner-0.5.0.tar.gz` & `tmp/nonebot_plugin_gshisbanner-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gshisbanner-0.5.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_gshisbanner-0.5.1.tar", max compression
```

## Comparing `nonebot_plugin_gshisbanner-0.5.0.tar` & `nonebot_plugin_gshisbanner-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/LICENSE
--rw-r--r--   0        0        0     4598 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/README.md
--rw-r--r--   0        0        0      389 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/__init__.py
--rw-r--r--   0        0        0     1030 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/alias.py
--rw-r--r--   0        0        0      427 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/api.py
--rw-r--r--   0        0        0      292 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/config.py
--rw-r--r--   0        0        0     3663 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/deal.py
--rw-r--r--   0        0        0     1182 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/deal_json.py
--rw-r--r--   0        0        0     4454 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/main.py
--rw-r--r--   0        0        0     2654 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/send.py
--rw-r--r--   0        0        0      576 2023-04-21 15:45:24.169326 nonebot_plugin_gshisbanner-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5291 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/LICENSE
+-rw-r--r--   0        0        0     5295 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/README.md
+-rw-r--r--   0        0        0      389 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/__init__.py
+-rw-r--r--   0        0        0     1030 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/alias.py
+-rw-r--r--   0        0        0      427 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/api.py
+-rw-r--r--   0        0        0      292 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/config.py
+-rw-r--r--   0        0        0     3280 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/deal.py
+-rw-r--r--   0        0        0     1232 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/deal_json.py
+-rw-r--r--   0        0        0     4622 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/main.py
+-rw-r--r--   0        0        0     2654 2023-05-10 13:29:48.696538 nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/send.py
+-rw-r--r--   0        0        0      576 2023-05-10 13:29:48.700538 nonebot_plugin_gshisbanner-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5988 1970-01-01 00:00:00.000000 nonebot_plugin_gshisbanner-0.5.1/PKG-INFO
```

### Comparing `nonebot_plugin_gshisbanner-0.5.0/LICENSE` & `nonebot_plugin_gshisbanner-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.0/README.md` & `nonebot_plugin_gshisbanner-0.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/forchannot/nonebot-plugin-gshisbanner.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-gshisbanner">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-gshisbanner.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
+<br />
+<a href="https://onebot.dev/">
+    <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
+</a>
 </div>
 
 ## 📖 介绍
 
-本插件用于在机器人上查询原神历史卡池信息
+本插件用于在机器人上查询原神历史卡池信息（当前仅适用于qq）
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
@@ -63,19 +66,19 @@
      ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
 ·· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/gacha"
      ##jsdelivr代理的文件，大多数情况可用，推荐
 ```
 
 ## 🎉 使用
 ### 指令表
-|        指令         |    权限    | 需要@ | 范围 |                             说明                             |
-| :-----------------: | :--------: | :---: | :--: | :----------------------------------------------------------: |
-| [name]历史卡池(num) |    ALL     |  否   | ALL  | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
-| [version]卡池[num]  |    ALL     |  否   | ALL  | version为版本号，如1.3，2.6等，num为1-3，对应上半（中）下半，可不填，如不填则发送该版本全部卡池 |
-|  刷新历史卡池/别名  | 管理员以上 |  否   | ALL  |                      刷新历史卡池或别名                      |
+|        指令        |  权限   | 需要@ | 范围  |                                说明                                |
+|:----------------:|:-----:|:---:|:---:|:----------------------------------------------------------------:|
+| [name]历史卡池(num)  |  ALL  |  否  | ALL | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
+| [version]卡池[num] |  ALL  |  否  | ALL |    version为版本号，如1.3，2.6等，num为1-3，对应上半（中）下半，可不填，如不填则发送该版本全部卡池     |
+|  刷新(更新)历史卡池/别名   | 管理员以上 |  否  | ALL |                            刷新历史卡池或别名                             |
 ### 效果图
 <details>
 <summary>历史卡池效果图</summary>
 <details>
 <summary>图1</summary>
 <img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230324/image.4jlu5w0mhko0.jpg" alt="help">
 </details>
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-gshisbanner _â¨
  æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ â¨_ [license]
-                                [pypi] [python]
-## ð ä»ç» æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ ##
-ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+                               [pypi] [python]
+                                   [onebot]
+## ð ä»ç»
+æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ï¼å½åä»éç¨äºqqï¼
+## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-gshisbanner   pip pip install nonebot-plugin-gshisbanner
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_gshisbanner"]  ##
 âï¸ éç½® ``` gshisbanner_forward_length: int #
 åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 #
 è¶å¤§åæ¬¡è½¬ååå®¹æ´å¤ï¼åå¹¶è½¬åçæ¬¡æ°æ´å°ï¼è¶å°ååæ¬¡è½¬ååå®¹æ´å°ï¼ä½åå¹¶è½¬åçæ¬¡æ°æ´å¤
@@ -19,19 +21,19 @@
 3."genshin-gacha-banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â·
 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/
 gacha" ##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
 (éè¦æ¯æhttps) Â·Â· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/
 gacha" ##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :-------
-----------: | :--------: | :---: | :--: | :------------------------------------
-----------------------: | | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
+ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:--------
+--------:|:-----:|:---:|:---:|:------------------------------------------------
+----------------:| | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
-| | å·æ°åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
+| | å·æ°(æ´æ°)åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾  åå²å¡æ± ææå¾  å¾1 [help]
 å¾2 [help]   å¾3 [help]    çæ¬å¡æ± ææå¾  å¾1 [help]   å¾2 [help]
 å¾3 [help]    å·æ°å¡æ± /å«åææå¾ [help]  ### é¸£è°¢ [genshin-gacha-
 banners](https://github.com/KeyPJ/genshin-gacha-banners) #åå²upå¡æ± æ¥æº
```

### Comparing `nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/alias.py` & `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/alias.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/deal.py` & `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/deal.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,19 +26,15 @@
 ) -> List[Dict[str, Union[str, List[str]]]]:
     """
     :param name: 名字
     :param choose: 类型
     :return: 获取到的历史卡池数据
     """
     result = []
-    jsons = (
-        await get_info_from_url(True)
-        if choose == "cha"
-        else await get_info_from_url(False)
-    )
+    jsons = await get_info_from_url(choose == "cha")
     for data in jsons:
         for item in data["items"]:
             if item["name"] == name:
                 temp = {
                     "start": data["start"],
                     "end": data["end"],
                     "version": data["version"],
@@ -65,36 +61,35 @@
     version: str, is_all: bool
 ) -> List[Dict[str, Union[str, List[str]]]]:
     """
     :param version: 版本号
     :param is_all: 是否获取全部卡池
     :return: 获取到的历史卡池数据
     """
+    # 获取所有卡池信息
     json = await get_info_from_url(True) + await get_info_from_url(False)  # type: ignore
+    # 卡池类型列表
     type_list = ["five_character", "four_character", "five_weapon", "four_weapon"]
     result = []
     for data in json:
+        # 判断是否为指定版本
         if data["version"][:3] == version if is_all else data["version"] == version:
-            result.append(
-                {
-                    "start": data["start"],
-                    "end": data["end"],
-                    # 利用 zip 将 type_list 和得到的对应值的列表合并成一个元组，其中 type_list 作为键，得到的列表作为值,最后将元组转换成字典
-                    **dict(
-                        zip(
-                            type_list,
-                            (
-                                [
-                                    x["name"]
-                                    for x in data["items"]
-                                    if x.get("rankType") == (5 if "five" in item else 4)
-                                    and x.get("itemType")
-                                    == item.split("_")[1].capitalize()
-                                ]
-                                for item in type_list
-                            ),
-                        )
-                    ),
-                    "version": data["version"],
-                }
-            )
+            # 构造卡池信息字典
+            temp = {
+                "start": data["start"],
+                "end": data["end"],
+                "version": data["version"],
+            }
+            # 遍历卡池类型列表
+            for item in type_list:
+                # 获取对应类型的卡池信息
+                temp[item] = [
+                    x["name"]
+                    for x in data["items"]
+                    if x.get("rankType") == (5 if "five" in item else 4)
+                    and x.get("itemType") == item.split("_")[1].capitalize()
+                ]
+            result.append(temp)
+    # 去除空值
     return [{k: v for k, v in data.items() if v} for data in result]
+
+
```

### Comparing `nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/deal_json.py` & `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/deal_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 async def load_json_from_url(
     url: str, path: Union[Path, str], force: bool = False
 ) -> Union[Dict, List[Dict]]:
     if path and Path(path).exists() and not force:
         return load_json(path=path)
     resp = await get(url)
+    if resp.status_code != 200:
+        return []
     try:
         data: Union[Dict, List[Dict]] = resp.json()
     except JSONDecodeError:
         return []
     if path and not Path(path).exists():
         save_json(data=data, path=path)
     return data
```

### Comparing `nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/main.py` & `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 version_gacha = on_regex(
     r"(?<!.)(?P<version>\d\.\d)(卡池|up)(?P<upordown>(1|2|3)?)(?!.)",
     priority=35,
     block=False,
 )
 refresh = on_regex(
-    r"(?<!.)刷新(?P<name>历史卡池|别名)(?!.)",
+    r"(?<!.)(刷新|更新)(?P<name>历史卡池|别名)(?!.)",
     permission=SUPERUSER | GROUP_ADMIN | GROUP_OWNER,
     priority=13,
     block=False,
 )
 
 DRIVER = get_driver()
 gacha_info_path = Path.cwd() / "data" / "genshin_history"
@@ -111,18 +111,21 @@
 
 
 @DRIVER.on_startup
 async def init_group_card():
     if not gacha_info_path.exists():
         gacha_info_path.mkdir(parents=True)
     url = "https://fastly.jsdelivr.net/gh/forchannot/nonebot-plugin-gshisbanner@main/data/genshin_history/alias.json"
+    if (gacha_info_path / "alias.json").exists():
+        logger.info("alias.json文件已存在，跳过下载，如需更新请使用刷新别名功能")
+        return
     try:
         resp = await get(url)
     except Exception as e:
         logger.warning(f"alias.json文件下载失败,错误信息:{e}")
-        return False
+        return
     if resp.status_code != 200:
         logger.warning("alias.json文件下载失败")
-        return False
+        return
     data = resp.json()
     save_json(data=data, path=gacha_info_path / "alias.json")
     logger.info("alias.json文件保存成功")
```

### Comparing `nonebot_plugin_gshisbanner-0.5.0/nonebot_plugin_gshisbanner/send.py` & `nonebot_plugin_gshisbanner-0.5.1/nonebot_plugin_gshisbanner/send.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gshisbanner-0.5.0/pyproject.toml` & `nonebot_plugin_gshisbanner-0.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gshisbanner"
-version = "0.5.0"
+version = "0.5.1"
 description = "Nonebot2查询原神历史卡池小插件"
 authors = ["forchannot <yy320206@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_gshisbanner"}]
 
 [[tool.poetry.source]]
```

### Comparing `nonebot_plugin_gshisbanner-0.5.0/PKG-INFO` & `nonebot_plugin_gshisbanner-0.5.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gshisbanner
-Version: 0.5.0
+Version: 0.5.1
 Summary: Nonebot2查询原神历史卡池小插件
 License: MIT
 Author: forchannot
 Author-email: yy320206@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,20 +32,23 @@
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/forchannot/nonebot-plugin-gshisbanner.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-gshisbanner">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-gshisbanner.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
+<br />
+<a href="https://onebot.dev/">
+    <img src="https://img.shields.io/badge/OneBot-v11-black?style=social&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABABAMAAABYR2ztAAAAIVBMVEUAAAAAAAADAwMHBwceHh4UFBQNDQ0ZGRkoKCgvLy8iIiLWSdWYAAAAAXRSTlMAQObYZgAAAQVJREFUSMftlM0RgjAQhV+0ATYK6i1Xb+iMd0qgBEqgBEuwBOxU2QDKsjvojQPvkJ/ZL5sXkgWrFirK4MibYUdE3OR2nEpuKz1/q8CdNxNQgthZCXYVLjyoDQftaKuniHHWRnPh2GCUetR2/9HsMAXyUT4/3UHwtQT2AggSCGKeSAsFnxBIOuAggdh3AKTL7pDuCyABcMb0aQP7aM4AnAbc/wHwA5D2wDHTTe56gIIOUA/4YYV2e1sg713PXdZJAuncdZMAGkAukU9OAn40O849+0ornPwT93rphWF0mgAbauUrEOthlX8Zu7P5A6kZyKCJy75hhw1Mgr9RAUvX7A3csGqZegEdniCx30c3agAAAABJRU5ErkJggg==" alt="onebot">
+</a>
 </div>
 
 ## 📖 介绍
 
-本插件用于在机器人上查询原神历史卡池信息
+本插件用于在机器人上查询原神历史卡池信息（当前仅适用于qq）
 
 ## 💿 安装
 
 <details>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
@@ -82,19 +85,19 @@
      ##前面的"ghproxy.com/"可以不写(如果你是国外机),或者换成你自建的github加速服务均可(需要支持https)
 ·· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/gacha"
      ##jsdelivr代理的文件，大多数情况可用，推荐
 ```
 
 ## 🎉 使用
 ### 指令表
-|        指令         |    权限    | 需要@ | 范围 |                             说明                             |
-| :-----------------: | :--------: | :---: | :--: | :----------------------------------------------------------: |
-| [name]历史卡池(num) |    ALL     |  否   | ALL  | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
-| [version]卡池[num]  |    ALL     |  否   | ALL  | version为版本号，如1.3，2.6等，num为1-3，对应上半（中）下半，可不填，如不填则发送该版本全部卡池 |
-|  刷新历史卡池/别名  | 管理员以上 |  否   | ALL  |                      刷新历史卡池或别名                      |
+|        指令        |  权限   | 需要@ | 范围  |                                说明                                |
+|:----------------:|:-----:|:---:|:---:|:----------------------------------------------------------------:|
+| [name]历史卡池(num)  |  ALL  |  否  | ALL | name必填，为角色名字或别名；num选填，为单次合并转发次数，若无则为gshisbanner_forward_length的值 |
+| [version]卡池[num] |  ALL  |  否  | ALL |    version为版本号，如1.3，2.6等，num为1-3，对应上半（中）下半，可不填，如不填则发送该版本全部卡池     |
+|  刷新(更新)历史卡池/别名   | 管理员以上 |  否  | ALL |                            刷新历史卡池或别名                             |
 ### 效果图
 <details>
 <summary>历史卡池效果图</summary>
 <details>
 <summary>图1</summary>
 <img src="https://cdn.staticaly.com/gh/forchannot/mypicgo@main/20230324/image.4jlu5w0mhko0.jpg" alt="help">
 </details>
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gshisbanner Version: 0.5.1 Summary:
 Nonebot2æ¥è¯¢åç¥åå²å¡æ± å°æä»¶ License: MIT Author: forchannot
 Author-email: yy320206@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: httpx (>=0.20.0,<1.0.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.1,<3.0) Requires-Dist: nonebot2 (>=2.0.0-rc.2,<3.0.0) Description-Content-
 Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
                        # nonebot-plugin-gshisbanner _â¨
  æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ â¨_ [license]
-                                [pypi] [python]
-## ð ä»ç» æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ ##
-ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
+                               [pypi] [python]
+                                   [onebot]
+## ð ä»ç»
+æ¬æä»¶ç¨äºå¨æºå¨äººä¸æ¥è¯¢åç¥åå²å¡æ± ä¿¡æ¯ï¼å½åä»éç¨äºqqï¼
+## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot-plugin-gshisbanner   pip pip install nonebot-plugin-gshisbanner
 æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
 [tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_gshisbanner"]  ##
 âï¸ éç½® ``` gshisbanner_forward_length: int #
 åæ¬¡åå¹¶è½¬åæ¶æ¯é¿åº¦ï¼intï¼,é»è®¤ä¸º10 #
 è¶å¤§åæ¬¡è½¬ååå®¹æ´å¤ï¼åå¹¶è½¬åçæ¬¡æ°æ´å°ï¼è¶å°ååæ¬¡è½¬ååå®¹æ´å°ï¼ä½åå¹¶è½¬åçæ¬¡æ°æ´å¤
@@ -29,19 +31,19 @@
 3."genshin-gacha-banners.52v6.com/data" #cloudfareä»£çï¼å¯è½ä¼è¢«å¢ Â·Â·
 4."ghproxy.com/https://raw.githubusercontent.com/KeyPJ/FetchData/main/data/
 gacha" ##ghproxyä»£ççrawæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼ä¸è¿ä¸ç¨³å®
 ##åé¢ç"ghproxy.com/"å¯ä»¥ä¸å
 (å¦æä½ æ¯å½å¤æº),æèæ¢æä½ èªå»ºçgithubå éæå¡åå¯
 (éè¦æ¯æhttps) Â·Â· 5."fastly.jsdelivr.net/gh/KeyPJ/FetchData@main/data/
 gacha" ##jsdelivrä»£ççæä»¶ï¼å¤§å¤æ°æåµå¯ç¨ï¼æ¨è ``` ## ð
-ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :-------
-----------: | :--------: | :---: | :--: | :------------------------------------
-----------------------: | | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
+ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:--------
+--------:|:-----:|:---:|:---:|:------------------------------------------------
+----------------:| | [name]åå²å¡æ± (num) | ALL | å¦ | ALL |
 nameå¿å¡«ï¼ä¸ºè§è²åå­æå«åï¼numéå¡«ï¼ä¸ºåæ¬¡åå¹¶è½¬åæ¬¡æ°ï¼è¥æ åä¸ºgshisbanner_forward_lengthçå¼
 | | [version]å¡æ± [num] | ALL | å¦ | ALL |
 versionä¸ºçæ¬å·ï¼å¦1.3ï¼2.6ç­ï¼numä¸º1-
 3ï¼å¯¹åºä¸åï¼ä¸­ï¼ä¸åï¼å¯ä¸å¡«ï¼å¦ä¸å¡«ååéè¯¥çæ¬å¨é¨å¡æ± 
-| | å·æ°åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
+| | å·æ°(æ´æ°)åå²å¡æ± /å«å | ç®¡çåä»¥ä¸ | å¦ | ALL |
 å·æ°åå²å¡æ± æå«å | ### ææå¾  åå²å¡æ± ææå¾  å¾1 [help]
 å¾2 [help]   å¾3 [help]    çæ¬å¡æ± ææå¾  å¾1 [help]   å¾2 [help]
 å¾3 [help]    å·æ°å¡æ± /å«åææå¾ [help]  ### é¸£è°¢ [genshin-gacha-
 banners](https://github.com/KeyPJ/genshin-gacha-banners) #åå²upå¡æ± æ¥æº
```

