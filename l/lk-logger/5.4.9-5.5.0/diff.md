# Comparing `tmp/lk_logger-5.4.9-py3-none-any.whl.zip` & `tmp/lk_logger-5.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 34029 bytes, number of entries: 24
--rw-r--r--  2.0 unx      557 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
--rw-r--r--  2.0 unx      649 b- defN 80-Jan-01 00:00 lk_logger/_print.py
--rw-r--r--  2.0 unx     1716 b- defN 80-Jan-01 00:00 lk_logger/cache.py
--rw-r--r--  2.0 unx     5366 b- defN 80-Jan-01 00:00 lk_logger/config.py
+Zip file size: 36317 bytes, number of entries: 24
+-rw-r--r--  2.0 unx      592 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
+-rw-r--r--  2.0 unx      591 b- defN 80-Jan-01 00:00 lk_logger/_print.py
+-rw-r--r--  2.0 unx     1672 b- defN 80-Jan-01 00:00 lk_logger/cache.py
+-rw-r--r--  2.0 unx     5487 b- defN 80-Jan-01 00:00 lk_logger/config.py
 -rw-r--r--  2.0 unx     1563 b- defN 80-Jan-01 00:00 lk_logger/console.py
 -rw-r--r--  2.0 unx     4503 b- defN 80-Jan-01 00:00 lk_logger/control.py
--rw-r--r--  2.0 unx    10678 b- defN 80-Jan-01 00:00 lk_logger/logger.py
--rw-r--r--  2.0 unx     4847 b- defN 80-Jan-01 00:00 lk_logger/markup.py
--rw-r--r--  2.0 unx     5271 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
--rw-r--r--  2.0 unx     7675 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
+-rw-r--r--  2.0 unx     6440 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
+-rw-r--r--  2.0 unx    11873 b- defN 80-Jan-01 00:00 lk_logger/logger.py
+-rw-r--r--  2.0 unx    10446 b- defN 80-Jan-01 00:00 lk_logger/markup.py
+-rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
+-rw-r--r--  2.0 unx     9899 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
 -rw-r--r--  2.0 unx     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
 -rw-r--r--  2.0 unx     2559 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
 -rw-r--r--  2.0 unx       71 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 unx     6247 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 unx     1128 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 unx     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 unx     9594 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 unx    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 unx      491 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
--rw-r--r--  2.0 unx     6666 b- defN 80-Jan-01 00:00 lk_logger/sourcemap.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.4.9.dist-info/WHEEL
--rw-r--r--  2.0 unx     4899 b- defN 80-Jan-01 00:00 lk_logger-5.4.9.dist-info/METADATA
-?rw-r--r--  2.0 unx     1919 b- defN 16-Jan-01 00:00 lk_logger-5.4.9.dist-info/RECORD
-24 files, 105177 bytes uncompressed, 30963 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 lk_logger-5.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     4884 b- defN 80-Jan-01 00:00 lk_logger-5.5.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     1921 b- defN 16-Jan-01 00:00 lk_logger-5.5.0.dist-info/RECORD
+24 files, 115004 bytes uncompressed, 33249 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: lk_logger/console.py
 Comment: 
 
 Filename: lk_logger/control.py
 Comment: 
 
+Filename: lk_logger/frame_info.py
+Comment: 
+
 Filename: lk_logger/logger.py
 Comment: 
 
 Filename: lk_logger/markup.py
 Comment: 
 
 Filename: lk_logger/message_builder.py
@@ -54,20 +57,17 @@
 
 Filename: lk_logger/scanner/text_scanner.py
 Comment: 
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
-Filename: lk_logger/sourcemap.py
-Comment: 
-
-Filename: lk_logger-5.4.9.dist-info/WHEEL
+Filename: lk_logger-5.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.4.9.dist-info/METADATA
+Filename: lk_logger-5.5.0.dist-info/METADATA
 Comment: 
 
-Filename: lk_logger-5.4.9.dist-info/RECORD
+Filename: lk_logger-5.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -5,19 +5,20 @@
 from .control import enable
 from .control import enable as unmute
 from .control import setup
 from .control import start_ipython
 from .control import unload
 from .control import unload as restore_builtin_print
 from .control import update
+from .frame_info import FrameInfo
 from .logger import lk
 from .pipeline import pipeline
 
 
 def __init():
     import traceback
     pipeline.add(traceback, bprint)
     setup(quiet=True)
 
 
 __init()
-__version__ = '5.4.9'
+__version__ = '5.5.0'
```

## lk_logger/_print.py

```diff
@@ -1,18 +1,17 @@
 import builtins
 from inspect import currentframe
 from os import name as os_name
 
-# DELETE: `builtin_print` is goint to be removed.
-bprint = builtin_print = builtins.print
+bprint = builtins.print
 std_print = builtins.print
 non_print = lambda *_, **__: None
 
 
-def debug(*args, condition=True):
+def debug(*args, condition=True) -> None:
     frame = currentframe().f_back
     filepath = _normpath(frame.f_globals["__file__"])
     lineno = frame.f_lineno
     source = '{}:{}'.format(filepath, lineno)
     if condition:
         bprint(source, '[LKDEBUG]', *args)
```

## lk_logger/cache.py

```diff
@@ -1,43 +1,40 @@
-from __future__ import annotations
-
 import typing as t
+from .markup import T as T0
 
 
 class T:  # Typehint
-    from .markup import T as _TMarkup  # noqa
-    
     FrameId = str
     MarkupPos = int
     Markup = str
     
     Cache = t.Dict[FrameId, t.TypedDict('_SubDict0', {
         'markup_pos'   : MarkupPos,  # noqa
-        'marks_meaning': _TMarkup.MarksMeaning,  # noqa
+        'marks_meaning': T0.MarksMeaning,  # noqa
         'info'         : t.Dict[Markup, dict]
     })]
 
 
 class LoggingCache:
     _cache: T.Cache
     
-    def __init__(self):
+    def __init__(self) -> None:
         from collections import defaultdict
         self._cache = defaultdict(lambda: {
             'markup_pos'   : None,
             'marks_meaning': {},
             'info'         : {},
         })
     
-    def clear_cache(self):
+    def clear_cache(self) -> None:
         self._cache.clear()
     
     # -------------------------------------------------------------------------
     
-    def get_markup_pos(self, frame_id: T.FrameId) -> T.MarkupPos | None:
+    def get_markup_pos(self, frame_id: T.FrameId) -> t.Optional[T.MarkupPos]:
         return self._cache[frame_id].get('markup_pos', None)
     
     def is_cached(self, frame_id: T.FrameId, markup: T.Markup) -> bool:
         return (
                 frame_id in self._cache and
                 markup in self._cache[frame_id]['info']
         )
