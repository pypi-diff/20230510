# Comparing `tmp/dtalarm-1.0.3.tar.gz` & `tmp/dtalarm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dtalarm-1.0.3.tar", last modified: Wed Nov  9 01:22:34 2022, max compression
+gzip compressed data, was "dist/dtalarm-1.1.0.tar", last modified: Wed May 10 07:02:47 2023, max compression
```

## Comparing `dtalarm-1.0.3.tar` & `dtalarm-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-11-09 01:22:34.000000 dtalarm-1.0.3/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     2218 2022-11-09 01:22:34.000000 dtalarm-1.0.3/PKG-INFO
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1078 2022-11-07 06:57:24.000000 dtalarm-1.0.3/LICENSE
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1584 2022-11-07 06:57:24.000000 dtalarm-1.0.3/README.md
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1228 2022-11-07 06:57:24.000000 dtalarm-1.0.3/setup.py
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       38 2022-11-09 01:22:34.000000 dtalarm-1.0.3/setup.cfg
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-11-09 01:22:34.000000 dtalarm-1.0.3/dtalarm.egg-info/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     2218 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/PKG-INFO
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      252 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/SOURCES.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       51 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/requires.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        8 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/top_level.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        1 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/dependency_links.txt
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-11-09 01:22:34.000000 dtalarm-1.0.3/dtalarm/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      181 2022-11-07 06:57:24.000000 dtalarm-1.0.3/dtalarm/config.py
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     7517 2022-11-07 06:57:24.000000 dtalarm-1.0.3/dtalarm/client.py
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      112 2022-11-07 06:57:24.000000 dtalarm-1.0.3/dtalarm/__init__.py
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)    10717 2022-11-07 06:57:24.000000 dtalarm-1.0.3/dtalarm/base.py
+drwxr-xr-x   0 danyanliu (1506875890) 334330370        0 2023-05-10 07:02:47.000000 dtalarm-1.1.0/
+-rw-r--r--   0 danyanliu (1506875890) 334330370     2449 2023-05-10 07:02:47.000000 dtalarm-1.1.0/PKG-INFO
+-rw-r--r--   0 danyanliu (1506875890) 334330370     1059 2023-04-28 01:48:20.000000 dtalarm-1.1.0/LICENSE
+-rw-r--r--   0 danyanliu (1506875890) 334330370     1817 2023-05-10 06:55:49.000000 dtalarm-1.1.0/README.md
+-rw-r--r--   0 danyanliu (1506875890) 334330370     1226 2023-05-10 07:01:42.000000 dtalarm-1.1.0/setup.py
+-rw-r--r--   0 danyanliu (1506875890) 334330370       38 2023-05-10 07:02:47.000000 dtalarm-1.1.0/setup.cfg
+drwxr-xr-x   0 danyanliu (1506875890) 334330370        0 2023-05-10 07:02:47.000000 dtalarm-1.1.0/dtalarm.egg-info/
+-rw-r--r--   0 danyanliu (1506875890) 334330370     2449 2023-05-10 07:02:46.000000 dtalarm-1.1.0/dtalarm.egg-info/PKG-INFO
+-rw-r--r--   0 danyanliu (1506875890) 334330370      252 2023-05-10 07:02:46.000000 dtalarm-1.1.0/dtalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 danyanliu (1506875890) 334330370       51 2023-05-10 07:02:46.000000 dtalarm-1.1.0/dtalarm.egg-info/requires.txt
+-rw-r--r--   0 danyanliu (1506875890) 334330370        8 2023-05-10 07:02:46.000000 dtalarm-1.1.0/dtalarm.egg-info/top_level.txt
+-rw-r--r--   0 danyanliu (1506875890) 334330370        1 2023-05-10 07:02:46.000000 dtalarm-1.1.0/dtalarm.egg-info/dependency_links.txt
+drwxr-xr-x   0 danyanliu (1506875890) 334330370        0 2023-05-10 07:02:47.000000 dtalarm-1.1.0/dtalarm/
+-rw-r--r--   0 danyanliu (1506875890) 334330370      268 2023-04-03 07:07:51.000000 dtalarm-1.1.0/dtalarm/config.py
+-rw-r--r--   0 danyanliu (1506875890) 334330370    13465 2023-04-26 03:02:25.000000 dtalarm-1.1.0/dtalarm/client.py
+-rw-r--r--   0 danyanliu (1506875890) 334330370     1089 2023-04-27 01:26:23.000000 dtalarm-1.1.0/dtalarm/__init__.py
+-rw-r--r--   0 danyanliu (1506875890) 334330370    10716 2023-05-10 06:21:50.000000 dtalarm-1.1.0/dtalarm/base.py
```

### Comparing `dtalarm-1.0.3/PKG-INFO` & `dtalarm-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dtalarm
-Version: 1.0.3
-Summary: Dtalarm for digital transformer
+Version: 1.1.0
+Summary: Python integration with DRIVE
 Home-page: UNKNOWN
 Author: TimeAshore
 Author-email: timeashore@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -25,62 +25,69 @@
 
 
 ```shell
 $ pip install dtalarm
 ```
 
 
