# Comparing `tmp/mys_goods_tool-2.0.0b1.tar.gz` & `tmp/mys_goods_tool-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mys_goods_tool-2.0.0b1.tar", max compression
+gzip compressed data, was "mys_goods_tool-2.0.1.tar", max compression
```

## Comparing `mys_goods_tool-2.0.0b1.tar` & `mys_goods_tool-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0     1065 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     5604 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/README.md
--rw-r--r--   0        0        0        0 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/__main__.py
--rw-r--r--   0        0        0    54998 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/api.py
--rw-r--r--   0        0        0     4689 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/custom_css.py
--rw-r--r--   0        0        0     7617 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/custom_widget.py
--rw-r--r--   0        0        0     7910 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/data_model.py
--rw-r--r--   0        0        0    13639 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/exchange_mode.py
--rw-r--r--   0        0        0    43297 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/exchange_plan_view.py
--rw-r--r--   0        0        0     6710 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/geetest-webui/index.html
--rw-r--r--   0        0        0    10861 2023-05-02 22:59:21.795677 mys_goods_tool-2.0.0b1/mys_goods_tool/geetest-webui/libs/gt.js
--rw-r--r--   0        0        0   366500 2023-05-02 22:59:21.799677 mys_goods_tool-2.0.0b1/mys_goods_tool/geetest-webui/libs/jquery.js
--rw-r--r--   0        0        0     6663 2023-05-02 22:59:21.799677 mys_goods_tool-2.0.0b1/mys_goods_tool/geetest-webui/localized.html
--rw-r--r--   0        0        0     9157 2023-05-02 22:59:21.799677 mys_goods_tool-2.0.0b1/mys_goods_tool/geetest.py
--rw-r--r--   0        0        0    22632 2023-05-02 22:59:21.799677 mys_goods_tool-2.0.0b1/mys_goods_tool/login_view.py
--rw-r--r--   0        0        0    12501 2023-05-02 22:59:21.799677 mys_goods_tool-2.0.0b1/mys_goods_tool/tui.py
--rw-r--r--   0        0        0    16996 2023-05-02 22:59:21.799677 mys_goods_tool-2.0.0b1/mys_goods_tool/user_data.py
--rw-r--r--   0        0        0    11252 2023-05-02 22:59:21.799677 mys_goods_tool-2.0.0b1/mys_goods_tool/utils.py
--rw-r--r--   0        0        0     1563 2023-05-02 22:59:21.799677 mys_goods_tool-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 mys_goods_tool-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4107 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/__main__.py
+-rw-r--r--   0        0        0    56543 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/api.py
+-rw-r--r--   0        0        0     5536 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/custom_css.py
+-rw-r--r--   0        0        0     7599 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/custom_widget.py
+-rw-r--r--   0        0        0     7910 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/data_model.py
+-rw-r--r--   0        0        0    13698 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/exchange_mode.py
+-rw-r--r--   0        0        0    43420 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/exchange_plan_view.py
+-rw-r--r--   0        0        0     6442 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/gt4-localized.html
+-rw-r--r--   0        0        0     6501 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/gt4.html
+-rw-r--r--   0        0        0     6840 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/index.html
+-rw-r--r--   0        0        0    10861 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/libs/gt.js
+-rw-r--r--   0        0        0    14792 2023-05-10 15:32:32.305375 mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/libs/gt4.js
+-rw-r--r--   0        0        0   366500 2023-05-10 15:32:32.309375 mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/libs/jquery.js
+-rw-r--r--   0        0        0     6910 2023-05-10 15:32:32.309375 mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/localized.html
+-rw-r--r--   0        0        0     9157 2023-05-10 15:32:32.309375 mys_goods_tool-2.0.1/mys_goods_tool/geetest.py
+-rw-r--r--   0        0        0    21679 2023-05-10 15:32:32.309375 mys_goods_tool-2.0.1/mys_goods_tool/login_view.py
+-rw-r--r--   0        0        0    12665 2023-05-10 15:32:32.309375 mys_goods_tool-2.0.1/mys_goods_tool/tui.py
+-rw-r--r--   0        0        0    17211 2023-05-10 15:32:32.309375 mys_goods_tool-2.0.1/mys_goods_tool/user_data.py
+-rw-r--r--   0        0        0    11252 2023-05-10 15:32:32.309375 mys_goods_tool-2.0.1/mys_goods_tool/utils.py
+-rw-r--r--   0        0        0     1535 2023-05-10 15:32:32.309375 mys_goods_tool-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 mys_goods_tool-2.0.1/PKG-INFO
```

### Comparing `mys_goods_tool-2.0.0b1/LICENSE` & `mys_goods_tool-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/__main__.py` & `mys_goods_tool-2.0.1/mys_goods_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/api.py` & `mys_goods_tool-2.0.1/mys_goods_tool/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -529,20 +529,48 @@
             logger.debug(f"网络请求返回: {res.text}")
             GetGoodDetailStatus(incorrect_return=True), None
         else:
             logger.exception(f"米游币商品兑换 - 获取商品详细信息: 网络请求失败")
             GetGoodDetailStatus(network_error=True), None
 
 