```

## lk_logger/config.py

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import sys
 import typing as t
 from sys import excepthook as _default_excepthook
 
 
 class LoggingConfig:
     """
@@ -48,51 +46,53 @@
                     show only the library name (surrounded by brackets).
                     example: '[lk_logger]'
             ps: if you don't want to show anything, you should turn to set
             `show_external_lib` to False.
     """
     async_: bool
     clear_unfinished_stream: bool
-    console_width: int | None
+    console_width: t.Optional[int]
     path_style_for_external_lib: str
     rich_traceback: bool
     separator: str
     show_external_lib: bool
     show_funcname: bool
     show_source: bool
     show_varnames: bool
+    v2_meaning: t.Literal['info', 'success']  # TODO: not used.
     
     _preset_conf = {
         'async_'                     : True,
         'clear_unfinished_stream'    : False,
         'console_width'              : None,
         'path_style_for_external_lib': 'pretty_relpath',
         'rich_traceback'             : True,
         'separator'                  : ';   ',
         'show_external_lib'          : True,
         'show_funcname'              : True,
         'show_source'                : True,
         'show_varnames'              : False,
+        'v2_meaning'                 : 'info',
     }
     
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         for k, v in self._merge_dict(self._preset_conf, kwargs).items():
             self._apply(k, v)
     
-    def update(self, **kwargs):
+    def update(self, **kwargs) -> None:
         for k, v in kwargs.items():
             if k in self._preset_conf and v != getattr(self, k, None):
                 self._apply(k, v)
     
-    def reset(self):
+    def reset(self) -> None:
         for k, v in self._preset_conf.items():
             if v != getattr(self, k, None):
                 self._apply(k, v)
     
-    def _apply(self, key: str, val: bool | int | str):
+    def _apply(self, key: str, val: t.Union[bool, int, str]) -> None:
         setattr(self, key, val)
         if key == 'console_width':
             if val and isinstance(val, int):
                 from .console import console
                 console.width = val
         elif key == 'rich_traceback':
             import sys
@@ -121,15 +121,15 @@
             print(':r', '[red dim]KeyboardInterrupt[/]')
             sys.exit(0)
         else:
             callback(type_, value, traceback)
     
     # -------------------------------------------------------------------------
     
-    def to_dict(self) -> dict[str, t.Any]:
+    def to_dict(self) -> t.Dict[str, t.Any]:
         return {
             k: getattr(self, k)
             for k in self._preset_conf
         }
     
     @staticmethod
     def _merge_dict(base: dict, update: dict) -> dict:
```

## lk_logger/logger.py

