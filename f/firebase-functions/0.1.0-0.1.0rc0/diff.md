# Comparing `tmp/firebase_functions-0.1.0.tar.gz` & `tmp/firebase_functions-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firebase_functions-0.1.0.tar", last modified: Tue May  9 22:17:01 2023, max compression
+gzip compressed data, was "firebase_functions-0.1.0rc0.tar", last modified: Fri Apr 28 23:59:43 2023, max compression
```

## Comparing `firebase_functions-0.1.0.tar` & `firebase_functions-0.1.0rc0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:17:01.773080 firebase_functions-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-09 22:17:01.773080 firebase_functions-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:17:01.773080 firebase_functions-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:17:01.769080 firebase_functions-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:17:01.769080 firebase_functions-0.1.0/src/firebase_functions/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:17:01.773080 firebase_functions-0.1.0/src/firebase_functions/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/alerts/app_distribution_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/alerts/billing_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/alerts/crashlytics_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/alerts/performance_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/db_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/firestore_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/https_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    37994 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:17:01.773080 firebase_functions-0.1.0/src/firebase_functions/private/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/private/_alerts_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/private/_identity_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/private/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/private/path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/private/serving.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/private/token_verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/private/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/storage_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/src/firebase_functions/test_lab_fn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:17:01.769080 firebase_functions-0.1.0/src/firebase_functions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-09 22:17:01.000000 firebase_functions-0.1.0/src/firebase_functions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-09 22:17:01.000000 firebase_functions-0.1.0/src/firebase_functions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:17:01.000000 firebase_functions-0.1.0/src/firebase_functions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-09 22:17:01.000000 firebase_functions-0.1.0/src/firebase_functions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 22:17:01.000000 firebase_functions-0.1.0/src/firebase_functions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:17:01.773080 firebase_functions-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_eventarc_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_pubsub_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_remote_config_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_scheduler_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_tasks_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_test_lab_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-09 22:16:27.000000 firebase_functions-0.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.483568 firebase_functions-0.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 23:59:43.483568 firebase_functions-0.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:59:43.483568 firebase_functions-0.1.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.475568 firebase_functions-0.1.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/src/firebase_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/app_distribution_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/billing_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/crashlytics_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts/performance_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/db_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/firestore_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/https_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37728 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/src/firebase_functions/private/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/_alerts_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/_identity_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/token_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/private/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/storage_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/src/firebase_functions/test_lab_fn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 23:59:43.000000 firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:59:43.479568 firebase_functions-0.1.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_eventarc_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_pubsub_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_remote_config_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_scheduler_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_tasks_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_test_lab_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-28 23:59:14.000000 firebase_functions-0.1.0rc0/tests/test_util.py
```

### Comparing `firebase_functions-0.1.0/LICENSE` & `firebase_functions-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/PKG-INFO` & `firebase_functions-0.1.0rc0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebase_functions
-Version: 0.1.0
+Version: 0.1.0rc0
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.1.0/setup.py` & `firebase_functions-0.1.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/__init__.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Firebase Functions for Python.
 """
 
-__version__ = "0.1.0"
+__version__ = "0.1.0rc0"
```

### Comparing `firebase_functions-0.1.0/src/firebase_functions/alerts/__init__.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/alerts/app_distribution_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/app_distribution_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/alerts/billing_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/billing_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/alerts/crashlytics_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/crashlytics_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/alerts/performance_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts/performance_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/alerts_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/alerts_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/core.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/core.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/db_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/db_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/eventarc_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/eventarc_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/firestore_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/firestore_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/https_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/https_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/identity_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/identity_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/options.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,42 +309,35 @@
             "vpc_connector",
             "vpc_connector_egress_settings",
         ]
         if not preserve_external_changes:
             for option in resettable_options:
                 if option not in merged_options:
                     merged_options[option] = RESET_VALUE
-
-        if self.secrets and not self.secrets == _util.Sentinel:
-
-            def convert_secret(secret) -> str:
-                secret_value = secret
-                if isinstance(secret, SecretParam):
-                    secret_value = secret.name
-                return secret_value
-
-            merged_options["secrets"] = list(
-                map(convert_secret, _typing.cast(list, self.secrets)))
         # _util.Sentinel values are converted to `None` in ManifestEndpoint generation
         # after other None values are removed - so as to keep them in the generated
         # YAML output as 'null' values.
         return merged_options
 
     def _endpoint(self, **kwargs) -> _manifest.ManifestEndpoint:
         assert kwargs["func_name"] is not None
         options_dict = self._asdict_with_global_options()
         options = self.__class__(**options_dict)
+
         secret_envs: list[
             _manifest.SecretEnvironmentVariable] | _util.Sentinel = []
         if options.secrets is not None:
             if isinstance(options.secrets, list):
 
                 def convert_secret(
                         secret) -> _manifest.SecretEnvironmentVariable:
-                    return {"key": secret}
+                    secret_value = secret
+                    if isinstance(secret, SecretParam):
+                        secret_value = secret.name
+                    return {"key": secret_value}
 
                 secret_envs = list(
                     map(convert_secret, _typing.cast(list, options.secrets)))
             elif options.secrets is _util.Sentinel:
                 secret_envs = _typing.cast(_util.Sentinel, options.secrets)
 
         region: list[str] | None = None
@@ -837,15 +830,15 @@
 @_dataclasses.dataclass(frozen=True, kw_only=True)
 class StorageOptions(RuntimeOptions):
     """
     Options specific to Storage function types.
     Internal use only.
     """
 
-    bucket: str | Expression[str] | None = None
+    bucket: str | None = None
     """
     The name of the bucket to watch for Storage events.
     """
 
     def _endpoint(
         self,
         **kwargs,
```

### Comparing `firebase_functions-0.1.0/src/firebase_functions/params.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,114 +13,94 @@
 # limitations under the License.
 """Module for params that can make Cloud Functions codebases generic."""
 
 import abc as _abc
 import dataclasses as _dataclasses
 import os as _os
 import re as _re
-import enum as _enum
 import typing as _typing
 
 _T = _typing.TypeVar("_T", str, int, float, bool, list)
 
 
 @_dataclasses.dataclass(frozen=True)
 class Expression(_abc.ABC, _typing.Generic[_T]):
     """
     A CEL expression which can be evaluated during function deployment, and
     resolved to a value of the generic type parameter: i.e, you can pass
     an Expression<number> as the value of an option that normally accepts numbers.
     """
 
-    def __cel__(self, expression: str):
-        object.__setattr__(self, "_cel_", expression)
-
-    def __str__(self):
-        return f"{{{{ {self._cel_} }}}}"
-
-    @property
     def value(self) -> _T:
         """
         Returns the Expression's runtime value, based on the CLI's resolution of params.
         """
         raise NotImplementedError()
 
-
-def _obj_cel_name(obj: _T) -> _T:
-    return obj if not isinstance(obj, Expression) else object.__getattribute__(
-        obj, "_cel_")
+    def to_cel(self) -> str:
+        """
+        Returns the Expression's representation as a braced CEL expression.
+        """
+        return f"{{{{ {self} }}}}"
 
 
 def _quote_if_string(literal: _T) -> _T:
-    return _obj_cel_name(literal) if not isinstance(literal,
-                                                    str) else f'"{literal}"'
+    return literal if not isinstance(literal, str) else f'"{literal}"'
 
 
 _params: dict[str, Expression] = {}
 
 
 @_dataclasses.dataclass(frozen=True)
 class TernaryExpression(Expression[_T], _typing.Generic[_T]):
-    """
-    A CEL expression that evaluates to one of two values based on the value of
-    another expression.
-    """
     test: Expression[bool]
     if_true: _T
     if_false: _T
 
-    def __post_init__(self):
-        test_str = _obj_cel_name(self.test)
-        true_str = _quote_if_string(self.if_true)
-        false_str = _quote_if_string(self.if_false)
-        expression = f"{test_str} ? {true_str} : {false_str}"
-        super().__cel__(expression)
-
-    @property
     def value(self) -> _T:
-        return self.if_true if self.test.value else self.if_false
+        return self.if_true if self.test.value() else self.if_false
+
+    def __str__(self) -> str:
+        return f"{self.test} ? {_quote_if_string(self.if_true)} : {_quote_if_string(self.if_false)}"
 
 
 @_dataclasses.dataclass(frozen=True)
 class CompareExpression(Expression[bool], _typing.Generic[_T]):
     """
     A CEL expression that evaluates to boolean true or false based on a comparison
     between the value of another expression and a literal of that same type.
     """
     comparator: str
     left: Expression[_T]
     right: _T
 
-    def __post_init__(self):
-        super().__cel__(
-            f"{_obj_cel_name(self.left)} {self.comparator} {_quote_if_string(self.right)}"
-        )
-
-    @property
     def value(self) -> bool:
-        left: _T = self.left.value
+        left: _T = self.left.value()
         if self.comparator == "==":
             return left == self.right
         elif self.comparator == ">":
             return left > self.right
         elif self.comparator == ">=":
             return left >= self.right
         elif self.comparator == "<":
             return left < self.right
         elif self.comparator == "<=":
             return left <= self.right
         else:
             raise ValueError(f"Unknown comparator {self.comparator}")
 
+    def __str__(self) -> str:
+        return f"{self.left} {self.comparator} {_quote_if_string(self.right)}"
+
     def then(self, if_true: _T, if_false: _T) -> TernaryExpression[_T]:
         return TernaryExpression(self, if_true, if_false)
 
 
 @_dataclasses.dataclass(frozen=True)
-class SelectOption(_typing.Generic[_T]):
+class SelectOptions(_typing.Generic[_T]):
     """
     A representation of an option that can be selected via a SelectInput.
     """
 
     value: _T
     """The value of the option."""
 
@@ -131,15 +111,15 @@
 @_dataclasses.dataclass(frozen=True)
 class SelectInput(_typing.Generic[_T]):
     """
     Specifies that a Param's value should be determined by having the user select
     from a list of pre-canned options interactively at deploy-time.
     """
 
-    options: list[SelectOption[_T]]
+    options: list[SelectOptions[_T]]
     """A list of user selectable options."""
 
 
 @_dataclasses.dataclass(frozen=True)
 class TextInput:
     """
     Specifies that a Param's value should be determined by prompting the user
