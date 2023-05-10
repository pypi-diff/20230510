# Comparing `tmp/commonX-0.4.4.tar.gz` & `tmp/commonX-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.4.4.tar", last modified: Wed May 10 07:04:10 2023, max compression
+gzip compressed data, was "dist\commonX-0.4.5.tar", last modified: Wed May 10 10:30:54 2023, max compression
```

## Comparing `commonX-0.4.4.tar` & `commonX-0.4.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/
--rw-rw-rw-   0        0        0      714 2023-05-10 07:04:10.000000 commonX-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-05-10 07:01:45.000000 commonX-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/
--rw-rw-rw-   0        0        0       86 2023-05-10 07:01:45.000000 commonX-0.4.4/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/base/
--rw-rw-rw-   0        0        0      622 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/mapper.py
--rw-rw-rw-   0        0        0     8399 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5182 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-05-10 07:01:45.000000 commonX-0.4.4/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/ext/
--rw-rw-rw-   0        0        0      187 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-05-10 07:01:45.000000 commonX-0.4.4/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/postman/
--rw-rw-rw-   0        0        0       87 2023-05-10 07:01:45.000000 commonX-0.4.4/common/postman/__init__.py
--rw-rw-rw-   0        0        0     5086 2023-05-10 07:01:45.000000 commonX-0.4.4/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     4839 2023-05-10 07:01:45.000000 commonX-0.4.4/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     4528 2023-05-10 07:01:45.000000 commonX-0.4.4/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/common/util/
--rw-rw-rw-   0        0        0      277 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/assert_util.py
--rw-rw-rw-   0        0        0     3273 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     2725 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/exception_utll.py
--rw-rw-rw-   0        0        0     7244 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/file_util.py
--rw-rw-rw-   0        0        0     2921 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/json_util.py
--rw-rw-rw-   0        0        0     6928 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4616 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-05-10 07:01:45.000000 commonX-0.4.4/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/
--rw-rw-rw-   0        0        0      714 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-10 07:04:10.000000 commonX-0.4.4/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 07:04:10.000000 commonX-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-05-10 07:01:45.000000 commonX-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/
+-rw-rw-rw-   0        0        0      714 2023-05-10 10:30:54.000000 commonX-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-05-10 10:30:27.000000 commonX-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/
+-rw-rw-rw-   0        0        0       86 2023-05-10 10:30:27.000000 commonX-0.4.5/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/base/
+-rw-rw-rw-   0        0        0      622 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/entity.py
+-rw-rw-rw-   0        0        0      359 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/factory.py
+-rw-rw-rw-   0        0        0     2927 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/genor.py
+-rw-rw-rw-   0        0        0     2916 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/hook.py
+-rw-rw-rw-   0        0        0     4135 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/logger.py
+-rw-rw-rw-   0        0        0     5710 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/mapper.py
+-rw-rw-rw-   0        0        0     8399 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/multi_task.py
+-rw-rw-rw-   0        0        0     5194 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/packer.py
+-rw-rw-rw-   0        0        0     1968 2023-05-10 10:30:27.000000 commonX-0.4.5/common/base/registry.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/ext/
+-rw-rw-rw-   0        0        0      187 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/cookie_parser.py
+-rw-rw-rw-   0        0        0     3845 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/iphone_client.py
+-rw-rw-rw-   0        0        0      220 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/ocr_support.py
+-rw-rw-rw-   0        0        0     1862 2023-05-10 10:30:27.000000 commonX-0.4.5/common/ext/qq_email.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/postman/
+-rw-rw-rw-   0        0        0       87 2023-05-10 10:30:27.000000 commonX-0.4.5/common/postman/__init__.py
+-rw-rw-rw-   0        0        0     5086 2023-05-10 10:30:27.000000 commonX-0.4.5/common/postman/postman_api.py
+-rw-rw-rw-   0        0        0     4457 2023-05-10 10:30:27.000000 commonX-0.4.5/common/postman/postman_impl.py
+-rw-rw-rw-   0        0        0     4528 2023-05-10 10:30:27.000000 commonX-0.4.5/common/postman/postman_proxy.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/common/util/
+-rw-rw-rw-   0        0        0      277 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/args_util.py
+-rw-rw-rw-   0        0        0     2176 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/assert_util.py
+-rw-rw-rw-   0        0        0     3273 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/decorator_util.py
+-rw-rw-rw-   0        0        0     2725 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/exception_utll.py
+-rw-rw-rw-   0        0        0     7244 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/file_util.py
+-rw-rw-rw-   0        0        0     2921 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/json_util.py
+-rw-rw-rw-   0        0        0     6928 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/requests_util.py
+-rw-rw-rw-   0        0        0     4616 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/sys_util.py
+-rw-rw-rw-   0        0        0      898 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/time_util.py
+-rw-rw-rw-   0        0        0      715 2023-05-10 10:30:27.000000 commonX-0.4.5/common/util/typing_util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 10:30:54.000000 commonX-0.4.5/commonX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 10:30:54.000000 commonX-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2023-05-10 10:30:27.000000 commonX-0.4.5/setup.py
```

### Comparing `commonX-0.4.4/PKG-INFO` & `commonX-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.4
+Version: 0.4.5
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.4/common/base/__init__.py` & `commonX-0.4.5/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/base/entity.py` & `commonX-0.4.5/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/base/genor.py` & `commonX-0.4.5/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/base/hook.py` & `commonX-0.4.5/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/base/logger.py` & `commonX-0.4.5/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/base/mapper.py` & `commonX-0.4.5/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/base/multi_task.py` & `commonX-0.4.5/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/base/packer.py` & `commonX-0.4.5/common/base/packer.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,20 @@
              ensure_ascii=False,
              indent=indent,
              )
 
     def load(self, fp, clazz) -> Any:
         from json import load
         dic: dict = load(fp)