```diff
@@ -2,34 +2,40 @@
 
 import typing as t
 from atexit import register
 from collections import deque
 from inspect import currentframe
 from threading import Thread
 from time import sleep
-from types import FrameType as _FrameType
 
+from rich.console import RenderableType
+from rich.traceback import Traceback
+
+from ._print import bprint
 from ._print import debug  # noqa
 from .cache import LoggingCache
 from .config import LoggingConfig
 from .console import con_print
+from .frame_info import FrameInfo
 from .markup import MarkMeaning
 from .markup import MarkupAnalyser
 from .markup import T as T0
 from .message_builder import MessageBuilder
 from .path_helper import path_helper
 from .pipeline import pipeline
-from .sourcemap import sourcemap
 
 __all__ = ['LKLogger', 'lk']
 
 
+class _RawArgs:  # a workaround. see its usage below.
+    def __init__(self, args: t.Tuple[t.Any, ...]):
+        self.args = args
+
+
 class T(T0):  # Typehint
-    Frame = _FrameType
-    
     Args = t.Tuple[t.Any, ...]
     MarkupPos = int  # -1, 0, 1
     
     # MessageQueue = t.List[
     #     t.Tuple[t.Union[str, tuple], dict,
     #             t.Optional[t.Callable]]
     # ]
@@ -43,16 +49,18 @@
     })
     
     FlushScheme = int
     #   0: no flush
     #   1: instant flush
     #   2: instant flush and drain
     #   3: wait for flush
-    ComposedMessage = t.Tuple[str, FlushScheme]
-    #   tuple[str message, int flush_scheme]
+    ComposedMessage = t.Tuple[
+        t.Union[str, RenderableType, Traceback, _RawArgs],
+        FlushScheme
+    ]
 
 
 class LKLogger:
     
     def __init__(self):
         self._analyser = MarkupAnalyser()
         self._builder = MessageBuilder()
@@ -81,117 +89,148 @@
         )
     
     @property
     def config(self) -> dict:
         return self._config.to_dict()
     
     def _start_running(self):
+        
+        def consume() -> None:
+            msg: t.Union[str, tuple]
+            kwargs: dict
+            custom_print: t.Optional[t.Callable]
+            
+            for i in range(len(self._message_queue)):
+                msg, kwargs, custom_print = self._message_queue.popleft()
+                if custom_print:
+                    # debug(custom_print, msg, kwargs)
+                    kwargs.pop('file', None)
+                    custom_print(*msg, **kwargs)
+                else:
+                    con_print(msg, **kwargs)
+        
         self._running = True
-        while self._running or self._message_queue:
+        while self._running:
             if self._message_queue:
-                try:
-                    msg, kwargs, custom_print = self._message_queue.popleft()
-                    if custom_print:
-                        custom_print(*msg, **kwargs)
-                    else:
-                        con_print(msg, **kwargs)
-                except Exception as e:
-                    debug(e)
-                    # raise e
+                consume()
             else:
                 sleep(10E-3)
+        else:
+            consume()
     
     def _stop_running(self):
-        self._running = False
         if self._config.clear_unfinished_stream:
             self._message_queue.clear()
+        self._running = False
         self._thread.join()
     
     # -------------------------------------------------------------------------
     
-    def log(self, *args, **kwargs) -> None:
-        caller_frame = currentframe().f_back
+    def log(self, *args, _frame_info: FrameInfo = None, **kwargs) -> None:
+        if _frame_info is None:
+            _frame_info = FrameInfo(currentframe().f_back)
         
-        if (path := caller_frame.f_globals.get('__file__')) and \
-                (custom_print := pipeline.get(path)):
+        if (path := _frame_info.filepath) \
+                and (custom_print := pipeline.get(path)):
             if self._config.async_:
                 self._message_queue.append((args, kwargs, custom_print))
             else:
                 custom_print(*args, **kwargs)
             return
         
-        msg, flush_scheme = self._build_message(caller_frame, *args)
+        msg, flush_scheme = self._build_message(_frame_info, *args)
+        is_raw = isinstance(msg, _RawArgs)
         # debug(msg)
         
         if flush_scheme == 0:
             if self._config.async_:
-                self._message_queue.append((msg, kwargs, None))
+                if is_raw:
+                    self._message_queue.append((msg.args, kwargs, bprint))
+                else:
+                    self._message_queue.append((msg, kwargs, None))
             else:
-                con_print(msg, **kwargs)
+                if is_raw:
+                    bprint(*msg.args, **kwargs)
+                else:
+                    con_print(msg, **kwargs)
         elif flush_scheme == 1:
-            con_print(msg, **kwargs)
+            while self._message_queue:
+                sleep(10E-3)
+            if is_raw:
+                bprint(*msg.args, **kwargs)
+            else:
+                con_print(msg, **kwargs)
         elif flush_scheme == 2:
             if skipped_count := len(self._message_queue):
                 self._message_queue.clear()
                 print(':frp', f'[red dim](... skipped '
                               f'{skipped_count} messages)[/]')
-            con_print(msg, **kwargs)
+            if is_raw:
+                bprint(*msg.args, **kwargs)
+            else:
+                con_print(msg, **kwargs)
         elif flush_scheme == 3:
-            while self._message_queue:
-                sleep(10E-3)
-            con_print(msg, **kwargs)
-    
-    def fmt(self, *args, **_) -> str:
-        return str(self._build_message(currentframe().f_back, *args)[0])
+            if is_raw:
+                bprint(*msg.args, **kwargs)
+            else:
+                con_print(msg, **kwargs)
     
-    def _build_message(self, frame: T.Frame, *args) -> T.ComposedMessage:
+    def fmt(self, _frame_info: FrameInfo = None, *args, **_) -> str:
+        return str(self._build_message(
+            _frame_info or FrameInfo(currentframe().f_back), *args
+        )[0])
+    
+    def _build_message(
+            self, frame_info: FrameInfo, *args
+    ) -> T.ComposedMessage:
         """
         return: (str message, bool is_flush, bool is_drain)
             flush: print the message immediately.
             drain: drain the message queue.
                 if drain is True, the flush must be True.
         """
-        frame_id = '{}:{}'.format(frame.f_code.co_filename, frame.f_lineno)
         args, markup_pos, markup = \
-            self._extract_markup_from_arguments(frame_id, args)
+            self._extract_markup_from_arguments(frame_info.id, args)
         marks = self._analyser.extract(markup)
-        marks_meaning = self._analyser.analyse(marks)
         
-        if marks['p']:
-            real_frame = frame
-            for _ in range(marks['p']):
-                real_frame = real_frame.f_back
-            frame_id = '{}:{}'.format(
-                real_frame.f_code.co_filename,
-                real_frame.f_lineno
-            )
-        # debug(frame_id)
+        get_varnames = frame_info.collect_varnames  # backup method pointer
+        if marks['p']: frame_info = frame_info.get_parent(marks['p'])
+        marks_meaning = self._analyser.analyse(marks, frame_info=frame_info)
+        del marks
         
         flush_scheme: T.FlushScheme = 0
         if MarkMeaning.FLUSH in marks_meaning:
             flush_scheme = 1
-        elif MarkMeaning.FLUSH_AND_DRAIN in marks_meaning:
+        elif MarkMeaning.FLUSH_CUTOFF in marks_meaning:
             flush_scheme = 2
-        elif MarkMeaning.WAIT_TO_FLUSH in marks_meaning:
+        elif MarkMeaning.FLUSH_EDDY in marks_meaning:
             flush_scheme = 3
         
         # check cache
-        if self._cache.is_cached(frame_id, markup):
-            cached_info = self._cache.get_cache(frame_id, markup)
+        if self._cache.is_cached(frame_info.id, markup):
+            cached_info = self._cache.get_cache(frame_info.id, markup)
             return self._builder.compose(
                 args, marks_meaning, cached_info
             ), flush_scheme
         
         # ---------------------------------------------------------------------
         
         if MarkMeaning.AGRESSIVE_PRUNE in marks_meaning:
             return self._builder.quick_compose(args), flush_scheme
+        elif MarkMeaning.BUILTIN_PRINT in marks_meaning:
+            return _RawArgs(args), flush_scheme
         elif MarkMeaning.RICH_OBJECT in marks_meaning:
-            # assert len(args) == 1 and isinstance(args[1], rich.Renderable)
-            return (args[0] if args else None), flush_scheme
+            assert len(args) == 1 and isinstance(args[0], RenderableType)
+            return args[0], flush_scheme
+        elif MarkMeaning.TRACEBACK_EXCEPTION in marks_meaning:
+            assert len(args) == 1 and isinstance(args[0], BaseException)
+            return self._builder.compose_exception(args[0], False), flush_scheme
+        elif MarkMeaning.TRACEBACK_EXCEPTION_WITH_LOCALS in marks_meaning:
+            assert len(args) == 1 and isinstance(args[0], BaseException)
+            return self._builder.compose_exception(args[0], True), flush_scheme
         
         info: T.Info = {
             'file_path'      : '',
             'line_number'    : '0',
             'is_external_lib': False,
             'function_name'  : '',
             'variable_names' : (),
@@ -199,62 +238,54 @@
         
         show_source = self._config.show_source
         show_funcname = self._config.show_funcname
         show_varnames = self._config.show_varnames and \
                         MarkMeaning.MODERATE_PRUNE not in marks_meaning
         
         if any((show_source, show_funcname, show_varnames)):
-            # PERF: here does redundant work in tracing real frame. we need to
-            #   merge this with the above tracing.
-            srcmap = sourcemap.get_sourcemap(
-                frame=frame,
-                traceback_level=marks['p'],
-                advanced=show_varnames,
-            )
-            
             if show_source:
                 def update_sourcemap():
                     """
                     this function updates follows:
                         info['is_external_lib']
                         info['file_path']
                         info['line_number']
                     """
-                    
-                    path = srcmap.filepath
+                    path = frame_info.filepath
                     info['is_external_lib'] = path_helper.is_external_lib(path)
                     
                     if info['is_external_lib']:
                         if self._config.show_external_lib:
                             style = self._config.path_style_for_external_lib
                             info['file_path'] = \
                                 path_helper.reformat_external_lib_path(
                                     path, style
                                 )
                         else:
                             info['file_path'] = ''
                     else:
                         info['file_path'] = path_helper.relpath(path)
                     
-                    info['line_number'] = str(srcmap.lineno)
+                    info['line_number'] = str(frame_info.lineno)
                 
                 update_sourcemap()
             
             if show_funcname:
-                info['function_name'] = srcmap.funcname
+                info['function_name'] = frame_info.funcname
             
             if show_varnames:
+                varnames = get_varnames()
                 if markup_pos == 0:
-                    info['variable_names'] = srcmap.varnames
+                    info['variable_names'] = varnames
                 elif markup_pos == 1:
-                    info['variable_names'] = srcmap.varnames[1:]
+                    info['variable_names'] = varnames[1:]
                 else:
-                    info['variable_names'] = srcmap.varnames[:-1]
+                    info['variable_names'] = varnames[:-1]
         
-        self._cache.store_info(frame_id, markup, info)
+        self._cache.store_info(frame_info.id, markup, info)
         
         return self._builder.compose(
             args, marks_meaning, info
         ), flush_scheme
     
     def _extract_markup_from_arguments(
             self, frame_id: str, args: T.Args
```

## lk_logger/markup.py