-## Dependencies
-
-
-Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
-
-You can install all dependencies automatically with the following command:
-
-
-```shell
-$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
-```
-
-
 ## Usage
 
-Register a new service on the DRIVE server and get a unique secret_key.
+Register a new service on the DRIVE server and get the secret key.
 
 
 The `DTAlarmConfig` module records the configuration information required to send alarms. Here, you need to configure a server address.
 
 ```python
 from dtalarm import DTAlarmConfig
 
 DTAlarmConfig.SERVER = ""
 ```
 
+Generating alarms is very easy if the service is pre-configured, the following case will send alarms to the preset receivers. 
+```python
+from dtalarm import Alarm
+
+alarm = Alarm(secret_key="")
+alarm.title = "Title"
+```
+
+If the service is not pre-configured, alarms can also be sent in the following way:
 
 Import the `TeamsChannelAlarm` class or the `TeamsPersonalAlarm` class from the package and configure the secret_key property.
 
-After you initialize an object, you can assign a value to the alarm object. If the alarm content is a dataframe, please use the to_json method and assign it to the table property.
+After initialize, you can assign a value to the alarm object. If the alarm content is a dataframe, please use the to_json method and assign it to the table property.
 ```python
 from dtalarm import TeamsChannelAlarm
 
 alarm = TeamsChannelAlarm(secret_key="", channel_address="", template="message_only_v1")
 
 alarm.title = "Title"
 alarm.text = "Content"
 alarm.table = df.to_json()
 ```
 
 
-Finally, use the send function to send the alarm, it will return the response, timeout property: (optional) how many seconds to wait for the server to send data
-        before giving up, as a float or tuple.
+Finally call the send function to send, which can receive parameters supported by requests like timeout (how many seconds to wait for the server response). 
 
 ```python
 response = alarm.send()
 ```
 
 
+## Dependencies
+
+
+Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
+
+You can install all dependencies automatically with the following command:
+
+
+```shell
+$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
+```
+
 
 ## Documentation
 
 *Please install the following version dependencies when send error: ['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']*
```

### Comparing `dtalarm-1.0.3/LICENSE` & `dtalarm-1.1.0/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) [year] [The Python Packaging Authority]
+Copyright (c) [2023] [Time Ashore]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dtalarm-1.0.3/README.md` & `dtalarm-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,60 +5,67 @@
 
 
 ```shell
 $ pip install dtalarm
 ```
 
 
-## Dependencies
-
-
-Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
-
-You can install all dependencies automatically with the following command:
-
-
-```shell
-$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
-```
-
-
 ## Usage
 
-Register a new service on the DRIVE server and get a unique secret_key.
+Register a new service on the DRIVE server and get the secret key.
 
 
 The `DTAlarmConfig` module records the configuration information required to send alarms. Here, you need to configure a server address.
 
 ```python
 from dtalarm import DTAlarmConfig
 
 DTAlarmConfig.SERVER = ""
 ```
 
