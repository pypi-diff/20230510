# Comparing `tmp/fastapi_dddocr-0.0.1.tar.gz` & `tmp/fastapi_dddocr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_dddocr-0.0.1.tar", last modified: Wed May 10 02:11:28 2023, max compression
+gzip compressed data, was "fastapi_dddocr-0.0.2.tar", last modified: Wed May 10 02:21:08 2023, max compression
```

## Comparing `fastapi_dddocr-0.0.1.tar` & `fastapi_dddocr-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 02:11:28.880365 fastapi_dddocr-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-06 06:29:33.000000 fastapi_dddocr-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      479 2023-05-10 02:11:28.880365 fastapi_dddocr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-05-10 02:09:37.000000 fastapi_dddocr-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 02:11:28.864741 fastapi_dddocr-0.0.1/fastapi_dddocr/
--rw-rw-rw-   0        0        0        0 2023-05-06 06:24:35.000000 fastapi_dddocr-0.0.1/fastapi_dddocr/__init__.py
--rw-rw-rw-   0        0        0     2726 2023-05-10 01:59:13.000000 fastapi_dddocr-0.0.1/fastapi_dddocr/fastapi_dama_docr.py
-drwxrwxrwx   0        0        0        0 2023-05-10 02:11:28.864741 fastapi_dddocr-0.0.1/fastapi_dddocr.egg-info/
--rw-rw-rw-   0        0        0      479 2023-05-10 02:11:28.000000 fastapi_dddocr-0.0.1/fastapi_dddocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-10 02:11:28.000000 fastapi_dddocr-0.0.1/fastapi_dddocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 02:11:28.000000 fastapi_dddocr-0.0.1/fastapi_dddocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 02:11:28.000000 fastapi_dddocr-0.0.1/fastapi_dddocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 02:11:28.880365 fastapi_dddocr-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1148 2023-05-10 02:09:46.000000 fastapi_dddocr-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:21:08.986063 fastapi_dddocr-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-06 06:29:33.000000 fastapi_dddocr-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      479 2023-05-10 02:21:08.986063 fastapi_dddocr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-05-10 02:09:37.000000 fastapi_dddocr-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 02:21:08.971067 fastapi_dddocr-0.0.2/fastapi_dddocr/
+-rw-rw-rw-   0        0        0        0 2023-05-06 06:24:35.000000 fastapi_dddocr-0.0.2/fastapi_dddocr/__init__.py
+-rw-rw-rw-   0        0        0     2727 2023-05-10 02:12:47.000000 fastapi_dddocr-0.0.2/fastapi_dddocr/fastapi_dddocr.py
+drwxrwxrwx   0        0        0        0 2023-05-10 02:21:08.986063 fastapi_dddocr-0.0.2/fastapi_dddocr.egg-info/
+-rw-rw-rw-   0        0        0      479 2023-05-10 02:21:08.000000 fastapi_dddocr-0.0.2/fastapi_dddocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-10 02:21:08.000000 fastapi_dddocr-0.0.2/fastapi_dddocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 02:21:08.000000 fastapi_dddocr-0.0.2/fastapi_dddocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-10 02:21:08.000000 fastapi_dddocr-0.0.2/fastapi_dddocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 02:21:08.000000 fastapi_dddocr-0.0.2/fastapi_dddocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 02:21:08.986063 fastapi_dddocr-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2023-05-10 02:21:04.000000 fastapi_dddocr-0.0.2/setup.py
```

### Comparing `fastapi_dddocr-0.0.1/LICENSE.txt` & `fastapi_dddocr-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_dddocr-0.0.1/fastapi_dddocr/fastapi_dama_docr.py` & `fastapi_dddocr-0.0.2/fastapi_dddocr/fastapi_dddocr.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,11 +87,11 @@
     else:
         item["state"] = -1
         item["remark"] = '图片为空!!!'
     return item
 
 def run():
     name_app = os.path.basename(__file__)[0:-3]
-    uvicorn.run(f'{name_app}:app', host="0.0.0.0", port=12135, reload=True)
+    uvicorn.run(f'{name_app}:app', host="0.0.0.0", port=12135, reload=False)
 
 if __name__ == "__main__":
     run()
```

### Comparing `fastapi_dddocr-0.0.1/setup.py` & `fastapi_dddocr-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,22 +9,27 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastapi_dddocr",  # 用自己的名替换
-    version="0.0.1",  # 包版本号，便于维护版本
+    version="0.0.2",  # 包版本号，便于维护版本
     author="jixn",  # 作者，可以写自己的姓名
     author_email="1770550067@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="这一个api接口，主要是用于验证码识别",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
+    install_requires=[
+            'ddddocr',
+            'fastapi',
+            'uvicorn'
+        ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',  # 对python的最低版本要求
 )
```