```diff
@@ -1,163 +1,296 @@
-from __future__ import annotations
-
 import typing as t
+from collections import defaultdict
 from enum import Enum
 from enum import auto
+from random import choices
 from re import compile as re_compile
+from string import ascii_lowercase
 from time import time
 
+from .frame_info import FrameInfo
+
 
 # noinspection PyArgumentList
 class MarkMeaning(Enum):
     AGRESSIVE_PRUNE = auto()
     BUILTIN_PRINT = auto()
     DIVIDER_LINE = auto()
     EXPAND_MULTIPLE_LINES = auto()
     FLUSH = auto()
-    FLUSH_AND_DRAIN = auto()
+    FLUSH_CUTOFF = auto()
+    FLUSH_EDDY = auto()
     MODERATE_PRUNE = auto()
+    PARENT_POINTER = auto()
     RESET_INDEX = auto()
     RESET_TIMER = auto()
     RICH_FORMAT = auto()
     RICH_OBJECT = auto()
+    SCOPED_COUNTER = auto()
+    SIMPLE_COUNTER = auto()
     START_TIMER = auto()
     STOP_TIMER = auto()
     TRACEBACK_EXCEPTION = auto()
-    UPDATE_INDEX = auto()
+    TRACEBACK_EXCEPTION_WITH_LOCALS = auto()
     VERBOSITY = auto()
-    WAIT_TO_FLUSH = auto()
 
 
 class T:
     Markup = str
     Marks = t.TypedDict('Marks', {
         'd': int,  # divider line
-        'e': int,  # exception stack trace  # TODO
+        'e': int,  # exception trace back
         'i': int,  # index
         'f': int,  # flush
         'l': int,  # long / loose / expanded (multiple lines)
         'p': int,  # parent layer
         'r': int,  # rich style
         's': int,  # short / simple / single line
         't': int,  # timer / timestamp
         'v': int,  # verbosity / log level
     })
     MarksMeaning = t.Dict[MarkMeaning, t.Any]
+    
+    class Counter:
+        ColorHex = str
+        Fid = str
+        Indent = int
+        Index = int
+        Uid = str
+        
+        Fid2Uid = t.DefaultDict[Indent, t.DefaultDict[Fid, Uid]]
+        ScopedCounts = t.DefaultDict[Uid, Index]
+        Uid2ColorHex = t.DefaultDict[Uid, ColorHex]
+
+
+class E:
+    class UnsupportedMarkup(Exception):
+        pass
 
 
 class MarkupAnalyser:
     """
     readme: prj:/docs/markup.zh.md
     """
+    _counter: '_Counter'
+    _levels: t.Tuple[str, ...]
     _mark_pattern_0 = re_compile(r'^:(?:[defilprstv][0-9]?)+$')
     _mark_pattern_1 = re_compile(r'\w\d?')
+    _simple_time: float
+    
+    def __init__(self) -> None:
+        self._counter = _Counter()
+        self._simple_time = time()
+        # TODO or DELETE: not used. see also `def extract : local_var levels`
+        self._levels = ('trace', 'debug', 'info', 'warn', 'error', 'fatal')
     
     def is_valid_markup(self, text: str) -> bool:
         return bool(self._mark_pattern_0.match(text))
     
     def extract(self, markup: T.Markup) -> T.Marks:
         """
+        description: (the asterisk * means default value)
+            * d0: divider line
+              d1: divider block                               *(not supported)*
+            * e0: exception trace back
+              e1: exception trace back with showing locals
+              e2: enter pdb                                   *(not supported)*
+            * f0: flush
+              f1: flush cutoff
+              f2: flush eddy               *(not a good option, maybe removed)*
+              i0: reset index
+            * i1: update index
+              i2: scoped counter
+              i3: progress                                    *(not supported)*
+            * l0: long / loose / expanded (multiple lines)
+              l1: force expand all nodes                      *(not supported)*
+              p0: self layer
+            * p1: parent layer
+              p2: grandparent layer                    *(be careful using p2+)*
+              p3: great-grandparent layer
+              p4: and so on...
+            * r0: rich style
+              r1: rich object (rich.table.Table, rich.panel.Panel, etc.)
+            * s0: short / simple / single line
+              s1: builtin-like print (remains markup features)
+              s2: builtin print
+              t0: reset timer
+              t1: start timer
+            * t2: stop timer and show statistics
+              v0: no obvious verbosity
+            * v1: debug
+              v2: info
+              v3: warning
+              v4: error
+              v5: critical
+        
         return:
-            dict[literal mark, int value]
+            dict[literal mark, int level]
         """
         defaults = {
-            'd': -1,
-            'e': -1,
-            'f': -1,
-            'i': -1,
-            'l': -1,
-            'p': 0,
-            'r': -1,
-            's': -1,
-            't': -1,
-            'v': 0,
-        }
-        shortcuts = {
             'd': 0,
             'e': 0,
             'f': 0,
-            'i': 1,
+            'i': 1,  # `:i0` is 'reset index'
             'l': 0,
-            'p': 1,
+            'p': 1,  # `:p0` points to 'self' layer
             'r': 0,
             's': 0,
-            't': 2,
-            'v': 1,
+            't': 2,  # `:t0` is 'reset timer'; `:t1` is 'start timer'
+            'v': 1,  # `:v0` is 'no obvious verbosity'
         }
-        
-        out = defaults.copy()
+        out = defaultdict(lambda: -1)
         for m in (self._mark_pattern_1.findall(markup) or ()):
             if len(m) == 1:
-                out[m[0]] = shortcuts[m[0]]
+                out[m[0]] = defaults[m[0]]
             else:
                 out[m[0]] = int(m[1:])
         return out
     
-    _simple_count = 0
-    _simple_time = time()
-    
-    def analyse(self, marks: T.Marks) -> T.MarksMeaning:
+    def analyse(self, marks: T.Marks, **kwargs) -> T.MarksMeaning:
         out = {}
         
         if marks['d'] >= 0:
-            out[MarkMeaning.DIVIDER_LINE] = '-' * 64
+            if marks['d'] == 0:
+                out[MarkMeaning.DIVIDER_LINE] = '-'  # pattern
+                #   TODO: currently suggest using only one character.
+            else:
+                raise E.UnsupportedMarkup(f':d{marks["d"]}')
         
         if marks['e'] >= 0:
-            out[MarkMeaning.TRACEBACK_EXCEPTION] = True
+            if marks['e'] == 0:
+                out[MarkMeaning.TRACEBACK_EXCEPTION] = True
+            elif marks['e'] == 1:
+                out[MarkMeaning.TRACEBACK_EXCEPTION_WITH_LOCALS] = True
+            else:
+                raise E.UnsupportedMarkup(f':e{marks["e"]}')
         
         if marks['f'] >= 0:
             if marks['f'] == 0:
                 out[MarkMeaning.FLUSH] = True
             elif marks['f'] == 1:
-                out[MarkMeaning.FLUSH_AND_DRAIN] = True
+                out[MarkMeaning.FLUSH_CUTOFF] = True
             elif marks['f'] == 2:
-                out[MarkMeaning.WAIT_TO_FLUSH] = True
+                out[MarkMeaning.FLUSH_EDDY] = True
+            else:
+                raise E.UnsupportedMarkup(f':f{marks["f"]}')
         
-        if marks['i'] == 0:
-            self._simple_count = 0
-            out[MarkMeaning.RESET_INDEX] = 0
-            out[MarkMeaning.RICH_FORMAT] = True
-        elif marks['i'] >= 1:
-            self._simple_count += 1
-            out[MarkMeaning.UPDATE_INDEX] = self._simple_count
+        if marks['i'] >= 0:
+            if marks['i'] == 0:
+                out[MarkMeaning.RESET_INDEX] = \
+                    self._counter.reset_simple_count()
+                out[MarkMeaning.RICH_FORMAT] = True
+            elif marks['i'] == 1:
+                out[MarkMeaning.SIMPLE_COUNTER] = \
+                    self._counter.update_simple_count()
+            elif marks['i'] == 2:
+                info: FrameInfo = kwargs['frame_info']
+                out[MarkMeaning.SCOPED_COUNTER] = \
+                    self._counter.update_scoped_count(
+                        info.id, info.indentation
+                    )
+            else:
+                raise E.UnsupportedMarkup(f':i{marks["i"]}')
         
         if marks['l'] >= 0:
-            out[MarkMeaning.EXPAND_MULTIPLE_LINES] = True
+            if marks['l'] == 0:
+                out[MarkMeaning.EXPAND_MULTIPLE_LINES] = True
+            else:
+                raise E.UnsupportedMarkup(f':l{marks["l"]}')
         
-        if marks['r'] == 0:
-            out[MarkMeaning.RICH_FORMAT] = True
-        elif marks['r'] == 1:
-            out[MarkMeaning.RICH_OBJECT] = True
+        if marks['p'] >= 0:
+            out[MarkMeaning.PARENT_POINTER] = marks['p']
+        else:
+            out[MarkMeaning.PARENT_POINTER] = 0
+        
+        if marks['r'] >= 0:
+            if marks['r'] == 0:
+                out[MarkMeaning.RICH_FORMAT] = True
+            elif marks['r'] == 1:
+                out[MarkMeaning.RICH_OBJECT] = True
+            else:
+                raise E.UnsupportedMarkup(f':r{marks["r"]}')
         
-        if marks['s'] == 0:
-            out[MarkMeaning.MODERATE_PRUNE] = True
-        elif marks['s'] == 1:
-            out[MarkMeaning.AGRESSIVE_PRUNE] = True
-        elif marks['s'] == 2:
-            out[MarkMeaning.BUILTIN_PRINT] = True
+        if marks['s'] >= 0:
+            if marks['s'] == 0:
+                out[MarkMeaning.MODERATE_PRUNE] = True
+            elif marks['s'] == 1:
+                out[MarkMeaning.AGRESSIVE_PRUNE] = True
+            elif marks['s'] == 2:
+                out[MarkMeaning.BUILTIN_PRINT] = True
+            else:
+                raise E.UnsupportedMarkup(f':s{marks["s"]}')
         
         if marks['t'] >= 0:
             out[MarkMeaning.RICH_FORMAT] = True
             if marks['t'] == 0:
                 t = self._simple_time = time()
                 out[MarkMeaning.RESET_TIMER] = t
             elif marks['t'] == 1:
                 t = self._simple_time = time()
                 out[MarkMeaning.START_TIMER] = t
             elif marks['t'] == 2:
                 start, end = self._simple_time, time()
                 self._simple_time = end
                 out[MarkMeaning.STOP_TIMER] = (start, end)
+            else:
+                raise E.UnsupportedMarkup(f':t{marks["t"]}')
         
         if marks['v'] >= 1:
             levels = ('trace', 'debug', 'info', 'warn', 'error', 'fatal')
             out[MarkMeaning.VERBOSITY] = levels[marks['v']]
         
-        # postfix
-        # if any((
-        #     MarkMeaning.RESET_INDEX in out,
-        #     MarkMeaning.EXPAND_MULTIPLE_LINES in out,
-        # )):
-        #     out[MarkMeaning.RICH_FORMAT] = True
-        
         return out
+
+
+class _Counter:
+    _fid_2_uid: T.Counter.Fid2Uid
+    _last_indent: T.Counter.Indent
+    _last_uid: T.Counter.Uid
+    _scoped_counts: T.Counter.ScopedCounts
+    _simple_count: T.Counter.Index
+    _uid_2_color: T.Counter.Uid2ColorHex
+    
+    def __init__(self) -> None:
+        self._simple_count = 0
+        self._scoped_counts = defaultdict(lambda: 0)
+        self._fid_2_uid = defaultdict(lambda: defaultdict(self._generate_uid))
+        self._uid_2_color = defaultdict(self._get_random_bright_color)
+        self._last_indent = 0
+        self._last_uid = ''
+    
+    @staticmethod
+    def _generate_uid() -> T.Counter.Uid:
+        """
+        randomly generate a four-character uid.
+        """
+        return ''.join(choices(ascii_lowercase, k=4))
+    
+    @staticmethod
+    def _get_random_bright_color() -> T.Counter.ColorHex:
+        # https://stackoverflow.com/questions/43437309
+        return '#' + ''.join(choices('89ABCDEF', k=6))
+    
+    def update_simple_count(self) -> T.Counter.Index:
+        self._simple_count += 1
+        return self._simple_count
+    
+    def update_scoped_count(
+            self,
+            fid: T.Counter.Fid,
+            indent: T.Counter.Indent
+    ) -> t.Tuple[T.Counter.Index, T.Counter.Uid, T.Counter.ColorHex]:
+        if self._last_indent > indent:
+            # reset all counts in higher indented levels
+            for indent_j in sorted(self._fid_2_uid.keys(), reverse=True):
+                if indent_j <= indent: break
+                for uid in self._fid_2_uid[indent_j].values():
+                    self._scoped_counts[uid] = 0
+        self._last_indent = indent
+        
+        uid = self._fid_2_uid[indent][fid]
+        self._scoped_counts[uid] += 1
+        return self._scoped_counts[uid], uid, self._uid_2_color[uid]
+    
+    def reset_simple_count(self) -> T.Counter.Index:
+        self._simple_count = 0
+        return 0
```

