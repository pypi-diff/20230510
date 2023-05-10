# Comparing `tmp/kognic-base-clients-1.0.3.tar.gz` & `tmp/kognic-base-clients-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kognic-base-clients-1.0.3.tar", last modified: Fri Dec  2 10:39:54 2022, max compression
+gzip compressed data, was "kognic-base-clients-1.1.0.tar", last modified: Wed May 10 12:38:25 2023, max compression
```

## Comparing `kognic-base-clients-1.0.3.tar` & `kognic-base-clients-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 10:39:54.543114 kognic-base-clients-1.0.3/
--rw-r--r--   0 peter     (1000) peter     (1000)     1450 2022-12-02 10:39:54.543114 kognic-base-clients-1.0.3/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      848 2022-12-02 10:39:37.000000 kognic-base-clients-1.0.3/README.md
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 10:39:54.543114 kognic-base-clients-1.0.3/kognic/
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 10:39:54.543114 kognic-base-clients-1.0.3/kognic/base_clients/
--rw-r--r--   0 peter     (1000) peter     (1000)      125 2022-11-29 07:52:55.000000 kognic-base-clients-1.0.3/kognic/base_clients/__init__.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 10:39:54.543114 kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/
--rw-r--r--   0 peter     (1000) peter     (1000)      107 2022-11-11 07:45:02.000000 kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/__init__.py
--rw-r--r--   0 peter     (1000) peter     (1000)     2327 2022-11-11 07:46:26.000000 kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/download_handler.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1873 2022-11-11 09:41:15.000000 kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/file_resource_client.py
--rw-r--r--   0 peter     (1000) peter     (1000)     4902 2022-11-29 07:52:55.000000 kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/upload_handler.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1417 2022-11-11 07:45:02.000000 kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/upload_spec.py
--rw-r--r--   0 peter     (1000) peter     (1000)     5382 2022-11-11 07:46:26.000000 kognic-base-clients-1.0.3/kognic/base_clients/http_client.py
--rw-r--r--   0 peter     (1000) peter     (1000)      739 2022-11-11 07:46:26.000000 kognic-base-clients-1.0.3/kognic/base_clients/models.py
--rw-r--r--   0 peter     (1000) peter     (1000)     1236 2022-11-11 07:45:02.000000 kognic-base-clients-1.0.3/kognic/base_clients/util.py
-drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2022-12-02 10:39:54.543114 kognic-base-clients-1.0.3/kognic_base_clients.egg-info/
--rw-r--r--   0 peter     (1000) peter     (1000)     1450 2022-12-02 10:39:54.000000 kognic-base-clients-1.0.3/kognic_base_clients.egg-info/PKG-INFO
--rw-r--r--   0 peter     (1000) peter     (1000)      668 2022-12-02 10:39:54.000000 kognic-base-clients-1.0.3/kognic_base_clients.egg-info/SOURCES.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        1 2022-12-02 10:39:54.000000 kognic-base-clients-1.0.3/kognic_base_clients.egg-info/dependency_links.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        7 2022-12-02 10:39:54.000000 kognic-base-clients-1.0.3/kognic_base_clients.egg-info/namespace_packages.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       55 2022-12-02 10:39:54.000000 kognic-base-clients-1.0.3/kognic_base_clients.egg-info/requires.txt
--rw-r--r--   0 peter     (1000) peter     (1000)        7 2022-12-02 10:39:54.000000 kognic-base-clients-1.0.3/kognic_base_clients.egg-info/top_level.txt
--rw-r--r--   0 peter     (1000) peter     (1000)       38 2022-12-02 10:39:54.543114 kognic-base-clients-1.0.3/setup.cfg
--rw-r--r--   0 peter     (1000) peter     (1000)     1678 2022-11-02 13:34:00.000000 kognic-base-clients-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/flake8.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/src/kognic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.258431 kognic-base-clients-1.1.0/src/kognic/base_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/download_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/file_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/upload_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/upload_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/retry_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-10 12:38:13.000000 kognic-base-clients-1.1.0/src/kognic/base_clients/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:38:25.262431 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 12:38:25.000000 kognic-base-clients-1.1.0/src/kognic_base_clients.egg-info/top_level.txt
```

### Comparing `kognic-base-clients-1.0.3/README.md` & `kognic-base-clients-1.1.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 Python 3 library for providing a base clients for interacting with the Kognic platform
 
 # Changelog
 
 All notable changes to this library will be documented in this file
 
+
+## [1.1.0] - 2023-05-10
+
+- Failed requests will be retried in a wider range of cases than previously, including both API calls and cloud storage.
+
 ## [1.0.3] - 2022-12-02
 
 - Improve handling of network errors during file uploads. TCP and SSL timeout errors will now result in retries.
 
 ## [1.0.2] - 2022-11-01
 - Internal re-work of scene upload handling to allow uploaded bytes from other sources than files
 - Removed an unused argument from some internal methods.
