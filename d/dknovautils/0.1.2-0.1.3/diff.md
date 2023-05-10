# Comparing `tmp/dknovautils-0.1.2.tar.gz` & `tmp/dknovautils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dknovautils-0.1.2.tar", last modified: Thu May  4 06:39:31 2023, max compression
+gzip compressed data, was "dist/dknovautils-0.1.3.tar", last modified: Wed May 10 06:54:53 2023, max compression
```

## Comparing `dknovautils-0.1.2.tar` & `dknovautils-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-04 06:39:31.000000 dknovautils-0.1.2/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-04 06:39:31.000000 dknovautils-0.1.2/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2903 2023-05-02 15:06:54.000000 dknovautils-0.1.2/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     7953 2023-05-04 06:39:30.000000 dknovautils-0.1.2/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      103 2023-05-04 04:54:01.000000 dknovautils-0.1.2/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1149 2023-04-22 02:58:52.000000 dknovautils-0.1.2/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-04 06:39:30.000000 dknovautils-0.1.2/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      490 2023-04-13 12:40:48.000000 dknovautils-0.1.2/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.2/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.2/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.2/dknovautils/__init__.py
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-04 06:39:31.000000 dknovautils-0.1.2/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-04 06:39:30.000000 dknovautils-0.1.2/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-04 06:39:30.000000 dknovautils-0.1.2/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-04 06:39:30.000000 dknovautils-0.1.2/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-04 06:39:30.000000 dknovautils-0.1.2/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-04 06:39:30.000000 dknovautils-0.1.2/dknovautils.egg-info/top_level.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.2/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-04 06:39:31.000000 dknovautils-0.1.2/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.2/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-04 06:39:31.000000 dknovautils-0.1.2/setup.cfg
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1157 2023-05-04 06:39:30.000000 dknovautils-0.1.2/setup.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-10 06:54:53.000000 dknovautils-0.1.3/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-10 06:54:53.000000 dknovautils-0.1.3/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2448 2023-05-10 03:57:08.000000 dknovautils-0.1.3/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     8644 2023-05-10 06:54:49.000000 dknovautils-0.1.3/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      103 2023-05-04 04:54:01.000000 dknovautils-0.1.3/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1153 2023-05-07 16:31:40.000000 dknovautils-0.1.3/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      711 2023-05-10 06:54:49.000000 dknovautils-0.1.3/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      501 2023-05-07 13:41:47.000000 dknovautils-0.1.3/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      140 2023-04-13 15:12:06.000000 dknovautils-0.1.3/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      160 2023-04-13 15:11:54.000000 dknovautils-0.1.3/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      307 2023-04-21 15:52:41.000000 dknovautils-0.1.3/dknovautils/__init__.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2023-05-10 06:54:53.000000 dknovautils-0.1.3/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2023-05-10 06:54:51.000000 dknovautils-0.1.3/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-10 06:54:51.000000 dknovautils-0.1.3/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-10 06:54:51.000000 dknovautils-0.1.3/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      407 2023-05-10 06:54:52.000000 dknovautils-0.1.3/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2023-05-10 06:54:51.000000 dknovautils-0.1.3/dknovautils.egg-info/top_level.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      105 2023-03-09 04:32:08.000000 dknovautils-0.1.3/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      880 2023-05-10 06:54:53.000000 dknovautils-0.1.3/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      472 2023-03-09 06:46:27.000000 dknovautils-0.1.3/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2023-05-10 06:54:53.000000 dknovautils-0.1.3/setup.cfg
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1157 2023-05-10 06:54:49.000000 dknovautils-0.1.3/setup.py
```

### Comparing `dknovautils-0.1.2/dknovautils/commons.py` & `dknovautils-0.1.3/dknovautils/commons.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 from dknovautils.dkat import *
 
 from dknovautils.dkipy import *
 
 
 def write_async():
+    AT.unimplemented()
     pass
 
 
 def dtprint(s: str):
