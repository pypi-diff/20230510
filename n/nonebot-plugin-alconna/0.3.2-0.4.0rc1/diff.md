# Comparing `tmp/nonebot-plugin-alconna-0.3.2.tar.gz` & `tmp/nonebot-plugin-alconna-0.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.3.2.tar", last modified: Sat Feb 25 12:55:46 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.4.0rc1.tar", last modified: Wed May 10 10:32:49 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.3.2.tar` & `nonebot-plugin-alconna-0.4.0rc1.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.3.2/LICENSE
--rw-r--r--   0        0        0      902 2023-02-25 12:25:06.738032 nonebot-plugin-alconna-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     7727 2023-02-22 17:35:07.483209 nonebot-plugin-alconna-0.3.2/README.md
--rw-r--r--   0        0        0      470 2023-02-20 09:54:27.190552 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0        0 2023-01-26 16:08:53.308451 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      195 2023-01-28 07:28:47.964612 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0      508 2023-02-15 14:24:34.489141 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0      762 2023-01-28 07:28:47.778569 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     1322 2023-01-28 07:28:47.806733 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      201 2023-01-28 07:28:47.915741 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0      577 2023-01-28 07:28:48.031029 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0     1972 2023-01-28 07:28:47.985553 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0      403 2023-01-28 06:54:29.300187 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     1973 2023-01-28 07:28:47.827494 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     1747 2023-01-28 07:28:48.007768 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     1775 2023-01-28 07:28:47.850432 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0      193 2023-01-28 07:28:47.941674 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/spigot.py
--rw-r--r--   0        0        0     1272 2023-01-28 07:28:47.871510 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0     1936 2023-02-20 09:29:57.582474 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/analyser.py
--rw-r--r--   0        0        0      315 2023-02-22 17:35:07.506211 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0       86 2023-01-26 15:45:50.153847 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0     3589 2023-02-25 12:34:42.833945 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1213 2023-02-25 12:48:57.742734 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     2036 2023-02-20 09:54:31.287130 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     4868 2023-02-25 12:48:57.768732 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0      628 2023-01-28 05:16:57.868797 nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.4.0rc1/LICENSE
+-rw-r--r--   0        0        0     1144 2023-05-10 08:21:46.157932 nonebot-plugin-alconna-0.4.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7529 2023-05-10 08:21:46.125592 nonebot-plugin-alconna-0.4.0rc1/README.md
+-rw-r--r--   0        0        0     1208 2023-05-10 08:50:46.247626 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-26 16:08:53.308451 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      115 2023-05-10 08:33:24.132983 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      190 2023-05-10 08:33:24.069340 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      170 2023-05-10 08:33:24.090951 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     3812 2023-05-10 09:00:57.030628 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1499 2023-05-10 08:54:25.558632 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1417 2023-05-10 08:27:49.596958 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     2187 2023-04-02 14:03:55.798752 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     9071 2023-05-10 10:32:39.813272 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     1591 2023-05-10 08:33:24.123949 nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     7641 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.4.0rc1/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.3.2/LICENSE` & `nonebot-plugin-alconna-0.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.3.2/README.md` & `nonebot-plugin-alconna-0.4.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -54,25 +54,24 @@
 assert not alc.parse(Message(["Hello!", img])).matched
 ```
 
 ### MessageSegment 标注
 
 ```python
 from nonebot_plugin_alconna.adapters.onebot12 import Mention
-from nonebot.adapters.onebot.v12 import Message, MessageSegment
+from nonebot.adapters.onebot.v12 import Message
 from arclet.alconna import Alconna, Args
-from arclet.alconna.tools import AlconnaString
 
-msg = Message(["Hello!", MessageSegment.mention("123")])
+msg = Message(["Hello!", Mention("123")])
 print(msg)  # Hello![mention:user_id=123]
 
-alc = AlconnaString("Hello! <target:Mention>")
+alc = Alconna("Hello!", Args["target", Mention])
 res = alc.parse(msg)
 assert res.matched
-assert res.target.data['user_id'] == '123'
+assert res.query("target").data['user_id'] == '123'
 ```
 
 ### Matcher 与 依赖注入
 ```python
 ...
 from nonebot import require
 require("nonebot_plugin_alconna")