@@ -160,28 +140,23 @@
 
     validation_error_message: str | None = None
     """
     An error message that is displayed to the user if validation_regex fails.
     """
 
 
-class ResourceType(str, _enum.Enum):
-    """The type of resource that a picker should pick."""
-    STORAGE_BUCKET = "storage.googleapis.com/Bucket"
-
-
 @_dataclasses.dataclass(frozen=True)
 class ResourceInput:
     """
     Specifies that a Param's value should be determined by having the user
     select from a list containing all the project's resources of a certain
     type. Currently, only type:"storage.googleapis.com/Bucket" is supported.
     """
 
-    type: ResourceType | str
+    type: str
     """
     The resource type. Currently, only type:"storage.googleapis.com/Bucket" is supported.
     """
 
 
 @_dataclasses.dataclass(frozen=True)
 class Param(Expression[_T]):
@@ -190,15 +165,15 @@
     """
 
     name: str
     """
     The environment variable of this parameter. Must be upper case.
     """
 
-    default: _T | Expression[_T] | None = None
+    default: _T | None = None
     """
     The default value to assign to this param if none provided.
     """
 
     label: str | None = None
     """
     A label that is displayed to the user for this param.
@@ -211,31 +186,32 @@
 
     immutable: bool | None = None
     """
     Whether the value of this parameter can change between function
     deployments.
     """
 
