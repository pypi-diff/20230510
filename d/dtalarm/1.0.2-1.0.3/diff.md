# Comparing `tmp/dtalarm-1.0.2.tar.gz` & `tmp/dtalarm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtalarm-1.0.2.tar", last modified: Mon Jun 27 14:45:34 2022, max compression
+gzip compressed data, was "dist/dtalarm-1.0.3.tar", last modified: Wed Nov  9 01:22:34 2022, max compression
```

## Comparing `dtalarm-1.0.2.tar` & `dtalarm-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-06-27 14:45:34.856683 dtalarm-1.0.2/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1078 2021-10-28 11:22:29.000000 dtalarm-1.0.2/LICENSE
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     2067 2022-06-27 14:45:34.856324 dtalarm-1.0.2/PKG-INFO
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1452 2022-06-27 14:26:47.000000 dtalarm-1.0.2/README.md
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-06-27 14:45:34.854050 dtalarm-1.0.2/dtalarm/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      112 2022-06-27 07:57:50.000000 dtalarm-1.0.2/dtalarm/__init__.py
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)    10717 2022-06-27 08:02:34.000000 dtalarm-1.0.2/dtalarm/base.py
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     7570 2022-06-27 08:02:31.000000 dtalarm-1.0.2/dtalarm/client.py
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      181 2022-06-27 08:02:31.000000 dtalarm-1.0.2/dtalarm/config.py
-drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-06-27 14:45:34.855967 dtalarm-1.0.2/dtalarm.egg-info/
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     2067 2022-06-27 14:45:34.000000 dtalarm-1.0.2/dtalarm.egg-info/PKG-INFO
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      252 2022-06-27 14:45:34.000000 dtalarm-1.0.2/dtalarm.egg-info/SOURCES.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        1 2022-06-27 14:45:34.000000 dtalarm-1.0.2/dtalarm.egg-info/dependency_links.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       88 2022-06-27 14:45:34.000000 dtalarm-1.0.2/dtalarm.egg-info/requires.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        8 2022-06-27 14:45:34.000000 dtalarm-1.0.2/dtalarm.egg-info/top_level.txt
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       38 2022-06-27 14:45:34.856793 dtalarm-1.0.2/setup.cfg
--rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1265 2022-06-27 10:13:06.000000 dtalarm-1.0.2/setup.py
+drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-11-09 01:22:34.000000 dtalarm-1.0.3/
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     2218 2022-11-09 01:22:34.000000 dtalarm-1.0.3/PKG-INFO
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1078 2022-11-07 06:57:24.000000 dtalarm-1.0.3/LICENSE
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1584 2022-11-07 06:57:24.000000 dtalarm-1.0.3/README.md
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     1228 2022-11-07 06:57:24.000000 dtalarm-1.0.3/setup.py
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       38 2022-11-09 01:22:34.000000 dtalarm-1.0.3/setup.cfg
+drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-11-09 01:22:34.000000 dtalarm-1.0.3/dtalarm.egg-info/
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     2218 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/PKG-INFO
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      252 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/SOURCES.txt
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)       51 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/requires.txt
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        8 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/top_level.txt
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        1 2022-11-09 01:22:33.000000 dtalarm-1.0.3/dtalarm.egg-info/dependency_links.txt
+drwxr-xr-x   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)        0 2022-11-09 01:22:34.000000 dtalarm-1.0.3/dtalarm/
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      181 2022-11-07 06:57:24.000000 dtalarm-1.0.3/dtalarm/config.py
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)     7517 2022-11-07 06:57:24.000000 dtalarm-1.0.3/dtalarm/client.py
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)      112 2022-11-07 06:57:24.000000 dtalarm-1.0.3/dtalarm/__init__.py
+-rw-r--r--   0 danyanliu (1506875890) TESLAMOTORS\Domain Users (334330370)    10717 2022-11-07 06:57:24.000000 dtalarm-1.0.3/dtalarm/base.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dtalarm-1.0.2/LICENSE` & `dtalarm-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dtalarm-1.0.2/PKG-INFO` & `dtalarm-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: dtalarm
-Version: 1.0.2
+Version: 1.0.3
 Summary: Dtalarm for digital transformer
+Home-page: UNKNOWN
 Author: TimeAshore
 Author-email: timeashore@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -33,15 +34,15 @@
 
 Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
 
 You can install all dependencies automatically with the following command:
 
 
 ```shell
-$ pip install dtalarm['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']
+$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
 ```
 
 
 ## Usage
 
 Register a new service on the DRIVE server and get a unique secret_key.
 
@@ -76,9 +77,10 @@
 response = alarm.send()
 ```
 
 
 
 ## Documentation
 
+*Please install the following version dependencies when send error: ['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']*
```

### Comparing `dtalarm-1.0.2/README.md` & `dtalarm-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
 
 You can install all dependencies automatically with the following command:
 
 
 ```shell
-$ pip install dtalarm['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']
+$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
 ```
 
 
 ## Usage
 
 Register a new service on the DRIVE server and get a unique secret_key.
 
@@ -57,7 +57,8 @@
 response = alarm.send()
 ```
 
 
 
 ## Documentation
 
+*Please install the following version dependencies when send error: ['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']*
```

### Comparing `dtalarm-1.0.2/dtalarm/base.py` & `dtalarm-1.0.3/dtalarm/base.py`

 * *Files identical despite different names*

### Comparing `dtalarm-1.0.2/dtalarm/client.py` & `dtalarm-1.0.3/dtalarm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,20 +204,20 @@
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
+        kwargs.update({
+            "json": payload
+        })
 
-        response = requests.post(DTAlarmConfig.SERVER, **kwarg)
+        response = requests.post(DTAlarmConfig.SERVER, **kwargs)
         return response
```

### Comparing `dtalarm-1.0.2/dtalarm.egg-info/PKG-INFO` & `dtalarm-1.0.3/dtalarm.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: dtalarm
-Version: 1.0.2
+Version: 1.0.3
 Summary: Dtalarm for digital transformer
+Home-page: UNKNOWN
 Author: TimeAshore
 Author-email: timeashore@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -33,15 +34,15 @@
 
 Dtalarm supports CPython 3.6.8+, PyPy, and PyPy3.6.8+.
 
 You can install all dependencies automatically with the following command:
 
 
 ```shell
-$ pip install dtalarm['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']
+$ pip install dtalarm['Pillow', 'requests', 'kaleido', 'plotly', 'numpy', 'pandas']
 ```
 
 
 ## Usage
 
 Register a new service on the DRIVE server and get a unique secret_key.
 
@@ -76,9 +77,10 @@
 response = alarm.send()
 ```
 
 
 
 ## Documentation
 
+*Please install the following version dependencies when send error: ['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']*
```

### Comparing `dtalarm-1.0.2/setup.py` & `dtalarm-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     desc = f.read()
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='dtalarm',
-    version='1.0.2',
+    version='1.0.3',
     author='TimeAshore',
     author_email='timeashore@163.com',
     description='Dtalarm for digital transformer',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
@@ -28,9 +28,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6.8',
-    install_requires=['Pillow==8.4.0', 'requests==2.27.1', 'kaleido==0.2.1', 'plotly==5.9.0', 'numpy==1.19.5', 'pandas==1.1.5']
+    install_requires=['Pillow', 'requests', 'kaleido>=0.2.1', 'plotly', 'numpy', 'pandas']
 )
```

