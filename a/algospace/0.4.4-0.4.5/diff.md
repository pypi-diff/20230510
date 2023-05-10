# Comparing `tmp/algospace-0.4.4.tar.gz` & `tmp/algospace-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algospace-0.4.4.tar", last modified: Mon Apr 10 08:41:11 2023, max compression
+gzip compressed data, was "algospace-0.4.5.tar", last modified: Wed May 10 08:47:40 2023, max compression
```

## Comparing `algospace-0.4.4.tar` & `algospace-0.4.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-10 08:41:00.000000 algospace-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 08:41:00.000000 algospace-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-10 08:41:11.246638 algospace-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-10 08:41:00.000000 algospace-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.242638 algospace-0.4.4/algospace/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/customer/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/customer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/customer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/customer/fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/customer/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/login.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/docker_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/enroll.py
--rw-r--r--   0 runner    (1001) docker     (123)    41153 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/stdio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/provider/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/algospace-config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace/provider/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-docker-logs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-docker-start.sh
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-docker-stop.sh
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/provider/templates/docker/algospace-dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/util.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 08:41:00.000000 algospace-0.4.4/algospace/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 08:41:11.246638 algospace-0.4.4/algospace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-10 08:41:11.000000 algospace-0.4.4/algospace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 08:41:11.246638 algospace-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-10 08:41:00.000000 algospace-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.723793 algospace-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 08:47:25.000000 algospace-0.4.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 08:47:25.000000 algospace-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-10 08:47:40.723793 algospace-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-10 08:47:25.000000 algospace-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/customer/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/customer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/customer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/customer/fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/customer/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/login.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24282 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/docker_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/enroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41280 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/stdio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace/provider/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/algospace-config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.723793 algospace-0.4.5/algospace/provider/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-docker-logs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-docker-start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-docker-stop.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/provider/templates/docker/algospace-dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 08:47:25.000000 algospace-0.4.5/algospace/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:47:40.719793 algospace-0.4.5/algospace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 08:47:40.000000 algospace-0.4.5/algospace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:47:40.723793 algospace-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 08:47:25.000000 algospace-0.4.5/setup.py
```

### Comparing `algospace-0.4.4/PKG-INFO` & `algospace-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.4
+Version: 0.4.5
 Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
```

### Comparing `algospace-0.4.4/README.md` & `algospace-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/__init__.py` & `algospace-0.4.5/algospace/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/__main__.py` & `algospace-0.4.5/algospace/__main__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/customer/fn.py` & `algospace-0.4.5/algospace/customer/fn.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/customer/service.py` & `algospace-0.4.5/algospace/customer/service.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/exceptions/__init__.py` & `algospace-0.4.5/algospace/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/logger.py` & `algospace-0.4.5/algospace/logger.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/login.py` & `algospace-0.4.5/algospace/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: 
 @Author: Ecohnoch(xcy)
 @Date: 2022-10-06 12:30:47
 @LastEditors: Kermit
