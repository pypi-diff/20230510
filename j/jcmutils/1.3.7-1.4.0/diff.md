# Comparing `tmp/jcmutils-1.3.7.tar.gz` & `tmp/jcmutils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcmutils-1.3.7.tar", last modified: Wed Apr 19 07:20:45 2023, max compression
+gzip compressed data, was "jcmutils-1.4.0.tar", last modified: Wed May 10 03:07:24 2023, max compression
```

## Comparing `jcmutils-1.3.7.tar` & `jcmutils-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 07:20:45.910784 jcmutils-1.3.7/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.3.7/LICENSE
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 07:20:45.910784 jcmutils-1.3.7/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.3.7/README.md
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 07:20:45.910784 jcmutils-1.3.7/jcmutils/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.3.7/jcmutils/__init__.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2613 2023-04-19 07:20:15.000000 jcmutils-1.3.7/jcmutils/dataset_utils.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.3.7/jcmutils/gen_sources.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.3.7/jcmutils/logger.py
--rw-rw-r--   0 junquan   (1002) junquan   (1003)     8002 2023-04-19 01:54:58.000000 jcmutils-1.3.7/jcmutils/solver.py
-drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-04-19 07:20:45.910784 jcmutils-1.3.7/jcmutils.egg-info/
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/PKG-INFO
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/SOURCES.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/dependency_links.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/requires.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-04-19 07:20:45.000000 jcmutils-1.3.7/jcmutils.egg-info/top_level.txt
--rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-04-19 07:20:45.910784 jcmutils-1.3.7/setup.cfg
--rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-04-19 07:20:18.000000 jcmutils-1.3.7/setup.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 03:07:24.555660 jcmutils-1.4.0/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1073 2023-04-15 12:55:54.000000 jcmutils-1.4.0/LICENSE
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-10 03:07:24.555660 jcmutils-1.4.0/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     3044 2023-04-15 12:55:54.000000 jcmutils-1.4.0/README.md
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 03:07:24.555660 jcmutils-1.4.0/jcmutils/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      165 2023-04-18 07:48:21.000000 jcmutils-1.4.0/jcmutils/__init__.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2613 2023-04-19 07:20:15.000000 jcmutils-1.4.0/jcmutils/dataset_utils.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     2151 2023-04-15 12:55:54.000000 jcmutils-1.4.0/jcmutils/gen_sources.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     1496 2023-04-15 12:55:54.000000 jcmutils-1.4.0/jcmutils/logger.py
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)     8801 2023-05-10 03:03:53.000000 jcmutils-1.4.0/jcmutils/solver.py
+drwxrwxr-x   0 junquan   (1002) junquan   (1003)        0 2023-05-10 03:07:24.555660 jcmutils-1.4.0/jcmutils.egg-info/
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      332 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/PKG-INFO
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      294 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        1 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       31 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/requires.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)        9 2023-05-10 03:07:24.000000 jcmutils-1.4.0/jcmutils.egg-info/top_level.txt
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)       38 2023-05-10 03:07:24.555660 jcmutils-1.4.0/setup.cfg
+-rw-rw-r--   0 junquan   (1002) junquan   (1003)      530 2023-05-10 03:06:10.000000 jcmutils-1.4.0/setup.py
```

### Comparing `jcmutils-1.3.7/LICENSE` & `jcmutils-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.7/README.md` & `jcmutils-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.7/jcmutils/dataset_utils.py` & `jcmutils-1.4.0/jcmutils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.7/jcmutils/gen_sources.py` & `jcmutils-1.4.0/jcmutils/gen_sources.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.7/jcmutils/logger.py` & `jcmutils-1.4.0/jcmutils/logger.py`

 * *Files identical despite different names*

### Comparing `jcmutils-1.3.7/jcmutils/solver.py` & `jcmutils-1.4.0/jcmutils/solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import jcmwave
 import numpy as np
 from .logger import logger
 import os
 import shutil
 import cv2
