# Comparing `tmp/commonX-0.4.3.tar.gz` & `tmp/commonX-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.4.3.tar", last modified: Mon May  1 08:00:05 2023, max compression
+gzip compressed data, was "dist\commonX-0.4.4.tar", last modified: Wed May 10 07:04:10 2023, max compression
```

## Comparing `commonX-0.4.3.tar` & `commonX-0.4.4.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 08:00:05.000000 commonX-0.4.3/
--rw-rw-rw-   0        0        0      714 2023-05-01 08:00:05.000000 commonX-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-05-01 07:59:31.000000 commonX-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/
--rw-rw-rw-   0        0        0       86 2023-05-01 07:59:31.000000 commonX-0.4.3/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/base/
--rw-rw-rw-   0        0        0      622 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/mapper.py
--rw-rw-rw-   0        0        0     8399 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5182 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-05-01 07:59:30.000000 commonX-0.4.3/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/ext/
--rw-rw-rw-   0        0        0      187 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-05-01 07:59:30.000000 commonX-0.4.3/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/postman/
--rw-rw-rw-   0        0        0       87 2023-05-01 07:59:30.000000 commonX-0.4.3/common/postman/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-05-01 07:59:30.000000 commonX-0.4.3/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     4903 2023-05-01 07:59:30.000000 commonX-0.4.3/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     4418 2023-05-01 07:59:30.000000 commonX-0.4.3/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/common/util/
--rw-rw-rw-   0        0        0      246 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/assert_util.py
--rw-rw-rw-   0        0        0     3273 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     7244 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/file_util.py
--rw-rw-rw-   0        0        0     2921 2023-05-01 07:59:30.000000 commonX-0.4.3/common/util/json_util.py
--rw-rw-rw-   0        0        0     6928 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4616 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-05-01 07:59:31.000000 commonX-0.4.3/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/
--rw-rw-rw-   0        0        0      714 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-01 08:00:04.000000 commonX-0.4.3/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 08:00:05.000000 commonX-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-05-01 07:59:55.000000 commonX-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/
+-rw-rw-rw-   0        0        0      714 2023-05-10 07:04:10.000000 commonX-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-05-10 07:01:45.000000 commonX-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/
+-rw-rw-rw-   0        0        0       86 2023-05-10 07:01:45.000000 commonX-0.4.4/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/base/
+-rw-rw-rw-   0        0        0      622 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/entity.py
+-rw-rw-rw-   0        0        0      359 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/factory.py
+-rw-rw-rw-   0        0        0     2927 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/genor.py
+-rw-rw-rw-   0        0        0     2916 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/hook.py
+-rw-rw-rw-   0        0        0     4135 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/logger.py
+-rw-rw-rw-   0        0        0     5710 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/mapper.py
+-rw-rw-rw-   0        0        0     8399 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/multi_task.py
+-rw-rw-rw-   0        0        0     5182 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/packer.py
+-rw-rw-rw-   0        0        0     1968 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/registry.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/ext/
+-rw-rw-rw-   0        0        0      187 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/cookie_parser.py
+-rw-rw-rw-   0        0        0     3845 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/iphone_client.py
+-rw-rw-rw-   0        0        0      220 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/ocr_support.py
+-rw-rw-rw-   0        0        0     1862 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/qq_email.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/postman/
+-rw-rw-rw-   0        0        0       87 2023-05-10 07:01:45.000000 commonX-0.4.4/common/postman/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-05-10 07:01:45.000000 commonX-0.4.4/common/postman/postman_api.py
+-rw-rw-rw-   0        0        0     4839 2023-05-10 07:01:45.000000 commonX-0.4.4/common/postman/postman_impl.py
+-rw-rw-rw-   0        0        0     4528 2023-05-10 07:01:45.000000 commonX-0.4.4/common/postman/postman_proxy.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/util/
+-rw-rw-rw-   0        0        0      277 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/args_util.py
+-rw-rw-rw-   0        0        0     2176 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/assert_util.py
+-rw-rw-rw-   0        0        0     3273 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/decorator_util.py
+-rw-rw-rw-   0        0        0     2725 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/exception_utll.py
+-rw-rw-rw-   0        0        0     7244 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/file_util.py
+-rw-rw-rw-   0        0        0     2921 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/json_util.py
+-rw-rw-rw-   0        0        0     6928 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/requests_util.py
+-rw-rw-rw-   0        0        0     4616 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/sys_util.py
+-rw-rw-rw-   0        0        0      898 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/time_util.py
+-rw-rw-rw-   0        0        0      715 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/typing_util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 07:04:10.000000 commonX-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-05-10 07:01:45.000000 commonX-0.4.4/setup.py
```

### Comparing `commonX-0.4.3/PKG-INFO` & `commonX-0.4.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.3
+Version: 0.4.4
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.3/common/base/__init__.py` & `commonX-0.4.4/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/base/entity.py` & `commonX-0.4.4/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/base/genor.py` & `commonX-0.4.4/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/base/hook.py` & `commonX-0.4.4/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/base/logger.py` & `commonX-0.4.4/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/base/mapper.py` & `commonX-0.4.4/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/base/multi_task.py` & `commonX-0.4.4/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/base/packer.py` & `commonX-0.4.4/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/base/registry.py` & `commonX-0.4.4/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/ext/cookie_parser.py` & `commonX-0.4.4/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/ext/iphone_client.py` & `commonX-0.4.4/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/ext/qq_email.py` & `commonX-0.4.4/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/postman/postman_api.py` & `commonX-0.4.4/common/postman/postman_api.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/postman/postman_impl.py` & `commonX-0.4.4/common/postman/postman_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,26 +65,25 @@
 
     def __post__(self):
         from curl_cffi import requests
         return requests.post
 
 
 class CffiSessionPostman(AbstractSessionPostman):