+Generating alarms is very easy if the service is pre-configured, the following case will send alarms to the preset receivers. 
+```python
+from dtalarm import Alarm
+
+alarm = Alarm(secret_key="")
+alarm.title = "Title"
+```
+
+If the service is not pre-configured, alarms can also be sent in the following way:
 
 Import the `TeamsChannelAlarm` class or the `TeamsPersonalAlarm` class from the package and configure the secret_key property.
 
-After you initialize an object, you can assign a value to the alarm object. If the alarm content is a dataframe, please use the to_json method and assign it to the table property.
+After initialize, you can assign a value to the alarm object. If the alarm content is a dataframe, please use the to_json method and assign it to the table property.
 ```python
 from dtalarm import TeamsChannelAlarm
 
 alarm = TeamsChannelAlarm(secret_key="", channel_address="", template="message_only_v1")
 
 alarm.title = "Title"
 alarm.text = "Content"
 alarm.table = df.to_json()
 ```
 
 
-Finally, use the send function to send the alarm, it will return the response, timeout property: (optional) how many seconds to wait for the server to send data
-        before giving up, as a float or tuple.
+Finally call the send function to send, which can receive parameters supported by requests like timeout (how many seconds to wait for the server response). 
 
 ```python
 response = alarm.send()
 ```
 
 
+## Dependencies
+
+
+Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
+
+You can install all dependencies automatically with the following command:
+
+
+```shell
+$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
+```
+
 
 ## Documentation
 
 *Please install the following version dependencies when send error: ['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']*
```

### Comparing `dtalarm-1.0.3/setup.py` & `dtalarm-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,18 @@
     desc = f.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='dtalarm',
-    version='1.0.3',
+    version='1.1.0',
     author='TimeAshore',
     author_email='timeashore@163.com',
-    description='Dtalarm for digital transformer',
+    description='Python integration with DRIVE',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

### Comparing `dtalarm-1.0.3/dtalarm.egg-info/PKG-INFO` & `dtalarm-1.1.0/dtalarm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dtalarm
-Version: 1.0.3
-Summary: Dtalarm for digital transformer
+Version: 1.1.0
+Summary: Python integration with DRIVE
 Home-page: UNKNOWN
 Author: TimeAshore
 Author-email: timeashore@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -25,62 +25,69 @@
 
 
 ```shell
 $ pip install dtalarm
 ```
 
 
-## Dependencies
-
-
-Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
-
-You can install all dependencies automatically with the following command:
-
-
-```shell
-$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
-```
-
-
 ## Usage
 
-Register a new service on the DRIVE server and get a unique secret_key.
+Register a new service on the DRIVE server and get the secret key.
 
 
 The `DTAlarmConfig` module records the configuration information required to send alarms. Here, you need to configure a server address.
 
 ```python
 from dtalarm import DTAlarmConfig
 
 DTAlarmConfig.SERVER = ""
 ```
 
+Generating alarms is very easy if the service is pre-configured, the following case will send alarms to the preset receivers. 
+```python
+from dtalarm import Alarm
+
+alarm = Alarm(secret_key="")
+alarm.title = "Title"
+```
+
+If the service is not pre-configured, alarms can also be sent in the following way:
 
 Import the `TeamsChannelAlarm` class or the `TeamsPersonalAlarm` class from the package and configure the secret_key property.
 
-After you initialize an object, you can assign a value to the alarm object. If the alarm content is a dataframe, please use the to_json method and assign it to the table property.
+After initialize, you can assign a value to the alarm object. If the alarm content is a dataframe, please use the to_json method and assign it to the table property.
 ```python
 from dtalarm import TeamsChannelAlarm
 
 alarm = TeamsChannelAlarm(secret_key="", channel_address="", template="message_only_v1")
 
 alarm.title = "Title"
 alarm.text = "Content"
 alarm.table = df.to_json()
 ```
 
 
-Finally, use the send function to send the alarm, it will return the response, timeout property: (optional) how many seconds to wait for the server to send data
-        before giving up, as a float or tuple.
+Finally call the send function to send, which can receive parameters supported by requests like timeout (how many seconds to wait for the server response). 
 
 ```python
 response = alarm.send()
 ```
 
 