-    input: TextInput | ResourceInput | SelectInput[_T] | None = None
+    input: TextInput | ResourceInput | SelectInput[_T] = TextInput()
     """
     The type of input that is required for this param, e.g. TextInput.
     """
 
-    @property
     def value(self) -> _T:
         raise NotImplementedError()
 
     def compare(self, compare: str, right: _T) -> CompareExpression:
         return CompareExpression(compare, self, right)
 
     def equals(self, right: _T) -> CompareExpression:
         return self.compare("==", right)
 
+    def __str__(self) -> str:
+        return f"params.{self.name}"
+
     def __post_init__(self):
-        super().__cel__(f"params.{self.name}")
         if isinstance(self, _DefaultStringParam):
             return
         if not _re.match(r"^[A-Z0-9_]+$", self.name):
             raise ValueError(
                 "Parameter names must only use uppercase letters, numbers and "
                 "underscores, e.g. 'UPPER_SNAKE_CASE'.")
         if self.name in _params:
@@ -268,27 +244,28 @@
 
     immutable: bool | None = None
     """
     Whether the value of this parameter can change between function
     deployments.
     """
 
+    def __str__(self):
+        return f"params.{self.name}"
+
     def __post_init__(self):
-        super().__cel__(f"params.{self.name}")
         if not _re.match(r"^[A-Z0-9_]+$", self.name):
             raise ValueError(
                 "Parameter names must only use uppercase letters, numbers and "
                 "underscores, e.g. 'UPPER_SNAKE_CASE'.")
         if self.name in _params:
             raise ValueError(
                 f"Duplicate Parameter Error: The parameter '{self.name}' has already been declared."
             )
         _params[self.name] = self
 
