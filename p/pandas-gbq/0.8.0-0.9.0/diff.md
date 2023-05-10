# Comparing `tmp/pandas-gbq-0.8.0.tar.gz` & `tmp/pandas-gbq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pandas-gbq-0.8.0.tar", last modified: Mon Nov 12 09:07:25 2018, max compression
+gzip compressed data, was "dist/pandas-gbq-0.9.0.tar", last modified: Fri Jan 11 17:52:19 2019, max compression
```

## Comparing `pandas-gbq-0.8.0.tar` & `pandas-gbq-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 swast    (212416) eng       (5000)        0 2018-11-12 09:07:25.000000 pandas-gbq-0.8.0/
--rw-r--r--   0 swast    (212416) eng       (5000)     2561 2018-11-12 09:07:25.000000 pandas-gbq-0.8.0/PKG-INFO
-drwxr-xr-x   0 swast    (212416) eng       (5000)        0 2018-11-12 09:07:25.000000 pandas-gbq-0.8.0/pandas_gbq/
--rw-r--r--   0 swast    (212416) eng       (5000)    10302 2018-10-19 17:24:56.000000 pandas-gbq-0.8.0/pandas_gbq/auth.py
--rw-r--r--   0 swast    (212416) eng       (5000)      497 2018-11-12 09:07:25.000000 pandas-gbq-0.8.0/pandas_gbq/_version.py
--rw-r--r--   0 swast    (212416) eng       (5000)      260 2018-09-14 17:23:11.000000 pandas-gbq-0.8.0/pandas_gbq/__init__.py
--rw-r--r--   0 swast    (212416) eng       (5000)      260 2018-08-31 18:32:04.000000 pandas-gbq-0.8.0/pandas_gbq/exceptions.py
--rw-r--r--   0 swast    (212416) eng       (5000)     2538 2018-11-12 09:06:32.000000 pandas-gbq-0.8.0/pandas_gbq/load.py
--rw-r--r--   0 swast    (212416) eng       (5000)    39190 2018-11-12 09:06:32.000000 pandas-gbq-0.8.0/pandas_gbq/gbq.py
--rw-r--r--   0 swast    (212416) eng       (5000)      844 2018-08-31 18:32:04.000000 pandas-gbq-0.8.0/pandas_gbq/schema.py
-drwxr-xr-x   0 swast    (212416) eng       (5000)        0 2018-11-12 09:07:25.000000 pandas-gbq-0.8.0/pandas_gbq.egg-info/
--rw-r--r--   0 swast    (212416) eng       (5000)     2561 2018-11-12 09:07:23.000000 pandas-gbq-0.8.0/pandas_gbq.egg-info/PKG-INFO
--rw-r--r--   0 swast    (212416) eng       (5000)      372 2018-11-12 09:07:23.000000 pandas-gbq-0.8.0/pandas_gbq.egg-info/SOURCES.txt
--rw-r--r--   0 swast    (212416) eng       (5000)      102 2018-11-12 09:07:23.000000 pandas-gbq-0.8.0/pandas_gbq.egg-info/requires.txt
--rw-r--r--   0 swast    (212416) eng       (5000)       11 2018-11-12 09:07:23.000000 pandas-gbq-0.8.0/pandas_gbq.egg-info/top_level.txt
--rw-r--r--   0 swast    (212416) eng       (5000)        1 2018-11-12 09:07:23.000000 pandas-gbq-0.8.0/pandas_gbq.egg-info/dependency_links.txt
--rw-r--r--   0 swast    (212416) eng       (5000)      314 2018-04-10 22:36:37.000000 pandas-gbq-0.8.0/MANIFEST.in
--rw-r--r--   0 swast    (212416) eng       (5000)     1531 2018-11-12 09:06:32.000000 pandas-gbq-0.8.0/setup.py
--rw-r--r--   0 swast    (212416) eng       (5000)      362 2018-11-12 09:07:25.000000 pandas-gbq-0.8.0/setup.cfg
--rw-r--r--   0 swast    (212416) eng       (5000)    68951 2018-10-19 17:24:56.000000 pandas-gbq-0.8.0/versioneer.py
--rw-r--r--   0 swast    (212416) eng       (5000)     1325 2018-11-12 09:06:32.000000 pandas-gbq-0.8.0/README.rst
+drwxr-xr-x   0 swast    (212416) eng       (5000)        0 2019-01-11 17:52:19.000000 pandas-gbq-0.9.0/
+-rw-r--r--   0 swast    (212416) eng       (5000)     2561 2019-01-11 17:52:19.000000 pandas-gbq-0.9.0/PKG-INFO
+drwxr-xr-x   0 swast    (212416) eng       (5000)        0 2019-01-11 17:52:19.000000 pandas-gbq-0.9.0/pandas_gbq/
+-rw-r--r--   0 swast    (212416) eng       (5000)     3657 2019-01-04 17:04:49.000000 pandas-gbq-0.9.0/pandas_gbq/auth.py
+-rw-r--r--   0 swast    (212416) eng       (5000)      497 2019-01-11 17:52:19.000000 pandas-gbq-0.9.0/pandas_gbq/_version.py
+-rw-r--r--   0 swast    (212416) eng       (5000)      260 2018-09-14 17:23:11.000000 pandas-gbq-0.9.0/pandas_gbq/__init__.py
+-rw-r--r--   0 swast    (212416) eng       (5000)      260 2018-08-31 18:32:04.000000 pandas-gbq-0.9.0/pandas_gbq/exceptions.py
+-rw-r--r--   0 swast    (212416) eng       (5000)     2538 2018-11-12 09:06:32.000000 pandas-gbq-0.9.0/pandas_gbq/load.py
+-rw-r--r--   0 swast    (212416) eng       (5000)    39915 2018-12-20 18:21:59.000000 pandas-gbq-0.9.0/pandas_gbq/gbq.py
+-rw-r--r--   0 swast    (212416) eng       (5000)      844 2018-08-31 18:32:04.000000 pandas-gbq-0.9.0/pandas_gbq/schema.py
+drwxr-xr-x   0 swast    (212416) eng       (5000)        0 2019-01-11 17:52:19.000000 pandas-gbq-0.9.0/pandas_gbq.egg-info/
+-rw-r--r--   0 swast    (212416) eng       (5000)     2561 2019-01-11 17:52:18.000000 pandas-gbq-0.9.0/pandas_gbq.egg-info/PKG-INFO
+-rw-r--r--   0 swast    (212416) eng       (5000)      372 2019-01-11 17:52:18.000000 pandas-gbq-0.9.0/pandas_gbq.egg-info/SOURCES.txt
+-rw-r--r--   0 swast    (212416) eng       (5000)      121 2019-01-11 17:52:18.000000 pandas-gbq-0.9.0/pandas_gbq.egg-info/requires.txt
+-rw-r--r--   0 swast    (212416) eng       (5000)       11 2019-01-11 17:52:18.000000 pandas-gbq-0.9.0/pandas_gbq.egg-info/top_level.txt
+-rw-r--r--   0 swast    (212416) eng       (5000)        1 2019-01-11 17:52:18.000000 pandas-gbq-0.9.0/pandas_gbq.egg-info/dependency_links.txt
+-rw-r--r--   0 swast    (212416) eng       (5000)      314 2018-04-10 22:36:37.000000 pandas-gbq-0.9.0/MANIFEST.in
+-rw-r--r--   0 swast    (212416) eng       (5000)     1557 2018-12-20 17:41:15.000000 pandas-gbq-0.9.0/setup.py
+-rw-r--r--   0 swast    (212416) eng       (5000)      362 2019-01-11 17:52:19.000000 pandas-gbq-0.9.0/setup.cfg
+-rw-r--r--   0 swast    (212416) eng       (5000)    68951 2018-10-19 17:24:56.000000 pandas-gbq-0.9.0/versioneer.py
+-rw-r--r--   0 swast    (212416) eng       (5000)     1325 2018-11-12 09:06:32.000000 pandas-gbq-0.9.0/README.rst
```

### Comparing `pandas-gbq-0.8.0/PKG-INFO` & `pandas-gbq-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-gbq
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pandas interface to Google BigQuery
 Home-page: https://github.com/pydata/pandas-gbq
 Author: The PyData Development Team
 Author-email: pydata@googlegroups.com
 License: BSD License
 Description: pandas-gbq
         ==========
