# Comparing `tmp/pwl-chat-python-1.4.0.tar.gz` & `tmp/pwl-chat-python-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl-chat-python-1.4.0.tar", last modified: Tue May  9 06:40:47 2023, max compression
+gzip compressed data, was "pwl-chat-python-1.4.1.tar", last modified: Wed May 10 01:31:14 2023, max compression
```

## Comparing `pwl-chat-python-1.4.0.tar` & `pwl-chat-python-1.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 06:40:47.022046 pwl-chat-python-1.4.0/
--rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/LICENSE
--rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 06:40:47.021508 pwl-chat-python-1.4.0/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)     1410 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/README.md
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 06:40:47.007974 pwl-chat-python-1.4.0/pwl_chat_python.egg-info/
--rw-r--r--   0 fangcong   (501) staff       (20)     2009 2023-05-09 06:40:46.000000 pwl-chat-python-1.4.0/pwl_chat_python.egg-info/PKG-INFO
--rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-09 06:40:46.000000 pwl-chat-python-1.4.0/pwl_chat_python.egg-info/SOURCES.txt
--rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-09 06:40:46.000000 pwl-chat-python-1.4.0/pwl_chat_python.egg-info/dependency_links.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-09 06:40:46.000000 pwl-chat-python-1.4.0/pwl_chat_python.egg-info/entry_points.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-09 06:40:46.000000 pwl-chat-python-1.4.0/pwl_chat_python.egg-info/requires.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-09 06:40:46.000000 pwl-chat-python-1.4.0/pwl_chat_python.egg-info/top_level.txt
--rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-09 06:40:47.022238 pwl-chat-python-1.4.0/setup.cfg
--rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/setup.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 06:40:47.008593 pwl-chat-python-1.4.0/src/
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 06:40:47.012071 pwl-chat-python-1.4.0/src/api/
--rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/api/__api__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1993 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/api/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/api/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/api/user.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 06:40:47.018438 pwl-chat-python-1.4.0/src/core/
--rw-r--r--   0 fangcong   (501) staff       (20)     2625 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/core/__init__.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/core/blacklist.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1818 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/core/chatroom.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1961 2023-05-09 06:39:45.000000 pwl-chat-python-1.4.0/src/core/cli.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/core/config.py
--rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/core/redpacket.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/core/user.py
--rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/core/websocket.py
--rw-r--r--   0 fangcong   (501) staff       (20)      991 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/main.py
-drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-09 06:40:47.020868 pwl-chat-python-1.4.0/src/utils/
--rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.0/src/utils/utils.py
--rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-09 06:39:45.000000 pwl-chat-python-1.4.0/src/utils/version.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.967748 pwl-chat-python-1.4.1/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1066 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/LICENSE
+-rw-r--r--   0 fangcong   (501) staff       (20)     1891 2023-05-10 01:31:14.967242 pwl-chat-python-1.4.1/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)     1292 2023-05-10 01:17:54.000000 pwl-chat-python-1.4.1/README.md
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.953730 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/
+-rw-r--r--   0 fangcong   (501) staff       (20)     1891 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/PKG-INFO
+-rw-r--r--   0 fangcong   (501) staff       (20)      549 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)        1 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/dependency_links.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       49 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/entry_points.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       45 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/requires.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       31 2023-05-10 01:31:14.000000 pwl-chat-python-1.4.1/pwl_chat_python.egg-info/top_level.txt
+-rw-r--r--   0 fangcong   (501) staff       (20)       38 2023-05-10 01:31:14.967907 pwl-chat-python-1.4.1/setup.cfg
+-rw-r--r--   0 fangcong   (501) staff       (20)     3546 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/setup.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.954101 pwl-chat-python-1.4.1/src/
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.957551 pwl-chat-python-1.4.1/src/api/
+-rw-r--r--   0 fangcong   (501) staff       (20)      312 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/api/__api__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1993 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/api/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1743 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/api/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1124 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/api/user.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.964428 pwl-chat-python-1.4.1/src/core/
+-rw-r--r--   0 fangcong   (501) staff       (20)     2625 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/__init__.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1623 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/blacklist.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1960 2023-05-10 01:27:04.000000 pwl-chat-python-1.4.1/src/core/chatroom.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1961 2023-05-09 06:39:45.000000 pwl-chat-python-1.4.1/src/core/cli.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1630 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/config.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     4435 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/redpacket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1360 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/user.py
+-rw-r--r--   0 fangcong   (501) staff       (20)     1226 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/core/websocket.py
+-rw-r--r--   0 fangcong   (501) staff       (20)      991 2023-05-10 01:28:45.000000 pwl-chat-python-1.4.1/src/main.py
+drwxr-xr-x   0 fangcong   (501) staff       (20)        0 2023-05-10 01:31:14.965956 pwl-chat-python-1.4.1/src/utils/
+-rw-r--r--   0 fangcong   (501) staff       (20)      739 2023-05-09 06:35:44.000000 pwl-chat-python-1.4.1/src/utils/utils.py
+-rw-r--r--   0 fangcong   (501) staff       (20)       21 2023-05-10 01:19:01.000000 pwl-chat-python-1.4.1/src/utils/version.py
```

### Comparing `pwl-chat-python-1.4.0/LICENSE` & `pwl-chat-python-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/PKG-INFO` & `pwl-chat-python-1.4.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.0
+Version: 1.4.1
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,70 +13,58 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # pwl-chat-python
->
-> 摸鱼派聊天室python命令行客户端
 