@@ -81,36 +80,36 @@
 from nonebot_plugin_alconna import (
     on_alconna, 
     Match,
     Query,
     AlconnaMatch, 
     AlconnaQuery,
     AlconnaResult, 
-    AlconnaMatches,
-    CommandResult
+    AlcMatches,
+    AlcResult
 )
 from arclet.alconna import Alconna, Args, Arparma, Option
 
 test = on_alconna(
     Alconna(
         "test",
         Option("foo", Args["bar", int]),
         Option("baz", Args["qux", bool, False])
     ),
     auto_send_output=True
 )
 
 
 @test.handle()
-async def handle_test1(result: CommandResult = AlconnaResult()):
+async def handle_test1(result: AlcResult):
     await test.send(f"matched: {result.matched}")
     await test.send(f"maybe output: {result.output}")
 
 @test.handle()
-async def handle_test2(result: Arparma = AlconnaMatches()):
+async def handle_test2(result: AlcMatches):
     await test.send(f"head result: {result.header_result}")
     await test.send(f"args: {result.all_matched_args}")
 
 @test.handle()
 async def handle_test3(bar: Match[int] = AlconnaMatch("bar")):
     if bar.available:    
         await test.send(f"foo={bar.result}")
@@ -223,28 +222,28 @@
 - `checker`: 命令解析结果的检查器
 - `skip_for_unmatch`: 是否在命令不匹配时跳过该响应
 - `auto_send_output`: 是否自动发送输出信息并跳过响应
 - `output_converter`: 输出信息字符串转换为 Message 方法
 
 ## 提供了 MessageSegment标注 的协议:
 