+## Dependencies
+
+
+Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
+
+You can install all dependencies automatically with the following command:
+
+
+```shell
+$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
+```
+
 
 ## Documentation
 
 *Please install the following version dependencies when send error: ['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']*
```

### Comparing `dtalarm-1.0.3/dtalarm/client.py` & `dtalarm-1.1.0/dtalarm/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 dtalarm.client
 ------------------
 
 This module contains the create of Dtalarm' teams alarm.
 """
 import requests
 from plotly.graph_objs._figure import Figure
+import mimetypes
 
 from .base import BaseCli
 from .config import DTAlarmConfig
 
 
 class TeamsChannelAlarm(BaseCli):
 
@@ -95,25 +96,26 @@
         if self.status_buttons:
             payload["data"]["status_buttons"] = self.status_buttons
         if self.additional_functions is not None:
             payload["data"]["additional_functions"] = self.additional_functions
 
         return payload
 
-    def send(self, timeout=None):
+    def send(self, **kwargs):
         """
         :param timeout: (optional) How many seconds to wait for the server to send data
         before giving up, as a float, or a :ref:`(connect timeout, read timeout) <timeouts>` tuple.
         :return: :class:`Response <Response>` object
         """
         payload = self._gen_kwargs()
-        kwarg = {"json": payload}
-        if timeout is not None:
-            kwarg.update({"timeout": timeout})
-        response = requests.post(DTAlarmConfig.SERVER, **kwarg)
+        kwargs.update({
+            "json": payload
+        })
+
+        response = requests.post(DTAlarmConfig.SERVER, **kwargs)
         return response
 
 
 class TeamsPersonalAlarm(BaseCli):
 
     def __init__(self, secret_key=None, accepter=None, template=None):
         super(TeamsPersonalAlarm, self).__init__()
@@ -217,7 +219,203 @@
         payload = self._gen_kwargs()
         kwargs.update({
             "json": payload
         })
 
         response = requests.post(DTAlarmConfig.SERVER, **kwargs)
         return response
+
+
+class Alarm(BaseCli):
+
+    def __init__(self, secret_key=None):
+        super(Alarm, self).__init__()
+        self.secret_key = secret_key
+
+        self.table = None
+        self.attachment = []
+        self.attachment_from_file = []
+
+    def _argsparser(self):
+        """
+        Parse the parameters assigned to the alarm object.
+
+        The attribute in the images list must be a plotly figure object.
+        Accepter need to be a list, and the maximum number cannot exceed 10.
+        :return:
+        """
+
+        for figure in self.images:
+            if isinstance(figure, Figure) is False:
+                raise Exception("Images should be a plotly graph object list.")
+
+    def attachment_upload(self, bytes_or_fp_buffer):
+        """
+
+        :param fp_bytes:
+        :return:
+        """
+        files = {
+            'file': bytes_or_fp_buffer
+        }
+
+        # obtain the DRIVE server address due to historical reasons...
+        ServerAddress = DTAlarmConfig.SERVER.split('/alarm')[0]
+
+        res = requests.post(f'{ServerAddress}{DTAlarmConfig.ATTACHMENT_UPLOAD_ROUTE}', files=files)
+
+        if res.json()['status'] is not True:
+            raise Exception(res.json())
+        return res.json()["data"]["key"]
+
+    def _attach_files(self) -> list:
+        """
+        Upload attachment and record the key meta information.
+
+        :return: [{
+                    "key": "s3 key",
+                    "filename": ""
+                }]
+        """
+        attachment_meta = []
+
+        memory_meta = self._upload_attachment_from_memory()
+        local_file_meta = self._upload_attachment_from_file()
+
+        attachment_meta.extend(memory_meta)
+        attachment_meta.extend(local_file_meta)
+
+        return attachment_meta
+
+    def _upload_attachment_from_memory(self) -> list:
+        """
+        Upload objects in memory.
+        :return:
+        """
+        attachment_meta = []
+
+        for dic in self.attachment:
+            key = self.attachment_upload(dic["file"])
+
+            attachment_meta.append({
+                "key": key,
+                "filename": dic.get("filename", key),
+            })
+
+        return attachment_meta
+
+    def _upload_attachment_from_file(self) -> list:
+        """
+        Upload local file.
+        :return:
+        """
+        attachment_meta = []
+
+        for filename in self.attachment_from_file:
+            fp = open(filename, 'rb')
+            key = self.attachment_upload(fp)
+
+            attachment_meta.append({
+                "key": key,
+                "filename": filename,
+            })
+
+        return attachment_meta
+
+    def _gen_alarm_payload(self):
+        """
+        Generate a request body with the template message+image_v2.
+
+        # New format of the Email alarm.
+        {
+            "secret_key": self.secret_key,
+            "presetting": True,
+            # "platform": "teams",
+            # "platform_subitem": "personal",
+            "data": {
+                # "accepter": "",
+                # "template": "message+image_v2",
+                "content": {
+                    "alarm_title": self.title,
+                    "message_title": self.message_title,
+                    "message_text": self.message_text,
+                    "image_base64": [
+                    ],
+                    "buttons": self.buttons,
+                    "table": self.table.to_json(),
+                    "table_h5": self.table.to_html(),
+                    "alarm_type": self.type,
+
+                    "attachment": [{
+                        "key": "",
+                        "filename": ""
+                    }]
+                },
+                "additional_functions": self.additional_functions,
+                "status_buttons": self.status_buttons,
+                "severity": self.severity
+            }
+        }
+
+        :return:
+        """
+
+        self._argsparser()
+        payload = {
+            "secret_key": self.secret_key,
+            "presetting": True,
+            "data": {
+                "content": {}
+            }
+        }
+
+        # fill data.content
+        if self.title:
+            payload["data"]["content"]["alarm_title"] = self.title
+        if self.message_title:
+            payload["data"]["content"]["message_title"] = self.message_title
+        if self.message_text:
+            payload["data"]["content"]["message_text"] = self.message_text
+
+        if self.images:
+            images = self._compression_img(self.images)
+            payload["data"]["content"]["image_base64"] = images
+
+        if self.buttons:
+            payload["data"]["content"]["buttons"] = self.buttons
+
+        if self.table is not None:
+            payload["data"]["content"]["table"] = self.table.to_json()
+            payload["data"]["content"]["table_h5"] = self.table.to_html(index=False)
+
+        if self.type:
+            payload["data"]["content"]["alarm_type"] = self.type
+
+        # add attachment information if any
+        if self.attachment or self.attachment_from_file:
+            attachment_meta = self._attach_files()
+            payload["data"]["content"]["attachment"] = attachment_meta
+
+        # fill data.*
+        if self.severity is not None:
+            payload["data"]["severity"] = self.severity
+        if self.status_buttons:
+            payload["data"]["status_buttons"] = self.status_buttons
+        if self.additional_functions is not None:
+            payload["data"]["additional_functions"] = self.additional_functions
+
+        return payload
+
+    def send(self, **kwargs):
+        """
+        :param timeout: (optional) How many seconds to wait for the server to send data
+        before giving up, as a float, or a :ref:`(connect timeout, read timeout) <timeouts>` tuple.
+        :return: :class:`Response <Response>` object
+        """
+
+        payload = self._gen_alarm_payload()
+        kwargs.update({
+            "json": payload
+        })
+
+        response = requests.post(DTAlarmConfig.SERVER, **kwargs)
+        return response
```

### Comparing `dtalarm-1.0.3/dtalarm/base.py` & `dtalarm-1.1.0/dtalarm/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # encoding: utf-8
 """
 dtalarm.base
 ------------------
 
 This module contains the base functions of Dtalarm' teams alarm.
 """
-
+from base64 import b64encode
+import plotly.graph_objects as go
 import base64
 import io
 import os
 import time
 from PIL import Image
-from base64 import b64encode
-import plotly.graph_objects as go
 
 
 class BaseCli:
 
     def __init__(self):
         self.compress_img = True
```