## lk_logger/message_builder.py

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import typing as t
 
+from rich.traceback import Traceback
+
 from .markup import MarkMeaning
 from .message_formatter import MessageFormatter
 
 
 class T:
     from .markup import T as _TMarkup  # noqa
     Args = t.Tuple[t.Any, ...]
@@ -31,18 +33,20 @@
     def quick_compose(self, args: T.Args) -> str:
         return (
             '[bright_black]{separator}[/]'.format(
                 separator=self._separator
             ).join(map(str, args))
         )
     
-    def compose(self,
-                args: T.Args,
-                marks_meaning: T.MarksMeaning,
-                info: dict) -> str:
+    def compose(
+            self,
+            args: T.Args,
+            marks_meaning: T.MarksMeaning,
+            info: dict
+    ) -> str:
         if MarkMeaning.AGRESSIVE_PRUNE in marks_meaning:
             return self.quick_compose(args)
         
         message_elements = []
         
         # 1. source
         if self._show_source:
@@ -76,28 +80,35 @@
             if MarkMeaning.MODERATE_PRUNE not in marks_meaning:
                 message_elements.append(
                     self._formatter.fmt_level(
                         marks_meaning[MarkMeaning.VERBOSITY],
                     )
                 )
                 message_elements.append(' ')
-
+        
         # 4. index
         if MarkMeaning.RESET_INDEX in marks_meaning:
             if MarkMeaning.MODERATE_PRUNE in marks_meaning:
                 pass
             else:
                 message_elements.append(self._formatter.fmt_index(0))
                 message_elements.append(' ')
                 if not args:
                     args = ('[grey50]reset index[/]',)