-    print(s)
+    iprint(s)
 
 
 def iprint(obj):
     iprint_debug(obj)
 
 
 def iprint_trace(obj):
@@ -47,57 +48,41 @@
 
     if AT._innerLoggerFun_ is not None:
         AT._innerLoggerFun_(obj, level)
         return
     else:
         pass
 
-    # now = datetime.now()
-    # dts = now.strftime("%d/%m/%Y %H:%M:%S")
-    # otstr = now.isoformat()[:(10 + 1 + 8+4)]
-
-    # _FORMAT_111 = '%(asctime)s %(message)s'
-    # logging.basicConfig(format=_FORMAT)
-
     global _log_inited
     if not _log_inited:
         _log_inited = True
 
         # 只在没有配置的时候起作用 不会重复执行
         logging.basicConfig(level=logging.NOTSET,
-                            # datefmt=AT._default_time_format,
                             datefmt=AT.STRFMT_ISO_SEC_A,
-                            format=AT._LOG_FORMAT_106)
-        
+                            format=AT._LOG_FORMAT_106,
+                            )
+
         '''
         
     formatter = logging.Formatter('%(asctime)s.%(msecs)03d-%(name)s-%(filename)s-[line:%(lineno)d]'
                                   '-%(levelname)s-[日志信息]: %(message)s',
                                   datefmt='%Y-%m-%d,%H:%M:%S')
   
         
         '''
 
-    # 采用这个将级别提升一下。不知为何 NotSET的设置没有生效 并不会打印。
+    # 将Trace级别提升一下。不知为何 NotSET的设置没有生效 并不会打印。
     if level == LLevel.Trace:
         level = LLevel.Debug
 
     logging.log(level.value, obj)
 
     return
 
-    if False:
-
-        otstr2 = datetime.fromtimestamp(time.time()).strftime(
-            "%Y-%m-%dT%H:%M:%S.%f")[0:23]
-
-        msg = f'[{otstr}]{obj}'
-
-    print(f"[{otstr}][{level.name.lower()}]{obj}")
-
 # _myCntInfos = {}
 
 
 '''
 
 https://docs.python.org/3/howto/logging.html
```

### Comparing `dknovautils-0.1.2/dknovautils/dkat.py` & `dknovautils-0.1.3/dknovautils/dkat.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 
 import dknovautils
 from dknovautils.commons import *
 
 import beepy
 
 
-DkAppVer = '0.1.2'
+DkAppVer = '0.1.3'
+
 _unknown_err = '_unknown_err4035'
 
 
 class AT(object):
 
     _innerLoggerFun_ = None
 
     _AstErrorCnt_ = 0
 
     __logger = None
 
     @classmethod
-    def log(cls, loggerName='dkn'):
+    def logger(cls, loggerName='dkn'):
         if cls.__logger is None:
             logger = logging.getLogger(loggerName)
             cls.__logger = logger
 
         return cls.__logger
 
     @staticmethod
     def log_loggerFun(loggerName='dkn', initInnerLoggerFun=True, beepError=True, beepWarn=False):
+        '''
+        创建一个logger 作为系统的缺省logger
+        '''
 
-        logger = logging.getLogger(loggerName)
+        _logger = logging.getLogger(loggerName)
 
         def mloggerFun(obj, llevel):
             assert isinstance(llevel, LLevel)
             if False:
                 pass
             elif llevel == LLevel.Trace:
                 # 也用debug级别。只是在prod模式下可以关闭。
-                logger.debug(obj)
+                _logger.debug(obj)
             elif llevel == LLevel.Debug:
-                logger.debug(obj)
+                _logger.debug(obj)
             elif llevel == LLevel.Info:
-                logger.info(obj)
+                _logger.info(obj)
             elif llevel == LLevel.Warn:
-                logger.warning(obj)
+                _logger.warning(obj)
                 if beepWarn:
                     AT.beep_error_buffered()
             elif llevel == LLevel.Error:
-                logger.error(obj)
+                _logger.error(obj)
                 if beepError:
                     AT.beep_error_buffered()
             else:
                 assert False, f"bad {llevel}"
 
             pass
 
@@ -78,37 +82,45 @@
     
     dtstr = datetime.now().strftime("%Y%m%dT%H%M%S")
 
         
     '''
 
     @classmethod
