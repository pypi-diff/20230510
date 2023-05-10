# Comparing `tmp/prodia-python-2.2.tar.gz` & `tmp/prodia-python-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodia-python-2.2.tar", last modified: Fri May  5 14:29:49 2023, max compression
+gzip compressed data, was "prodia-python-2.3.tar", last modified: Wed May 10 10:09:45 2023, max compression
```

## Comparing `prodia-python-2.2.tar` & `prodia-python-2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 14:29:49.383146 prodia-python-2.2/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-2.2/LICENSE
--rw-rw-rw-   0        0        0     2354 2023-05-05 14:29:49.382596 prodia-python-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2128 2023-05-05 12:19:03.000000 prodia-python-2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 14:29:49.372146 prodia-python-2.2/prodia/
--rw-rw-rw-   0        0        0       95 2023-05-05 14:08:13.000000 prodia-python-2.2/prodia/__init__.py
--rw-rw-rw-   0        0        0     2225 2023-05-05 10:09:12.000000 prodia-python-2.2/prodia/data.py
--rw-rw-rw-   0        0        0     5249 2023-05-05 11:51:07.000000 prodia-python-2.2/prodia/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 14:29:49.381147 prodia-python-2.2/prodia_python.egg-info/
--rw-rw-rw-   0        0        0     2354 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 14:29:49.000000 prodia-python-2.2/prodia_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 14:29:49.383146 prodia-python-2.2/setup.cfg
--rw-rw-rw-   0        0        0      401 2023-05-05 12:19:48.000000 prodia-python-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:45.593871 prodia-python-2.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodia-python-2.3/LICENSE
+-rw-rw-rw-   0        0        0     2678 2023-05-10 10:09:45.593661 prodia-python-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2452 2023-05-10 07:48:22.000000 prodia-python-2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:45.578871 prodia-python-2.3/prodia/
+-rw-rw-rw-   0        0        0      111 2023-05-10 09:58:54.000000 prodia-python-2.3/prodia/__init__.py
+-rw-rw-rw-   0        0        0     2225 2023-05-05 10:09:12.000000 prodia-python-2.3/prodia/data.py
+-rw-rw-rw-   0        0        0    10126 2023-05-10 10:02:36.000000 prodia-python-2.3/prodia/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:09:45.591870 prodia-python-2.3/prodia_python.egg-info/
+-rw-rw-rw-   0        0        0     2678 2023-05-10 10:09:45.000000 prodia-python-2.3/prodia_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-05-10 10:09:45.000000 prodia-python-2.3/prodia_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:09:45.000000 prodia-python-2.3/prodia_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 10:09:45.000000 prodia-python-2.3/prodia_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 10:09:45.000000 prodia-python-2.3/prodia_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 10:09:45.593871 prodia-python-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      401 2023-05-10 09:58:38.000000 prodia-python-2.3/setup.py
```

### Comparing `prodia-python-2.2/LICENSE` & `prodia-python-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prodia-python-2.2/PKG-INFO` & `prodia-python-2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: prodia-python
-Version: 2.2
+Version: 2.3
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodia-python==2.2
+pip install prodia-python==2.3
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
@@ -42,14 +42,29 @@
 image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
 
 image = prodia.img2img(imageUrl=image_url, prompt="winter nature wallpaper")
 
 print(image)
 ```
 
+### Asynchronous usage
+```py
+import prodia
+import asyncio
+prodia.Client(api_key='your-api-key')
+
+async def test():
+#...
+    text2image = await prodia.arunv1(prompt="clouds")
+    image2image = await prodia.arunv2(imageUrl="here-url", prompt="clouds")
+    print(text2image, image2image)
+
+asyncio.run(test)
+```
+
 ### Additional info
 
 All available arguments for txt2img():
 - prompt:str(required)
 - negative_prompt:str
 - model:str check all available models on https://docs.prodia.com/reference/generate
 - sampler:str check all available samplers on https://docs.prodia.com/reference/generate
```

### Comparing `prodia-python-2.2/README.md` & `prodia-python-2.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodia-python==2.2
+pip install prodia-python==2.3
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
@@ -32,14 +32,29 @@
 image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
 
 image = prodia.img2img(imageUrl=image_url, prompt="winter nature wallpaper")
 
 print(image)
 ```
 
+### Asynchronous usage
+```py
+import prodia
+import asyncio
+prodia.Client(api_key='your-api-key')
+
+async def test():
+#...
+    text2image = await prodia.arunv1(prompt="clouds")
+    image2image = await prodia.arunv2(imageUrl="here-url", prompt="clouds")
+    print(text2image, image2image)
+
+asyncio.run(test)
+```
+
 ### Additional info
 
 All available arguments for txt2img():
 - prompt:str(required)
 - negative_prompt:str
 - model:str check all available models on https://docs.prodia.com/reference/generate
 - sampler:str check all available samplers on https://docs.prodia.com/reference/generate
```

### Comparing `prodia-python-2.2/prodia/data.py` & `prodia-python-2.3/prodia/data.py`

 * *Files identical despite different names*

### Comparing `prodia-python-2.2/prodia_python.egg-info/PKG-INFO` & `prodia-python-2.3/prodia_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: prodia-python
-Version: 2.2
+Version: 2.3
 Summary: Prodia API Python Wrapper
 Author: yoou3-cyber
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodia-python
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodia-python==2.2
+pip install prodia-python==2.3
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
@@ -42,14 +42,29 @@
 image_url = 'https://images.prodia.xyz/a77bfbb2-4808-4178-8bed-eed51077a476.png' #here should be url of your image
 
 image = prodia.img2img(imageUrl=image_url, prompt="winter nature wallpaper")
 
 print(image)
 ```
 
+### Asynchronous usage
+```py
+import prodia
+import asyncio
+prodia.Client(api_key='your-api-key')
+
+async def test():
+#...
+    text2image = await prodia.arunv1(prompt="clouds")
+    image2image = await prodia.arunv2(imageUrl="here-url", prompt="clouds")
+    print(text2image, image2image)
+
+asyncio.run(test)
+```
+
 ### Additional info
 
 All available arguments for txt2img():
 - prompt:str(required)
 - negative_prompt:str
 - model:str check all available models on https://docs.prodia.com/reference/generate
 - sampler:str check all available samplers on https://docs.prodia.com/reference/generate
```

