# Comparing `tmp/pollination-streamlit-0.5.3.tar.gz` & `tmp/pollination-streamlit-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-streamlit-0.5.3.tar", last modified: Mon Apr  3 17:56:09 2023, max compression
+gzip compressed data, was "dist/pollination-streamlit-0.5.4.tar", last modified: Wed May 10 17:40:18 2023, max compression
```

## Comparing `pollination-streamlit-0.5.3.tar` & `pollination-streamlit-0.5.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/pollination_streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/pollination_streamlit/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/api/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/api/recipes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/api/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/interactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/pollination_streamlit/selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/pollination_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/pollination_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/pollination_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/pollination_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/pollination_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/pollination_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:56:09.000000 pollination-streamlit-0.5.3/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/assets/artifact-list.json
--rw-r--r--   0 runner    (1001) docker     (123)    29209 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/assets/job-pollination-api.json
--rw-r--r--   0 runner    (1001) docker     (123)    65739 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/assets/recipe-pollination-api.json
--rw-r--r--   0 runner    (1001) docker     (123)    41840 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/assets/run-pollination-api.json
--rw-r--r--   0 runner    (1001) docker     (123)   178730 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/assets/run-results.json
--rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-03 17:54:54.000000 pollination-streamlit-0.5.3/tests/test_interactors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/pollination_streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/pollination_streamlit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/api/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/api/recipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/api/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/interactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/pollination_streamlit/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/pollination_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-10 17:40:17.000000 pollination-streamlit-0.5.4/pollination_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/pollination_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:40:17.000000 pollination-streamlit-0.5.4/pollination_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 17:40:17.000000 pollination-streamlit-0.5.4/pollination_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 17:40:17.000000 pollination-streamlit-0.5.4/pollination_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:40:18.000000 pollination-streamlit-0.5.4/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/assets/artifact-list.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29209 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/assets/job-pollination-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65739 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/assets/recipe-pollination-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41840 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/assets/run-pollination-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)   178730 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/assets/run-results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-10 17:38:43.000000 pollination-streamlit-0.5.4/tests/test_interactors.py
```

### Comparing `pollination-streamlit-0.5.3/.devcontainer/Dockerfile` & `pollination-streamlit-0.5.4/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/.devcontainer/devcontainer.json` & `pollination-streamlit-0.5.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/.github/workflows/ci.yaml` & `pollination-streamlit-0.5.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/.github/workflows/tests.yaml` & `pollination-streamlit-0.5.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/.gitignore` & `pollination-streamlit-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/LICENSE` & `pollination-streamlit-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/PKG-INFO` & `pollination-streamlit-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-streamlit
-Version: 0.5.3
+Version: 0.5.4
 Summary: A Pollination extension to facilitate working with Pollination in Streamlit apps.
 Home-page: https://github.com/pollination/pollination-streamlit
 Author: Pollination
 Author-email: info@pollination.cloud
 License: Apache-2.0 License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pollination-streamlit-0.5.3/README.md` & `pollination-streamlit-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit/api/client.py` & `pollination-streamlit-0.5.4/pollination_streamlit/api/client.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit/api/jobs.py` & `pollination-streamlit-0.5.4/pollination_streamlit/api/jobs.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit/api/runs.py` & `pollination-streamlit-0.5.4/pollination_streamlit/api/runs.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit/authentication.py` & `pollination-streamlit-0.5.4/pollination_streamlit/authentication.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import requests
 import streamlit as st
 
 COOKIE_NAME = os.getenv('COOKIE_NAME', 'pollination-authz')
 PROXY_URL = os.getenv('PROXY_URL', 'http://localhost:8000')
 
 
-@st.cache(allow_output_mutation=True)
+@st.cache_data
 def get_manager():
     return stx.CookieManager()
 
 
 def _decode_base64(data):
     """Decode base64, padding being optional.
```

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit/dataframe.py` & `pollination-streamlit-0.5.4/pollination_streamlit/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 class RunsDataFrame:
 
     def __init__(self, df: pd.DataFrame, meta: ColumnMeta = ColumnMeta):
         self._df = df
         self._column_meta = meta
 
     @classmethod
-    @st.cache(allow_output_mutation=True)
+    @st.cache_data
     def from_run_results(cls, data: t.List[t.List[dict]]) -> 'RunsDataFrame':
         meta = ColumnMeta()
         df = pd.DataFrame()
         for run in data:
             meta.extend_from_run_result(run)
             sub_df = pd.DataFrame(run)
             sub_df = pd.DataFrame(
```

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit/interactors.py` & `pollination-streamlit-0.5.4/pollination_streamlit/interactors.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit/selectors.py` & `pollination-streamlit-0.5.4/pollination_streamlit/selectors.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit.egg-info/PKG-INFO` & `pollination-streamlit-0.5.4/pollination_streamlit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-streamlit
-Version: 0.5.3
+Version: 0.5.4
 Summary: A Pollination extension to facilitate working with Pollination in Streamlit apps.
 Home-page: https://github.com/pollination/pollination-streamlit
 Author: Pollination
 Author-email: info@pollination.cloud
 License: Apache-2.0 License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pollination-streamlit-0.5.3/pollination_streamlit.egg-info/SOURCES.txt` & `pollination-streamlit-0.5.4/pollination_streamlit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/setup.py` & `pollination-streamlit-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/assets/job-pollination-api.json` & `pollination-streamlit-0.5.4/tests/assets/job-pollination-api.json`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/assets/recipe-pollination-api.json` & `pollination-streamlit-0.5.4/tests/assets/recipe-pollination-api.json`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/assets/run-pollination-api.json` & `pollination-streamlit-0.5.4/tests/assets/run-pollination-api.json`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/assets/run-results.json` & `pollination-streamlit-0.5.4/tests/assets/run-results.json`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/conftest.py` & `pollination-streamlit-0.5.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/test_api.py` & `pollination-streamlit-0.5.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/test_authentication.py` & `pollination-streamlit-0.5.4/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/test_dataframe.py` & `pollination-streamlit-0.5.4/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `pollination-streamlit-0.5.3/tests/test_interactors.py` & `pollination-streamlit-0.5.4/tests/test_interactors.py`

 * *Files identical despite different names*