-    def log_basicConfig(cls, filename='tmp_test.log', loggerName='dkn', initInnerLoggerFun=True):
+    def log_basicConfig(cls, filename='tmp_test.log', loggerName='dkn', level=logging.DEBUG, initInnerLoggerFun=True):
+        '''
+        这个 dkn logger的设置好像不太好。
+        暂时不用这个
 
-        logging.basicConfig(filename=filename, level=logging.NOTSET,
+        '''
+
+        # AT.unsupported()
+
+        logging.basicConfig(filename=filename, level=level,
                             format=cls._LOG_FORMAT_106,
+                            datefmt=AT.STRFMT_ISO_SEC_A,
                             # datefmt=cls._DATE_FORMAT_100,
                             force=True)
 
         logger = logging.getLogger(loggerName)
-        logger.setLevel(logging.DEBUG)
+        logger.setLevel(level)
 
-        # create console handler and set level to debug
-        ch = logging.StreamHandler()
-        ch.setLevel(logging.DEBUG)
+        # # create console handler and set level to debug
+        # ch = logging.StreamHandler()
+        # ch.setLevel(logging.DEBUG)
 
-        # create formatter
-        formatter = logging.Formatter(
-            cls._LOG_FORMAT_106)
+        # # create formatter
+        # formatter = logging.Formatter(
+        #     cls._LOG_FORMAT_106)
 
-        # add formatter to ch
-        ch.setFormatter(formatter)
+        # # add formatter to ch
+        # ch.setFormatter(formatter)
 
-        # add ch to logger
-        logger.addHandler(ch)
+        # # add ch to logger
+        # logger.addHandler(ch)
 
         mloggerFun = AT.log_loggerFun(loggerName, initInnerLoggerFun)
 
         return mloggerFun
 
     @staticmethod
     def assertAllNotNone(*args):
@@ -141,16 +153,20 @@
         beepy.beep(sound=tone)
 
     @staticmethod
     def beep2():
         #!wget -q -T 1 http://localhost:333/hello
         print('\7')
 
+    @staticmethod
+    def vassert_(b: bool, s: str = None):
+        AT.assert_(b, s)        
+
     @classmethod
-    def never(cls,s=None):
+    def never(cls, s=None):
         AT.assert_(False,  s if s is not None else 'should never come here')
 
     @staticmethod
     def checksys():
         assert sys.version_info >= (3, 11)
 
     @classmethod
@@ -160,17 +176,17 @@
 
     _last_epochsecs = 0.0
 
     @classmethod
     def fepochSecs(cls) -> float:
         '''
          time.monotonic()不是epoch值。fuck
+        # return time.monotonic()
 
         '''
-        # return time.monotonic()
         r = time.time()
         if r <= cls._last_epochsecs:
             return cls._last_epochsecs
         else:
             cls._last_epochsecs = r
             return r
 
@@ -183,15 +199,15 @@
     dts = datetime.now().strftime("%Y%m%dT%H%M%S")
     print("date and time =", dts)
     
     
     '''
 
     @classmethod
-    def sdf_isocompact_format_datetime(cls,dt=None, *, precise: str = 's'):
+    def sdf_isocompact_format_datetime(cls, dt=None, *, precise: str = 's'):
         assert precise in ['d', 's', 'ms', 'a'], 'err5554 bad precise'
 
         if dt is not None:
             AT.unsupported()
 
         dt = AT._now_dt()
         dts = dt.strftime(AT.STRFMT_ISO_COMPACT_ALL_A)
@@ -207,23 +223,24 @@
         else:
             AT.never()
 
         return dts
 
     @staticmethod
     def sdf_logger():
+        AT.unimplemented()
         pass
 
     @staticmethod
     def _now_dt():
         dt = datetime.now()
         return dt
 
     @classmethod
-    def sdf_logger_format_datetime(cls,dt: int = None, *, precise: str = 's') -> str:
+    def sdf_logger_format_datetime(cls, dt: int = None, *, precise: str = 's') -> str:
         '''
 https://strftime.org/    
 https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes
 https://man7.org/linux/man-pages/man3/strftime.3.html
 
 2023-12-01T08:30:00.123456
 