-        elif MarkMeaning.UPDATE_INDEX in marks_meaning:
+        elif MarkMeaning.SIMPLE_COUNTER in marks_meaning:
             message_elements.append(
                 self._formatter.fmt_index(
-                    marks_meaning[MarkMeaning.UPDATE_INDEX]
+                    marks_meaning[MarkMeaning.SIMPLE_COUNTER]
+                )
+            )
+            message_elements.append(' ')
+        elif MarkMeaning.SCOPED_COUNTER in marks_meaning:
+            message_elements.append(
+                self._formatter.fmt_scoped_index(
+                    *marks_meaning[MarkMeaning.SCOPED_COUNTER]
                 )
             )
             message_elements.append(' ')
         
         # 5. timestamp
         if MarkMeaning.RESET_TIMER in marks_meaning:
             if not args:
@@ -118,21 +129,21 @@
                     marks_meaning[MarkMeaning.RESET_TIMER]
                 )
             ), *args)
         elif MarkMeaning.STOP_TIMER in marks_meaning:
             s, e = marks_meaning[MarkMeaning.STOP_TIMER]
             args = (self._formatter.fmt_time(s, e), *args)
         
-        # 6. divider
-        if MarkMeaning.DIVIDER_LINE in marks_meaning:
-            div = marks_meaning[MarkMeaning.DIVIDER_LINE]
-            message_elements.append(
-                self._formatter.fmt_divider(div)
-            )
-            message_elements.append(' ')
+        # # 6. divider
+        # if MarkMeaning.DIVIDER_LINE in marks_meaning:
+        #     pattern = marks_meaning[MarkMeaning.DIVIDER_LINE]
+        #     message_elements.append(
+        #         self._formatter.fmt_divider(pattern)
+        #     )
+        #     message_elements.append(' ')
         
         # 7. arguments
         message_elements.append(
             self._formatter.fmt_message(
                 arguments=args,
                 varnames=info['variable_names'] if self._show_varnames else (),
                 rich=MarkMeaning.RICH_FORMAT in marks_meaning,
@@ -143,8 +154,25 @@
         if MarkMeaning.VERBOSITY in marks_meaning and \
                 MarkMeaning.EXPAND_MULTIPLE_LINES not in marks_meaning:
             message_elements[-1] = self._formatter.fmt_level(
                 marks_meaning[MarkMeaning.VERBOSITY],
                 text=message_elements[-1]
             )
         
+        # PERF: this is not a good design.
+        # 6. divider
+        if MarkMeaning.DIVIDER_LINE in marks_meaning:
+            message_elements.insert(len(message_elements) - 1, ' ')
+            pattern = marks_meaning[MarkMeaning.DIVIDER_LINE]
+            divider = self._formatter.fmt_divider(
+                pattern, context=message_elements
+            )
+            message_elements.insert(len(message_elements) - 2, divider)
+        
         return ''.join(message_elements)
+    
+    def compose_exception(
+            self,
+            e: BaseException,
+            show_locals: bool
+    ) -> Traceback:
+        return self._formatter.fmt_exception(e, show_locals)
```

## lk_logger/message_formatter.py

```diff
@@ -4,16 +4,18 @@
 from math import ceil
 from textwrap import indent
 from time import localtime
 from time import strftime as _strftime
 from traceback import format_exception
 
 from rich.pretty import pretty_repr
+from rich.traceback import Traceback
 
 from ._print import debug  # noqa
+from .console import console
 
 strftime = lambda t: _strftime('%H:%M:%S', localtime(t)) \
     if t is not None else ''
 
 
 class Color:  # TODO: not used yet (and not ready).
     SEPARATOR = 'bright_black'
@@ -53,16 +55,142 @@
                 out.append('[{}]{}[/]'.format(mark, text))
             else:
                 out.append(text)
         return ''.join(out)
     
     # -------------------------------------------------------------------------
     
-    def fmt_source(self, filepath: str, lineno: t.Union[int, str],
-                   is_external_lib: bool = False, fmt_width=False) -> str:
+    def fmt_divider(
+            self, pattern: str = '-', length: int = None,
+            context: list[str] = None
+    ) -> str:  # PERF: not a good design.
+        if length is None:
+            if context:
+                measure = console.measure(''.join(context))
+                # length = console.width - measure.maximum
+                length = min((console.width, 200)) - measure.maximum
+                # if length > 80:
+                #     length = 80
+                if length <= 0:
+                    if len(context) > 1 and context[-1]:
+                        # strip the last element and try again
+                        measure = console.measure(''.join(context[:-1]))
+                        length = console.width - measure.maximum
+                        if length > 0:
+                            # return self.markup((
+                            #     pattern * length + '\n' + pattern * 3,
+                            #     'yellow'
+                            # ))
+                            return self.markup(
+                                (pattern * length, 'yellow'),
+                                ('\n', ''),
+                                (pattern * 3, 'yellow dim')
+                            )
+                        else:
+                            length = 3
+                    else:
+                        # raise ValueError('invalid context', context)
+                        length = 80
+            else:
+                length = 80
+        return self.markup((pattern * length, 'yellow'))
+    
+    @staticmethod
+    def fmt_exception(e: BaseException, show_locals=False) -> Traceback:
+        trace = Traceback.from_exception(
+            type(e), e, e.__traceback__,
+            show_locals=show_locals
+        )
+        return trace
+    
+    def fmt_funcname(self, funcname: str, fmt_width=False) -> str:
+        is_func = not funcname.startswith('<')
+        if is_func:
+            funcname += '()'
+        else:
+            funcname = funcname[1:-1]
+        if fmt_width:
+            funcname = self._fmt_width(
+                funcname, min_width=8, unit_spaces=4
+            )
+        if is_func:
+            return self.markup((funcname, 'green'))
+        else:
+            return self.markup((funcname, 'magenta'))
+    
+    def fmt_index(self, idx: int) -> str:
+        return self.markup(
+            (f'[{idx}]', 'grey50' if idx == 0 else 'red')
+        )
+    
+    def fmt_level(self, level: str, text='') -> str:
+        if level == 'trace':
+            return ''
+        labels = {
+            'trace': '',
+            'debug': '[DEBUG]',
+            'info' : '[ INFO]',
+            'warn' : '[ WARN]',
+            'error': '[ERROR]',
+            'fatal': '[FATAL]',
+        }
+        colors = {
+            'trace': '',
+            'debug': 'grey50',
+            'info' : 'blue',
+            'warn' : 'yellow',
+            'error': 'red',
+            'fatal': 'bold #ffffff on red',
+        }
+        if not text: text = labels[level]
+        return self.markup((text, colors[level]))
+    
+    def fmt_message(
+            self, arguments: t.Iterable[t.Any], varnames: tuple[str],
+            rich: bool, expand=False, separator=';   '
+    ) -> str:
+        """
+        notice the process sequence:
+            1. expand
+            2. varnames
+            3. rich
+        """
+        if expand:
+            arguments = tuple(map(self._expand_object, arguments))
+        if varnames:
+            arguments = self._mix_arguments_with_varnames(arguments, varnames)
+        else:
+            arguments = map(str, arguments)
+        if not rich:
+            arguments = (x.replace('[', '\\[') for x in arguments)
+        
+        if expand:
+            return '\n' + indent('\n'.join(arguments), '    ')
+        else:
+            return self.markup((separator, 'bright_black')).join(arguments)
+    
+    def fmt_scoped_index(self, idx: int, uid: str, color: str = '') -> str:
+        # return self.markup(
+        #     ('\\[', 'magenta'),
+        #     (f'{idx}', 'magenta'),
+        #     (f'/{uid}', 'magenta dim'),
+        #     (']', 'magenta'),
+        # )
+        return self.markup(
+            (f'\\[{uid}]', f'{color} dim'),
+            (f'\\[{idx}]', f'{color}'),
+        )
+    
+    def fmt_separator(self, sep: str = ' >> ', color='bright_black') -> str:
+        return self.markup((sep, color))
+    
+    def fmt_source(
+            self, filepath: str, lineno: t.Union[int, str],
+            is_external_lib: bool = False, fmt_width=False
+    ) -> str:
         if fmt_width:
             text_a = f'{filepath}:{lineno}'
             text_b = self._fmt_width(text_a, min_width=12)
             additional_space = ' ' * (len(text_b) - len(text_a))
         else:
             additional_space = ''
         if is_external_lib:
@@ -84,37 +212,14 @@
             return self.markup(
                 (filepath.replace('[', '\\['), 'bold blue'),
                 (':', 'bright_black'),
                 (str(lineno), 'bold blue'),
                 (additional_space, ''),
             )
     
-    def fmt_separator(self, sep: str = ' >> ', color='bright_black') -> str:
-        return self.markup((sep, color))
-    
-    def fmt_funcname(self, funcname: str, fmt_width=False) -> str:
-        is_func = not funcname.startswith('<')
-        if is_func:
-            funcname += '()'
-        else:
-            funcname = funcname[1:-1]
-        if fmt_width:
-            funcname = self._fmt_width(
-                funcname, min_width=8, unit_spaces=4
-            )
-        if is_func:
-            return self.markup((funcname, 'green'))
-        else:
-            return self.markup((funcname, 'magenta'))
-    
-    def fmt_index(self, idx: int) -> str:
-        return self.markup(
-            (f'[{idx}]', 'grey50' if idx == 0 else 'red')
-        )
-    
     @staticmethod
     def fmt_time(start: float, end: float = None, color_s='green') -> str:
         if end is None:
             return '[{}]\\[{}][/]'.format(color_s, strftime(start))
         
         diff = end - start  # float >= 0
         
@@ -154,61 +259,14 @@
                 diff=diff,
                 color_s=color_s,
                 color_e=color_e,
                 color_d=color_d,
             )
         )
     