-        config = clazz(**dic)
-        for k, v in dic.items():
-            config.__setattr__(k, v)
-        return config
+        if clazz is None:
+            return dic
+
+        obj: object = clazz()
+        obj.__dict__.update(dic)
+        return obj
 
     @classmethod
     def to_dict(cls, obj):
         """将对象转换为字典"""
         if hasattr(obj, "__dict__"):
             d = dict(obj.__dict__)
             for key, value in d.items():
```

### Comparing `commonX-0.4.4/common/base/registry.py` & `commonX-0.4.5/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/ext/cookie_parser.py` & `commonX-0.4.5/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/ext/iphone_client.py` & `commonX-0.4.5/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/ext/qq_email.py` & `commonX-0.4.5/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/postman/postman_api.py` & `commonX-0.4.5/common/postman/postman_api.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/postman/postman_impl.py` & `commonX-0.4.5/common/postman/postman_impl.py`

 * *Files 24% similar despite different names*

```diff
@@ -90,34 +90,29 @@
     Type[RequestsSessionPostman],
     Type[TslClientSessionPostman],
 ]
 
 
 class Postmans:
     postman_impl_class_dict: Dict[str, PostmanImplClazz] = {
-        # 使用 requests，最基础的请求方式
         'requests': RequestsPostman,
-        # 使用 requests.Session，自动维护 cookies
         'requests_Session': RequestsSessionPostman,
-        # 使用以下支持伪装【tls指纹】的库，更加安全稳如苟
         'cffi': CffiPostman,
         'cffi_Session': CffiSessionPostman,
-        # 注意: tls_client 不支持 response.content 和 cookies维护
-        # 'tls_client': TslClientSessionPostman,
     }
 
     @classmethod
     def get_impl_clazz(cls, key='requests') -> PostmanImplClazz:
         return cls.postman_impl_class_dict[key]
 
     @classmethod
-    def build_from_config_file(cls,
-                               filepath='./postman.yml',
-                               data=None,
-                               ) -> Postman:
+    def create(cls,
+               filepath='./postman.yml',
+               data=None,
+               ) -> Postman:
         if data is None:
             from common import PackerUtil
             data = PackerUtil.unpack(filepath)[0]
             if data is None:
                 raise AssertionError(f'空配置文件: {filepath}')
 
         return cls.PostmanDslBuilder().build_postman(data)
```

### Comparing `commonX-0.4.4/common/postman/postman_proxy.py` & `commonX-0.4.5/common/postman/postman_proxy.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/args_util.py` & `commonX-0.4.5/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/assert_util.py` & `commonX-0.4.5/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/decorator_util.py` & `commonX-0.4.5/common/util/decorator_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/exception_utll.py` & `commonX-0.4.5/common/util/exception_utll.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/file_util.py` & `commonX-0.4.5/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/json_util.py` & `commonX-0.4.5/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/requests_util.py` & `commonX-0.4.5/common/util/requests_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/sys_util.py` & `commonX-0.4.5/common/util/sys_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/time_util.py` & `commonX-0.4.5/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/common/util/typing_util.py` & `commonX-0.4.5/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/commonX.egg-info/PKG-INFO` & `commonX-0.4.5/commonX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.4
+Version: 0.4.5
 Summary: python common toolkit
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `commonX-0.4.4/commonX.egg-info/SOURCES.txt` & `commonX-0.4.5/commonX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonX-0.4.4/setup.py` & `commonX-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.4.4'
+VERSION = '0.4.5'
 DESCRIPTION = 'python common toolkit'
 
 setup(
     name='commonX',
     version=VERSION,
     description=DESCRIPTION,
     author='hect0x7',
```