@@ -277,31 +294,37 @@
 
     @staticmethod
     def mychdir(s):
         assert isinstance(s, str) and len(s) > 0
         iprint_debug(f'chdir: {s}')
         os.chdir(s)
 
-    # @staticmethod
-    # def never(s=None):
-    #     AT.assert_(False, f"should never come here {s}")
-
     @staticmethod
     def astTrace(b: bool, s: str):
         '''在prod中完全不需要的'''
         AT.assert_(b, s)
 
     @staticmethod
     def unsupported(s: str = 'feature'):
         AT.assert_(False, f'err8255 unsupported [{s}]')
 
     @staticmethod
     def unimplemented(s: str = 'feature'):
         AT.assert_(False, f'err4173 unimplemented [{s}]')
 
+    # @staticmethod
+    # def f_matploglib_logger():
+    #     logger = logging.getLogger('matplotlib.font_manager')
+    #     logger.setLevel(level=logging.INFO)
+
+    @staticmethod
+    def log_conf_matploglib_logger(level=logging.INFO):
+        logger = logging.getLogger('matplotlib.font_manager')
+        logger.setLevel(level=level)        
+
     VERSION = DkAppVer
 
 
 class DkAstException(Exception):
     pass
```

### Comparing `dknovautils-0.1.2/dknovautils/dkipy.py` & `dknovautils-0.1.3/dknovautils/dkipy.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,44 +5,45 @@
 
 
 from IPython.core.getipython import get_ipython
 
 
 class DkIpyUtils(object):
 
-    # class attribute
-
     @staticmethod
     def hello(a):
         commons.iprint_info("hello")
         return a  # 为了测试该文件是否正常
 
     @staticmethod
     def mfc(cmd: str, logcmd: bool = True):
         DkIpyUtils.mfr(cmd, logcmd)
-        # assert isinstance(cmd, str) and len(cmd) > 0, 'err3581'
-        # get_ipython().getoutput(cmd)
-        # # AT.unimplemented()
+
+    _cmd_id = 1000
 
     @staticmethod
     def mfr(cmd, logcmd=True) -> any:
         assert isinstance(cmd, str) and len(cmd) > 0, 'err3581'
+        DkIpyUtils._cmd_id += 1
         if logcmd:
-            commons.iprint_info(f'begin run cmd: {cmd}')
+            commons.iprint_info(f'run cmd begin {DkIpyUtils._cmd_id}: {cmd}')
 
         r = get_ipython().getoutput(cmd)
+
+        if logcmd:
+            commons.iprint_info(f'run cmd end {DkIpyUtils._cmd_id}')
+
         return r
 
 
 def dk_mfc(cmd, logcmd): DkIpyUtils.mfc(cmd, logcmd)
 
 
 def dk_mfr(cmd, logcmd): return DkIpyUtils.mfr(cmd, logcmd)
 
-
 '''
 
 !{cmd}
 
 r=get_ipython().getoutput('{cmd}')
```

### Comparing `dknovautils-0.1.2/dknovautils/dk_imports.py` & `dknovautils-0.1.3/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.1.2/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.1.3/dknovautils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.1.2/PKG-INFO` & `dknovautils-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is the tools for dknova.
 Home-page: http://example.com
 Author: dknova
 Author-email: dknova@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dknovautils-0.1.2/setup.py` & `dknovautils-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import setuptools
 
 from distutils.core import setup
 from setuptools import find_packages
 
-DkAppVer = '0.1.2'
+DkAppVer = '0.1.3'
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="dknovautils",
     version=DkAppVer,
```