+import datetime
 
 
 class solver:
     def __init__(self, jcmp_path, database_path, keys):
         # 初始化成员变量
         self.jcmp_path = jcmp_path
         self.keys = keys
@@ -19,38 +20,34 @@
             os.makedirs(os.path.dirname(database_path))
         self.resultbag = jcmwave.Resultbag(abs_resultbag_dir)
         self.has_inited = True
         logger.info("solver inited")
         logger.debug(f"solver parameters:jcmp_path-{jcmp_path};database_path-{abs_resultbag_dir}")
 
     def solve(self):
-        # 检查是否被以被初始化，若还未被初始化则报错
-        try:
-            if self.has_inited:
-                logger.debug("solver class have been inited")
-        except NameError:
-            print("Error ! please init solver befor using it!!!!!!")
-            raise Exception("Please init solver before using it")
+        self.__check_logger()
 
         # 初始化变量
         job_ids = []
         waiting_keys = self.keys
         no_error = False
 
         # 当存在有报错的项目或首次执行时进入循环
         while not no_error:
 
             # 开始计算
+            last_time = self.__start_timing()
             for key in waiting_keys:
                 job_id = jcmwave.solve(
                     self.jcmp_path, keys=key, temporary=True, resultbag=self.resultbag)
                 job_ids.append(job_id)
             logger.info("solve queue added done! start solving")
             jcmwave.daemon.wait(job_ids, resultbag=self.resultbag)
-            logger.info("solver program completed! analysing results...")
+            cost_time = self.__count_time(last_time)
+            logger.info(f"solver program completed!,cost{cost_time} analysing results...")
             no_error = True
 
             # 提取错误信息，如果是oom错误则加入队列重新计算
             backup_keys = []
             for key in waiting_keys:
                 jcm_log = self.resultbag.get_log(key)
                 if jcm_log['ExitCode'] == 0:
@@ -76,66 +73,67 @@
             # 如果出现了oom错误，替换队列，再次计算
             if not no_error:
                 waiting_keys = backup_keys
 
         logger.info("analyse complete ! No error report ! solve mission done!!")
 
     def show_image(self, key, num_of_result, is_light_intense=False,vmax=None):
-        if not self.resultbag.check_result(key):
-            logger.error("get result failed! target key not find")
-            logger.error(f"the key is : {key}")
-            return -1
+        self.__check_logger()
+        self.check_result(key)
 
         # 开始提取
         result = self.resultbag.get_result(key)
         field = (result[num_of_result]['field'][0].conj() *
                  result[num_of_result]['field'][0]).sum(axis=2).real
         if is_light_intense:
             field = np.power(field, 2)
         vmaxa = np.max(field) if vmax is None else vmax
         field = (field / vmaxa)*235
         field = np.rot90(field)
         cv2.imshow("image",field)
 
     def get_result(self, key):
+        self.__check_logger()
+        self.check_result(key)
         return self.resultbag.get_result(key)
 
     def save_image(self, target_directory, key, num_of_result, is_light_intense=False,vmax=None):
-        if not self.resultbag.check_result(key):
-            logger.error("get result failed! target key not find")
-            logger.error(f"the key is : {key}")
-            return -1
+        self.__check_logger()
+        self.check_result(key)
 
         # 开始提取
         result = self.resultbag.get_result(key)
         field = (result[num_of_result]['field'][0].conj() *
                  result[num_of_result]['field'][0]).sum(axis=2).real
         if is_light_intense:
             field = np.power(field, 2)
         if not os.path.exists(target_directory):
-            logger.debug("target directory dosen't exist,creating...")
+            logger.info("target directory dosen't exist,creating...")
             os.makedirs(target_directory)
         vmaxa = np.max(field) if vmax is None else vmax
         field = (field / vmaxa)*235
         field = np.rot90(field)
         cv2.imwrite(target_directory.rstrip("/")+"output.jpg",field)