```

### Comparing `pandas-gbq-0.8.0/pandas_gbq/load.py` & `pandas-gbq-0.9.0/pandas_gbq/load.py`

 * *Files identical despite different names*

### Comparing `pandas-gbq-0.8.0/pandas_gbq/gbq.py` & `pandas-gbq-0.9.0/pandas_gbq/gbq.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,30 @@
 
 from pandas_gbq.exceptions import AccessDenied
 
 logger = logging.getLogger(__name__)
 
 BIGQUERY_INSTALLED_VERSION = None
 SHOW_VERBOSE_DEPRECATION = False
+SHOW_PRIVATE_KEY_DEPRECATION = False
+PRIVATE_KEY_DEPRECATION_MESSAGE = (
+    "private_key is deprecated and will be removed in a future version."
+    "Use the credentials argument instead. See "
+    "https://pandas-gbq.readthedocs.io/en/latest/howto/authentication.html "
+    "for examples on using the credentials argument with service account keys."
+)
 
 try:
     import tqdm  # noqa
 except ImportError:
     tqdm = None
 
 
 def _check_google_client_version():
-    global BIGQUERY_INSTALLED_VERSION, SHOW_VERBOSE_DEPRECATION
+    global BIGQUERY_INSTALLED_VERSION, SHOW_VERBOSE_DEPRECATION, SHOW_PRIVATE_KEY_DEPRECATION
 
     try:
         import pkg_resources
 
     except ImportError:
         raise ImportError("Could not import pkg_resources (setuptools).")
 