-    @property
     def value(self) -> str:
         """Current value of this parameter."""
         return _os.environ.get(self.name, "")
 
     def compare(self, compare: str, right: _T) -> CompareExpression:
         return CompareExpression(compare, self, right)
 
@@ -296,70 +273,78 @@
         return self.compare("==", right)
 
 
 @_dataclasses.dataclass(frozen=True)
 class StringParam(Param[str]):
     """A parameter as a string value."""
 
-    @property
     def value(self) -> str:
         if _os.environ.get(self.name) is not None:
             return _os.environ[self.name]
 
         if self.default is not None:
-            return self.default.value if isinstance(
-                self.default, Expression) else self.default
+            return self.default
 
         return str()
 
 
 @_dataclasses.dataclass(frozen=True)
 class IntParam(Param[int]):
     """A parameter as a int value."""
 
-    @property
     def value(self) -> int:
         if _os.environ.get(self.name) is not None:
             return int(_os.environ[self.name])
         if self.default is not None:
-            return self.default.value if isinstance(
-                self.default, Expression) else self.default
+            return self.default
         return int()
 
 
 @_dataclasses.dataclass(frozen=True)
 class FloatParam(Param[float]):
     """A parameter as a float value."""
 
-    @property
     def value(self) -> float:
         if _os.environ.get(self.name) is not None:
             return float(_os.environ[self.name])
         if self.default is not None:
-            return self.default.value if isinstance(
-                self.default, Expression) else self.default
+            return self.default
         return float()
 
 
 @_dataclasses.dataclass(frozen=True)
 class BoolParam(Param[bool]):
     """A parameter as a bool value."""
 
-    @property
     def value(self) -> bool:
         env_value = _os.environ.get(self.name)
         if env_value is not None:
-            return env_value.lower() == "true"
+            if env_value.lower() in ["true", "t", "1", "y", "yes"]:
+                return True
+            if env_value.lower() in ["false", "f", "0", "n", "no"]:
+                return False
+            raise ValueError(f"Invalid value for {self.name}: {env_value}")
         if self.default is not None:
-            return self.default.value if isinstance(
-                self.default, Expression) else self.default
+            return self.default
         return False
 
 
 @_dataclasses.dataclass(frozen=True)
+class ListParam(Param[list]):
+    """A parameter as a list of strings."""
+
+    def value(self) -> list[str]:
+        if _os.environ.get(self.name) is not None:
+            return list(filter(len, _os.environ[self.name].split(",")))
+        if self.default is not None:
+            return self.default
+        return []
+
+
+@_dataclasses.dataclass(frozen=True)
 class _DefaultStringParam(StringParam):
     """
     Internal use only.
     This is a parameter that is available by default in all functions.
     These are excluded from the list of parameters that are prompted to the user.
     """
```

### Comparing `firebase_functions-0.1.0/src/firebase_functions/private/__init__.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/__init__.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/private/_alerts_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/_alerts_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/private/_identity_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/_identity_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/private/manifest.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,89 +176,52 @@
     specVersion: str = "v1alpha1"
     params: list[_typing.Any] | None = _dataclasses.field(
         default_factory=list[_typing.Any])
     requiredAPIs: list[ManifestRequiredApi] = _dataclasses.field(
         default_factory=list[ManifestRequiredApi])
 
 
-def _param_input_to_spec(
-    param_input: _params.TextInput | _params.ResourceInput | _params.SelectInput
-) -> dict[str, _typing.Any]:
-    if isinstance(param_input, _params.TextInput):
-        return {
-            "text": {
-                key: value for key, value in {
-                    "example":
-                        param_input.example,
-                    "validationRegex":
-                        param_input.validation_regex,
-                    "validationErrorMessage":
-                        param_input.validation_error_message,
-                }.items() if value is not None
-            }
-        }
-
-    if isinstance(param_input, _params.ResourceInput):
-        return {
-            "resource": {
-                "type": param_input.type,
-            },
-        }
-
-    if isinstance(param_input, _params.SelectInput):
-        return {
-            "select": {
-                "options": [{
-                    key: value for key, value in {
-                        "value": option.value,
-                        "label": option.label,
-                    }.items() if value is not None
-                } for option in param_input.options],
-            },
-        }
-
-    return {}
-
-
 def _param_to_spec(
         param: _params.Param | _params.SecretParam) -> dict[str, _typing.Any]:
     spec_dict: dict[str, _typing.Any] = {
         "name": param.name,
         "label": param.label,
         "description": param.description,
         "immutable": param.immutable,
     }
 
     if isinstance(param, _params.Param):