-    from curl_cffi import requests
-    Session = requests.Session
-    CffiResp = requests.Response
 
     def __init__(self, kwargs: dict) -> None:
         super().__init__(kwargs)
 
     def create_session(self, kwargs):
         return self.new_cffi_session(kwargs)
 
+    # noinspection PyMethodMayBeStatic
     def new_cffi_session(self, kwargs: dict):
-        return self.Session(**kwargs)
+        from curl_cffi import requests
+        return requests.Session(**kwargs)
 
 
 # help typing
 PostmanImplClazz = Union[
     Type[CffiPostman],
     Type[CffiSessionPostman],
     Type[RequestsPostman],
@@ -117,18 +116,18 @@
                                ) -> Postman:
         if data is None:
             from common import PackerUtil
             data = PackerUtil.unpack(filepath)[0]
             if data is None:
                 raise AssertionError(f'空配置文件: {filepath}')
 
-        return cls.PostmanDslHandler().build_postman(data)
+        return cls.PostmanDslBuilder().build_postman(data)
 
     # noinspection PyMethodMayBeStatic
-    class PostmanDslHandler:
+    class PostmanDslBuilder:
 
         def __init__(self) -> None:
             self.dsl_handler_list: list[Callable[[Dict], Union[Postman, None]]] = [
                 self.proxy_handler,
                 self.impltype_handler,
             ]
 
@@ -151,8 +150,8 @@
 
         def build_postman(self, data):
             for handler in self.dsl_handler_list:
                 postman = handler(data)
                 if postman is not None:
                     return postman
 
-            raise NotImplementedError('no available handler to build your postman')
+            raise NotImplementedError
```

### Comparing `commonX-0.4.3/common/postman/postman_proxy.py` & `commonX-0.4.4/common/postman/postman_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,19 @@
                  postman: Postman,
                  retry_times: int,
                  ):
         super().__init__(postman)
         self.retry_times = retry_times
 
     def retry_request(self, request, url, **kwargs):
-        for i in range(self.retry_times):
+        retry_times = self.retry_times
+        if retry_times <= 0:
+            return request(url, **kwargs)
+
+        for i in range(retry_times):
             try:
                 return request(url, **kwargs)
             except KeyboardInterrupt as e:
                 raise e
             except Exception as e:
                 self.excp_handle(e)
                 self.tip_retrying(i, request, url, kwargs)
```

### Comparing `commonX-0.4.3/common/util/args_util.py` & `commonX-0.4.4/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/util/assert_util.py` & `commonX-0.4.4/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/util/decorator_util.py` & `commonX-0.4.4/common/util/decorator_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/util/file_util.py` & `commonX-0.4.4/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/util/json_util.py` & `commonX-0.4.4/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/util/requests_util.py` & `commonX-0.4.4/common/util/requests_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/util/sys_util.py` & `commonX-0.4.4/common/util/sys_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/util/time_util.py` & `commonX-0.4.4/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/common/util/typing_util.py` & `commonX-0.4.4/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.3/commonX.egg-info/PKG-INFO` & `commonX-0.4.4/commonX.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.3
+Version: 0.4.4
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.3/commonX.egg-info/SOURCES.txt` & `commonX-0.4.4/commonX.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,13 +24,14 @@
 common/postman/postman_api.py
 common/postman/postman_impl.py
 common/postman/postman_proxy.py
 common/util/__init__.py
 common/util/args_util.py
 common/util/assert_util.py
 common/util/decorator_util.py
+common/util/exception_utll.py
 common/util/file_util.py
 common/util/json_util.py
 common/util/requests_util.py
 common/util/sys_util.py
 common/util/time_util.py
 common/util/typing_util.py
```

### Comparing `commonX-0.4.3/setup.py` & `commonX-0.4.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.4.3'
+VERSION = '0.4.4'
 DESCRIPTION = 'python common toolkit'
 
 setup(
     name='commonX',
     version=VERSION,
     description=DESCRIPTION,
     author='hect0x7',
```