-    def fmt_divider(self, div_: str = '-' * 64) -> str:
-        return self.markup((div_, 'yellow'))
-    
-    def fmt_message(self, arguments: t.Iterable[t.Any], varnames: tuple[str],
-                    rich: bool, expand=False, separator=';   ') -> str:
-        """
-        notice the process sequence:
-            1. expand
-            2. varnames
-            3. rich
-        """
-        if expand:
-            arguments = tuple(map(self._expand_object, arguments))
-        if varnames:
-            arguments = self._mix_arguments_with_varnames(arguments, varnames)
-        else:
-            arguments = map(str, arguments)
-        if not rich:
-            arguments = (x.replace('[', '\\[') for x in arguments)
-        
-        if expand:
-            return '\n' + indent('\n'.join(arguments), '    ')
-        else:
-            return self.markup((separator, 'bright_black')).join(arguments)
-    
-    def fmt_level(self, level: str, text='') -> str:
-        if level == 'trace':
-            return ''
-        labels = {
-            'trace': '',
-            'debug': '[DEBUG]',
-            'info' : '[ INFO]',
-            'warn' : '[ WARN]',
-            'error': '[ERROR]',
-            'fatal': '[FATAL]',
-        }
-        colors = {
-            'trace': '',
-            'debug': 'grey50',
-            'info' : 'blue',
-            'warn' : 'yellow',
-            'error': 'red',
-            'fatal': 'bold #ffffff on red',
-        }
-        if not text: text = labels[level]
-        return self.markup((text, colors[level]))
-    
     # -------------------------------------------------------------------------
     
     @staticmethod
     def _expand_object(obj: t.Any) -> str:
         if isinstance(obj, Exception):
             return '\n' + indent(''.join(format_exception(obj)), '│ ')
         else:
```

## Comparing `lk_logger/sourcemap.py` & `lk_logger/frame_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,63 @@
+import inspect
 import re
-from collections import namedtuple
+import typing as t
 from types import FrameType
 
-from ._print import debug  # noqa
 from .scanner import get_all_blocks
 from .scanner import get_variables
+from .scanner.const import SUBSCRIPTABLE
+from .scanner.const import VARIABLE_NAME
+from .scanner.exceptions import ScanningError
+from .scanner.exceptions import UnresolvedCase
+
+
+class T:
+    VarNames = t.Tuple[str, ...]
+    SourceMap = t.Dict[str, t.Dict[int, VarNames]]
 
 
 class SourceMap:
+    _sourcemap: T.SourceMap
     
     def __init__(self):
         self._sourcemap = {}
-        #   dict[str filepath, dict[int lineno, tuple[str varname, ...]]]
     
-    @staticmethod
-    def get_frame_info(frame: FrameType, traceback_level: int):
-        from .path_helper import normpath
-        
-        frame_0 = frame
-        frame_x: FrameType
-        for _ in range(traceback_level):
-            frame = frame.f_back
-        frame_x = frame
-        
-        struct = namedtuple('FrameInfo', (
-            'direct_filepath', 'direct_lineno',
-            'target_filepath', 'target_lineno',
-            'target_funcname',
-        ))
-        
-        return struct(
-            normpath(frame_0.f_globals.get('__file__', '<unknown>')),
-            frame_0.f_lineno,
-            normpath(frame_x.f_globals.get('__file__', '<unknown>')),
-            frame_x.f_lineno,
-            frame_x.f_code.co_name,
-        )
+    def get_varnames(self, filepath: str, lineno: int) -> T.VarNames:
+        if filepath not in self._sourcemap:
+            self._indexing_filemap(filepath)
+        return self._sourcemap[filepath].get(lineno, ())
     