-        spec_dict["default"] = f"{param.default}" if isinstance(
-            param.default, _params.Expression) else param.default
-        if param.input:
-            spec_dict["input"] = _param_input_to_spec(param.input)
+        spec_dict["default"] = param.default
+        # TODO spec representation of inputs
 
     if isinstance(param, _params.BoolParam):
         spec_dict["type"] = "boolean"
     elif isinstance(param, _params.IntParam):
         spec_dict["type"] = "int"
     elif isinstance(param, _params.FloatParam):
         spec_dict["type"] = "float"
     elif isinstance(param, _params.SecretParam):
         spec_dict["type"] = "secret"
+    elif isinstance(param, _params.ListParam):
+        spec_dict["type"] = "list"
+        if spec_dict["default"] is not None:
+            spec_dict["default"] = ",".join(spec_dict["default"])
     elif isinstance(param, _params.StringParam):
         spec_dict["type"] = "string"
     else:
         raise NotImplementedError("Unsupported param type.")
 
     return _dict_to_spec(spec_dict)
 
 
 def _object_to_spec(data) -> object:
     if isinstance(data, _Enum):
         return data.value
     elif isinstance(data, _params.Expression):
-        return f"{data}"
+        return data.to_cel()
     elif _dataclasses.is_dataclass(data):
         return _dataclass_to_spec(data)
     elif isinstance(data, list):
         return list(map(_object_to_spec, data))
     elif isinstance(data, dict):
         return _dict_to_spec(data)
     else:
```

### Comparing `firebase_functions-0.1.0/src/firebase_functions/private/path_pattern.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/private/serving.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/serving.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/private/token_verifier.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/token_verifier.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/private/util.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/private/util.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/pubsub_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/pubsub_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/remote_config_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/remote_config_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/scheduler_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/scheduler_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/storage_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/storage_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/tasks_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/tasks_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/src/firebase_functions/test_lab_fn.py` & `firebase_functions-0.1.0rc0/src/firebase_functions/test_lab_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
             results_uri=event_data["resultStorage"]["resultsUri"],
             gcs_path=event_data["resultStorage"]["gcsPath"],
             tool_results_execution=event_data["resultStorage"].get(
                 "toolResultsExecution"),
         ),
         client_info=ClientInfo(
             client=event_data["clientInfo"]["client"],
-            details=event_data["clientInfo"].get("details", {}),
+            details=event_data["clientInfo"]["details"],
         ),
         test_matrix_id=event_data["testMatrixId"],
     )
 
     event: CloudEvent[TestMatrixCompletedData] = CloudEvent(
         data=test_lab_data,
         id=event_dict["id"],
```

### Comparing `firebase_functions-0.1.0/src/firebase_functions.egg-info/PKG-INFO` & `firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebase-functions
-Version: 0.1.0
+Version: 0.1.0rc0
 Summary: Firebase Functions Python SDK
 Home-page: https://github.com/firebase/firebase-functions-python
 Author: Firebase Team
 License: Apache License 2.0
 Keywords: firebase,functions,google,cloud
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `firebase_functions-0.1.0/src/firebase_functions.egg-info/SOURCES.txt` & `firebase_functions-0.1.0rc0/src/firebase_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/tests/test_eventarc_fn.py` & `firebase_functions-0.1.0rc0/tests/test_eventarc_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/tests/test_manifest.py` & `firebase_functions-0.1.0rc0/tests/test_manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,51 +64,49 @@
     endpoints={"test": full_endpoint},
     params=[
         _params.BoolParam("BOOL_TEST", default=False),
         _params.IntParam("INT_TEST", description="int_description"),
         _params.FloatParam("FLOAT_TEST", immutable=True),
         _params.SecretParam("SECRET_TEST"),
         _params.StringParam("STRING_TEST"),
+        _params.ListParam("LIST_TEST", default=["1", "2", "3"]),
     ],
     requiredAPIs=[{
         "api": "test_api",
         "reason": "testing"
-    }],
-)
+    }])
 
 full_stack_dict = {
     "specVersion": "v1alpha1",
     "endpoints": {
         "test": full_endpoint_dict
     },
-    "params": [
-        {
-            "name": "BOOL_TEST",
-            "type": "boolean",
-            "default": False,
-        },
-        {
-            "name": "INT_TEST",
-            "type": "int",
-            "description": "int_description"
-        },
-        {
-            "name": "FLOAT_TEST",
-            "type": "float",
-            "immutable": True,
-        },
-        {
-            "name": "SECRET_TEST",
-            "type": "secret"
-        },
-        {
-            "name": "STRING_TEST",
-            "type": "string"
-        },
-    ],
+    "params": [{
+        "name": "BOOL_TEST",
+        "type": "boolean",
+        "default": False,
+    }, {
+        "name": "INT_TEST",
+        "type": "int",
+        "description": "int_description"
+    }, {
+        "name": "FLOAT_TEST",
+        "type": "float",
+        "immutable": True,
+    }, {
+        "name": "SECRET_TEST",
+        "type": "secret"
+    }, {
+        "name": "STRING_TEST",
+        "type": "string"
+    }, {
+        "default": "1,2,3",
+        "name": "LIST_TEST",
+        "type": "list"
+    }],
     "requiredAPIs": [{
         "api": "test_api",
         "reason": "testing"
     }]
 }
```

### Comparing `firebase_functions-0.1.0/tests/test_options.py` & `firebase_functions-0.1.0rc0/tests/test_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     """
     Test Param or Expression option values are converted to their
     CEL values for manifest representation.
     """
     int_param = params.IntParam("MIN")
     https_options_dict = options.HttpsOptions(
         min_instances=int_param)._asdict_with_global_options()
-    assert https_options_dict[
-        "min_instances"] == f"{int_param}", "param was not converted to CEL string"
+    assert https_options_dict["min_instances"] == int_param.to_cel(
+    ), "param was not converted to CEL string"
 
 
 def test_options_preserve_external_changes():
     """
     Testing if setting a global option internally change the values.
     """
     assert (options._GLOBAL_OPTIONS.preserve_external_changes
```

### Comparing `firebase_functions-0.1.0/tests/test_params.py` & `firebase_functions-0.1.0rc0/tests/test_params.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,154 +20,201 @@
 
 class TestBoolParams:
     """BoolParam unit tests."""
 
     def test_bool_param_value_true_or_false(self):
         """Testing if bool params correctly returns a true or false value."""
         bool_param = params.BoolParam("BOOL_VALUE_TEST1")
-        for value_true, value_false in zip(["true"],
-                                           ["false", "anything", "else"]):
+        for value_true, value_false in zip(["true", "t", "1", "y", "yes"],
+                                           ["false", "f", "0", "n", "no"]):
             environ["BOOL_VALUE_TEST1"] = value_true
-            assert (bool_param.value is True), "Failure, params returned False"
+            assert (bool_param.value()
+                    is True), "Failure, params returned False"
             environ["BOOL_VALUE_TEST1"] = value_false
-            assert (bool_param.value is False), "Failure, params returned True"
+            assert (bool_param.value()
+                    is False), "Failure, params returned True"
+
+    def test_bool_param_value_error(self):
+        """Testing if bool params throws a value error if invalid value."""
+        with pytest.raises(ValueError):
+            environ["BOOL_VALUE_TEST2"] = "bad_value"
+            params.BoolParam("BOOL_VALUE_TEST2").value()
 
     def test_bool_param_empty_default(self):
         """Testing if bool params defaults to False if no value and no default."""
-        assert (params.BoolParam("BOOL_DEFAULT_TEST").value
+        assert (params.BoolParam("BOOL_DEFAULT_TEST").value()
                 is False), "Failure, params returned True"
 
     def test_bool_param_default(self):
         """Testing if bool params defaults to provided default value."""
-        assert (params.BoolParam("BOOL_DEFAULT_TEST_FALSE", default=False).value
+        assert (params.BoolParam("BOOL_DEFAULT_TEST_FALSE",
+                                 default=False).value()
                 is False), "Failure, params returned True"
-        assert (params.BoolParam("BOOL_DEFAULT_TEST_TRUE", default=True).value
+        assert (params.BoolParam("BOOL_DEFAULT_TEST_TRUE",
+                                 default=True).value()
                 is True), "Failure, params returned False"
 
     def test_bool_param_equality(self):
         """Test bool equality."""
         assert (params.BoolParam("BOOL_TEST1",
-                                 default=False).equals(False).value
+                                 default=False).equals(False).value()
                 is True), "Failure, equality check returned False"
-        assert (params.BoolParam("BOOL_TEST2", default=True).equals(False).value
+        assert (params.BoolParam("BOOL_TEST2",
+                                 default=True).equals(False).value()
                 is False), "Failure, equality check returned False"
 
 
 class TestFloatParams:
     """FloatParam unit tests."""
 
     def test_float_param_value(self):
         """Testing if float params correctly returns a value."""
         environ["FLOAT_VALUE_TEST"] = "123.456"
-        assert params.FloatParam("FLOAT_VALUE_TEST",).value == 123.456, \
+        assert params.FloatParam("FLOAT_VALUE_TEST",).value() == 123.456, \
             "Failure, params value != 123.456"
 
     def test_float_param_empty_default(self):
         """Testing if float params defaults to empty float if no value and no default."""
-        assert params.FloatParam("FLOAT_DEFAULT_TEST1").value == float(), \
+        assert params.FloatParam("FLOAT_DEFAULT_TEST1").value() == float(), \
             "Failure, params value is not float"
 
     def test_float_param_default(self):
         """Testing if float param defaults to provided default value."""
         assert params.FloatParam("FLOAT_DEFAULT_TEST2",
-        default=float(456.789)).value == 456.789, \
+        default=float(456.789)).value() == 456.789, \
             "Failure, params default value != 456.789"
 
     def test_float_param_equality(self):
         """Test float equality."""
         assert (params.FloatParam("FLOAT_TEST1",
-                                  default=123.456).equals(123.456).value
+                                  default=123.456).equals(123.456).value()
                 is True), "Failure, equality check returned False"
         assert (params.FloatParam("FLOAT_TEST2",
-                                  default=456.789).equals(123.456).value
+                                  default=456.789).equals(123.456).value()
                 is False), "Failure, equality check returned False"
 
 
 class TestIntParams:
     """IntParam unit tests."""
 
     def test_int_param_value(self):
         """Testing if int param correctly returns a value."""
         environ["INT_VALUE_TEST"] = "123"
         assert params.IntParam(
-            "INT_VALUE_TEST").value == 123, "Failure, params value != 123"
+            "INT_VALUE_TEST").value() == 123, "Failure, params value != 123"
 
     def test_int_param_empty_default(self):
         """Testing if int param defaults to empty int if no value and no default."""
-        assert params.IntParam("INT_DEFAULT_TEST1").value == int(
+        assert params.IntParam("INT_DEFAULT_TEST1").value() == int(
         ), "Failure, params value is not int"
 
     def test_int_param_default(self):
         """Testing if int param defaults to provided default value."""
-        assert params.IntParam("INT_DEFAULT_TEST2", default=456).value == 456, \
+        assert params.IntParam("INT_DEFAULT_TEST2", default=456).value() == 456, \
             "Failure, params default value != 456"
 
     def test_int_param_equality(self):
         """Test int equality."""
-        assert (params.IntParam("INT_TEST1", default=123).equals(123).value
+        assert (params.IntParam("INT_TEST1", default=123).equals(123).value()
                 is True), "Failure, equality check returned False"
-        assert (params.IntParam("INT_TEST2", default=456).equals(123).value
+        assert (params.IntParam("INT_TEST2", default=456).equals(123).value()
                 is False), "Failure, equality check returned False"
 
 
 class TestStringParams:
     """StringParam unit tests."""
 
     def test_string_param_value(self):
         """Testing if string param correctly returns a value."""
         environ["STRING_VALUE_TEST"] = "STRING_TEST"
-        assert params.StringParam("STRING_VALUE_TEST").value == "STRING_TEST", \
+        assert params.StringParam("STRING_VALUE_TEST").value() == "STRING_TEST", \
             'Failure, params value != "STRING_TEST"'
 
     def test_param_name_upper_snake_case(self):
         """Testing if param names are validated to be upper snake case."""
         with pytest.raises(ValueError) as context:
             params.StringParam("lower")
         assert "UPPER_SNAKE_CASE" in str(context)
 
     def test_string_param_empty_default(self):
         """Testing if string param defaults to empty string if no value and no default."""
-        assert params.StringParam("STRING_DEFAULT_TEST1").value == str(), \
+        assert params.StringParam("STRING_DEFAULT_TEST1").value() == str(), \
             "Failure, params value is not a string"
 
     def test_string_param_default(self):
         """Testing if string param defaults to provided default value."""
         assert (params.StringParam("STRING_DEFAULT_TEST2",
-        default="string_override_default").value
+        default="string_override_default").value()
                 == "string_override_default"), \
             'Failure, params default value != "string_override_default"'
 
     def test_string_param_equality(self):
         """Test string equality."""
         assert (params.StringParam("STRING_TEST1",
-                                   default="123").equals("123").value
+                                   default="123").equals("123").value()
                 is True), "Failure, equality check returned False"
         assert (params.StringParam("STRING_TEST2",
-                                   default="456").equals("123").value
+                                   default="456").equals("123").value()
+                is False), "Failure, equality check returned False"
+
+
+class TestListParams:
+    """ListParam unit tests."""
+
+    def test_list_param_value(self):
+        """Testing if list param correctly returns list values."""
+        environ["LIST_VALUE_TEST1"] = "item1,item2"
+        assert params.ListParam("LIST_VALUE_TEST1").value() == ["item1","item2"], \
+            'Failure, params value != ["item1","item2"]'
+
+    def test_list_param_filter_empty_strings(self):
+        """Testing if list param correctly returns list values wth empty strings excluded."""
+        environ["LIST_VALUE_TEST2"] = ",,item1,item2,,,item3,"
+        assert params.ListParam("LIST_VALUE_TEST2").value() == ["item1","item2", "item3"], \
+            'Failure, params value != ["item1","item2", "item3"]'
+
+    def test_list_param_empty_default(self):
+        """Testing if list param defaults to an empty list if no value and no default."""
+        assert params.ListParam("LIST_DEFAULT_TEST1").value() == [], \
+            "Failure, params value is not an empty list"
+
+    def test_list_param_default(self):
+        """Testing if list param defaults to the provided default value."""
+        assert (params.ListParam("LIST_DEFAULT_TEST2", default=["1", "2"]).value()
+                == ["1", "2"]), \
+            'Failure, params default value != ["1", "2"]'
+
+    def test_list_param_equality(self):
+        """Test list equality."""
+        assert (params.ListParam("LIST_TEST1",
+                                 default=["123"]).equals(["123"]).value()
+                is True), "Failure, equality check returned False"
+        assert (params.ListParam("LIST_TEST2",
+                                 default=["456"]).equals(["123"]).value()
                 is False), "Failure, equality check returned False"
 
 
 class TestParamsManifest:
     """
     Tests any created params are tracked for the purposes
     of outputting to the generated manifest.
     """
 
     def test_params_stored(self):
         """Testing if params are internally stored."""
         environ["TEST_STORING"] = "TEST_STORING_VALUE"
         param = params.StringParam("TEST_STORING")
-        assert param.value == "TEST_STORING_VALUE", \
+        assert param.value() == "TEST_STORING_VALUE", \
             'Failure, params value != "TEST_STORING_VALUE"'
         # pylint: disable=protected-access
         assert params._params["TEST_STORING"] == param, \
             "Failure, param was not stored"
 
     def test_default_params_not_stored(self):
         """Testing if default params are skipped from being stored."""
         environ["GCLOUD_PROJECT"] = "python-testing-project"
 
-        assert params.PROJECT_ID.value == "python-testing-project", \
+        assert params.PROJECT_ID.value() == "python-testing-project", \
             'Failure, params value != "python-testing-project"'
         # pylint: disable=protected-access
         assert params._params.get("GCLOUD_PROJECT") is None, \
             "Failure, default param was stored when it should not have been"
```

### Comparing `firebase_functions-0.1.0/tests/test_path_pattern.py` & `firebase_functions-0.1.0rc0/tests/test_path_pattern.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/tests/test_pubsub_fn.py` & `firebase_functions-0.1.0rc0/tests/test_pubsub_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/tests/test_remote_config_fn.py` & `firebase_functions-0.1.0rc0/tests/test_remote_config_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/tests/test_scheduler_fn.py` & `firebase_functions-0.1.0rc0/tests/test_scheduler_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/tests/test_tasks_fn.py` & `firebase_functions-0.1.0rc0/tests/test_tasks_fn.py`

 * *Files identical despite different names*

### Comparing `firebase_functions-0.1.0/tests/test_test_lab_fn.py` & `firebase_functions-0.1.0rc0/tests/test_test_lab_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
                     "gcsPath":
                         "gs://bucket/path/to/somewhere",
                     "toolResultsExecution":
                         "projects/123/histories/456/executions/789",
                 },
                 "clientInfo": {
                     "client": "gcloud",
+                    "details": {
+                        "someKey": "someValue",
+                    },
                 },
                 "testMatrixId": "testmatrix-123",
             })
 
         _event_handler(func, raw_event)
 
         func.assert_called_once()
```

### Comparing `firebase_functions-0.1.0/tests/test_util.py` & `firebase_functions-0.1.0rc0/tests/test_util.py`

 * *Files identical despite different names*