```

### Comparing `kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/download_handler.py` & `kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/download_handler.py`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/file_resource_client.py` & `kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/file_resource_client.py`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.0.3/kognic/base_clients/cloud_storage/upload_spec.py` & `kognic-base-clients-1.1.0/src/kognic/base_clients/cloud_storage/upload_spec.py`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.0.3/kognic/base_clients/http_client.py` & `kognic-base-clients-1.1.0/src/kognic/base_clients/http_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 """Client for communicating with the Kognic platform."""
 import logging
 import urllib.parse
 from typing import Optional, Union
 
-import requests
+from humps import decamelize
 from kognic.auth.requests.auth_session import RequestsAuthSession
+from requests import HTTPError
 
 from kognic.base_clients import __version__
 from kognic.base_clients.models import PaginatedResponse
+from kognic.base_clients.retry_support import request_with_retry
 from kognic.base_clients.util import filter_none
 
-from humps import decamelize
-
 log = logging.getLogger(__name__)
 
 ENVELOPED_JSON_TAG = "data"
 
 
 class HttpClient:
     """Http Client dealing with auth and communication with API."""
 
-    def __init__(self, auth, host: str, auth_host: str, client_organization_id: int = None, timeout: int = 60):
+    def __init__(self, auth, host: str, auth_host: str, client_organization_id: int = None, timeout: int = 60,
+                 max_retries: int = 10):
         """
         :param auth: auth credentials, see https://developers.kognic.com/docs/kognic-auth
         :param host: override for api url
         :param auth_host: override for authentication url
-        :param client_organization_id: Overrides your users organization id. Only works with an Kognic user.
-        :param max_upload_retry_attempts: Max number of attempts to retry uploading a file to GCS.
-        :param max_upload_retry_wait_time: Max with time before retrying an upload to GCS.
+        :param client_organization_id: Overrides your users organization id. Only works with a Kognic user.
+        :param max_retries: Max number of attempts to retry uploading a file to GCS.
         :param timeout: Max time to wait for response from server.
         """
 
         self.host = host
         self._auth_req_session = RequestsAuthSession(host=auth_host, auth=auth)
         self.headers = {
             "Accept-Encoding": "gzip",
             "Accept": "application/json",
             "User-Agent": f"kognic-{decamelize(self.__class__.__name__)}/{__version__}"
         }
         self.dryrun_header = {"X-Dryrun": ""}
         self.timeout = timeout
+        self.max_retries = max_retries
 
         if client_organization_id is not None:
             self.headers["X-Organization-Id"] = str(client_organization_id)
             log.warning(
                 f"WARNING: You will now act as if you are part of organization: {client_organization_id}. "
                 f"This will not work unless you are an Kognic user."
             )
 
     @property
     def session(self):
         return self._auth_req_session.session
 
     @staticmethod
-    def _raise_on_error(resp: requests.Response) -> requests.Response:
-        try:
-            resp.raise_for_status()
-        except requests.HTTPError as exception:
-            if exception.response is not None and exception.response.status_code == 400:
-                try:
-                    message = exception.response.json()["message"]
-                except ValueError:
-                    message = exception.response.text
-                raise RuntimeError(message) from exception
-
-            raise exception from None
-        return resp
+    def _http_error_handler(exception: HTTPError) -> None:
+        """
+        Raises a RuntimeError using error details from an enveloped HTTP 400 response.
+        """
+        if exception.response is not None and exception.response.status_code == 400:
+            try:
+                message = exception.response.json()["message"]
+            except ValueError:
+                message = exception.response.text
+            raise RuntimeError(message) from exception
+        raise exception from None
 
     @staticmethod
     def _unwrap_enveloped_json(js: dict) -> Union[dict, list, PaginatedResponse]:
         if isinstance(js, list):
             return js
         elif js is not None and js.get('metadata') is not None:
             return PaginatedResponse.from_json(js)
@@ -77,55 +76,74 @@
             return js[ENVELOPED_JSON_TAG]
         return js
 
     def get(self, endpoint, **kwargs) -> dict:
         r"""Sends a GET request. Returns :class:`dict` object.
 
         :param endpoint: endpoint to be appended to `client.host`.
-        :param \*\*kwargs: Optional arguments that ``request`` takes.
+        :param \**kwargs: Optional arguments that ``request`` takes.
         :rtype: dict
         """
 
         kwargs.setdefault("headers", self.headers)
         kwargs.setdefault("timeout", self.timeout)
         url = urllib.parse.urljoin(self.host, endpoint)
-        resp = self.session.get(url, **kwargs)
-        return self._unwrap_enveloped_json(self._raise_on_error(resp).json())
+        resp = request_with_retry(self.session.get,
+                                  self.max_retries,
+                                  self.timeout,
+                                  HttpClient._http_error_handler,
+                                  url=url, **kwargs)
+        return self._unwrap_enveloped_json(resp.json())
 
     def post(self, endpoint, data=None, json=None, dryrun=False, discard_response=False, **kwargs) -> Optional[dict]:
         r"""Sends a POST request. Returns :class:`dict` object.
 
         :param endpoint: endpoint to be appended to `client.host`.
         :param data: (optional) Dictionary, list of tuples, bytes, or file-like
             object to send in the body of the :class:`Request`.
+        :param json: (optional) JSON blob to send
+        :param dryrun: (optional) Send a dry-run header with the request.
+        :param discard_response: (optional) Ignore the response and return None
         :param json: (optional) json to send in the body of the :class:`Request`.
-        :param \*\*kwargs: Optional arguments that ``request`` takes.
+        :param \**kwargs: Optional arguments that ``request`` takes.
         :rtype: dict
         """
 
         if dryrun:
             headers = {**self.headers, **self.dryrun_header}
         else:
             headers = {**self.headers}
 
         kwargs.setdefault("headers", headers)
         kwargs.setdefault("timeout", self.timeout)
-        resp = self.session.post(f"{self.host}/{endpoint}", data, filter_none(json), **kwargs)
+        resp = request_with_retry(self.session.post,
+                                  self.max_retries,
+                                  self.timeout,
+                                  HttpClient._http_error_handler,
+                                  url=f"{self.host}/{endpoint}",
+                                  data=data,
+                                  json=filter_none(json),
+                                  **kwargs)
         if discard_response:
-            self._raise_on_error(resp)
             return None
         else:
-            return self._unwrap_enveloped_json(self._raise_on_error(resp).json())
+            return self._unwrap_enveloped_json(resp.json())
 
     def put(self, endpoint, data, **kwargs) -> dict:
         r"""Sends a PUT request. Returns :class:`dict` object.
 
         :param endpoint: endpoint to be appended to `client.host`.
         :param data: (optional) Dictionary, list of tuples, bytes, or file-like
             object to send in the body of the :class:`Request`.
-        :param \*\*kwargs: Optional arguments that ``request`` takes.
+        :param \**kwargs: Optional arguments that ``request`` takes.
         :rtype: dict
         """
         kwargs.setdefault("headers", self.headers)
         kwargs.setdefault("timeout", self.timeout)
-        resp = self.session.put(f"{self.host}/{endpoint}", filter_none(data), **kwargs)
-        return self._unwrap_enveloped_json(self._raise_on_error(resp).json())
+        resp = request_with_retry(self.session.put,
+                                  self.max_retries,
+                                  self.timeout,
+                                  HttpClient._http_error_handler,
+                                  url=f"{self.host}/{endpoint}",
+                                  data=filter_none(data),
+                                  **kwargs)
+        return self._unwrap_enveloped_json(resp.json())
```