-| 协议名称                                                                      | 路径                                   |
-|---------------------------------------------------------------------------|--------------------------------------|
-| [OneBot 协议](https://onebot.dev/)                                          | adapters.onebot11, adapters.onebot12 |
-| [Telegram](https://core.telegram.org/bots/api)                            | adapters.telegram                    |
-| [飞书](https://open.feishu.cn/document/home/index)                          | adapters.feishu                      |
-| [GitHub](https://docs.github.com/en/developers/apps)                      | adapters.github                      |
-| [QQ 频道](https://bot.q.qq.com/wiki/)                                       | adapters.qqguild                     |
-| [钉钉](https://open.dingtalk.com/document/)                                 | adapters.ding                        |
-| [Console](https://github.com/nonebot/adapter-console)                     | adapters.console                     |
-| [开黑啦](https://developer.kookapp.cn/)                                      | adapters.kook                        |
-| [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)                     | adapters.mirai                       |
-| [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)                | adapters.ntchat                      |
-| [MineCraft (Spigot)](https://github.com/17TheWord/nonebot-adapter-spigot) | adapters.spigot                      |
-| [BiliBili Live](https://github.com/wwweww/adapter-bilibili)               | adapters.bilibili                    |
+| 协议名称                                                                | 路径                                   |
+|---------------------------------------------------------------------|--------------------------------------|
+| [OneBot 协议](https://onebot.dev/)                                    | adapters.onebot11, adapters.onebot12 |
+| [Telegram](https://core.telegram.org/bots/api)                      | adapters.telegram                    |
+| [飞书](https://open.feishu.cn/document/home/index)                    | adapters.feishu                      |
+| [GitHub](https://docs.github.com/en/developers/apps)                | adapters.github                      |
+| [QQ 频道](https://bot.q.qq.com/wiki/)                                 | adapters.qqguild                     |
+| [钉钉](https://open.dingtalk.com/document/)                           | adapters.ding                        |
+| [Console](https://github.com/nonebot/adapter-console)               | adapters.console                     |
+| [开黑啦](https://developer.kookapp.cn/)                                | adapters.kook                        |
+| [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)               | adapters.mirai                       |
+| [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)          | adapters.ntchat                      |
+| [MineCraft](https://github.com/17TheWord/nonebot-adapter-minecraft) | adapters.minecraft                   |
+| [BiliBili Live](https://github.com/wwweww/adapter-bilibili)         | adapters.bilibili                    |
 
 
 
 
 ## 体验
 
 [demo bot](./src/test/plugins/demo.py)
```

### Comparing `nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/matcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from nonebot.matcher import Matcher
 from nonebot.adapters import Message
 from nonebot.plugin.on import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_RuleChecker
 
 from .rule import alconna
+from .model import CompConfig
+from .typings import OutputType
 
 
 def match_path(path: str):
     """
     当 Arpamar 解析成功后, 依据 path 是否存在以继续执行事件处理
 
     当 path 为 ‘$main’ 时表示认定当且仅当主命令匹配
@@ -55,33 +57,36 @@
     if or_not:
         return lambda x: match_path("$main") or match_path(path)  # type: ignore
     return match_path(path)
 
 
 def on_alconna(
     command: Alconna | str,
-    *checker: Callable[[Arparma], bool],
+    checker: list[Callable[[Arparma], bool]] | None = None,
     rule: Rule | T_RuleChecker | None = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
-    output_converter: Callable[[str], Message | Awaitable[Message]] | None = None,
+    output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
     aliases: set[str | tuple[str, ...]] | None = None,
+    comp_config: CompConfig | None = None,
+    *args,
     _depth: int = 0,
     **kwargs,
 ) -> type[Matcher]:
     """注册一个消息事件响应器，并且当消息由指定 Alconna 解析并传出有效结果时响应。
 
     参数:
         command: Alconna 命令
         checker: Arparma 检查器，会在解析后使用
         rule: 事件响应规则
         skip_for_unmatch: 是否在解析失败时跳过
         auto_send_output: 是否自动发送输出信息并跳过
         output_converter: 输出信息字符串转换为 Message 方法
         aliases: 命令别名
+        comp_config: 补全会话配置, 不传入则不启用补全会话
         permission: 事件响应权限
         handlers: 事件处理函数列表
         temp: 是否为临时事件响应器（仅执行一次）
         expire_time: 事件响应器最终有效时间点，过时即被删除
         priority: 事件响应器优先级
         block: 是否阻止事件向更低优先级传递
         state: 默认 state
@@ -93,15 +98,17 @@
         aliases.add(str(command.command))
         command.command = "(" + "|".join(aliases) + ")"
         command._hash = command._calc_hash()
         command_manager.register(command)
     return on_message(
         alconna(
             command,
-            *checker,
-            skip_for_unmatch=skip_for_unmatch,
-            auto_send_output=auto_send_output,
-            output_converter=output_converter
+            checker or [],
+            skip_for_unmatch,
+            auto_send_output,
+            output_converter,
+            comp_config
         ) & rule,
+        *args,
         **kwargs,
         _depth=_depth + 1  # type: ignore
     )
```

### Comparing `nonebot-plugin-alconna-0.3.2/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.4.0rc1/src/nonebot_plugin_alconna/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional, Type, TypeVar, overload
+from typing_extensions import Annotated
 
 from arclet.alconna import Arparma, Duplication, Empty
 from arclet.alconna.duplication import generate_duplication
 from nonebot.internal.params import Depends as Depends
 from nonebot.typing import T_State
 
 from .consts import ALCONNA_RESULT
@@ -64,7 +65,11 @@
 
 def AlconnaDuplication(__t: Optional[Type[T_Duplication]] = None) -> Duplication:
     def _alconna_match(state: T_State) -> Duplication:
         arp = _alconna_result(state).result
         return __t(arp) if __t else generate_duplication(arp)
 
     return Depends(_alconna_match, use_cache=False)
+
+
+AlcResult = Annotated[CommandResult, AlconnaResult()]
+AlcMatches = Annotated[Arparma, AlconnaMatches()]
```

### Comparing `nonebot-plugin-alconna-0.3.2/PKG-INFO` & `nonebot-plugin-alconna-0.4.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.3.2
+Version: 0.4.0rc1
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
@@ -65,25 +65,24 @@
 assert not alc.parse(Message(["Hello!", img])).matched
 ```
 
 ### MessageSegment 标注
 
 ```python
 from nonebot_plugin_alconna.adapters.onebot12 import Mention
-from nonebot.adapters.onebot.v12 import Message, MessageSegment
+from nonebot.adapters.onebot.v12 import Message
 from arclet.alconna import Alconna, Args
-from arclet.alconna.tools import AlconnaString
 
-msg = Message(["Hello!", MessageSegment.mention("123")])
+msg = Message(["Hello!", Mention("123")])
 print(msg)  # Hello![mention:user_id=123]
 
-alc = AlconnaString("Hello! <target:Mention>")
+alc = Alconna("Hello!", Args["target", Mention])
 res = alc.parse(msg)
 assert res.matched
-assert res.target.data['user_id'] == '123'
+assert res.query("target").data['user_id'] == '123'
 ```
 
 ### Matcher 与 依赖注入
 ```python
 ...
 from nonebot import require
 require("nonebot_plugin_alconna")
@@ -92,36 +91,36 @@
 from nonebot_plugin_alconna import (
     on_alconna, 
     Match,
     Query,
     AlconnaMatch, 
     AlconnaQuery,
     AlconnaResult, 
-    AlconnaMatches,
-    CommandResult
+    AlcMatches,
+    AlcResult
 )
 from arclet.alconna import Alconna, Args, Arparma, Option
 
 test = on_alconna(
     Alconna(
         "test",
         Option("foo", Args["bar", int]),
         Option("baz", Args["qux", bool, False])
     ),
     auto_send_output=True
 )
 
 
 @test.handle()
-async def handle_test1(result: CommandResult = AlconnaResult()):
+async def handle_test1(result: AlcResult):
     await test.send(f"matched: {result.matched}")
     await test.send(f"maybe output: {result.output}")
 
 @test.handle()
-async def handle_test2(result: Arparma = AlconnaMatches()):
+async def handle_test2(result: AlcMatches):
     await test.send(f"head result: {result.header_result}")
     await test.send(f"args: {result.all_matched_args}")
 
 @test.handle()
 async def handle_test3(bar: Match[int] = AlconnaMatch("bar")):
     if bar.available:    
         await test.send(f"foo={bar.result}")
@@ -234,28 +233,28 @@
 - `checker`: 命令解析结果的检查器
 - `skip_for_unmatch`: 是否在命令不匹配时跳过该响应
 - `auto_send_output`: 是否自动发送输出信息并跳过响应
 - `output_converter`: 输出信息字符串转换为 Message 方法
 
 ## 提供了 MessageSegment标注 的协议:
 
-| 协议名称                                                                      | 路径                                   |
-|---------------------------------------------------------------------------|--------------------------------------|
-| [OneBot 协议](https://onebot.dev/)                                          | adapters.onebot11, adapters.onebot12 |
-| [Telegram](https://core.telegram.org/bots/api)                            | adapters.telegram                    |
-| [飞书](https://open.feishu.cn/document/home/index)                          | adapters.feishu                      |
-| [GitHub](https://docs.github.com/en/developers/apps)                      | adapters.github                      |
-| [QQ 频道](https://bot.q.qq.com/wiki/)                                       | adapters.qqguild                     |
-| [钉钉](https://open.dingtalk.com/document/)                                 | adapters.ding                        |
-| [Console](https://github.com/nonebot/adapter-console)                     | adapters.console                     |
-| [开黑啦](https://developer.kookapp.cn/)                                      | adapters.kook                        |
-| [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)                     | adapters.mirai                       |
-| [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)                | adapters.ntchat                      |
-| [MineCraft (Spigot)](https://github.com/17TheWord/nonebot-adapter-spigot) | adapters.spigot                      |
-| [BiliBili Live](https://github.com/wwweww/adapter-bilibili)               | adapters.bilibili                    |
+| 协议名称                                                                | 路径                                   |
+|---------------------------------------------------------------------|--------------------------------------|
+| [OneBot 协议](https://onebot.dev/)                                    | adapters.onebot11, adapters.onebot12 |
+| [Telegram](https://core.telegram.org/bots/api)                      | adapters.telegram                    |
+| [飞书](https://open.feishu.cn/document/home/index)                    | adapters.feishu                      |
+| [GitHub](https://docs.github.com/en/developers/apps)                | adapters.github                      |
+| [QQ 频道](https://bot.q.qq.com/wiki/)                                 | adapters.qqguild                     |
+| [钉钉](https://open.dingtalk.com/document/)                           | adapters.ding                        |
+| [Console](https://github.com/nonebot/adapter-console)               | adapters.console                     |
+| [开黑啦](https://developer.kookapp.cn/)                                | adapters.kook                        |
+| [Mirai](https://docs.mirai.mamoe.net/mirai-api-http/)               | adapters.mirai                       |
+| [Ntchat](https://github.com/JustUndertaker/adapter-ntchat)          | adapters.ntchat                      |
+| [MineCraft](https://github.com/17TheWord/nonebot-adapter-minecraft) | adapters.minecraft                   |
+| [BiliBili Live](https://github.com/wwweww/adapter-bilibili)         | adapters.bilibili                    |
 
 
 
 
 ## 体验
 
 [demo bot](./src/test/plugins/demo.py)
```