@@ -49,19 +56,30 @@
     pandas_installed_version = pkg_resources.get_distribution(
         "pandas"
     ).parsed_version
     pandas_version_wo_verbosity = pkg_resources.parse_version("0.23.0")
     SHOW_VERBOSE_DEPRECATION = (
         pandas_installed_version >= pandas_version_wo_verbosity
     )
+    pandas_version_with_credentials_arg = pkg_resources.parse_version("0.24.0")
+    SHOW_PRIVATE_KEY_DEPRECATION = (
+        pandas_installed_version >= pandas_version_with_credentials_arg
+    )
 
 
 def _test_google_api_imports():
 
     try:
+        import pydata_google_auth
+    except ImportError as ex:
+        raise ImportError(
+            "pandas-gbq requires pydata-google-auth: {0}".format(ex)
+        )
+
+    try:
         from google_auth_oauthlib.flow import InstalledAppFlow  # noqa
     except ImportError as ex:
         raise ImportError(
             "pandas-gbq requires google-auth-oauthlib: {0}".format(ex)
         )
 
     try:
@@ -282,15 +300,14 @@
         self,
         project_id,
         reauth=False,
         private_key=None,
         auth_local_webserver=False,
         dialect="legacy",
         location=None,
-        try_credentials=None,
         credentials=None,
     ):
         global context
         from google.api_core.exceptions import GoogleAPIError
         from google.api_core.exceptions import ClientError
         from pandas_gbq import auth
 
@@ -298,30 +315,28 @@
         self.project_id = project_id
         self.location = location
         self.reauth = reauth
         self.private_key = private_key
         self.auth_local_webserver = auth_local_webserver
         self.dialect = dialect
         self.credentials = credentials