-基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室python客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
+> 摸鱼派聊天室 python 命令行客户端
 
-* 💬 基本聊天吹水；
-* ⬆️ 社区快捷命令
-  * 领取昨日活跃度奖励
-  * 查看个人积分
-  * 查看签到状态
-  * 查看当前活跃度
-  * 查看聊天室在线用户列表
-  * 查询用户详细信息
-* 🤖️ 自动复读
-* 💉 健康检查
-  * 掉线自动恢复
-* 🧠 自言自语
-  * 自定义语句池
-  * 定时发送
-* 🈲️ 小黑屋功能
-  * 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
-  * 将某人从小黑屋中放出
-* 🧧 自动化抢红包（脚本哥）
-  * 自定义抢红包延时
-  * 心跳红包防止踩坑
-  * 心跳红包风险预测
-  * ~~猜拳红包百分百胜率~~
-
-## 效果
-
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
+基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室 python 客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
 
 ## 安装
 
-环境: Python3.10以上
-
-### 第一步
+环境: Python3.10 以上
 
 执行
 
-~~~bash
-pip install -r requirements.txt
-~~~
-
-### 第二步
+```bash
+pip install pwl-chat-python
+```
+
+## 运行
+
+```bash
+pwl-chat-python -u username -p password -c <两步验证码>
+```
+
+## 功能
+
+- 💬 基本聊天吹水；
+- ⬆️ 社区快捷命令
+  - 领取昨日活跃度奖励
+  - 查看个人积分
+  - 查看签到状态
+  - 查看当前活跃度
+  - 查看聊天室在线用户列表
+  - 查询用户详细信息
+- 🤖️ 自动复读
+- 💉 健康检查
+  - 掉线自动恢复
+- 🧠 自言自语
+  - 自定义语句池
+  - 定时发送
+- 🈲️ 小黑屋功能
+  - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
+  - 将某人从小黑屋中放出
+- 🧧 自动化抢红包（脚本哥）
+  - 自定义抢红包延时
+  - 心跳红包防止踩坑
+  - 心跳红包风险预测
+  - ~~猜拳红包百分百胜率~~
 
-在 `config.ini`中配置摸鱼派账号登陆信息
-
-### 第三步
-
-执行
+## 效果
 