-@LastEditTime: 2023-02-17 13:57:13
+@LastEditTime: 2023-05-10 16:43:49
 '''
 
 import time
 from typing import Optional
 import requests
 import traceback
 import algospace.config as config
@@ -28,14 +28,15 @@
 class LoginInstance(metaclass=Singleton):
     def __init__(self, cookie: str = '', timestamp: int = 0):
         self.cookie = cookie
         self.timestamp = timestamp
         self.secret = ''
         self.username = ''
         self.password = ''
+        self.privilege = 'CUSTOMER'
 
     def ever_logined(self) -> bool:
         return self.secret != '' or (self.username != '' and self.password != '')
 
     def is_outdated(self) -> bool:
         curr_timestamp = int(time.time())
         return curr_timestamp - self.timestamp > 10 * 24 * 60 * 60
@@ -54,34 +55,35 @@
     def get_header(self) -> dict:
         return {'Cookie': self.get_cookie()}
 
     def login(self,
               secret: Optional[str] = '',
               username: Optional[str] = '',
               password: Optional[str] = '',
-              privilege: Optional[str] = 'CUSTOMER') -> bool:
+              privilege: Optional[str] = '') -> bool:
         self.secret = secret or self.secret
         self.username = username or self.username
         self.password = password or self.password
+        self.privilege = privilege or self.privilege
         try:
             login_url = config.login_by_secret_url if self.secret != '' else config.login_url
             login_data = {
                 'user_id': self.username,
                 'password': self.password
             } if self.secret == '' else {
                 'secret': self.secret
             }
             response = requests.post(login_url, data=login_data)
             if response.status_code != 200 and response.status_code != 201:
                 raise Exception(response.status_code, response.content.decode())
             if response.json()['status'] != 200:
                 raise Exception(response.json().get('err_msg', 'Login error.'))
             if self.secret != '':
-                if response.json()['data']['privilege'] != 'ADMINISTER' and response.json()['data']['privilege'] != privilege:
-                    raise LoginError(f'LoginError: Secret privilege is not {privilege}.')
+                if response.json()['data']['privilege'] != 'ADMINISTER' and response.json()['data']['privilege'] != self.privilege:
+                    raise LoginError(f'LoginError: Secret privilege is not {self.privilege}.')
                 self.username = response.json()['data']['user_id']
                 self.password = ''
             self.set_cookie(response.headers['Set-Cookie'], int(time.time()))
             return True
         except Exception as e:
             traceback.print_exc()
             return False
```

### Comparing `algospace-0.4.4/algospace/provider/cloud.py` & `algospace-0.4.5/algospace/provider/cloud.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/provider/config.py` & `algospace-0.4.5/algospace/provider/config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/provider/config_generator.py` & `algospace-0.4.5/algospace/provider/config_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/provider/config_loader.py` & `algospace-0.4.5/algospace/provider/config_loader.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/provider/docker_generator.py` & `algospace-0.4.5/algospace/provider/docker_generator.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/provider/enroll.py` & `algospace-0.4.5/algospace/provider/enroll.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/provider/service.py` & `algospace-0.4.5/algospace/provider/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 '''
 @Description: 算法提供者核心服务
 @Author: Kermit
 @Date: 2022-11-05 16:46:46
 @LastEditors: Kermit
-@LastEditTime: 2023-04-04 14:54:51
+@LastEditTime: 2023-04-14 12:52:52
 '''
 
 from typing import Any, Callable, Optional, List, Tuple, Union
 from algospace.logger import Logger, algospace_logger
 from algospace.util import create_timestamp_filename
 from . import config
 from .config import Algoinfo
@@ -881,20 +881,23 @@
             stdio_exec_all = queue_stdio_exec.exec_all
             is_execed = True
             while True:
                 try:
                     if not is_execed:
                         await asyncio.sleep(0.1)
                     is_execed = await asyncio.get_running_loop().run_in_executor(None, stdio_exec)
-                except Exception as e:
-                    traceback.print_exc()
-                    self.algo_logger.error(f'Handle subprocess stdio error: {str(e)}')
+                except concurrent.futures._base.CancelledError:
+                    stdio_exec_all()
+                    raise
                 except asyncio.CancelledError:
                     stdio_exec_all()
                     raise
+                except Exception as e:
+                    traceback.print_exc()
+                    self.algo_logger.error(f'Handle subprocess stdio error: {str(e)}')
 
         # 当有任务抛出异常时，停止所有任务
         tasks = [alive_task(), heartbeat_task(), subprocess_stdio_task()]
         done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_EXCEPTION)
         for task in pending:
             task.cancel()
         for task in done:
```

### Comparing `algospace-0.4.4/algospace/provider/stdio.py` & `algospace-0.4.5/algospace/provider/stdio.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace/provider/templates/algospace-config.py` & `algospace-0.4.5/algospace/provider/templates/algospace-config.py`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/algospace.egg-info/PKG-INFO` & `algospace-0.4.5/algospace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algospace
-Version: 0.4.4
+Version: 0.4.5
 Summary: AlgoSpace: A platform for displaying and using algorithm achievements
 Home-page: https://github.com/Algo-Space/algospace-pypi
 Author: DBIIR
 Author-email: ckeming@outlook.com
 Maintainer: DBIIR
 Maintainer-email: ckeming@outlook.com
 License: BSD License
```

### Comparing `algospace-0.4.4/algospace.egg-info/SOURCES.txt` & `algospace-0.4.5/algospace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `algospace-0.4.4/setup.py` & `algospace-0.4.5/setup.py`

 * *Files identical despite different names*