### Comparing `kognic-base-clients-1.0.3/kognic/base_clients/models.py` & `kognic-base-clients-1.1.0/src/kognic/base_clients/models.py`

 * *Files identical despite different names*

### Comparing `kognic-base-clients-1.0.3/kognic/base_clients/util.py` & `kognic-base-clients-1.1.0/src/kognic/base_clients/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import mimetypes
 import random
 from typing import Mapping
 
 from urllib3.util import parse_url, Url
 
 RETRYABLE_STATUS_CODES = [408, 429, 500, 501, 502, 503, 504, 505, 506, 507, 508, 509, 510, 511, 598, 599]
-
 GCS_SCHEME = "gs"
 
 
 def filter_none(js: dict) -> dict:
     if isinstance(js, Mapping):
         return {k: filter_none(v) for k, v in js.items() if v is not None}
     else:
@@ -24,13 +22,14 @@
 
 # https://cloud.google.com/iot/docs/how-tos/exponential-backoff
 def get_wait_time(upload_attempt: int, max_retry_wait_time: int) -> float:
     """
     Calculates the wait time before attempting another file upload or download
 
     :param upload_attempt: How many attempts to upload that have been made
+    :param max_retry_wait_time: How long to wait (max) between retries
     :return: int: The time to wait before retrying upload
     """
     initial_wait_time_seconds: int = pow(2, upload_attempt - 1)
     wait_time_seconds: float = initial_wait_time_seconds + random.random()
     wait_time_seconds: float = wait_time_seconds if wait_time_seconds < max_retry_wait_time else max_retry_wait_time
     return wait_time_seconds
```

