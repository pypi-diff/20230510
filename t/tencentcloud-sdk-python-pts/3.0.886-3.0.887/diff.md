# Comparing `tmp/tencentcloud-sdk-python-pts-3.0.886.tar.gz` & `tmp/tencentcloud-sdk-python-pts-3.0.887.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-pts-3.0.886.tar", last modified: Mon May  8 03:48:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-pts-3.0.887.tar", last modified: Tue May  9 03:11:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-pts-3.0.886.tar` & `tencentcloud-sdk-python-pts-3.0.887.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/v20210728/
--rw-r--r--   0 root         (0) root         (0)    39215 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/v20210728/pts_client.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/v20210728/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/v20210728/__init__.py
--rw-r--r--   0 root         (0) root         (0)   193898 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/v20210728/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud_sdk_python_pts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud_sdk_python_pts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud_sdk_python_pts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud_sdk_python_pts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/tencentcloud_sdk_python_pts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-08 03:48:14.000000 tencentcloud-sdk-python-pts-3.0.886/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/v20210728/
+-rw-r--r--   0 root         (0) root         (0)    39215 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/v20210728/pts_client.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/v20210728/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/v20210728/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   193898 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/v20210728/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud_sdk_python_pts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud_sdk_python_pts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud_sdk_python_pts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud_sdk_python_pts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/tencentcloud_sdk_python_pts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-09 03:11:35.000000 tencentcloud-sdk-python-pts-3.0.887/setup.cfg
```

### Comparing `tencentcloud-sdk-python-pts-3.0.886/README.rst` & `tencentcloud-sdk-python-pts-3.0.887/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/v20210728/pts_client.py` & `tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/v20210728/pts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/v20210728/errorcodes.py` & `tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/v20210728/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.886/tencentcloud/pts/v20210728/models.py` & `tencentcloud-sdk-python-pts-3.0.887/tencentcloud/pts/v20210728/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.886/tencentcloud/__init__.py` & `tencentcloud-sdk-python-pts-3.0.887/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.886'
+__version__ = '3.0.887'
```

### Comparing `tencentcloud-sdk-python-pts-3.0.886/PKG-INFO` & `tencentcloud-sdk-python-pts-3.0.887/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-pts
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Pts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-pts-3.0.886/tencentcloud_sdk_python_pts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-pts-3.0.887/tencentcloud_sdk_python_pts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-pts
-Version: 3.0.886
+Version: 3.0.887
 Summary: Tencent Cloud Pts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-pts-3.0.886/setup.py` & `tencentcloud-sdk-python-pts-3.0.887/setup.py`

 * *Files identical despite different names*