-    def get_sourcemap(self, frame: FrameType, traceback_level: int = 0,
-                      advanced=False):
-        info = self.get_frame_info(frame, traceback_level)
-        
-        struct = namedtuple('InfoStruct', (
-            'filepath', 'lineno', 'funcname', 'varnames'
-        ))
-        
-        if advanced:
-            if info.direct_filepath not in self._sourcemap:
-                self._indexing_filemap(info.direct_filepath)
-            varnames = self._sourcemap[info.direct_filepath].get(
-                info.direct_lineno, ())
-        else:
-            varnames = ()
-        
-        return struct(
-            info.target_filepath,
-            info.target_lineno,
-            info.target_funcname,
-            varnames,
-        )
-    
-    def _indexing_filemap(self, filepath: str):
-        """
-        Args:
-            filepath
-        """
+    def _indexing_filemap(self, filepath: str) -> None:
         if filepath.startswith('<'):
-            # see `FrameFinder.getinfo._fix_filepath_location`
+            # see `FrameInfo > property filepath > docstring notice`
             self._sourcemap.setdefault(filepath, {})
             return
         
-        from .scanner.const import VARIABLE_NAME
-        from .scanner.const import SUBSCRIPTABLE
-        from .scanner.exceptions import ScanningError
-        from .scanner.exceptions import UnresolvedCase
-        
-        def _get_blocks(lines):
+        def get_blocks(lines: t.Iterator[str]) -> t.Dict[int, T.VarNames]:
+            out = {}
             for match in get_all_blocks(*lines):
                 text = match.fulltext.strip()
                 if not text:
                     continue
                 if not text.startswith('print'):  # FIXME: this is not stable
                     continue
                 try:
-                    nonlocal node
                     varnames = _analyse_block(text)
                     lineno = match.cursor.lineno + 1
-                    node[lineno] = tuple(varnames)
+                    out[lineno] = tuple(varnames)
                 except ScanningError:
-                    nonlocal filepath
                     raise ScanningError(
                         match.cursor.lineno + 1, text,
                         0, '<unknown>',
                         f'<filepath: {filepath}>'
                     )
+            return out
         
-        def _analyse_block(text: str):
+        def _analyse_block(text: str) -> t.List[str]:
             varnames = []
             try:
                 for element, type_ in get_variables(text):
                     if type_ == VARIABLE_NAME:
                         varnames.append(element)
                     elif type_ == SUBSCRIPTABLE:
                         varnames.append(_analyse_subscriptables(
@@ -108,17 +66,22 @@
                     else:
                         varnames.append('')
             except UnresolvedCase:
                 varnames.clear()
             finally:
                 return varnames
         
+        _quotes_pattern_1 = re.compile(r'\'\'\'[\w\W]*\'\'\'|"""[\w\W]*"""')
+        _quotes_pattern_2 = re.compile(r'\'[^\']*\'|"[^"]*"')
+        
         def _analyse_subscriptables(
-                text: str, shorten_sub_substrings=True, threshold=20
-        ):
+                text: str,
+                shorten_sub_substrings: bool = True,
+                threshold: int = 20
+        ) -> str:
             """
             shorten_sub_strings:
                 example:
                     case 1: when captured a "varname" like "xxx('hello world')":
                         if shorten_sub_strings is True:
                             varname updated: "xxx('...')"
                         if shorten_sub_strings is False:
@@ -140,22 +103,19 @@
             
             backslash_mask = []
             for i in re.findall(r'\\.', text):
                 backslash_mask.append(i)
             if backslash_mask:
                 text = re.sub(r'\\.', '__BACKSLASK_MASK__', text)
             
-            quotes_pattern_1 = re.compile(r'\'\'\'[\w\W]*\'\'\'|"""[\w\W]*"""')
-            quotes_pattern_2 = re.compile(r'\'[^\']*\'|"[^"]*"')
-            
-            for i in set(quotes_pattern_1.findall(text)):
+            for i in set(_quotes_pattern_1.findall(text)):
                 if '\n' in i or len(i) > threshold:
                     text = text.replace(i, '"""..."""')
             
-            for i in set(quotes_pattern_2.findall(text)):
+            for i in set(_quotes_pattern_2.findall(text)):
                 if '\n' in i or len(i) > threshold:
                     text = text.replace(i, '"..."')
             
             # restore backslashes
             if backslash_mask:
                 for i in backslash_mask:
                     text = text.replace('__BACKSLASK_MASK__', i, 1)
@@ -163,17 +123,56 @@
             
             text = re.sub(r'\s+', ' ', text)
             #   note: this ^measure takes a side effect that it may replace
             #   sequential whitespaces to one whitespace inside quote strings.
             
             return text
         
-        node = self._sourcemap.setdefault(filepath, {})
-        
         with open(filepath, 'r', encoding='utf-8') as f:
-            node = self._sourcemap.setdefault(filepath, {})
-            _get_blocks((x.rstrip('\n') for x in f.readlines()))
+            self._sourcemap.setdefault(
+                filepath, get_blocks((x.rstrip('\n') for x in f.readlines()))
+            )
 
 
 sourcemap = SourceMap()
 
-__all__ = ['sourcemap']
+
+class FrameInfo:
+    
+    def __init__(self, frame: FrameType):
+        self._frame = frame
+    
+    @property
+    def id(self) -> str:
+        return f'{self.filepath}:{self.lineno}'
+    
+    @property
+    def filepath(self) -> str:
+        """
+        notice: the returned value may be '<string>', '<unknown>' etc.
+        """
+        return self._frame.f_globals.get(
+            '__file__', self._frame.f_code.co_filename
+        )
+    
+    @property
+    def lineno(self) -> int:
+        return self._frame.f_lineno
+    
+    @property
+    def indentation(self) -> int:
+        # https://stackoverflow.com/a/39172552
+        ctx = inspect.getframeinfo(self._frame).code_context[0]
+        return len(ctx) - len(ctx.lstrip())
+    
+    @property
+    def funcname(self) -> str:
+        return self._frame.f_code.co_name
+    
+    def collect_varnames(self) -> T.VarNames:
+        return sourcemap.get_varnames(self.filepath, self.lineno)
+    
+    def get_parent(self, traceback_level: int = 1) -> 'FrameInfo':
+        frame = self._frame
+        for _ in range(traceback_level):
+            frame = frame.f_back
+        return FrameInfo(frame)
```

## Comparing `lk_logger-5.4.9.dist-info/METADATA` & `lk_logger-5.5.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: lk-logger
-Version: 5.4.9
+Version: 5.5.0
 Summary: Python advanced print with varnames.
 Home-page: https://github.com/likianta/lk-logger
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: rich (>=12.6,<14.0)
+Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # LK Logger
 
 [中文版](https://blog.csdn.net/Likianta/article/details/124358443)
 
 An alternative to Python built-in `print` function.
```