+        logger.info("target image saved successfully")
 
     def save_all_image(self, num_of_result, target_directory, is_light_intense=False, is_symmetry=False,vmax=None):
-        if not self.resultbag.check_result(self.keys[0]):
-            logger.error("get result failed! target key not find")
-            logger.error(f"the key is : {self.keys[0]}")
-            return -1
+        self.__check_logger()
+        self.check_result(self.keys[0])
 
+        # 计时
+        last_time = self.__start_timing()
+        
         # 开始提取
         # 先确定total_result的形状
         temp_result = self.resultbag.get_result(self.keys[0])
         field = (temp_result[num_of_result]['field'][0].conj() *
                  temp_result[num_of_result]['field'][0]).sum(axis=2).real
         total_results = np.zeros(field.shape)
         logger.debug(f"total_result shape defined as {total_results.shape}")
+        
 
         # 开始逐个提取结果
         for key in self.keys:
             # 目录检查
             if not os.path.exists(target_directory):
                 logger.debug("target directory dosen't exist,creating...")
                 os.makedirs(target_directory)
@@ -160,16 +158,18 @@
                 logger.debug("key was rotated for symmetry")
 
         logger.debug(f"printing max value of results:{np.max(total_results)}")
         vmaxa = np.max(total_results) if vmax is None else vmax
         sfield = (total_results/ vmaxa)*235
         file_name = target_directory.rstrip('/') + '/' + "total_result.jpg"
         cv2.imwrite(file_name,sfield)
-        logger.info("all target image saved completed!")
+        cost_time = self.__count_time(last_time)
+        logger.info(f"all target image saved completed! cost {cost_time}")
 
+    # 工具函数，处理词典，用处是将保存时的文件名缩短
     def __solve_dict(self, target_dict):
         res = ""
         for key, value in target_dict.items():
             res += key + "-"
             if isinstance(value, list):
                 for i in value:
                     if isinstance(i, float):
@@ -177,14 +177,38 @@
                     else:
                         res += f"{i}-"
             else:
                 res += f"{value}-"
         res.rstrip('-')
         return res
 
+    # 将root_dir目录下面的total_result.jpg移动至目标位置
     def move_total_results(self,root_dir,target_dir):
+        self.__check_logger()
         filelist = os.listdir(root_dir)
         for file in filelist:
             if file == "total_result.jpg":
                 if not os.path.exists(target_dir):
                     os.makedirs(target_dir)
-                shutil.copyfile(os.path.join(root_dir,file),os.path.join(target_dir,os.path.basename(root_dir) + ".jpg"))
+                shutil.copyfile(os.path.join(root_dir,file),os.path.join(target_dir,os.path.basename(root_dir) + ".jpg"))
+    
+    # 检查是否被以被初始化，若还未被初始化则报错
+    def __check_logger(self):
+        try:
+            if self.has_inited:
+                logger.debug("solver class have been inited")
+        except NameError:
+            print("Error ! please init solver befor using it!!!!!!")
+            raise Exception("Please init solver before using it")
+
+    # 检查是否存在目标键值，如无则报错
+    def check_result(self,key):
+        if not self.resultbag.check_result(key):
+            logger.error("get result failed! target key not find in resultbag")
+            logger.error(f"the key is : {key}")
+            raise Exception(f"get result failed! target key not find in resultbag,the key is {key}")
+    
+    def __start_timing(self):
+        return datetime.datetime.now()
+    
+    def __count_time(self,last_time):
+        return datetime.timedelta(datetime.datetime.now() - last_time)
```

### Comparing `jcmutils-1.3.7/setup.py` & `jcmutils-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 
-VERSION = '1.3.7'
+VERSION = '1.4.0'
 DESCRIPTION = "A general utils for jcmsuite"
 
 setup(
     name="jcmutils",
     version=VERSION,
     author="crafter-z",
     author_email="crafterz@163.com",
```