-~~~bash
-python main/main.py
-~~~
-
-后台执行
-
-~~~bash
-nohup python -u main/main.py >> pwl.log 2>&1 &
-~~~
+![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
+![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
+![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.0/pwl_chat_python.egg-info/PKG-INFO` & `pwl-chat-python-1.4.1/pwl_chat_python.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl-chat-python
-Version: 1.4.0
+Version: 1.4.1
 Summary: 摸鱼派聊天室python客户端
 Home-page: https://github.com/gakkiyomi/pwl-chat-python
 Author: gakkiyomi
 Author-email: gakkiyomi@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -13,70 +13,58 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # pwl-chat-python
->
-> 摸鱼派聊天室python命令行客户端
 
-基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室python客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
+> 摸鱼派聊天室 python 命令行客户端
 
-* 💬 基本聊天吹水；
-* ⬆️ 社区快捷命令
-  * 领取昨日活跃度奖励
-  * 查看个人积分
-  * 查看签到状态
-  * 查看当前活跃度
-  * 查看聊天室在线用户列表
-  * 查询用户详细信息
-* 🤖️ 自动复读
-* 💉 健康检查
-  * 掉线自动恢复
-* 🧠 自言自语
-  * 自定义语句池
-  * 定时发送
-* 🈲️ 小黑屋功能
-  * 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
-  * 将某人从小黑屋中放出
-* 🧧 自动化抢红包（脚本哥）
-  * 自定义抢红包延时
-  * 心跳红包防止踩坑
-  * 心跳红包风险预测
-  * ~~猜拳红包百分百胜率~~
-
-## 效果
-
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
-![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
+基于摸鱼打工人社区——摸鱼派开放 API 开发的摸鱼派聊天室 python 客户端程序，可以在里面边写 Bug 边愉快地吹水摸鱼。
 
 ## 安装
 
-环境: Python3.10以上
-
-### 第一步
+环境: Python3.10 以上
 
 执行
 
-~~~bash
-pip install -r requirements.txt
-~~~
-
-### 第二步
+```bash
+pip install pwl-chat-python
+```
+
+## 运行
+
+```bash
+pwl-chat-python -u username -p password -c <两步验证码>
+```
+
+## 功能
+
+- 💬 基本聊天吹水；
+- ⬆️ 社区快捷命令
+  - 领取昨日活跃度奖励
+  - 查看个人积分
+  - 查看签到状态
+  - 查看当前活跃度
+  - 查看聊天室在线用户列表
+  - 查询用户详细信息
+- 🤖️ 自动复读
+- 💉 健康检查
+  - 掉线自动恢复
+- 🧠 自言自语
+  - 自定义语句池
+  - 定时发送
+- 🈲️ 小黑屋功能
+  - 拒绝接收黑名单在聊天室发送的信息 (红包除外 😂 )
+  - 将某人从小黑屋中放出
+- 🧧 自动化抢红包（脚本哥）
+  - 自定义抢红包延时
+  - 心跳红包防止踩坑
+  - 心跳红包风险预测
+  - ~~猜拳红包百分百胜率~~
 
-在 `config.ini`中配置摸鱼派账号登陆信息
-
-### 第三步
-
-执行
+## 效果
 
-~~~bash
-python main/main.py
-~~~
-
-后台执行
-
-~~~bash
-nohup python -u main/main.py >> pwl.log 2>&1 &
-~~~
+![image.png](https://pwl.stackoverflow.wiki/2022/01/image-71dba0ea.png)
+![image.png](https://pwl.stackoverflow.wiki/2022/01/image-f74aae7e.png)
+![image.png](https://pwl.stackoverflow.wiki/2022/01/image-1b685256.png)
```

### Comparing `pwl-chat-python-1.4.0/pwl_chat_python.egg-info/SOURCES.txt` & `pwl-chat-python-1.4.1/pwl_chat_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/setup.py` & `pwl-chat-python-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/api/__init__.py` & `pwl-chat-python-1.4.1/src/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/api/chatroom.py` & `pwl-chat-python-1.4.1/src/api/chatroom.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/api/user.py` & `pwl-chat-python-1.4.1/src/api/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/core/__init__.py` & `pwl-chat-python-1.4.1/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/core/blacklist.py` & `pwl-chat-python-1.4.1/src/core/blacklist.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/core/chatroom.py` & `pwl-chat-python-1.4.1/src/core/chatroom.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,17 @@
             if len(GLOBAL_CONFIG.repeat_config.blacklist) > 0 \
                     and GLOBAL_CONFIG.repeat_config.blacklist.__contains__(user):
                 return
             if user == GLOBAL_CONFIG.auth_config.username:
                 print('\t\t\t\t\t\t[' + time + ']')
                 print('\t\t\t\t\t\t你说: ' + message['md'])
             else:
-                print('[' + time + ']')
+                if 'client' in message:
+                    print('[' + time + '] 来自(' + message['client']+')')
+                else:
+                    print('[' + time + ']')
                 print(user + '说:')
                 print(message['md'])
                 print('\r\n')
             if GLOBAL_CONFIG.repeat_config.repeat_mode_switch:
                 msg = message['md']
                 repeat(api, msg)
```

### Comparing `pwl-chat-python-1.4.0/src/core/cli.py` & `pwl-chat-python-1.4.1/src/core/cli.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/core/config.py` & `pwl-chat-python-1.4.1/src/core/config.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/core/redpacket.py` & `pwl-chat-python-1.4.1/src/core/redpacket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/core/user.py` & `pwl-chat-python-1.4.1/src/core/user.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/core/websocket.py` & `pwl-chat-python-1.4.1/src/core/websocket.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/main.py` & `pwl-chat-python-1.4.1/src/main.py`

 * *Files identical despite different names*

### Comparing `pwl-chat-python-1.4.0/src/utils/utils.py` & `pwl-chat-python-1.4.1/src/utils/utils.py`

 * *Files identical despite different names*