-        self.credentials_path = _get_credentials_file()
         default_project = None
 
         # Load credentials from cache.
         if not self.credentials:
             self.credentials = context.credentials
             default_project = context.project
 
         # Credentials were explicitly asked for, so don't use the cache.
         if private_key or reauth or not self.credentials:
             self.credentials, default_project = auth.get_credentials(
                 private_key=private_key,
                 project_id=project_id,
                 reauth=reauth,
                 auth_local_webserver=auth_local_webserver,
-                try_credentials=try_credentials,
             )
 
         if self.project_id is None:
             self.project_id = default_project
 
         if self.project_id is None:
             raise ValueError(
@@ -620,18 +635,14 @@
         table = _Table(
             self.project_id, dataset_id, credentials=self.credentials
         )
         table.delete(table_id)
         table.create(table_id, table_schema)
 
 
-def _get_credentials_file():
-    return os.environ.get("PANDAS_GBQ_CREDENTIALS_FILE")
-
-
 def _parse_schema(schema_fields):
     # see:
     # http://pandas.pydata.org/pandas-docs/dev/missing_data.html
     # #missing-data-casting-rules-and-indexing
     dtype_map = {
         "FLOAT": np.dtype(float),
         "TIMESTAMP": "datetime64[ns]",
@@ -801,14 +812,19 @@
             "verbose is deprecated and will be removed in "
             "a future version. Set logging level in order to vary "
             "verbosity",
             FutureWarning,
             stacklevel=2,
         )
 
+    if private_key is not None and SHOW_PRIVATE_KEY_DEPRECATION:
+        warnings.warn(
+            PRIVATE_KEY_DEPRECATION_MESSAGE, FutureWarning, stacklevel=2
+        )
+
     if dialect not in ("legacy", "standard"):
         raise ValueError("'{0}' is not valid for dialect".format(dialect))
 
     connector = GbqConnector(
         project_id,
         reauth=reauth,
         dialect=dialect,
@@ -965,30 +981,32 @@
             "verbose is deprecated and will be removed in "
             "a future version. Set logging level in order to vary "
             "verbosity",
             FutureWarning,
             stacklevel=1,
         )
 
+    if private_key is not None and SHOW_PRIVATE_KEY_DEPRECATION:
+        warnings.warn(
+            PRIVATE_KEY_DEPRECATION_MESSAGE, FutureWarning, stacklevel=2
+        )
+
     if if_exists not in ("fail", "replace", "append"):
         raise ValueError("'{0}' is not valid for if_exists".format(if_exists))
 
     if "." not in destination_table:
         raise NotFoundException(
             "Invalid Table Name. Should be of the form 'datasetId.tableId' "
         )
 
     connector = GbqConnector(
         project_id,
         reauth=reauth,
         auth_local_webserver=auth_local_webserver,
         location=location,
-        # Avoid reads when writing tables.
-        # https://github.com/pydata/pandas-gbq/issues/202
-        try_credentials=lambda project, creds: creds,
         credentials=credentials,
         private_key=private_key,
     )
     dataset_id, table_id = destination_table.rsplit(".", 1)
 
     table = _Table(
         project_id,
```

### Comparing `pandas-gbq-0.8.0/pandas_gbq/schema.py` & `pandas-gbq-0.9.0/pandas_gbq/schema.py`

 * *Files identical despite different names*

### Comparing `pandas-gbq-0.8.0/pandas_gbq.egg-info/PKG-INFO` & `pandas-gbq-0.9.0/pandas_gbq.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-gbq
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pandas interface to Google BigQuery
 Home-page: https://github.com/pydata/pandas-gbq
 Author: The PyData Development Team
 Author-email: pydata@googlegroups.com
 License: BSD License
 Description: pandas-gbq
         ==========
```

### Comparing `pandas-gbq-0.8.0/setup.py` & `pandas-gbq-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     with open("README.rst") as f:
         return f.read()
 
 
 INSTALL_REQUIRES = [
     "setuptools",
     "pandas",
+    "pydata-google-auth",
     "google-auth",
     "google-auth-oauthlib",
     "google-cloud-bigquery>=0.32.0",
 ]
 
 extras = {"tqdm": "tqdm>=4.23.0"}
```

### Comparing `pandas-gbq-0.8.0/versioneer.py` & `pandas-gbq-0.9.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `pandas-gbq-0.8.0/README.rst` & `pandas-gbq-0.9.0/README.rst`

 * *Files identical despite different names*

