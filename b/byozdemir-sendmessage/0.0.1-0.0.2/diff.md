# Comparing `tmp/byozdemir-sendmessage-0.0.1.tar.gz` & `tmp/byozdemir-sendmessage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byozdemir-sendmessage-0.0.1.tar", last modified: Mon May  8 11:24:02 2023, max compression
+gzip compressed data, was "byozdemir-sendmessage-0.0.2.tar", last modified: Wed May 10 09:10:44 2023, max compression
```

## Comparing `byozdemir-sendmessage-0.0.1.tar` & `byozdemir-sendmessage-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 11:24:02.474216 byozdemir-sendmessage-0.0.1/
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      959 2023-05-08 11:24:02.474216 byozdemir-sendmessage-0.0.1/PKG-INFO
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      556 2023-05-08 11:23:43.000000 byozdemir-sendmessage-0.0.1/README.md
-drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 11:24:02.474216 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage/
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      272 2023-05-08 11:09:07.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage/__init__.py
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      392 2023-05-08 11:08:44.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage/discord.py
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      725 2023-05-08 11:07:43.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage/mail.py
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      178 2023-05-03 13:41:55.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage/netgsm.py
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      245 2023-05-08 11:08:32.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage/telegram.py
-drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-08 11:24:02.474216 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage.egg-info/
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      959 2023-05-08 11:24:02.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage.egg-info/PKG-INFO
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      405 2023-05-08 11:24:02.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage.egg-info/SOURCES.txt
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)        1 2023-05-08 11:24:02.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage.egg-info/dependency_links.txt
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       17 2023-05-08 11:24:02.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage.egg-info/requires.txt
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       22 2023-05-08 11:24:02.000000 byozdemir-sendmessage-0.0.1/byozdemir_sendmessage.egg-info/top_level.txt
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       38 2023-05-08 11:24:02.474216 byozdemir-sendmessage-0.0.1/setup.cfg
--rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      796 2023-05-08 11:23:25.000000 byozdemir-sendmessage-0.0.1/setup.py
+drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-10 09:10:44.489820 byozdemir-sendmessage-0.0.2/
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      953 2023-05-10 09:10:44.489820 byozdemir-sendmessage-0.0.2/PKG-INFO
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      676 2023-05-10 09:10:21.000000 byozdemir-sendmessage-0.0.2/README.md
+drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-10 09:10:44.489820 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage/
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      272 2023-05-08 11:09:07.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage/__init__.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      578 2023-05-10 09:06:49.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage/discord.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      971 2023-05-10 09:08:34.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage/mail.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      178 2023-05-03 13:41:55.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage/netgsm.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      829 2023-05-10 09:05:55.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage/skype.py
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      435 2023-05-10 09:07:28.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage/telegram.py
+drwxr-xr-x   0 modernistasyon  (1000) modernistasyon  (1000)        0 2023-05-10 09:10:44.489820 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage.egg-info/
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      953 2023-05-10 09:10:44.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage.egg-info/PKG-INFO
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      436 2023-05-10 09:10:44.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)        1 2023-05-10 09:10:44.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       22 2023-05-10 09:10:44.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage.egg-info/requires.txt
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       22 2023-05-10 09:10:44.000000 byozdemir-sendmessage-0.0.2/byozdemir_sendmessage.egg-info/top_level.txt
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)       38 2023-05-10 09:10:44.489820 byozdemir-sendmessage-0.0.2/setup.cfg
+-rw-r--r--   0 modernistasyon  (1000) modernistasyon  (1000)      675 2023-05-10 09:09:15.000000 byozdemir-sendmessage-0.0.2/setup.py
```

### Comparing `byozdemir-sendmessage-0.0.1/PKG-INFO` & `byozdemir-sendmessage-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: byozdemir-sendmessage
-Version: 0.0.1
+Version: 0.0.2
 Summary: It's helps you tou send message via populer apps
 Author: Byozdemir
 Author-email: emrenetwork@yandex.com
 License: MIT
 Keywords: telegram messager,discord messager
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 
 # byozdemir-sendmessage
 
 This is the library that you can send messages via telegram,discord and email. 
 
 ## Installation
@@ -25,13 +22,22 @@
 
 ## Usage
 
 ```python
 import byozdemir_sendmessage
 
 # Returns 'provider which is you selected'
-# You can select telegram,discord,mail
+# You can select telegram,discord,mail,skype
 messager = byozdemir_sendmessage.getProvider('discord',key="discord key here")
 
 #Send Message
-messager.sendMessage('receiver_id','This is an test message')
+messager.sendMessage('receiver_id','This is a test message')
 
+#Help. This method returns how to use the selected provider.
+messager.help()
+
+#TODO
+```bash
+signal
+line
+netgsm
+```
```

### Comparing `byozdemir-sendmessage-0.0.1/byozdemir_sendmessage/mail.py` & `byozdemir-sendmessage-0.0.2/byozdemir_sendmessage/mail.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,8 +11,15 @@
         msg = MIMEText(message)
         msg['Subject'] = data.get('subject')
         msg['From'] = self.SMTP_user
         msg['To'] = receiver_id
         smtp_server = smtplib.SMTP_SSL(self.SMTP_server, self.SMTP_port)
         smtp_server.login(self.SMTP_user, self.SMTP_password)
         smtp_server.sendmail(self.SMTP_user, receiver_id, msg.as_string())
-        smtp_server.quit()
+        smtp_server.quit()
+
+    def help(self):
+        print("""
+Usage
+    messager = byozdemir_sendmessage.getProvider("mail",user='user',password='password',server='server',port='port')
+    message.sendMessage('targetMail','message here',subject='subject')
+        """)
```

### Comparing `byozdemir-sendmessage-0.0.1/byozdemir_sendmessage.egg-info/PKG-INFO` & `byozdemir-sendmessage-0.0.2/byozdemir_sendmessage.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: byozdemir-sendmessage
-Version: 0.0.1
+Version: 0.0.2
 Summary: It's helps you tou send message via populer apps
 Author: Byozdemir
 Author-email: emrenetwork@yandex.com
 License: MIT
 Keywords: telegram messager,discord messager
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
 
 # byozdemir-sendmessage
 
 This is the library that you can send messages via telegram,discord and email. 
 
 ## Installation
@@ -25,13 +22,22 @@
 
 ## Usage
 
 ```python
 import byozdemir_sendmessage
 
 # Returns 'provider which is you selected'
-# You can select telegram,discord,mail
+# You can select telegram,discord,mail,skype
 messager = byozdemir_sendmessage.getProvider('discord',key="discord key here")
 
 #Send Message
-messager.sendMessage('receiver_id','This is an test message')
+messager.sendMessage('receiver_id','This is a test message')
 
+#Help. This method returns how to use the selected provider.
+messager.help()
+
+#TODO
+```bash
+signal
+line
+netgsm
+```
```

### Comparing `byozdemir-sendmessage-0.0.1/setup.py` & `byozdemir-sendmessage-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,19 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = "byozdemir-sendmessage",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Byozdemir",
     author_email = "emrenetwork@yandex.com",
     description = ("It's helps you tou send message via populer apps"),
     license = "MIT",
     keywords = "telegram messager,discord messager",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    install_requires = ['requests','telepot'],
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Topic :: Utilities",
-        "License :: OSI Approved :: BSD License",
-    ],
+    install_requires = ['requests','telepot','skpy'],
+    classifiers=[],
 )
```