-async def get_good_list(game: str, retry: bool = True) -> Tuple[
+async def get_good_games(retry: bool = True) -> Tuple[BaseApiStatus, Optional[List[Tuple[str, str]]]]:
+    """
+    获取商品分区列表
+
+    :param retry: 是否允许重试
+    :return: (商品分区全名, 字母简称) 的列表
+    """
+    try:
+        async for attempt in tenacity.AsyncRetrying(stop=custom_attempt_times(retry), reraise=True,
+                                                    wait=tenacity.wait_fixed(conf.preference.retry_interval)):
+            with attempt:
+                async with httpx.AsyncClient() as client:
+                    res = await client.get(URL_GOOD_LIST.format(page=1,
+                                                                game=""),
+                                           headers=HEADERS_GOOD_LIST,
+                                           timeout=conf.preference.timeout)
+                api_result = ApiResultHandler(res.json())
+                return BaseApiStatus(success=True), list(map(lambda x: (x["name"], x["key"]), api_result.data["games"]))
+    except tenacity.RetryError as e:
+        if is_incorrect_return(e):
+            logger.exception(f"米游币商品兑换 - 获取商品列表: 服务器没有正确返回")
+            logger.debug(f"网络请求返回: {res.text}")
+            return BaseApiStatus(incorrect_return=True), None
+        else:
+            logger.exception(f"米游币商品兑换 - 获取商品列表: 网络请求失败")
+            return BaseApiStatus(network_error=True), None
+
+
+async def get_good_list(game: str = "", retry: bool = True) -> Tuple[
     BaseApiStatus, Optional[List[Good]]]:
     """
     获取商品信息列表
 
-    :param game: 游戏简称
+    :param game: 游戏简称（默认为空，即获取所有游戏的商品）
     :param retry: 是否允许重试
     :return: 商品信息列表
     """
     good_list = []
     page = 1
 
     try:
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/custom_css.py` & `mys_goods_tool-2.0.1/mys_goods_tool/custom_css.py`

 * *Files 11% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     """
 
 
 class AboveFold(Container):
     DEFAULT_CSS = """
     AboveFold {
         width: 100%;
-        height: 100%;
+        height: auto;
         align: center middle;
     }
     """
 
 
 class Section(Container):
     DEFAULT_CSS = """
@@ -261,7 +261,56 @@
     
     ExchangePlanContent Horizontal LoadingIndicator {
         width: auto;
         min-width: 16;
         height: 3;
     }
     """
+
+
+class CaptchaTips(Container):
+    """
+    登陆信息面板文本视图
+    """
+    DEFAULT_CSS = """
+    CaptchaTips {
+        height: 100%;
+        width: 1fr;
+        align: right middle;
+        padding: 1;
+        overflow: auto;
+        border: round #666;
+    }
+
+    App.-light-mode Tips {
+        border: round #CCC;
+    }
+
+    CaptchaTips StaticStatus {
+        width: 100%;
+        align: center top;
+        text-align: center;
+    }
+    """
+
+
+class CaptchaStepSet(Container):
+    """
+    登陆进度节点集合视图
+    """
+    DEFAULT_CSS = """
+    CaptchaStepSet {
+        height: auto;
+        width: 1fr;
+        align: left middle;
+        overflow: auto;
+        border: round #666;
+    }
+
+    App.-light-mode StepSet {
+        border: round #CCC;
+    }
+
+    CaptchaStepSet RadioStatus {
+        margin: 1 1;
+    }
+    """
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/custom_widget.py` & `mys_goods_tool-2.0.1/mys_goods_tool/custom_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 from itertools import zip_longest
-from typing import Optional
+from typing import Optional, Tuple
 
 from rich.console import RenderableType
 from rich.text import TextType
 from textual import events
 from textual.app import ComposeResult
 from textual.events import Event
 from textual.widgets import (
     Button,
     LoadingIndicator, RadioButton, TabbedContent, TabPane, ContentSwitcher, Tabs, ListItem
 )
 from textual.widgets._button import ButtonVariant
 from textual.widgets._tabbed_content import ContentTab
 
 from mys_goods_tool.custom_css import *
-from mys_goods_tool.data_model import GameInfo
 from mys_goods_tool.user_data import ExchangePlan
 
 
 class RadioStatus(RadioButton, can_focus=False):
     """
     完成的进度节点，不允许点击交互
     可通过触发事件以即时修改value属性
@@ -213,18 +212,18 @@
             label: TextType | None = None,
             variant: ButtonVariant = "default",
             *,
             name: str | None = None,
             id: str | None = None,
             classes: str | None = None,
             disabled: bool = False,
-            game: GameInfo
+            partition: Tuple[str, str]
     ):
         super().__init__(label, variant, name=name, id=id, classes=classes, disabled=disabled)
-        self.game = game
+        self.partition = partition
 
     class Pressed(Button.Pressed):
         def __init__(self, button: GameButton):
             super().__init__(button)
             self.button = button
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/data_model.py` & `mys_goods_tool-2.0.1/mys_goods_tool/data_model.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/exchange_mode.py` & `mys_goods_tool-2.0.1/mys_goods_tool/exchange_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import sys
 from datetime import datetime
 from typing import Optional, Union, Tuple, Set
 from urllib.parse import urlparse
 
 import ping3
 from apscheduler.events import JobExecutionEvent, EVENT_JOB_EXECUTED
-from apscheduler.schedulers.asyncio import AsyncIOScheduler
-from apscheduler.schedulers.base import STATE_STOPPED
+from apscheduler.schedulers.background import BackgroundScheduler
+from apscheduler.schedulers.base import STATE_STOPPED, BaseScheduler
+from apscheduler.schedulers.blocking import BlockingScheduler
 from rich.console import RenderableType
 from textual import events
 from textual.app import ComposeResult
 from textual.containers import Container, Horizontal
 from textual.events import Event
 from textual.reactive import reactive
 from textual.widgets import Static, ListView, ListItem
@@ -47,19 +48,18 @@
     if result is None:
         logger.info(f"Ping 商品兑换API服务器 {hostname} 超时")
     elif result is False:
         logger.info(f"Ping 商品兑换API服务器 {hostname} 失败")
     return result
 
 
-def get_scheduler():
+def set_scheduler(scheduler: BaseScheduler):
     """
-    获取兑换计划调度器
+    向兑换计划调度器添加兑换任务以及ping循环
     """
-    scheduler = AsyncIOScheduler()
     scheduler.configure(timezone=conf.preference.timezone or Preference.timezone)
 
     if conf.preference.enable_connection_test:
         interval = conf.preference.connection_test_interval or Preference.connection_test_interval
         scheduler.add_job(_connection_test, "interval", seconds=interval, id=f"exchange-connection_test")
 
     for plan in conf.exchange_plans:
@@ -95,15 +95,15 @@
     普通文本模式（无Textual）
     """
     logger.add(sys.stdout, diagnose=True, format=LOG_FORMAT, level="DEBUG")
     if not conf.exchange_plans:
         logger.info("无兑换计划需要执行")
         return
 
-    scheduler = get_scheduler()
+    scheduler = set_scheduler(BlockingScheduler())
     finished_plans = set()
 
     @lambda func: scheduler.add_listener(func, EVENT_JOB_EXECUTED)
     def on_executed(event: JobExecutionEvent):
         """
         接收兑换结果
         """
@@ -134,20 +134,20 @@
         elif event.job_id == "exchange-connection_test":
             result: Union[float, bool, None] = event.retval
             if result:
                 print(
                     f"Ping 商品兑换API服务器 {_get_api_host() or 'N/A'} - 延迟 {round(result, 2) if result else 'N/A'} ms")
 
     try:
+        logger.info("启动兑换计划定时器")
         scheduler.start()
-        logger.info("兑换计划定时器已启动")
-        asyncio.get_event_loop().run_forever()
+
     except KeyboardInterrupt:
+        logger.info("停止兑换计划定时器")
         scheduler.shutdown()
-        logger.info("兑换计划定时器已停止")
 
 
 class EnterExchangeMode(Event):
     """
     进入兑换模式的事件
     """
     pass
@@ -208,15 +208,15 @@
 
     button_enter = ControllableButton("确定", variant="warning", id="button-exchange_mode-enter")
     button_exit = ControllableButton("退出", variant="error", id="button-exchange_mode-exit")
     button_refresh = ControllableButton("刷新", id="button-exchange_mode-refresh")
     button_exit.hide()
     warning_text = ExchangeModeWarning()
     """进入/退出 兑换模式的提示文本"""
-    scheduler = get_scheduler()
+    scheduler = set_scheduler(BackgroundScheduler())
     """兑换计划调度器"""
     empty_data_item = ListItem(Static("暂无兑换计划，你可以尝试刷新"))
     list_view = ListView(empty_data_item)
     """兑换计划列表"""
 
     def compose(self) -> ComposeResult:
         with Horizontal():
@@ -368,15 +368,14 @@
     DEFAULT_CSS = """
     ExchangeModePing {
         margin: 1 0;
     }
     """
     DEFAULT_VALUE = False
     ping_value: reactive[Union[float, bool, None]] = reactive(DEFAULT_VALUE)
-    scheduler = get_scheduler()
 
     def render(self) -> RenderableType:
         return f"⚡ Ping | 商品兑换API服务器 [yellow]{_get_api_host() or 'N/A'}[/]" \
                f" - 延迟 [bold green]{round(self.ping_value, 2) or 'N/A'}[/] ms"
 
     def update_ping(self, event: JobExecutionEvent):
         """
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/exchange_plan_view.py` & `mys_goods_tool-2.0.1/mys_goods_tool/exchange_plan_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from textual.reactive import reactive
 from textual.widget import Widget
 from textual.widgets import (
     TabbedContent, TabPane, OptionList, ListView
 )
 from textual.widgets._option_list import Option, Separator
 
-from mys_goods_tool.api import get_good_list, get_game_list, get_address, get_game_record, good_exchange, \
-    get_good_detail
+from mys_goods_tool.api import get_good_list, get_address, get_game_record, good_exchange, \
+    get_good_detail, get_good_games
 from mys_goods_tool.custom_css import *
 from mys_goods_tool.custom_widget import StaticStatus, ControllableButton, LoadingDisplay, \
     DynamicTabbedContent, GameButton, PlanButton, UnClickableItem
-from mys_goods_tool.data_model import Good, GameInfo, Address, GameRecord
+from mys_goods_tool.data_model import Good, Address, GameRecord
 from mys_goods_tool.user_data import config as conf, UserAccount, ExchangePlan
 
 _T = TypeVar("_T")
 
 
 class BaseExchangePlan(ExchangePlanContent):
     DEFAULT_TEXT: RenderableType
@@ -238,51 +238,52 @@
 
     button_refresh = ControllableButton("🔄 刷新", variant="primary", id="button-goods-refresh")
     button_reset = ControllableButton("↩ 重置", variant="warning", id="button-goods-reset", disabled=True)
 
     loading = LoadingDisplay()
     loading.hide()
 
-    good_dict: Dict[int, GoodsDictValue] = {}
-    """获取到的商品数据以及相关的控件"""
-    selected_tuple: Optional[Tuple[GameInfo, int]] = None
-    """已选择的商品位置"""
+    good_dict: Dict[str, GoodsDictValue] = {}
+    """获取到的商品数据以及相关的控件 商品分区简称 -> 商品数据"""
+    selected_tuple: Optional[Tuple[Tuple[str, str], int]] = None
+    """已选择的商品位置 ((商品分区, 分区简称), 商品在OptionList中的位置)"""
 
     empty_data_option = Option("暂无商品数据，可能是目前没有限时兑换的商品，可尝试刷新", disabled=True)
     """空的商品选项列表"""
     tabbed_content = DynamicTabbedContent()
 
     class GoodsDictValue:
         """
         游戏频道对应的商品数据相关
         """
 
         def __init__(self,
-                     game_info: GameInfo,
+                     partition: Tuple[str, str],
                      button_select: Optional[GameButton] = None,
                      tap_pane: Optional[TabPane] = None,
                      good_list: List[Good] = None,
                      ):
             """
-            :param game_info: 商品频道数据
+            :param partition: (商品分区, 字母简称) 数据
             :param tap_pane: 频道对应的 `TabPane` 标签页
             :param good_list: 商品数据
             :param button_select: 选择商品的按钮
             """
-            self.game_info = game_info
+            name, abbr = partition
+            self.partition = partition
             """商品频道数据"""
             self.button_select = button_select or GameButton(
                 "💾 确定",
-                id=f"button-goods-select-{game_info.id}",
+                id=f"button-goods-select-{abbr}",
                 disabled=True,
-                game=game_info)
+                partition=partition)
             """选择商品的按钮"""
             self.option_list = OptionList(GoodsContent.empty_data_option, disabled=True)
             """商品的选项列表"""
-            self.tap_pane = tap_pane or TabPane(game_info.name, Horizontal(self.button_select, self.option_list))
+            self.tap_pane = tap_pane or TabPane(name, Horizontal(self.button_select, self.option_list))
             """频道对应的 `TabPane` 标签页"""
             self.good_list = good_list
             """商品数据"""
 
     def compose(self) -> ComposeResult:
         yield self.text_view
         with Horizontal():
@@ -296,21 +297,22 @@
         刷新商品信息
         """
         # 进度条、刷新按钮
         self.loading.show()
         self.button_refresh.disable()
 
         for goods_data in self.good_dict.values():
-            good_list_status, good_list = await get_good_list(goods_data.game_info.op_name)
+            name, abbr = goods_data.partition
+            good_list_status, good_list = await get_good_list(abbr)
             good_list = list(filter(lambda x: x.is_time_limited() and not x.is_time_end(), good_list))
 
             # 一种情况是获取成功但返回的商品数据为空，一种是API请求失败
             goods_data.option_list.clear_options()
             if not good_list_status:
-                self.app.notice(f"[bold red]获取频道 [bold red]{goods_data.game_info.name}[/] 的商品数据失败！[/]")
+                self.app.notice(f"[bold red]获取频道 [bold red]{name}[/] 的商品数据失败！[/]")
                 # TODO 待补充各种错误情况
             if good_list:
                 goods_data.good_list = good_list
                 good_names = map(lambda x: x.general_name, good_list)
                 for name in good_names:
                     goods_data.option_list.add_option(name)
                 goods_data.button_select.enable()
@@ -327,21 +329,23 @@
 
     async def _on_mount(self, _: events.Mount):
         # 进度条、刷新按钮
         self.button_refresh.disable()
         self.loading.show()
 
         # 更新商品频道列表
-        game_list_status, game_list = await get_game_list()
-        if game_list_status:
-            for game in game_list:
-                if game.id not in self.good_dict:
+        partition_status, partition_all = await get_good_games()
+        # 过滤掉 "全部" 分区
+        partitions = filter(lambda x: x[1] != "all", partition_all)
+        if partition_status:
+            for name, abbr in partitions:
+                if abbr not in self.good_dict:
                     # 如果没有商品频道对应值，则进行创建
-                    goods_data = self.GoodsDictValue(game)
-                    self.good_dict.setdefault(game.id, goods_data)
+                    goods_data = self.GoodsDictValue((name, abbr))
+                    self.good_dict.setdefault(abbr, goods_data)
                     await self.tabbed_content.append(goods_data.tap_pane)
 
             # 更新每个频道的商品数据
             await self.update_data()
         else:
             self.text_view.update("[bold red]⚠ 获取商品频道列表失败，可尝试刷新[/]")
             self.app.notice("[bold red]获取商品频道列表失败！[/]")
@@ -373,30 +377,27 @@
         ExchangePlanView.game_record_content.reset_selected()
         GameRecordContent.check_good_type()
 
     async def _on_button_pressed(self, event: GameButton.Pressed) -> None:
         if event.button.id.startswith("button-goods-select"):
             # 按下“保存”按钮时触发的事件
 
-            game = event.button.game
-            if not game:
-                self.app.notice("[bold red]未找到对应的频道数据或频道不可用[/]")
-                return
-            option_list = self.good_dict[game.id].option_list
+            name, abbr = event.button.partition
+            option_list = self.good_dict[abbr].option_list
             selected_index = option_list.highlighted
             if selected_index is None:
                 self.app.notice("[bold red]请先从列表中选择商品！[/]")
                 return
-            good_dict_value = self.good_dict.get(game.id)
+            good_dict_value = self.good_dict.get(abbr)
             if not good_dict_value:
                 self.app.notice("[bold red]未找到对应的频道[/]")
                 return
 
             good = good_dict_value.good_list[selected_index]
-            GoodsContent.selected_tuple = game, selected_index
+            GoodsContent.selected_tuple = name, abbr, selected_index
 
             # 获取商品详情
             self.loading.show()
             good_detail_status, good_detail = await get_good_detail(good.goods_id)
             self.loading.hide()
             if not good_detail_status:
                 # TODO 待补充各种错误情况
@@ -417,15 +418,15 @@
             # 如果是虚拟/实物商品，则地址、游戏账号视图需要更新
             AddressContent.check_good_type()
             if AccountContent._selected is not None:
                 GameRecordContent.check_good_type()
 
             self.text_view.update(f"已选择商品："
                                   f"\n[list]"
-                                  f"\n🗂️ 商品频道：[bold green]{game.name}[/]"
+                                  f"\n🗂️ 商品频道：[bold green]{name}[/]"
                                   f"\n📌 名称：[bold green]{good.general_name}[/]"
                                   f"\n💰 价格：[bold green]{good.price}[/] 米游币"
                                   f"\n📦 库存：[bold green]{good.stoke_text}[/] 件"
                                   f"\n📅 兑换时间：[bold green]{good.time_text}[/]"
                                   f"\n📌 商品ID：[bold green]{good.goods_id}[/]"
                                   f"\n[/list]")
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/geetest-webui/index.html` & `mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/localized.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!DOCTYPE html>
-<!-- v0.1.1-dev -->
+<!-- v0.1.1-dev localized -->
 <html lang="zh-CN">
 <head>
     <link rel="shortcut icon" href="//www.geetest.com/static/imgs/favicon.ico"/>
     <meta charset="UTF-8">
     <meta content="width=device-width, initial-scale=1" name="viewport">
     <title>GEETEST 行为验证</title>
     <style>
@@ -79,33 +79,38 @@
                 <p id="errorDescription"></p>
             </div>
         </div>
     </div>
 </form>
 
 <!-- 注意，验证码本身是不需要 jquery 库，此处使用 jquery 仅为了在 demo 中使用，减少代码量 -->
-<script src="//apps.bdimg.com/libs/jquery/1.9.1/jquery.js"></script>
+<script src="/libs/jquery.js"></script>
 <!-- 引入 gt.js，既可以使用其中提供的 initGeetest 初始化函数 -->
-<script src="//static.geetest.com/static/tools/gt.js"></script>
+<script src="/libs/gt.js"></script>
 <script>
     let success = false;
 
     /**
      * 显示错误信息
      * @param {string} text 提示文本
-     * @param {Error} error GeetestError 错误对象
+     * @param {Error} error 错误对象
+     * @param isGeetestError 是否为 GeetestError
      */
-    function displayError(text, error = null) {
+    function displayError(text, error = null, isGeetestError = true) {
         $("#wait").hide();
         const errorText = $("#errorText");
         errorText.text(text);
-        if (error) {
+        if (error && isGeetestError) {
             $("#errorCode").text(error.code);
             $("#errorMessage").text(error.msg);
-            $("#errorDescription").text(error.user_error);
+            $("#errorDescription").text(error.desc);
+            $("#errorDiv").show();
+        } else if (error) {
+            $("#errorCode").text(error.status);
+            $("#errorMessage").text(error.statusText);
             $("#errorDiv").show();
         }
         errorText.show();
     }
 
     /**
      * 显示成功信息
@@ -154,15 +159,15 @@
                 success = true;
                 displayGeetestResult("已成功获取验证结果", result.geetest_validate, result.geetest_seccode);
                 $.get("/result", {validate: result.geetest_validate, seccode: result.geetest_seccode})
                     .done(function (_) {
                         displaySuccess("已成功将验证结果发送至服务器");
                     })
                     .fail(function (error) {
-                        displayError("发送验证结果至服务器失败", error);
+                        displayError("发送验证结果至服务器失败", error, false);
                     });
             }
         }, 1000);
     };
 
     function start() {
         const queryString = window.location.search;
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/geetest-webui/libs/gt.js` & `mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/libs/gt.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/geetest-webui/libs/jquery.js` & `mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/libs/jquery.js`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/geetest-webui/localized.html` & `mys_goods_tool-2.0.1/mys_goods_tool/geetest-webui/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!DOCTYPE html>
-<!-- v0.1.1-dev localized -->
+<!-- v0.1.2 -->
 <html lang="zh-CN">
 <head>
     <link rel="shortcut icon" href="//www.geetest.com/static/imgs/favicon.ico"/>
     <meta charset="UTF-8">
     <meta content="width=device-width, initial-scale=1" name="viewport">
     <title>GEETEST 行为验证</title>
     <style>
@@ -78,34 +78,38 @@
                 <h3>description: </h3>
                 <p id="errorDescription"></p>
             </div>
         </div>
     </div>
 </form>
 
-<!-- 注意，验证码本身是不需要 jquery 库，此处使用 jquery 仅为了在 demo 中使用，减少代码量 -->
-<script src="/libs/jquery.js"></script>
+<script src="https://apps.bdimg.com/libs/jquery/1.9.1/jquery.js"></script>
 <!-- 引入 gt.js，既可以使用其中提供的 initGeetest 初始化函数 -->
-<script src="/libs/gt.js"></script>
+<script src="https://static.geetest.com/static/tools/gt.js"></script>
 <script>
     let success = false;
 
     /**
      * 显示错误信息
      * @param {string} text 提示文本
-     * @param {Error} error GeetestError 错误对象
+     * @param {Error} error 错误对象
+     * @param isGeetestError 是否为 GeetestError
      */
-    function displayError(text, error = null) {
+    function displayError(text, error = null, isGeetestError = true) {
         $("#wait").hide();
         const errorText = $("#errorText");
         errorText.text(text);
-        if (error) {
+        if (error && isGeetestError) {
             $("#errorCode").text(error.code);
             $("#errorMessage").text(error.msg);
-            $("#errorDescription").text(error.user_error);
+            $("#errorDescription").text(error.desc);
+            $("#errorDiv").show();
+        } else if (error) {
+            $("#errorCode").text(error.status);
+            $("#errorMessage").text(error.statusText);
             $("#errorDiv").show();
         }
         errorText.show();
     }
 
     /**
      * 显示成功信息
@@ -154,15 +158,15 @@
                 success = true;
                 displayGeetestResult("已成功获取验证结果", result.geetest_validate, result.geetest_seccode);
                 $.get("/result", {validate: result.geetest_validate, seccode: result.geetest_seccode})
                     .done(function (_) {
                         displaySuccess("已成功将验证结果发送至服务器");
                     })
                     .fail(function (error) {
-                        displayError("发送验证结果至服务器失败", error);
+                        displayError("发送验证结果至服务器失败", error, false);
                     });
             }
         }, 1000);
     };
 
     function start() {
         const queryString = window.location.search;
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/geetest.py` & `mys_goods_tool-2.0.1/mys_goods_tool/geetest.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/login_view.py` & `mys_goods_tool-2.0.1/mys_goods_tool/login_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,61 +50,14 @@
     }
 
     CaptchaLoginInformation Horizontal {
         align: center middle;
     }
     """
 
-    class Tips(Container):
-        """
-        登陆信息面板文本视图
-        """
-        DEFAULT_CSS = """
-        Tips {
-            height: 100%;
-            width: 1fr;
-            align: right middle;
-            padding: 1;
-            overflow: auto;
-            border: round #666;
-        }
-
-        App.-light-mode Tips {
-            border: round #CCC;
-        }
-
-        Tips StaticStatus {
-            width: 100%;
-            align: center top;
-            text-align: center;
-        }
-        """
-
-    class StepSet(Container):
-        """
-        登陆进度节点集合视图
-        """
-        DEFAULT_CSS = """
-        StepSet {
-            height: auto;
-            width: 1fr;
-            align: left middle;
-            overflow: auto;
-            border: round #666;
-        }
-
-        App.-light-mode StepSet {
-            border: round #CCC;
-        }
-
-        StepSet RadioStatus {
-            margin: 1 1;
-        }
-        """
-
     RadioTuple = NamedTuple("RadioTuple",
                             create_geetest=RadioStatus,
                             http_server=RadioStatus,
                             geetest_finished=RadioStatus,
                             create_captcha=RadioStatus,
                             login_ticket_by_captcha=RadioStatus,
                             multi_token_by_login_ticket=RadioStatus,
@@ -136,16 +89,16 @@
     GEETEST_TEXT = "- 暂无需要完成的人机验证任务 -"
 
     static_tuple = StaticTuple(
         geetest_title=Static(Markdown("## GEETEST人机验证链接")),
         geetest_text=StaticStatus(GEETEST_TEXT)
     )
 
-    radio_set = StepSet(*radio_tuple)
-    static_set = Tips(*static_tuple)
+    radio_set = CaptchaStepSet(*radio_tuple)
+    static_set = CaptchaTips(*static_tuple)
 
     def compose(self) -> ComposeResult:
         yield Horizontal(self.radio_set, self.static_set)
 
 
 class PhoneForm(LoginForm):
     """
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/tui.py` & `mys_goods_tool-2.0.1/mys_goods_tool/tui.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,40 +23,46 @@
 from mys_goods_tool.exchange_mode import ExchangeModeView, EnterExchangeMode, ExitExchangeMode
 from mys_goods_tool.exchange_plan_view import ExchangePlanView
 from mys_goods_tool.login_view import LoginView
 from mys_goods_tool.user_data import ROOT_PATH, VERSION
 from mys_goods_tool.utils import LOG_FORMAT, logger
 
 WELCOME_MD = """
+# Mys_Goods_Tool - 米游社商品兑换工具
+
+## 更新说明
+- 修复米游社（大别野）等商品分区无商品的问题
+- 修复图形界面兑换模式下不会执行兑换的问题
+
 ## 功能和特性
-- 使用 Textual 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
+
+- 使用 [Textual](https://github.com/Textualize/textual) 终端图形界面库，支持 Windows / Linux / macOS 甚至可能是移动端SSH客户端
 - 短信验证码登录（只需接收一次验证码）
 - 内置人机验证页面，无需前往官网验证
 - 多账号支持
 - 支持米游社所有分区的商品兑换
 
 ### TODO
 - 支持在图形界面中编辑偏好设置
 - 密码登录
-
-## 偏好设置
-默认配置下基本上可以正常使用，如果需要修改配置，可以参考 [`mys_goods_tool/user_data.py`]() 进行配置。
-
-默认配置文件路径为 `./user_data.json`，可以通过 `-c` 或 `--conf` 参数指定配置文件路径。
+- 解决SSH客户端无法跳转人机验证链接的问题
+- 更新至极验第四代适应性验证
 
 ## 其他
+- [**🔗完整说明文档**](https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki)
 - 仅供学习时参考
 
 - 相似项目推荐:  \
-**mysTool - 米游社辅助工具插件**  \
-简介：NoneBot2 插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒  \
-🔗 https://github.com/Ljzd-PRO/nonebot-plugin-mystool
-
+  **mysTool - 米游社辅助工具插件**  \
+  简介：NoneBot2 插件 | 米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒  \
+  🔗 https://github.com/Ljzd-PRO/nonebot-plugin-mystool
+  
 - 本项目已开启[🔗Github Actions](https://github.com/Ljzd-PRO/Mys_Goods_Tool/actions)。
-欢迎[🔗指出Bug](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues)和[🔗贡献代码](https://github.com/Ljzd-PRO/Mys_Goods_Tool/pulls)👏
+  欢迎[🔗指出Bug](https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues)
+  和[🔗贡献代码](https://github.com/Ljzd-PRO/Mys_Goods_Tool/pulls)👏
 
 - 开发版分支：[🔗dev](https://github.com/Ljzd-PRO/Mys_Goods_Tool/tree/dev/)
 """
 
 
 class Welcome(Container):
     DEFAULT_CSS = """
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/user_data.py` & `mys_goods_tool-2.0.1/mys_goods_tool/user_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import traceback
 from json import JSONDecodeError
 from pathlib import Path
 from typing import List, Union, Optional, Tuple, Any, Dict, Set, Callable, TYPE_CHECKING, AbstractSet, \
     Mapping
 
 from httpx import Cookies
 from loguru import logger
@@ -13,15 +12,15 @@
 
 ROOT_PATH = Path("./")
 """程序所在目录"""
 
 CONFIG_PATH = ROOT_PATH / "user_data.json"
 """用户数据文件默认路径"""
 
-VERSION = "2.0.0-beta.1"
+VERSION = "2.0.1"
 """程序当前版本"""
 
 if TYPE_CHECKING:
     IntStr = Union[int, str]
     DictStrAny = Dict[str, Any]
     AbstractSetIntStr = AbstractSet[IntStr]
     MappingIntStrAny = Mapping[IntStr, Any]
@@ -292,25 +291,31 @@
     """兑换时所用的时区"""
     geetest_statics_path: Optional[Path]
     """GEETEST行为验证 网站静态文件目录（默认读取本地包自带的静态文件）"""
     geetest_listen_address: Optional[Tuple[str, int]] = ("localhost", 0)
     """登录时使用的 GEETEST行为验证 WEB服务 本地监听地址"""
     exchange_thread_count: int = 2
     """兑换线程数"""
-    exchange_latency: Tuple[float, float] = (0, 0.35)
+    exchange_latency: Tuple[float, float] = (0, 0.2)
     """兑换时间延迟随机范围（单位：秒）（防止因为发出请求的时间过于精准而被服务器认定为非人工操作）"""
     enable_log_output: bool = True
     """是否保存日志"""
     log_path: Optional[Path] = ROOT_PATH / "logs" / "mys_goods_tool.log"
     """日志保存路径"""
 
     @validator("log_path")
     def _(cls, v: Optional[Path]):
         absolute_path = v.absolute()
-        if not os.access(absolute_path, os.W_OK):
+        if not os.path.exists(absolute_path) or not os.path.isfile(absolute_path):
+            absolute_parent = absolute_path.parent
+            try:
+                os.makedirs(absolute_parent, exist_ok=True)
+            except PermissionError:
+                logger.warning(f"程序没有创建日志目录 {absolute_parent} 的权限")
+        elif not os.access(absolute_path, os.W_OK):
             logger.warning(f"程序没有写入日志文件 {absolute_path} 的权限")
         return v
 
     class Config:
         env_prefix = "MYS_GOODS_TOOL_"  # 环境变量前缀
 
 
@@ -469,32 +474,29 @@
     return True
 
 
 def load_config():
     """
     加载用户数据文件
     """
-    if os.path.isfile(CONFIG_PATH):
+    if os.path.exists(CONFIG_PATH) and os.path.isfile(CONFIG_PATH):
         try:
             return UserData.parse_file(CONFIG_PATH)
         except (ValidationError, JSONDecodeError):
-            logger.error(f"读取用户数据文件失败，请检查用户数据文件 {CONFIG_PATH} 格式是否正确")
-            logger.debug(traceback.format_exc())
+            logger.exception(f"读取用户数据文件失败，请检查用户数据文件 {CONFIG_PATH} 格式是否正确")
             exit(1)
         except:
-            logger.error(f"读取用户数据文件失败，请检查用户数据文件 {CONFIG_PATH} 是否存在且程序有权限读取和写入")
-            logger.debug(traceback.format_exc())
+            logger.exception(f"读取用户数据文件失败，请检查用户数据文件 {CONFIG_PATH} 是否存在且程序有权限读取和写入")
             exit(1)
     else:
         user_data = UserData()
         try:
             write_config_file(user_data)
         except PermissionError:
-            logger.error(f"创建用户数据文件失败，请检查程序是否有权限读取和写入 {CONFIG_PATH}")
-            logger.debug(traceback.format_exc())
+            logger.exception(f"创建用户数据文件失败，请检查程序是否有权限读取和写入 {CONFIG_PATH}")
             exit(1)
         # logger.info(f"用户数据文件 {CONFIG_PATH} 不存在，已创建默认用户数据文件。")
         # 由于会输出到标准输出流，影响TUI观感，因此暂时取消
 
         return user_data
```

### Comparing `mys_goods_tool-2.0.0b1/mys_goods_tool/utils.py` & `mys_goods_tool-2.0.1/mys_goods_tool/utils.py`

 * *Files identical despite different names*

### Comparing `mys_goods_tool-2.0.0b1/pyproject.toml` & `mys_goods_tool-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mys-goods-tool"
-version = "2.0.0-beta.1"
+version = "2.0.1"
 description = "米游社商品兑换工具|短信验证登录|终端TUI界面"
 authors = ["Ljzd-PRO <ljzd@office.ljzd-pro.ml>"]
 readme = "README.md"
 homepage = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 repository = "https://github.com/Ljzd-PRO/Mys_Goods_Tool"
 documentation = "https://github.com/Ljzd-PRO/Mys_Goods_Tool/wiki"
 keywords = ["mihoyo", "mihoyobbs", "genshin impact", "textual", "tui"]
@@ -19,23 +19,22 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Ljzd-PRO/Mys_Goods_Tool/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 tenacity = "^8.2.2"
-requests = "^2.29.0"
+requests = "^2.30.0"
 ping3 = "^4.0.4"
 ntplib = "^0.4.0"
-pyperclip = "^1.8.2"
 pydantic = "^1.10.6"
 loguru = "^0.7.0"
 httpx = "^0.24.0"
 rich = "^13.3.5"
-textual = "^0.22.3"
+textual = "^0.24.1"
 socksio = "^1.0.0"
 apscheduler = "^3.10.1"
 
 [tool.poetry.group.pyinstaller.dependencies]
 pyinstaller = "==5.10.1"
 
 [tool.poetry.group.test.dependencies]
```

